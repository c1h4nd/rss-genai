# 17. Callable Bonds and the Mortgage Prepayment Option

<https://www.youtube.com/watch?v=rH-0KBgQk2E>

Bu ders, **Prof. John Geanakoplos** tarafından Yale Üniversitesi'nde verilen *Callable Bonds* (çağrılabilir/faiz düşüşünde geri çağrılabilir tahviller) ve *Mortgage Prepayment Options* (ipotekli konut kredisini erken ödeme opsiyonu) konularını ele almaktadır.

Dersin öne çıkan önemli noktaları ve detaylı özeti aşağıda sıralanmıştır:

### 1. Temel Yaklaşım ve Yöntem

- **Opsiyon Değerlemesi:** Opsiyonların (bir şeyi yapma veya yapmama hakkı) çoğu zaman insanların fark ettiğinden daha değerli olduğu ve değerlerinin **Backward Induction** (geriye doğru tümevarım) yöntemiyle hesaplandığı vurgulanmaktadır [[00:23](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=23)].
- **Faiz Oranlarında Belirsizlik (Geometric Random Walk):**

  - Faiz oranlarının gelecekte nasıl hareket edeceği ikili/ağaç modeli (**Binomial Tree / Geometric Random Walk**) ile modellenir [[05:00](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=300)].
  - Faiz oranı her dönem bir `up multiplier` (eσ+de^{\sigma + d}eσ+d) veya `down multiplier` (e−σ+de^{-\sigma + d}e−σ+d) ile çarpılarak hareket eder [[05:28](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=328)].
  - Ağaçlarda hesaplama kolaylığı için eksponansiyel notation kullanılır [[06:32](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=392)].

### 2. Callable Bonds (Çağrılabilir Tahviller)

- **Yapısı:**

  - Şirket belirli bir kupon faizi ödeme sözü verir (örneğin %9 kupon ödemesi) [[01:34](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=94)].
  - Vade sonunda anapara (ör. 100$) ödenir. Şirket, istediği bir aşamada kupon ödemesini yaptıktan sonra anaparayı (100$) ödeyerek borcu sonlandırma (**Call Option**) hakkına sahiptir [[01:44](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=104)].
- **Callable vs. Non-Callable Bond:**

  - **Non-Callable Bond:** Şirketin vadeden önce borcu bitirme opsiyonu yoktur. Örnekte başlangıç faizi %8 iken kupon %9 olduğundan, bu tahvilin bugünkü değeri **113.23$** seviyesindedir [[18:50](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1130)].
  - **Callable Bond:** Şirket 100$ ödeyip borcu bitirebildiği için bu opsiyon tahvilin değerini **95.52$** seviyesine düşürür [[23:35](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1415)].
  - Araya giren fark (**18$ civarı / ~%18**), şirketin elindeki Call Option'ın ne kadar devasa bir değere sahip olduğunu gösterir [[24:26](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1466)].
- **Erken Çağırma Stratejisi (Optimal Execution):**

  - Şirket faizler %8'den %6.8'e ilk düştüğünde tahvili hemen geri çağırmayabilir [[23:16](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1396)]. Çünkü faizlerin gelecekte daha da yükselip borcu şirket lehine çevirmesi ihtimali (opsiyon zaman değeri) vardır [[21:03](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1263)].
  - Ancak zaman azaldıkça ve faiz düşük kaldıkça opsiyonun zaman değeri azalır ve şirket zararı kesmek için tahvili çağırır (100$ öder) [[31:55](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1915)].

### 3. Modelin Genişletilmesi: Trinomial Trees

