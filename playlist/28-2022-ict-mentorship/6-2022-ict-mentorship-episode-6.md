# 2022 ICT Mentorship Episode 6

<https://www.youtube.com/watch?v=Bkt8B3kLATQ>

Michael J. Huddleston’ın (Inner Circle Trader) **"2022 ICT Mentorship Episode 6"** başlıklı videosunun (*Market Efficiency Paradigm & Institutional Order Flow / Fair Value Gap & Market Structure Shifts*) detaylı, maddeler halinde özeti:

## 📌 Videosunun Genel Amacı

Bu derste ICT, fiyat hareketlerinin (price action) tamamen rastgele olmadığını, algoritmik bir sistem olan **IPDA (Interbank Price Delivery Algorithm)** tarafından yönlendirildiğini anlatır. *Market Efficiency Paradigm* çerçevesinde, markette likidite avı (*stop hunt*) ve yapı kırılımları (*Market Structure Shift*) sonrası oluşan **Fair Value Gap (FVG)** yapılarını detaylandırır.

## 🔑 Ana Başlıklar ve Detaylı Notlar

### 1. Market Efficiency Paradigm (Piyasa Verimlilik Paradigması)

- **Algoritmik Fiyat Teslimatı:** Piyasa, alıcı ve satıcıların serbest iradesiyle değil; bankalar arası fiyatlama algoritması (IPDA) tarafından kontrol edilir.
- **Likidite Hedefleme:** Algoritma sürekli iki ana hedefe yönelir:

  - **Liquidity Pools:** Stop order'ların biriktiği seviyeler (*Buyside Liquidity* / *Sellside Liquidity*).
  - **Inefficiencies (Imbalances):** Fiyatın hızlı kaçtığı ve geride dengesizlik bıraktığı alanlar (*Fair Value Gap*).
- **Stop Hunt Mantığı:**

  - Büyük ve belirgin bir düşüş dalgası bekleniyorsa, öncesinde mutlaka **Buystop Liquidity**'ye yönelik bir likidite temizliği (*Stop Hunt*) gerçekleşir.
  - Büyük bir yükseliş dalgası bekleniyorsa, öncelikle **Sellstop Liquidity** süpürülür.

### 2. Market Structure Shift (MSS) ve Displacement

- **Displacement (Şiddetli Fiyat Hareketi):**

  - Fiyat, likiditeyi aldıktan sonra ters yöne doğru tek taraflı ve gövdeli mumlarla (*energetic / aggressive expansion*) hızlıca hareket etmelidir.
  - Bu hızlı hareket, algoritmanın piyasaya kurumlar düzeyinde yön verdiğinin kanıtıdır.
- **Market Structure Shift (MSS):**

  - Yükseliş yönlü bir MSS için: Fiyatın *Sellside Liquidity* süpürdükten sonra en son oluşan *Swing High* seviyesini ihlal edip üzerinde mum kapanışı yapması gerekir.
  - Düşüş yönlü bir MSS için: Fiyatın *Buyside Liquidity* süpürdükten sonra en son oluşan *Swing Low* seviyesini aşağı yönlü kırması gerekir.

### 3. Fair Value Gap (FVG) Mantığı ve Giriş Stratejisi

- **FVG Tanımı:** 3 mumlu bir formasyonda 1. mumun en yüksek/en düşük seviyesi ile 3. mumun en yüksek/en düşük seviyesi arasında oluşan boşluktur (2. mumun gövdesi bu alanı tek başına kaplar).
- **Verimsizlik Tespit Etme:**

  - Sadece tek yönlü fiyat teslimatı olan alanlar (örneğin sadece alıcıların olduğu uzun bir yeşil mum), algoritma tarafından tekrar ziyaret edilerek dengelenmek zorundadır (*rebalance*).
- **Giriş ve Seviye Seçimi:**

  - **Consequent Encroachment (CE):** FVG alanının tam orta noktası (%50 seviyesi). Fiyatın bu noktadan tepki vermesi oldukça yaygındır.
  - **Birden Fazla FVG Varsa:** Fiyat bazen daha derindeki (*deeper FVG*) FVG seviyesine sarkar. Derindeki FVG'ye dokunduktan sonra sığ FVG'ye geri döndüğünde işleme girmek riski azaltır.

### 4. Zaman Dilimleri ve Seans Saatleri (Killzones & Timeframes)

- **Zaman Dilimleri:**

  - Analiz 1 saatlik ve 15 dakikalık grafiklerde ana yönü (bias) bulmak için başlatılır.
  - Giriş ve hassas tetikleyici tespitleri için **1 min, 2 min ve 3 min** gibi düşük zaman dilimleri (Lower Timeframe - LTF) tercih edilir (5 min yerine 1-3 min aralığı daha nettir).
- **Zaman Pencereleri (Time Windows):**

  - ICT, özellikle **08:30 AM - 11:00 AM EST** (New York AM Session) aralığına odaklanır. Bu zaman dilimi en yüksek likidite ve yön belirleme hacmine sahiptir.

### 5. Trade Setup (İşlem Modeli Özeti)

1. **Bias & Liquidity Check:** 1H / 15m grafikte *Buystop* veya *Sellstop* seviyesini belirle.
2. **Liquidity Sweep:** Fiyatın bu seviyeyi temizlemesini bekle.
3. **Displacement & MSS:** LTF'de (1m-3m) mum gövdesiyle gerçekleşen net bir *Market Structure Shift* gör.
4. **Identify FVG:** Displacement hareketi sırasında oluşan *Fair Value Gap* alanını işaretle.
5. **Entry & Stop Loss:**

   - **Entry:** FVG alanının üst/alt sınırından ya da *Consequent Encroachment* (%50) seviyesinden limit emir.
   - **Stop Loss:** Likiditeyi süpüren en uç nokta (*High* / *Low*) veya kırılımı başlatan *Order Block* arkası.
6. **Take Profit (TP):** İçeride kalan yakın tarihteki swing noktaları veya karşı taraftaki likidite (*Internal Range Liquidity* / *External Range Liquidity*).

### 6. Psikoloji ve Disiplin Notları

- Fiyatın her yaptığı mum hareketinde işlem aranmamalıdır.
- Her zaman diliminde oluşan her boşluk geçerli bir FVG değildir; sadece likidite alımı ve MSS sonrasında oluşan FVG'ler yüksek ihtimalli işlem imkanı sunar (*High Probability Setup*).
- Yanlış gidişatlarda veya kaçan fırsatlarda kendinizi suçlamak yerine algoritmanın ritmine ayak uydurmaya odaklanılmalıdır.
