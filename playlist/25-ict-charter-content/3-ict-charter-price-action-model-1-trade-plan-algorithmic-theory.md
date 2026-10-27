# ICT Charter Price Action Model 1 \ Trade Plan & Algorithmic Theory

<https://www.youtube.com/watch?v=4f1vjQMlV50>

Bu videoda (ICT Charter Price Action Model 1) Michael J. Huddleston (ICT), **Scalping Trade Plan** ve **Algorithmic Theory** konularını detaylıca anlatıyor. Öne çıkan ve planın ana kemiğini oluşturan önemli noktalar şunlardır:

### 1. Genel Model Amaç ve Çerçevesi

- **Hedef:** İşlem başına **15 - 20 Pip** scalp kârı yakalamak.
- **Model Rolü:** Verilen strateji temel bir "iskelet" (skeleton) niteliğindedir; kişisel deneyimlerle geliştirilebilir.
- **Uygulama Alanı:** İşlemlerin disiplin kazanılması adına **Demo Hesapta** çalışılması tavsiye edilmektedir.

### 2. Trade Planının 5 Ana Aşaması

Bir işlem planı 5 adımdan oluşur:

1. **Preparation (Hazırlık):** Bekleme ve piyasayı analiz etme evresi.
2. **Opportunity Discovery (Fırsat Keşfi):** Fiyat hareketini takip ederek fırsatı fark etme.
3. **Trade Planning (İşlem Planlama):** İşlem çerçevesini ve kurallarını belirleme.
4. **Execution (İşlem Girişi):** Belirlenen kurallara göre emri iletme.
5. **Trade Management (İşlem Yönetimi):** Pozisyondayken stop ve kâr alma yönetimi.

### 3. Hazırlık ve IPDA Data Range (Lookback)

- **Economic Calendar:** Gelecek haftanın orta ve yüksek etkili (medium/high impact) haber günleri/saatleri taranır.
- **IPDA Data Range (20-Day Lookback):**

  - Pazar günleri sayılmadan geriye dönük son **20 işlem günü** (Trading Days) bakılır.
  - Bu 20 günlük aralıktaki **Highest High** (en yüksek tepe) ve **Lowest Low** (en düşük dip) tespit edilir.
- **Draw on Liquidity & Bias:**

  - Fiyatın gideceği bir sonraki nokta belirlenir: Bir **Liquidity Pool** (Buy-side/Sell-side) veya rebalance edilecek bir **PD Array** (Fair Value Gap vb.).
  - **Bullish Bias:** Bearish Premium PD Array'den veya Sell-side Liquidity alındıktan sonra hedeflenir.
  - **Bearish Bias:** Bullish Discount PD Array'den veya Buy-side Liquidity alındıktan sonra hedeflenir.

### 4. Zaman Pencereleri ve Grafik

- **Kill Zone:** New York Session için zaman aralığı **07:00 AM – 10:00 AM (EST / New York local time)**. *(Petrol haberleri veya sürpriz veri akışlarında 11:00 AM'e uzayabilir).*
- **Grafik Zaman Dilimi:** Giriş düzeni **5-Minute Chart (5m)** üzerinde aranır.

### 5. Algorithmic Theory Rules (Kurallar Bütünü)

#### **Günün Seçimi (Day of Week):**

- **Pazartesi, Salı, Çarşamba:** İşlem için en ideal koşullara sahip günlerdir.
- **Perşembe:** Sadece fiyat henüz 20 günlük aralıktaki eski tepeye (Bullish) veya eski dibe (Bearish) ulaşmadıysa işleme girilebilir.
- **Cuma:** **No Trade** (İşlem yapılmaz).
- **Saat 10:00 AM EST Geçildiyse:** **No Trade**.

#### **Giriş ve Emir Tipleri:**

- **Bullish Scenario (Long):**

  - **Entry:** 5 dakikalık grafikte oluşan Bullish OTE (Optimal Trade Entry) yapısında **62% Fibonacci Retracement seviyesi + 5 Pip** üzerine **Buy Limit** yerleştirilir.
  - **Stop Loss:** OTE salınımının **Anchor Low** (en dip noktası) değerinin **5 Pip altına** konur.
- **Bearish Scenario (Short):**

  - **Entry:** 5 dakikalık grafikte oluşan Bearish OTE yapısında **62% Fibonacci Retracement seviyesi - 5 Pip** altına **Sell Limit** yerleştirilir.
  - **Stop Loss:** OTE salınımının **Anchor High** (en tepe noktası) değerinin **5 Pip üstüne** konur.
- **Stop Out Kuralı:** Eğer stop olunursa, o gün için kesinlikle **tekrar giriş (Re-entry) yapılmaz** (*One and done*).

#### **Kâr Alma (Take Profit & Partials):**

1. **1st Partial (İlk Parçalı Kâr):** Fiyat OTE salınımının **Anchor High / Anchor Low** noktasına ulaştığında ilk kısım kapatılır.
2. **Stop Move:** İlk kâr alındıktan sonra koruma stobu çekilerek **5 - 10 Pip kâr kilitlenir**.
3. **2nd Partial:** Fiyat 20 günlük IPDA aralığındaki eski tepe/dip noktasına veya **Fibonacci Extension #2** seviyesine ulaştığında kapatılır.
4. **Final Closure:** Fiyat **Symmetrical Swing Extension** (1:1 ölçülü hareket hedefi) seviyesine ulaştığında işlem tamamen kapatılır.

### 6. Para ve Risk Yönetimi (Money & Risk Management)

- **Position Size Formülü:**

  Position Size=Account Equity×Risk %Stop Loss (Pips)\text{Position Size} = \frac{\text{Account Equity} \times \text{Risk \%}}{\text{Stop Loss (Pips)}}Position Size=Stop Loss (Pips)Account Equity×Risk %​
- **Pozisyon Bölüşümü:** 15 Pip ve 20 Pip kâr hedefleri için birden fazla emir kullanılıyorsa, hesaplanan toplam riski (ör. %1.5 risk) pozisyon adedine bölmek gerekir.
- **Kayıp Yönetimi (Drawdown Protocol):**

  - Tam kayıp (stop) yaşandığında, bir sonraki işlemdeki **Risk %50 oranında düşürülür**.
  - Kayıp %50 oranında telafi edildiğinde tekrar maksimum riske dönülebilir.
- **Seri Kazanç Yönetimi (Equity Curve Protection):**

  - Üst üste **5 kazançlı işlem (Winning Trades)** sonrasında risk %50 oranında düşürülür. Bu kural, psikolojik aşırı özgüveni engeller ve sert bakiye düşüşlerini (drawdown) önler.

Videoya doğrudan ulaşmak için: [ICT Charter Price Action Model 1](https://www.youtube.com/watch?v=4f1vjQMlV50)

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Charter Price Action Model 1 \ Trade Plan & Algorithmic Theory

The Inner Circle Trader · 252K views

 [Open in ICT Charter Price Action Model 1 \ Trade Plan & Algorithmic Theory](http://www.youtube.com/watch?v=4f1vjQMlV50)](http://www.youtube.com/watch?v=4f1vjQMlV50)

![](https://i.ytimg.com/vi/4f1vjQMlV50/maxresdefault.jpg)
