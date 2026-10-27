# 11. Evolutionary stability: cooperation, mutation, and equilibrium

<https://www.youtube.com/watch?v=er9KvYn4ldk>

Bu video, Prof. Ben Polak tarafından Yale Üniversitesi'nde verilen **Oyun Teorisi (Game Theory)** dersinin *"11. Evolutionary stability: cooperation, mutation, and equilibrium"* başlıklı bölümüdür. Video, Oyun Teorisi ile Evrimsel Biyoloji arasındaki ilişkiyi ve **Evrimsel Olarak Kararlı Strateji (Evolutionary Stable Strategy - ESS)** kavramını incelemektedir.

Videoda öne çıkan tüm önemli noktalar ve detaylar aşağıda listelenmiştir:

### 1. Oyun Teorisi ve Evrim İlişkisi (Giriş ve Motivasyon)

- **Biyolojide Oyun Teorisi Kullanımı:**

  - Biyolojide (özellikle hayvan davranışlarında) stratejiler **genler (veya fenotipler)** ile, kazanımlar (payoffs) ise **genetik uyum başarısı (genetic fitness)** ile ilişkilendirilir.
  - Başarılı stratejilere sahip genler popülasyonda çoğalır, başarısız olanlar yok olur.
- **Klasik Oyun Teorisi ile Temel Fark:**

  - Klasik oyun teorisinde rasyonel bireyler stratejilerini *düşünerek/seçerek* belirler.
  - Evrimsel oyun teorisinde stratejiler **hardwired (sabitleşmiş/genetik olarak kodlanmış)** kabul edilir. Hayvanlar mantık yürütmez, genlerinin getirdiği davranışı uygular.
- **Sosyal Bilimlere Yansımaları:**

  - Evrim kavramı iktisat ve sosyolojide bir metafor olarak kullanılır.
  - Örneğin iktisatta firmalar rasyonel kararlar almasalar bile piyasadaki rekabet ortama uyum sağlayan (düşük maliyetli, yüksek kârlı) firmaları hayatta tutar; iflas eden firmalar genlerin yok olması gibidir.

### 2. Modeli Basitleştiren Temel Varsayımlar

- **Within-species competition:** Rekabet tür içi gerçekleşir (aslanlar aslanlarla, karıncalar karıncalarla).
- **Symmetric 2-player games:** İki oyunculu, simetrik oyunlar kullanılır (her iki oyuncu aynı strateji setine ve kazanım matrisine sahiptir).
- **Random matching:** Geniş bir popülasyondan rastgele iki birey eşleşir, hardwired oldukları stratejiyi oynar ve ortalama kazanımlar (average payoffs) hesaplanır.
- **Asexual reproduction (Eşeysiz Üreme):** Stratejik mantığı basit tutmak adına gen yeniden dağılımı (gene redistribution) olmadığı, yani tek ebeveynli üreme olduğu varsayılır.

### 3. Evrimsel Kararlılık (Evolutionary Stability) Mantığı

