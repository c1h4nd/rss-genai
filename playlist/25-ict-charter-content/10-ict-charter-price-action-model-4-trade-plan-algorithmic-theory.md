# ICT Charter Price Action Model 4 \ Trade Plan & Algorithmic Theory

<https://www.youtube.com/watch?v=H05w52zQGdQ>

Bu videoda (**ICT Charter Price Action Model 4 - Position Trading Trade Plan & Algorithmic Theory**) ICT'nin sunduğu temel ve detaylı başlıklar şunlardır:

### 1. Genel Bakış ve Modelin Amacı

- **Trade Hedefi:** Trade başına minimum **500+ Pip** kazanmayı hedefleyen bir **Position Trading** modelidir.
- **Zaman Dilimleri & Perspektif:** Temel analiz ve yön tayini için **Monthly** ve **Weekly** grafiklere odaklanılır. Yaklaşık 2 ay veya daha uzun süren **Quarterly Shifts** (çeyreklik yön değişimleri) esas alınır.
- **5 Aşamalı Süreç:** Diğer tüm ICT trade planlarında olduğu gibi süreç şu aşamalardan oluşur:

  1. **Preparation** (Hazırlık)
  2. **Opportunity Discovery** (Fırsat Keşfi)
  3. **Trade Planning** (Planlama)
  4. **Trade Execution** (Giriş / İşleme Alma)
  5. **Trade Management** (Yönetim)

### 2. Trade Preparation (Hazırlık Aşaması)

- **Economic Calendar:** Gelecek haftanın orta (**medium**) ve yüksek (**high impact**) etkili haber akışları takip edilir. Günlük haber bültenlerinin yarattığı volatilite enjeksiyonları, büyük oyuncuların ana manipülasyon hareketlerini gizlemek için kullandığı bir "smoke screen" (sis perdesi) görevi görür.
- **IPDA Data Range:** Mevcut gün dahil edilerek geriye dönük **20, 40 ve 60 işlem günü** (Pazarlar hariç) hesaplanır:

  - Bu aralıklardaki en yüksek tepe (**Highest High**) ve en düşük dip (**Lowest Low**) belirlenerek **Current Dealing Range** oluşturulur.
  - Position trading için 500 pip hedefine ulaşmak adına sıklıkla **60 günlük IPDA Data Range** referans alınır.
- **Seasonal Tendencies (Mevsimsellik Trendleri):**

  - Yıllık bazda en güçlü mevsimsel eğilimlere sahip pariteler/emtialar seçilir (ör. Nisan ayında EUR/USD'nin tepe yapıp Mayıs'a doğru düşme eğilimi).
  - Yıl başında (Ocak ayı başı/Noel arası) tüm yılın mevsimsel haritası planlanır. Mevsimsellik kesin bir kural değil, olasılığı yüksek bir **road map**'tir.
- **COT (Commitment of Traders) & Hedge Program:** Commercial trader'ların 6 aylık trendi ve pozisyonlanması incelenir.

  - COT ve mevsimsellik **bullish** ise: IPDA aralığı içindeki **Discount PD Arrays** (alım için) ve aralığın üzerindeki **Premium PD Arrays** (hedef için) belirlenir.
  - COT ve mevsimsellik **bearish** ise: IPDA aralığı içindeki **Premium PD Arrays** (satış için) ve aralığın altındaki **Discount PD Arrays** (hedef için) belirlenir.

### 3. Opportunity Discovery & Trade Planning (Fırsat Keşfi ve Planlama)

- **PD Array & Matrix Matçleşmesi:**

  - **Bearish Senaryo:** Fiyatın 4 saatlik (**4-Hour**) **Premium Fair Value Gap (FVG)** içine çekilmesi ve **Standard Deviation** olarak maks `+3` sapma ile çakışması (convergence) beklenir.
  - **Bullish Senaryo:** Fiyatın 4 saatlik (**4-Hour**) **Discount Fair Value Gap (FVG)** içine çekilmesi ve maks `-3` sapma ile çakışması beklenir.
- **Weekly Profile & Timing:**

  - Haftalık yönü belirlerken haftanın dip/tepe noktasının **Pazartesi - Çarşamba** (New York açılışına kadar) oluşması beklenir.
  - İstatistiksel olarak **Salı günü**, haftanın dip (bullish ise) veya tepe (bearish ise) noktasını oluşturma konusunda %70 gibi yüksek bir olasılığa sahiptir.
  - Avrupa seansı açılış fiyatı (**European Opening Price**) filtre olarak kullanılır. Örnek: Bullish beklentide Avrupa açılış fiyatının altındaki ve 4H Discount FVG ile örtüşen seviyeler en ideal alım alanıdır.
- **Alt Zaman Dilimi Entegrasyonu:** Risk azaltmak isteyenler **Scalping** veya 15 dakikalık (**15-min**) Institutional Order Flow Entry Drill (IOFED) kurallarını bu aşamaya entegre edebilir.

### 4. Trade Execution (İşleme Giriş Kriterleri)

