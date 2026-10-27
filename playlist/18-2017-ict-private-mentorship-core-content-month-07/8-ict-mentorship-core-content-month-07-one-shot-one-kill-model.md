# ICT Mentorship Core Content - Month 07 - One Shot One Kill Model

<https://www.youtube.com/watch?v=LBlK6JB0QS0>

"**ICT Mentorship Core Content - Month 07 - One Shot One Kill Model**" başlıklı videoda öne çıkan ve detaylandırılan önemli noktalar şunlardır:

### 1. Modelin Temel Ön Koşulları (Prerequisites)

- **Macro Conditions & IPDA Data Ranges:** Son 20, 40 ve 60 işlem gününe bakarak IPDA Data Ranges ve **PD Array Matrix** konseptlerini hem zaman hem de fiyat üzerinde etkin şekilde uygulamak.
- **Modül Entegrasyonları:** Position Trading, Swing Trading, Short-Term Trading ve ICT Day Trading modüllerindeki konseptlerin bir arada kullanılması.
- **Power of 3 (PO3):** Haftalık mumlar/aralıklar (weekly candles/ranges) üzerinde Power of 3 konseptini uygulamak.
- **Day of Week Concept:** Haftalık yüksek veya düşük seviyenin (High/Low of Week) %76 ihtimalle **Pazartesi – Çarşamba** günleri arasında oluşacağını bilmek.
- **Zamanlama ve Mevsimsellik:**

  - Girişler için **ICT Kill Zones** ve **Time of Day** kurallarına uymak.
  - Yönsel beklentiyi (directional bias) doğrulamak için **Seasonal Changes / Seasonal Tendencies** takibi yapmak.
- **COT & Commercial Hedging:** **Commitment of Traders (COT)** analizi ve kurumsal (Commercial) hedge programlarının mantığını kavramak.

### 2. One Shot One Kill İşlem Adımları (Procedure)

- **Quarterly Shift:** Mevcut veya olası bir sonraki **Quarterly Shift** yönünü belirlemek.
- **Higher Time Frame PD Arrays:** Üst zaman dilimlerindeki (HTF) PD Array seviyelerini tespit etmek.
- **Faiz Oranları (Interest Rate Differentials):** Hazine tahvilleri (Treasuries, Bund vb.) trend halinde mi yoksa konsolide mi? Faiz oranları trendde ise döviz çiftlerinde (ör. EUR/USD) hareket alanı oluşur.
- **Swing Analizi (Fractal Structure):** HTF’den 60 dakikalık (1-Hour) grafiklere inerek fiyat sal"**Let's build the GPT Tokenizer from scratch**" (Andrej Karpathy) başlıklı YouTube videosunun detaylı ve önemli noktalarını kapsayan özeti aşağıda bulabilirsin. Orijinal teknik terimler korunmuştur:

## 1. Tokenization Nedir ve Neden Önemlidir?

- **Temel Tanım:** Tokenization, ham metni (raw text) LLM'lerin (Large Language Models) işleyebileceği sayılara (**Token ID**) dönüştürme ve tekrar metne çevirme (encode/decode) işlemidir.
- **LLM Problemlerinin Kökü:** Karpathy, LLM'lerde karşılaşılan birçok tuhaf davranışın arkasında **Tokenization** olduğunu vurgular:

  - Modelin basit dize (string) manipülasyonlarını (örn. kelimeyi ters çevirme) yapamaması.
  - İspanyolca veya Türkçe gibi dillerde/kodlama görevlerinde performans düşüklüğü.
  - `100000 + 10000` gibi basit matematiksel işlemlerde zorlanma.
  - Trailing whitespace (sonlanan boşluk) uyarıları ve "Python print" hataları.
  - `"<|endoftext|>"` gibi **Special Token** enjeksiyonuyla modelin çökmesi.

## 2. Karakter Seviyesinden Byte Seviyesine Geçiş

- **ASCII & Unicode Standardı:**

  - Unicode, her karaktere bir **Code Point** atar (örn. 'A' →\rightarrow→ `U+0041`).
  - Ancak Unicode code point'leri doğrudan token olarak kullanmak verimsizdir (150.000+ karakter var, vocabulary çok büyür).
- **UTF-8 Encoding:**

  - Metinler hafızada **UTF-8** bayt dizilimi (byte stream) olarak saklanır.
  - UTF-8, değişken uzunluktadır (1 ila 4 byte arası).
  - Temel vocabulary boyutunu **256** (8-bit byte karşılığı) olarak başlatmak, dünyadaki tüm metinleri ve medyayı kapsamanın en minimalist yoludur.

