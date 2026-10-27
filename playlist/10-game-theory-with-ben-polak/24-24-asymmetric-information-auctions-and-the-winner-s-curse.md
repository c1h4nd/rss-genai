# 24. Asymmetric information: auctions and the winner's curse

<https://www.youtube.com/watch?v=pJAhnc8VuDo>

Yale Üniversitesi'nin **"Game Theory" (Oyun Teorisi)** dersinden *"Asymmetric Information: Auctions and the Winner's Curse"* (Asimetrik Bilgi: İhaleler ve Kazananın Laneti) başlıklı videonun detaylı ders özeti ve öne çıkan ana noktaları aşağıda sıralanmıştır:

### 1. Giriş ve Kuramsal Bağlam (00:00 - 02:20)

- **Önceki Konulardan Farkı:** Dersin bu aşamasına kadar oyuncuların kendi payoff'larını ve rakiplerinin payoff'larını tam olarak bildiği senaryolar incelenmişti.
- **Asymmetric Information:** Bu derste ise oyuncuların rakiplerinin payoff'larını (örneğin satılan bir mala ne kadar değer biçtiklerini) **bilmediği** durumlar ve ihaleler (auctions) ele alınır.

### 2. Bilgi Yapısı: Common Values vs. Private Values (02:20 - 08:20)

İhale modellerinde değer takdiri açısından iki aşırı uç (extreme) tanımlanır:

- **Common Values (Ortak Değerler):**

  - Satılan malın gerçek değeri (VVV) **tüm katılımcılar için aynıdır**.
  - Katılımcılar malın gerçek değerini kesin olarak bilmez, sadece kendi tahminlerine (estimates) dayanarak teklif verirler.
  - **Örnek:** Petrol arama sahası ihaleleri (Oil wells) veya sınıfta yapılan bozuk para dolu kavanoz ihalesi.
