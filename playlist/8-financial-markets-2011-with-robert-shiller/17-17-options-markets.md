# 17. Options Markets

<https://www.youtube.com/watch?v=VkUEWUxI6u0>

Yale Üniversitesi’nin **"17. Options Markets" (Opsiyon Piyasaları)** dersinden öne çıkan temel ve detaylı başlıklar şunlardır:

### 1. Opsiyon Kavramı ve Temel Türler

- **Call Option (Alım Opsiyonu):** Belirli bir **Exercise Price / Strike Price** (kullanım / kullanım fiyatı) üzerinden bir varlığı belirli bir tarihe kadar (**Exercise Date**) satın alma hakkı verir [[01:07](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=67)].
- **Put Option (Satım Opsiyonu):** Belirli bir strike price üzerinden bir varlığı satma hakkı verir [[01:26](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=86)].
- **Amerikan vs. Avrupa Opsiyonları (American vs. European Options):**

  - **American Option:** Kullanım tarihine (*exercise date*) kadar herhangi bir anda kullanılabilir [[03:32](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=212)].
  - **European Option:** Sadece son kullanım tarihinde (*exercise date*) kullanılabilir [[03:43](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=223)].
  - Esneklik nedeniyle Amerikan opsiyonu alıcı için teorik olarak daha değerlidir veya en az Avrupa opsiyonuna eşittir [[03:51](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=231)].
- **Option Value (Opsiyon Değeri):** Opsiyon erken kullanıldığında (exercise edildiğinde) seçme özgürlüğü ve esneklik kaybedildiği için opsiyon değeri yok olur; bu nedenle call opsiyonlar genelde vadeden önce erken exercise edilmez [[04:51](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=291)].

### 2. Opsiyonların Ekonomik ve Davranışsal Rolü

- **Fiyat Keşfi ve Risk Yönetimi (Price Discovery):**

  - Opsiyonlar piyasayı tamamlar (**Completing the State Space** - Kenneth Arrow & Stephen Ross) [[09:46](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=586)]. Piyasada gelecekteki olası durumların fiyatlanmasını sağlayarak ekonomik verimlilik sunar [[10:39](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=639)].
  - Opsiyonlar sadece bir "kumar aracı" değil, bilgi sağlayan ve yatırım kararlarını yönlendiren finansal enstrümanlardır [[08:08](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=488)].
- **Davranışsal Finans Açısı (Behavioral Purpose):**

  - **Incentive Stock Options:** Şirket çalışanlarına hisse opsiyonu verilmesi, onların dikkatini (**attention & salience**) şirketin hisse değerine ve başarısına odaklamalarını sağlar [[14:32](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=872)].
  - **Insurance (Sigorta) & Peace of Mind:** Ev sigortası aslında ev üzerine alınmış bir **Put Option** gibidir; felaket durumunda yatırımcıya huzur (*peace of mind*) sağlar [[15:35](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=935)].

### 3. Piyasalar, Aktörler ve Türev Ürünler

- **Alıcı ve Yazıcı (Buyer vs. Writer):** Opsiyonu alan taraf kullanım hakkına sahiptir; opsiyonu yazan taraf (**Writer**) ise taahhüdü karşılamakla yükümlüdür [[21:48](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1308)]. Elinde dayanak varlık olmadan opsiyon satanlara **Naked Seller** denir [[22:46](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1366)].
- **Türev Piyasası (Derivatives Market):** 1973 yılında kurulan **Chicago Board Options Exchange (CBOE)**, modernize edilmiş ilk opsiyon borsasıdır ve türev ürün piyasalarının büyümesinde dönüm noktasıdır [[23:56](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1436)].

### 4. Opsiyonların Vade Sonu Değeri ve Put-Call Parity

