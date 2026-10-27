# 14. Quantifying Uncertainty and Risk

<https://www.youtube.com/watch?v=yvcg_WE5O-o>

**Yale Courses – 14. Quantifying Uncertainty and Risk (Prof. John Geanakoplos)** dersinin öne çıkan ve detaylı konu başlıkları:

### 1. Belirsizlik (Uncertainty) vs. Kesinlik (Certainty)

- **Temel Fark:** Ders, o ana kadar işlenen "kesinlik" (certainty) varsayımından belirsizlik dünyasına geçişi işaret eder [[00:00](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=0)].
- **Shiller’ın Görüşü:** Robert Shiller'ın "insanların geleceğe dair olasılıkları bilmediği, sadece hikayelere/duygulara göre iyimser ya da kötümser olduğu" yaklaşımına değinilir; fakat derste olasılıkları tam olarak tanımlanabilen **Random Variables** (Rassal Değişkenler) üzerinde durulacağı belirtilir [[01:16](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=76)].

### 2. İstatistiksel Temeller: Expectation, Variance ve Standard Deviation

- **States of Nature / World:** Leibniz’in fikri olan olası durumlar üzerinden basit bir örnek kurulur (XXX: %50 ihtimalle +1+1+1, %50 ihtimalle −1-1−1) [[02:00](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=120)].
- **Beklenen Değer (Expectation / E[X]E[X]E[X]):** Değişkenin ortalama getirisini ifade eder [[02:26](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=146)].
- **Varyans (Variance / Var(X)Var(X)Var(X)) & Standart Sapma (Standard Deviation / σ\sigmaσ):**

  - Belirsizlik ve riskin ölçüsüdür [[02:42](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=162)].
  - Finansal modellerde varyans yerine **Standard Deviation** tercih edilir; çünkü ölçekleme (scaling) yapıldığında (örneğin portföyü 2 katına çıkardığınızda) Beklenen Değer ve Standart Sapma 2 katına çıkarken, Varyans 4 katına çıkar [[03:53](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=233)].
- **Aynı Ortalamaya/Varyansa Sahip Farklı Dağılımlar:** Farklı bir YYY değişkeni (%90 ihtimalle +1/3+1/3+1/3, %10 ihtimalle −3-3−3) örneği üzerinden, sadece E[X]E[X]E[X] ve Standard Deviation değerlerinin iki dağılımın tüm yapısını tek başına açıklayamayacağı gösterilir [[04:29](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=269)].

### 3. Covariance (Kovaryans) ve İlişkili Değişkenler

- **Joint Distribution (Ortak Dağılım) vs. Marginal Distributions:** Değişkenlerin tekil dağılımlarını bilmek, birlikte nasıl hareket ettiklerini (Joint Distribution) belirlemeye yetmez [[07:08](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=428)].
- **Covariance Mantığı:** İki değişkenin aynı yönde mi (long diagonal) yoksa ters yönde mi (off-diagonal) hareket ettiğini ölçer [[08:25](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=505)].
- **Bağımsızlık (Independence):**

  - İki değişken bağımsızsa Cov(X,Y)=0Cov(X, Y) = 0Cov(X,Y)=0 olur [[18:21](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1101)].
  - Bağımsızlık durumunda bir değişken hakkında bilgi sahibi olmak diğer değişken hakkında hiçbir bilgi sağlamaz [[17:59](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1079)].

### 4. Çeşitlendirme (Diversification) ve Risk Azaltımı

