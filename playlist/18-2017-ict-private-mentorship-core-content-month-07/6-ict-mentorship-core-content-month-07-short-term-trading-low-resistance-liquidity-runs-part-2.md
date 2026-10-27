# ICT Mentorship Core Content - Month 07 - Short Term Trading Low Resistance Liquidity Runs Part 2

<https://www.youtube.com/watch?v=O69iFqP1j7o>

**ICT Mentorship Core Content - Month 07 - Short Term Trading Low Resistance Liquidity Runs Part 2** başlıklı videoda öne çıkan detaylı konular şunlardır:

### 1. Zaman ve Fiyat Teorisi (Time & Price Theory) ve Veri Aralığı

- **IPDA Data Range**: Market maker algoritmalarının geçmiş **20, 40 ve 60 işlem gününü** referans aldığı zaman ve fiyat teorisi vurgulanır [[[00:27](https://www.youtube.com/watch?v=O69iFqP1j7o&t=27)]].
- **Short-Term Trading / One Shot One Kill**: Kısa vadeli işlemler ve bu model için odak noktası öncelikle son **3 aylık** zaman dilimindeki institutional reference point'lerdir [[[00:41](https://www.youtube.com/watch?v=O69iFqP1j7o&t=41)]].
- **PD Array’ler Arası İşlem**: Fiyatın bir **PD Array**'den (Premium/Discount array) diğerine doğru hareket ettiği, ideal senaryonun belirgin bir **Discount** bölgesinden **Premium** bölgesine doğru gerçekleştiği aktarılır [[[00:51](https://www.youtube.com/watch?v=O69iFqP1j7o&t=51)]].

### 2. Market Koşulları ve Grafik Analizi

- **Fractal Yapı**: Fiyatın universal olarak **fractal** yapıda olduğu; büyük zaman dilimindeki bir consolidation (konsolidasyon) alanının, alt zaman dilimlerinde belirgin bir **trending environment** (trend piyasası) sunduğu belirtilir [[[01:30](https://www.youtube.com/watch?v=O69iFqP1j7o&t=90)]].
- **Discount -> Premium Dynamics**: Fiyat Deep Discount alanında destek bulduğunda, smart money kurumlarının pozisyon biriktirmesi (position building) ve fiyatı agresif bir şekilde (displacement ile) yukarı taşıyarak daha yüksek seviyelerdeki **Premium PD Array**'lerde likidite alması hedeflenir [[[02:20](https://www.youtube.com/watch?v=O69iFqP1j7o&t=140)]].

### 3. 4 Saatlik (4H) Grafik ve "One Shot One Kill" Modeli

- **Ana Zaman Dilimi**: ICT, One Shot One Kill / kısa vadeli işlem modellerini kurgulamak için **4 saatlik (4H) grafiklerin** en verimli zaman dilimi olduğunu ifade eder [[[03:48](https://www.youtube.com/watch?v=O69iFqP1j7o&t=228)]].
- **Weekly Dividers (Haftalık Ayraçlar)**: MT4 veya diğer platformlarda `Ctrl + Y` kısayolu ile açılan dikey hatlar 4H grafikte **haftalık zaman dilimlerini (Weekly Dividers)** gösterir [[[04:49](https://www.youtube.com/watch?v=O69iFqP1j7o&t=289)]].
- **Quadrants & Grading Ranges**:

  - Fiyat aralıklarının (price swing) en yüksek ve en düşük gövde (body) seviyelerinden belirlenip kademeli olarak ikiye/dörde bölünmesi (grading/quadrants) önerilir [[[10:13](https://www.youtube.com/watch?v=O69iFqP1j7o&t=613)]].
  - Bu seviyeler, klasik Pivot Points mantığından farklı olarak algoritmanın fiyatı üzerine çektiği birer **mıknatıs (magnet)** ve algoritma için **mile marker** işlevi görür [[[11:37](https://www.youtube.com/watch?v=O69iFqP1j7o&t=697)]], [[[13:54](https://www.youtube.com/watch?v=O69iFqP1j7o&t=834)]].
- **Pip Hedefleri**: Trade modellerinde haftalık gerçekçi pip hedeflerinin belirlenmesi önerilir:

  - Başlangıç seviyesi: **30 - 50 Pip / hafta** [[[07:12](https://www.youtube.com/watch?v=O69iFqP1j7o&t=432)]]
  - İlerleyen süreç: **50 - 75 Pip / hafta** [[[07:12](https://www.youtube.com/watch?v=O69iFqP1j7o&t=432)]]
  - Üst sınır: **75 - 100 Pip / hafta** (Haftalık toplam range küçük kaldığında 100 Pip üstü hedefler yakalamak zorlaşır) [[[07:17](https://www.youtube.com/watch?v=O69iFqP1j7o&t=437)]].

### 4. Günlük / Haftalık Akış ve "Power of 3" (PO3)

- **Power of 3**: Bullish haftalarda haftalık mumun **Open** seviyesinin **Low** seviyesine yakın olduğu, **Close** seviyesinin ise haftanın **High** seviyesinde/yakınında gerçekleştiği kuralı vurgulanır [[[08:32](https://www.youtube.com/watch?v=O69iFqP1j7o&t=512)]].
- **Haftalık Ön Görü (Anticipatory Price Skills)**:

  - Pazar akşamı piyasa açılmadan önce 4H grafiğe Monthly, Weekly ve Daily PD Array’lerin eklenmesi önerilir [[[16:10](https://www.youtube.com/watch?v=O69iFqP1j7o&t=970)]].
  - Amaç, haftanın alabileceği muhtemel mum yapısını ve fiyatın ulaşabileceği **Low Resistance Liquidity** hedeflerini önceden tahmin etme becerisini geliştirmektir [[[16:35](https://www.youtube.com/watch?v=O69iFqP1j7o&t=995)]].

### 5. 1 Saatlik (60 Min) Grafik ve Gün Bazlı Algoritmik Olgular (Day of Week Phenomenon)

- **Zaman Dilimi Ayrımı**: 4H seviyelerini belirledikten sonra **60 dakikalık (1H) grafik**, Breaker ve Mitigation Block gibi detayları netleştirmek ve işlem riskini düşürmek için kullanılır [[[18:30](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1110)]], [[[19:46](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1186)]]. (1H altı zaman dilimlerinin daha çok scalping/day trading alanına girdiği belirtilir) [[[20:06](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1206)]].
- **Haftanın Dip/Tepesinin Oluşum Günleri (Low/High of the Week)**:

  - Bullish trend koşullarında **Low of the Week** genellikle **Pazartesi, Salı veya Çarşamba** günleri oluşur [[[20:52](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1252)]].
- **Haftalık Range Tamamlanma Oranı**:

  - Genellikle haftalık hareketin **%30 ile %50'si** Çarşamba günkü London Close seansına kadar tamamlanmış olur [[[23:34](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1414)]].
  - Pazartesi-Çarşamba arasındaki ana hareketi kaçırdıysanız, Perşembe veya Cuma günleri son iki günde büyük bir hareket beklentisine girmemeniz ("pip drunk" olmamanız) gerektiği belirtilir [[[24:38](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1478)]]. Cuma günleri çoğunlukla retracement ya da nötr kapanış gösterir [[[25:22](https://www.youtube.com/watch?v=O69iFqP1j7o&t=1522)]].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    ICT Mentorship Core Content - Month 07 - Short Term Trading Low Resistance Liquidity Runs Part 2

    The Inner Circle Trader · 166K views

     [Open in ICT Mentorship Core Content - Month 07 - Short Term Trading Low Resistance Liquidity Runs Part 2](http://www.youtube.com/watch?v=O69iFqP1j7o)](http://www.youtube.com/watch?v=O69iFqP1j7o)

    ![](https://i.ytimg.com/vi/O69iFqP1j7o/maxresdefault.jpg)
