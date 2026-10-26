# Nature of Genius 213 Intelligence Has Many Forms

<https://www.youtube.com/watch?v=9qCVD1LLQwc>

Bu video (**"System Design for Beginners Course"** by freeCodeCamp / NeetCode), ölçeklenebilir ve yüksek performanslı sistemler tasarlamak için kullanılan temel kavramları adım adım inceler.

Önemli başlıklar ve detaylı açıklamaları aşağıda listelenmiştir:

### 1. Vertical vs. Horizontal Scaling

- **Vertical Scaling (Scaling Up):** Mevcut sunucunun donanım kapasitesini (CPU, RAM, SSD) artırmaktır.

  - *Artıları:* Yönetimi ve uygulaması kolaydır; mimari değişiklik gerektirmez.
  - *Eksileri:* Donanımsal bir üst sınır (hardware limit) vardır ve maliyet yüksek seviyelerde üssel (exponential) artar. *Single Point of Failure (SPOF)* riski taşır.
- **Horizontal Scaling (Scaling Out):** Sisteme daha fazla sunucu (instance) ekleyerek yükü dağıtmaktır.

  - *Artıları:* Teorik olarak sınırsız ölçeklenme sağlar, yüksek erişilebilirlik (High Availability) sunar.
  - *Eksileri:* **Load Balancer** kullanımı, **Data Consistency** ve durumu olmayan (Stateless) mimari yönetimi gibi ek karmaşıklıklar getirir.

### 2. Load Balancing (Yük Dengelenmesi)

- **Tanım:** Gelen ağ trafiğini arka plandaki (backend) sunucu havuzuna dağıtan yapıdır.
- **Algoritmalar:**

  - **Round Robin:** İstekleri sırayla sunuculara dağıtır.
  - **Weighted Round Robin:** Sunucu kapasitelerine göre ağırlık vererek dağıtım yapar.
  - **Least Connections:** O an en az aktif bağlantıya sahip sunucuya yönlendirir.
  - **IP Hash:** Kullanıcının IP adresine göre istekleri hep aynı sunucuya yönlendirir (Session Persistence / Sticky Sessions için kullanışlıdır).
- **Konumlandırma:** Client →\rightarrow→ Load Balancer →\rightarrow→ Web Server →\rightarrow→ Load Balancer →\rightarrow→ Database şeklinde birden fazla katmanda kullanılabilir.

### 3. Caching (Önbellekleme)

- **Amacı:** Sık erişilen verileri hızlı erişilebilir (RAM tabanlı) depolama alanlarında tutarak veritabanı yükünü düşürmek ve **Latency** değerini azaltmaktır (Örn: Redis, Memcached).
- **Cache Eviction Policies (Önbellek Temizleme Stratejileri):**

  - **LRU (Least Recently Used):** En uzun süredir erişilmeyen veriyi siler.
  - **LFU (Least Frequently Used):** En az erişim sayısına sahip veriyi siler.
  - **FIFO (First In First Out):** İlk giren veriyi ilk çıkarır.
- **Cache Caching Strategies / Write Patterns:**

  - **Cache-Aside (Read-Through):** Uygulama veriyi önce cache'te arar; yoksa DB'den okuyup cache'e yazar.
  - **Write-Through:** Veri aynı anda hem cache'e hem DB'ye yazılır.
  - **Write-Back (Write-Behind):** Veri önce cache'e yazılır, DB'ye asenkron olarak arka planda aktarılır (Yüksek performans sağlar ama veri kaybı riski vardır).

### 4. Content Delivery Network (CDN)

- Coğrafi olarak dağıtılmış bir sunucu ağıdır.
- Görseller, videolar, CSS/JS dosyaları gibi **Static Assets** içerikleri kullanıcının fiziksel konumuna en yakın sunucudan (**Edge Server**) sunarak gecikmeyi (latency) minimize eder.

### 5. Databases: Relational (SQL) vs. Non-Relational (NoSQL)