- **Risk/Getiri Dengesi:** Yatırımcılar genel olarak yüksek **Expectation** ister, yüksek **Standard Deviation** (risk) istemezler [[03:37](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=217)].
- **Diversification Etkisi:**

  - Parayı bağımsız iki varlığa yarı yarıya bölüştürmek (12X+12Y\frac{1}{2}X + \frac{1}{2}Y21​X+21​Y), beklenen getiriyi (E[X]=0E[X]=0E[X]=0) değiştirmes de Standart Sapmayı 111'den 12≈0.707\frac{1}{\sqrt{2}}\approx 0.7072![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
    c-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14
    c0,-2,0.3,-3.3,1,-4c1.3,-2.7,23.83,-20.7,67.5,-54
    c44.2,-33.3,65.8,-50.3,66.5,-51c1.3,-1.3,3,-2,5,-2c4.7,0,8.7,3.3,12,10
    s173,378,173,378c0.7,0,35.3,-71,104,-213c68.7,-142,137.5,-285,206.5,-429
    c69,-144,104.5,-217.7,106.5,-221
    l0 -0
    c5.3,-9.3,12,-14,20,-14
    H400000v40H845.2724
    s-225.272,467,-225.272,467s-235,486,-235,486c-2.7,4.7,-9,7,-19,7
    c-6,0,-10,-1,-12,-3s-194,-422,-194,-422s-65,47,-65,47z
    M834 80h400000v40h-400000z"></path></svg>)​1​≈0.707'ye düşürür [[22:32](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1352)].
  - **Genel Formül:** Aynı beklenen getiri EEE ve varyans σ2\sigma^2σ2'ye sahip NNN tane bağımsız riskli varlığa eşit dağıtıldığında (1N\frac{1}{N}N1​):

    - Yeni Beklenen Getiri: EEE
    - Yeni Varyans: σ2N\frac{\sigma^2}{N}Nσ2​
    - Yeni Standart Sapma: σN\frac{\sigma}{\sqrt{N}}N![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
      c-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14
      c0,-2,0.3,-3.3,1,-4c1.3,-2.7,23.83,-20.7,67.5,-54
      c44.2,-33.3,65.8,-50.3,66.5,-51c1.3,-1.3,3,-2,5,-2c4.7,0,8.7,3.3,12,10
      s173,378,173,378c0.7,0,35.3,-71,104,-213c68.7,-142,137.5,-285,206.5,-429
      c69,-144,104.5,-217.7,106.5,-221
      l0 -0
      c5.3,-9.3,12,-14,20,-14
      H400000v40H845.2724
      s-225.272,467,-225.272,467s-235,486,-235,486c-2.7,4.7,-9,7,-19,7
      c-6,0,-10,-1,-12,-3s-194,-422,-194,-422s-65,47,-65,47z
      M834 80h400000v40h-400000z"></path></svg>)​σ​ [[27:09](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1629)]
- **Tarihsel Referans:** Shakespeare’in *Venedik Taciri* oyunundaki Antonio örneği verilir (Gemilerini farklı denizlere göndererek bağımsız riskler üzerinden çeşitlendirme sağlamıştır) [[23:17](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1397)].

### 5. Merkezî Limit Teoremi ve Normal Dağılım

- **Normal Distribution (Bell Curve):** Birçok bağımsız rassal değişken toplandığında sonuç Normal Dağılım'a yaklaşır [[29:18](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1758)].
- **Parametreler:** Normal dağılım tamamen Mean (μ\muμ) ve Standard Deviation (σ\sigmaσ) ile karakterize edilir [[32:47](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1967)].
- **İktisadi Eleştiri:** Klasik iktisat modelleri Normal Dağılım varsayımına (ince kuyruklar / thin tails) dayanır ve aşırı uç olayların (outliers) neredeyse hiç yaşanmayacağını öngörür. Ancak gerçek piyasalarda çok fazla uç olay yaşandığı için bu varsayım eleştirilir [[33:03](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=1983)].

### 6. Law of Iterated Expectations (Yinelemeli Beklentiler Yasası)

- **Conditional Expectation (Koşullu Beklenti):** Yeni bilgi geldikçe olasılıkların güncellenmesiyle hesaplanan beklentidir [[35:02](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2102)].
- **Yinelemeli Beklentiler Yasası:** Bugün geleceğe dair sahip olduğunuz beklenti (E[X]E[X]E[X]), yarın elde edeceğiniz bilgiye dayalı koşullu beklentilerin bugünkü ortalamasına eşittir (E[X]=E[E[X∣Information]]E[X] = E[E[X\vert{}\text{Information}]]E[X]=E[E[X∣Information]]) [[37:45](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2265)].
- **Yankees vs. Dodgers Örneği:** 3 maçlık World Series örneğinde, ilk maçı kazanma/kaybetme durumuna göre güncellenen şansların ortalaması, başlangıçtaki toplam şansı verir [[38:42](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2322)].

### 7. Ağaç Modelleri ve Backward Induction (Geriye Doğru Tümevarım)

- **Binomial Tree (İki Terimli Ağaçlar):** Olaylar süreci zamanla dallanarak ilerler.
- **Recombining Tree (Yeniden Birleşen Ağaçlar):**

  - Üstel büyüyen (2N2^N2N) standart ağaçlar yerine, sıranın önemsiz olduğu düğümler birleştirilir (ör. 1 galibiyet - 1 mağlubiyet ile 1 mağlubiyet - 1 galibiyet aynıdır) [[43:06](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2586)].
  - Bu sayede ağaç boyutu doğrusal (NNN) büyür ve bilgisayarda hesaplamak son derece kolaylaşır [[44:07](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2647)].
- **Backward Induction:** En son noktadaki çıktı değerlerinden başlanarak, *Law of Iterated Expectations* kullanılarak bugüne doğru hesaplama yapılır [[44:59](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2699)]. Ders içinde bu mantık Excel tablosu üzerinde simüle edilmiştir [[48:37](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=2917)].

### 8. İskonto Teorisi, Sabırsızlık ve Hyperbolic Discounting

- **İmpatience (Sabırsızlık):** Irving Fisher'a göre faiz oranının ve varlık fiyatlamasının temel taşıdır [[54:21](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3261)].
- **Exponential vs. Hyperbolic Discounting:**

  - **Exponential Discounting (Üstel İskonto):** Standart modelde her yıl sabit bir δ\deltaδ oranıyla iskonto edilir (δ,δ2,δ3...\delta, \delta^2, \delta^3...δ,δ2,δ3...) [[55:06](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3306)].
  - **Hyperbolic Discounting (Hiperbolik İskonto):** İnsanlar ve hayvanlar "bugün ile yarın" arasındaki farka devasa önem verirken, "1 yıl sonraki bugün ile 1 yıl 1 gün sonra" arasındaki farkı neredeyse önemsemezler [[55:50](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3350)].
  - **Çevre İktisadı İçin Önemi:** Üstel iskontoda 100 yıl sonrası neredeyse sıfır değer taşıdığı için bugün çevreye yatırım yapmak mantıksız görünür. Ancak hiperbolik iskontoda geleceğe verilen değer daha yavaş düşer [[57:35](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3455)].

### 9. Belirsiz Faiz Oranları (Uncertain Interest Rates / Ho-Lee Model)

- **Ho-Lee Interest Rate Model:** İskonto/faiz oranının kendisi belirsiz olduğunda ve rastgele adımlarla (up/down) değiştiğinde gelecekteki 1 Doların bugünkü değeri nasıl hesaplanır? [[01:01:00](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3660)]
- **Gelecek Vadeli Nakit Akışlarını Fiyatlama:** Faiz oranları belirsiz olduğunda, geriye doğru tümevarım (backward induction) ile çok uzun vadeli (100+ yıl) iskontolarda doğal bir **Hyperbolic Discounting** etkisi ortaya çıkar [[01:01:34](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3694), [01:03:43](https://www.youtube.com/watch?v=yvcg_WE5O-o&t=3823)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  14. Quantifying Uncertainty and Risk

  YaleCourses · 57K views

   [Open in 14. Quantifying Uncertainty and Risk](http://www.youtube.com/watch?v=yvcg_WE5O-o)](http://www.youtube.com/watch?v=yvcg_WE5O-o)

  ![](https://i.ytimg.com/vi/yvcg_WE5O-o/hqdefault.jpg)
