# NQ High Of Day Short Review

<https://www.youtube.com/watch?v=P8Pn8DHFSW8>

Bu video, **The Inner Circle Trader (ICT)** kanalına ait **"NQ High Of Day Short Review"** başlıklı derstir. NQ (Nasdaq Futures) üzerindeki High of Day (günün en yüksek seviyesi) short işlem kurulumunun teknik ve algoritmik analizini sunar.

### **1. Genel Context ve Hazırlık Phase'i**

- **Timeframe ve Enstrüman:** Analiz **NQ (Nasdaq Futures)** piyasası üzerinde, ağırlıklı olarak **1-minute chart** ve **continuous contract** verileri kullanılarak yapılmıştır.
- **Pre-Market Rules (07:00 – 09:00 AM ET):**

  - İşlem öncesinde pre-market seansında oluşan konsolidasyon alanları, yüksek/düşük seviyeler ve likidite havuzları haritalandırılır.
  - Piyasanın açılış öncesi gösterdiği yapının (consolidation / expansion) gün içindeki **bias** (yön beklentisi) için belirleyici olduğu vurgulanır.

### **2. Trade Setup ve Entry Mechanics**

- **Liquidity Sweep & High of Day:**

  - Fiyat, günün zirvesini (**High of Day**) yaparken var olan likiditeyi (Buy-side Liquidity) temizler.
  - Bu hareket, algoritmik olarak bir **Premium** bölgeye erişim ve short yönlü likidite alımı anlamına gelir.
- **Imbalance ve Fair Value Gap (FVG):**

  - Günün zirvesi yapıldıktan sonra sert bir düşüşle **Fair Value Gap (FVG)** ve **Volume Balance** alanları oluşur.
  - Fiyatın bu FVG / Volume Balance bölgesine re-test yapmasıyla birlikte short entry (satış) fırsatı yakalanır.
- **Candle Body vs. Wick Mantığı:**

  - Fiyat dengesizlikleri ve yapı değişimleri analiz edilirken mum gövdeleri (**Candle Bodies**) baz alınır; uzantılar (**Wicks**) sadece likidite iğneleri olarak değerlendirilir.
  - Gövdelerin belirlenen seviyenin altında kapanması (**Close below midpoint/Consequent Encroachment**) düşüş yönlü **Order Flow** teyididir.

### **3. Stop-Loss & Trade Management Rules**

- **Stop Placement:**

  - **Stop-Loss**, ilgili dalganın mum gövdesi zirvesinin veya yapısal **Volume Balance / High** seviyesinin hemen üstüne konumlandırılır.
- **Drawdown ve Disiplin:**

  - İşlem sürecinde yaşanan küçük drawdown'ların normal olduğu, trade modelinin disiplinle takip edilmesi gerektiği ifade edilir.
- **Targeting:**

  - Hedef seviye olarak aşağıdaki **Sell-side Liquidity** alanları, önceden bırakılmış açılış boşlukları (**New Week Opening Gap / Gap Low**) ve indirimli bölgedeki (**Discount**) FVG'ler belirlenir.

### **4. Öne Çıkan Core Concepts & Key Takeaways**

- **PDA (Premium / Discount Array) Grading:**

  - Fiyat aralığının orta noktası (**Midpoint / Equilibrium**) baz alınarak, üst yarısı **Premium** (satış arama alanı), alt yarısı ise **Discount** (alım arama alanı) olarak sınıflandırılır.
- **Order Flow Confirmation:**

  - Mum gövdelerinin alt yarıda yoğunlaşması bearish order flow’u, üst yarıda kalması ise bullish order flow’u gösterir.
- **Process over Outcome:**

  - Doğru çıkma ihtiyacını ortadan kaldırıp (**removing the need to be right**), tamamen sisteme ve algoritmik kurallara bağlı kalınması gerektiği vurgulanır.
