# 15. Backward induction: chess, strategies, and credible threats

<https://www.youtube.com/watch?v=Bm8lM73lTmk>

Bu video, Prof. Ben Polak tarafından Yale Üniversitesi'nde verilen "GAME 211: Game Theory" dersinin 15. bölümüdür ("Backward induction: chess, strategies, and credible threats").

Videonun öne çıkan ana başlıkları ve önemli noktaları şunlardır:

### 1. Zermelo's Theorem (Zermelo Teoremi) [[01:34](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=94)]

Dersin başında geçen haftaki *Game of Nim* örneğinden yola çıkılarak **Zermelo Teoremi** ele alınıyor.

- **Koşullar:**

  - 2 oyunculu [[02:08](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=128)]
  - **Perfect Information** (tam bilgiye sahip: her oyuncu hamle yaparken geçmişte ne olduğunu tam olarak bilir) [[02:14](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=134)]
  - **Finite number of nodes** (sonlu sayıda hamle/düğüm, oyun sonsuza uzayamaz) [[02:43](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=163)]
  - **Sonuçlar:** Kazanma (W1W\_1W1​), Kaybetme (L1L\_1L1​ / W2W\_2W2​) veya Beraberlik (Tie) [[03:05](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=185)].
- **Teoremin İddiası:** Bu şartları sağlayan her oyunda şu 3 durumdan **biri kesinlikle doğrudur** [[03:46](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=226)]:

  1. 1. oyuncu (Player 1) ne olursa olsun **galibiyeti zorlayabilir** (*force a win*).
  2. 1. oyuncu en azından **beraberliği zorlayabilir** (*force a tie*).
  3. 2. oyuncu 1. oyuncuya **mağlubiyeti zorlayabilir** (*force a loss for Player 1 / win for Player 2*).
- **Uygulama Örnekleri:**

  - **Tic-Tac-Toe:** İki taraf da doğru oynarsa oyun her zaman beraberlikle biter [[07:54](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=474)].
  - **Checkers (Dama) & Chess (Satranç):** Satranç sonlu ve tam bilgili bir oyun olduğu için teorik olarak tam bir çözümü vardır [[09:33](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=573)]. Ancak teorem çözümün ne olduğunu (*how to play*) söylemez, sadece bir çözümün **var olduğunu** kanıtlar [[10:03](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=603)].

### 2. Induction ile Kanıt (Proof by Induction) [[10:58](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=658)]

Zermelo Teoremi'nin kanıtı, oyunun maksimum uzunluğu (nnn) üzerinden **matematiksel tümevarım (induction)** ile gösteriliyor:

- **Base Step (n=1n = 1n=1):** Tek hamlelik oyunlarda Player 1 önündeki dallara bakarak kendisi için en iyi sonucu (W1>Tie>L1W\_1 > \text{Tie} > L\_1W1​>Tie>L1​) seçer, sonuç çok açıktır [[13:09](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=789)].
- **Inductive Step (n→n+1n \to n+1n→n+1):** nnn veya daha kısa uzunluktaki tüm oyunların/alt oyunların (subgames) bir çözümü olduğu varsayılır [[17:12](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=1032)].

  - n+1n+1n+1 uzunluğundaki bir oyun, Player 1'in ilk hamlesinin ardından gelen nnn veya daha kısa uzunluktaki **Subgame**'lerden oluşur [[20:26](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=1226)].
  - Alt oyunlar kendi içlerinde çözülebildiği için Player 1 başlangıçta kendisine en iyi sonucu veren alt oyuna yönelir. Böylece n+1n+1n+1 uzunluğundaki oyun da çözülmüş olur [[28:01](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=1681)].

### 3. Sınıf İçi Deney: Array of Rocks (Chomp Oyunu) [[32:14](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=1934)]

Öğrencilerle tahtada taş matrisi (satır ve sütunlar) üzerinden bir oyun oynanıyor.

- **Kurallar:** Bir taş seçildiğinde, o taş ve onun **Kuzeydoğusundaki (üstünde ve sağında kalan) tüm taşlar** silinir [[33:18](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=1998)]. Son taşı alan oyunu kaybeder [[34:00](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2040)].
- **Çıkarım:** Zermelo Teoremi'ne göre bu oyunun da matris boyutlarına (n×mn \times mn×m) bağlı kesin bir çözümü vardır [[38:59](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2339)].

### 4. Formal Tanımlar: Perfect Information & Pure Strategy [[41:47](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2507)]

