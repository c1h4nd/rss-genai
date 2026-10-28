# 2023 ICT Mentorship - Opening Range Gap Repricing Macro

<https://www.youtube.com/watch?v=Sf_uYZBWTrA>

Bu video, Michael J. Huddleston (The Inner Circle Trader - ICT) tarafından hazırlanan **2023 ICT Mentorship** serisine ait **"Opening Range Gap Repricing Macro"** (Açılış Aralığı Boşluğunun Makro ile Yeniden Fiyatlanması) konulu derstir.

İşte videoda aktarılan konseptlerin, kuralların ve stratejinin maddeler halinde detaylı özeti:

### 1. Temel Tanımlar & Konseptler

- **Opening Range Gap (ORG):** Piyasaların (özellikle Index Futures / NQ & ES) New York seansı açılışı olan **09:30 EST** ile birlikte oluşturduğu fiyat aralığı veya gap yapısıdır.
- **Time Macros (Zaman Makroları):** Algoritmanın belirli zaman aralıklarında (örneğin 09:50 - 10:10 EST veya 10:50 - 11:10 EST gibi kısa pencerelerde) **Liquidity** toplamak veya **Inefficiency / Fair Value Gap (FVG)** bölgelerini yeniden fiyatlamak (repricing) üzere kurgulanmış algoritmik komut dizileridir.
- **Repricing (Yeniden Fiyatlama):** Fiyatın daha önce geride bıraktığı eksik/dengesiz alanlara (**Fair Value Gap**, **Opening Range Gap**) geri dönerek bu seviyeleri "doldurması" ve dengelemesi sürecidir.

### 2. Opening Range Gap (ORG) Türleri ve Mantığı

- **Discount Opening Range Gap:** Açılış gap'inin önceki seansın kapanışına göre daha aşağıda oluşması halidir. Algoritma için bir alım (**Discount**) fırsatı ve repricing alanı oluşturur.
- **Premium Opening Range Gap:** Fiyatın önceki seansa göre daha yukarıda gap açması durumudur. Algoritma burayı satım (**Premium**) yönlü repricing için hedefleyebilir.
- **Fibonacci Tool Kullanımı:** ORG alanının üst ve alt sınırlarına Fibonacci çizilerek **%50 (Consequent Encroachment / Equilibrium)** seviyesi belirlenir. Fiyatın bu %50 seviyesine göstereceği reaksiyon algoritmanın yönü hakkında kritik ipucu verir.

### 3. Macro ve ORG Entegrasyonu (Strateji ve İşleyiş)

- **Zaman Pencerelerinin Önemi:** Algoritma gün boyu rastgele hareket etmez. Açılış sonrasındaki makro pencerelerinde (**Macro Window**) önceden oluşmuş ORG seviyelerine retest / repricing yapar.
- **Support & Resistance Görevi:** Doldurulan veya repricing edilen ORG, trend yönünde bir **Support (Destek)** veya **Resistance (Direnç)** bloğuna dönüşür.
- **1st Presented FVG ile Eşleşme:** Açılışın (09:30) hemen ardından 1 dakikalık grafiklerde oluşan **First Presented Fair Value Gap** ile ORG seviyeleri çakışıyorsa, bu bölge yüksek olasılıklı bir **Institutional Order Flow** giriş alanı haline gelir.

### 4. Trade Kuralları ve Execution Adımları

- **Higher Timeframe Bias:** Makro içi işlemlere girmeden önce günlük/saatlik grafikteki **Draw on Liquidity** ve ana yön (**Bias**) netleştirilmelidir.
- **1-Minute Chart Precision:**

  1. 09:30 açılışından sonra **Opening Range** ve gap bölgesi işaretlenir.
  2. İlgili **Macro Window** zamanı geldiğinde fiyatın ORG veya FVG bölgesine çekilmesi (**Retracement**) beklenir.
  3. Fiyat bu alana girdiğinde **Market Structure Shift (MSS)** ve hacimli bir **Displacement** mumu ile teyit aranır.
- **Stop-Loss ve Take-Profit Mantığı:**

  - **Stop-Loss (SL):** Yapıyı oluşturan ilgili Swing High/Low seviyesinin veya FVG'nin hemen arkasına konur.
  - **Take-Profit (TP):** Karşı taraftaki Likidite havuzları (**Buyside Liquidity / Sellside Liquidity**) veya tamamlanmamış **PD Array** alanları hedef olarak belirlenir.

### 5. Önemli Ders Notları & ICT Tavsiyeleri

- **Patience over Bias:** Makro saati gelmeden ve fiyat tam olarak ilgilendiğiniz **PD Array / ORG** bölgesine repricing yapmadan aceleyle işleme girilmemelidir.
- **Timeframe Shopping Yapmayın:** Hangi timeframe üzerinde gap veya FVG analiz ediliyorsa (ör. 1M / 5M) tutarlı bir şekilde o zaman diliminde kalınmalıdır; grafikler arasında sürekli timeframe değiştirerek zorlama gap aranmamalıdır.
- **Risk Management:** Makro pencerelerinde algoritmanın hareketleri hızlı ve sert olabileceğinden **Stop-Loss** disiplinine ve sabit risk oranlarına sadık kalınmalıdır.
