# ICT Mentorship Core Content - Month 06 - The Million Dollar Swing Setup

<https://www.youtube.com/watch?v=VL4YLTRerHY>

Videodaki **"The Million Dollar Swing Setup"** modelinin işlem adımları ve önemli noktaları detaylı olarak aşağıda listelenmiştir:

### 1. Temel Mantık ve Yaklaşım

- **Adı Nereden Geliyor?**: Milyon dolar kazandıracağı anlamına gelmez; ICT'nin teknik araçları içinde en yüksek olasılığa ve güvene sahip **Swing Trade** koşullarını ifade eder [[00:28](https://www.youtube.com/watch?v=VL4YLTRerHY&t=28)].
- **Disiplin ve Eleme Sistemi**: İşlem adımları aşamalı bir karar ağacı (flowchart) gibidir [[02:44](https://www.youtube.com/watch?v=VL4YLTRerHY&t=164)]. Bir aşamadaki şart sağlanmazsa sonraki aşamaya geçilmez; swing trade aranmaz, short-term/day trading'e geçilir veya beklenir [[03:14](https://www.youtube.com/watch?v=VL4YLTRerHY&t=194)].

### 2. Adım Adım Kurulum Süreci (Top-Down Process)

#### A. Seasonal Tendency (Mevsimsel Eğilim)

- **İlk Filtre**: Mevsimsel bir alım/satım eğilimi var mı? Yoksa swing trade aranmaz [[03:21](https://www.youtube.com/watch?v=VL4YLTRerHY&t=201)].
- Modelin tarihsel başarı olasılığının temelini bu tarihsel tekrarlar oluşturur [[04:00](https://www.youtube.com/watch?v=VL4YLTRerHY&t=240)].

#### B. Major Market Analysis (Ana Piyasa Analizi)

- **Trend Şartı**: Interest rate piyasaları ve/veya US Dollar Index (DXY) trend halinde mi? [[04:24](https://www.youtube.com/watch?v=VL4YLTRerHY&t=264)]
- Commodities veya Stock markets trend halinde mi? [[05:17](https://www.youtube.com/watch?v=VL4YLTRerHY&t=317)]
- Her gruptan en az bir piyasanın trend halinde olması gerekir [[05:37](https://www.youtube.com/watch?v=VL4YLTRerHY&t=337)].

#### C. Intermarket Analysis & COT Data (Piyasalar Arası Analiz)

- **Commercials (COT Report)**: Son 12 ayın net pozisyon aralığı (Range High & Low) dikkate alınır [[07:11](https://www.youtube.com/watch?v=VL4YLTRerHY&t=431)].

  - **Bullish Setup**: Commercials net short olsa bile son 12 ayın aralığına göre short pozisyonlarını azaltıyor (buying side) veya net long duruma geçiyorsa [[06:51](https://www.youtube.com/watch?v=VL4YLTRerHY&t=411)].
  - **Bearish Setup**: Commercials net long pozisyonlarını azaltıyor veya net short durumundaysa [[10:48](https://www.youtube.com/watch?v=VL4YLTRerHY&t=648)].
- **DXY Korelasyonu & SMT Divergence**:

  - Bullish metal/currency işlemleri için DXY'nin düşüş eğiliminde olması veya SMT Divergence ile bunu desteklemesi gerekir [[08:43](https://www.youtube.com/watch?v=VL4YLTRerHY&t=523)].
- **Commodity & Open Interest (OI) Filter**:

  - **Bullish**: Emtialar yükseliyor, Open Interest %10-15 veya daha fazla düşüyorsa (Commercial Short Covering göstergesi) [[09:51](https://www.youtube.com/watch?v=VL4YLTRerHY&t=591)].
  - **Bearish**: Emtialar düşüyor, Open Interest %10-15 veya daha fazla artıyorsa (Commercial Short Selling göstergesi) [[12:00](https://www.youtube.com/watch?v=VL4YLTRerHY&t=720)].

#### D. Top-Down Analysis (Zaman Dilimleri ve Yapı)

- **9 - 18 Aylık Fiyat Geçmişi**: Fiyatın ana yönünü ve yapısını anlamak için analiz edilir [[12:21](https://www.youtube.com/watch?v=VL4YLTRerHY&t=741)].
- **PD Array İşaretleme**: Monthly, Weekly, Daily ve 4-Hour zaman dilimlerindeki tüm PD Array'ler belirlenip 4H grafiğine taşınır [[12:31](https://www.youtube.com/watch?v=VL4YLTRerHY&t=751)].
- **IPDA Data Ranges**: Günlük grafikte 20, 40 ve 60 günlük Lookback aralıklarına bakılır [[12:41](https://www.youtube.com/watch?v=VL4YLTRerHY&t=761)].
- **Kurumsal Akış (Institutional Order Flow)**: IPDA aralıkları ile PD Array'lerin çakıştığı (confluence) noktalar tespit edilir [[13:03](https://www.youtube.com/watch?v=VL4YLTRerHY&t=783)].

  - *Bullish*: Monthly / Weekly / Daily **Discount Array**'lere odaklanılır [[13:22](https://www.youtube.com/watch?v=VL4YLTRerHY&t=802)].
  - *Bearish*: Monthly / Weekly / Daily **Premium Array**'lere odaklanılır [[13:28](https://www.youtube.com/watch?v=VL4YLTRerHY&t=808)].

### 3. İşlem Giriş Teknikleri (Execution Types)

- **Stop Order (Piyasa Emri / Stop ile Giriş)**:

  - Bullish / Bearish **Breaker** [[14:24](https://www.youtube.com/watch?v=VL4YLTRerHY&t=864)]
  - Bullish / Bearish **Mitigation Block** [[14:24](https://www.youtube.com/watch?v=VL4YLTRerHY&t=864)]
  - **Fair Value Gap (FVG)** / Liquidity Void [[14:33](https://www.youtube.com/watch?v=VL4YLTRerHY&t=873)]
- **Limit Order (Limit Emirle Giriş)**:

  - Bullish / Bearish **Order Block (OB)** [[14:42](https://www.youtube.com/watch?v=VL4YLTRerHY&t=882)]
  - **Rejection Block** [[14:42](https://www.youtube.com/watch?v=VL4YLTRerHY&t=882)]
  - Old High / Old Low ihlalleri (Liquidity Runs) [[14:42](https://www.youtube.com/watch?v=VL4YLTRerHY&t=882)]

### 4. Trade Management (İşlem Yönetimi & Kar Al/Stop Kuralları)

- **Stop Loss Hareketleri**:

  - Fiyat hedeflenen yönün **1/3'üne** ulaşana kadar Stop Loss ilk koyulduğu yerde sabit tutulur [[16:37](https://www.youtube.com/watch?v=VL4YLTRerHY&t=997)].
  - Hedeflenen hedefin **1/4'üne (%25)** ulaşıldığında pozisyonun %20 - %30'u kapatılır (Partial Take Profit) [[16:47](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1007)].
  - **Break Even (Başabaş)**: Stop Loss, YALNIZCA ilk kâr alındıktan sonra Break Even seviyesine çekilir (Daha önce kesinlikle çekilmez) [[16:57](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1017)].
- **Re-entry & Scaling**:

  - Fiyat hedefin **%50'sine (Equilibrium)** ulaştığında geri çekilmelerde satılan %25'lik kısım yeni bir Discount/Premium Array üzerinden pozisyona geri eklenebilir [[17:06](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1026)].
- **Stop Run Beklentisi**:

  - %50 (Equilibrium) seviyesi geçildikten sonra piyasanın likidite temizliği (Stop Run) yapması oldukça yaygındır. Bu yüzden stop seviyeleri erken sürüklenmemelidir [[17:23](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1043)].
- **Hedef ve Kapanış**:

  - Karşı taraftaki Monthly / Weekly / Daily PD Array hedefine gelindiğinde pozisyonun tamamı veya %75-%80'i kapatılır [[17:16](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1036)]. Kalan kısım için 4-Hour short-term high/low seviyeleri altında/üstünde Trail Stop uygulanır [[17:23](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1043)].

### 5. Örnek İnceleme: Gold (Altın) İşlem Kurgusu

- **Seasonal Tendency**: Aralık ortasından Ocak/Şubat aylarına kadar Altın'da güçlü bir yükseliş eğilimi bulunur [[19:24](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1164)].
- **Analiz Adımları**:

  - Bond piyasası ve DXY trend halindeydi [[20:26](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1226)].
  - COT Raporunda Commercials net short'larını ciddi oranda azaltmıştı [[21:31](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1291)].
  - Open Interest 100.000 kontratın üzerinde sert düşüş gösterdi [[21:49](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1309)].
  - Emtialar (Soybeans, Copper, Crude Oil) genel olarak güç gösteriyordu [[22:48](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1368)].
- **Seviye Analizi & Fraktal Yapı**:

  - Monthly Bullish Order Block seviyesi olan **1142** dip destek olarak belirlendi [[23:45](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1425)].
  - Ana hedef **1255 - 1260** Weekly Premium Array olarak tespit edildi [[24:21](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1461)].
  - Hedef aralığının **Equilibrium (%50) noktası 1200** seviyesiydi [[25:59](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1559)]. Fiyat 1200'ü kırdıktan sonra beklendiği gibi aşağı doğru Likidite Temizliği (Stop Run) yaptı [[26:07](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1567)].
  - Daily Order Block (1175-1180) ve Fibonacci extension (1.272 / 1.618) çakışmasıyla 1260 hedefine doğru ikinci büyük dalga gerçekleşti [[27:52](https://www.youtube.com/watch?v=VL4YLTRerHY&t=1672)].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    ICT Mentorship Core Content - Month 06 - The Million Dollar Swing Setup

    The Inner Circle Trader · 155K views

     [Open in ICT Mentorship Core Content - Month 06 - The Million Dollar Swing Setup](http://www.youtube.com/watch?v=VL4YLTRerHY)](http://www.youtube.com/watch?v=VL4YLTRerHY)

    ![](https://i.ytimg.com/vi/VL4YLTRerHY/maxresdefault.jpg)