- İkili ağaç (Binomial) modeli gerçek hayattaki çoklu ihtimalleri basitleştirir. Ancak model **Trinomial Tree** (üçlü ağaç: yukarı, sabit, aşağı) veya çoklu adımlara genişletilse bile sonuçlar neredeyse aynı çıkar [[32:45](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=1965)].
- Varyans ve beklenti (mean & variance) sabit tutulacak şekilde volatilite adjustment (2⋅σ\sqrt{2} \cdot \sigma2![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
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
  M834 80h400000v40h-400000z"></path></svg>)​⋅σ) yapıldığında:

  - Non-Callable Bond: **113.23$** [[41:37](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=2497)]
  - Callable Bond: **95.14$** [[41:45](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=2505)]
- Bu durum, dönemsel adımlar kısaltıldığı sürece Binomial modelin genelliği bozmadan gayet doğru sonuçlar verdiğini kanıtlar [[42:11](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=2531)].

### 4. Mortgage ve Erken Ödeme Opsiyonu (Prepayment Option)

- **Amortizing Mortgage Yapısı:**

  - Mortgage, belirli bir süre boyunca (ör. 30 yıl) her dönem sabit ödeme (XXX) yapılan bir amortisman yapısıdır [[43:26](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=2606)].
  - Her ödeme iki bileşenden oluşur: **Interest Payment** (Faiz ödemesi) ve **Scheduled Principal Reduction** (Anapara düşüşü) [[55:05](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3305)].
  - Zaman geçtikçe kalan anapara borcu (BtB\_tBt​) azaldığı için yapılan ödemelerin daha büyük bir kısmı anapara indirimine gider [[57:56](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3476)].
- **Erken Ödeme Hakkı (Prepayment Option):**

  - Ev sahibi, kupon ödemesini yaptıktan sonra kalan anapara bakiyesini (BtB\_tBt​) tek seferde ödeyip mortgage'ı kapatma hakkına (**Prepay**) sahiptir [[54:41](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3281)].
  - Faizler yükseldiğinde ev sahibi düşük sabitlemiş olduğu faizden borçlanmaya devam ettiği için kârlı durumdadır (ev sahipleri faizlerin yükselmesini temenni etmelidir) [[01:01:57](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3717)].
  - Faizler düştüğünde ise ev sahibi kredisini kapatıp daha düşük faizle yeniden borçlanabilir (**Refinancing**) [[01:03:17](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3797)].

### 5. Banka ve Ev Sahibi Açısından Değerleme & Mantık Dışılık

- **Neden Mortgage Faizleri Piyasa Faizinden Yüksektir?**

  - Piyasa faizi %6 iken bir banka %7-%8 faizle mortgage verir [[59:06](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3546)].
  - Sebebi, ev sahibine bedelsiz verilen **Prepayment Option**'ın banka riskini artırmasıdır [[01:01:15](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=3675)].
  - Tamamen rasyonel davranan ev sahipleri karşısında bankanın bu opsiyon nedeniyle zarar etmemesi için mortgage kupon faizini piyasa faizinin oldukça üzerinde tutması gerekir [[01:07:54](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=4074)].
- **Rasyonel Olmayan Davranışlar ve Finansal Gerçeklik:**

  - Uygulamada bankalar mortgage faizlerini teorik olarak hesaplanan aşırı yüksek seviyelere çıkarmazlar [[01:09:34](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=4174)].
  - Çünkü toplumdaki borçluların tamamı rasyonel davranarak faiz düştüğünde kredisini erken ödemez (**Inattention**, prosedür zahmeti/hassle, finansal okuryazarlık eksikliği) [[01:11:48](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=4308)].
  - Bankalar ve mortgage hedge fund'ları, nüfusun ne kadarının rasyonel (*smart*) ne kadarının opsiyonu kullanmayan (*dumb/inattentive*) kişilerden oluştuğunu geçmiş verilerden kalibre ederek modellerini kurarlar [[01:10:01](https://www.youtube.com/watch?v=rH-0KBgQk2E&t=4201)].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    17. Callable Bonds and the Mortgage Prepayment Option

    YaleCourses · 30K views

     [Open in 17. Callable Bonds and the Mortgage Prepayment Option](http://www.youtube.com/watch?v=rH-0KBgQk2E)](http://www.youtube.com/watch?v=rH-0KBgQk2E)

    ![](https://i.ytimg.com/vi/rH-0KBgQk2E/hqdefault.jpg)
