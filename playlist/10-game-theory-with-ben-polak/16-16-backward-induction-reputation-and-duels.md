# 16. Backward induction: reputation and duels

<https://www.youtube.com/watch?v=SE7kP7XZuV4>

Dersin (**Yale Econ 159: Game Theory - Lecture 16**) öne çıkan ve detaylı başlıkları aşağıdaki gibidir:

### 1. Giriş ve Geçmiş Konunun Hatırlatılması: Market Entry & Backward Induction

- **Önceki Oyun Matrisi Özeti:**

  - Pazara girmek isteyen bir **Entrant** ve pazarı elinde tutan bir **Incumbent** (Monopolist) vardır.
  - Matris analizinde iki tane **Nash Equilibrium** bulunur: `(In, Not Fight)` ve `(Out, Fight)`.
- **Geriye Doğru Tümevarım (Backward Induction):**

  - Pazara girildikten sonra Incumbent için **Fight** ($0 kazanç) yerine **Not Fight / Accommodate** ($1M kazanç) seçmek rasyoneldir.
  - Bu nedenle Entrant pazara girer (`In`).
  - `(Out, Fight)` dengesindeki "Fight" tehdidi gerçekçi değildir (**Not Credible Threat** / İnandırıcı olmayan tehdit).

### 2. İtibar (Reputation) ve Chain Store Paradox

- **Genişletilmiş Senaryo (10 Pazarlı Monopolist):**

  - Ali adlı monopolistin 10 farklı şehirde (Miami, Madison, Bridgeport vb.) pizzacısı vardır ve rakipler sırayla pazara girmeye çalışır.
- **Sınıfta Yapılan Deney (Simülasyon):**

  - Ali ilk pazara giren rakiple **savaştı (Fight)**.
  - Bunu gören sonraki rakiplerin birçoğu korkarak pazara girmekten vazgeçti (**Stay Out**).
- **Teori ile Pratik Arasındaki Çelişki (Chain Store Paradox):**

  - **İtibar Sezgisi:** İlk başta savaşarak "sert/tavizsiz" bir imaj (**reputation**) çizmek, sonraki rakipleri caydırır.
  - **Backward Induction Çelişkisi:**

    1. 10. (son) pazarda Ali'nin gelecekte koruyacağı başka bir pazar kalmadığı için savaşması mantıksızdır (`Not Fight`).
    2. 10. rakip bunu bildiği için girer.
    3. 9. rakip, 10. rakibin her halükarda gireceğini bildiğinden Ali'nin 9. pazarda da savaşmayacağını anlar ve girer.
    4. Geriye doğru zincirleme olarak oyun çözülür: **Herkes girmeli, Ali kimseyle savaşmamalıdır.**
  - Bu teorik çelişki Reinhard Selten tarafından **Chain Store Paradox** olarak adlandırılmıştır.

### 3. İtibar Modelini Matematiksel Olarak Çözmek: "Deli / Bonkers" Oyuncu

- **Model Değişikliği (Perturbation / Unreasonable Type):**

  - %1 gibi çok küçük bir ihtimalle (ϵ\epsilonϵ kadar bir olasılıkla) Ali'nin "kavga etmeyi seven / çılgın" (**Bonkers / Crazy**) biri olduğu varsayılır.
- **Mekanizma:**

  - Rakip ilk başta Ali'nin mantıklı olduğunu düşünse bile, Ali savaştığında rakip inancını günceller (Bayesian updating). Ali'nin "çılgın" olma ihtimali gözünde büyür ve sonraki rakipler girmekten vazgeçer.
- **Akıllı (Sane) Oyuncunun "Çılgın" Taklidi Yapması:**

  - Rasyonel/akıllı Ali de bu durumu bildiği için, sırf rakipleri korkutup caydırmak adına "çılgın" gibi davranıp savaşır (**Deterrence**).
  - **Püf Nokta:** Gerçek dengede (equilibrium) karma stratejiler (**mixed strategies**) kullanılır.
- **Gerçek Hayattan İtibar Örnekleri:**

  - **Çabuk Öfkelenen İnsanlar / Kardeşler:** Küçük bir tartışmada hemen parlayan kişilerin istediklerini elde etme oranı daha yüksektir (başkaları çekindiği için).
  - **Rehin Pazarlığı (Hostage Negotiations):** "Teröristlerle/reine alanlarla pazarlık edilmez" kuralı, gelecekteki potansiyel eylemleri caydırmak için itibar oluşturma amacı taşır.
  - **Mesleki Güven (Doctors / Accountants):** Dürüstlük itibarı (ör. Arthur Andersen skandalı / Enron).

### 4. Düello Oyunu (Duel Game) ve Zamanlama Problemi

- **Zamanlama (Timing) Stratejisi:**

  - Klasik oyunların aksine ("Ne yapmalıyım?"), bu oyunda soru **"Ne zaman yapmalıyım?"** (When to act) sorusudur.
  - **Gerçek Hayat Örnekleri:**

    - Tour de France'ta gruptan (**peloton**) ne zaman kopup atak yapmalı? (Erken yaparsan yorulursun, geç yaparsan sprinters seni geçer).
    - Yeni bir teknoloji/ürün ne zaman piyasaya sürülmeli? (Erken sürersen ürün bozuk olabilir, geç sürersen pazar kapılır).
