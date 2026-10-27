# 18. Modeling Mortgage Prepayments and Valuing Mortgages

<https://www.youtube.com/watch?v=qbEsK92KpQI>

YaleCourses kanalının **"18. Modeling Mortgage Prepayments and Valuing Mortgages"** (Mortgage Erken Ödemelerini Modelleme ve Mortgage Değerleme) başlıklı dersinde öne çıkan önemli konular detaylı olarak aşağıda listelenmiştir:

### 1. Mortgage'ın Tarihsel ve Temel Yapısı

- **Tarihsel Köken:** Mortgage kavramı yeni bir American icadı değildir; kökeni yaklaşık 3.800 yıl öncesine, Babil dönemine (kil tabletlere) dayanır. [[00:18](https://www.youtube.com/watch?v=qbEsK92KpQI&t=18)]
- **Temel Mekanizma:** Mortgage üç temel bileşene dayanır:

  1. İleriye dönük bir söz/taahhüt (promise), [[00:35](https://www.youtube.com/watch?v=qbEsK92KpQI&t=35)]
  2. Sözün teminatı olarak bir varlık (**collateral** - ev), [[00:40](https://www.youtube.com/watch?v=qbEsK92KpQI&t=40)]
  3. Evden taşınma veya koşulların değişmesi durumunda borcu erken kapatma/iptal etme seçeneği (**prepaying / refinancing option**). [[00:57](https://www.youtube.com/watch?v=qbEsK92KpQI&t=57)]

### 2. İptal / Erken Ödeme Seçeneği (Refinancing Option) ve İtfa (Amortization)

- **Amortizing Mortgage Yapısı:** Eski mortgage'larda sabit faiz ödenip en sonda anapara ödemesi (**balloon payment**) yapılırken, modern mortgage'larda her dönem eşit ödemeler (**level payments**) yapılır. [[02:14](https://www.youtube.com/watch?v=qbEsK92KpQI&t=134)]
- **Geri Ödeme Dinamiği:** Yıllık ödemenin faiz oranını aşan kısmı, kalan anapara bakiyesini (**remaining balance**) zamanla kademeli olarak düşürür. Bu durum borç vereni (**lender**) risk açısından zamanla daha güvenli hale getirir. [[03:07](https://www.youtube.com/watch?v=qbEsK92KpQI&t=187)]
- **Refinancing (Yeniden Yapılandırma) Opsiyonu:** Borçlu (**borrower**), kalan bakiyeyi kapatarak istediği zaman sözleşmeyi sonlandırabilir. Bu opsiyon mortgage'ın değerlemesini oldukça karmaşık ve finansal açıdan çekici kılar. [[03:21](https://www.youtube.com/watch?v=qbEsK92KpQI&t=201)]

### 3. Faiz Oranları Değişiminin Borçlu ve Alacaklıya Etkisi

- **Faiz Yükseldiğinde:** Yanlış bilinenin aksine borçlu için avantajlıdır. Ekonomide faizler (%12-%19 seviyelerine) yükselirken borçlu %8'den borçlanmaya devam eder ve parasını yüksek faizle değerlendirebilir. Borç veren ise zarar eder. [[04:15](https://www.youtube.com/watch?v=qbEsK92KpQI&t=255)]
- **Faiz Düştüğünde / Deflasyon:** Borçlu, borcun bugünkü değerindeki devasa artışla karşılaşmamak için kalan bakiyeyi erken ödeyerek (**prepay**) daha düşük faizden borçlanır ve riskini sınırlandırır (**protects downside**). [[05:22](https://www.youtube.com/watch?v=qbEsK92KpQI&t=322)]
- **Deflasyonun Ekonomiye Etkisi:** Irving Fisher'a göre Büyük Buhran'ın (Great Depression) bu kadar ağır geçmesinin ana sebeplerinden biri, girişimcilerin borçlu yakalanması ve deflasyonla birlikte ezilmeleridir. [[04:29](https://www.youtube.com/watch?v=qbEsK92KpQI&t=269)]

### 4. Bakiye Başına Değerleme (Dollar of Remaining Balance & Backward Induction)

- Borçlunun erken ödeme yapıp yapmayacağını modellemek için ağaç yapısı üzerinde geriye dönük tümevarım (**backward induction**) kullanılır. [[09:03](https://www.youtube.com/watch?v=qbEsK92KpQI&t=543)]
- 100 birimlik mutlak tutarlar yerine, kalan anapara bakiyesini 1$'a ölçekleyerek (**dollar of remaining balance**) hesaplama yapmak modellerde erken ödeme kararlarının alındığı düğümleri (**nodes**) net şekilde (değerin `1` olduğu yerler) tespit etmeyi kolaylaştırır. [[13:04](https://www.youtube.com/watch?v=qbEsK92KpQI&t=784)]

### 5. Rasyonellik Varsayımı ve Gerçek Dünya Verileri

- **Optimal Karar Alma:** Teorik olarak herkes rasyonel hareket etse, faizler düştüğü an tüm borçluların aynı anda erken ödeme yapması gerekirdi. [[17:56](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1076)]
- **Gerçek Piyasa Verileri (Historical Prepayments):**

  - Faiz düştüğünde (ör. 90'ların başındaki durgunlukta faiz indirimleri) erken ödemeler hızla artar. [[15:31](https://www.youtube.com/watch?v=qbEsK92KpQI&t=931)]
  - Ancak pratikte erken ödeme oranları hiçbir zaman %100'e ulaşmaz (genelde maksimum %60-%70 bandında kalır). [[26:16](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1576)]
  - Faizler yüksek olsa bile boşanma, taşınma gibi nedenlerle baseline %10 civarında bir erken ödeme her zaman devam eder. [[29:33](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1773)]
- **Bankaların Fiyatlaması:** Bankalar borçluların tam anlamıyla optimal/rasyonel davranmadığını bildikleri için opsiyonun teorik değerinden daha düşük faiz oranları sunabilmektedir. [[18:56](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1136)]

### 6. Erken Ödeme Modelleme Yaklaşımları (Prepayment Modeling)

- **Senaryo Bazlı Tahmin (Contingent Predictions / Scenario Trees):** Tek bir geleceğe dayalı sabit tahmin yapmak yetersizdir. Olası gelecek senaryolarını bir ağaç (**tree of possible futures**) şeklinde contingent (koşullara bağlı) modellemek şarttır. [[22:16](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1336)]
- **Geleneksel Toplu Veri Yaklaşımı (Aggregate Prepayment Function):** Faiz farkına dayalı eğriler uydurularak ekonometrik regresyonlar yapılır, ancak bu modeller borçlu profillerini göz ardı eder. [[25:31](https://www.youtube.com/watch?v=qbEsK92KpQI&t=1531)]
- **Olumsuz Seçilimin Tersi / Olumlu Seçilim (Favorable / Proverse Selection & Burnout):**

  - Havuzdan borçlular erken ödeme yaparak çıktığında, geride dikkat etmeyen, faiz takibi yapmayan veya işlem maliyeti yüksek olan kişiler kalır. [[34:44](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2084)]
  - Faizler tekrar yükselip eski seviyesine dönse dahi, geride kalan borçlu havuzu (**burned out pool**) borç veren/banka için başlangıçtakinden çok daha kârlı/değerli hale gelir. [[39:52](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2392)]

### 7. Ajan Tabanlı Model (Agent-Based Prepayment Model)

- Profesyonel hedge fonlarda tek bir toplu regresyon yerine **Agent-Based Model** kullanılır:

  - Borçlular iki ana parametre ile tanımlanır: **Alertness** (Dikkat/Farkındalık seviyesi) ve **Cost of Prepaying** (Erken ödeme işlem/fırsat maliyeti). [[42:41](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2561)]
  - Dikkat seviyesi yüksek ve maliyeti düşük ("Alert & Low Cost") rasyonel borçlular havuzdan hızla ayrılır. Geride dikkatsiz veya maliyeti yüksek borçlular kalır. [[43:14](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2594)]
  - İstatistiksel dağılımda sadece 4 parametre tanımlanarak binlerce mortgage havuzunun geçmiş ve gelecekteki davranışı son derece yüksek bir hassasiyetle tahmin edilebilir. [[44:42](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2682)]
- **Volatility Etkisi:** Volatillik (oynaklık) arttığında opsiyonun zaman değeri arttığı için rasyonel borçlular erken ödemeyi geciktirir (prepayments slow down). [[46:15](https://www.youtube.com/watch?v=qbEsK92KpQI&t=2775)]

### 8. Negatif Konveksite (Negative Convexity)

- Normal tahvillerde faizler düştükçe tahvilin değeri artan bir eğri çizer.
- Mortgage'larda ise faiz düştükçe borçluların erken ödeme opsiyonunu kullanma ihtimali arttığı için mortgage'ın değeri 100 seviyelerinde sınırlanır ya da borçluların tepki süresine göre önce 100'ün üzerine çıkıp aşırı düşük faizlerde tekrar 100'e çekilir.
- Bu durum mortgage portföylerinde **Negative Convexity** riskini ortaya çıkarır. [[54:02](https://www.youtube.com/watch?v=qbEsK92KpQI&t=3242)]

### 9. Dinamik Korunma (Dynamic Hedging)

- **Mesele:** Portföydeki risklerden korunmak için nihai sonucu (**final outcome**) değil, bir sonraki adımı / bir sonraki günü (**next day's outcome / mark-to-market**) hedge etmek gerekir. [[01:06:30](https://www.youtube.com/watch?v=qbEsK92KpQI&t=3990)]
- **World Series (Yankees vs Phillies) Örneği:**

  - Yanlış bilgiye sahip bir taraftara karşı kârlı bir bahis alındığında bile, riskten tamamen kaçınmak için diğer bahisçilerle tek tek maç bazında zıt pozisyonlar (**offsetting bets**) alınır. [[59:41](https://www.youtube.com/watch?v=qbEsK92KpQI&t=3581)]
  - Ağaç üzerindeki her bir düğümde kârı sabitleyecek (**lock in**) oranda dinamik adımlarla pozisyon ayarlanarak şans faktörü/risk sıfırlanır ve teorik kâr tamamen garantilenir. [[01:10:35](https://www.youtube.com/watch?v=qbEsK92KpQI&t=4235)]

    [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

    18. Modeling Mortgage Prepayments and Valuing Mortgages

    YaleCourses · 40K views

     [Open in 18. Modeling Mortgage Prepayments and Valuing Mortgages](http://www.youtube.com/watch?v=qbEsK92KpQI)](http://www.youtube.com/watch?v=qbEsK92KpQI)

    ![](https://i.ytimg.com/vi/qbEsK92KpQI/hqdefault.jpg)
