# ICT 2024 Mentorship \ Lecture #5    August 9, 2024

<https://www.youtube.com/watch?v=ul6x6BwOg6M>

Bu video, Inner Circle Trader (ICT) kanalının **"ICT 2024 Mentorship \ Lecture #5"** (9 Ağustos 2024) başlıklı dersidir.

Video, New York seansını takip edemeyen (örneğin tam zamanlı çalışan) tüccarlar için **Asian Session (Asya Seansı)** odaklı bir işlem modeli ile grafik temizliği, likidite mantığı ve zaman önceliğini ele almaktadır.

## 1. Grafik Disiplini ve Zihinsel Esneklik

- **Temiz Grafik Kullanımı:** Yeni başlayanların grafiğe işaretlemeler yapması normaldir; ancak tecrübe kazandıkça grafiklerin olabildiğince **clean** tutulması gerekir.
- **Çok Fazla İndikatör/Çizim Riski:** Grafikte çok fazla çizgi bulunması tüccarları inatçılaştırır; zararı kesmek (stop/cut loss) yerine çizilen seviyelere körü körüne bağlanmaya yol açar.
- **Esneklik:** ICT, grafikleri sadeleştirmenin piyasaya uyum sağlama esnekliğini artırdığını ve **naked chart** (sade grafik) analizine geçiş için adım adım tecrübe kazanılması gerektiğini vurgulamaktadır.

## 2. Piyasada Zaman Önceliği (Time First)

- **Zamanın Önemi:** Piyasalar sadece belirli bir **Time Window** (zaman penceresi) geldiğinde hareket eder.
- **Algoritmik Yapı:** Zaman ve likidite eşleşmediği sürece fiyat teknik yapılara tepki vermez; zaman unsuru her zaman ilk sırada değerlendirilmelidir.
- **Midnight Opening Range Clarification:** Ders içerisinde Londra/Midnight seansı için açılış aralığının **00:00 - 00:30 (EST)** olduğu netleştirilmiştir.

## 3. Asya Seansı İşlem Modeli (Asian Session / 9-to-5 Traders Model)

New York seansında ekran başında olamayanlar için 18:00 - 21:00 (EST) zaman aralığında uygulanan model adımları:

### A. NDOG (New Day Opening Gap) Tespiti

- **17:00 EST Kapanışı & 18:00 EST Açılışı:**

  - Saat 17:00 kapanışı ile 18:00 açılışı arasındaki fiyat boşluğuna **NDOG (New Day Opening Gap)** denir.
  - 18:00 açılış fiyatı 17:00 kapanışının üzerindeyse **NDOG High**, altındaysa **NDOG Low** seviyesi olarak işaretlenir.
- **Consequent Encroachment (CE):**

  - Eğer NDOG aralığı 20 pip/handle'dan büyükse, boşluğun tam orta noktası (%50 seviyesi) olan **Consequent Encroachment (CE)** işaretlenir.
  - 20 pip'ten küçükse göz kararı takip edilebilir.

### B. İlk Hareket ve Likidite Oluşumu (Initial Range)

- **Hemen İşleme Girilmez:** Gap oluşur oluşmaz doğrudan işlem alınmaz. Fiyatın NDOG etrafında hareket etmesi beklenir.
- **Initial Buyside & Sellside Liquidity:**

  - Fiyatın NDOG seviyesinden uzaklaşıp geri dönerek oluşturduğu kısa vadeli dip ve tepeler işaretlenir (Initial BSL ve Initial SSL).
  - Bu yapılar algoritmanın likidite mühendisliği (engineered liquidity) yaptığı alanlardır.

### C. İşlem Pencereleri ve Kurgu (19:00 - 21:00 EST)

- **Saat 19:00 EST:** Algorithmic programların (Buy/Sell programs) aktif olduğu saat başlangıcıdır.
- **Bullish (Yükseliş) Senaryosu:**

  - Saat 19:00 sonrasında fiyat NDOG seviyesinin üzerine çıkıp gövde kapanışı yaparsa, geri çekilmelerde **ICT Optimal Trade Entry (OTE)** kurgusu aranır.
  - **Target:** Initial BSL veya sol taraftaki daha büyük likidite havuzları.
- **Bearish (Düşüş) Senaryosu:**

  - Fiyat NDOG altında kapanış yaparsa, yukarı yönlü düzeltmelerde short yönlü OTE aranır.
  - **Target:** Initial SSL veya alt taraftaki likidite havuzları.

## 4. Draw on Liquidity (DOL) ve Risk Yönetimi

- **Likidite Mıknatısı:** **NDOG** ve **NWOG** (New Week Opening Gap) seviyeleri fiyat için güçlü birer magnet (çekim alanı) görevi görür. Haber akışı olmasa bile fiyat bu boşluklara çekilme eğilimindedir.
- **Açgözlü Olmamak & Partials:**

  - Büyük "home run" kazançlar yerine disiplinli kâr alımları (**partials**) yapılmalıdır.
  - Kârı kilitlemek psikolojik baskıyı azaltır ve piyasa dalgalanmalarına karşı hesabı korur.
- **Divergence (Uyumsuzluk) Kullanımı:**

  - Tek başına Dow Jones üzerindeki uyumsuzluklar yetersizdir; ancak **NQ (Nasdaq)** ve **ES (S&P 500)** üzerinde eşzamanlı yeni yüksek/düşük yapamama durumu (**SMR / SMT Divergence**) tespit edilirse yön yönelimi doğrulanır.
