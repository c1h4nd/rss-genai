# European Intellectual History since Nietzsche: Class 23, “Antipolitics” & the Philosophy of Dissent

<https://www.youtube.com/watch?v=94b025iHtAw>

Verdiğin YouTube bağlantısı (94b025iHtAw) Andrej Karpathy'nin ünlü **"Let's build GPT: from scratch, in code, spelled out."** başlıklı videosuna ait.

Bu videoda Karpathy, OpenAI'ın GPT-2 / GPT-3 mimarisini temel alarak sıfırdan bir **Decoder-only Transformer** (Generative Pre-trained Transformer) modelini `PyTorch` kullanarak adım adım inşa ediyor.

Soru-cevap ve önemli noktaları konseptlerine göre detaylandırılmış olarak aşağıda bulabilirsin:

### 1. Giriş ve Veri Seti hazılama (Data Preparation)

- **Dataset:** Uygulama için Tiny Shakespeare (Shakespeare eserlerinden oluşan ~1MB'lık metin dosyası) kullanılıyor.
- **Tokenization:**

  - Metinler token'lara ayrılır. Üretim seviyesinde (production) **Byte Pair Encoding (BPE)** (örneğin OpenAI'ın `tiktoken` kütüphanesi) kullanılırken, anlaşılabilirlik açısından bu derste **character-level tokenization** tercih ediliyor.
  - Her benzersiz karakter bir integer'a (ID) eşlenir.
- **Train / Validation Split:** Verinin %90'ı eğitim (train), %10'u doğrulama (validation) için ayrılır.
- **Context Length (Block Size):** Modelin bir kerede tahmin yapmak için baktığı maksimum karakter uzunluğudur.
- **Batch Size:** Paralel işlem yapmak için aynı anda GPU'ya gönderilen bağımsız metin dizilerinin (sequences) sayısıdır.

### 2. Başlangıç Modeli: Bigram Language Model

- **Basit Başlangıç:** Karpathy önce sadece bir önceki karaktere bakarak bir sonraki karakteri tahmin eden en basit model olan **Bigram Model** ile başlıyor.
- **Embedding Matrix:** Karakter ID'leri bir `nn.Embedding` tablosuna girer ve doğrudan bir sonraki karakterin *logits* (ham olasılık) değerlerini verir.
- **Loss Function:** Tahmin edilen logits ile gerçek hedef (target) arasındaki farkı ölçmek için **Cross-Entropy Loss** kullanılır.
- **Optimization:** `PyTorch` içindeki `torch.optim.AdamW` optimizer'ı kullanılarak loss değeri düşürülür.

### 3. Self-Attention Mekanizması (Çekirdek Konsept)

Self-Attention, her token'ın diğer token'larla iletişim kurarak bağlam (context) toplamasını sağlar.

- **Query, Key, Value (Q,K,VQ, K, VQ,K,V):**

  - **Query (QQQ):** Token'ın *"Ne arıyorum?"* sorusudur.
  - **Key (KKK):** Token'ın *"Ben neyim/neye sahibim?"* cevabıdır.
  - **Value (VVV):** Token'ın *"Eğer benimle ilgileniyorsan sana aktaracağım bilgi budur"* değeridir.
