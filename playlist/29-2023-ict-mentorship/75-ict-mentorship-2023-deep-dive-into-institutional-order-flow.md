# ICT Mentorship 2023 - Deep Dive Into Institutional Order Flow

<https://www.youtube.com/watch?v=vN2BkfyRWE4>

**ICT Mentorship 2023 - Deep Dive Into Institutional Order Flow** videosunun detaylı özetini aşağıda bulabilirsin.

İsteğin üzerine tüm teknik terimler, konsept isimleri ve jargon **orijinal İngilizce** haliyle korunmuştur.

## 1. What is Institutional Order Flow (IOF)?

- **Misconception of Order Flow:** ICT, *Depth of Market (DOM)*, *Level 2 data*, *Footprint charts* veya *Volume profile* verilerinin gerçek Institutional Order Flow olmadığını açıkça belirtir.
- **Spoofing Danger:** DOM ve Level 2 üzerindeki emirler/rakamlar piyasa yapıcılar tarafından yanıltıcı şekilde gösterilip silinebilir (*spoofing*).
- **True Definition of IOF:** Gerçek Institutional Order Flow, doğrudan fiyat grafiğinin kendisinde (*Price Action*), özellikle *Higher Timeframe (HTF)* üzerindeki delivery mekanizmasında okunur.
- **Algorithm-Driven:** Piyasa tamamen algoritma (IPDA) tarafından yönlendirilir. Fiyat tesadüfi hareket etmez; sürekli olarak *Liquidity Pool* veya *Inefficiency / Imbalance* arar.

## 2. Core Framework & Narrative Building

- **Top-Down Analysis:** Analiz her zaman HTF (Weekly, Daily, 4H) ile başlamalıdır.
- **Draw on Liquidity (DOL):** Fiyatın gitmek istediği ana hedef tespit edilmelidir. IOF mantığı, fiyatın bir sonraki aşamada *Buyside Liquidity (BSL)* mi yoksa *Sellside Liquidity (SSL)* mi hedeflediğini belirler.
- **Symmetry in Order Flow:** *Bullish Order Flow* ve *Bearish Order Flow* tamamen simetriktir; mantık her iki yönde de aynı çalışır.

  - **Bullish IOF:** Fiyat *Discount PD Arrays* seviyelerine çekilir (retrace eder) ve BSL / Premium seviyeleri hedefler.
  - **Bearish IOF:** Fiyat *Premium PD Arrays* seviyelerine yükselir ve SSL / Discount seviyeleri hedefler.

## 3. Key PD Arrays & Their Roles in Order Flow

- **Fair Value Gaps (FVG) & Displacement:**

  - Güçlü mum gövdeleriyle oluşan *Displacement*, algoritmik hevesi (*willingness*) gösterir.
  - FVG'ler emrin doldurulduğu (*rebalanced*) ana reaksiyon bölgeleridir.
- **Balanced Price Range (BPR):**

  - Çift taraflı (hem alış hem satış yönlü) FVG çakışmasıyla oluşan BPR, çok yüksek olasılıklı (*high-conviction*) bir konsepttir.
  - BPR bölgesine geri çekilmelerde ICT daha yüksek pozisyon büyüklüğü (*position sizing / leverage*) kullanılabileceğini vurgular.
- **Breaker Block vs. Mitigation Block Hierarchy:**

  - **Breaker Block:** Likidite alımı yaptıktan (*liquidity sweep*) sonra yapıyı kıran (*Market Structure Shift - MSS*) bloklardır. Breaker'lar çok daha güçlü bir *Support / Resistance* görevi görür.
  - **Mitigation Block:** Likidite alımı yapmadan gerçekleşen yapı kırılımlarıdır. Mitigation bloklar giriş için kullanılmaktan ziyade, fiyatın geçiş güzergahındaki ikincil hedefler (*mile markers*) olarak değerlendirilmelidir.
- **Inversion Fair Value Gap (IFVG):** Saygı duyulmayıp ihlal edilen (*violated*) bir FVG, ters yönde dinamik destek/direnç (IFVG) olarak çalışır.
- **Wicks and Tails:** Mum fitilleri algoritma tarafından boşluk (*gap*) olarak değerlendirilir. Fitilin orta noktası olan **Consequent Encroachment (CE)** önemli bir destek/direnç noktasıdır.

## 4. Execution & Model Rules

- **Where vs. When:**

  - *PD Arrays* fiyatın **nerede** (*WHERE*) tepki vereceğini söyler.
  - *Time & Macro Windows / Killzones* fiyatın **ne zaman** (*WHEN*) hareket edeceğini belirler.
- **Internal Range Liquidity (IRL) to External Range Liquidity (ERL):**

  - Fiyat yapısı her zaman IRL (FVG'ler, Imbalances) ile ERL (Old Highs / Old Lows) arasında salınım yapar.
  - Piyasa IRL'deki dengesizliği doldurduktan sonra ERL'deki likiditeyi süpürmeye gider.
- **SMT Divergence:** Korele olan enstrümanlar arasında (örneğin NQ ve ES / S&P500 ve Nasdaq) oluşan uyumsuzluklar (*SMT Divergence*), kurumsal emrin yönünü ve manipülasyonu doğrulamak için kullanılır.

## 5. Summary Takeaways

1. DOM veya Footprint verilerine bağımlı olmayın; bu veriler yanıltıcı olabilir.
2. İşlemlerinizi sadece indikatörlere göre değil, **HTF Bias + Draw on Liquidity + PD Array Alignment** üzerine kurduğunuz bir *Narrative* doğrultusunda alın.
3. Güçlü bir Institutional Order Flow akışında fiyat, yönündeki FVG ve Breaker'ları korur, karşı yöndeki yapıları ise ihlal eder (*Inversion*).
