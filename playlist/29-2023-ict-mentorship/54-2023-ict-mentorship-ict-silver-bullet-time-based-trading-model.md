# 2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model

<https://www.youtube.com/watch?v=tRq1hyGGtl4>

**"2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model"** başlıklı (The Inner Circle Trader - ICT kanalı) videonun detaylı Türkçe/İngilizce karma özeti:

## 🎯 Genel Bakış ve Konsept (Overview)

- **Silver Bullet Model:** ICT’nin zaman bazlı (Time-Based Trading) geliştirdiği, gün içinde belirli dar saat aralıklarında ortaya çıkan yüksek ihtimalli (high probability) işlem kurulumlarını hedefleyen mekanik bir modeldir.
- **Algoritmik Zaman Pencereleri (Time Windows):** Algoritma piyasayı belirli zaman aralıklarında **Liquidity (likidite)** çekmeye veya **Fair Value Gap (FVG)** doldurmaya zorlar.

## ⏰ Silver Bullet Execution Hours (İşlem Saatleri)

Model sadece **New York Local Time (EST/EDT)** zaman dilimine göre belirli 1 saatlik pencerelerde uygulanır:

1. **London Open Window:** `03:00 AM – 04:00 AM NY Time`
2. **New York AM Session Window:** `10:00 AM – 11:00 AM NY Time` (En popüler pencere)
3. **New York PM Session Window:** `02:00 PM – 03:00 PM NY Time`

> **Önemli Kural:** İşleme girmek için setup'ın (tetikleyici ve FVG oluşumu) bu 1 saatlik pencere içerisinde gerçekleşmesi gerekir.

## 🛠️ Temel Bileşenler ve Koşullar (Core Components)

1. **Liquidity Sweep (Likidite Temizliği):**

   - Fiyatın önce yakın dönemdeki bir **Liquidity Pool**'u (Sell-side Liquidity veya Buy-side Liquidity) temizlemesi beklenir.
   - Örnekler: *Previous Day High/Low (PDH/PDL), Previous Session High/Low, Equal Highs/Lows (EQH/EQL)*.
2. **Displacement & Market Structure Shift (MSS):**

   - Likidite alındıktan sonra güçlü, hacimli bir mum hareketi (**Displacement**) ile yapının kırılması (**MSS**) gerekir.
3. **Fair Value Gap (FVG):**

   - Displacement sırasında 3 mumluk yapıda oluşan imbalans / dengesizlik alanı (**Fair Value Gap**).
   - Giriş seviyesi olarak bu FVG kullanılır.

## 📐 İşlem Adımları ve Kurallar (Step-by-Step Setup)

- **Step 1:** Belirlenen **Silver Bullet** saat dilimi başladığında grafiği açın (1-min / 3-min / 5-min chart).
- **Step 2:** Fiyatın hedeflenen bir **Liquidity Level**'ı süpürmesini bekleyin.
- **Step 3:** Süpürme sonrası ters yönde sert bir **Displacement** ve **MSS** arayın.
- **Step 4:** Oluşan **FVG** içerisine **Limit Order** koyun (veya re-test anında **Market Entry**).
- **Stop Loss (SL):** **MSS**'i oluşturan Swing High / Swing Low seviyesinin hemen arkasına konur.
- **Take Profit (TP) / Target:**

  - En az **1:2 Risk-to-Reward (R:R)** hedefi.
  - Karşı taraftaki en yakın likidite havuzu (Unmet Liquidity) veya karşı FVG / Liquidity Void.

## 💡 Önemli İpuçları (Key Takeaways)

- **Daily Bias Şart Değil (No Daily Bias Required):** Silver Bullet modeli intraday scalping odaklı olduğu için, uzun vadeli Daily Bias tam net olmasa bile zaman pencereleri içindeki likidite hareketleriyle işlem kurulabilir.
- **Time is First, Price is Second:** Önce zaman penceresi (`Time Window`), sonra fiyat yapısı (`Price Action`) dikkate alınır.
- **One & Done:** Eğer ilgili 1 saatlik pencerede 1 başarılı işlem (veya hedef R/R) yakalandıysa, o oturum için trading kapatılmalıdır.