- **Game of Perfect Information:** Oyundaki her karar düğümünde (node), hamle sırası gelen oyuncu tam olarak hangi düğümde olduğunu ve oraya **nasıl ulaştığını (oyunun tüm geçmişini)** bilir [[42:08](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2528)].
- **Pure Strategy (Saf Strateji):** Bir oyuncunun karar vermesi gereken **tüm olası düğümlerde (node)** ne yapacağını eksiksiz belirten tam bir eylem planıdır (*complete plan of action*) [[44:39](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2679)].

  - *Önemli Detay:* Bir düğüm oyun esnasında hiç ziyaret edilmeyecek/ulaşılmayacak olsa bile, strateji tanımı gereği o düğümde ne yapılacağını belirtmek zorundadır (*Redundancy*) [[51:33](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3093)].

### 5. Backward Induction vs. Nash Equilibrium [[47:02](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=2822)]

Ağaç yapısındaki sıralı bir oyun matriks formatına (4x2) çevrilerek inceleniyor [[55:40](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3340)]:

- **Farklılık:** Oyunda 2 adet Nash Dengesi (Nash Equilibrium) bulunuyor [[58:27](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3507)]:

  1. Backward Induction sonucu çıkan mantıklı denge [[58:58](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3538)].
  2. Ulaşılmayan düğümlerde rasyonel olmayan (saçma) kararlara dayanan ikinci bir Nash Dengesi [[59:16](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3556)].
- **Sorun:** Nash Dengesi tek başına, oyuncuların hiç ulaşılmayan durumlardaki Mantıksız/Aptalca eylemlerini filtreleyemez [[01:01:02](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3662)].

### 6. Ekonomik Örnek: Entry Deterrence & Non-Credible Threats [[01:01:39](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3699)]

Konsepti somutlaştırmak için bir piyasaya giriş modeli inceleniyor:

- **Oyuncular & Senaryo:**

  - Piyasada var olan bir **Incumbent** (Tekel/Yerleşik Firma) ve pazara girmeyi düşünen bir **Entrant** (Yeni Girişimci) var [[01:02:18](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3738)].
  - Entrant: `In` (Gir) veya `Out` (Uzak Dur) seçebilir.
  - Entrant girerse, Incumbent: `Fight` (Savaş/Fiyat Kırma) veya `Not Fight` (Uyum Sağlama/Paylaşma) seçebilir.
- **Matriks Analizi ve Denge Durumları:**

  - **1. Denge:** (`In`, `Not Fight`) →\to→ Backward Induction ile bulunan makul denge [[01:06:33](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3993)].
  - **2. Denge:** (`Out`, `Fight`) →\to→ Incumbent "Eğer girersen fiyatları sıfırlar seni batırırım" der, Entrant da girmekten vazgeçer [[01:05:47](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=3947)].
- **Credible Threat (Incredible Threat) Kavramı:**

  - Incumbent'ın "Savaşırım" tehdidi **Credible Threat (İnandırıcı Tehdit) değildir** [[01:08:37](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=4117)].
  - Çünkü Entrant pazara gerçekten girdiğinde, Incumbent için `Fight` demek (kazanç: 0) `Not Fight` demekten (kazanç: 1M) daha kötüdür [[01:08:30](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=4110)].
  - Dolayısıyla pazara giriş gerçekleştiğinde tekelci firma savaşmayacaktır; savurduğu tehdit **Incredible Threat** (İnandırıcı Olmayan Tehdit) olarak kalır [[01:08:47](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=4127)].
- **Dersin Sonu ve Gelecek Hafta Sorusu:** Piyasada Bill Gates / Microsoft gibi oyuncuların bu tehditlerinin neden yine de ciddiye alındığı sorgulanıyor [[01:07:15](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=4035)]. Sınıftan gelen yanıt: Tekelci firma, arkadan gelecek diğer potansiyel rakiplere **ibret olsun (make an example)** diye ilk gireni cezalandırmak isteyebilir [[01:11:44](https://www.youtube.com/watch?v=Bm8lM73lTmk&t=4304)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  15. Backward induction: chess, strategies, and credible threats

  YaleCourses · 59K views

   [Open in 15. Backward induction: chess, strategies, and credible threats](http://www.youtube.com/watch?v=Bm8lM73lTmk)](http://www.youtube.com/watch?v=Bm8lM73lTmk)

  ![](https://i.ytimg.com/vi/Bm8lM73lTmk/hqdefault.jpg)
