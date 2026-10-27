# ICT Mentorship Core Content - Month 03 - Institutional Order Flow

<https://www.youtube.com/watch?v=PQkcFbr61FI>

**Inner Circle Trader (ICT) – Month 03: Institutional Order Flow** videosundaki öne çıkan ve detaylı anlatılan önemli noktalar şunlardır:

### 1. **Institutional Order Flow (Kurumsal Emir Akışı) Mantığı**

- **Market Efficiency Paradigm:** Kurumsal yapının ana amacı, piyasadaki **maksimum likiditeyi (maximum level of liquidity)** bulmak ve fiyatı oraya çekmektir [[02:51](https://www.youtube.com/watch?v=PQkcFbr61FI&t=171)].
- **Balinaları (Large Funds/Wholesales) Takip Etmek:** Algoritmalar ve bankalar bireysel (retail) tüccarların küçük bakiyelerini değil, milyarlarca dolar yöneten büyük fonların **Monthly** ve **Weekly** grafiklerdeki emsalsiz likidite havuzlarını hedefler [[13:00](https://www.youtube.com/watch?v=PQkcFbr61FI&t=780)], [[28:15](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1695)].
- **Piyasa İki Ana Modda Çalışır:**

  1. Likidite havuzlarına (**Sell Stops** / **Buy Stops**) ulaşmak/süpürmek (Liquidity Sweeps) [[03:51](https://www.youtube.com/watch?v=PQkcFbr61FI&t=231)].
  2. Dengesizlikleri (**Liquidity Void** / **FVG**) doldurmak ve **Order Block**’lara geri dönerek fiyatı yeniden dengelemek (Rebalancing) [[03:21](https://www.youtube.com/watch?v=PQkcFbr61FI&t=201)].

### 2. **Candle Bodies (Mum Gövdeleri) vs. Wicks (Fitiller/Iğneler)**

- **Hacim Gövdelerdedir:** Gerçek **Institutional Volume** (kurumsal hacim) ve interbank fiyatlaması mumların **gövde kapanışlarında/açılışlarında** saklıdır [[06:12](https://www.youtube.com/watch?v=PQkcFbr61FI&t=372)].
- **Fitiller Retail Alanıdır:** Fitiller (wicks) genellikle bireysel yatırımcı platformlarındaki fiyat kaymalarını, broker spread farklarını ve aşırı fiyat patlamalarını (erroneous / extreme price delivery) temsil eder [[05:19](https://www.youtube.com/watch?v=PQkcFbr61FI&t=319)], [[06:19](https://www.youtube.com/watch?v=PQkcFbr61FI&t=379)].
- **Analiz Kuralı:** Likidite ve seviye analizi yaparken odak noktası mumların gövdeleri olmalıdır; fiyatın gövdelerin altına/üstüne sarması likidite süpürmek için yeterlidir, fitilin en uç noktasını kırması şart değildir [[06:52](https://www.youtube.com/watch?v=PQkcFbr61FI&t=412)], [[11:32](https://www.youtube.com/watch?v=PQkcFbr61FI&t=692)].

### 3. **Top-Down Analysis (Yukarıdan Aşağıya Grafik Analizi)**

- **Monthly (Aylık Grafik):**

  - Yönsel beklenti (directional bias) ve ana likidite havuzları **Monthly** grafikte belirlenir [[01:26](https://www.youtube.com/watch?v=PQkcFbr61FI&t=86)], [[07:43](https://www.youtube.com/watch?v=PQkcFbr61FI&t=463)].
  - Piyasanın ana hedefi (Bullish / Bearish Order Flow) aylık yapılardaki Order Block ve Liquidity Void'ler üzerinden tespit edilir [[11:45](https://www.youtube.com/watch?v=PQkcFbr61FI&t=705)].
- **Weekly (Haftalık Grafik):**

  - Monthly'de belirlenen **Bearish/Bullish** alanlar Weekly grafiğe aktarılarak genel trend ve piyasa yapısı dilimlere ayrılır [[12:00](https://www.youtube.com/watch?v=PQkcFbr61FI&t=720)].
- **Daily (Günlük Grafik):**

  - Giriş (entry) hassasiyetinin sağlandığı yerdir. Yüksek zaman dilimindeki (Monthly/Weekly) hedeflere doğru Daily grafikte oluşan **Order Block**, **Breaker** veya **Mitigation Block** yapıları işlem fırsatı sunar [[21:37](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1297)], [[28:08](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1688)].

### 4. **Ana Konseptler ve Mekanizmaları**

- **Order Blocks (Kurumsal Emir Blokları):**

  - **Bullish Order Block:** Yönün yukarı beklendiği dönemde, yükseliş dalgasından önceki **son düşüş mumu (down candle)** [[04:23](https://www.youtube.com/watch?v=PQkcFbr61FI&t=263)], [[17:49](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1069)].
  - **Bearish Order Block:** Yönün aşağı beklendiği dönemde, düşüş dalgasından önceki **son yükseliş mumu (up candle)** [[04:34](https://www.youtube.com/watch?v=PQkcFbr61FI&t=274)], [[15:27](https://www.youtube.com/watch?v=PQkcFbr61FI&t=927)].
  - **Mean Threshold:** Bir Order Block mumunun tam orta noktası (%50 seviyesi) fiyatın en hassas tepki vereceği yerdir [[05:01](https://www.youtube.com/watch?v=PQkcFbr61FI&t=301)].
- **Liquidity Void (Likidite Boşluğu):**

  - Fiyatın tek yönlü ve agresif şekilde düşmesi (ör. peş peşe siyah/kırmızı mumlar) piyasada dengesizlik yaratır [[03:27](https://www.youtube.com/watch?v=PQkcFbr61FI&t=207)], [[04:38](https://www.youtube.com/watch?v=PQkcFbr61FI&t=278)].
  - Piyasa mekanizması gereği, sell-side sunulan bu alana daha sonra buy-side teklif (yeşil/yükseliş mumları) verilerek boşluk kapatılmalıdır [[03:41](https://www.youtube.com/watch?v=PQkcFbr61FI&t=221)], [[04:42](https://www.youtube.com/watch?v=PQkcFbr61FI&t=282)].
- **Mitigation Block (Yumuşatma / Pozisyon Kapatma Blokları):**

  - Kurumsallar fiyatı yukarı/aşağı sürerken kendi açtıkları karşıt pozisyonları (hedging) zararsız veya başabaş kapatmak için fiyatı eski seviyeye geri getirirler [[15:09](https://www.youtube.com/watch?v=PQkcFbr61FI&t=909)], [[19:09](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1149)].
  - Zirve/dip likiditesi alındıktan sonra fiyatın bu alana tekrar gelmesi, kurumsalların zararda kalan pozisyonlarını likide edip yeni net pozisyonlar açmasını sağlar [[19:36](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1176)].
- **Breaker Block:**

  - Likiditeyi süpüren (eski tepeyi/dibi kıran) ancak başarısız olup yapıyı tersine kıran mum gruplarıdır [[14:43](https://www.youtube.com/watch?v=PQkcFbr61FI&t=883)], [[26:07](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1567)]. Fiyat bu kırılım mumuna geri döndüğünde re-entry (yeniden giriş) fırsatı verir [[14:43](https://www.youtube.com/watch?v=PQkcFbr61FI&t=883)].

### 5. **Market Maker Profile (Piyasa Yapıcı Profili)**

- Piyasa bir zirveden diğerine veya bir likidite havuzundan diğerine giderken sürekli bir döngü takip eder:

  1. **Consolidation** (Birikim) [[17:06](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1026)]
  2. **Accumulation / Re-accumulation** (Toplama) [[17:06](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1026)]
  3. **Smart Money Reversal** (Akıllı Para Dönüşü) [[17:06](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1026)]
  4. **Redistribution** (Dağıtım) [[17:06](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1026)]
  5. **Liquidity Sweep** (Likidite Temizliği) [[17:06](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1026)]

Bu derste anlatılan tüm bu kuralların ana mesajı: **Günlük veya daha düşük zaman dilimlerinde işlem yaparken, fiyatın Monthly ve Weekly zaman dilimlerindeki büyük oyuncuların (whales) likidite alanlarına doğru çekildiğini bilmek ve işlemlerinizi bu doğrultuda kurgulamaktır** [[28:59](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1739)], [[29:18](https://www.youtube.com/watch?v=PQkcFbr61FI&t=1758)].

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Mentorship Core Content - Month 03 - Institutional Order Flow

The Inner Circle Trader · 594K views

 [Open in ICT Mentorship Core Content - Month 03 - Institutional Order Flow](http://www.youtube.com/watch?v=PQkcFbr61FI)](http://www.youtube.com/watch?v=PQkcFbr61FI)

![](https://i.ytimg.com/vi/PQkcFbr61FI/maxresdefault.jpg)
