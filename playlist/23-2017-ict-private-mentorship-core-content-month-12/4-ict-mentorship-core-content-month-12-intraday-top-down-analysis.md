# ICT Mentorship Core Content - Month 12 - Intraday Top Down Analysis

<https://www.youtube.com/watch?v=Oec_0NM_OeY>

ICT Mentorship Month 12 dersinin (**Intraday Top Down Analysis**) önemli yerlerinin detaylı bir dökümü:

- **Top-Down Analysis Perspective ([[00:32](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=32)]):**

  - Analize **4-hour (4 saatlik)** grafik ile başlanır ve sırasıyla alt zaman dilimlerine (**60m, 30m, 15m, 5m**) inilerek intraday directional bias (yönsel önyargı) belirlenir.
  - Haftalık, günlük ve aylık analiz perspektifleri 4 saatlik grafik incelenirken zaten hesaba katılmış olmalıdır.
- **Analysis Checklist & Time Elements ([[01:11](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=71)]):**

  - **Day of the Week:** İşlem yapılan haftanın günü (özellikle Pazartesi-Çarşamba aralığı) ve olası haftalık şablonlar/profiller göz önüne alınır.
  - **True Day & Kill Zones:** True day parametreleri ve belirli seans açılışları (**Kill Zones:** London Open, New York Open, London Close, Asia) takip edilir.
  - **Central Bank Dealers Range (CBDR) & Asian Range ([[02:36](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=156)]):** Konsolidasyon alanları ve potansiyel High/Low of the Day seviyeleri için standart sapmalar (**standard deviations**) hesaplanır.
  - **FLOUT (CBDR + Asian Range Combined) ([[03:05](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=185)]):** CBDR ve Asian Range zaman dilimlerinin birleştirilerek toplam aralığın yarıya bölünmesiyle elde edilen standart sapmalar kullanılır.
- **Timeframe Breakdown & Refinement ([[04:18](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=258)]):**

  - 4 saatlik grafikten sonra 30 dakikalık veya 15 dakikalık grafiklere inilerek işlemler **5 dakikalık (5m)** grafikte refine edilir (giriş ve execution).
  - Alt zaman dilimlerinde **Fair Value Gaps (FVG)** ve **Order Block** gibi PD Array'lerin daha net görülmesi amaçlanır.
- **Day of the Week Dynamics ([[06:21](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=381)]):**

  - Yüksek zaman dilimindeki bias bearish ise Pazartesi, Salı, Çarşamba günleri **short**; bullish ise **long** fırsatları aranır.
  - Eğer hafta başında beklenen hareket gelmezse, **Thursday ve Friday (Perşembe/Cuma)** şablonlarına odaklanılır.
- **Time of Day & Kill Zones ([[07:47](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=467)]):**

  - **London Open:** Yüksek zaman dilimi bullish ise *Low of the Day*, bearish ise *High of the Day* hedeflenir.
  - **New York Open:** Londra'da kaçırılan fırsatlar için yeniden konumlanma veya seans içi tersine dönüşler (**reversal**) beklenir.
  - **Profit Taking:** Sabah **10:00 - 11:00 (New York time)** aralığında pozisyonların kapatılması/hafifletilmesi planlanır.
- **Standard Deviations & Confluences ([[08:41](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=521)]):**

  - *Bullish:* CBDR, Asian Range veya FLOUT'un negatif standart sapmaları (**-1, -2, -3**) alt zaman dilimindeki **discount array**'ler (15m-60m) ile çakıştırılarak long girişler aranır.
  - *Bearish:* Pozitif standart sapmalar (**+1, +2, +3**) üst zaman dilimindeki **premium array**'ler ile çakıştırılarak short girişler aranır.
- **Intraday Profiles & New York Reversals ([[15:43](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=943)]):**

  - 4 saatlik grafik henüz bir discount veya premium array'e temas etmediyse, New York seansı çoğunlukla bir **continuation** (devam) niteliği taşır.
  - Eğer 4 saatlik grafik premium/discount array'e ulaştıysa, New York seansında bir **market reversal** (tersine dönüş) olasılığı yüksektir.
- **Average Daily Range (ADR) Projections ([[17:33](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=1053)]):**

  - 5 günlük ADR projeksiyonları ve Fibonacci uzantıları (**127% ve 162% extensions**), 15m/60m premium/discount array'leri ile çakıştırılarak intraday ekstrem seviyeler belirlenir.
  - Hedeften **10 pip önce** kâr alımı mantıklıdır (aşırı zorlamamak gerekir).
- **ICT Bullish & Bearish Patterns (Go-To Setups) ([[21:01](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=1261)]):**

  - **Pattern 1 (Internal Range Liquidity / Optimal Trade Entry):** Fiyat bir discount array'den seker, FVG bırakır, kısa vadeli bir low/high oluşturur, ardından geri çekilerek FVG ve order block bölgesinden işlem açılır (Optimal Trade Entry - OTE).
  - **Pattern 2 (External Range Liquidity / Turtle Soup):** Beklenen seviyenin hemen öncesinde sahte bir dip/tepe oluşur, ardından stop'lar patlatılır (**stop raid / liquidity pool**). Akıllı para (smart money) bu stop'ları toplayarak ters yönde pozisyon açar.
  - **Pattern 3 (Breaker Entry / Contingency Plan):** İlk fırsat (Turtle Soup) kaçırıldığında, kırılan seviyenin **Breaker** olarak çalışması beklenir ve fiyat geri döndüğünde oradan işleme girilir (veya mevcut pozisyona **pyramiding** yapılır).
- **Gold Market Case Study ([[51:58](https://www.youtube.com/watch?v=Oec_0NM_OeY&t=3118)]):**

  - 4 saatlik ve 1 മണിക്കurluk (hourly) grafikler üzerinde altın (Gold) piyasası üzerinden yukarıdaki konseptlerin (discount array, FVG, OTE, breaker) adım adım nasıl uygulandığı pratik bir örnekle gösterilmiştir.

İlgili YouTube Videosu: <https://www.youtube.com/watch?v=Oec_0NM_OeY>

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Mentorship Core Content - Month 12 - Intraday Top Down Analysis

The Inner Circle Trader · 364K views

 [Open in ICT Mentorship Core Content - Month 12 - Intraday Top Down Analysis](http://www.youtube.com/watch?v=Oec_0NM_OeY)](http://www.youtube.com/watch?v=Oec_0NM_OeY)

![](https://i.ytimg.com/vi/Oec_0NM_OeY/maxresdefault.jpg)
