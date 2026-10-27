# ICT Mentorship Core Content - Month 04 - ICT Vacuum Block

<https://www.youtube.com/watch?v=shPGUz9pU-A>

Videoda (ICT Mentorship Core Content - Month 04 - **ICT Vacuum Block**) anlatılan temel ve detaylı konular maddeler halinde şu şekildedir:

### 1. **Vacuum Block Tanımı ve Oluşum Sebepleri**

- **Tanım:** Volatilitenin yüksek olduğu anlarda (**volatility event**) fiyatın iki mum arasında işlem görmeden (likidite olmadan) sıçraması/atlaması sonucu oluşan boşluklardır (**gap**).
- **Tetikleyici Etkenler:**

  - **Ekonomik Takvim Verileri:** NFP (Non-Farm Payroll), FOMC faiz kararları [[01:06](https://www.youtube.com/watch?v=shPGUz9pU-A&t=66)].
  - **Piyasa Açılışları:** Vadeli işlem (Futures) veya hisse senedi/endeks piyasalarının seans açılışları [[01:06](https://www.youtube.com/watch?v=shPGUz9pU-A&t=66)].
  - **Beklenmeyen Olaylar:** Jeopolitik şoklar veya takvimde olmayan anlık gelişmeler [[01:56](https://www.youtube.com/watch?v=shPGUz9pU-A&t=116)].
- **Mekanizma:** Merkez bankaları / kurumsal seviyede hızlı fiyat güncellenmesi (**repricing**) gerçekleştiği için iki fiyat seviyesi arasında işlem gerçekleşmez; bu durum bir **liquidity vacuum** (likidite vakumu) oluşturur [[04:28](https://www.youtube.com/watch?v=shPGUz9pU-A&t=268)].

### 2. **Fiyatın Boşluğa Yaklaşımı ve Beklentiler**

- Çoğu perakende tüccar (retail trader) gap oluştuğunda fiyatın hemen o yönde akıp gideceğini varsayar [[02:21](https://www.youtube.com/watch?v=shPGUz9pU-A&t=141)].
- AncakBu video, **AI agent'lar (yapay zeka ajanları)** geliştirirken karşılaşılan zorluklar, tasarım kalıpları ve en iyi uygulama yöntemleri (best practices) üzerine harika bir özet sunuyor.

Videonun en önemli ve öne çıkan noktalarını detaylı bir şekilde aşağıda bulabilirsin:

## 1. Agent vs. Chain (Ajan ve Zincir Farkı)

- **Deterministic vs. Non-deterministic:** Klasik **Chains** (zincirler) belirli bir rotayı izleyen (hard-coded) adımlardan oluşurken, **Agents** durum bazlı kararlar vererek dinamik bir rotada ilerler.
- **Control Loop (Kontrol Döngüsü):** Bir agent'ın temel mekanizması; ortamı gözlemleme (*observe*), karar verme (*plan/reason*) ve eylem gerçekleştirme (*act*) döngüsüne dayanır.

## 2. Temel Mimari Bileşenler (Core Architecture)

- **Planning (Planlama):**

  - **ReAct (Reason + Act):** Agent'ın adım adım düşünüp hareket etmesini sağlayan temel prompting/logic pattern'ı.
  - **Plan-and-Execute:** Karmaşık görevleri önce küçük alt görevlere (sub-tasks) bölen, ardından bunları sırayla çalıştıran yapı.
- **Memory (Hafıza Yapısı):**

  - **Short-term Memory:** Konuşma geçmişi (Chat History) veya anlık execution context'i.
  - **Long-term Memory:** Vector database'ler (RAG) veya harici veritabanları kullanarak geçmiş etkileşimleri ve bilgileri saklama.
- **Tools (Araç Kullanımı):**

  - Agent'ların dış dünyayla etkileşime girmesini sağlayan API'lar, Python interpreter'ları veya arama motorları.
  - Tool tanımlarının (descriptions) açık venet olması, LLM'in doğru aracı seçmesi açısından kritiktir.

## 3. Production'a Geçerken Karşılaşılan Zorluklar

- **Looping & Hallucination:** Agent'ların sonsuz döngüye girmesi (aynı tool'u sürekli çağırması) veya yanlış tool parameter'ları üretmesi.
- **Latency (Gecikme):** Çözüm için birden fazla LLM çağrısı (multi-step reasoning) gerektiğinden yanıt sürelerinin uzaması.
- **Cost (Maliyet):** Her bir eylem adımında ve genişleyen context window nedeniyle token tüketiminin katlanması.

## 4. Best Practices & Çözüm Önerileri

- **Human-in-the-Loop (HITL):** Kritik eylemlerde (örneğin mail gönderme, veritabanı silme/güncelleme) agent'ın insan onayına sunulması breakpoint'leri eklemek.
- **Structured Output:** LLM çıktılarını JSON veya Pydantic modelleri ile kısıtlayarak (function calling / tool calling) hata oranını düşürmek.
- **State Management:** Agent'ın durumunu (State) merkezi bir yerde tutmak ve gerektiğinde geçmiş adımlara geri dönebilmek (*Time Travel / Checkpointing*).
- **Multi-Agent Systems:** Tek bir süper agent oluşturmak yerine, belirli uzmanlık alanları olan küçük agent'ların (örneğin: *Researcher*, *Coder*, *Reviewer*) bir orkestrasyon içinde birlikte çalışması.

Videonun odaklandığı belirli bir framework (LangGraph, AutoGen, CrewAI vb.) veya teknik detay hakkında daha derinlemesine bir analiz istersen yardımcı olmaktan mutluluk duyarım!

[![](https://www.gstatic.com/images/branding/productlogos/youtube/v9/192px.svg)

ICT Mentorship Core Content - Month 04 - ICT Vacuum Block

The Inner Circle Trader · 271K views

 [Open in ICT Mentorship Core Content - Month 04 - ICT Vacuum Block](http://www.youtube.com/watch?v=shPGUz9pU-A)](http://www.youtube.com/watch?v=shPGUz9pU-A)

![](https://i.ytimg.com/vi/shPGUz9pU-A/maxresdefault.jpg)
