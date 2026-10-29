# ICT Algorithmic Time & Price Grids

<https://www.youtube.com/watch?v=4SJlJdIANCo>

İstediğin **"ICT Algorithmic Time & Price Grids"** başlıklı Inner Circle Trader (Michael J. Huddleston) videosunun detaylı, maddeler halinde düzenlenmiş özeti aşağıdadır. Orijinal teknik terimler (Time & Price, Macro, Grid vb.) İngilizce halleriyle korunmuştur.

## 📌 Videonun Temel Amacı ve Konusu

Bu derste ICT, kurumların (Institutional Traders) **Macro Time** penceresini, grafik üzerindeki **Price Action/Structure** delivery’si ile nasıl hizaladığını açıklıyor. Fiyatı sadece seviye seviye değil; belirli zaman dilimlerinde (Time Window) **Grid/Matris** mantığıyla okumanın algoritmayı anlama konusundaki önemini NQ (Nasdaq Futures) canlı/geçmiş fiyat hareketleri üzerinden inceliyor.

## 🔑 Önemli Maddeler ve Detaylı Özet

### 1. Algorithmic Time & Price Grid Kavramı

- **Grid Yapısı:** Fiyatı analiz ederken zamanı (X ekseni) ve fiyatı (Y ekseni) belirli periyotlara bölerek **Grid (Izgara)** matrisi oluşturulur.
- **Macro Windows:** Algoritmanın piyasaya likidite enjekte ettiği veya fiyatı manipüle/reprice ettiği spesifik zaman aralıkları (Macro'lar) bulunur.
- ICT, bu Macro pencerelerini sadece tek bir blok olarak görmek yerine, kendi içerisinde eşit parçalara (örneğin 2'ye veya 4'e bölerek) alt Grid'lere ayırmayı gösterir.

### 2. Time (Zaman) Faktörünün Fiyat Üzerindeki Önceliği

- ICT, "Time control Price" (Zaman, Fiyatı kontrol eder) ilkesini vurgular.
- Seviyelerin (Fair Value Gap, Order Block, Liquidity Pool) ne zaman test edildiği (Time), seviyenin kendisinden çok daha kritik bir onay mekanizmasıdır.
- Piyasada gerçekleşen sert **sell-off** veya **fast reversal** hareketleri rastgele değildir; tam olarak bu Algorithmic Macro pencerelerinin açılış ve kapanış noktalarına denk getirilir.

### 3. Nasdaq (NQ) Futures Üzerinden Market Review & Execution Analysis

- **Open & Aggressive Sell-off:** Piyasa açılışıyla birlikte gerçekleşen agresif düşüşün, Algorithmic Time dilimi açıldığında nasıl hızlandığını gösterir.
- **Liquidity Sweep / Purge:** Fiyatın önceden belirlenmiş Sell-side Liquidity (SSL) seviyelerine ulaştıktan hemen sonra Macro Time Grid'inin belirli bir bölmesinde tepki verdiğini ve hızlı bir **reversal / V-shape recovery** oluşturduğunu anlatır.
- **Macro Sub-divisions:** Makro zaman dilimi ikiye veya dörde bölündüğünde; ilk yarıda **Manipulation / Protraction**, ikinci yarıda ise **Distribution / Expansion** gerçekleşir.

### 4. Grid Nasıl Kullanılır? (Practical Application)

- **Time Alignment:** İşleme girmeden önce açılan Macro zaman aralığının başlangıcını belirleyin.
- **Price Alignment:** Aradığınız PD Array (FVG, Order Block, Breaker Block vb.) ve Likidite alanlarını işaretleyin.
- **Grid Intersections:** Fiyat tam bu Macro Grid dikey çizgilerine ulaştığı anda (Time) ve yatay fiyat seviyeleriyle (Price) kesiştiğinde yüksek olasılıklı (High Probability) işlem fırsatı doğar.
- **Algorithmic Repricing:** Algoritmanın hedef seviyelere (Buy-side Liquidity / Target FVG) nasıl milimetrik bir hassasiyetle ulaşarak teslimatı (Price Delivery) tamamladığı vurgulanır.

### 💡 Ana Çıkarım (Key Takeaway)

> Algoritma rastgele çalışmaz; belirli **Time Macro** saatlerinde aktif hale gelerek fiyatı bir sonraki likidite alanına veya verimsizliğe (Fair Value Gap) sürükler. İşlemlerinizde sadece fiyat seviyesine bakmak yerine, zaman dilimini Grid matrisleri halinde bölerek **Time & Price Confluence** (Zaman ve Fiyatın çakışması) aramalısınız.

*Başka bir ICT konsepti veya belirli bir zaman damgası (timestamp) hakkında detay incelemesi isterseniz yardımcı olabilirim!*