- **Relational Databases (SQL - Postgres, MySQL):**

  - Tablo tabanlıdır, katı bir şema (schema) gerektirir.
  - **ACID** (Atomicity, Consistency, Isolation, Durability) garantisi sunar.
  - Finansal işlemler ve ilişkisel veriler için idealdir.
- **NoSQL Databases (MongoDB, Cassandra, DynamoDB):**

  - Key-Value, Document, Columnar veya Graph yapısında esnek şemasız veriler tutar.
  - Horizontal Scaling için çok daha uygundur.
  - Esnek veri yapıları ve devasa ölçekteki okuma/yazma yükleri için kullanılır.

### 6. Database Scaling & Optimization Techniques

- **Database Replication:**

  - **Primary / Replica (Master / Slave):** Yazma işlemleri yalnızca Primary DB'ye yapılır, okuma işlemleri Replica DB'lere dağıtılır. Read-heavy sistemler için idealdir.
- **Database Sharding (Horizontal Partitioning):**

  - Veritabanını **Shard Key** (Örn: `user_id`) bazında birden fazla fiziksel sunucuya bölmektir.
  - Veritabanı boyutunun tek bir sunucuya sığmadığı durumlar için kullanılır.
- **Indexing:** Okuma sorgularının performansını kat kat artırır ancak yazma (Write) işlemlerini biraz yavaşlatır.

### 7. CAP Theorem

Dağıtık sistemlerde (Distributed Systems) aynı anda yalnızca **iki** tanesinin garanti edilebileceğini belirtir:

1. **Consistency (Tutarlılık):** Tüm node'lar aynı anda aynı veriyi görür.
2. **Availability (Erişilebilirlik):** Her istek başarılı bir yanıt alır (son verinin güncel olduğu garanti edilmeyebilir).
3. **Partition Tolerance (Bölünme Toleransı):** Ağ kopukluklarına / iletişim sorunlarına rağmen sistem çalışmaya devam eder.

> Dağıtık bir sistemde ağ arızaları kaçınılmaz olduğu için genellikle tercih **CP (Consistency + Partition Tolerance)** veya **AP (Availability + Partition Tolerance)** arasında yapılır.

### 8. Asynchronous Processing & Message Queues

- Uzun süren ve eşzamansız yapılabilecek işleri (email gönderimi, video işleme) ana istek akışından (**Request-Response Cycle**) ayırmak için kullanılır.
- **Teknolojiler:** RabbitMQ, Apache Kafka, Amazon SQS.
- **Decoupling:** Servislerin birbirine sıkı sıkıya bağımlı olmasını önler (Loose Coupling) ve anlık yük artışlarını (**Traffic Spikes**) absorbe eder.

### 9. Microservices Architecture & API Gateway

- **Monolith vs. Microservices:**

  - Monolith uygulamalar tek parça halindedir, ölçeklemek ve yönetmek zamanla zorlaşır.
  - Microservices mimarisinde sistem küçük, bağımsız ve kendi veritabanına sahip servislere bölünür.
- **API Gateway:**

  - Client ile Microservice'ler arasında tek giriş noktası (Single Entry Point) olarak görev yapar.
  - **Routing**, **Authentication/Authorization**, **Rate Limiting** ve **Request Logging** gibi ortak görevleri üstlenir.

### 10. System Design Interview / Approach Steps

Örnek bir sistem tasarımı yaparken izlenmesi gereken adımlar:

1. **Requirements Clarification:** Functional & Non-Functional gereksinimleri netleştir.
2. **Estimation (Back-of-the-envelope calculations):** Trafik (RPS - Requests Per Second), depolama alanı ve band genişliği ihtiyaçlarını hesapla.
3. **High-Level Design:** Temel bileşenleri (Client, LB, Web Server, DB, Cache) blok diyagram olarak çiz.
4. **Detailed Component Design:** Bottleneck noktalarını belirle, Sharding, Replication, Caching stratejilerini detaylandır.
5. **Trade-offs:** Yapılan mimari seçimlerin artı ve eksilerini tartış.

*Başka bir bölüm veya spesifik bir kavram üzerine daha detaylı odaklanmamı istersen sormaktan çekinme!*
