# ICT Charter Price Action Model 9 - One Shot One Kill

<https://www.youtube.com/watch?v=twIPoG2TZ1o>

Bu video (**"Let's Build VectorDB - Part 1: Quantization & Vector Search"**), vektör veritabanlarının (VectorDB) arkasındaki temel matematiksel ve mimari prensipleri sıfırdan anlatmaktadır.

Öne çıkan önemli noktalar ve teknik detaylar şunlardır:

## 1. Vektör Arama (Vector Search) ve Temel Kavramlar

- **Neden VectorDB?**: Standart SQL veya NoSQL veritabanları tam eşleşme (exact match) ararken, vektör veritabanları yüksek boyutlu uzayda **anlamsal benzerlik (semantic similarity)** arar.
- **Similarity Metrics (Benzerlik Ölçütleri)**:

  - **Cosine Similarity**: İki vektör arasındaki açıyı ölçer. Vektörlerin uzunluklarından ziyade yönlerine (direction) odaklanır.
  - **Dot Product (İç Çarpım)**: Hem yönü hem de vektör büyüklüğünü (magnitude) hesaba katar. Vektörler normalize edilmişse Cosine Similarity ile aynı sonucu verir.
  - **Euclidean Distance (L2L\_2L2​ Distance)**: İki nokta arasındaki dik mesafeyi ölçer.

## 2. K-Nearest Neighbors (k-NN) ve Ölçeklenebilirlik Problemi

- **Exact Search (k-NN)**: Sorgu vektörünü veritabanındaki tüm vektörlerle tek tek karşılaştırır (Brute-force).
- **Dimensionality Curse & Scale Issue**: Vektör sayısı milyonlara veya milyarlara ulaştığında O(N⋅D)O(N \cdot D)O(N⋅D) zaman karmaşıklığı (NNN: vektör sayısı, DDD: boyut) nedeniyle k-NN çok yavaşlar ve bellek yetersiz kalır.
- **Çözüm: Approximate Nearest Neighbors (ANN)**: Yüzde yüz kesinlikten (100% accuracy) biraz ödün vererek **milisaniyeler içinde** arama yapmayı sağlayan yaklaşımdır.

## 3. Quantization (Nicemleme) Teknikleri

Bellek kullanımını azaltmak ve arama hızını artırmak için kullanılan en kritik tekniklerden biridir.

- **Scalar Quantization (SQ)**:

  - 32-bit floating point (`fp32`) değerlerini 8-bit integer (`int8`) gibi daha küçük veri tiplerine dönüştürür.
  - Bellek ayak izini (memory footprint) **4 kat** azaltır.
  - Arama sırasında vektörler dequantize edilir veya doğrudan integer seviyesinde hızlı SIMD talimatlarıyla hesaplanır.
- **Product Quantization (PQ)**:

  - High-dimensional (ör. 512 boyutlu) bir vektörü daha küçük **sub-vector**'lere (ör. 64 adet 8 boyutlu sub-vector) böler.
  - Her sub-space için K-Means clustering çalıştırılarak **centroids (küme merkezleri)** ve bir **Codebook** oluşturulur.
  - Orijinal vektörler artık float değerler olarak değil, centroid'lerin **index (ID)** değerleri olarak saklanır.
  - **Inverted File (IVF) + PQ**: Arama süresini k-NN'e kıyasla yüzlerce kat hızlandırır ve bellek tüketimini muazzam oranda düşürür.

## 4. Indexing & Graph-Based Structures

- **Inverted File Index (IVF)**:

  - Arama alanını Voronoi hücrelerine (Voronoi cells) böler.
  - Sorgu geldiğinde sadece en yakın birkaç küme (nprobe) içindeki vektörler taranır, tüm veritabanı taranmaz.
- **HNSW (Hierarchical Navigable Small World)**:

  - Graph-based bir ANN algoritmasıdır.
  - Skip-list veri yapısına benzer şekilde çok katmanlı (multi-layer) bir graf yapısı kurar. Üst katmanlarda uzun mesafeli atlamalar (expressways), alt katmanlarda hassas aramalar yapılır.
  - Yüksek **Recall** oranları ve ultra düşük **latency** sağlar, ancak bellek kullanımı (RAM footprint) Quantization yöntemlerine göre daha fazladır.

## 5. Pratik Mimari ve Uygulama Notları

- **Memory vs. Accuracy Trade-off**: VectorDB mimarisinde her zaman hız/bellek kullanımı ile doğruluk (Recall rate) arasında bir denge (trade-off) kurulmalıdır.
- **RAM Optimization**: Büyük ölçekli sistemlerde tüm vektörleri `fp32` olarak RAM'de tutmak maliyetli olduğu için **PQ + IVF** veya **DiskANN** gibi diski/RAM'i hibrit kullanan yapılar tercih edilir.

Videonun devam eden bölümlerinde bu anlatılan teorik altyapının (özellikle Quantization ve Codebook mantığının) C++ veya Rust/Python ile kodlama adımlarına geçilmektedir.

Detaylandırmak istediğin belirli bir kısım (örneğin Product Quantization matematiği veya HNSW yapısı) olursa daha da açabilirim!
