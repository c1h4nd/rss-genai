# ICT Mentorship Core Content - Month 05 - Defining HTF PD Arrays

<https://www.youtube.com/watch?v=pwO-E-OOH5k>

Videoda (**ICT Mentorship Core Content - Month 05 - Defining HTF PD Arrays**) öne çıkan önemli noktalar ve kavramsal hiyerarşi detaylı olarak aşağıda listelenmiştir:

### 1. Temel Piyasa Algısı ve İki Ana Unsur

- **Piyasa Bakış Açısı:** Piyasa analiz edilirken zaman dilimi fark etmeksizin iki ana unsur öne çıkar: **Time (Zaman)** ve **Price (Fiyat)** [[00:35](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=35)], [[13:12](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=792)].
- **Algoritmanın Mantığı:** Borsa algoritması piyasayı "Aşırı Ucuz" (**Discount**) veya "Aşırı Pahalı" (**Premium**) olarak fiyatlandırır [[00:56](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=56)].
- **Denge Noktası (Equilibrium):** Bir *Trading Range* (fiyat aralığı) içinde en yüksek (Old High) ve en düşük (Old Low) seviyelerin tam orta noktası **Equilibrium** (denge) seviyesidir [[09:41](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=581)], [[18:06](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1086)].

  - *Equilibrium* üstü: **Premium** (Satış/Short aranacak veya Bullish hedeflerin alınacağı bölge) [[09:50](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=590)], [[29:57](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1797)].
  - *Equilibrium* altı: **Discount** (Alış/Long aranacak veya Bearish hedeflerin alınacağı bölge) [[09:55](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=595)], [[30:12](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1812)].

### 2. PD Array Hiyerarşisi (PD Array Hierarchy)

ICT, PD Array'leri karmaşık bir yapıdan çıkarıp fiyatın izleyeceği sıraya ve önem derecesine göre bir hiyerarşiye oturtur [[02:06](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=126)], [[24:00](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1440)].

#### **A. Premium PD Arrays (Yukarı Yönlü Fiyat Hareketinde Karşılaşılacak Sıra)**

Fiyat *Equilibrium* seviyesinden yukarı doğru hareket ederken karşılaştığı/test ettiği yapılar (en yakın yapıdan en uzaktakine doğru) [[24:15](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1455)]:

1. **Mitigation Block:** Yukarı harekette fiyatın ilk takılabileceği en düşük seviyedeki Premium yapıdır [[20:46](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1246)], [[24:27](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1467)].
2. **Bearish Breaker:** *Turtle Soup* veya likidite alımı sonrası oluşan kırılım yapısıdır. **Çok kritiktir:** Eğer grafikte güçlü bir Bearish Breaker varsa, fiyatın daha üstteki Fair Value Gap veya Bearish Order Block seviyelerine gitmesine izin vermez, fiyatı direkt aşağı bastırır [[21:19](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1279)], [[25:48](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1548)], [[26:46](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1606)].
3. **Liquidity Void:** Fiyatın hızlıca düştüğü ve boşluk bıraktığı alanlardır [[20:21](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1221)], [[21:56](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1316)].
4. **Fair Value Gap (FVG):** Fiyatın tek taraflı teslim edildiği (inefficiency) küçük gap alanlarıdır [[20:35](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1235)], [[22:00](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1320)].
5. **Bearish Order Block:** Derin Premium bölgesinde yer alan güçlü satış bloğudur [[20:40](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1240)], [[22:30](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1350)].
6. **Rejection Block:** Mum wicks/gölgeleri hariç, mum gövdelerinin (bodies) hemen üstünde yer alan likidite bölgesidir [[18:52](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1132)], [[23:06](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1386)].
7. **Old High / Old Low:** Premium bölgesinin en üst sınırıdır; eski bir tepe (Old High) veya geçmişte destek olmuş eski bir dip (Old Low) seviyesini temsil eder [[18:31](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1111)], [[23:23](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1403)].

#### **B. Discount PD Arrays (Aşağı Yönlü Fiyat Hareketinde Karşılaşılacak Sıra)**

Fiyat *Equilibrium* seviyesinden aşağı doğru düşerken test edeceği yapılar (en yakın yapıdan en uzaktakine doğru) [[27:39](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1659)]:

1. **Mitigation Block:** Düşüşte ilk karşılaşılacak alım desteği adayıdır [[27:07](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1627)], [[27:46](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1666)].
2. **Bullish Breaker:** İki dip arasındaki yükseliş mumudur. **Önemli kural:** Fiyat Bullish Breaker'a ulaştığında destek bulursa, daha alttaki *Liquidity Void* veya *FVG* doldurulmadan fiyat doğrudan yukarı dönebilir [[27:54](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1674)], [[28:21](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1701)].
3. **Liquidity Void:** Aşağı doğru oluşan verimsiz fiyat boşluklarıdır [[27:46](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1666)].
4. **Fair Value Gap (FVG):** Alt tarafta kalan dengesizlik alanlarıdır [[28:46](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1726)].
5. **Bullish Order Block:** Düşüşün tepki alacağı ana alıcı bloğudur [[28:59](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1739)].
6. **Rejection Block:** En dip mumların wick'leri hariç, gövdelerinin hemen altında kalan bölgedir [[29:04](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1744)].
7. **Old Low / Historic High:** Discount bölgesinin en derin noktasıdır; eski dip (Old Low) veya çok geçmişteki bir tepe seviyesidir [[29:22](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1762)].

### 3. Fiyat ve Zaman İlişkisi (Time & Price)

- **Zamanın Önemi:** İşleme girerken zaman unsuruna boyun eğmek gerekir (*Submit to time*). Bir kurgunun çalışması veya hedefe ulaşması için ne kadar zaman geçeceğini kesin olarak bilemeyiz [[12:51](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=771)], [[13:48](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=828)].
- **Fiyat Analizi:** İşlemdeyken veya analiz yaparken *Institutional Order Flow* (kurumsal emir akışı) takip edilerek fiyatın adımları incelenmelidir [[14:14](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=854)], [[15:50](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=950)]. Fiyat asla düz bir çizgi halinde hedefe gitmez; dalgalanarak ilerler [[14:38](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=878)].

### 4. Zaman Dilimleri ve Uygulama (HTF Context)

- **Zaman Dilimi Ayrımı:** Bu dersteki HTF (Higher Time Frame) analizleri **Monthly**, **Weekly** ve **Daily** grafiklerini kapsar [[06:34](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=394)], [[07:34](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=454)].
- **Makro Çerçeve:** Monthly ve Weekly grafikler piyasanın genel bağlamını (*context*) ve yönünü anlamak için kullanılır [[07:34](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=454)].
- **Tüm HTF'lerde Aynı Mantık:** Aynı PD Array hiyerarşisi ve öncelik sırası Monthly, Weekly ve Daily grafiklerinin tamamında birebir aynı mantıkla çalışır [[30:24](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1824)], [[31:22](https://www.youtube.com/watch?v=pwO-E-OOH5k&t=1882)].

  [![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

  ICT Mentorship Core Content - Month 05 - Defining HTF PD Arrays

  The Inner Circle Trader · 346K views

   [Open in ICT Mentorship Core Content - Month 05 - Defining HTF PD Arrays](http://www.youtube.com/watch?v=pwO-E-OOH5k)](http://www.youtube.com/watch?v=pwO-E-OOH5k)

  ![](https://i.ytimg.com/vi/pwO-E-OOH5k/maxresdefault.jpg)
