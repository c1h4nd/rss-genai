# ICT Mentorship 2023 - September 22, 2023 - High Frequency Trading Algorithmic Entries

<https://www.youtube.com/watch?v=tjnir-o4rsQ>

Bu video, Inner Circle Trader (ICT) kanalının **"ICT Mentorship 2023 - September 22, 2023 - High Frequency Trading Algorithmic Entries"** başlıklı dersine aittir.

Videoda ICT (Michael J. Huddleston), yüksek frekanslı algoritmik fiyat hareketlerini, alt zaman dilimlerindeki (özellikle 15 saniyelik grafikler) giriş stratejilerini ve **Breaker Block** ile **Order Block** birleşimini detaylı olarak incelemektedir.

## 📌 Genel Özet ve Konu Başlıkları

- **Video Başlığı:** ICT Mentorship 2023 - High Frequency Trading Algorithmic Entries
- **Tarih / Süre:** 22 Eylül 2023 / ~12 dakika
- **Odak Konusu:** High Frequency Trading (HFT) algoritmalarının bıraktığı izler, düşük zaman diliminde (15-second chart) hassas (precise) işlem girişleri ve Breaker yapısının kullanımı.

## 📑 Detaylı Video Özeti (Bullet Points)

### 1. Üst Zaman Dilimi Çerçevesi (Higher Timeframe Context)

- **Higher Timeframe PD Array Retest:** Fiyat öncelikle üst zaman dilimindeki kilit bir seviyeye, özellikle bir **Order Block** alanına geri çekilme (retest) yapar.
- **Algoritmik Tepki:** Algoritmik fiyat teslimatı (Algorithmic Price Delivery), bu ana Order Block seviyesine temas edildiği anda hızlanır ve tepki üretir.

### 2. Alt Zaman Dilimine İniş (15-Second Chart Management)

- **Zaman Dilimi Ölçekleme:** Büyük zaman dilimindeki yapı doğrulandıktan sonra, giriş hassasiyetini yakalamak için **15-second chart** (15 saniyelik grafik) gibi ultra düşük zaman dilimlerine geçilir.
- **High Frequency Trading (HFT) İmzaları:** HFT algoritmalarının yüksek frekanslı emir iletimi sırasında grafik üzerinde oluşturduğu hızlı gap'ler ve ani fiyat kaymaları incelenir.

### 3. Giriş Stratejisi ve Breaker Block Kullanımı

- **Bullish Breaker Formation:** Fiyatın önceki **Liquidity Sweep** (likidite temizliği) sonrası yapısal kırılım yapmasıyla oluşan **Bullish Breaker Block** belirlenir.
- **Fair Value Gap (FVG) ile Kesişim:** Breaker seviyesinin bir **FVG (Fair Value Gap)** ile çakıştığı noktalar (Confluence) en yüksek olasılıklı (high-probability) giriş bölgesi olarak seçilir.
- **Algorithmic Entry (Giriş İcrası):** Fiyatın bu Breaker / FVG alanına yeniden girmesiyle birlikte (mitigation) işleme dahil olunur.

### 4. Risk Yönetimi ve Hedefleme (Risk & Target Management)

- **Stop-Loss Yerleşimi:** Stop seviyesi, yapıyı bozan son swing low'un veya Breaker Block'un tabanının hemen altına konumlandırılır.
- **Draw on Liquidity (Hedefler):** Kar alma hedefleri (Take Profit) olarak üst zaman dilimindeki karşıt **Buyside Liquidity (BSL)** havuzları veya eski salınım zirveleri (Old Highs) hedeflenir.
- **Execution & Trade Management:** İşleme girdikten sonra fiyatın kararlı bir şekilde yükselmesi beklenir; algoritmik modda geri çekilmelerin sığ kalması ve momentumun korunması gerektiği vurgulanır.

Bu konseptleri grafik üzerinde uygulamak veya daha derinlemesine incelemek isterseniz:
