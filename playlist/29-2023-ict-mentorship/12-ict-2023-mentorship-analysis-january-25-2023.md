# ICT 2023 Mentorship Analysis \ January 25, 2023

<https://www.youtube.com/watch?v=HkiPAi1Mdu8>

Bu video, **Inner Circle Trader (ICT)** tarafından sunulan **"ICT 2023 Mentorship Analysis \ January 25, 2023"** dersidir. Videoda ağırlıklı olarak **ES (E-mini S&P 500)** piyasa analizi, **PD Array** kullanımı, **Fair Value Gap (FVG)** davranışları ve işlem yönetimi detaylandırılmaktadır.

### 1. Temel Konseptler & Analiz Çerçevesi

- **Market Structure & PD Arrays:** Fiyatın yönünü (Bias) belirlemek ve giriş noktaları bulmak için Higher Timeframe (HTF) seviyelerindeki PD Array'ler (FVG, Order Block, Liquidity Pool) esas alınır.
- **Consequent Encroachment (C.E.):** Bir Fair Value Gap (FVG) veya Imbalance bölgesinin tam orta noktasıdır (%50 seviyesi).

  - Fiyat C.E. seviyesine tepki verdiğinde, boşluğun tamamen dolmasını engelleyen algoritma bazlı güçlü bir destek/direnç işlevi görebilir.

### 2. Fair Value Gap (FVG) ve Inefficiency Yönetimi

- **Sıralı/Birden Fazla FVG Durumu:** Market Structure Shift (MSS) sonrası grafikte birden fazla FVG oluşursa, fiyatın hangi boşluktan döneceğini anlamak için C.E. ve çevre Market Structure gözlemlenmelidir.
- **Dolmayan Boşluklar (Gap Handling):** Fiyat bir FVG'nin C.E. seviyesine dokunup sertçe yön değiştirdiğinde bu, Institutional Order Flow'un aşırı güçlü olduğuna ve boşluğu tam kapatma ihtiyacı duymadığına işaret eder.

### 3. Order Block Kullanım Kuralları

- **Consecutive Candles (Arka Arkaya Gelen Mumlar):** Bir Order Block yapısını belirlerken, aynı yönde üst üste kapatan birden fazla mum tek bir blok/bölge olarak ele alınmalıdır.
- **Order Block Geçerliliği:** Fiyat Order Block bölgesine çekildiğinde, mum gövdelerinin (candle bodies) bu seviyeleri ihlal etmemesi (özellikle Mean Threshold / %50 seviyesini tutması) beklenir.

### 4. İşlem Yönetimi & Risk Disiplini

- **Mean Threshold & Risk Control:** Risk yönetimi yapılırken stop-loss ve entry seviyelerinde tolerans Payı FVG veya Order Block'un %50 noktalarına göre ayarlanmalıdır.
- **Time & Price Theory:** İşlem arayışlarında New York Kill Zone saat aralıklarına sadık kalınmalı, likidite alımları (Liquidity Sweeps) sonrası yapının onaylanması beklenmelidir.

*Not: İsteğinize uygun olarak ICT metodolojisindeki tüm teknik terimler (`Consequent Encroachment`, `PD Array`, `Order Block`, `Market Structure Shift`, `FVG` vb.) orijinal İngilizce halleriyle bırakılmıştır.*