- **Private Values (Özel/Kişisel Değerler):**

  - Malın katılımcı için değeri tamamen **kişiye özeldir (idiosyncratic)** ve bir katılımcının değerlemesi (ViV\_iVi​), diğer bir katılımcının değerlemesinden veya tatmininden tamamen bağımsızdır.
  - Tek bir kişinin değerlemesi başkası için önem taşımaz.
  - **Örnek:** Tekrar satılma ihtimali olmayan, anında tüketilen **pure consumption goods** (örneğin eBay'de satılan bir pasta).
- **Gerçek Hayat Uyumlaması:** Çoğu durum bu iki uç arasında yer alır:

  - *Ev Alımı (Homes):* Yaşama/kullanım kısmı private value olsa da ileride yeniden satma (investment/resale value) faktörü nedeniyle içinde common value öğeleri barındırır.

### 3. Sınıf İçi Deney ve "Winner's Curse" (Kazananın Laneti) (08:20 - 27:00)

- **Deney:** Profesör sınıfta bozuk para dolu iki kavanoz (büyük ve küçük) için kapalı zarf usulü teklif (first-price sealed bid) toplayarak ihale gerçekleştirir.
- **Sonuç:** Büyük kavanozdaki gerçek değer $2.07 olmasına rağmen, en yüksek teklifi veren öğrenci **$5.00** teklif ederek ihaleyi kazanır ve ciddi oranda zarar eder.
- **Winner's Curse Nedir?**

  - Common value ihalelerinde, katılımcıların tahminleri gerçek değer etrafında bir gürültü (Yi=V+ϵiY\_i = V + \epsilon\_iYi​=V+ϵi​) barındırır.
  - İhaleyi kazanan kişi, **en yüksek tahmini (Yi=max⁡Y\_i = \maxYi​=max)** yapan kişidir. Yani sistematik olarak **en büyük pozitif hatayı/sapmayı (ϵi=max⁡\epsilon\_i = \maxϵi​=max)** yapan kişi kazanır.
  - Bu durum, kazananın malın gerçek değerinin çok üzerinde teklif vererek zarar etmesine yol açar (**Winner's Curse**).
- **Gerçek Dünya Örnekleri:**

  - Meksika Körfezi'ndeki petrol kuyusu ihaleleri.
  - Beyzbol serbest oyuncu transferleri (Free Agent market).
  - Şirket halka arzları (IPOs - Initial Public Offerings).

### 4. Winner's Curse'ten Korunma ve Doğru Bidding Stratejisi (27:00 - 42:40)

- **Yanlış Strateji (Naive Bidding):** Sadece kendi tahminini (YiY\_iYi​) esas alıp bundan çok az bir miktar düşerek teklif vermek (shading).
- **Koşullu Tahmin (Conditional Estimation):**

  - Başkalarının tahminlerinin sizinkinden düşük olduğunu öğrenmek, sizin malın değerine dair inancınızı da aşağı çeker.
  - Yalnızca **ihaleyi kazandığınız durumda** ihale sonucunun sizin için bir anlamı vardır.
  - İhaleyi kazanmak, aslında sizin tahmininizin gruptaki en yüksek tahmin (Yi≥YjY\_i \ge Y\_jYi​≥Yj​) olduğu bilgisini içerir.
- **Altın Kural (Bid as if you know you win):**

  - İhaleye girerken teklifinizi **"İhaleyi kazandığımı farz etseydim, bu malın değerini ne olarak tahmin ederdim?"** düşünce deneyine (counterfactual) göre belirlemelisiniz.
  - Teklifi bu şekilde ciddi oranda düşürmek (shade down etmek), ihale sonrasında yaşanacak regret (pişmanlık) durumunu engeller.

### 5. İhale Formatları (Auction Formats) (42:40 - 52:45)

Ders 4 temel ihale yapısını inceler:

1. **First-Price Sealed-Bid Auction:** Herkes kapalı teklif verir; en yüksek teklifi veren kazanır ve **kendi teklif ettiği tutarı** öder.
2. **Second-Price Sealed-Bid Auction (Vickrey Auction):** Herkes kapalı teklif verir; en yüksek teklifi veren kazanır ancak **ikinci en yüksek teklifi** öder.
3. **Ascending Open Auction (English Auction):** Fiyat sıfırdan başlayarak yükselir, katılımcılar çekildikçe en son kalan kişi kazanır (Örn: eBay).
4. **Descending Open Auction (Dutch Auction):** Fiyat çok yüksekten başlar ve aşağı doğru iner; ilk elini kaldıran teklifi veren kazanır (Örn: Filene's Basement).

#### Formatlar Arasındaki Eşdeğerlikler:

- **D=AD = AD=A (Dutch Auction ≡\equiv≡ First-Price Sealed-Bid):** Katılımcıların kafasında el kaldıracağı bir fiyat eşiği vardır. Dışarıdan bakıldığında bu durum stratejik olarak kapalı zarf teklif vermekle tamamen aynıdır.
- **B≈CB \approx CB≈C (Vickrey Auction ≈\approx≈ English Auction):** English auction'da kazanan kişi son ana kadar elini kaldırmaya devam eder ancak ödediği nihai fiyat, elini indiren **ikinci en son kişinin bıraktığı fiyat** olur. (Private value ortamında stratejik olarak ikinci fiyat kapalı zarf ihalesiyle benzeşir).

### 6. Private Value Ortamında Optimal Bidding (52:45 - 59:45)

Common value ve Winner's Curse faktörünün olmadığı sırf **Private Value** senaryolarında:

- **Second-Price / Open Ascending (eBay) Auctions:**

  - Kendi gerçek değerini teklif etmek (bi=Vib\_i = V\_ibi​=Vi​) bir **weakly dominant strategy**'dir (zayıf baskın strateji).
  - Değerinin üzerinde teklif vermek zarar riski taşır, altında teklif vermek ise karlı bir fırsatı kaçırmanıza yol açar.
- **First-Price Auctions:**

  - Kendi gerçek değerini teklif etmek (bi=Vib\_i = V\_ibi​=Vi​) **weakly dominated** bir stratejidir, çünkü kazansanız bile surplus (kâr/fayda) sıfır olur.
  - Dolayısıyla teklifinizi kendi değerinizin altına çekmelisiniz (bi<Vib\_i < V\_ibi​<Vi​).
  - Burada klasik bir **marginal benefit vs. marginal cost** dengesi vardır: Teklifi yükseltmek kazanma olasılığını artırır (marjinal fayda), ancak kazanıldığında elde edilecek surplus'ı azaltır (marjinal maliyet).

### 7. Revenue Equivalence Theorem (Gelir Eşdeğerliği Teoremi) (59:45 - 01:02:21)

- **Soru:** Satıcı açısından bakıldığında, katılımcıların gerçek değerlerini sunduğu fakat ikinci fiyatı ödediği *Second-Price Auction* mı, yoksa katılımcıların tekliflerini düşürerek verdikleri ama kazananın teklifini ödediği *First-Price Auction* mı daha fazla gelir sağlar?
- **Teorem (Revenue Equivalence Theorem):**

  - Bağımsız, simetrik ve özel değerlemeli (**Independent Symmetric Private Values**) bir ortamda;
  - Denge durumunda en yüksek değere sahip olan katılımcının ürünü kazandığı **tüm ihale formatları (First-price, Second-price vb.) bekleme/ortalamada (in expectation) tam olarak aynı geliri (Revenue) üretir.**

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    24. Asymmetric information: auctions and the winner's curse

    YaleCourses · 58K views

     [Open in 24. Asymmetric information: auctions and the winner's curse](http://www.youtube.com/watch?v=pJAhnc8VuDo)](http://www.youtube.com/watch?v=pJAhnc8VuDo)

    ![](https://i.ytimg.com/vi/pJAhnc8VuDo/hqdefault.jpg)