- Popülasyonun büyük çoğunluğu bir sss (incumbent/yerleşik) stratejisini oynarken küçük bir grup mutasyon geçirerek S′S'S′ (mutant) stratejisini oynamaya başlar.
- Eğer her türlü küçük mutasyon grubu (S′S'S′) rastgele eşleşmeler sonucunda zamanla yok oluyorsa, ana strateji sss **Evolutionarily Stable (ES / Evrimsel Olarak Kararlı)** kabul edilir.
- Mutasyon ilk başladığında oranı çok küçük (ϵ\epsilonϵ) olduğu için mutantlar genellikle ana popülasyon (sss) ile karşılaşır; iki mutantın birbiriyle karşılaşması oldukça nadirdir.

### 4. Örnekler Üzerinden Analiz

#### A. Prisoner's Dilemma (Mahkum İkilemi)

- Stratejiler: Cooperate (CCC) ve Defect (DDD).
- **İşbirliği (CCC) Evrimsel Kararlı mıdır?**

  - Popülasyon CCC oynarken küçük bir grup DDD (mutant) ortaya çıkarsa; DDD mutantları CCC oynayanlarla karşılaştığında daha yüksek kazanım elde eder.
  - Mutantlar çoğalır ve CCC popülasyonunu işgal eder. Dolayısıyla **CCC (Cooperate) Evrimsel Kararlı değildir.**
- **Bozgunculuk/İhanet (DDD) Evrimsel Kararlı mıdır?**

  - Popülasyon DDD oynarken CCC mutantı (ETETET örneği) girdiğinde, CCC mutantları sürekli DDD ile karşılaşarak 0 kazanım alır ve elenir.
  - Dolayısıyla **DDD (Defect) Evrimsel Kararlı bir stratejidir.**
- **Doğa ve Verimlilik Yorumu ("Nature can suck"):**

  - Doğadaki evrimsel süreçler her zaman ahlaki veya toplumsal olarak en verimli (efficient) sonucu doğurmaz. DDD stajatejisinin kalıcı olması toplumsal toplam kazanımı düşürür.
  - Gerçek doğada işbirliğinin (cooperation) görülme nedeni ise eşeyli üreme (sexual reproduction) ve genlerin akrabalar üzerindeki korunumu (kin selection) ile açıklanır.

#### B. Strictly Dominated Stratejiler

- **Ders:** Strictly dominated (kesin domine edilen) bir strateji **asla evrimsel olarak kararlı olamaz**.
- Çünkü onu domine eden strateji bir mutasyon olarak ortaya çıktığında popülasyonu kolayca işgal eder.

#### C. 3x3 Oyun Örneği ve Invader Stratejiler

- Bir stratejinin evrimsel olarak kararlı olmaması için onu işgal eden mutantın (S′S'S′) kendisinin kararlı olması gerekmez.
- Örnekte CCC stratejisini işgal eden BBB mutantı da kararlı değildir (onu da tekrar CCC işgal edebilir); ancak BBB'nin varlığı CCC'nin kararlılığını bozmaya yeterlidir.

### 5. Nash Dengesi ve Evrimsel Kararlılık İlişkisi

- **Nash Dengesi Bağlantısı:**

  - Eğer bir sss stratejisi **Nash Equilibrium değilse**, o strateji **Evrimsel Olarak Kararlı da DEĞİLDİR**.
  - Bunun mantığı: Nash Dengesi olmaması, başka bir stratejinin sapma (deviation) yaparak daha yüksek kazanım elde edebileceği anlamına gelir. Bu kârlı sapma stratejisi, popülasyonu işgal eden başarılı bir mutasyondur.
  - *Ters Mantık:* Eğer sss Evrimsel Olarak Kararlı ise, (s,s)(s, s)(s,s) çifti mutlaka bir **Nash Equilibrium** olmalıdır.
- **Nash Dengesi Olup Evrimsel Kararlı Olmayan Durumlar:**

  - Her Nash dengesi evrimsel olarak kararlı değildir.
  - Özellikle **Weak Best Response (Zayıf En İyi Tepki)** içeren Nash dengeleri evrimsel kararlılık göstermeyebilir. Mutantlar yerleşik popülasyona karşı aynı kazanımı elde etse bile, kendi aralarındaki nadir karşılaşmalarda daha yüksek kazanım alırlarsa popülasyonda büyüyebilirler.
- **Strict Nash Dengesinin Gücü:**

  - Eğer (s,s)(s, s)(s,s) bir **Strict Nash Equilibrium** ise (yani sss, sss'ye karşı *kesin* en iyi tepkiyse), sss kesinlikle **Evrimsel Olarak Kararlıdır**.

### 6. Evrimsel Kararlılığın Matematiksel Tanımları

#### Definition 1: Biyoloji Tanımı (Maynard Smith, 1972)

Bir s∗s^\*s∗ (s-hat) pure stratejisinin evrimsel olarak kararlı olması için, yeterince küçük tüm mutasyon oranları (ϵ<ϵˉ\epsilon < \bar{\epsilon}ϵ<ϵˉ) ve tüm farklı S′S'S′ mutasyonları için şu eşitsizlik sağlanmalıdır:

(1−ϵ)⋅U(s∗,s∗)+ϵ⋅U(s∗,S′)>(1−ϵ)⋅U(S′,s∗)+ϵ⋅U(S′,S′)(1-\epsilon) \cdot U(s^\*, s^\*) + \epsilon \cdot U(s^\*, S') > (1-\epsilon) \cdot U(S', s^\*) + \epsilon \cdot U(S', S')(1−ϵ)⋅U(s∗,s∗)+ϵ⋅U(s∗,S′)>(1−ϵ)⋅U(S′,s∗)+ϵ⋅U(S′,S′)

*(Sol taraf: Yerleşik popülasyonun mutant içeren gruptaki ortalama kazanımı; Sağ taraf: Mutantın ortalama kazanımı)*

#### Definition 2: Oyun Teorisi / İktisat Tanımı (Eşdeğer Tanım)

s∗s^\*s∗ stratejisi şu iki koşulu sağlıyorsa **ES (Evrimsel Kararlı)** olur:

1. **(s∗,s∗)(s^\*, s^\*)(s∗,s∗) bir Nash Dengesi olmalıdır:**

   U(s∗,s∗)≥U(S′,s∗)∀S′U(s^\*, s^\*) \ge U(S', s^\*) \quad \forall S'U(s∗,s∗)≥U(S′,s∗)∀S′
2. **Eğer S′S'S′ stratejisi zayıf bir sapma ise (yani eşitlik durumu U(s∗,s∗)=U(S′,s∗)U(s^\*, s^\*) = U(S', s^\*)U(s∗,s∗)=U(S′,s∗) varsa):**

   Yerleşik stratejinin mutanta vereceği tepki, mutantın kendisine vereceği tepkiden strictly daha büyük olmalıdır:

   U(s∗,S′)>U(S′,S′)U(s^\*, S') > U(S', S')U(s∗,S′)>U(S′,S′)

### 7. İki Tanımın Eşdeğerliği ve Önemi

- **Biyoloji ve İktisadın Kesişimi:** 19. yüzyılda Darwin'in biyolojide geliştirdiği evrim fikMaalesef doğrudan internete erişip YouTube linklerinin içeriğini veya transkriptlerini anlık olarak çekme yeteneğim bulunmuyor.

Ancak videonun **konusunu, başlığını veya anlatılan temel başlıkları** (örneğin: *yazılım mimarisi, belirli bir kütüphane, yapay zekâ modeli veya sunum konusu*) kısaca belirtirseniz ya da video metnini/transkriptini buraya yapıştırırsanız, istediğiniz detay seviyesinde ve İngilizce orijinal terimleri koruyarak maddeler halinde kapsamlı bir özet çıkarabilirim.

Videonun genel olarak ne hakkında olduğunu paylaşabilir misiniz?

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

11. Evolutionary stability: cooperation, mutation, and equilibrium

YaleCourses · 63K views

 [Open in 11. Evolutionary stability: cooperation, mutation, and equilibrium](http://www.youtube.com/watch?v=er9KvYn4ldk)](http://www.youtube.com/watch?v=er9KvYn4ldk)

![](https://i.ytimg.com/vi/er9KvYn4ldk/hqdefault.jpg)
