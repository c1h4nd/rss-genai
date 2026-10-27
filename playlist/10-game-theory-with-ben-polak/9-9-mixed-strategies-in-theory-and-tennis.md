# 9. Mixed strategies in theory and tennis

<https://www.youtube.com/watch?v=unvJofv0wl8>

Yale Üniversitesi'nin Game Theory (Oyun Teorisi) dersinden alınan bu videoda (**"9. Mixed strategies in theory and tennis"**), **Karma Stratejiler (Mixed Strategies)**, **Karma Strateji Nash Dengesi (Mixed Strategy Nash Equilibrium)** ve bunun tenisteki bir vuruş/savunma senaryosuna uygulaması anlatılmaktadır.

Videodaki önemli ve öne çıkan noktalar detaylı olarak aşağıda sıralanmıştır:

### 1. Mixed Strategy (Karma Strateji) Tanımı ve Notasyonu [[00:17](https://www.youtube.com/watch?v=unvJofv0wl8&t=17)]

- **Tanım:** Karma strateji (PiP\_iPi​), bir oyuncunun kendi *pure strategy*’leri (saf stratejileri) üzerindeki olasılık dağılımıdır (randomization).
- **Olasılık Değerleri (Pi(Si)P\_i(S\_i)Pi​(Si​)):**

  - Bir stratejiye verilen olasılık 000 olabilir [[02:04](https://www.youtube.com/watch?v=unvJofv0wl8&t=124)]. Yani karma strateji oynamak tüm saf stratejileri dahil etmeyi gerektirmez (örn. Taş-Kağıt-Makas'ta (12,12,0)(\frac{1}{2}, \frac{1}{2}, 0)(21​,21​,0)).
  - Bir saf stratejiye 111 olasılık veriliyorsa (Pi(Si)=1P\_i(S\_i) = 1Pi​(Si​)=1), bu durum **Pure Strategy**'nin özel bir halidir [[03:05](https://www.youtube.com/watch?v=unvJofv0wl8&t=185)]. Dolayısıyla pure strategy'ler, mixed strategy kumesinin içinde yer alır.

### 2. Expected Payoff (Beklenen Getiri) Hesaplaması [[04:45](https://www.youtube.com/watch?v=unvJofv0wl8&t=285)]

- Karma stratejinin **Expected Payoff**'u, o karışımda yer alan (pozitif olasılık atanan) pure strategy'lerin beklenen getirilerinin **ağırlıklı ortalamasıdır (weighted average)** [[05:16](https://www.youtube.com/watch?v=unvJofv0wl8&t=316)].
- **Ağırlıklı Ortalama İlkesi:** Bir karma stratejinin beklenen getirisi, dahil edilen en yüksek ve en düşük pure strategy getirileri arasında yer alır [[13:16](https://www.youtube.com/watch?v=unvJofv0wl8&t=796)].

### 3. Temel Ders ve Çıkarım (Lesson & Key Conclusion) [[15:49](https://www.youtube.com/watch?v=unvJofv0wl8&t=949)]

- **Ana İlke:** Eğer bir *mixed strategy* bir **Best Response (En İyi Yanıt)** ise, bu karma strateji içinde pozitif olasılık verilen **her bir pure strategy de kendi başına bir Best Response olmak zorundadır** [[16:20](https://www.youtube.com/watch?v=unvJofv0wl8&t=980)].
- **Eşit Getiri Kuralı:** Dolayısıyla, karma stratejide kullanılan tüm pure strategy'ler **aynı expected payoff**'u vermek zorundadır [[17:05](https://www.youtube.com/watch?v=unvJofv0wl8&t=1025)]. (Biri daha düşük getiri verseydi, onu karışımdan çıkararak ortalama getiri artırılabilirdi).

### 4. Tenis Örneği: Venus ve Serena Williams (2x2 Matrix Game) [[27:38](https://www.youtube.com/watch?v=unvJofv0wl8&t=1658)]

- **Senaryo:** Serena filede, Venus ise pas geçiş vuruşu (passing shot) yapacak.

  - **Venus (Row Player):** LLL (Serena'nın soluna/backhand tarafına pas vuruşu) veya RRR (Serena'nın sağına/forehand tarafına pas vuruşu).
  - **Serena (Column Player):** LLL (kendi soluna/backhand tarafına yatkın durma) veya RRR (kendi sağına/forehand tarafına yatkın durma).
- **Pure Strategy Nash Equilibrium Yokluğu [[35:44](https://www.youtube.com/watch?v=unvJofv0wl8&t=2144)]:**

  - Tarafların best response'ları örtüşmez; sürekli bir döngü oluşur (Serena doğru yönü tahmin ederse sayı kazanma şansı artar, Venus ise Serena'nın olmadığı tarafa vurmak ister).
  - Pure strategy seviyesinde denge olmadığı için çözüm **Mixed Strategy Nash Equilibrium**'dadır [[37:52](https://www.youtube.com/watch?v=unvJofv0wl8&t=2272)].

### 5. Mixed Strategy Nash Equilibrium Bulma Yöntemi (The Trick) [[40:51](https://www.youtube.com/watch?v=unvJofv0wl8&t=2451)]

Bir oyuncunun dengedeki karma stratejisini bulmak için **karşı tarafın payoff'ları** eşitlenir:

- **Serena’nın Karışımını (Q,1−QQ, 1-QQ,1−Q) Bulmak [[41:04](https://www.youtube.com/watch?v=unvJofv0wl8&t=2464)]:**

  - Venus dengede karma strateji oynuyorsa, Venus'ün LLL ve RRR vuruşlarından elde ettiği *expected payoff*'lar eşit olmalıdır [[45:20](https://www.youtube.com/watch?v=unvJofv0wl8&t=2720)].
  - E[PayoffVenus(L)]=E[PayoffVenus(R)]E[Payoff\_{Venus}(L)] = E[Payoff\_{Venus}(R)]E[PayoffVenus​(L)]=E[PayoffVenus​(R)] yazılarak Serena'nın karıştırma olasılığı Q=0.6Q = 0.6Q=0.6 (LLL) ve 0.40.40.4 (RRR) olarak bulunur [[46:58](https://www.youtube.com/watch?v=unvJofv0wl8&t=2818)].
- **Venus’ün Karışımını (P,1−PP, 1-PP,1−P) Bulmak [[48:50](https://www.youtube.com/watch?v=unvJofv0wl8&t=2930)]:**

  - Serena dengede karıştırıyorsa, Serena'nın LLL ve RRR pozisyonlarından alacağı *expected payoff*'lar eşit olmalıdır.
  - E[PayoffSerena(L)]=E[PayoffSerena(R)]E[Payoff\_{Serena}(L)] = E[Payoff\_{Serena}(R)]E[PayoffSerena​(L)]=E[PayoffSerena​(R)] eşitliği çözülerek Venus'ün karıştırma olasılığı P=0.7P = 0.7P=0.7 (LLL) ve 0.30.30.3 (RRR) olarak bulunur [[51:54](https://www.youtube.com/watch?v=unvJofv0wl8&t=3114)].

### 6. Karşılaştırılmalı Statik Analiz (Comparative Statics) & Sezgisel Sonuçlar [[56:04](https://www.youtube.com/watch?v=unvJofv0wl8&t=3364)]

Dersin en önemli taktiksel çıkarımı bu bölümde gösterilir:

- **Senaryo Değişimi:** Serena'nın backhand vole vuruşunu geliştirdiği kabul edilir (Serena'nın LLL pozisyonunda doğru tahmin yaptığı durumdaki sayı kazanma oranı artar) [[56:58](https://www.youtube.com/watch?v=unvJofv0wl8&t=3418)].
- **Çatışan İki Etki [[58:16](https://www.youtube.com/watch?v=unvJofv0wl8&t=3496)]:**

  1. **Direct Effect (Doğrudan Etki):** Serena backhand vuruşunda daha iyi olduğu için sol tarafa daha fazla yatkın durmalıdır (QQQ artmalı).
  2. **Indirect / Strategic Effect (Stratejik Etki):** Venus, Serena'nın backhand'inin güçlendiğini bildiği için onun soluna (LLL) daha az vuracaktır. Bu yüzden top o tarafa daha az geleceğinden, Serena sol tarafa daha az yatkın durmalıdır (QQQ düşmeli).
- **Sonuç (Strategic Effect Dominance) [[01:05:03](https://www.youtube.com/watch?v=unvJofv0wl8&t=3903)]:**

  - Matematiksel hesaplama yapıldığında **Strategic Effect** daha baskın çıkar ve Serena'nın sol tarafı koruma olasılığı Q=0.6Q = 0.6Q=0.6'dan Q=0.5Q = 0.5Q=0.5'e **düşer** [[01:05:37](https://www.youtube.com/watch?v=unvJofv0wl8&t=3937)].
  - Venus'ün Serena'nın soluna atış yapma olasılığı ise P=0.7P = 0.7P=0.7'den P=712≈0.58P = \frac{7}{12} \approx 0.58P=127​≈0.58'e **düşer** [[01:09:25](https://www.youtube.com/watch?v=unvJofv0wl8&t=4165)].
  - **Özet Mantık:** Kendi yeteneğinizi/gücünüzü geliştirdiğinizde, rakibiniz stratejisini buna adapte eder (güçlü yönünüze daha az oynar). Dolayısıyla siz de o güçlü yönünüzü eskisine kıyasla **daha az** koruma eğiliminde olursunuz [[01:11:30](https://www.youtube.com/watch?v=unvJofv0wl8&t=4290)].

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    9. Mixed strategies in theory and tennis

    YaleCourses · 81K views

     [Open in 9. Mixed strategies in theory and tennis](http://www.youtube.com/watch?v=unvJofv0wl8)](http://www.youtube.com/watch?v=unvJofv0wl8)

    ![](https://i.ytimg.com/vi/unvJofv0wl8/hqdefault.jpg)
