# OTE Pattern Recognition Series - Vol. 14

<https://www.youtube.com/watch?v=cYzS_kFxv7M>

Bu YouTube videosundaki (**"System Design - How to design WhatsApp"**) tüm önemli ve öne çıkan noktaların detaylı, yapılandırılmış özeti aşağıdadır:

## 1. Geniş Ölçek & Gereksinimler (Requirements & Scale)

- **Ölçek (Scale):**

  - Yaklaşık **500 Milyon aktif kullanıcı** (Active Users).
  - Günlük ortalama **50 Milyar mesaj** gönderiliyor.
- **Functional Requirements (İşlevsel Gereksinimler):**

  - 1-to-1 (birebir) sohbet/mesajlaşma.
  - Grup sohbetleri (Group chats).
  - Mesaj durumları: Sent (Gönderildi), Delivered (İletildi), Read (Okundu).
  - Medya paylaşımı (Görsel, video vb.).
- **Non-Functional Requirements (İşlevsel Olmayan Gereksinimler):**

  - **Low Latency (Düşük Gecikme):** Mesajların milisaniyeler içinde iletilmesi.
  - **High Availability (Yüksek Erişilebilirlik):** Sistemin kesintisiz çalışması.
  - **No Data Loss (Veri Kaybı Yok):** Gönderilen mesajların kaybolmaması.
  - **End-to-End Encryption (Uçtan Uca Şifreleme):** Güvenlik ve gizlilik.

## 2. İletişim Protokolleri & Bağlantı Yönetimi

- **HTTP / HTTPS Neden Yetersiz?**

  - HTTP *stateless* olduğu için her istekte yeni bir bağlantı kurulumu gerektirir. Sürekli mesajlaşma için overhead (ek yük) yaratır.
- **WebSocket Protokolü:**

  - İki yönlü (**Bi-directional**), tam çift yönlü (**Full-duplex**) ve uzun ömürlü (**Persistent**) bir bağlantı sunar.
  - İstemci (Client) ve Sunucu (Server) arasında sürekli açık tutulur.
- **Gateway Server / Connection Manager:**

  - Kullanıcıların WebSocket bağlantılarını yöneten sunucu katmanıdır.
  - Hangi kullanıcının hangi Gateway Server'a bağlı olduğunu tutmak için bir **Sessions DB / Table** (örneğin Redis üzerinde) tutulur.

## 3. Birebir Mesajlaşma Akışı (1-to-1 Messaging Flow)

1. **Mesaj Gönderimi:** Kullanıcı A, mesajı WebSocket bağlantısı üzerinden kendi Gateway Server'ına iletir.
2. **Yönlendirme (Routing):**

   - Gateway Server, alıcı (Kullanıcı B) için açık bir bağlantı olup olmadığını kontrol etmek üzere **Session Service**'e sorgu atar.
3. **Senaryo A (Kullanıcı B Online ise):**

   - Kullanıcı B'nin bağlı olduğu Gateway Server bulunur.
   - Mesaj anında Kullanıcı B'ye push edilir.
   - Kullanıcı B'den alınan ACK (Acknowledgement), Kullanıcı A'ya iletilerek mesaj durumu "Delivered" yapılır.
4. **Senaryo B (Kullanıcı B Offline ise):**

   - Mesaj bir **Transient Storage / Message Queue** (geçici depolama) katmanında saklanır.
   - Kullanıcı B tekrar online olduğunda, bekleyen mesajlar sırayla cihazına indirilir ve depolamadan silinir.

## 4. Mesaj Durumu Yönetimi (Status Tracking: Sent, Delivered, Read)

- **ACK (Acknowledgement) Mekanizması:**

  - Mesaj sunucuya ulaştığında sunucu gönderene ACK döner (Tek tık / Sent).
  - Mesaj alıcının cihazına ulaştığında alıcı sunucuya ACK döner, sunucu da bunu gönderene iletir (Çift tık / Delivered).
  - Alıcı sohbet ekranını açıp mesajı okuduğunda "Read ACK" tetiklenir (Mavi tık / Read).

## 5. Grup Sohbetleri (Group Messaging Architecture)

- **Small Groups (Küçük Gruplar):**

  - WhatsApp grup limitleri sınırlı tutulduğu için mesaj, gruptaki her bir üye için ayrı ayrı kopyalanıp bağlantılarına push edilir (**Fan-out on write** veya sunucu tarafında paralel dağıtım).
- **Group Service & Metadata:**

  - Grupların üye listesi, yönetici hakları gibi bilgiler ayrı bir **Group Service / Relational DB** üzerinde tutulur.
- **Grup Mesajı Akışı:**

  1. Gönderici grup mesajını sunucuya atar.
  2. Sunucu Group Service'ten gruptaki aktif üyelerin listesini çeker.
  3. Üyelerin online durumlarına göre her birinin Gateway Server'ına mesaj yönlendirilir.

## 6. Veri Depolama ve Veritabanı Seçimleri (Database Architecture)

- **Client-Side Storage (İstemci Tarafı Depolama):**

  - WhatsApp, mesaj geçmişini kendi merkezi sunucularında uzun süreli saklamaz. Mesajlar esas olarak kullanıcıların cihazlarında (**SQLite**) depolanır.
- **Server-Side Transient Storage (Sunucu Tarafı Geçici Depolama):**

  - Yalnızca alıcısına henüz ulaşmamış (offline) mesajlar geçici olarak tutulur.
  - Bu işlem için yüksek okuma/yazma performansı sunan NoSQL sistemler (örn. **Cassandra**, **HBase** veya **Redis**) tercih edilir.
- **Media Storage (Medya Depolama):**

  - Fotoğraf, video ve ses dosyaları doğrudan ana mesaj DB'sinde tutulmaz.
  - Medya dosyaları **Object Storage (AWS S3 vb.)** üzerinde depolanır.
  - Hızlı indirme ve performans için **CDN (Content Delivery Network)** kullanılır.
  - Mesaj metni içinde yalnızca medyanın *Encrypted URL* adresi ve *Thumbnail* bilgisi taşınır.

## 7. Güvenlik: Uçtan Uca Şifreleme (End-to-End Encryption - E2EE)

- **Signal Protocol:** WhatsApp, E2EE için Signal Protokolünü kullanır.
- **Public / Private Key Pair:**

  - Her cihaz kendi Public ve Private anahtarlarını üretir. Public key sunucuya kaydedilir, Private key cihazda saklanır.
- **Şifreleme Süreci:**

  - Mesaj henüz gönderici cihazdan çıkmadan alıcının Public Key'i ile şifrelenir.
  - Sunucu (WhatsApp) mesaj içeriğini göremez, yalnızca bir "payload" olarak taşır.
  - Mesajı sadece alıcı kendi Private Key'i ile çözebilir (decrypt).

## 8. Ölçekleme ve Sistem Bileşenleri Özet Mimarısı

- **Load Balancers:** Bağlantı isteklerini Gateway Server'lara dengeli şekilde dağıtır.
- **Heartbeat Mechanism:** İstemcilerin (Mobile app) online olup olmadığını ve bağlantının kopup kopmadığını anlamak için düzenli olarak ping/pong (heartbeat) paketleri gönderilir.
- **Caching (Önbellekleme):**

  - Kullanıcı oturumları (User Sessions) ve online durumları (Last Seen / Presence Status) için **Redis** gibi in-memory cache çözümleri kullanılır.

İhtiyacınıza göre bu mimarinin belirli bir kısmını (örneğin *Signal Protocol detayları* veya *Cassandra sharding yapısı*) daha da detaylandırabiliriz!
