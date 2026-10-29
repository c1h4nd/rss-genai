# 2025 Lecture Series - Algorithmic Price Delivery Continuum

<https://www.youtube.com/watch?v=vgG9JAKwng4>

Inner Circle Trader (ICT) tarafından yayınlanan **"2025 Lecture Series - Algorithmic Price Delivery Continuum"** başlıklı videonun detaylı ve maddeler halinde özeti aşağıdadır.

Orijinal terminoloji ve konsept isimleri (PD Arrays, Low/High Resistance Liquidity Run, Fair Value Gap vb.) İngilizce korunmuştur.

### 📋 Genel Bakış ve Temel Felsefe

- **Algoritmik Piyasa Yapısı:** Fiyat hareketleri rastgele (random walk) değildir; algoritmik bir döngü ve zaman/fiyat ilişkisi (*Time & Price*) çerçevesinde teslim edilir (*Price Delivery*).
- **Continuum (Süreklilik):** Algoritma, piyasa koşullarına bağlı olarak belirli evreler (Consolidation, Expansion, Retracement, Reversal) arasında sürekli bir geçiş halindedir.

### ⚙️ Algorithmic Price Delivery Cycle (4 Temel Evre)

Piyasadaki fiyat hareketi şu 4 aşamalı sürekli döngüyü takip eder:

1. **Consolidation (Konsolidasyon):**

   - Algoritmanın likidite ve sipariş biriktirdiği (*Order Accumulation/Distribution*) dar bant aralığı.
   - Liquidity'nin oluşturulduğu ana bölgedir (Buy-side & Sell-side Liquidity).
2. **Expansion (Genişleme / Re-pricing):**

   - Fiyatın konsolidasyondan hızlı bir şekilde çıkarak bir sonraki **PD Array**'e doğru yönelmesi.
   - Bu evrede genellikle **Fair Value Gap (FVG)** oluşur.
3. **Retracement (Geri Çekilme):**

   - Fiyatın yeni oluşturduğu aralık (*Recently Created Fair Value Gap / Imbalance*) içine tekrar geri süzülerek likiditeyi dengelemesi.
4. **Reversal (Tersine Dönüş):**

   - Fiyatın key HTF (Higher Time Frame) PD Array'e ulaştıktan sonra yön değiştirerek karşıt likidite hedefine (*Liquidity Pool*) yönelmesi.

### 📊 Low Resistance Liquidity Run (LRLR) vs. High Resistance Liquidity Run (HRLR)

#### **1. Low Resistance Liquidity Run (LRLR)**

- **Tanım:** Fiyatın hedefe doğru zahmetsizce, hızlı ve güçlü mumlarla ilerlediği ideal işlem koşullarıdır.
- **Belirtileri:**

  - Grafiklerde belirgin **Fair Value Gap (FVG)**'ler oluşur (Örn: 15-dk veya 5-dk grafiklerde her çeyrekte FVG birikimi).
  - **Breakaway Gap:** Kırılım seviyelerinde oluşan boşluklar açık kalır (*Unfilled*) ve fiyat hemen geri dönüp doldurmaz.
  - Yol boyunca karşıt PD Array'ler neredeyse hiç direnç göstermez.

#### **2. High Resistance Liquidity Run (HRLR)**

- **Tanım:** Fiyatın çok fazla testere (chop/noise) yaptığı, sık sık geri çekildiği ve hedefe ulaşmakta zorlandığı koşullardır.
- **Belirtileri:**

  - 15-dk veya 5-dk grafiklerde **FVG oluşmaz** ya da oluşan boşluklar hemen tam olarak kapatılır.
  - Fiyat, eski seviyeleri tekrar tekrar ziyaret eder.
- **Kural:** HRLR koşullarında işlem açmak risklidir; ICT bu aşamalarda işlem yapmayıp kenarda beklenmesini (*Sit Still*) tavsiye eder.

### 🕒 Time & Price Grids (Zaman Boyutu ve Makrolar)

- **Algorithmic Time Windows:** Fiyat hareketinin en agresif ve tahmin edilebilir olduğu zaman dilimleri dikkate alınmalıdır (Örn: NY Open, NY Lunch Macro, PM Session).
- **Quarterly Theory / Hourly Splits:** Saatlik mumların 15'er dakikalık 4 çeyreğe (Quarters) bölünerek incelenmesi; her çeyrekte algoritmik bir FVG veya Displacement aranması.

### 🎯 Trade Execution & Risk Yönetimi Prensipleri

- **PD Array Matrix Alignment:** İşlem girerken mutlaka HTF (Higher Time Frame) Trend/Bias ile LTF (Lower Time Frame) PD Array'lerinin uyum içinde olması gerekir.
- **Fresh vs. Exhausted PD Arrays:** Daha önce test edilmemiş (*Fresh*) PD Array'ler en yüksek tepki potansiyeline sahiptir; defalarca test edilmiş (*Exhausted*) seviyeler likidite kaynağı olmaktan çıkar.
- **Psikoloji & Disiplin:** HRLR günlerinde zorlama işlemler yapıp sermayeyi eritmek yerine, algoritmik akışın netleştiği (FVG'lerin temiz bırakıldığı LRLR) anları beklemek ana anahtardır.

Teknik terimler veya konseptlerden detaylandırmamı istediğiniz özel bir bölüm olursa sorabilirsiniz!
