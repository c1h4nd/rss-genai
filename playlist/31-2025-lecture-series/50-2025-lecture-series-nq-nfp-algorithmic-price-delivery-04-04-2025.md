# 2025 Lecture Series - NQ NFP Algorithmic Price Delivery  \ 04/04/2025

<https://www.youtube.com/watch?v=JipPODfc5_U>

Bu video, **Inner Circle Trader (ICT)** kanalı tarafından yayınlanan **"2025 Lecture Series - NQ NFP Algorithmic Price Delivery \ 04/04/2025"** başlıklı ders videosudur.

İşte videonun ana başlıklar ve orijinal teknik terimler korunarak hazırlanmış detaylı özeti:

## 1. Genel Bakış ve NFP Gününün Dinamikleri

- **NFP (Non-Farm Payrolls) Duyarlılığı:** NFP haber günlerinde piyasada oluşan yüksek volatilite ve algoritmik fiyatlanma mekanizması incelenmektedir.
- **NQ (Nasdaq Futures):** Analiz ve fiyatlanma hareketleri doğrudan NQ kontratı üzerinde 4 Nisan 2025 tarihli canlı/geçmiş grafik akışı üzerinden gösterilir.
- **Interbank Price Delivery Algorithm (IPDA):** Piyasa hareketlerinin rastgele olmadığını, algoritmik Liquidity (likidite) avı ve Inefficiency (verimsizlik) kapatma prensiplerine dayandığını vurgular.

## 2. Piyasaya Giriş Kuralları & Algoritmik Zamanlama (Time & Price)

- **Time & Price Filtresi:** Algoritmanın belirli zaman dilimlerinde (Kill Zones & Macro zamanları) Liquidity çekim noktalarına yöneldiği anlatılır.
- **Economic Data Release etkisi:** NFP haberinin açıklanmasıyla birlikte oluşan ilk spike (sıçrama) hareketlerinin doğrudan bir yön belirleyici değil, likidite alma (Liquidity Run) amacı taşıdığı gösterilir.
- **1st Presented FVG (Fair Value Gap):** Piyasa açılışı veya haber sonrası oluşan ilk **Fair Value Gap** yapısının yön tayini ve işlem kurgusunda nasıl ele alınması gerektiği aktarılır.

## 3. Fiyat Yapısı ve PD Arrays Analizi

- **Liquidity Pool / External Range Liquidity:** Fiyatın yöneldiği ana hedefler (Buyside Liquidity - BSL veya Sellside Liquidity - SSL) belirlenir.
- **Internal Range Liquidity (IRL):** Fiyatın External Liquidity aldıktan sonra retrace ettiği FVG, Order Block veya Volume Imbalance alanları.
- **Displacement:** Piyasanın kararlı bir şekilde bir yöne kırılım göstermesi ve arkasında FVG bırakması algoritmik onay için şart koşulur.
- **Market Structure Shift (MSS):** Düşük zaman dilimlerinde (1-min / 3-min / 5-min) gerçekleşen yapısal değişim ile yönün teyit edilmesi.

## 4. İşlem Kurgusu ve Risk Yönetimi (Trade Setup)

- **Entry (Giriş) Tespiti:**

  - Premium / Discount bölgesinde oluşan FVG veya Rejection Block seviyelerine retrace beklenir.
  - *Turtle Soup* veya Fakeout hareketleri sonrasında oluşan *FVG Entry* modelleri detaylandırılır.
- **Stop Loss Placement:** Risk seviyesinin invalidation seviyesinin (Swing High/Low veya Swing Order Block) hemen arkasına yerleştirilmesi.
- **Draw on Liquidity (DOL):** Fiyatın ulaşması beklenen en yüksek olasılıklı hedef seviyesi belirlenerek kâr alma (Take Profit / Partial TP) noktaları planlanır.

## 5. Önemli Dersler ve Algoritmik İpuçları

- **Haber Günlerinde Sabır:** NFP gibi yüksek etkili haberlerde ilk dakikalarda işlem yapmaktan kaçınarak algoritmanın likiditeyi temizlemesini ve net bir FVG/Displacement bırakmasını beklemek gerekir.
- **Tape Reading:** Candle bodies (mum gövdeleri) fiyatlanmanın ağırlıklı olduğu yeri gösterirken, wicks (mum fitilleri) sadece likidite taraması (Liquidity Probe) amacına hizmet eder.
- **Journaling & Review:** Bu tür NFP günlerinin işlem günlüğüne eklenerek zaman-fiyat korelasyonlarının düzenli incelenmesi önerilir.