- **Limit Order Kullanımı:**

  - **Bearish / Short:** `Standard Deviation & PD Array Convergence - 5 Pips` seviyesine **Sell Limit** konulur.
  - **Bullish / Long:** `Standard Deviation & PD Array Convergence + 5 Pips` seviyesine **Buy Limit** konulur.
- **Stop Loss Tanımlama:**

  - **Short:** Giriş yapılan yapının Tepesi + **25 Pip** zararı durdur seviyesi olarak belirlenir.
  - **Long:** Giriş yapılan yapının Dibi - **25 Pip** zararı durdur seviyesi olarak belirlenir.
  - Position trading'de ilk denemede stop olunsa bile yapı geçerliyse ikincil giriş (**secondary entry**) kovalanmalıdır.

### 5. Trade & Risk Management (Pozisyon ve Risk Yönetimi)

- **Kar Al (Take Profit / Partial) Stratejisi:**

  - Pozisyon genellikle birden fazla parçaya (order) bölünerek yönetilir:

    1. **1. Hedef:** 100 Pip ulaşıldığında ilk parça kapatılır.
    2. **2. Hedef:** 250 Pip ulaşıldığında ikinci parça kapatılır.
    3. **3. Hedef (500 Pip):** 500 Pip hedefine ulaşıldığında **toplam pozisyon büyüklüğünün %80'i kapatılmalıdır**. Kalan %20 trendin devamı ihtimaline karşılık açık bırakılabilir.
- **Trailing Stop / Risk Kaydırma:**

  - Beklenen hedefin **%25**'i kar bölgesine girilince: Stop Loss %25 daraltılır.
  - Beklenen hedefin **%50**'si kar bölgesine girilince: Stop Loss %50 daraltılır.
  - Beklenen hedefin **%75**'ine ulaşıldığında: Stop Loss **Break Even** (Giriş seviyesi) yapılır.
- **Sermaye Risk Kuralları (R% Scaling):**

  - Position trading için işlem başına tavsiye edilen maksimum risk **%1 - %1.5** aralığıdır (%1 tercih edilir).
  - **Kayıp Durumunda:** Tam bir kayıp (R%) yaşandığında, bir sonraki işlemin riski **%50 azaltılır** (ör. %1'den %0.5'e düşürülür). Kayıp miktarının %50'si geri kazanılana kadar risk artırılmaz.
  - **Seri Galibiyet Durumunda:** Üst üste **5 kazançlı işlemden** sonra risk oranı **%50 azaltılır**. Amaç, kaçınılmaz olan gelecekteki olası bir kayıpta equity curve üzerindeki sert düşüşleri (drawdown) yumuşatmaktır.

### 6. Algorithmic Theory & Örnek Analiz (EUR/USD)

- **Örnek Senaryo:** 2022 Nisan EUR/USD paritesi.
- **SMT Divergence & Market Structure:**

  - Dolar Endeksi (DXY) yükselirken Euro'da düşüş beklenir.
  - EUR/USD eski tepeyi temizleyip yukarı gittiğinde, eşleşen kardeş parite (ör. GBP/USD) daha düşük bir tepe yaparak **Bearish SMT Divergence** oluşturur.
- **Entry Execution & Targeting:**

  - Eski tepeyi kıran mumun açılış fiyatına (**Order Block / Opening Price**) **Sell Stop** emri koyularak zayıflık satılır.
  - **Targeting:** Likidite havuzları, eski aylık/haftalık dipler ve **Offset Distribution** mantığı kullanılır.
  - **Offset Distribution:** Fiyat eski bir dip seviyesini kırdıktan sonra küçük bir duraksama/düzeltme yapar. Bu süreçte yeni sell stop'lar birikir. Fiyat bu yeni stop'ları da temizlemek adına likiditeye doğru bir kez daha aşağı sarkar (ör. 1.0400 psikolojik seviyesine doğru).
- **Risk/Ödül Oranı:** Yaklaşık 135 pip risk ile 950+ pip hedefleme yapılarak tek bir işlemde **1:7 Risk/Reward (R:R)** seviyesine ulaşma örneği sunulur.

### 7. Sezonluk İşlem Tavsiyeleri

- **En Verimli İki Sezon:** Yıl içerisinde **Spring (İlkbahar)** ve **Fall (Sonbahar)** dönemleri algoritmik hareketlerin ve mevsimsel trendlerin en temiz çalıştığı dönemlerdir.
- **Doldrums (Sakınma Dönemleri):** **Ocak başı**, **Temmuz-Ağustos (Yaz durgunluğu)** ve **Aralık sonu** gibi düşük volatilite veya tatil dönemlerinde işlem yapmaktan kaçınılması/işlem hacminin düşürülmesi önerilir.

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  ICT Charter Price Action Model 4 \ Trade Plan & Algorithmic Theory

  The Inner Circle Trader · 66K views

   [Open in ICT Charter Price Action Model 4 \ Trade Plan & Algorithmic Theory](http://www.youtube.com/watch?v=H05w52zQGdQ)](http://www.youtube.com/watch?v=H05w52zQGdQ)

  ![](https://i.ytimg.com/vi/H05w52zQGdQ/maxresdefault.jpg)
