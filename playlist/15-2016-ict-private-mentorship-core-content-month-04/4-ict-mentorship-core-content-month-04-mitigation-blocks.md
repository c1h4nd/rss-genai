# ICT Mentorship Core Content - Month 04 - Mitigation Blocks

<https://www.youtube.com/watch?v=FOUzW0QmsfI>

İstediğin YouTube videosu **ICT (Inner Circle Trader) Mentorship Core Content - Month 04: Mitigation Blocks** dersidir.

Konunun teknik yapısını ve detaylarını bozmamak adına orijinal İngilizce terimleri (`Order Block`, `Breaker`, `Failure Swing` vb.) koruyarak hazırladığım detaylı özet aşağıdadır:

## 1. Mitigation Block Nedir? (Temel Mantık)

- **Tanım:** Fiyatın eski bir salınım yükseğini/düşüğünü (swing high/low) **kıramayıp** başarsız olduğu (Failure Swing) durumlarda oluşan ve kurumsal oyuncuların (Smart Money) zararda kalan pozisyonlarını kapatmak/hafifletmek (`mitigate`) için kullandığı fiyat bölgesidir.
- **Breaker Block ile Temel Farkı:**

  - **Breaker Block:** Fiyat önce likiditeyi süpürür (yeni bir High veya Low yapar) ve ardından yapıyı sertçe kırar.
  - **Mitigation Block:** Fiyat likiditeyi süpürmede **başarısız olur** (yani yeni bir High veya Low yapamaz - *Failure Swing* oluşur), ardından piyasa yapısı kırılır.

## 2. Bearish Mitigation Block (Satış Yönlü Senaryo)

- **Oluşum Adımları:**

  1. Fiyat yukarı yönlü bir hareketle bir **Swing High** (Yüksek) oluşturur.
  2. Piyasa bir miktar geri çekilir (**Swing Low** yapar).
  3. Fiyat tekrar yukarı hamle yapar ancak önceki yüksek seviyeyi **geçemez** (*Failure Swing* / Lower High oluşur).
  4. Ardından fiyat sert bir düşüşle aradaki Swing Low seviyesini aşağı kırar (Market Structure Shift / MSS).
  5. **Mitigation Zone:** Bu sert düşüş öncesinde oluşan son yukarı yönlü mum(lar) (Up-close candle/range) bizim *Bearish Mitigation Block* bölgemiz olur.
- **İşlem Arayışı (Trade Execution):**

  - Fiyat kırılım sonrası tekrar yükselerek bu Mitigation Block seviyesine geri çekildiğinde (`Retrace / Test`) **Sell (Short)** yönlü işlem aranır.
  - **Amaç:** Yükseliş denemesinde terste kalan Smart Money / Kurumsal satıcılar bu noktada başabaş (breakeven) seviyesinde zararlarını kapatırlar veya yeni satış eklerler.

## 3. Bullish Mitigation Block (Alış Yönlü Senaryo)

- **Oluşum Adımları:**

  1. Fiyat aşağı yönlü bir düşüşle bir **Swing Low** (Düşük) oluşturur.
  2. Fiyat yukarı tepki verir (**Swing High** yapar).
  3. Fiyat tekrar aşağı düşer fakat önceki dip seviyesinin altına **inemez** (*Failure Swing* / Higher Low oluşur).
  4. Fiyat güçlü bir yükselişle aradaki Swing High seviyesini yukarı kırar.
  5. **Mitigation Zone:** Kırılım öncesindeki son aşağı yönlü mum(lar) (Down-close candle/range) *Bullish Mitigation Block* olarak işaretlenir.
- **İşlem Arayışı (Trade Execution):**

  - Fiyat tekrar bu bloğa doğru geri düştüğünde **Buy (Long)** yönlü işlem fırsatı verir.

## 4. Kritik Kurallar ve Püf Noktaları

- **Failure Swing Zorunluluğu:** Mitigation Block yapısının oluşması için Likidite Süpürme (*Liquidity Sweep*) olmaması gerekir. Eğer önceki High/Low kırılsaydı bu yapı Mitigation değil, **Breaker Block** olurdu.
- **Market Structure Shift (MSS):** Bloğun valide olması için fiyatın yapıyı net ve gövdeli bir mumla kırması (Displacement) şarttır.
- **Stop Loss Yerleşimi:**

  - *Bearish:* Stop Loss, Mitigation Block'un en yüksek iğnesinin (*High*) biraz üstüne konur.
  - *Bullish:* Stop Loss, Mitigation Block'un en düşük iğnesinin (*Low*) biraz altına konur.
- **Confluence (Kesişim) Faktörleri:** Mitigation Block tek başına kullanılmak yerine Fair Value Gap (FVG), Premium/Discount bölgeleri ve HTF (Higher Timeframe) Bias ile desteklendiğinde başarı oranı yükselir.