- **Düello Oyun Kuralları (Sünger Atma Deneyi):**

  - İki oyuncunun elinde **sadece 1 adet ısıl sünger** vardır.
  - Sırayla hamle yapılır: Ya sünger atılır ya da karşı tarafa doğru 1 adım atılır.
  - Süngeri atıp vurursan kazanırsın. **Isıkar/kaçırırsan** rakip senin dibine kadar yürüyüp süngeri kafana koyarak kazanır.

### 5. Düello Oyununun Matematiksel Analizi

#### Olasılık Tanımı

- Pi(d)P\_i(d)Pi​(d): iii oyuncusunun ddd mesafesinden atış yaptığında vurma olasılığı.
- d=0d = 0d=0 iken P(0)=1P(0) = 1P(0)=1 (Tam dibindeyken vurma olasılığı %100).
- Mesafe arttıkça vurma olasılığı düşer.

#### Temel Kurallar (Fact A & Fact B)

1. **Fact A:** Eğer henüz kimse sünger atmadıysa ve iii oyuncusu, rakibi jjj'nin yarın (d−1d-1d−1 mesafesinde) **atış yapmayacağını** biliyorsa; bugün atış yapmamalı, adım atmalıdır (daha yakından atış yapmak için).
2. **Fact B:** Eğer iii oyuncusu, rakibi jjj'nin yarın (d−1d-1d−1 mesafesinde) **atış yapacağını** biliyorsa; bugün atış yapmalıdır.

   - **Koşul:** iii'nin bugün vurma olasılığı, jjj'nin yarın kaçırma olasılığından büyük olmalıdır (Pi(d)≥1−Pj(d−1)P\_i(d) \ge 1 - P\_j(d-1)Pi​(d)≥1−Pj​(d−1)).
   - Düzenlersek: **Pi(d)+Pj(d−1)≥1P\_i(d) + P\_j(d-1) \ge 1Pi​(d)+Pj​(d−1)≥1** (Buna **Star Inequality** denir).

#### Kritik Kritik Mesafe (d∗d^\*d∗) ve Çözüm

- **Dominance (Baskın Strateji) Analizi:** Çok uzak mesafelerde Pi(d)+Pj(d−1)<1P\_i(d) + P\_j(d-1) < 1Pi​(d)+Pj​(d−1)<1 olduğu için rakibin ne yapacağından bağımsız olarak kimse atış yapmaz, sadece yaklaşır.
- **Geriye Doğru Tümevarım (Backward Induction) ile Çözüm:**

  - d=0d = 0d=0'da sırası gelen kesinlikle atar (Olasılık = 1).
  - d=1d = 1d=1'de sırası gelen, rakibinin d=0d=0d=0'da atacağını bildiği için kendisi atar (P1(1)+P2(0)>1P\_1(1) + P\_2(0) > 1P1​(1)+P2​(0)>1).
  - Bu mantık geriye doğru d∗d^\*d∗ noktasına kadar devam eder.
- **Sonuç:** Pi(d)+Pj(d−1)≥1P\_i(d) + P\_j(d-1) \ge 1Pi​(d)+Pj​(d−1)≥1 eşitsizliğini sağlayan **ilk mesafe olan d∗d^\*d∗ anında, sırası gelen ilk oyuncu süngerini atmalıdır.**

### 6. Psikolojik/Davranışsal Boyut ve Dersin Özet Sonuçları

- **Proactive Bias (Aşırı Aktif Olma Eğilimi):**

  - Sınıfta oyuncular genelde d∗d^\*d∗ noktasından çok daha önce ateş edip ıskalamışlardır.
  - Bunun sebebi insanların kendi yeteneklerine aşırı güvenmesi (**overconfidence**) ve "en azından denerken kaybettim" anlayışına sahip olmasıdır.
- Baskın Strateji (DominYouTube URL'lerine veya video içeriklerine doğrudan erişim (videoyu izleme veya altyazılarını çekme) yeteneğim bulunmuyor.

Ancak listelemeyi yapabilmem için bana yardımcı olabilecek **iki hızlı yoldan birini** kullanabiliriz:

1. **Videonun konusunu / başlığını ve konuşmacısını** paylaşabilirsin (Böylece konuyu ve önemli noktalarını detaylıca özetleyebilirim).
2. **Videonun altyazı metnini (transcript)** veya özetlemek istediğin metin parçalarını buraya yapıştırabilirsin.

Hangisi senin için uygunsa o şekilde ilerleyelim!

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

16. Backward induction: reputation and duels

YaleCourses · 36K views

 [Open in 16. Backward induction: reputation and duels](http://www.youtube.com/watch?v=SE7kP7XZuV4)](http://www.youtube.com/watch?v=SE7kP7XZuV4)

![](https://i.ytimg.com/vi/SE7kP7XZuV4/hqdefault.jpg)
