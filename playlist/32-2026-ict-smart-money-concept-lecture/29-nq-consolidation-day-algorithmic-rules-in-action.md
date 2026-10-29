# NQ Consolidation Day Algorithmic Rules In Action

<https://www.youtube.com/watch?v=0olLwAiLa3o>

**Inner Circle Trader (ICT)** tarafından yayınlanan **"NQ Consolidation Day Algorithmic Rules In Action"** başlıklı videonun detaylı ve maddeler halinde özeti:

### 📌 Genel Bakış & Giriş

- **Video Amacı:** NQ (Nasdaq Futures) piyasasında yatay/konsolidasyon (*consolidation day*) günlerinde algoritmanın nasıl davrandığını ve bu günlerde geçerli olan algoritmik kuralları canlı/teknik incelemeyle göstermek.
- **Not Tutma Vurgusu:** ICT, ders boyunca izleyicilerin mutlaka kağıt-kalem kullanarak detaylı not almalarını ve kuralları şablonlaştırmalarını vurguluyor.

### ⏱️ Pre-Market Zaman Dilimi ve Kural Seti (7:00 – 9:00 AM ET)

- **Altın Pencere:** Pre-market analizi için **7:00 AM – 9:00 AM ET** aralığı referans zaman dilimi olarak belirlenir.
- **High / Low Ölçümü:** Bu saat aralığında oluşan en yüksek seviye (*highest high*) ve en düşük seviye (*lowest low*) işaretlenir.
- **Midpoint (Consequent Encroachment / Equilibrium):** Bu aralığın tam orta noktası (*midpoint*) hesaplanır:

  - **Midpoint Üzeri:** *Premium* (Satış/Short arayışı için uygun alan).
  - **Midpoint Altı:** *Discount* (Alış/Long arayışı veya hedeflere ulaşma alanı).

### 📊 Algoritmik Konsolidasyon Kuralları

- **Seek & Destroy / Range-Bound Yapı:** Konsolidasyon günlerinde algoritma trend oluşturmak yerine liquidity çekmeye (her iki yöndeki stop'ları temizlemeye) odaklanır.
- **Grading Imbalances:** FVG (*Fair Value Gap*) ve likidite boşlukları değerlendirilirken mumların iğnelerinden (*wicks*) ziyade **mum gövdelerine (*candlestick bodies*)** öncelik verilir.

  - Mum gövdelerinin PD Array veya imbalance seviyesinin neresinde kapandığı (*upper half* veya *lower half*) sipariş akışının (*order flow*) yönünü belirler.
- **Midpoint Seviyelerinin Tepkisi:** Konsolidasyon günlerinde fiyat, açılış veya pre-market aralığının midpoint seviyesini sıklıkla mıknatıs gibi çeker veya etrafında salınım yapar.

### 🎯 Trade Execution ve Risk Yönetimi (Real-Time Review)

- **Zaman Dilimi:** Analiz ve işlem yönetimi için ağırlıklı olarak **1-minute chart** (1 dakikalık grafik) kullanılır.
- **Stop Placement:**

  - Stop-loss seviyeleri geniş tutulmaz; spesifik mum gövdelerinin (*candle bodies*) veya mum iğnelerinin (*wick highs/lows*) hemen üstüne/altına yerleştirilir.
- **Target & Entry:**

  - Girişler belirlenen Fair Value Gap (FVG) ve PD Array seviyelerine limit emirlerle ya da onay alarak yapılır.
  - Hedefler ise karşı taraftaki likidite havuzları (*buy-side / sell-side liquidity*) veya imbalance dolum noktalarıdır.
- **Disiplin ve Yönetim:** Konsolidasyon günlerinde büyük "home-run" hareketler beklemek yerine, algoritmanın kurallarına sadık kalarak ve tanımlı hedeflerde kar alarak (*take profit*) işlem yönetilmelidir.
