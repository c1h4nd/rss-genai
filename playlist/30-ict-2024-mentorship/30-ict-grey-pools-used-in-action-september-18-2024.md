# ICT Grey Pools Used In Action September 18, 2024

<https://www.youtube.com/watch?v=AxNoqk5Vx8o>

**ICT (Inner Circle Trader)** tarafından yayınlanan **"ICT Grey Pools Used In Action September 18, 2024"** başlıklı videonun detaylı Türkçe özeti:

### 📌 Video Genel Bakış ve Amaç

- **Video Başlığı:** ICT Grey Pools Used In Action (18 Eylül 2024)
- **Ana Konu:** ICT’nin 2024 Mentorship serisinde tanıttığı **"Grey Pools"** kavramının canlı/gerçek zamanlı piyasa hareketleri üzerinde nasıl kullanılacağının ve algoritmik mantığının gösterimi.
- **Kapsam:** Fiyat hareketlerini analiz ederken **PD Array** hiyerarşisi, likidite kümelenmeleri ve zaman-fiyat (**Time & Price**) ilişkisi üzerinden işlem fırsatlarının nasıl okunacağı anlatılmaktadır.

### 🔑 Temel Kavramlar ve Tanımlar

- **Grey Pools Definition:**

  - **NWOG (New Week Opening Gap)** ve **NDOG (New Day Opening Gap)** seviyelerinin veya fiyat boşluklarının (**Gap / Inefficiency**) birbirine çok yakın kümelendiği (clustering) alanlar arasında kalan bölgeye denir.
  - Algoritma, bu alanları fiyatı çekmek veya destek/direnç mantığıyla fiyatı oradan tepkiletmek için bir **Magnet (mıknatıs)** veya **PD Array (Institutional Support/Resistance)** gibi kullanır.
- **Institutional Order Flow & Algorithmic Delivery:**

  - Piyasanın rastgele hareket etmediği, tamamen **IPDA (Interbank Price Delivery Algorithm)** tarafından zaman ve fiyat hassasiyetine göre sürüldüğü vurgulanır.
  - Fiyatın belirli **PD Array**'lere dokunup dönmesi şans değil, algoritmik bir **Rebalance (Yeniden Dengeleme)** sürecidir.

### 📊 Teknik Detaylar ve Uygulama Adımları

- **Grey Pool Alanının Tes tbiti:**

  - Grafikte üst üste binen veya ardışık oluşan **NDOG / NWOG** seviyelerinin üst ve alt sınırları belirlenir.
  - Bu iki sınır arasında kalan bölge (Gap / Inefficiency alanı) bir **"Grey Pool"** olarak işaretlenir.
- **Market Structure & PD Arrays:**

  - Fiyat Grey Pool alanına girdiğinde, iç yapıdaki **Fair Value Gap (FVG)**, **Inversion FVG (IFVG)** veya **Order Block (OB)** yapıları taranır.
  - Grey Pool seviyesi ile çakışan (confluence) diğer PD Array'ler işlemin olasılığını (high probability) artırır.
- **Immediate Rebalance & Execution:**

  - Fiyat Grey Pool seviyesini ziyaret ettiğinde **Immediate Rebalance** (ani dengeleme) tepkisi gözlemlenir.
  - Karşı yönlü likidite hedeflerine (**Buy Side Liquidity / Sell Side Liquidity**) ulaşmak için uygun **Market Structure Shift (MSS)** beklenir.

### 💡 ICT'nin Önemli Notları ve İpuçları

- **Patience & Confirmation:**

  - Her Grey Pool temasında körü körüne işleme girilmemeli; işlem için seans zaman dilimleri (**Killzones**) ve zaman-fiyat çakışmaları göz önünde bulundurulmalıdır.
- **Risk Management:**

  - Stop-loss yerleşimi Grey Pool yapısının dışına veya belirleyici bir **Swing High / Swing Low** seviyesine koyulmalıdır.
- **PD Array Hierarchy:**

  - Grey Pools, diğer klasik PD Array'lerin (OB, FVG, Volume Imbalance vb.) yerini tamamen almaz; analizde bir **ekstra onay / likidite bölgesi** olarak harmanlanır.

ICT konseptleriyle ilgili belirli bir grafik örneği veya strateji aşaması hakkında daha ayrıntılı bir inceleme isterseniz belirtmeniz yeterlidir.
