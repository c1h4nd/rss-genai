# ICT Mentorship Core Content - Month 07 - Short Term Trading Blending IPDA Data Ranges & PD Arrays

<https://www.youtube.com/watch?v=YV4fEF4d2wA>

Bu videoda (**ICT Mentorship Core Content - Month 07: Short Term Trading Blending IPDA Data Ranges & PD Arrays**), Michael J. Huddleston (ICT) zaman (IPDA Data Ranges) ve fiyat (PD Array Matrix) bileşenlerini harmanlayarak kısa vadeli işlem (Short-Term Trading) stratejilerini detaylı bir şekilde açıklıyor.

Videoda öne çıkan tüm önemli noktalar detaylandırılmış olarak şu şekildedir:

### 1. Temel Mantık: Zaman ve Fiyatın Harmanlanması (Time & Price Blending) [[00:26](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=26)]

- **IPDA Data Ranges (Zaman):** Algoritmanın geriye dönük baktığı zaman dilimlerini ifade eder.
- **PD Arrays (Fiyat):** Fiyatın ulaştığı veya ulaşmayı hedeflediği spesifik seviyeleri/yapıları ifade eder.
- **IPDA (Interbank Price Delivery Algorithm):** Bankalararası fiyat sunum algoritması, geçmiş verileri analiz ederek likiditeyi ve eksik kalmış fiyat alanlarını doldurmak için bu iki bileşeni birlikte kullanır [[01:15](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=75)].

### 2. IPDA Look-Back Period (Geriye Dönük Veri Aralıkları) [[00:48](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=48)]

Algoritma ve analistlerin geriye doğru bakması gereken temel 3 zaman dilimi tanımlanmıştır:

- **20 Trading Days (1 Ay):** En yakın zaman dilimi ve mevcut range referansı.
- **40 Trading Days (2 Ay):** Orta vadeli zaman aralığı.
- **60 Trading Days (3 Ay):** Geniş çerçeveli ana likidite ve range analizi [[05:02](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=302)].
- Her yeni gün ilerledikçe bu 20, 40 ve 60 günlük pencere de birer gün ileriye kaydırılır (Shift Forward) [[01:05](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=65)].

### 3. PD Array Hierarchy & Matrix (Hiyerarşi Dizilimi) [[01:35](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=95)]

Algoritmanın fiyatı sürdüğü yön ve sırasına göre **PD Array Matrix** ikiye ayrılır:

#### **Premium Market (Fiyat mevcut seviyenin üstündeyse / Bearish hedefler) [[01:45](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=105)]:**

Fiyat yukarı yönlü hareket ederken hiyerarşik sırayla şu seviyeleri arar:

1. Bearish Mitigation Block
2. Bearish Breaker
3. Liquidity Void / Fair Value Gap (FVG)
4. Bearish Order Block
5. Rejection Block
6. Old High / Old Low

#### **Discount Market (Fiyat mevcut seviyenin altındaysa / Bullish hedefler) [[02:08](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=128)]:**

Fiyat aşağı yönlü hareket ederken hiyerarşik sırayla şu seviyeleri arar:

1. Bullish Mitigation Block
2. Bullish Breaker
3. Liquidity Void / Fair Value Gap (FVG)
4. Bullish Order Block
5. Rejection Block
6. Old Low / Old High

> **Önemli Not:** Grafikte her zaman bu PD Array'lerin tamamı bulunmak zorunda değildir. Mevcut olan yapılar (2-3 tanesi bile olsa) kurulum kurmak için yeterlidir [[03:37](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=217)]. Bir PD Array test edilip tepki verdiyse **tükenmiş (exhausted)** kabul edilir ve bir sonrakine bakılır [[04:21](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=261)].

### 4. Trend Yönüne Göre Hedefleme Mantığı [[05:27](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=327)]

- **Bearish (Düşüş) Piyasa Koşullarında:**

  - Premium PD Array'ler **Direniş / Satış (Resistance / Sell Setup)** seviyeleri olarak kullanılır.
  - Discount PD Array'ler ise fiyatın düşmeyi hedeflediği **Kâr Al (Take Profit / Target)** seviyeleridir.
- **Bullish (Yükseliş) Piyasa Koşullarında:** Mantık tam tersine işler; Discount alanlar giriş, Premium alanlar hedeftir.

### 5. Grafikte Uygulama Adımları ve AUD/USD Canlı Örnek Analizi [[06:23](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=383)]

Videoda AUD/USD Günlük (Daily) ve 4 Saatlik (4H) grafikleri üzerinden canlı bir işlem örneği incelenir:

1. **Range Belirleme:** Günlük grafikte son 20, 40 ve 60 günlük en yüksek (Highest High) ve en düşük (Lowest Low) seviyeler işaretlenir [[07:05](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=425)].
2. **Matrix Overlay:** Günlük range Premium ve Discount olarak ikiye bölünür [[07:16](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=436)].
3. **Senaryo Değişimi (Pivot/Failure Swing):**

   - ICT, haftanın başında AUD/USD paritesinde Bullish (yükseliş) beklentisine sahip olduğunu, ancak Salı günü fiyatın yeni bir yüksek yaptıktan sonra başarısız olup hızla reddedildiğini (Failure Swing / Liquidity Pool Raid) belirtir [[11:32](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=692)].
   - Analiz hatalı çıktığında algoritmik yapıyı anlayarak **yön değiştirebilmenin (reverse analysis)** önemi vurgulanır [[11:16](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=676)].
4. **Zaman Dilimi Düşürme (Top-Down Analysis):**

   - Daily seviyelerde oluşan likidite alımından sonra işlem fırsatı ve hedef aramak için **4H ve 1H (Zaman dilimleri)** grafiklerine inilir [[12:23](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=743)].
5. **İşlem Girişi ve Hedef:**

   - 4H grafikte fiyat 76.80 seviyesindeki Institutional Level & Mitigation/Breaker bölgesine çekilerek satış fırsatı sunar [[12:40](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=760)].
   - Hedef olarak alt tarafta açık duran **Liquidity Void (76.05)** hedeflenir ve fiyat noktası noktasına (to the pip) bu boşluğu doldurur [[13:47](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=827)].

### 6. Market Maker Manipulation Template (Piyasa Yapıcı Manipülasyon Şablonu) [[13:47](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=827)]

- Haftanın en yüksek seviyesinin (High of the Week) genellikle Pazartesi/Salı günü oluştuğu ve önceki günün/haftanın likiditesini temizledikten sonra (Liquidity Pool Raid) ana hareketin başladığı gösterilir [[13:55](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=835)].
- Günlük chart'taki likidite temizliğinin ardından daha alt zaman dilimlerindeki (4H/1H) Discount PD Array'lerin nokta atışı hedef haline geldiği özetlenir [[14:49](https://www.youtube.com/watch?v=YV4fEF4d2wA&t=889)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  ICT Mentorship Core Content - Month 07 - Short Term Trading Blending IPDA Data Ranges & PD Arrays

  The Inner Circle Trader · 219K views

   [Open in ICT Mentorship Core Content - Month 07 - Short Term Trading Blending IPDA Data Ranges & PD Arrays](http://www.youtube.com/watch?v=YV4fEF4d2wA)](http://www.youtube.com/watch?v=YV4fEF4d2wA)

  ![](https://i.ytimg.com/vi/YV4fEF4d2wA/maxresdefault.jpg)
