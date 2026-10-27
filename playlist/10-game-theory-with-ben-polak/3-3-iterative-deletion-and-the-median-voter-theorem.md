# 3. Iterative deletion and the median-voter theorem

<https://www.youtube.com/watch?v=kqDu0RVWTYw>

Yale Üniversitesi’nin **"Iterative Deletion and the Median-Voter Theorem"** (Oyun Teorisi Ders 3) başlıklı bu dersinin detaylı Türkçe özeti ve öne çıkan önemli noktaları aşağıda sıralanmıştır:

### 1. Iterative Deletion of Dominated Strategies (Baskılanmış Stratejilerin Ardışık Elemesi)

- **Temel Kavram [[00:06](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=6)]:** Oyuncuların hiçbir senaryoda kendilerine en yüksek faydayı sağlamayacak "dominated" (baskılanmış/baskın olmayan) stratejileri elemesi, ardından yeni oluşan oyunda tekrar baskılanmış stratejileri bulup onları da elemesi sürecine denir.
- **Manevi/Mantıksal Boyut [[00:37](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=37)]:** Kendini başkasının yerine koyma, onun ne yapacağını tahmin etme ve karşı tarafın da aynısını sizin için düşündüğünü öngörme mantığına dayanır.
- **Uygulamada Dikkat Edilmesi Gereken İpucu [[01:45](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=105)]:** Hata yapmamak için her adımda **tüm oyuncuların** o turdaki dominated stratejileri aynı anda tespit edilmeli, ardından topluca elenip bir sonraki tura geçilmelidir.

### 2. Siyasette Bir Uygulama: Siyasi Spektrum ve Seçim Modeli

Dersin ilk yarısında bu eleme yöntemi siyaset biliminden bir model üzerinde detaylandırılır:

- **Modelin Kuralları [[02:21](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=141)]:**

  - **Oyuncular:** 2 aday/parti.
  - **Stratejiler (Siyasi Spektrum):** 111'den 101010'a kadar numaralandırılmış siyasi pozisyonlar (111 aşırı sol, 101010 aşırı sağ) [[03:03](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=183)].
  - **Seçmen Dağılımı:** Seçmenlerin %10'u her bir pozisyonda bulunmaktadır (üniform dağılım) [[04:13](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=253)].
  - **Seçmen Davranışı:** Seçmenler kendilerine en yakın olan adaya oy verir; eşit uzaklıktaki durumlarda (tie) oylar yarı yarıya bölünür [[04:31](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=271)].
  - **Payoff (Kazanç):** Adayların amacı aldıkları oy oranını (share of the vote) maksimize etmektir [[05:24](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=324)].
- **Adım Adım Iterative Deletion Süreci:**

  1. **1. Tur [[06:48](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=408)]:** 111 numaralı pozisyon 222 numaralı pozisyon tarafından *strictly dominate* edilir (Çünkü rakip ne yaparsa yapsın, 222'de durmak 111'de durmaktan her zaman %5 daha fazla oy kazandırır) [[12:34](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=754)]. Simetrik olarak 101010 numaralı pozisyon da 999 tarafından dominate edilir [[13:16](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=796)]. 111 ve 101010 elenir.
  2. **2. Tur [[17:44](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1064)]:** Seçmenler yerinde kalsa da adayların 111 ve 101010'a geçmeyeceği anlaşıldıktan sonra, yeni oyunda 222 numaralı pozisyon 333 tarafından, 999 numaralı pozisyon da 888 tarafından dominate edilir [[20:25](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1225)]. 222 ve 999 elenir.
  3. **Devam Eden Turlar [[21:46](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1306)]:** Sırasıyla 333 ve 888, ardından 444 ve 777 elenir.
  4. **Sonuç [[22:25](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1345)]:** Geride sadece **555 ve 666** (merkez pozisyonlar) kalır.

### 3. Median-Voter Theorem (Ortanca Seçmen Teoremi)

