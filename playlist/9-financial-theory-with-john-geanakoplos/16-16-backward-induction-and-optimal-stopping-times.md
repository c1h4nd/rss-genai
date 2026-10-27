# 16. Backward Induction and Optimal Stopping Times

<https://www.youtube.com/watch?v=IPNl-jD1vhw>

Yale Courses kanalına ait **"16. Backward Induction and Optimal Stopping Times"** başlıklı dersin öne çıkan konuları ve detaylı özeti:

### 1. Default (Temerrüt) İhtimalleri ve İskonto Oranları

- **Temerrüt Modeli:**

  - Borçluların ödeme zamanı gelmeden temerrüde düşmeyeceği varsayılır [[01:45](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=105)].
  - Bir aşamada temerrüt gerçekleştiğinde, sonraki dönem ödemelerinin sıfır (000) olacağı kabul edilir [[02:17](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=137)].
- **Temerrüdün İskonto Etkisi:**

  - Temerrüt ihtimali (DDD), gelecekteki nakit akışlarını 1−D1 - D1−D ile çarpmak anlamına gelir [[03:40](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=220)].
  - Bu durum, finansal matematikte ek bir risk primi / spread ekleyerek daha yüksek bir iskonto oranı (R+SR + SR+S) kullanmakla aynı etkiyi yaratır [[05:15](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=315)].
- **Forward Rate & Default Spread İlişkisi:**

  - ABD tahvilleri (temerrüt riski içermeyen) ile Arjantin tahvilleri (temerrüt riski taşıyan) karşılaştırıldığında, Arjantin forward oranlarının daha yüksek olması temerrüt olasılığından kaynaklanır [[18:32](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=1112)].
  - Temerrüt olasılığı çok küçük olduğunda, iki ülkenin forward oranları arasındaki fark doğrudan **Default Spread** (Temerrüt Marjı) olarak adlandırılır [[27:48](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=1668)].

### 2. Backward Induction (Geriye Dönük Tümevarım)

- **Tarihsel ve Matematiksel Arka Plan:**

  - Kavram ilk kez **Ernst Zermelo (1910)** tarafından satranç oyunu bağlamında formüle edilmiştir [[28:36](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=1716)].
  - Zermelo, sonlu hamleye sahip iki kişilik oyunlarda geriye doğru giderek her iki taraf için de bir *optimal strategy* olduğunu kanıtlamıştır [[28:54](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=1734)].
- **Stratejik (Strategic) vs. Taktiksel (Tactical) Düşünce:**

  - Satranç ustası Wilhelm Steinitz, tüm ağacı (tree) analiz etmek yerine tahtadaki pozisyonel değerleri hesaba katan **Strategic Thinking** kavramını geliştirdi [[33:30](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2010)].
  - Bütün olasılıkları sonuna kadar analiz etmek ise **Tactical Thinking** (Backwards Induction) olarak geçer [[34:31](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2071)].
  - Ekonomi ve Finans teorisinde *Strategy* kavramı elenir ve analiz doğrudan Backward Induction üzerinden yürütülür [[35:00](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2100)].
- **Satranç Algoritmaları (Claude Shannon):**

  - Claude Shannon, satranç ağacının tamamını taramak imkansız olduğu için derinliği sınırlı tutup uç noktalara pozisyonel değer atayan ve geriye doğru hesaplama yapan modern arama algoritmalarının temelini atmıştır [[35:25](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2125)].

### 3. Optimal Stopping Times (Optimal Durdurma Zamanları)

Sözleşmeler, mortgage erken ödemeleri veya tahvil çağırma (call bond) gibi durumlar birer **stopping game** örneğidir [[38:15](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2295)].

#### A. Red and Black Game (Kırmızı ve Siyah Oyunu)

- **Kurallar:**

  - 52 kartlık destede 26 Siyah (+$1) ve 26 Kırmızı (-$1) kart vardır [[37:30](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2250)]. İstediğiniz an oyunu durdurma (*stop*) opsiyonunuz bulunur [[38:01](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2281)].
- **Opsiyon Değeri (Option Value):**

  - Çoğu insan destede kırmızı sayısı arttığında durmayı tercih etse de (riskten kaçınma veya yanlış hesaplama yüzünden) [[46:10](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2770)], opsiyonun varlığı nedeniyle oyuna devam etmek beklenenden çok daha değerlidir [[46:34](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2794)].
  - 26 Siyah ve 26 Kırmızı kart ile başlanan oyunun beklenen opsiyon değeri tam olarak **$2.61**'dir [[56:24](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=3384)].
- **Matematiksel Formül:**

  V(B,R)=max⁡(0, BB+R[1+V(B−1,R)]+RB+R[−1+V(B,R−1)])V(B, R) = \max\left(0, \, \frac{B}{B+R}[1 + V(B-1, R)] + \frac{R}{B+R}[-1 + V(B, R-1)]\right)V(B,R)=max(0,B+RB​[1+V(B−1,R)]+B+RR​[−1+V(B,R−1)])

  - BBB: Kalan siyah kart sayısı, RRR: Kalan kırmızı kart sayısı [[49:06](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=2946)].
  - Kenar değerlerden (sadece kırmızı veya sadece siyah kalınan durumlar) başlayarak backward induction ile tüm düğümler hesaplanır [[51:35](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=3095)].

#### B. Optimal Marriage Problem (Optimal Evlilik / Sekreter Problemi)

- **Kurallar:**

  - Sırayla 1000 aday ile karşılaşıyorsunuz. Her adayın uygunluğu [0,1][0, 1][0,1] aralığında uniform dağılmıştır [[01:07:23](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=4043)].
  - Bir adayı reddedip ilerlediğinizde geriye dönüp onu seçme imkanınız yoktur [[01:08:32](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=4112)].
- **Eşik Değer (Threshold) ve Çözüm:**

  - Zaman azaldıkça (kalan aday sayısı düştükçe) kriterler/eşik değer düşer (*desperation sets in*) [[01:09:49](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=4189)].
  - TTT aday kaldığında uygulanacak optimal eşik değer, T−1T-1T−1 aday kaldığındaki beklenen değere eşittir:

    Threshold(T)=V(T−1)\text{Threshold}(T) = V(T-1)Threshold(T)=V(T−1)
- **Sezgisel Sonuç:**

  - Aday sayısı çok yüksek olduğunda (N→∞N \to \inftyN→∞), sıralı karar vermek zorunda olmanıza rağmen optimal stratejiyle elde edeceğiniz ortalama kalite, tüm adayları görüp seçebileceğiniz **en iyi 2. adayın (second best option)** beklenen kalitesine yaklaşır [[01:13:02](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=4382)], [[01:18:56](https://www.youtube.com/watch?v=IPNl-jD1vhw&t=4736)].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    16. Backward Induction and Optimal Stopping Times

    YaleCourses · 30K views

     [Open in 16. Backward Induction and Optimal Stopping Times](http://www.youtube.com/watch?v=IPNl-jD1vhw)](http://www.youtube.com/watch?v=IPNl-jD1vhw)

    ![](https://i.ytimg.com/vi/IPNl-jD1vhw/hqdefault.jpg)
