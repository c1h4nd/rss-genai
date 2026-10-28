# NQ Trading Seek & Destroy Profile Jackson Hole Symposium Day 1

<https://www.youtube.com/watch?v=SUcRywSry5U>

Bu YouTube videosunda (**"SUcRywSry5U"** - *Deep Learning / Neural Networks* temellerini ve mimarisini ele alan teknik anlatım) öne çıkan önemli konular ve detaylar şu şekildedir:

### 1. Neural Network Temelleri ve Perceptron

- **Perceptron Mantığı:** Yapay sinir ağlarının en temel yapı taşıdır. Girdileri (xix\_ixi​), ağırlıklar (wiw\_iwi​) ile çarparak toplar, bir **bias (bbb)** ekler ve çıkan sonucu bir aktivasyon fonksiyonundan geçirir (y=f(∑wixi+b)y = f(\sum w\_i x\_i + b)y=f(∑wi​xi​+b)).
- **Bias'ın Rolü:** Aktivasyon fonksiyonunu sağa/sola kaydırarak modelin veri üzerindeki esnekliğini ve öğrenme kapasitesini artırır.
- **Non-linearity (Doğrusal Olmayan Yapı):** Ağın sadece doğrusal ilişkileri değil, karmaşık ve çok katmanlı örüntüleri (patterns) öğrenebilmesi için aktivasyon fonksiyonları şarttır.

### 2. Aktivasyon Fonksiyonları (Activation Functions)

- **Sigmoid:** Çıktıyı `(0, 1)` aralığına sıkıştırır. Özellikle olasılık tahminlerinde veya ikili sınıflandırmada (binary classification) kullanılır. *Dezavantajı:* **Vanishing Gradient** (kaybolan türev) problemine yol açabilir.
- **ReLU (Rectified Linear Unit):** f(x)=max⁡(0,x)f(x) = \max(0, x)f(x)=max(0,x). Hesaplama açısından çok hızlıdır ve derin ağlarda en çok tercih edilen fonksiyondur. Pozitif değerlerde türev sabit kaldığı için Vanishing Gradient sorununu büyük oranda çözer.
- **Softmax:** Multi-class classification (çok sınıflı sınıflandırma) problemlerinde çıkış katmanında kullanılır; çıktıları toplamı 1 olan bir olasılık dağılımına dönüştürür.

### 3. İleri Besleme ve Hata Hesaplama (Forward Propagation & Loss)

- **Forward Pass:** Verinin giriş katmanından (input layer) başlayarak gizli katmanlar (hidden layers) boyunca ilerleyip çıkış katmanına (output layer) ulaşması ve tahmin üretmesidir.
- **Loss Function (Kayıp Fonksiyonu):** Modelin tahmini (y^\hat{y}y^​) ile gerçek hedef (yyy) arasındaki farkı/hatayı ölçer.

  - **MSE (Mean Squared Error):** Regression (bağıntı/sayısal tahmin) problemleri için.
  - **Cross-Entropy Loss:** Classification (sınıflandırma) problemleri için tercih edilir.

### 4. Geri Yayılım ve Optimizasyon (Backpropagation & Gradient Descent)

- **Backpropagation:** Modelin yaptığı hatayı çıkıştan girişe doğru geriye yayarak her bir ağırlığın (www) ve bias'ın (bbb) hatadaki payını (**Gradient / Türev**) hesaplama işlemidir. Bu adımda **Chain Rule (Zincir Kuralı)** kullanılır.
- **Gradient Descent (Eğim İnişi):** Ağın parametrelerini (weights) hatayı en aza indirecek şekilde güncelleme algoritmasıdır.

  - Güncelleme formülü mantığı: wnew=wold−(Learning Rate×Gradient)w\_{new} = w\_{old} - (\text{Learning Rate} \times \text{Gradient})wnew​=wold​−(Learning Rate×Gradient)
- **Learning Rate (η\etaη):** Modelin her adımda ne kadar büyük bir güncelleme yapacağını belirleyen hyperparameter'dır.

  - *Çok yüksek olursa:* Minimum noktayı atlayabilir (overshoot/divergence).
  - *Çok düşük olursa:* Öğrenme çok yavaş gerçekleşir ve local minima'ya takılabilir.

### 5. Eğitim Süreci ve Hyperparameters

- **Epoch:** Tüm veri setinin ağ üzerinden tam bir kez geçmesidir (bir forward + bir backward pass).
- **Batch Size:** Ağırlıkların güncellenmesi için bir kerede modele verilen veri örneği sayısı.

  - **SGD (Stochastic Gradient Descent):** Her veri örneğinde ağırlık günceller (gürültülü ama hızlı).
  - **Mini-batch Gradient Descent:** Veriyi küçük gruplar halinde işler (en yaygın ve dengeli yaklaşım).
- **Overfitting (Aşırı Öğrenme):** Modelin eğitim verisini ezberlemesi ve görmediği test verisinde başarısız olması durumudur.

  - *Çözümler:* **Dropout** (rastgele nöron kapatma), **L1/L2 Regularization** ve **Early Stopping**.
