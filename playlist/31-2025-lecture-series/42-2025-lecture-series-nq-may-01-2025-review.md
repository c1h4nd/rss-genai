# 2025 Lecture Series - NQ May 01, 2025 Review

<https://www.youtube.com/watch?v=AmTpyveQsbg>

Verdiğiniz YouTube linki (**`[https://www.youtube.com/watch?v=AmTpyveQsbg](https://www.youtube.com/watch?v=AmTpyveQsbg)`** / Andrej Karpathy'nin ünlü **"Let's build GPT: from scratch, in code, spelled out."** videosu) göz önünde bulundurularak hazırlanan detaylı, teknik ve maddeler halinde özeti aşağıda bulabilirsiniz.

Teknik jargon, fonksiyon ve parametre isimleri orjinal **İngilizce** halleriyle korunmuştur.

## 1. Giriş ve Genel Bakış (Introduction & Overview)

- **Amaç:** GPT (Generative Pre-trained Transformer) ve ChatGPT tarzı Büyük Dil Modellerinin (LLM) sıfırdan (`from scratch`), Python ve PyTorch kullanarak adım adım kodlanması ve eğitilmesi.
- **Veri Kümesi (Dataset):** Shakespeare eserlerinden oluşan küçük bir metin dosyası (`Tiny Shakespeare`, ~1MB).
- **Tokenization Düzeyi:** Model basitleştirmek adına **Character-level Tokenizer** kullanır. Metindeki her benzersiz karakter bir tamsayıya (`integer`) dönüştürülür.

## 2. Veri Hazırlığı ve İnceleme (Data Preparation & Loading)

- **Vocabulary (Vocab):** Verisetindeki tüm benzersiz karakterler çıkarılır (`vocab_size` yaklaşık 65 karakter).
- **Encode / Decode Functions:**

  - `encode`: Metni tamsayı listesine dönüştürür (`string -> List[int]`).
  - `decode`: Tamsayı listesini tekrar okunabilir metne dönüştürür (`List[int] -> string`).
- **Train / Validation Split:** Verinin %90'ı eğitim (`train_data`), %10'u doğrulama (`val_data`) için ayrılır.
- **Data Loader & Context Window:**

  - `block_size` (veya `context_length`): Modelin tahmin yaparken geriye dönük bakacağı maksimum token sayısı.
  - `batch_size`: Parallel processing için bir adımda GPU/CPU'ya gönderilen bağımsız dizi sayısı.
  - Model, bir dizideki her adımda bir sonraki token'ı tahmin etmeyi öğrenir (`Predict the next token given the context`).

## 3. Temel Model: Bigram Language Model

- Karpathy, karmaşık mimariye geçmeden önce en basit baseline olan **Bigram Language Model**'i kurar.
- **Embedding Lookup Table:** Karakter index'ini doğrudan bir sonraki karakterin olasılıklarını belirten **Logits** değerlerine eşler (`nn.Embedding(vocab_size, vocab_size)`).
- **Loss Function:** Tahmin edilen logits ile gerçek hedef (target) arasındaki farkı ölçmek için **Cross Entropy Loss** (`nn.functional.cross_entropy`) kullanılır.
- **Generation:** `torch.multinomial` kullanılarak logits değerlerinden olasılıksal örnekleme (sampling) yapılır ve adım adım metin üretilir.

## 4. Optimization ve Training Loop

- **Optimizer:** Klasik SGD yerine Transformer yapılarında standart olan **AdamW** optimizer tercih edilir.
- **Training Step:** Forward pass →\rightarrow→ Loss hesaplama →\rightarrow→ `zero_grad()` →\rightarrow→ Backward pass (`loss.backward()`) →\rightarrow→ Optimizer adımı (`optimizer.step()`).
- **Evaluation:** Modelin eğitim esnasındaki Overfitting durumunu takip etmek için düzenli aralıklarla train ve validation loss hesaplayan bir `estimate_loss` yardımcı fonksiyonu yazılır.

## 5. Self-Attention Mekanizmasının İnşası

Self-Attention, Transformer mimarisinin kalbidir. Token'ların kendi aralarında iletişim kurmasını sağlar.

- **Queries, Keys, and Values (Q, K, V):**

  - **Query (QQQ):** Token'ın ne aradığı (`what am I looking for?`).
  - **Key (KKK):** Token'ın ne içerdiği (`what do I contain?`).
  - **Value (VVV):** Token'ın aktarmak istediği bilgi (`what information do I communicate?`).
  - Q=X⋅WqQ = X \cdot W\_qQ=X⋅Wq​, K=X⋅WkK = X \cdot W\_kK=X⋅Wk​, V=X⋅WvV = X \cdot W\_vV=X⋅Wv​ işlemleri Linear layer'lar ile yapılır.
- **Attention Scores & Matrix Multiplication:**

  - Affinity (ilgi) matrisi: Q⋅KTQ \cdot K^TQ⋅KT ile hesaplanır.
- **Masking (Causal Self-Attention / Decoder Attention):**

  - Dil modellerinde gelecekteki token'ları görmemek zorunludur.
  - Matrisin üst üçgen kısmı −∞-\infty−∞ (`-inf`) ile doldurulur (`tril` masking).
  - Softmax uygulandığında bu −∞-\infty−∞ değerleri 000 olasılığa dönüşür, böylece token'lar yalnızca geçmişe bakar.
- **Scaled Dot-Product Attention:**

  - Variance patlamasını önlemek için Q⋅KTQ \cdot K^TQ⋅KT sonucu dk\sqrt{d\_k}dk​![](data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
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
    M834 80h400000v40h-400000z"></path></svg>)​ (head dimension'ın karekökü) değerine bölünür.
- **Multi-Head Attention:**

  - Tek bir büyük attention kanalı yerine, bağımsız çalışan birden fazla "Head" (ör. 4 veya 8 head) paralel hesaplama yapar.
  - Her head farklı ilişkileri (ör. dilbilgisi, isim-fiil uyumu vs.) öğrenir.
  - Çıktılar en sonda `torch.cat` ile birleştirilir.

## 6. Feed-Forward Network & Transformer Block

- **Position-wise Feed-Forward Network (FFN):**

  - Self-Attention iletişim evresidir. FFN ise her token'ın kendi içinde elde edilen bilgiyi işlemesini (computation / thinking phase) sağlayan basit bir MLP'dir (`Linear -> ReLU/GELU -> Linear`).
- **Residual Connections (Skip Connections):**

  - Derin ağlarda gradient vanishing/exploding problemlerini engellemek için girdi doğrudan bloğun çıkışına eklenir (`x = x + SelfAttention(x)`).
- **Layer Normalization (LayerNorm):**

  - Activations'ların dağılımını optimize etmek için kullanılır.
  - Karpathy, modern LLM'lerde (ör. GPT-2/GPT-3) tercih edilen **Pre-LN** yapısını uygular (LayerNorm, Attention/FFN öncesinde çağrılır).
- **Dropout:** Overfitting'i önlemek için network'e Regularization amacıyla Dropout eklenir.

## 7. Modelin Büyütülmesi ve GPT Yapısının Tamamlanması

- Tüm parçalar `Block` sınıfı altında birleştirilir ve bu bloklar üst üste dizilir (`nn.Sequential` ile `n_layer` kadar).
- **Positional Embeddings:** Transformer yapısı sıradan bağımsız çalıştığı için, her token'ın dizideki konumunu belirten `position_embedding_table` (`nn.Embedding(block_size, n_embd)`) eklenir.
- **Son Mimari (Hyperparameters):**

  - `n_embd`: Embedding boyutu.
  - `n_head`: Attention head sayısı.
  - `n_layer`: Katman (Block) sayısı.
  - `block_size`: Context window genişliği.

## 8. NanoGPT Eğitimi ve Sonuçlar

- Script GPU üzerine taşınır (`device = 'cuda' if torch.cuda.is_available() else 'cpu'`).
- Model eğitildikten sonra başlangıç prompt'u verilerek Shakespeare tarzında mantıklı, kelime yapısına uyan yeni metinler üretilir.

## 9. ChatGPT / Pre-training & Fine-Tuning Ek Açıklamaları

Videonun son kısmında Karpathy, kendi kodladığı temel dil modelinden (Base Model) ChatGPT gibi bir asistana nasıl geçildiğini açıklar:

1. **Pre-training:** Büyük internet verisi üzerinde bir sonraki kelimeyi tahmin etme eğitimi (Videonun ana konusu).
2. **Supervised Fine-Tuning (SFT):** Soru-Cevap formatındaki özel diyalog verisetleri ile modelin asistana dönüştürülmesi.
3. **RLHF (Reinforcement Learning from Human Feedback):** İnsan tercihlerine (PPO / Reward Model) göre yanıtların kalitesini, güvenliğini ve hizalanmasını (alignment) artırma.