- **Teoremin Tahmini [[24:03](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1443)]:** Seçimi kazanmak veya oy oranını artırmak isteyen adaylar merkeze yığılır (**crowd the center**). Politikalar merkezin (ortanca seçmenin) taleplerine göre şekillenir.
- **Tarihten / Gerçek Hayattan Örnekler [[24:32](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1472)]:**

  - **Siyaset (ABD):** 1960 Kennedy-Nixon tartışmaları (Kennedy'nin merkeze yaklaşması), 1968 Nixon ve 1992 Bill Clinton'ın merkeze kayma stratejileri [[24:47](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1487)].
  - **Ekonomi (Hotelling's Law / Product Placement) [[25:54](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1554)]:** Benzin istasyonlarının veya mağazaların kasabaya eşit dağılmak yerine aynı cadde/kavşakta yan yana toplanması.
- **Modelin Eksikleri ve Eleştirisi (Varsayımların Esnetilmesi) [[28:42](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1722)]:**

  - **Seçmenlerin homojen dağılmaması:** Seçmenler Çan Eğrisi (bell curve) şeklinde dağılsa bile merkezde toplanma sonucu **değişmez** [[35:49](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2149)].
  - **İkiden fazla aday olması / Oy kullanmama (Not voting) seçeneği:** Sonucu doğrudan değiştirir [[30:46](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1846)].
  - **Taahhüt edememe (Inability to commit) / Güvenilirlik:** Adayın "Ben merkezdeyim" demesi seçmen tarafından inandırıcı bulunmayabilir; geçmiş performans/track record önem kazanır [[31:53](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1913)].
  - **Çok boyutluluk (High dimensions):** Siyasetin sadece Sol-Sağ ekseninde değil; çevre, dış politika, karakter vb. farklı boyutlarda yürümesi [[30:08](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=1808)].

### 4. Yeni Analiz Aracı: Best Response (En İyi Tepki)

- **Tanım [[40:39](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2439)]:** Karşı tarafın belirli bir stratejisine veya **inancına (belief / probability)** karşılık oyuncunun elde edebileceği beklenen getiriyi (expected payoff) maksimize eden stratejidir.
- **Matris Örneği Üzerinden İnceleme [[40:54](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2454)]:**

  - Player 1 Stratejileri: Up(U)Up (U)Up(U), Middle(M)Middle (M)Middle(M), Down(D)Down (D)Down(D)
  - Player 2 Stratejileri: Left(L)Left (L)Left(L), Right(R)Right (R)Right(R)
  - Bu oyunda hiçbir strateji *dominated* değildir; bu yüzden iterative deletion işe yaramaz [[41:36](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2496)].
- **Best Response ve Beklenen Getiri Hesabı [[43:44](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2624)]:**

  - Karşı taraf kesinlikle LeftLeftLeft oynuyorsa →\rightarrow→ Best Response: **UpUpUp**
  - Karşı taraf kesinlikle RightRightRight oynuyorsa →\rightarrow→ Best Response: **MiddleMiddleMiddle**
  - Karşı tarafın %50 LeftLeftLeft, %50 RightRightRight oynayacağına inanılıyorsa [[46:48](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2808)]:

    - Expected Payoffs:Expected\ Payoffs:Expected Payoffs: Up=2.5Up = 2.5Up=2.5, Middle=2.5Middle = 2.5Middle=2.5, Down=3.0Down = 3.0Down=3.0
    - Bu olasılıkta Best Response: **DownDownDown** [[48:28](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=2908)].
- **Grafik Analizi (Expected Payoff vs Beliefs) [[50:04](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3004)]:**

  - Yatay eksen: Rakibin RightRightRight oynama olasılığı (PRP\_RPR​) [[50:13](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3013)].
  - Dikey eksen: Oyuncunun beklenen getirisi (Expected PayoffExpected\ PayoffExpected Payoff) [[50:43](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3043)].
  - Rakibin RightRightRight oynama olasılığı 000 ile xxx arasındaysa (PR<xP\_R < xPR​<x) →\rightarrow→ **Best Response: UpUpUp** [[57:01](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3421)].
  - Olasılık xxx ile yyy arasındaysa (x<PR<yx < P\_R < yx<PR​<y) →\rightarrow→ **Best Response: DownDownDown** [[58:08](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3488)].
  - Olasılık yyy'den büyükse (PR>yP\_R > yPR​>y) →\rightarrow→ **Best Response: MiddleMiddleMiddle** [[57:31](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3451)].
  - xxx ve yyy denge noktalarını bulmak için iki stratejinin beklenen getiri denklemleri birbirine eşitlenir [[59:04](https://www.youtube.com/watch?v=kqDu0RVWTYw&t=3544)].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    3. Iterative deletion and the median-voter theorem

    YaleCourses · 184K views

     [Open in 3. Iterative deletion and the median-voter theorem](http://www.youtube.com/watch?v=kqDu0RVWTYw)](http://www.youtube.com/watch?v=kqDu0RVWTYw)

    ![](https://i.ytimg.com/vi/kqDu0RVWTYw/hqdefault.jpg)
