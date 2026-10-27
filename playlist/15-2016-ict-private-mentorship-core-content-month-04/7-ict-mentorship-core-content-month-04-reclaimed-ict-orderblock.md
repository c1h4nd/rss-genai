# ICT Mentorship Core Content - Month 04 - Reclaimed ICT Orderblock

<https://www.youtube.com/watch?v=X5pQjfkAUCI>

Videodaki (ICT Mentorship Core Content - Month 04 - Reclaimed ICT Orderblock) önemli noktalar ve teknik detaylar:

## 1. Temel Mantık ve Model Yapısı

- **Market Maker Models:** Fiyat hareketleri iki temel eğri üzerinden modellenir:

  - **Market Maker Buy Model (MMBM):** Fiyatın daha yüksek seviyelere gitmeden önce alt zaman dilimindeki veya ana destek seviyesine (Old High/Low, Bullish Orderblock, Fair Value Gap veya Liquidity Void) doğru geri çekilmesi [[00:54](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=54)].
  - **Market Maker Sell Model (MMSM):** Fiyatın aşağı düşmeden önce bir direnç seviyesine doğru yükselmesi [[06:32](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=392)].
- **Sell Side & Buy Side of the Curve:**

  - **Left Side (Sol Taraf):** Trendin oluştuğu ve Smart Money'nin pozisyon biriktirdiği (hedging) taraftır [[01:46](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=106)].
  - **Right Side (Sağ Taraf):** Ana dönüş gerçekleştikten sonra sol taraftaki yapılardan faydalanılarak yeni işleme girilen taraftır [[04:12](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=252)].

## 2. Reclaimed Orderblock Nedir?

- **Tanım:** Eğrinin sol tarafında (örneğin MMBM düşüşü sırasında) küçük yükseliş hareketlerinden (minor displacement) önce oluşmuş **eski mum/blok yapılarının**, fiyat sağ tarafa geçtiğinde tekrar kullanılmasıdır [[05:05](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=305)].
- **Kurumsal İşleyiş (Smart Money & Hedging):**

  - Kurumsal oyuncular büyük pozisyon büyüklükleri nedeniyle tek bir noktadan tüm emirleri giremezler [[02:06](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=126)].
  - Trendin tersi yönündeki küçük tepki hareketleri (minor displacements), kurumsalların önceden **hedging** yaparak kademeli pozisyon topladığını gösterir [[02:45](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=165)].
  - Fiyat ana dönüşü yaptıktan sonra (Buy Side of the Curve), bu eski hedging seviyelerine geri çekildiğinde bu bloklar **reclaimed** edilir ve yeni pozisyon açmak için kullanılır [[04:44](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=284)].

## 3. Reclaimed Bullish Orderblock (MMBM İçinde)

- **Nasıl Oluşur?**

  - Düşüş eğrisi (sell side of the curve) esnasında fiyat alt destek seviyesine inerken küçük tepki yükselişleri yapar [[02:32](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=152)].
  - Bu tepki yükselişlerinden hemen önceki **en son düşüş mumu (down candle)** bir Bullish Orderblock'tur [[03:36](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=216)].
- **İşlem Aşaması:**

  - Fiyat ana dip seviyesine ulaşıp yükselişe geçtiğinde (buy side of the curve), sol taraftaki bu eski düşüş mumlarına denk gelen seviyeleri hedefler [[04:25](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=265)].
  - Fiyat bu eski muma temas ettiğinde **recapitalization / reclaim** gerçekleşir ve yeni **Long** işlemler için fırsat verir [[05:11](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=311)].

## 4. Reclaimed Bearish Orderblock (MMSM İçinde)

- **Nasıl Oluşur?**

  - Yükseliş eğrisi (buy side of the curve) esnasında fiyat direnç seviyesine çıkarken küçük düşüş tepkileri verir [[06:58](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=418)].
  - Bu küçük düşüşlerden önceki **en son yükseliş mumu (up candle)** bir Bearish Orderblock yapısı oluşturur [[07:12](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=432)].
- **İşlem Aşaması:**

  - Fiyat zirveyi yapıp düşüş eğrisine (sell side of the curve) geçtiğinde, yukarı yönlü düzeltmelerde sol taraftaki eski **up candle** yapılarına temas eder [[08:21](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=501)].
  - Bu eski yükseliş mumları direnç görevi görerek **reclaimed** edilir ve yeni **Short** girişleri sağlar [[08:28](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=508)].

## 5. Grafikte Uygulama & Özet

- **Eşleşme İlkesi (Matching Up):** Grafiğin sol tarafında kalan ve displacement üreten bloklar ile sağ tarafındaki fiyat tepkileri birebir örtüşür (to the pip) [[04:58](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=298)], [[06:21](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=381)].
- **Perakende (Retail) Tuzaklar:** Sol taraftaki küçük tepkiler esnasında erken giren perakende tüccarlar genellikle stop olur; çünkü bu hareketler sadece kurumsal hedging amacıyla yapılmıştır [[03:15](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=195)].
- **Özet Mantık:** Yalnızca sağ tarafa geçildiğinde (curve reversal), sol taraftaki minor displacement oluşturan mumları işaretleyip fiyatın bu seviyeleri "reclaim" etmesini beklemek gerekir [[10:19](https://www.youtube.com/watch?v=X5pQjfkAUCI&t=619)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  ICT Mentorship Core Content - Month 04 - Reclaimed ICT Orderblock

  The Inner Circle Trader · 369K views

   [Open in ICT Mentorship Core Content - Month 04 - Reclaimed ICT Orderblock](http://www.youtube.com/watch?v=X5pQjfkAUCI)](http://www.youtube.com/watch?v=X5pQjfkAUCI)

  ![](https://i.ytimg.com/vi/X5pQjfkAUCI/maxresdefault.jpg)
