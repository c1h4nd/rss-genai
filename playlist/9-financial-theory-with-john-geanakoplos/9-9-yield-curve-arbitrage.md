# 9. Yield Curve Arbitrage

<https://www.youtube.com/watch?v=5SHYky2ddp4>

Yale Üniversitesi’nin Financial Markets (FINC 251) dersi kapsamındaki **"9. Yield Curve Arbitrage"** ders videosunun öne çıkan detaylı özeti aşağıda maddeler halinde verilmiştir:

### 1. **Yield (Verim) Kavramı ve Sınırları**

- **TANIM:** Yield, dış piyasa şartlarını gözetmeksizin yalnızca bir yatırımın kendi nakit akışlarına (cash flows) bakarak cazibesini tek bir sayı ile ölçme çabasıdır [[00:44](https://www.youtube.com/watch?v=5SHYky2ddp4&t=44)].
- **SORUNLARI:**

  - **Çoklu Çözüm (Ambiguity):** Cash flow yönlerinin değiştiği durumlarda (ör. 1,−4,31, -4, 31,−4,3), İç Verim Oranı (Internal Rate of Return / YTM) denkleminin 0%0\%0% ve 200%200\%200% gibi birden fazla matematiksel çözümü olabilir [[02:30](https://www.youtube.com/watch?v=5SHYky2ddp4&t=150)].
  - **Zamanlama Problemi:** Fonların faal olmadığı uzun boşluklarda, yüksek iskonto oranları nedeniyle erken dönemdeki nakit akışlarına aşırı duyarlılık oluşur [[04:09](https://www.youtube.com/watch?v=5SHYky2ddp4&t=249)].
- **Irving Fisher Yaklaşımı:** Bir yatırımı değerlendirirken sadece cash flow'lara bakıp piyasayı yok saymak yanlıştır. Enflasyondan arındırılmış nakit akışları, piyasada geçerli olan faiz oranları ile iskonto edilerek **Present Value (Bugünkü Değer)** hesaplanmalıdır [[05:45](https://www.youtube.com/watch?v=5SHYky2ddp4&t=345)].

### 2. **Yield Curve (Getiri Eğrisi) ve Piyasa Dinamikleri**

- **YIELDCURVE TÜRLERİ:**

  - **Flat Yield Curve:** Kısa ve uzun vadeli getiri oranlarının birbirine eşit veya çok yakın olduğu durumlar (ör. Aralık 2000 dönemi) [[08:37](https://www.youtube.com/watch?v=5SHYky2ddp4&t=517)].
  - **Upward Sloping Yield Curve:** Kısa vadeli oranların düşük, uzun vadeli oranların daha yüksek olduğu durumlar (ör. 2008 krizi sonrası ve 2009 dönemi) [[08:45](https://www.youtube.com/watch?v=5SHYky2ddp4&t=525)].
- **PİYASA BEKLENTİLERİ:** Uzun vadeli faizlerin kısa vadelilere göre belirgin şekilde yüksek olması iki temele dayanır:

  1. İleride **inflation** beklentisinin artması [[01:12:05](https://www.youtube.com/watch?v=5SHYky2ddp4&t=4325)].
  2. Ekonomik üretkenlik (productivity) artışı beklentisiyle **real interest rate**'in yükselmesi [[01:12:14](https://www.youtube.com/watch?v=5SHYky2ddp4&t=4334)].

### 3. **Zero-Coupon Bond Prices (πt\pi\_tπt​) ve Replikasyon**

- **Sıfır Kupon Fiyatı (πt\pi\_tπt​):** Bugün ödenerek ttt zamanında 1$1 \$1$ elde etmeyi sağlayan bugünkü para fiyatıdır [[16:58](https://www.youtube.com/watch?v=5SHYky2ddp4&t=1018)].
- **Replication (Replikasyon) Yöntemi:** Piyasa doğrudan Zero-Coupon Bond işlemleri sunmasa da, Benchmark Treasury kuponlu tahvillerinden portföyler oluşturularak bu akışlar taklit edilebilir [[25:28](https://www.youtube.com/watch?v=5SHYky2ddp4&t=1528)]:

  - **1 Yıllık Zero (π1\pi\_1π1​):** 1 yıllık kuponlu tahvilin ödemesine oranlanarak bulunur [[23:59](https://www.youtube.com/watch?v=5SHYky2ddp4&t=1439)].
  - **2 Yıllık Zero (π2\pi\_2π2​):** 2 yıllık kuponlu tahvilden uzun (long) pozisyon alıp, ilk yıl fazladan gelen kupon ödemesini netleştirmek için 1 yıllık tahvilde kısa (short) pozisyon alarak hesaplanır [[37:04](https://www.youtube.com/watch?v=5SHYky2ddp4&t=2224)].

### 4. **Arbitraj ve Duality (İkileme/Tersine Çözüm) İlkesi**

- **Arbitrage Profits:** Eğer piyasada bir Zero-Coupon varlık adil replikasyon fiyatından farklı bir fiyata (örneğin 91.7 cent yerine 93 cent) satılıyorsa; açığa satış ve replikasyon portföyü alma yoluyla **risksiz kar** kilitlenebilir [[43:24](https://www.youtube.com/watch?v=5SHYky2ddp4&t=2604)].
- **Matematiksel Çözüm (Duality Principle):** Karmaşık replikasyon portföy oranlarını tek tek türetmek yerine, kuponlu tahvillerin piyasa fiyatları ile bilinmeyen π\piπ parametreleri denklem sistemine dönüştürülür [[44:26](https://www.youtube.com/watch?v=5SHYky2ddp4&t=2666)]:

  Market Pricei=∑t=1nCashFlowt×πt\text{Market Price}\_i = \sum\_{t=1}^{n} \text{CashFlow}\_t \times \pi\_tMarket Pricei​=t=1∑n​CashFlowt​×πt​

  Excel matris/çözücü araçları veya doğrusal denklem sistemleri ile nnn bilinmeyenli nnn denklem çözülerek π1,π2,…,πn\pi\_1, \pi\_2, \dots, \pi\_nπ1​,π2​,…,πn​ doğrudan elde edilir [[47:30](https://www.youtube.com/watch?v=5SHYky2ddp4&t=2850)].

### 5. **Forward Interest Rates (Vadeli Faiz Oranları)**

- **TANIM:** Bugün anlaşılan ancak gelecekteki iki dönem arasında (ttt ile t+1t+1t+1) geçerli olacak vadeli faiz oranıdır (if,ti\_{f,t}if,t​) [[54:03](https://www.youtube.com/watch?v=5SHYky2ddp4&t=3243)].
- **HESAPLAMA:** Sıfır kupon fiyatlarının oranından türetilir [[55:13](https://www.youtube.com/watch?v=5SHYky2ddp4&t=3313)]:

  1+if,t=πtπt+11 + i\_{f,t} = \frac{\pi\_t}{\pi\_{t+1}}1+if,t​=πt+1​πt​​
- **FORWARD vs. YIELD EĞRİSİ İLİŞKİSİ:**

  - Getiri eğrisi yukarı yönlü (upward sloping) ise, **Forward Rate**'ler getiri eğrisine (Yield Curve) kıyasla çok daha dik ve hızlı yükselir [[01:01:17](https://www.youtube.com/watch?v=5SHYky2ddp4&t=3677)].
  - Bunun sebebi "ortalama" mantığıdır: Uzun vadeli ortalama verimi (Yield) yukarı çekebilmek için son dönemdeki marjinal faizin (Forward Rate) ortalamadan çok daha yüksek olması gerekir [[01:02:54](https://www.youtube.com/watch?v=5SHYky2ddp4&t=3774)].
- **Gelecek Tahmini (Expectations Theory):** Tam kesinlik (certainty) altındaki bir piyasada vadeli faiz oranları (ifi\_fif​), piyasa aktörlerinin gelecekte gerçekleşmesini kesin beklediği spot faiz oranlarının birebir karşılığıdır [[01:08:07](https://www.youtube.com/watch?v=5SHYky2ddp4&t=4087)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  9. Yield Curve Arbitrage

  YaleCourses · 100K views

   [Open in 9. Yield Curve Arbitrage](http://www.youtube.com/watch?v=5SHYky2ddp4)](http://www.youtube.com/watch?v=5SHYky2ddp4)

  ![](https://i.ytimg.com/vi/5SHYky2ddp4/hqdefault.jpg)