- **Affinity (Akan Bilgi Miktarı):** Query ve Key vektörlerinin iç çarpımı (Q×KTQ \times K^TQ×KT) alınarak token'ların birbiriyle olan ilişkisi/alaka düzeyi hesaplanır.
- **Scaled Dot-Product Attention:** Matematiksel kararlılık için Q×KTQ \times K^TQ×KT sonucu dk\sqrt{d\_k}dk​![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
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
  M834 80h400000v40h-400000z"></path></svg>)​ (dkd\_kdk​: head size) değerine bölünür. Aksi takdirde Softmax çıktısı çok keskinleşir (one-hot benzeri) ve gradient'lar yok olur.

### 4. Causal Masking (Decoder Özelliği)

- **Autoregressive Özellik:** Model gelecek zaman adımlarındaki token'ları "görmemelidir" (örneğin 3. token tahmin edilirken 4. ve 5. token gizlenmelidir).
- **Masking (Tril Matrix):** Gelecek pozisyonlara denk gelen değerlere −∞-\infty−∞ (eksi sonsuz) verilir. Softmax alındığında bu −∞-\infty−∞ değerleri 000 olasılığa dönüşür ve geçmiş bilgiyle gelecek bilgi izole edilir.

### 5. Multi-Head Attention & Feed-Forward Block

- **Multi-Head Attention:**

  - Tek bir büyük Attention mekanizması yerine, veriyi farklı alt uzaylara (subspaces) bölen birden fazla "Head" (kafa) paralel çalıştırılır.
  - Örneğin tek bir head karakterlerin harf dizilimine bakarken, diğer bir head noktalama işaretlerine odaklanabilir. Çıktılar en sonda birleştirilir (`torch.cat`).
- **Feed-Forward Network (FFN):**

  - Attention sadece token'ların birbiriyle iletişim kurmasını (communication) sağlar.
  - FFN ise her bir token'ın bu iletişimden aldığı bilgiyi bağımsız olarak işlemesini ve "düşünmesini" (computation) sağlayan basit bir MLP (Multi-Layer Perceptron) bloğudur (Linear→ReLU→LinearLinear \rightarrow ReLU \rightarrow LinearLinear→ReLU→Linear).

### 6. Mimariyi Büyütme: Transformers (Residuals & Norms)

Model derinleştikçe yaşanan "vanishing/exploding gradient" ve "training instability" problemlerini çözmek için eklenen teknikler:

- **Residual Connections (Skip Connections):**

  - Girdinin, bloğun çıktısına doğrudan eklenmesi (x+f(x)x + f(x)x+f(x)).
  - Backpropagation sırasında gradient'ların hiçbir engel olmadan geriye doğru akmasını (gradient highway) sağlar.
- **Layer Normalization (LayerNorm):**

  - BatchNorm'dan farklı olarak, batch boyutundan bağımsız çalışır ve her bir örneğin kendi feature'larını normalize eder.
  - GPT-2 mimarisinde LayerNorm, Attention ve FFN bloklarının **önüne** eklenmiştir (**Pre-LN** yapısı).
- **Dropout:**

  - Eğitim sırasında nöronların belirli bir yüzdesini rastgele sıfırlayarak modelin ezber yapmasını (overfitting) önleyen bir regularization yöntemidir.

### 7. Final GPT Mimarisi ve Kod Yapısı

Tüm bileşenler bir araya getirilerek ana `GPTLanguageModel` oluşturulur:

1. **Input:** Character IDs + Positional Embeddings (Karakterlerin pozisyon bilgisi).
2. **Blocks:** Peş peşe dizilmiş N adet Transformer Block (`Multi-Head Attention` + `Feed-Forward` + `LayerNorm` + `Residuals`).
3. **Final LayerNorm & LM Head:** Çıktı önce son bir LayerNorm'dan geçer, ardından vocabulary boyutuna dönüştüren bir Linear katman (`lm_head`) ile karakter logits değerleri üretilir.
4. **Generation:** Model eğitildikten sonra `softmax` ve `torch.multinomial` ile bir sonraki karakter örneklenerek (sampling) metin üretimi gerçekleştirilir.

Karpathy'nin kodladığı bu nihai Transformer modeli, doğru hiperparametreler ile eğitildiğinde Tiny Shakespeare verisinde oldukça başarılı, Shakespeare üslubuna benzeyen anlamlı metinler üretebilir hale geliyor.

Bu özette açıklanmasını istediğin spesifik bir teknik detay (örneğin *Scaled Dot-Product'ın matematiksel açıklaması* veya *Positional Embedding'lerin mantığı*) var mı?
