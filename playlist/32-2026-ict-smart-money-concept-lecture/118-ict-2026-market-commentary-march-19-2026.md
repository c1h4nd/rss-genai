# ICT 2026 Market Commentary \ March 19, 2026

<https://www.youtube.com/watch?v=w2zTfhjScDg>

Bu YouTube videosu (`w2zTfhjScDg`), Inner Circle Trader (ICT / Michael J. Huddleston) tarafından yayınlanan ve **Price Action**, **Algorithmic Price Delivery** ve **Market Structure** konularını detaylıca ele alan canlı piyasa analizi ve eğitim derslerinden biridir.

İşte videonun ana başlıklar ve orijinal terminolojileri korunarak hazırlanmış detaylı özeti:

### 1. Temel Piyasa Mantığı ve Algoritma Yaklaşımı

- **Interbank Price Engine (IPDA):** Piyasa hareketlerinin rastgele veya indikatör odaklı değil, belirli algoritmik zaman/fiyat pencerelerine (**Time and Price**) göre hareket ettiği vurgulanıyor.
- **Liquidity Pools:** Piyasanın ana amacının likidite toplamak olduğu belirtiliyor:

  - **Buy Side Liquidity (BSL):** Eski zirvelerin (Old Highs / Equal Highs) üzerindeki stop-loss emirleri.
  - **Sell Side Liquidity (SSL):** Eski diplerin (Old Lows / Equal Lows) altındaki stop-loss emirleri.

### 2. Önemli Yapısal Kavramlar (Price Action Concepts)

- **Fair Value Gap (FVG):** Fiyatın hızlıca tek yönlü hareket ederek arkasında bıraktığı dengesizlik (imbalance) alanları. Algoritmanın bu alanları doldurmak (**rebalance**) üzere geri çekilme yaptığı anlatılıyor.
- **Order Block (OB):** Piyasa yön değiştirmeden önceki son karşıt renkli mum. Fiyatın reaksiyon alması beklenen kilit destek/direnç seviyesi olarak takip ediliyor.
- **Breaker Block / Mitigation Block:** Destek veya direncin kırılmasıyla yapının yön değiştirmesi durumunda likidite temizliği yapmış/yapmamış mumların rolü ve retest alanları.
- **Liquidity Void / Range Expansion:** Piyasanın sert bir şekilde tek bir yöne genişleyip boşluklar bırakması.

### 3. Zaman Seansları ve Zaman Dilimleri (Timing & Killzones)

- **ICT Killzones:** İşlem stratejilerinin başarı oranının zamanlamaya doğrudan bağlı olduğu vurgulanıyor:

  - **London Open Killzone**
  - **New York Open Killzone**
  - **London Close Killzone**
- **Judas Swing:** Özellikle London Session başlangıcında piyasanın gerçek yönünün aksi yönüne yapılan sahte kırılım (false breakout / trap) hareketi.
- **Higher Time Frame (HTF) Narrative:** Düşük zaman dilimlerindeki (1m, 5m) girişlerin başarılı olabilmesi için mutlaka Higher Time Frame (Daily, 4H, 1H) yönünün ve hedeflerinin doğru analiz edilmesi gerektiği hatırlatılıyor.

### 4. İşlem Kurulumu ve Ticaret Yönetimi (Trade Setup & Execution)

- **Bias Belirleme:** İşlem öncesinde piyasanın **Premium** (pahalı) mı yoksa **Discount** (ucuz) bölgesinde mi olduğuna göre yön (Bullish / Bearish Bias) belirlenmeli.
- **Market Structure Shift (MSS):** Alt zaman diliminde (Lower Time Frame - LTF) trendin değiştiğini doğrulayan yapısal kırılım.
- **Entry Model:**

  1. HTF Liquidity veya FVG seviyesine temas.
  2. LTF üzerinde Market Structure Shift (MSS) oluşması.
  3. Oluşan yeni FVG veya Order Block seviyesine geri çekilme (retracement) ile işleme giriş.
- **Risk & Trade Management:**

  - Stop-loss yerleşimi mutlaka swing high/low arkasına yapılmalı.
  - Kar alma hedefleri (**Take Profit**) karşı taraftaki BSL veya SSL seviyeleri olarak seçilmeli.
  - Partial profit (parçalı kar) alarak risk azaltmanın önemi vurgulanıyor.
