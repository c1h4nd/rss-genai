# ICT 2024 Mentorship \ September 11, 2024

<https://www.youtube.com/watch?v=A1mLNIoEsq0>

Paylaştığın bağlantı **Inner Circle Trader (ICT) - 2024 Mentorship Series, Lecture #25** videosuna aittir.

Videoda ele alınan ana başlıklar, kavramlar ve teknik detayların maddeler halinde geniş özeti aşağıdadır:

### 1. Temel Konsept: Porous Price Action (Gözenekli Fiyat Hareketi) & Patchwork

- **Porous Price Action Mantığı:** Mum gövdelerinin (candle bodies) üst üste binmediği, aralarında boşlukların ve verimsizliklerin oluştuğu yapılardır. Perakende (retail) tüccarlar için anlamsız görünen bu alanlar, algoritmik fiyatlandırmada eksik bırakılmış verimsiz bölgelerdir.
- **Patchwork (Yama / Onarım) Kavramı:** Fiyat motoru (price engine) bu "porous" bölgelere geri dönerek yeniden teslimat (**algorithmic redelivery**) yapmak zorundadır. Bu geri dönüş işlemine ICT "Patchwork" adını verir.
- **Volume Imbalance İlişkisi:** Porous alanlar, klasik Fair Value Gap (FVG) ve Volume Imbalance yapılarının daha geniş veya düzensiz bir türevidir.

### 2. Algoritmik Fiyat Hareketleri ve HFT Rolü

- **HFT (High-Frequency Trading) Çalışma Şekli:** Fiyat porous bölgeye geri çekildiğinde (**retracement**), HFT algoritmaları ana yön (bias) doğrultusunda agresif bir şekilde pozisyon açar.
- **Liquidity Delivery:**

  - Bearish senaryoda, fiyat yükselerek premium porous bölgeye girdiğinde algoritmalar sürekli *short* emirler iletir.
  - Bullish senaryoda, fiyat düşerek discount porous bölgeye girdiğinde algoritmalar *long* emirler iletir.
- **Görünmez Likidite (Invisibility of Retail Drivers):** Bu hareketlerin arkasında insan psikolojisi değil, tamamen kodlanmış teslimat algoritmaları yer alır.

### 3. İşlem Kurulumu ve Risk Yönetimi (Trade Setup & Execution)

- **Giriş Stratejisi (Entry):** Fiyatın bias yönünde hareket ettikten sonra, bırakılan porous bölgeye (veya FVG/Patchwork alanına) yeniden girmesini (re-entry) beklemek.
- **Stop Loss Yerleşimi:** Porous alanın en uç sınırının (**far boundary**) hemen ötesine stop koyulmalıdır.
- **Kâr Al (Take Profit / Partial Targets):**

  - **İlk Kar Alım Noktası (First Partial):** Porous alanın orta noktası olan **Consequent Encroachment (CE)** seviyesi.
  - **Ana Hedef (Full Target):** Porous aralığının diğer ucu.
  - **Genişletilmiş Hedef (Extended Target):** Bölge kapandıktan ("patched" olduktan) sonra, grafikteki likidite havuzları (**Relative Equal Lows / Highs**, **Liquidity Pools**).

### 4. Piyasa Koşulları ve Önemli Uyarılar

- **Zaman Dilimi ve Context:** Porous price action yapıları yönü olmayan, konsolide (directionless consolidation) piyasalarda daha az güvenilirdir. Net bir **Higher Timeframe (HTF) Bias** ile birlikte takip edilmelidir.
- **Mumu Gövdesi vs. Fitil (Bodies vs. Wicks):** ICT, fiyat simetrisi ve verimlilik analizinde mumu gövdelerinin (bodies) kapanış/açılış ilişkilerine bakılmasını, fitillerin (wicks) ise sadece likidite taraması anlamında değerlendirilmesini vurgular.
