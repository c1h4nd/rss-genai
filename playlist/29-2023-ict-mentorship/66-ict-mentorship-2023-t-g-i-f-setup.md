# ICT Mentorship 2023 - T.G.I.F. Setup

<https://www.youtube.com/watch?v=wTR-vhOdMgo>

İstediğiniz YouTube videosu (**Inner Circle Trader / ICT – Mentorship 2023: T.G.I.F. Setup**) detaylı ve maddeler halinde özetlenmiştir.

Orijinal finans/ICT terimleri ve konsept adları **İngilizce** bırakılmıştır.

## 📌 Genel Bakış & Tanım

- **T.G.I.F. (Thank God It's Friday) Setup:** Yalnızca **Cuma günleri** uygulanan, tarih/gün bazlı (date-based algorithmic) bir ICT ticaret modelidir.
- **Temel Amacı:** Haftalık mumun (Weekly Candle) oluşturduğu yönlü hareketten (directional expansion/expansion move) sonra, haftanın kapanışına doğru gerçekleşen **Weekly Range Retracement** (haftalık aralığa geri çekilme) hareketini yakalamaktır.
- **Ne Değildir?:** Tam bir trend dönüşü (Full Trend Reversal) değildir; sadece haftalık mumun aşırı genişlemesi sonucu oluşan bir **Draw on Liquidity** (likidite mıknatısı / kar realizasyonu) geri çekilmesidir.
- **Kullanılan Piyasalar:** Forex, Index Futures (NQ, ES), Crypto ve Commodities dahil **tüm finansal enstrümanlarda** geçerlidir.

## ⚙️ Modelin Çalışma Mantığı & Algoritmik Yapısı

- **Institutional Order Flow & Profit Taking:** Hafta boyunca pozisyon biriktiren akıllı para (Smart Money) ve kurumsal oyuncular, Cuma günü kar realizasyonuna (position squaring) gider.
- **Buy/Sell Side Liquidity Sweep:** Cuma sabahı ya da öğle saatlerine kadar piyasa, haftanın en yüksek (**Weekly High**) veya en düşük (**Weekly Low**) seviyesini yapar (Genellikle bir *Judas Swing* veya likidite temizliği ile).
- **Retail Trap:** Perakende (retail) tüccarlar Cuma günü breakout veya devam formasyonları (ör. Bull/Bear Flag) beklerken, piyasa tam tersine algoritmik bir çekilme başlatır.

## 📐 Hedefleme ve Fibonacci Kuralları (20% – 30% Rule)

- **Weekly Range Ölçümü:**

  - Pazartesi açılışından Cuma günü saat **1:30 PM - 2:00 PM NY Time** civarında oluşan haftalık uç noktaya (Highest High veya Lowest Low) kadar bir Fibonacci çekilir.
- **Ideal Target Zone (Tatlı Nokta):**

  - Primary Target (Ana Hedef): **0.20 (%20 Retracement)**.
  - Secondary Target (İkinci Hedef): **0.30 (%30 Retracement)**.
  - Extended Target: Nadiren %40 veya %50 (Equilibrium) seviyelerine kadar uzayabilir.
- **Örnek (Bullish Week):**

  - Hafta boyunca yukarı yönlü (Bullish) bir hareket olduysa, Cuma günü **Weekly High** yapıldıktan sonra hedeflenen alan: Weekly High'dan aşağı doğru hesaplanan **%20-%30 Weekly Range** çekilmesidir.

## ⏳ Zaman Dilimi, Oturumlar & Kurallar (Rules of Engagement)

- **Execution Windows (Zaman Pencereleri):**

  - **Weekly Extreme Formation:** Weekly High veya Weekly Low genellikle Cuma **AM Session** (sabah) veya en geç **1:30 PM – 2:00 PM NY Time** arasında tamamlanır.
  - **Entry Window:** İşlem girişleri ağırlıklı olarak **2:00 PM – 3:00 PM PM Session (NY PM Silver Bullet Window)** süresince aranır.
- **Gerekli Ön Koşullar (Prerequisites):**

  1. **Directional Week:** Haftanın net bir yönü (trend) olmalıdır.
  2. **Higher Timeframe PD Array Target:** Fiyatın günlük (D1) veya 4 saatlik (H4) grafikte bir **Premium PD Array** (Short için) veya **Discount PD Array** (Long için) seviyesine ulaşmış olması gerekir.
  3. **Lower Timeframe Confirmation:** İşlem için alt zaman dilimlerinde (M5 / M15) bir **Market Structure Shift (MSS)** veya **Change in State of Delivery (CISD)** gerçekleşmelidir.

## 🎯 Giriş ve Risk Yönetimi (Entry & Execution)

- **Giriş Tetikleyicileri (Entry Models):**

  - Lower Timeframe'de MSS oluştuktan sonra oluşan **Fair Value Gap (FVG)**, **Order Block (OB)** veya **Breaker Block** konseptleri üzerinden işleme girilir.
- **Stop Loss Yeri:**

  - Muhafazakar: Oluşan **Weekly High / Weekly Low** seviyesinin hemen üstü/altı.
  - Agresif: PM Session'da yapıyı kıran son salınımın (**Structure Shift High/Low**) üzeri/altı.
- **Take Profit Strategy:**

  - Pozisyonun büyük kısmı **%20 ve %30 Fibonacci seviyelerinde** kademeli (partial exit) olarak kapatılır.
  - Tüm pozisyonlar haftasonu riskini almamak adına **Cuma piyasa kapanışından önce (Market Close)** tamamen kapatılmalıdır.

## ⚠️ Önemli Uyarılar & İstisnalar (Exceptions)

- **All-Time Highs (ATH) / All-Time Lows (ATL):** Fiyat All-Time High yapıyorsa ve tavan/direnç görünmüyorsa **TGIF modeli uygulanmaz / pas geçilir** (çünkü fiyat keşif modundadır, ne kadar uzayacağı kestirilemez).
- **No Setup = No Trade:** Cuma günü haftalık uç nokta netleşmediyse ya da alt zaman diliminde MSS gerçekleşmediyse zorlama işlem alınmamalıdır.
