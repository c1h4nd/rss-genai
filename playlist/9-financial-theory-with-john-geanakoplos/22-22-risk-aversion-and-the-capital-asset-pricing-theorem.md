# 22. Risk Aversion and the Capital Asset Pricing Theorem

<https://www.youtube.com/watch?v=aGQsjueE07Y>

Yale University'da **Prof. Robert Shiller** tarafından verilen **"22. Risk Aversion and the Capital Asset Pricing Theorem"** başlıklı bu dersin detaylı, ana başlıklar halinde özetlenmiş özeti aşağıdadır:

### 1. Giriş ve Temel Problem: Hedging ve Reel Risk

- **Capital Asset Pricing Model (CAPM):** Finans teorisinin en büyük başarılarından biridir.
- **Tam Hedging İmkânsızlığı:** Bireyler piyasadaki tüm risklerden tamamen kaçınmak (**hedge**) isterler. Ancak ekonomide petrol krizleri gibi **aggregate risk** (toplam risk) bulunduğu için herkesin her koşulda aynı tüketimi elde etmesi imkânsızdır.
- **Shakespeare ve Merchant of Venice Örneği:**

  - Antonio, gemilerini farklı denizlere göndererek **diversification** (çeşitlendirme) yapar.
  - Portia ile evlenmek için riskli sandıkları seçen talipler, yüksek risk karşılığında yüksek ödül ararlar (**Risk-Return Tradeoff**).
  - Riskli varlıkların fiyatı, beklenen getirilerinden (**expected payoff**) daha düşük olmalı; yani riskli varlıklar daha yüksek **expected rate of return** sunmalıdır.

### 2. St. Petersburg Paradox ve Expected Utility Theory

- **St. Petersburg Paradox (Bernoulli):** Tura gelene kadar yazı-tura atılan ve nnn. atışta 2n2^n2n dolar ödeyen bir oyunda **expected payoff** sonsuzdur (∞\infty∞). Ancak insanlar bu oyuna sadece çok küçük tutarlar ($4 gibi) ödemeye razıdır.
- **Expected Utility:** Daniel Bernoulli, insanların doğrudan nominal parasal getiriye değil, o getirinin sunduğu faydaya (**utility**) odaklandığını öne sürmüştür.
- **Diminishing Marginal Utility (Azalan Marjinal Fayda):** Utility fonksiyonu içbükeydir (**concave**, U′′(x)<0U''(x) < 0U′′(x)<0). Servet arttıkça ek her bir doların sunduğu marjinal fayda azalır.
- **Risk Aversion (Riskten Kaçınma):** Concave utility fonksiyonuna sahip bireyler, kesin bir getiriyi aynı beklenen değere sahip riskli/kumar bir getiriye tercih ederler.

### 3. Quadratic Utility ve Mean-Variance Analizi

- **Quadratic Utility:** U(x)=x−12αx2U(x) = x - \frac{1}{2} \alpha x^2U(x)=x−21​αx2
- **Matematiksel Kolaylık:** Utility beklentisi alındığında, sonuç sadece E[X]E[X]E[X] (**expected return**) ve Var(X)Var(X)Var(X) (**variance**) cinsinden ifade edilebilir:

  Expected Utility≈E[X]−sabit⋅Var(X)\text{Expected Utility} \approx E[X] - \text{sabit} \cdot Var(X)Expected Utility≈E[X]−sabit⋅Var(X)
- Bireyler beklenen getiriden memnun olurken, yüksek varyans (risk) sebebiyle faydalarını cezalandırırlar. CAPM'in temeli bu **Mean-Variance** basitleştirmesine dayanır.

### 4. Arrow-Debreu General Equilibrium Model & State-Contingent Securities

- **Fisher’s Trick & Arrow-Debreu:** Farklı zaman ve durumlardaki (**states of nature**) mallar farklı **state-contingent commodities** olarak fiyatlandırılır.
- **Arrow Securities:** Belirli bir sss durumunda 1 birim ödeyen, diğer durumlarda 0 ödeyen menkul kıymetlerdir (psp\_sps​ fiyatlı).
- **Genel Denge (Equilibrium):** Her birey marjinal faydasını fiyatlara oranlar:

  MU0p0=MUsps\frac{MU\_0}{p\_0} = \frac{MU\_s}{p\_s}p0​MU0​​=ps​MUs​​

### 5. İki Farklı Senaryo Analizi (Dersteki Sayısal Model)

#### **Senaryo A: Aggregate Risk Olmayan Ekonomi (No Aggregate Risk)**

- Toplam üretimin tüm durumlarda sabit (500500500) olduğu durum.
- **Sonuç:** Bireyler **diversification** (çeşitlendirme) yaparak tüm kişisel riskleri ortadan kaldırırlar.
- Durum fiyatları (psp\_sps​) doğrudan olasılıklarla (γs\gamma\_sγs​) orantılı çıkar (ps/γs=sabitp\_s / \gamma\_s = \text{sabit}ps​/γs​=sabit).
- Risk primi gerekmez, varlıklar sadece **riskless interest rate** ile iskonto edilir.

#### **Senaryo B: Aggregate Risk İçeren Ekonomi (Real World Risk)**

- Toplam üretimin durumlara göre değiştiği (S1=200,S2=280,S3=440S\_1=200, S\_2=280, S\_3=440S1​=200,S2​=280,S3​=440) durum.
- **Sonuçlar:**

  - Bireyler riskin tamamından kaçınamaz (**aggregate risk** kalır).
  - Kötü durumda (S1S\_1S1​) kıtlık olduğu için o duruma ait Arrow security fiyatı (p1/γ1p\_1 / \gamma\_1p1​/γ1​) yüksek, bolluk olan S3S\_3S3​ durumunun fiyatı düşük çıkar.
  - Riskli durumların fiyatı sadece olasılığa bağlı kalmaz; **risk aversion** nedeniyle varlığın piyasa geneliyle olan korelasyonu fiyatı belirler.

### 6. Ana Çıkarımlar ve İki Büyük Teorem

- **Mutual Fund Theorem (Two-Fund Separation Theorem):**

  - Piyasa dengesinde, binlerce hisse senedi veya karmaşık durum olmasına rağmen **her yatırımcı aynı iki temel varlığı tutar:**

    1. **Riskless Asset** (Risk-free borçlanma/borç verme veya banka mevduatı).
    2. **Market Portfolio** (Piyasadaki tüm riskli hisse senetlerinin içinde bulunduğu toplam piyasa portföyü).
  - Riskten daha çok kaçınan biri (**more risk-averse**) market portfolio oranını düşürüp parayı risksiz varlığa yatırır; riski seven biri ise risksiz varlıktan borçlanıp market portfolio oranını artırır.
- **Piyasa Uygulaması & Credit Default Swaps (CDS):**

  - Gerçek dünyada tam anlamıyla Arrow Securities olmasa da CDS gibi **event-contingent** türev araçlar bu mantığa yaklaşır.

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    22. Risk Aversion and the Capital Asset Pricing Theorem

    YaleCourses · 57K views

     [Open in 22. Risk Aversion and the Capital Asset Pricing Theorem](http://www.youtube.com/watch?v=aGQsjueE07Y)](http://www.youtube.com/watch?v=aGQsjueE07Y)

    ![](https://i.ytimg.com/vi/aGQsjueE07Y/hqdefault.jpg)