- **Vade Sonundaki Durum (Exercise Date Payoff):**

  - **In the Money / Out of the Money:** Call opsiyon için hisse fiyatı strike price'ın üzerindeyse *In the money*, altındaysa *Out of the money* durumundadır [[26:44](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1604)].
  - Vade gününde opsiyonun değeri kırıklı bir doğru (**broken straight line**) çizer: max⁡(0,S−E)\max(0, S - E)max(0,S−E) [[28:13](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1693)].
- **Put-Call Parity (Put-Call Eşitliği):**

  - Bir Call opsiyon alıp aynı özelliklerde bir Put opsiyon satmak, doğrudan hisse senedi pozisyonu almayı simüle eder [[30:16](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1816)].
  - **Formül:** S=C−P+PV(E)+PV(Dividends)S = C - P + \text{PV}(E) + \text{PV}(\text{Dividends})S=C−P+PV(E)+PV(Dividends) [[32:47](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1967)].
  - Bu ilişki arbitrage (risksiz kazanç) imkanını önlemek için geçerli olmak zorundadır [[33:04](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=1984)].

### 5. Fiyatlama Modelleri ve İki Önemli Yaklaşım

- **Binomial Model & No-Arbitrage Condition:**

  - İki durumlu (up/down) basit modelde risksiz bir portföy (**Hedge Ratio**) oluşturularak opsiyon fiyatı türetilir [[44:45](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=2685)].
  - Şaşırtıcı şekilde opsiyon fiyatlamasında hissenin yukarı veya aşağı gitme **olasılığı (probability) denklemde yer almaz**; sadece no-arbitrage koşulu yeterlidir [[50:02](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3002)].
- **Black-Scholes Option Pricing Model:**

  - Fischer Black ve Myron Scholes tarafından geliştirilen süreklilik bazlı modeldir [[51:28](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3088)].
  - Opsiyon fiyatı; hisse fiyatı (SSS), strike fiyatı (EEE), vadeye kalan süre (TTT), risksiz faiz oranı (rrr) ve hisse volatilitesine (σ\sigmaσ) bağlıdır [[55:27](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3327)].

### 6. Implied Volatility (Örtük Volatilite) ve VIX

- **Implied Volatility:** Black-Scholes denklemi tersine çalıştırılarak piyasanın geleceğe dönük volatilite beklentisi elde edilir [[56:26](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3386)].
- **VIX Endeksi:** CBOE tarafından hesaplanan ve S&P 500 opsiyonlarının örtük volatilitesini gösteren "korku endeksi"dir [[57:55](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3475)].
- **Tarihsel Volatilite Sıçramaları:**

  - 1987 Borsa Çöküşü, 1990'lardaki Asya Finansal Krizi ve 2008 Lehman Brothers İflası dönemlerinde VIX tavan yapmıştır [[01:00:42](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3642)].
  - Tarihsel verilere (1871-günümüz) bakıldığında piyasa volatilitesi genel olarak istikrarlıdır; en büyük ekstrem volatilite dönemi **Büyük Buhran (Great Depression, 1930'lar)** olmuştur [[01:05:05](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=3905)].

### 7. Black-Scholes'un Sınırları ve Real-World Uygulamaları

- **Fat Tails / Black Swan Riskleri:** Black-Scholes modeli normal dağılım varsayımına dayanır; bu nedenle "Siyah Kuğu" (beklenmedik krizler ve uç değerler) risklerini tam olarak modelleyemez [[01:08:48](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=4128)].
- **Gayrimenkul ve Opsiyonlar:** Bireylerin konut fiyat düşüşlerine karşı korunması için gayrimenkul put opsiyonlarının veya mortgage'lara entegre opsiyon sistemlerinin önemi büyüktür [[01:10:08](https://www.youtube.com/watch?v=VkUEWUxI6u0&t=4208)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  17. Options Markets

  YaleCourses · 278K views

   [Open in 17. Options Markets](http://www.youtube.com/watch?v=VkUEWUxI6u0)](http://www.youtube.com/watch?v=VkUEWUxI6u0)

  ![](https://i.ytimg.com/vi/VkUEWUxI6u0/maxresdefault.jpg)
