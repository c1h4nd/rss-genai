# ICT Mentorship 2023 - Market Maker Models

<https://www.youtube.com/watch?v=iKsIbUblSWM>

Bu video (**ICT / Market Maker Models** konulu eğitim videosu), piyasa yapıcı modelleri (**Market Maker Models - MMM**) kullanarak işlem yapmanın (trading) detaylarını ve **PD Arrays** (Price Delivery Arrays) kavramını ele alıyor.

İşte videodaki tüm önemli noktaların detaylı ve maddelenmiş özeti:

## 1. Genel Yaklaşım ve Ön Koşullar

- **İleri Seviye Konsept:** Market Maker Model yöntemi yeni başlayanlar için ağır gelebilir; bu stratejiyi etkili kullanmak için temel **PD Array** yapılarına hakim olmak gerekir.
- **PD Array Mantığı:** Fiyat hareketindeki likidite (**Liquidity**), verimsizlikler (**Inefficiencies**) ve konsolidasyon alanlarını okuyabilmek için Order Block, Breaker, Fair Value Gap (FVG) gibi araçların bütünsel olarak anlaşılması gerekir.

## 2. Temel Yapı Taşları ve PD Arrays (Price Delivery Arrays)

- **Order Block (OB) & Breaker Block:** Piyasa yapıcının likiditeyi topladıktan sonra yön değiştirdiği ana kırılım ve tepki noktaları.
- **Fair Value Gap (FVG) & Inversion FVG:** Fiyatın hızlı hareket ettiği ve arkasında bıraktığı boşluklar/verimsizlikler. Fiyatın bu alanlara geri çekilerek (rebalance) dengelenmesi beklenir.
- **Mitigation Block:** Başarısız yeni en yüksek/en düşük seviyelerden sonra oluşan düzeltme alanları.
- **Liquidity Pools (Likidite Havuzları):** **Relative Equal Highs** (EQL) ve **Relative Equal Lows** (EQH) seviyelerinin altında veya üstünde biriken Stop-Loss emirleri piyasa yapıcı tarafından hedef alınır.

## 3. Market Maker Model (MMM) Mekaniği

- **Market Maker Buy/Sell Model:** Fiyat önce bir konsolidasyon ve birikim dönemi (**Accumulation**) geçirir, ardından manipülasyon (**Manipulation**) ile likiditeyi temizler ve ardından asıl trend yönünde dağıtım (**Distribution**) gerçekleşir.
- **Market Structure Shift (MSS):** Modelin teyit edilmesi için fiyatta belirgin bir yapı kırılımı (MSS) aranmalıdır.
- **Inefficiency Alignment:** Fiyatın dönüş noktalarında tek bir sinyal yerine birkaç farklı PD Array'in üst üste binmesi (**Confluence**) işlem başarısını artırır.

## 4. Uygulama, Tutarlılık ve Günlük Tutma (Journaling)

- **Trade Journaling:** İşlemleri detaylıca not etmek, grafikler üzerinde **PD Array**'leri işaretlemek ve analiz yapmak beynin bu kalıpları tanımasını kolaylaştırır.
- **Grafik Güncelleme & Notlandırma:** Başarılı ve başarısız tüm senaryoları kaydetmek, psikolojik dayanıklılığı artırır ve stratejiye olan güveni pekiştirir.

### Özetle İşlem Adımları (Key Takeaways):

1. **Likidite Seviyesini Belirle:** Grafikteki Likidite Havuzlarını (BSL - Buyside Liquidity / SSL - Sellside Liquidity) tespit et.
2. **Yapı Kırılımını Bekle:** Fiyat likiditeyi aldıktan sonra Market Structure Shift (MSS) gerçekleşmesini bekle.
3. **PD Array ile Giriş Ara:** FVG, Breaker veya Order Block bölgesine geri çekilmede giriş fırsatı değerlendir.
4. **Disiplinli Günlük Tut:** İşlem sonrası analizi Journal'ına kaydederek tecrübeni pekiştir.
