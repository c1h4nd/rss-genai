# Part 2 High Precision Secrets To Intraday Price Action

<https://www.youtube.com/watch?v=BD7kqmgdBU8>

Bu video, **ICT (The Inner Circle Trader - Michael J. Huddleston)** tarafından yayınlanan **"Part 2 \ High Precision Secrets To Intraday Price Action"** dersinin detaylı özetidir.

Video, intraday (gün içi) fiyat hareketlerini yüksek hassasiyetle okumak ve seans seviyelerini doğru kurgulamak üzerine teknik ve metodolojik ipuçları sunmaktadır.

### 1. Ana Konsept ve Çalışma Prensibi (Core Concept)

- **Daily Chart & Daily Range:** Gün içi seviyeleri analiz etmeden önce referans noktası **Daily Chart**'tır. Gün içi dalgalanmalar (Daily Range) günlük grafiğin sunduğu likidite ve yönelime (Bias) göre şekillenir.
- **Time & Price Synchronization:** Zaman ve fiyatın eşleşmesi esastır. Sadece seviye (fiyat) değil, fiyatın o seviyeye **hangi saat diliminde (Killzones)** temas ettiği kritik önem taşır.

### 2. Opening Range Gap (ORG) ve Seviye Açıları

- **Gap Anchor Noktaları:**

  - Güncel seansın **9:30 AM Eastern Open** fiyatı.
  - Bir önceki seansın Kapanışı / Settlement fiyatı (örneğin **4:14 PM Eastern**).
- **Consequent Encroachment (CE):**

  - Oluşan Gap'in tam orta noktasıdır (%50 seviyesi).
  - Bu seviyenin üzerindeki bölge **Premium**, altındaki bölge ise **Discount** olarak kabul edilir.
- **Quadrant ve Octant Bölünmeleri:**

  - Gap aralığı sadece yarıya bölünmez; hassas ölçümler için **Quadrant (%25, %50, %75)** ve **Octant (%12.5, %37.5 vb.)** seviyeleri çizilir.
  - Bu mikro seviyeler, fiyatın algoritma tarafından nerede durdurulduğunu veya tepki aldığını belirler.

### 3. Candle Body vs. Wick (Mum Gövdesi ve İğne Ayrımı)

- **Wick (İğne/Fitil):** Fiyatın likidite havuzlarına ulaştığı ve aradaki emirleri temizlediği (Liquidity Sweep) alanlardır. İğneler kilit seviyeleri veya CE'yi aşabilir.
- **Body (Mum Gövdesi):** Kurumsal hacmin ve gerçek fiyat kabulünün (Volume / Fair Value) olduğu yerdir.
- **Kural:** İğneler Quadrant/CE seviyelerini geçse bile, mum gövdelerinin (Candle Bodies) bu seviyelerin altında/üstünde **kapanış yapamaması** seviyenin korunduğunu gösterir.

### 4. PD Arrays ve Algoritmik Fiyat Akışı (Workflow)

- **Array Derecelendirmeleri:**

  - **FVG (Fair Value Gap)**, **Order Block (OB)** ve **Breaker Block** gibi yapıların intraday Gap seviyeleriyle nasıl çakıştığı takip edilir.
- **Breakaway Gap:**

  - Fiyat iki belirgin PD Array arasında konsolide olduktan sonra güçlü bir **Displacement** (hacimli mum hareketi) ile aşağı veya yukarı kırılırsa, geride kalan Gap bir **Breakaway Gap** olarak davranır ve kolay kolay dolmaz.
- **Inversion / IFVG (Inversion Fair Value Gap):**

  - Destek olarak çalışması beklenen bir Gap/FVG sert bir şekilde kırılırsa, tam tersi yönde direnç olarak çalışmaya başlar.

### 5. Intraday Execution & Trade Management (İşlem Yönetimi)

- **Scaled Position / Partial Taking:**

  - Gün içi işlemlerde fiyat hedef seviyelere (Quadrant hatları veya Likidite havuzları) ulaştıkça kademeli kar alımı (Scale out / Partials) yapılmalıdır.
- **Stop Distance & Risk Exposure:**

  - Stop mesafe kurgusu intraday volatiliteye göre ayarlanmalı, sadece "haklı çıkmak" üzerine değil, algoritmik yapı bozulduğu anda işlemden çıkılacak şekilde planlanmalıdır.

### 6. Duyuru ve Genel Notlar

- Video sonunda ICT, St. Jude çocuk hastanesi için düzenlenen bağış kampanyası ve sponsorluk/kod detaylarına değinmektedir.

İncelemek istediğiniz belirli bir dakika, grafik örneği veya konsept *(örneğin Inversion FVG veya Quadrant hesabı)* var mı?
