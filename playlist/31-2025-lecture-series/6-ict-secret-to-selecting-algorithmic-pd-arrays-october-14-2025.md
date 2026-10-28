# ICT Secret To Selecting Algorithmic PD Arrays \ October 14, 2025

<https://www.youtube.com/watch?v=p9w1Nc6FK0c>

**"ICT Secret To Selecting Algorithmic PD Arrays"** başlıklı (14 Ekim 2025 tarihli) video için ana başlıklar ve detaylı maddeler halinde hazırlanmış Türkçe/İngilizce karma özet:

## 1. Core Framework & Algorithmic Delivery (Temel Algoritmik Mantık)

- **IPDA (Interbank Price Delivery Algorithm):** Fiyat hareketleri rastgele değildir; algoritma likidite çekim noktalarına (**Liquidity Pools**) ve fiyat dengesizliklerine (**Imbalances**) göre fiyatı teslim eder.
- **PD Array Hierarchy (Hiyerarşi):** Algoritmanın reaksiyon vereceği **PD Array** seçilirken üst zaman dilimindeki (**HTF - Higher Time Frame**) yapı her zaman alt zaman dilimini (**LTF - Lower Time Frame**) domine eder.
- **Premium vs. Discount Framework:**

  - Fiyat, **True Open** seviyesinin veya mevcut fiyat aralığının (**Dealing Range**) üst yarısındaysa (**Premium**), satış yönlü PD Array’ler (**Bearish PD Arrays**) önceliklendirilir.
  - Fiyat alt yarısındaysa (**Discount**), alış yönlü PD Array’ler (**Bullish PD Arrays**) seçilir.

## 2. Selection Criteria for Valid PD Arrays (Doğru PD Array Seçim Kriterleri)

- **Displacement (Şiddetli Fiyat Hareketi):**

  - Bir PD Array'in (örneğin Order Block veya Fair Value Gap) geçerli olması için ardında güçlü bir **Displacement** bırakması gerekir.
  - Yavaş ve zayıf fiyat hareketleriyle oluşan yapıların algoritmik desteği düşüktür.
- **Liquidity Sweep / Stop Run Prioritization:**

  - En yüksek olasılıklı (**High-Probability**) PD Array'ler, öncesinde bir **Buyside Liquidity (BSL)** veya **Sellside Liquidity (SSL)** alımından sonra oluşan yapılardır.
  - Bir likidite temizliği (Stop Run) yaşanmadan oluşan boşluklar veya bloklar genellikle algoritmik olarak ihlal edilebilir (vuruş ihtimali düşüktür).

## 3. Order Blocks & Fair Value Gaps (FVG) İlişkisi

- **FVG & Displacement Şartı:** Bir **Order Block (OB)** seçilirken, mum hareketinden hemen sonra net bir **Fair Value Gap (FVG)** oluşmuş olması şarttır. FVG içermeyen mum grupları güçlü bir algoritmik Order Block kabul edilmez.
- **Confluence (Çakışma / Birleşim):**

  - **Order Block + FVG + Liquidity Sweep** bileşimi, algoritmik tepki potansiyeli en yüksek olan yapıdır.
- **Open Gaps as Strength Indicators:**

  - Güçlü trendlerde bazı FVG’lerin tamamen dolmaması (left open) piyasadaki kurumsal gücün (institutional delivery) ne kadar baskın olduğunu gösterir.

## 4. Wicks, Bodies & Consequent Encroachment (Mum İğneleri ve Gövdeler)

- **Body vs. Wick:**

  - **Candle Bodies (Mum Gövdeleri):** Hacmi ve gerçek fiyat akışını temsil eder. Fiyat gövdesi belirli bir PD Array seviyesinin ötesinde kapanış yaparsa yapı bozulmuş (**Failure**) sayılır.
  - **Wicks (İğneler):** Likidite alımını temsil eder. Fiyatın iğne atıp geri dönmesi yapının çalıştığını gösterir.
- **Consequent Encroachment (CE):**

  - FVG veya Wick aralıklarının tam orta noktasıdır (%50 seviyesi). Algoritma fiyatı dengelerken çoğunlukla bu seviyeye kadar temas arar.

## 5. Algorithmic PD Array Matrix (Matrix Mantığıyla Eleme)

- **Top-Down Analysis:** HTF üzerindeki ana hedef/bias belirlenmeden LTF üzerindeki PD Array'ler tek başına kullanılmamalıdır.
- **Nested PD Arrays:** HTF PD Array'i içerisindeki LTF PD Array'leri (**PD Array inside a PD Array**) işlem hassasiyetini ve **Risk/Reward (R:R)** oranını artırmak için kullanılır.

Anlamadığınız veya derinleştirmemi istediğiniz spesifik bir kavram (örneğin *Displacement*, *Consequent Encroachment* veya *Liquidity Sweep*) olursa detaylandırabilirim!
