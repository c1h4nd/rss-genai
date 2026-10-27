# 17. Backward induction: ultimatums and bargaining

<https://www.youtube.com/watch?v=XpEmuxE4qWk>

Prof. Ben Polak’ın Yale Üniversitesi’nde verdiği Oyun Teorisi dersinden (**"17. Backward induction: ultimatums and bargaining"**) çıkarılan detaylı özet ve önemli noktalar:

### 1. Ultimatom Oyunu (The Ultimatom Game) ve Gözlemler

- **Oyunun Yapısı:**

  - 2 oyuncu bulunur. Oyuncu 1, toplam pastanın/paranın (örneğin $1 veya $10) paylaşımı için bir **"Take-it-or-leave-it" (Ya kabul et ya terk et)** teklifi yapar (sss kendisine, 1−s1-s1−s diğerine).
  - Oyuncu 2 teklifi **kabul ederse (Accept)** pasta belirtildiği gibi bölünür. **Reddederse (Reject)** her iki taraf da sıfır ($0) alır [[01:06](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=66)].
- **Backward Induction (Geriye Doğru Tümevarım) Tahmini:**

  - Teorik olarak Oyuncu 2, $0 yerine $0.01 bile alsa rasyonel bir aktör olarak kabul etmelidir.
  - Bu durumda Oyuncu 1'in tek kuruş ($0.01) teklif edip paranın neredeyse tamamını kendine tutması beklenir [[05:40](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=340), [07:48](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=468)].
- **Sınıf İçi Deney ve Gerçek Dünya Sonuçları (Teoriden Sapma):**

  - Sınıftaki deneylerde 1 cent veya 30 cent gibi düşük teklifler reddedilmiştir. Teklifler ancak $5/50% seviyesine çekildiğinde kabul görmüştür [00:03:22 - 00:04:55].
  - **İnsanların düşük teklifleri reddetme nedenleri:**

    - **Gurur / Onur (Pride):** Aşağılayıcı teklifleri kabul etmeme [[06:53](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=413)].
    - **Adalet hissi ve Moral Indignation:** Dürüstlük/eşitlik normları ve karşı tarafa ceza verme/ders öğretme isteği [[10:28](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=628)].
    - **Reputation (İtibar) ve Dağıtımsal Adalet (Distributional Justice):** Oyunu gerçek hayattaki tekrarlayan etkileşimlerin bir parçası gibi görme eğilimi [[11:09](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=669), [12:48](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=768)].
- **Dictator Game İlişkisi:**

  - Karşı tarafın reddetme yetkisinin olmadığı **Dictator Game** yapıldığında bile insanların para bağışladığı/paylaştığı görülür; bu da zihinlerde yerleşmiş bir **Fairness (Adalet)** algısının varlığını kanıtlar [[13:08](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=788)].

### 2. İki Aşamalı Pazarlık Oyunu (2-Stage Bargaining Game)

- **Oyunun Yapısı ve Discounting (İskonto/Zaman Değeri):**

  - 1. Aşamada Oyuncu 1 teklif yapar. Oyuncu 2 reddederse 2. Aşamaya geçilir ve **roller değişir** (Oyuncu 2 teklif yapar) [[15:07](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=907)].
  - Zamanın geçmesi maliyetlidir; 2. Aşamadaki pasta erir veya değeri düşer. Bu durum bir **Discount Factor (Δ<1\Delta < 1Δ<1)** ile modellenir (Örn: $1 yerine 2. aşamada $0.90 olur) [[16:44](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=1004), [17:38](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=1058)].
- **Backward Induction Analizi:**

  - 2. Aşama tek aşamalı bir Ultimatom Oyununa dönüşür. 2. Aşamada teklif yapan Oyuncu 2, 2. aşamanın tüm pastasını kendine tutar.
  - Bu durum Oyuncu 2'ye yarın $1 kazandırır, ancak bugünün parasal değeriyle bu Δ×1=Δ\Delta \times 1 = \DeltaΔ×1=Δ kadardır [[25:11](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=1511)].
  - Oyuncu 1, 1. Aşamada Oyuncu 2’yi ikna edebilmek için ona en az **Δ\DeltaΔ** teklif etmelidir.
  - **Sonuç (1. Aşama Dengesi):** Oyuncu 1 kendisine 1−Δ1 - \Delta1−Δ, Oyuncu 2'ye ise Δ\DeltaΔ teklif eder ve teklif **1. aşamada kabul edilir** [[26:27](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=1587), [29:57](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=1797)].

### 3. Çok Aşamalı Pazarlık Oyunları (Multi-Stage / Alternating-Offer Bargaining)

Oyun aşama sayısı arttıkça mantık şu şekilde geriye doğru yürütülür:

- **3-Stage Game:**

  - 3. aşamaya kalırsa Oyuncu 1 her şeyi alır (bugünkü değeri Δ2\Delta^2Δ2).
  - 2. aşamada Oyuncu 2 teklif sunarken Oyuncu 1'e en az Δ\DeltaΔ (1−Δ1-\Delta1−Δ) teklif etmelidir.
  - 1. aşamada Oyuncu 1, Oyuncu 2'ye yarınki alternatif getirisi olan **Δ(1−Δ)\Delta(1-\Delta)Δ(1−Δ)** kadar ödemeli, kendine **1−Δ(1−Δ)1 - \Delta(1-\Delta)1−Δ(1−Δ)** tutmalıdır [[36:43](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2203), [37:17](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2237)].
- **4-Stage Game:**

  - Oyuncu 1, Oyuncu 2'ye 1. Aşamada **Δ(1−Δ(1−Δ))=Δ−Δ2+Δ3\Delta(1 - \Delta(1-\Delta)) = \Delta - \Delta^2 + \Delta^3Δ(1−Δ(1−Δ))=Δ−Δ2+Δ3** verir [[39:56](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2396), [41:35](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2495)].