## 3. Byte Pair Encoding (BPE) Algoritması

Metni sadece 256 bayt ile ifade etmek dizileri çok uzatacağı için **BPE (Byte Pair Encoding)** algoritması ile vocabulary genişletilir.

### BPE Eğitim (Training) Mantığı:

1. **İstatistik Toplama:** Metindeki en sık yan yana gelen bayt çifti (adjacent pair) bulunur.
2. **Merge (Birlestirme):** En sık tekrarlanan bu çift, vocabulary'e yeni bir token id olarak eklenir (örn. `101 108` baytları →\rightarrow→ yeni `256` token'ı).
3. **Iterative Process:** Belirlenen `vocab_size` hedefine (örn. 512, 32k, 100k) ulaşılana kadar bu işlem tekrarlanır.
4. **Minting Rules:** Yeni oluşturulan her birleştirme kuralı `merges` sözlüğünde tutulur.

### Encoding & Decoding:

- **Encoding:** Girdideki baytlar sırayla taranır ve eğitilen `merges` kurallarına göre birleştirilerek nihai token ID dizisi oluşturulur.
- **Decoding:** Token ID'leri vocabulary'deki karşılık gelen bayt dizilimlerine çevrilir ve UTF-8 decode (`errors='replace'`) uygulanarak string elde edilir.

## 4. Tiktoken ve Regex Split Mechanics (GPT-2 / GPT-4 Farkları)

- **Neden Regex Splitting Yapılır?**

  - BPE'nin kelime sınırlarını aşarak anlamsız birleştirmeler yapmasını engellemek için metin önce **Regex Pattern** ile parçalara bölünün (chunking).
  - Örneğin; harfler, sayılar ve noktalama işaretleri ayrı gruplara bölünür ki bir harf ile bir sayı asla tek bir token içinde birleşmesin.
- **GPT-2 vs. GPT-4 Tokenizer:**

  - **GPT-2:** Büyük/küçük harf duyarlılığı, noktalama ve harf ayrımı için temel bir regex kullanır.
  - **GPT-4:** Regex kalıbı güncellenmiştir. Özellikle sayıları daha küçük parçalara (1, 2 veya 3 basamaklı) bölerek modelin aritmetik yeteneğini artırmıştır. Ayrıca boşluk (whitespace) handling iyileştirilmiştir.

## 5. Special Tokens (Özel Token'lar)

- **Kontrol Token'ları:** Modelin metin sınırlarını, mesaj başlangıç/bitişlerini anlaması için eklenir.

  - Örneğin: `<|endoftext|>` (dizinin bittiğini belirtir), `<|im_start|>`, `<|im_end|>`.
- **Vocabulary Expansion:** Special token'lar var olan vocabulary'e ek (outer) ID'ler olarak eklenir (`vocab_size + 1`).
- **Security & Injection Issues:** Kullanıcı girdisinde special token string'i bulunursa (örn. prompt injection), tokenizer'ın bunu varsayılan olarak bir kontrol token'ı gibi değil, normal metin gibi encode etmesi (`allowed_special` parametre kontrolü) gerekir.

## 6. Model Parameters & Vocabulary Size Trade-off

- **Vocabulary Size Dengesi:**

  - **Küçük Vocab Size:** Token dizileri çok uzun olur →\rightarrow→ Transformer'ın attention mekanizması O(N2)O(N^2)O(N2) maliyetli olduğu için context window çabuk dolar ve hesaplama pahalılaşır.
  - **Büyük Vocab Size:** Token dizisi kısalır →\rightarrow→ Ancak embedding layer ve son linear head tabakası aşırı büyür, parametre sayısı ve GPU bellek kullanımı artar.
- **Llama 3 / VLM Dönemi:** Modern modellerde vocabulary boyutunun (32k'dan 128k+ seviyelerine) büyütülmesi trend haline gelmiştir.

Sormak istediğin veya kod aşamasında derinleşmek istediğin spesifik bir bölüm var mı?

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Mentorship Core Content - Month 07 - One Shot One Kill Model

The Inner Circle Trader · 210K views

 [Open in ICT Mentorship Core Content - Month 07 - One Shot One Kill Model](http://www.youtube.com/watch?v=LBlK6JB0QS0)](http://www.youtube.com/watch?v=LBlK6JB0QS0)

![](https://i.ytimg.com/vi/LBlK6JB0QS0/maxresdefault.jpg)
