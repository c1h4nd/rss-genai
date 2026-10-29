# Part 1 \ High Precision Secrets To Intraday Price Action

<https://www.youtube.com/watch?v=DRTvbkKmuAw>

Paylaştığınız YouTube linki, **The Inner Circle Trader (ICT)** kanalına ait **"Part 1 | High Precision Secrets To Intraday Price Action"** isimli derse aittir.

Aşağıda videoda anlatılan temel konseptlerin ve metodolojinin detaylı maddeler halindeki özeti yer almaktadır:

## 📌 Genel Genel Bakış & Giriş

- Video, ICT'nin gün içi (intraday) fiyat hareketlerini yüksek hassasiyetle okumak için geliştirdiği **mekanik zaman/fiyat matrisi (time & price framework)** üzerine kuruludur.
- ICT, indikatörlere veya gecikmeli verilere güvenmek yerine, belirli **zaman pencereleri (time windows)** ve **fiyat aralıkları (ranges)** üzerinden piyasa algoritmalarını okuma yöntemini aktarır.

## ⏰ Pre-Session Window (7:00 AM – 9:00 AM EST)

- **Zamanın Önemi (Fix the Clock First):** Tüm grafik ayarlarının mutlaka **Eastern Time (EST / New York saati)** olarak ayarlanması gerekir.
- **Kritik Zaman Dilimi:** 9:30 AM EST (Regular Trading Hours - RTH) açılışından önceki **07:00 AM – 09:00 AM EST** arası tam 2 saatlik mum/fiyat hareketi esas alınır.
- **Aralığın Belirlenmesi:**

  - 09:00 AM EST olduktan sonra, bu 2 saatlik zaman dilimi içinde kalan **en yüksek seviye (High)** ve **en düşük seviye (Low)** işaretlenir.
  - Bu iki seviye arasındaki aralık, günün geri kalanı için referans matrisini oluşturur.

## 📐 Price Range Bölünmesi & Matris Yapısı

07:00–09:00 AM aralığı belirlendikten sonra bu aralık matematiksel alt bölümlere ayrılır (Quadrant & Octant çizgileri):

- **50% Midpoint (Equilibrium / Consequent Encroachment):** Range'in tam orta noktası belirlenir.
- **Quadrant Lines (Çeyrek Bölümler):** Range %25, %50 ve %75 seviyelerine bölünür.
- **Octant Subdivisions (Sekizde Bir Bölümler):** Daha mikro seviyedeki tepkileri ölçmek için aralık 8 eşit parçaya kadar bölünebilir.
- **Premium & Discount Konsepti:**

  - Midpoint üzerindeki bölge **Premium** (satış aranacak alan),
  - Midpoint altındaki bölge **Discount** (alış aranacak alan) olarak değerlendirilir.

## 🎯 Seviyelerin Projeksiyonu ve Gelecek Fiyat Hareketleri

- **Price Projection (Projeksiyon):** Bu 7:00–9:00 AM range'i ve alt seviyeleri (quadrant'lar), saat 09:30 AM açılışı sonrasındaki RTH seansına doğru sağa aktarılır (carry forward).
- **Algoritmik Tepkiler:** Fiyat 09:30 AM sonrasında hareket ettiğinde, rastgele noktalardan dönmez; daha önceden çizilmiş olan bu quadrant/octant seviyelerine, **FVG (Fair Value Gap)**'lere veya **Liquidity** alanlarına temas eder.
- **Price Arrays ile Birleştirme:** Bu seviyeler tek başına değil, Daily Chart projeksiyonları, likidite referansları ve imbalance'lar (FVG, Volume Imbalance) ile çakıştığı yerlerde (confluence) işleme giriş için kullanılır.

## 💡 Candle Body vs. Wick (Mum Gövdesi ve İğne Ayrımı)

- **İğneler (Wicks):** Fiyatın likidite temizliği (liquidity run / sweep) yapmak veya seviyeleri test etmek amacıyla delip geçtiği alanlardır.
- **Gövdeler (Candle Bodies):** Fiyatın esas kabul gördüğü alanı gösterir (narrative & volume).
- Eğer mum iğnesi quadrant/midpoint çizgisini geçiyor ancak **mum gövdesi (body) çizginin üzerinde/altında kapanıyorsa**, o seviye algoritmik olarak saygı görmüş demektir.

## 📋 İşlem Modeli / Workflow Checklist

1. **Clock Setup:** Grafiği New York (EST) saatine sabitle.
2. **Wait for 09:00 AM:** Saat 09:00 AM EST olana kadar 07:00–09:00 AM aralığına müdahale etme.
3. **Mark High & Low:** Saat 09:00 AM'de bu 2 saatlik pencerenin en yüksek ve en düşük seviyesini çiz.
4. **Subdivide:** %50 (Midpoint), %25 ve %75 (Quadrant) çizgilerini yerleştir.
5. **Formulate Narrative:** Daily chart yönünü ve mevcut FVG / Liquidity hedeflerini belirle.
6. **Execution Window:** 09:30 AM EST sonrasında fiyatın Premium/Discount bölgelerindeki bu seviyelere vereceği tepkileri ve FVG dolumlarını izleyerek işleme dahil ol.

*Videodaki belirli bir timestamp veya konsept (örneğin FVG, Consequent Encroachment ya da Liquidity detayları) hakkında daha derinlemesine bilgi isterseniz sorabilirsiniz!*