- **10-Stage Game ve Geometric Series (Geometrik Seri):**

  - 10 aşamalı oyunda teklif geometrik seriye dönüşür: S10=1−Δ+Δ2−Δ3+⋯−Δ9S\_{10} = 1 - \Delta + \Delta^2 - \Delta^3 + \dots - \Delta^9S10​=1−Δ+Δ2−Δ3+⋯−Δ9 [[43:10](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2590)].
  - Geometrik seri toplam formülü kullanılarak basitleştirildiğinde:

    - Oyuncu 1'in aldığı pay: **1−Δ101+Δ\frac{1 - \Delta^{10}}{1 + \Delta}1+Δ1−Δ10​**
    - Oyuncu 2'nin aldığı pay: **Δ+Δ101+Δ\frac{\Delta + \Delta^{10}}{1 + \Delta}1+ΔΔ+Δ10​** [[46:45](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2805), [47:25](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=2845)].

### 4. Sonsuz Aşamalı Pazarlık Oyunu (Infinite-Horizon Bargaining - Rubinstein Model)

- **Sonsuz Aşama Limiti (∞\infty∞-stage):**

  - Teklif aşamaları sonsuza uzayabildiğinde Δ∞→0\Delta^\infty \to 0Δ∞→0 olur.
  - **Oyuncu 1'in Payı:** 11+Δ\frac{1}{1 + \Delta}1+Δ1​
  - **Oyuncu 2'nin Payı:** Δ1+Δ\frac{\Delta}{1 + \Delta}1+ΔΔ​ [00:52:08 - 00:52:51].
- **Rapid Offers (Hızlı Teklifler / Δ→1\Delta \to 1Δ→1 Limiti):**

  - Aşamalar arası bekleme süresi kısaldıkça (teklifler peş peşe yapıldıkça), iskonto faktörü Δ\DeltaΔ 1'e yaklaşır (Δ→1\Delta \to 1Δ→1) [[53:48](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3228)].
  - Bu durumda denklem: 11+1=12\frac{1}{1 + 1} = \frac{1}{2}1+11​=21​ yani **%50 / %50 eşit bölünmeye (50/50 Even Split)** dönüşür [[54:20](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3260)].

### 5. 50/50 Eşit Bölünmenin 3 Temel Varsayımı

Teorik pazarlık modelinin %50 / %50 eşit bölünmeyle sonuçlanması için **üç şartın aynı anda sağlanması gerekir** [00:55:25 - 00:57:48]:

1. **Potansiyel olarak sonsuz teklif yapabilme imkanı** *(Potentially infinite offers)*.
2. **Tekliflerin çok hızlı yapılabilmesi / Zaman kaygısının olmaması** *(No discounting / Rapid offers - Δ→1\Delta \to 1Δ→1)*.
3. **Eşit Sabırsızlık Derecesi** *(Symmetric patience / Δ1=Δ2\Delta\_1 = \Delta\_2Δ1​=Δ2​)*.

- **Patience (Sabır) Farklarının Etkisi:**

  - Gerçek hayatta tarafların iskonto oranları farklıdır. Daha **Patient (sabırlı)** olan taraf pazarlıkta her zaman daha avantajlıdır.
  - **Impatient (sabırsız/aceleci)** olan ve paraya/anlaşmaya hemen ihtiyacı olan taraf pazarlık gücünü kaybeder [[58:31](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3511), [01:06:06](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3966)].
  - *Örnekler:* Serveti az olan işçilerin/bireylerin kira/fatura ödeme baskısı nedeniyle pazarlıkta daha zayıf kalması [[01:07:33](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=4053)] veya dizilerinin senaryosuna acil ihtiyaç duyan TV kanalı yöneticilerinin grevdeki senaristlere karşı zayıf konumda olması [[01:06:54](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=4014)].

### 6. Teorik Model ile Gerçek Dünya Arasındaki Farklar ve İnefficiency (Verimsizlik)

Backward Induction teorisi gerçek dünyaya uyarlandığında **iki büyük gerçek dışı tahmin** ortaya koyar [01:00:21 - 01:02:00]:

1. **No Haggling (Pazarlıksız İlk Aşamada Kabul):** Teoriye göre pazarlık süreci yalnızca zihinde simüle edilir ve **ilk yapılan teklif derhal kabul edilir**, gerçek hayattaki gibi tekliflerin gidip geldiği süreçler yaşanmaz [[01:01:24](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3684)].
2. **Incomplete Information (Eksik/Gizli Bilgi):**

- Modelde tarafların pastanın büyüklüğünü (PieSizePie SizePieSize) ve birbirlerinin sabır düzeyini (Δ\DeltaΔ) tam bildiği varsayılır [[01:05:00](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3900)].
- Gerçek dünyada ise **Uncertainty (belirsizlik)** vardır. Taraflar ne kadar sabırlı veya sert durduklarını kanıtlamak için teklifleri reddederler [[01:02:40](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3760), [01:04:20](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=3860)].
- Bu durum gerçek hayatta pazarlıkların uzamasına, **Strike (grev)** durumlarına ve ekonomik **Inefficiency (verimsizliğe / kayıplara)** yol açar [[01:10:16](https://www.youtube.com/watch?v=XpEmuxE4qWk&t=4216)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  17. Backward induction: ultimatums and bargaining

  YaleCourses · 43K views

   [Open in 17. Backward induction: ultimatums and bargaining](http://www.youtube.com/watch?v=XpEmuxE4qWk)](http://www.youtube.com/watch?v=XpEmuxE4qWk)

  ![](https://i.ytimg.com/vi/XpEmuxE4qWk/hqdefault.jpg)
