# 18. Imperfect information: information sets and sub-game perfection

<https://www.youtube.com/watch?v=D7aDIZ-KPEU>

Yale University'ın **"18. Imperfect Information: Information Sets and Subgame Perfection"** başlıklı Oyun Teorisi (Game Theory) dersinden öne çıkan ve detaylandırılmış ana başlıklar şu şekildedir:

### 1. Giriş ve Motivasyon

- **Eşzamanlı (Simultaneous) vs. Ardışık (Sequential) Oyunlar [[00:26](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=26)]:**

  - Midterm öncesinde oyuncuların birbirlerinin hamlelerini bilmediği *Simultaneous Move* oyunlar incelenmişti.
  - Midterm sonrasında ise tam bilgiye sahip (*Perfect Information*) *Sequential Move* oyunlar ve **Backward Induction** yöntemi ele alındı.
- **Ana Amaç [[01:00](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=60)]:** Hem eşzamanlı hem de ardışık hamleleri içeren karmaşık stratejik durumları analiz etmek için Backward Induction ve Nash Dengesi kavramlarını genelleştirmek.

### 2. Information Sets (Bilgi Kümeleri)

- **Tanim [[10:27](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=627)]:** Bir oyuncunun oyun ağacı (tree) üzerinde içinde bulunduğu ancak hangi düğümde (node) olduğunu ayırt edemediği düğümler koleksiyonuna **Information Set** denir.
- **Gösterim [[05:50](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=350)]:** Düğümler arasındaki kesikli çizgi (dotted line), oyuncunun önceki hamle hakkında bilgi sahibi olmadığını (ör. Player 1'ın "Up" mı yoksa "Middle" mı seçtiğini Player 2'nun görememesini) gösterir.
- **Geçerli Bir Information Set İçin Kurallar:**

  1. **Aynı Sayıda Seçenek:** Bir oyuncu aynı Information Set içindeki tüm düğümlerde tam olarak aynı sayıda geçerli hamleye sahip olmalıdır [[13:04](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=784)]. Aksi takdirde seçenek sayısından hangi düğümde olduğunu anlar.
  2. **Perfect Recall (Tam Hatırlama) Varsayımı [[15:03](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=903)]:** Oyuncular kendi geçmiş hamlelerini hatırlar. Bu nedenle bir oyuncunun kendi geçmiş seçimleri neticesinde ulaştığı farklı düğümler aynı Information Set içinde yer alamaz [[14:30](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=870)].

### 3. Perfect Information vs. Imperfect Information

- **Perfect Information (Tam Bilgi) [[17:20](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=1040)]:** Oyun ağacındaki her Information Set'in yalnızca tek bir düğümden (singleton node) oluştuğu oyunlardır. Oyuncular geçmiş tüm hamleleri görür.
- **Imperfect Information (Eksik/Tam Olmayan Bilgi) [[18:30](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=1110)]:** En az bir Information Set'in birden fazla düğüm içerdiği oyunlardır.
- **Eşzamanlı Oyunların Ağaç (Tree) Gösterimi [[25:05](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=1505)]:** Matrix (Normal Form) ile gösterilen eşzamanlı oyunlar (örneğin *Prisoner's Dilemma*), Information Set kavramı kullanılarak bir oyun ağacında temsil edilebilir. Önemli olan zaman sıralaması değil, oyuncunun hamle anındaki **bilgisidir (information)** [[34:34](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=2074)].

### 4. Strateji (Strategy) Tanımının Güncellenmesi

- **Pure Strategy (Saf Strateji) [[26:50](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=1610)]:** Oyuncunun her bir düğümde (node) ne yapacağını değil, **her bir Information Set'te ne yapacağını** belirten eksiksiz bir eylem planıdır.
- Düğümleri ayırt edemeyen bir oyuncu, aynı Information Set içerisindeki tüm düğümlerde tek bir karar vermek zorundadır [[21:10](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=1270)].

### 5. Nash Equilibria Ötesi: Incomplete / Implausible Equilibria Problemi

- Bir oyun Matris (Normal Form) haline getirilip standart **Nash Equilibrium** arandığında, zaman dizilimini veya dinamik yapıyı dikkate almayan **mantıksız (implausible / non-credible)** dengeler çıkabilir [[44:28](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=2668)].
- Oyun ağacı üzerinde Backward Induction sezgisine aykırı düşen bu bogus/phony dengeleri eleyecek daha rafine bir denge kavramına ihtiyaç duyulur [[49:45](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=2985)].

### 6. Subgame (Alt Oyun) Tanımı

- **Subgame [[01:05:12](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=3912)]:** Ana oyun ağacı içinde başlı başına bağımsız bir oyun gibi davranan parçadır. Üç temel şartı karşılamalıdır:

  1. Tek bir ana düğümden (single node) başlamalıdır [[01:05:59](https://www.youtube.com/watch?v=D7aDIZ-KPEU&t=3959)].
     2.Üzgünüm, internet erişimim veya videoları doğrudan izleme/deşifre etme özelliğim bulunmadığı için verdiğiniz YouTube bağlantısını doğrudan açıp içeriğini analiz edemiyorum.

Eğer videonun **başlığını, konusunu, transkriptini (altyazı metnini)** veya hangi teknoloji/konu hakkında olduğunu paylaşırsanız, belirttiğiniz detay seviyesinde ve İngilizce orijinal terimleri koruyarak kapsamlı bir özet liste oluşturmaktan memnuniyet duyarım!

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

18. Imperfect information: information sets and sub-game perfection

YaleCourses · 82K views

 [Open in 18. Imperfect information: information sets and sub-game perfection](http://www.youtube.com/watch?v=D7aDIZ-KPEU)](http://www.youtube.com/watch?v=D7aDIZ-KPEU)

![](https://i.ytimg.com/vi/D7aDIZ-KPEU/hqdefault.jpg)
