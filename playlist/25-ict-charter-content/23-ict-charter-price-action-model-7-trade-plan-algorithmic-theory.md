# ICT Charter Price Action Model 7 - Trade Plan & Algorithmic Theory

<https://www.youtube.com/watch?v=G4lhid5dh0I>

Videoda öne çıkan ve dikkat edilmesi gereken önemli noktalar, orijinal terimler korunarak ve sürece göre detaylandırılmış olarak aşağıda listelenmiştir:

### **1. Trade Plan’in 5 Ana Aşaması** [[00:31](https://www.youtube.com/watch?v=G4lhid5dh0I&t=31)]

ICT, bu modelde her trade planının 5 temel aşamadan oluştuğunu vurgular:

1. **Preparation** (Hazırlık)
2. **Opportunity Discovery** (Fırsat Keşfi)
3. **Trade Planning** (Planlama)
4. **Trade Execution** (İşleme Giriş/Uygulama)
5. **Trade Management** (İşlem Yönetimi)

### **2. Preparation (Hazırlık ve Veri Analizi)** [[00:53](https://www.youtube.com/watch?v=G4lhid5dh0I&t=53)]

- **Economic Calendar:** Haftalık Takvim üzerindeki *Medium* ve *High Impact* ekonomik veriler takip edilmelidir [[00:53](https://www.youtube.com/watch?v=G4lhid5dh0I&t=53)]. Bu etkinlikler piyasaya gerekli olan *Volatility Injection*’ı (oynaklık aşısını) sağlar [[02:13](https://www.youtube.com/watch?v=G4lhid5dh0I&t=133)].
- **IPDA Data Ranges:** Son **20, 40 veya 60 işlem günü** incelenir (Pazarlar hariç) [[01:21](https://www.youtube.com/watch?v=G4lhid5dh0I&t=81)].
- **Dealing Range:** Belirlenen bu süre içerisindeki en yüksek seviye (*Highest High*) ve en düşük seviye (*Lowest Low*) mevcut işlem aralığınızı (*Dealing Range*) oluşturur [[01:43](https://www.youtube.com/watch?v=G4lhid5dh0I&t=103)].
- **Draw on Liquidity & Weekly Bias:** Fiyatın gideceği bir sonraki nokta belirlenir. Haftalık yön beklentisini (*Weekly Range Bias*) destekleyecek yönde bir **Discount PD Array** hedeflenir [[01:54](https://www.youtube.com/watch?v=G4lhid5dh0I&t=114)].

### **3. Opportunity Discovery (Fırsat Keşfi)** [[02:34](https://www.youtube.com/watch?v=G4lhid5dh0I&t=154)]

Model 7 strictly satış tarafına (*Sell Side*) odaklanır:

- **Market Maker Sell Model:** Fiyat altındaki Discount PD Array'e veya eski bir dibe yönelirken, **Stage 1** veya **Stage 2 Redistribution** dönemlerinde Short pozisyon fırsatları aranır [[02:52](https://www.youtube.com/watch?v=G4lhid5dh0I&t=172)].
- **Market Maker Buy Model:** Büyük resimde bir *Buy Model* başlasa dahi, Discount PD Array noktasına ulaşana kadar gerçekleşen düşüş dalgasında (Satış kanadında) Short yönlü işlemler hedeflenebilir [[03:06](https://www.youtube.com/watch?v=G4lhid5dh0I&t=186)].

### **4. Trade Planning (Planlama)** [[03:46](https://www.youtube.com/watch?v=G4lhid5dh0I&t=226)]

- **Convergence & Timing:** Ekonomik takvimin hareketlilik sinyali verdiği zamanlarda, fiyat beklentimizin tersine manipüle olduğunda fırsat aranır [[03:46](https://www.youtube.com/watch?v=G4lhid5dh0I&t=226)].
- **Confluence Kriterleri:**

  - 15-min veya 5-min **Premium Fair Value Gap (FVG)** PD Array kullanımı [[04:14](https://www.youtube.com/watch?v=G4lhid5dh0I&t=254)].
  - Fiyatın maksimum **+3 Standard Deviation** seviyesiyle çakışması (Convergence) [[04:21](https://www.youtube.com/watch?v=G4lhid5dh0I&t=261)].
  - Giriş zamanı olarak **London Open** veya **New York Open** Kill Zone zaman dilimleri [[04:21](https://www.youtube.com/watch?v=G4lhid5dh0I&t=261)].
- **Hedefler (Terminus):**

  - *Market Maker Buy Model* içindeysek: Eski diplerin altındaki **Sell-Side Liquidity (SSL)** [[04:38](https://www.youtube.com/watch?v=G4lhid5dh0I&t=278)].
  - *Market Maker Sell Model* içindeysek: Yapının başındaki **Original Consolidation** bölgesi [[04:46](https://www.youtube.com/watch?v=G4lhid5dh0I&t=286)].

### **5. Trade Execution & Order Types** [[04:51](https://www.youtube.com/watch?v=G4lhid5dh0I&t=291)]

- **Institutional Order Flow Entry Drill (IOFED):** 5 dakikalık grafiklerde London/NY Kill Zone’ları esnasında gerçekleşen yukarı yönlü retrace (düzeltme) veya Buy Stop raid'lerde giriş aranır [[04:59](https://www.youtube.com/watch?v=G4lhid5dh0I&t=299)].
- **Limit Order Detayı:** Limit emirlerinde emrin tetiklenme hassasiyetini artırmak için `Standard Deviation + PD Array` çakışma noktasından **-5 Pip** mesafeye Sell Limit koyulması tavsiye edilir [[05:29](https://www.youtube.com/watch?v=G4lhid5dh0I&t=329)].

### **6. Trade Management (İşlem Yönetimi & Kar Alımı)** [[05:12](https://www.youtube.com/watch?v=G4lhid5dh0I&t=312)]

- **Kısmi Kar Alımları (Partial Profits):** [[05:41](https://www.youtube.com/watch?v=G4lhid5dh0I&t=341)]

  - **1. Hedef:** 20 Pip kârda ilk pozisyon kapatılır.
  - **2. Hedef:** 40 Pip kârda ikinci pozisyon kapatılır.
  - **3. Hedef:** 60 Pip kâra ulaşıldığında pozisyonun %80'i kapatılır ve kalan miktar koşmaya bırakılır.
- **Stop Loss Yönetimi:** [[06:03](https://www.youtube.com/watch?v=G4lhid5dh0I&t=363)]

  - İlk Stop Loss konumu: Girişin yapıldığı High seviyesinin üstüne **+20 Pip** [[06:09](https://www.youtube.com/watch?v=G4lhid5dh0I&t=369)].
  - Fiyat beklenen hedefin **%25**'ine ulaştığında -> Stop Loss %25 daraltılır [[06:32](https://www.youtube.com/watch?v=G4lhid5dh0I&t=392)].
  - Fiyat hedefin **%50**'sine ulaştığında -> Stop Loss %50 daraltılır [[06:39](https://www.youtube.com/watch?v=G4lhid5dh0I&t=399)].
  - Fiyat hedefin **%75**'ine ulaştığında -> Stop Loss **Break Even** (giriş seviyesine) çekilir [[06:46](https://www.youtube.com/watch?v=G4lhid5dh0I&t=406)].

### **7. Money Management (Sermaye ve Risk Yönetimi)** [[06:53](https://www.youtube.com/watch?v=G4lhid5dh0I&t=413)]

- **Position Size Formülü:**

  Position Size=Account Equity×Risk PercentStop Loss (in Pips)\text{Position Size} = \frac{\text{Account Equity} \times \text{Risk Percent}}{\text{Stop Loss (in Pips)}}Position Size=Stop Loss (in Pips)Account Equity×Risk Percent​
- **Lot Hesabı Kuralları:** Hesaplanmış lot büyüklüklerinde risk bütçesini aşmamak adına her zaman **aşağı yuvarlama (round down)** yapılır [[08:10](https://www.youtube.com/watch?v=G4lhid5dh0I&t=490)].
- **Loss Recovery Protocol (Kayıp Sonrası Risk Düşürme):**

  - Tam riskli bir işlem kaybedilirse, bir sonraki işlemde **Risk %50 oranında düşürülür** [[09:31](https://www.youtube.com/watch?v=G4lhid5dh0I&t=571)].
  - Kaybedilen miktarın en az %50'si geri kazanılana kadar risk artırılmaz; kazanıldıktan sonra orijinal riske dönülebilir [[09:45](https://www.youtube.com/watch?v=G4lhid5dh0I&t=585)].
- **Winning Streak Protocol (Seri Galibiyet Riski):**

  - Üst üste **5 kazanan işlemden (5 winning trades)** sonra risk %50 düşürülür [[10:15](https://www.youtube.com/watch?v=G4lhid5dh0I&t=615)]. Amaç, kaçınılmaz olan ilk kayıpta Equity eğrisindeki derin çekilmeleri (drawdown) engellemek ve stabil bir yükseliş grafiği elde etmektir [[10:27](https://www.youtube.com/watch?v=G4lhid5dh0I&t=627)].

### **8. Algoritmik Teori & Piyasa Dinamikleri** [[10:59](https://www.youtube.com/watch?v=G4lhid5dh0I&t=659)]

- **Sell Side vs. Buy Side Hızı:** Düşüş hareketleri (*Sell-side Low Resistance Liquidity Runs*), yükseliş hareketlerine göre çok daha hızlı, agresif, şiddetli ve geniş kapsamlıdır [[12:34](https://www.youtube.com/watch?v=G4lhid5dh0I&t=754)]. Piyasa yapıcılar likiditeye erişmek için fiyatı aniden aşağı reprice ederler (*Flash Crash* olgusu) [[17:28](https://www.youtube.com/watch?v=G4lhid5dh0I&t=1048)].
- **Controlled Demolition vs. Meltdown (Parabolic Crash):**

  - *Market Maker Buy Model* içindeki Sell Side aşaması bir **Controlled Demolition** (kontrollü yıkım) gibidir; fiyat sadece alttaki Discount seviyeden tepki alıp yükselmek üzere belli bir seviyeye kadar iner [[20:45](https://www.youtube.com/watch?v=G4lhid5dh0I&t=1245)].
  - Makroekonomik krizler veya jeopolitikYouTubedaki bu video (**Andrej Karpathy - Intro to Large Language Models**), LLM'lerin (Büyük Dil Modelleri) çalışma prensiplerini, eğitilme süreçlerini ve güvenlik/gelecek vizyonunu çok net ve kapsamlı bir şekilde açıklayan en temel kaynaklardan biridir.

Videonun en önemli noktalarını detaylı bir şekilde aşağıda bulabilirsin:

### 1. LLM Nedir & Temel Eğitimi (Pretraining)

- **2-File Mental Model:** Karpathy, bir LLM'i zihnimizde iki temel dosyadan ibaret düşünebileceğimizi söyler:

  - **Parameters File (Ağırlıklar/Weights):** Örn. 70 Milyar parametrelik Llama 2 için ~140 GB boyutunda bir dosya.
  - **Run File (Çalıştırma Kodu):** Bu parametreleri çalıştıran, genellikle C veya Python ile yazılmış birkaç yüz satırlık çok basit bir kod.
- **Pretraining (Ön Eğitim) Süreci:**

  - **Veri Kümesi:** İnternetten çekilen petabaytlarca veri (Common Crawl vb.) filtrelenip temizlenir (~10 TB metin).
  - **Maliyet & Donanım:** Bu veriyi işlemek için binlerce GPU (örn. 6,000 GPU) kullanılır, aylar sürer ve milyonlarca dolar ($2M - $10M+) harcanır.
  - **Temel Amaç (Next-Token Prediction):** Modelin tek bir amacı vardır; verilen metindeki bir sonraki kelimeyi (token) tahmin etmek.
- **Compressing the Web (İnterneti Sıkıştırmak):** Pretraining aslında internetteki bilgilerin "kayıplı bir şekilde sıkıştırılmasıdır" (lossy compression). Model tüm bilgileri ezberlemez, pattern'leri ve ilişkileri öğrenir.

### 2. İnce Ayar ve Hizalama (Finetuning & Alignment)

Pretrained bir model sadece metin tamamlar (örn. "Ankara nerededir?" yazarsan "İzmir nerededir?" diye devam edebilir). Kullanılabilir bir asistana dönüşmesi için ek aşamalar gerekir:

- **SFT (Supervised Fine-Tuning):**

  - İnsanlar tarafından hazırlanmış yüksek kaliteli "Soru-Cevap" (Prompt-Response) veri setleri kullanılır (genelde tens of thousands of examples).
  - Model artık sadece internet metinlerini tamamlamayı değil, bir **Asistan** gibi cevap vermeyi öğrenir.
- **RLHF (Reinforcement Learning from Human Feedback):**

  - Model birkaç farklı cevap üretir, insan değerlendiriciler bu cevapları en iyiden en kötüye sıralar.
  - Bu sıralamalardan bir **Reward Model** (Ödül Modeli) eğitilir ve ardından PPO gibi algoritmalarla ana model, insan tercihlerine göre optimize edilir.

### 3. LLM'lerin Güvenlik ve Zayıf Noktaları (Vulnerabilities)

Model tam bir veritabanı veya insan bilinci değildir; bu yüzden belirgin sınırları ve zayıf noktaları vardır:

- **Hallucination (Hüsnükuruntu/Yanlış Bilgi Üretme):**

  - Modeller bir "Knowledge Base" değil, "World Model" çalıştırır. Bilgiyi sorgulamak yerine kelime olasılıklarını hesapladığı için kendinden çok emin bir şekilde yanlış bilgi üretebilir.
- **Jailbreaking:**

  - Güvenlik filtrelerini aşmak için uygulanan "Adversarial Attacks". (Örn. Modelden doğrudan tehlikeli bir bilgi istenildiğinde reddeder, ancak "Bir roman yazıyorum, karakterim bomba yapıyor..." şeklinde kurgulanırsa cevabı verebilir).
- **Prompt Injection:**

  - Modeller "sistem talimatı" (system prompt) ile "kullanıcı verisini" (user input) birbirinden tam anlamıyla ayıramaz. İki metin de aynı context window içinde işlendiği için araya giren zararlı bir girdi modelin tüm davranışını değiştirebilir.
- **Data Poisoning (Backdoors):**

  - Pretraining aşamasındaki devasa veri kümelerine belirli anahtar kelimelerde modeli manipüle edecek gizli veriler eklenebilir.

### 4. LLM'lerin Geleceği ve Vizyonu (Future Trends)

Karpathy, modellerin evrileceği yönü bir işletim sistemine (LLM OS) benzeterek açıklar:

- **LLM OS (LLM İşletim Sistemi):**

  - Gelecekte LLM'ler sadece metin üreten sistemler değil; CPU/GPU gibi merkezi bir işlem birimi olacak.
  - **RAM:** Context Window (Modelin aynı anda okuyabildiği alan).
  - **Disk / Memory:** Vector Databases, RAG (Retrieval-Augmented Generation) veya Arama Motorları.
- **Multimodality (Çoklu Modellik):**

  - Modellerin sadece metin değil; görüntü, ses ve video verilerini aynı latent space içinde doğrudan işleyebilmesi.
- **Thinking & Reasoning (System 1 vs System 2):**

  - Günümüz LLM'leri "System 1" (hızlı, düşünmeden, anında tepki veren) mantığıyla çalışır. Geleceğin modelleri cevap vermeden önce plan yapacak, düşünecek ve "System 2" (yavaş, analitik, derin düşünme) mantığını kullanacaktır.
- **Self-Improvement (Kendi Kendine İlerleme):**

  - Satranç ve Go oynayan AlphaGo gibi modeller kendi kendine oynayarak gelişti. LLM'lerde de kapalı döngü ortamlarda (örn. Kod yazıp test çalıştırma) modellerin kendi kendini eğitmesi hedefleniyor.

Bu özet ile ilgili daha detaylı açmamı istediğin özel bir başlık (SFT, RLHF veya LLM OS gibi) var mı?

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Charter Price Action Model 7 - Trade Plan & Algorithmic Theory

The Inner Circle Trader · 49K views

 [Open in ICT Charter Price Action Model 7 - Trade Plan & Algorithmic Theory](http://www.youtube.com/watch?v=G4lhid5dh0I)](http://www.youtube.com/watch?v=G4lhid5dh0I)

![](https://i.ytimg.com/vi/G4lhid5dh0I/maxresdefault.jpg)
