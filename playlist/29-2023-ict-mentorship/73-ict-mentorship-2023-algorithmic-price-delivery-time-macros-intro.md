# ICT Mentorship 2023 - Algorithmic Price Delivery & Time Macros Intro

<https://www.youtube.com/watch?v=fXVJnBVizYY>

Bu video, Inner Circle Trader (ICT) konseptlerinden **"ICT Gems: How Time Delivers Liquidity"** başlıklı içeriğe aittir. Videonun ana odağı, piyasalarda fiyat hareketinden ziyade **zamanın (Time)** likiditeyi ve fiyat akışını nasıl yönlendirdiğidir.

İşte videonun detaylı ve maddeler halinde özeti:

## 📌 1. Bir Trader'ın Temel Görevi (A Trader's Job)

- Trader'ın asıl görevi, piyasada kendisine bir **Edge** (üstünlük/avantaj) sağlayan bir sistem kurmak, bunu tutarlı bir şekilde tekrarlamak ve **Law of Large Numbers** (Büyük Sayılar Yasası) çerçevesinde istatistiksel üstünlük elde etmektir.
- **Time & Price Mechanics:** Fiyatlar rastgele hareket etmez; piyasa algoritması önce **Time** (zaman) parametresini çalıştırır, ardından fiyatı **Liquidity** veya **Inefficiency** (Fair Value Gap - FVG) alanlarına doğru yönlendirir.

## ⏰ 2. Time, Kill Zones & Key Sessions

Piyasalarda volatilite ve hacmin yoğunlaştığı belirli zaman dilimleri vardır:

- **Kill Zone Dönemleri:**

  - **London Open Kill Zone:** 02:00 – 05:00 AM (EST)
  - **New York Open Kill Zone:** 07:00 – 09:00 AM (EST)
  - **New York AM Session:** 08:30 AM – 12:00 PM (EST)
- **Silver Bullet Window:** 10:00 – 11:00 AM (EST) gibi spesifik likidite pencereleri.
- Bu zaman dilimlerinde oluşan **Displacement** (sert fiyat hareketi), yüksek olasılıklı **FVG (Fair Value Gap)** yapılarının oluşmasını sağlar.

## ⚡ 3. ICT Macros Nedir ve Nasıl Çalışır?

- **Macro:** Fiyat hareketinde genellikle 20 dakika civarında süren ve algoritmanın fiyatı belirli bir hedefe sürüklediği özel zaman pencereleridir.
- **Önemli Macro Saat Aralıkları (EST / New York Time):**

  - `08:50 - 09:10` (Morning Macro)
  - `09:50 - 10:10` (Önemli değişim/dönüş penceresi)
  - `10:50 - 11:10`
  - `11:50 - 12:10` (Midday / Lunch Macro)
  - `13:10 - 13:40` & `15:15 - 15:45` (Afternoon / Close Macros)
- **Macro Mekaniği:** Algoritma bu pencerelerde piyasada bulunan **Sell-side Liquidity** veya **Buy-side Liquidity** seviyelerine doğru bir koşu (Run) başlatır. Eğer bu pencerelerde belirgin bir hareket veya **Inefficiency** avı yoksa, o seansta işlem yapmamak (Stop Trading) daha mantıklıdır.

## 🎯 4. Fiyat Hareketlerinin Dinamikleri & Tape Reading

- **Tape Reading & Context:** Yalnızca Macro saatini bilmek yeterli değildir. Trader'ın **Directional Bias** (yön beklentisi), **Higher Timeframe (HTF) Context** ve **Liquidity Pool** yerlerini doğru okuması gerekir.
- **Liquidity Targets:** Fiyat genellikle önceki günlerin/haftaların en yüksek ve en düşük seviyelerine (**Previous Daily High/Low - PDH/PDL**) veya likidite boşluklarına (**FVG / Inefficiencies**) çekilir.
- **News Events & Traps:** Non-Farm Payroll (NFP) veya yüksek etkili haber zamanlarında piyasa, yön değiştirmeden önce perakende trader'ları yanlış yönde tuzağa düşürmek (**Liquidity Trap / Fakeout**) için ilk sert hareketi yapar.

## 📊 5. Order Blocks & Opening Ranges

- **Bullish / Bearish Order Block:** Stop seviyeleri temizlendikten (**Liquidity Sweep**) sonra gerçekleşen sert dönüşlerde, kurumsal girişlerin yapıldığı ana mum yapılarıdır.
- **Opening Range (Açılış Aralığı):** Seans açılışındaki fiyat aralığı, günün geri kalanındaki likidite arayışı ve yön tayini açısından kilit role sahiptir.
- **Lunch Hour Behavior:** Öğle saatlerindeki Macro dönemi, piyasanın ya konsolide olduğu ya da sabah seansında bırakılan likiditeleri temizlediği bir geçiş evresidir.

## 💡 Önemli Çıkarımlar (Key Takeaways)

1. **Timing Control:** Macro saatleri **Direction (Yön)** vermez, yalnızca **Timing (Zamanlama)** sunar. Yönü belirleyen şey **Higher Timeframe Bias** ve **Liquidity Target**'tır.
2. **No Setup = No Trade:** Bir Macro penceresi içinde fiyat Liquidity veya Inefficiency arayışına girmeyip yatay kalıyorsa, o seans için işlem pas geçilmelidir.
3. **Execution:** Macro saatleri ile 1m, 3m veya 5m grafiklerdeki **Order Block**, **FVG** ve **Liquidity Sweep** yapıları birleştirildiğinde yüksek başarı oranına sahip kurulumlar ortaya çıkar.
