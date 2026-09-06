---
layout: default
title: "Horizon Summary: 2026-09-06 (EN)"
date: 2026-09-06
lang: en
---

> From 143 items, 18 important content pieces were selected

---

**Technology News**
1. [Language Models Can Declare Their Own Attention Regions](#item-tech-news-1) ⭐️ 8.0/10
2. [SGLang v0.5.19 Adds Qwen3.8 Support, Beam Search, and AMD Optimizations](#item-tech-news-2) ⭐️ 7.0/10
3. [Nvidia PAIR Software Turns Idle Home PCs into Local AI Cluster](#item-tech-news-3) ⭐️ 7.0/10

**Financial News**
1. [Middle East Conflict Forces Rewrite of Oil Trade Routes](#item-finance-news-1) ⭐️ 9.0/10
2. [Japan and U.S. advance reported $550 billion AI and chip investment pact](#item-finance-news-2) ⭐️ 9.0/10
3. [Anthropic Delays IPO Roadshow to Mid-October, Prospectus to Late September](#item-finance-news-3) ⭐️ 8.0/10
4. [U.S.-Iran Attacks Rattle Dow Futures; Chip Stocks Signal Buys](#item-finance-news-4) ⭐️ 8.0/10
5. [AMD Reportedly Commits Up to $5B to Anthropic as IPO Filing Nears](#item-finance-news-5) ⭐️ 8.0/10
6. [Strong August Jobs Report Sends Government Bond Yields Higher](#item-finance-news-6) ⭐️ 8.0/10
7. [Cooler Inflation Data May Keep Warsh&\#x27;s Fed From Moving Rates, Reuters Reports](#item-finance-news-7) ⭐️ 8.0/10
8. [Federal Reserve Holds Rates Steady, Signals Possible Hike](#item-finance-news-8) ⭐️ 8.0/10
9. [US Federal Reserve Holds Rates Steady Under New Chair Warsh](#item-finance-news-9) ⭐️ 8.0/10
10. [Federal Reserve holds rates steady amid fresh inflation concerns](#item-finance-news-10) ⭐️ 8.0/10
11. [Fed&\#x27;s preferred inflation gauge rises at fastest pace in 3 years](#item-finance-news-11) ⭐️ 8.0/10
12. [US, Japan, and South Korea Sign Nuclear Cooperation Deal on Small Reactors](#item-finance-news-12) ⭐️ 7.0/10
13. [U.S. Army’s $2.2 Billion Microreactor Plan Targets 2028 Deployment](#item-finance-news-13) ⭐️ 7.0/10
14. [Anthropic Reportedly Plans IPO Valuing It Up to $2 Trillion](#item-finance-news-14) ⭐️ 7.0/10
15. [US Auto Alliance Urges Permanent Ban on Chinese Connected Vehicles and Software](#item-finance-news-15) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Language Models Can Declare Their Own Attention Regions](https://www.reddit.com/r/MachineLearning/comments/1w7sgf3/language_models_can_control_their_own_attention_r/) ⭐️ 8.0/10

The paper introduces Declarative Attention \(DA\), a protocol that lets language models declare which parts of the context they need to attend to by outputting &lt;global&gt;, &lt;focus&gt;, or &lt;local&gt; markers in their chain-of-thought, so the inference engine can skip most of the KV cache read. Across zero-shot evaluation on 15 long-context tasks, DA applied to off-the-shelf Gemma-4-31B and Qwen-3.6-27B reduced total attended tokens during decoding by 52.0% and 31.1%, respectively, with modest accuracy drops of 1.27 and 2.75 percentage points that shrink as model scale increases. Because the model itself declares the needed attention region instead of relying on external proxy scoring, DA offers an intrinsic alternative to prior sparse-attention methods that still require O\(N\) scoring per step. The authors frame DA as a new axis of sparse attention with additional potential under future training-based approaches.

reddit · r/MachineLearning · /u/eigenlaplace · Sep 5, 06:07

**「Background」** Modern long-context language models typically attend over every cached key and value token, meaning each generated token requires scanning the entire KV cache even when only a small portion of the context is relevant. Existing sparse-attention methods try to reduce this cost by pre-selecting relevant tokens with lightweight proxy scores, but such extrinsic scoring still incurs O\(N\) work per step. Declarative Attention instead makes the model state its attention focus directly as part of its generated output.

**「Impact」** Developers and researchers working on long-context LLM inference can use Declarative Attention to reduce KV-cache reads by more than half on off-the-shelf models while accepting controlled accuracy trade-offs, with the trade-off improving at larger model scales.

**Tags**: `#attention-mechanisms`, `#LLM-inference`, `#KV-cache`, `#efficiency`, `#machine-learning-research`

---

<a id="item-tech-news-2"></a>
### [SGLang v0.5.19 Adds Qwen3.8 Support, Beam Search, and AMD Optimizations](https://github.com/sgl-project/sglang/releases/tag/v0.5.19) ⭐️ 7.0/10

SGLang v0.5.19 was released with 786 pull requests from 214 contributors, adding support for multiple new models including Qwen3.8, Qwen3.8-27B, Ling-3.0-flash, Ling-3.0-tiny, Granite 4.2, and the diffusion models LongCat-Image-Edit and Edit-Turbo. The release introduces native beam search through a beam\_width request parameter, which returns the n best sequences and works alongside regular requests but not with speculative decoding, disaggregation, DP attention, or HiCache. New performance features include DeepEP v2&\#x27;s ElasticBuffer engine for DeepSeek-V3/V4 and Qwen3-MoE in FP8, layer norm sequence parallelism that reduces Qwen3-8B prefill time by 3.5% on H100 and 5.6% on B200, W4A8 MoE quantization on Hopper that boosts DeepSeek-V4-Flash output throughput by about 12%, and persistent Lean attention kernels on AMD MI300X and MI355X with up to 1.52x more throughput and up to 3.62x lower inter-token latency. The release also updates dependencies to FlashInfer 0.6.18, sgl-deep-ep 0.1.2, sgl-deep-gemm 0.1.7, and mooncake 0.3.13, while making the unified radix tree the default cache for all models.

github · Qiaolin-Yu · Sep 5, 02:27

**「What is SGLang?」** SGLang is an open-source, high-performance serving framework for large language models and multimodal models, designed for low-latency and high-throughput inference from a single GPU to large distributed clusters. It uses optimizations such as RadixAttention and continuous batching to handle requests efficiently. This release, v0.5.19, is one of the project&\#x27;s periodic versioned updates, and its highlights include support for new models and inference improvements across several backends.

**「Impact」** Developers using SGLang v0.5.19 gain native beam search for sequence generation, can deploy newly supported models such as Qwen3.8 and Ling-3.0, and can benefit from notable throughput and latency improvements on Blackwell GPUs, Hopper GPUs, and AMD MI355X accelerators.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl - project / sglang : SGLang is a high-performance serving...</a></li>
<li><a href="https://www.sglang.io/">SGLang – Fast, Open-Source LLM &amp; Multimodal Serving Framework</a></li>
<li><a href="https://mintlify.wiki/sgl-project/sglang/introduction">SGLang documentation - SGLang</a></li>

</ul>
</details>

**Tags**: `#SGLang`, `#LLM inference`, `#open source`, `#Qwen3.8`, `#model support`

---

<a id="item-tech-news-3"></a>
### [Nvidia PAIR Software Turns Idle Home PCs into Local AI Cluster](https://www.techspot.com/news/113742-nvidia-pair-software-turns-idle-home-computers-local.html) ⭐️ 7.0/10

Nvidia has released open-source software called PAIR \(Personal AI Router\) that lets users combine idle home computers, including GeForce RTX GPUs, DGX Spark systems, and Macs, into a local AI cluster without requiring special cabling and with setup completed in minutes. The software supports inference backends such as Ollama and LM Studio, and it keeps data and queries on the local network to preserve privacy. Nvidia claims the approach can mobilize roughly 165 teraFLOPS of otherwise idle household compute. This development matters because it provides an accessible, privacy-preserving way to boost local AI inference capacity for practitioners and hobbyists by aggregating consumer hardware they already own.

telegram · zaihuapd · Sep 5, 02:55

**「Background」** Running large models locally often hits the limits of one PC&\#x27;s GPU memory and compute, so advanced users have looked for ways to pool machines. NVIDIA&\#x27;s new open-source PAIR \(Personal AI Router\) tool, announced as a free beta, lets compatible computers on the same home network share idle processing power for local AI inference and agentic workloads, including GeForce RTX GPUs, DGX Spark systems, and Macs. It works with inference backends such as Ollama and LM Studio, requires no special cabling, and, according to NVIDIA, can draw on roughly 165 teraFLOPS of idle home compute while keeping queries on the local network.

**「Impact」** PAIR allows owners of GeForce RTX PCs, DGX Spark systems, and Macs to combine idle home compute into a private local AI inference cluster, making it easier for hobbyists and developers to run Ollama, LM Studio, and similar backends without sending data outside their home network and without special cabling. NVIDIA says this can marshal roughly 165 teraFLOPS of otherwise idle residential compute, and because the software is free and open source, it lowers the barrier to local AI experimentation; however, its beta status means features and stability may still evolve.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/113742-nvidia-pair-software-turns-idle-home-computers-local.html">Nvidia &#x27;s PAIR software turns idle home computers into a local AI ...</a></li>
<li><a href="https://www.expresscomputer.in/news/nvidias-free-pair-tool-turns-idle-home-pcs-into-a-personal-ai-cluster/138446/">Nvidia &#x27;s free PAIR tool turns idle home PCs into a personal AI cluster</a></li>
<li><a href="https://www.nvidia.com/en-eu/ai-on-rtx/personal-ai-router/">Personal AI Router for Local Inference | NVIDIA PAIR</a></li>
<li><a href="https://au.pcmag.com/ai/119713/nvidia-wants-to-turn-your-idle-pcs-into-a-personal-home-data-center-with-pair">Nvidia Wants to Turn Your Idle PCs Into a Personal Home Data...</a></li>
<li><a href="https://wccftech.com/nvidia-pair-turns-your-idle-home-pcs-into-a-local-ai-cluster/">NVIDIA PAIR Turns Your Idle Home PCs Into A Local AI Cluster...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Local AI`, `#Open Source`, `#AI Infrastructure`, `#GPU Clustering`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Middle East Conflict Forces Rewrite of Oil Trade Routes](https://oilprice.com/Energy/Crude-Oil/Iran-War-Forces-a-Rewrite-of-Global-Oil-Trade-Routes.html) ⭐️ 9.0/10

The Middle East war is forcing a rewrite of global oil and gas trade routes as daily crude flows through the Strait of Hormuz fall from close to 20 million barrels before U.S. and Israeli strikes on Iran to an estimated 6–8 million barrels, Oilprice.com reports. The disruption has added roughly $330 billion to the expected global energy import bill for March–August and is pushing importers such as Japan toward costlier alternative suppliers.

rss · OilPrice.com · Sep 5, 23:00

**「Background」** The Strait of Hormuz is a narrow waterway that carried one of the world&\#x27;s largest volumes of oil and LNG exports before the strikes. Qatar, the region&\#x27;s biggest LNG producer, has declared force majeure after damage to its Ras Laffan hub, while Saudi Arabia and the UAE are using alternative pipelines and ports that have limited capacity.

**「Impact」** Energy importers that relied on short Persian Gulf routes are now paying more because substitute suppliers are farther away. Japan, which got nearly all its crude from the Middle East before the war, saw its monthly import bill hit a record $76.39 billion in July as it turned to the U.S., Canada, African producers, and Azerbaijan.

**Tags**: `#Oil Trade Routes`, `#Middle East Conflict`, `#Energy Security`, `#Crude Oil Prices`, `#Strait of Hormuz`

---

<a id="item-finance-news-2"></a>
### [Japan and U.S. advance reported $550 billion AI and chip investment pact](https://finance.yahoo.com/technology/ai/articles/japan-u-advance-550-billion-040214374.html) ⭐️ 9.0/10

Japan and the United States are moving forward on a bilateral investment pact reported at $550 billion, with a focus on artificial intelligence and semiconductors.

openbb · NVDA · Sep 5, 04:02

**「Background」** Japan and the U.S. are moving forward on a previously announced $550 billion bilateral investment pact, and Japanese Trade Minister Ryosei Akazawa said discussions on artificial intelligence and semiconductor projects will carry very significant weight in the next round of projects under the agreement.

**「Impact」** Companies and investors in AI, semiconductors, and critical-mineral supply chains could face new cross-border investment and future trade or tariff negotiations as Japan and the U.S. advance the pact.

<details><summary>References</summary>
<ul>
<li><a href="https://au.finance.yahoo.com/news/japan-u-advance-550-billion-040611431.html">Japan , U . S . advance $ 550 billion investment pact with AI , chips in...</a></li>
<li><a href="https://thenextweb.com/news/japan-550-billion-us-investment-pact-ai-chips-third-tranche-eu-turnberry-600-billion-40-billion-us-ai-chips-gigafactories">Japan says progress made on $ 550 B pact , with AI and chips weighing...</a></li>
<li><a href="https://thefinrate.com/japan-reports-progress-on-550-billion-usinvestment-pact-as-ai-and-chips-take-center-stage/">Japan $550 Billion Investment Pact With US Makes Progress</a></li>

</ul>
</details>

**Tags**: `#Japan`, `#United States`, `#investment pact`, `#artificial intelligence`, `#semiconductors`

---

<a id="item-finance-news-3"></a>
### [Anthropic Delays IPO Roadshow to Mid-October, Prospectus to Late September](https://www.reuters.com/world/anthropic-ipo-launch-shifts-toward-mid-october-sources-say-2026-09-04/) ⭐️ 8.0/10

Anthropic has delayed its IPO roadshow to around mid-October and its public prospectus to late September, people familiar with the matter said, after the filing had been expected as early as next week. Some investors expect a potential valuation of about $2 trillion, and Anthropic is finalizing a $15 billion revolving credit facility with banks including Morgan Stanley, Goldman Sachs, JPMorgan and Citi; plans could still change.

telegram · zaihuapd · Sep 5, 15:05

**「Background」** Anthropic is an artificial-intelligence company preparing a stock-market listing ahead of the November U.S. midterm elections; an IPO roadshow is the period when executives market the offering to investors, and a prospectus is the public filing that discloses details of the shares being sold.

**Tags**: `#Anthropic`, `#IPO`, `#AI`, `#Credit Facility`, `#Capital Markets`

---

<a id="item-finance-news-4"></a>
### [U.S.-Iran Attacks Rattle Dow Futures; Chip Stocks Signal Buys](https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-nvidia-micron-sandisk-buy-signals-apple-inflation-reports/?src=A00220&amp;yptr=yahoo) ⭐️ 8.0/10

A market report says the U.S. and Iran exchanged attacks, which affected Dow Jones futures, and that Nvidia, Micron, and Sandisk flashed technical buy signals ahead of upcoming Apple and inflation reports.

openbb · NVDA · Sep 5, 18:22

**「Background」** The market backdrop is renewed U.S.-Iran hostilities: after the two sides exchanged attacks for the first time in weeks, crude oil prices jumped and Dow Jones, S&amp;P 500, and Nasdaq futures moved lower early Monday.

**「Impact」** AI-driven memory-cost inflation has begun to hit Apple: analysts cited by CNBC expect the pressure to persist for several more quarters, and Apple has raised prices on iPads and laptops to offset higher costs, directly affecting Apple consumers and shareholders.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-microsoft-titans-mask-market-weakness/">Dow Jones Futures Fall, Oil Prices Jump As U.S., Iran ...</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/aapl-stock-downgrade-wall-street-memory-inflation-pressures-several-quarters/cZo5nX1RJEH">AAPL Stock Gets Downgrades As Wall Street Sees Memory Inflation Pressures Persisting For &#x27;Several More Quarters&#x27;</a></li>
<li><a href="https://www.cnbc.com/2026/08/04/apple-shares-downgraded-due-to-memory-chip-inflation.html">Apple shares downgraded due to memory chip inflation</a></li>
<li><a href="https://www.nbcnews.com/business/consumer/apple-stock-ipad-macbook-price-hikes-rcna351786">Apple’s shares plunge after it hikes prices on iPads and laptops</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#stock futures`, `#Nvidia`, `#Micron`, `#technical analysis`

---

<a id="item-finance-news-5"></a>
### [AMD Reportedly Commits Up to $5B to Anthropic as IPO Filing Nears](https://finance.yahoo.com/technology/ai/articles/amd-committed-5-billion-anthropic-220301412.html) ⭐️ 8.0/10

AMD has reportedly committed up to $5 billion to Anthropic, an AI company whose IPO prospectus is reportedly expected to be filed within days. The figure is an unconfirmed reported commitment, not a confirmed transaction.

openbb · NVDA · Sep 5, 22:03

**「Background」** In late July 2026, AMD announced a partnership to invest up to $5 billion in Anthropic, with Anthropic also agreeing to deploy up to 2 gigawatts of AMD&\#x27;s Instinct MI450 AI GPUs. AMD&\#x27;s latest quarterly filing reportedly describes the commitments as subject to contingencies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/09/05/amd-committed-up-to-usd5-billion-to-anthropic-and-anthropic-s-ipo-prospectus-is-reportedly-days-away/">AMD Committed Up to $5 Billion to Anthropic, and Anthropic&#x27;s IPO Prospectus Is Reportedly Days Away | The Motley Fool</a></li>
<li><a href="https://www.cnbc.com/2026/07/22/amd-anthropic-ai-chip-investment.html">AMD to invest up to $5 billion in Anthropic as part of computing power deal</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#Anthropic`, `#IPO`, `#Artificial Intelligence`, `#Investment`

---

<a id="item-finance-news-6"></a>
### [Strong August Jobs Report Sends Government Bond Yields Higher](https://news.google.com/rss/articles/CBMimwFBVV95cUxNdTJNUkhrZnFtcjZwZmtHcGNSYTBCNkZKZFBlUy1IS3BiTlhBYzRNSm1VRWlLRFhHdmVjUEt4ajZmWFRHOGUzWHBKeFhWSlllYzdoc3g3dmFDVFpfLXQ5d19GRmtiT2UtT0gyV0d1cnpaQmY4RElYZzBBY0pfY2I5Q01HRjhxak1pOHo2c0JiUlJIWmdiX0NZX3Z1Zw?oc=5) ⭐️ 8.0/10

According to Reuters, a strong August U.S. jobs report pushed government bond yields higher, as investors responded to the better-than-expected labor market data.

google\_news · Reuters · Sep 4, 13:41

**「Background」** Government bond yields rise when investors expect the Federal Reserve to keep interest rates higher. The August jobs report showed U.S. job growth accelerated sharply while the unemployment rate held at 4.1%, suggesting a stable labor market and leaving the possibility of a Fed rate hike this month on the table.

<details><summary>References</summary>
<ul>
<li><a href="https://wtvbam.com/2026/09/04/strong-august-jobs-report-sends-yields-higher/">Strong August jobs report sends yields higher | WTVB | 1590 AM · 95.5 FM | The Voice of Branch County</a></li>

</ul>
</details>

**Tags**: `#jobs report`, `#yields`, `#economic data`, `#Federal Reserve`, `#markets`

---

<a id="item-finance-news-7"></a>
### [Cooler Inflation Data May Keep Warsh&\#x27;s Fed From Moving Rates, Reuters Reports](https://news.google.com/rss/articles/CBMisAFBVV95cUxQbDJaOWp0UVZZRVd3MUp5UGNUVk1EOXNybWFfeXRKR2FQYzJsUnJCN3VEU1I2bldJWHFodHlUWXQxcUdzXzVtaTN4RmEyaHlwREhvdVpialZycTYyaFozME5kWWV3MGFqT1hGS00zTnMyQmVDZkZXZTFvT0VGR0RSMU1FMnBiT3dyZFlSQmx5RDRXX0JsZ1dPMy1KOTNteGVOaVJRemdUaDhtWkpmRndEeQ?oc=5) ⭐️ 8.0/10

Reuters reports that cooler inflation data may push the divided Federal Reserve led by Kevin Warsh to leave interest rates unchanged, rather than raising or lowering them.

google\_news · Reuters · Aug 14, 07:00

**「Background」** Kevin Warsh became Federal Reserve chair in May with officials split over whether more interest-rate hikes are needed to control inflation, which has run above target for about five years. Some policymakers worry that prolonged above-target inflation could lift inflation expectations and make future price pressures harder to contain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/28/kevin-warsh-jackson-hole-federal-reserve-inflation.html">Fed Chairman Warsh warns on inflation at Jackson Hole - CNBC</a></li>
<li><a href="https://www.reuters.com/business/cooler-inflation-data-may-force-warshs-divided-fed-hold-line-rates-2026-08-14/">Cooler inflation data may force Warsh&#x27;s divided Fed to hold ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#inflation`, `#interest rates`, `#Kevin Warsh`

---

<a id="item-finance-news-8"></a>
### [Federal Reserve Holds Rates Steady, Signals Possible Hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

The Federal Reserve kept interest rates unchanged but left the door open to a future rate hike, according to CBS News.

google\_news · CBS News · Jun 17, 07:00

**「Background」** At its latest meeting, the Federal Reserve’s policy-setting committee, the FOMC, left the federal funds rate—the benchmark that influences borrowing costs across the economy—unchanged, but nearly half of its policymakers signaled they could support a rate hike later this year if inflation does not cool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door open to hike - CBS News</a></li>
<li><a href="https://www.msn.com/en-us/money/markets/federal-reserve-holds-interest-rates-steady-amid-resurgent-inflation/ar-AA25TWIp">Federal Reserve holds interest rates steady but leaves door open to hike</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#economy`

---

<a id="item-finance-news-9"></a>
### [US Federal Reserve Holds Rates Steady Under New Chair Warsh](https://news.google.com/rss/articles/CBMipgFBVV95cUxOM3c5cXgydnhwSFlrWmlyVjJobnRCbFkxaHg2c3NtTEl6Z2VLSGNIMXN3dmlKS2JZSF9Gc2p1TTVrd1hEcVdxSzBRaU13RVh1eTJRLW1pRkp0cHdKbk9FSU5SZ2FncC1ZangzQzZkZjFSaHNRWm94TlNROExtSm56Zk1qckpwT1JweWVKV1daY0tUMk03eFZJakRpMjNBVzl5N1NEQzFn0gGrAUFVX3lxTE1wYkYxa2NtTktYZkMyQ3VCSG5vYkw3UkE1cGpqaTRwOXE1MVpsd1ZfbDA2X3lGOEF5WG51SHFBbEhXbWs1enFfS1k2ZWRDMzVUU21sT2RMbC04VkoxUXk0Z1pYMVpWejF0ZGNyaUpiVWxjLWZYWVVBU28tb082QWlwT29PX1o3ekFTUk1fdTdGb3drUm5FOEIzZEc3UGlCRjhaUDlsS3Y0Yk8wMA?oc=5) ⭐️ 8.0/10

Al Jazeera reported that the US Federal Reserve, under new Chair Kevin Warsh, held interest rates steady after its latest policy meeting.

google\_news · Al Jazeera · Jun 17, 07:00

**「Background」** The Fed’s June 2026 meeting was Kevin Warsh’s first as chair, and officials voted unanimously to keep the benchmark rate at 3.5–3.75 percent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nbcnews.com/business/economy/inflation-kevin-warsh-fed-fomc-meeting-rcna350411">Federal Reserve under Kevin Warsh holds interest rates steady</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh | Inflation News | Al Jazeera</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#Kevin Warsh`, `#central bank`

---

<a id="item-finance-news-10"></a>
### [Federal Reserve holds rates steady amid fresh inflation concerns](https://news.google.com/rss/articles/CBMilAFBVV95cUxPdERIN3pDeThkLVR4YkNjUmF0WTlyR2RoZ0V4RzdxdDMxQlZJaEhPLXpBUXJ4VUsxZld1TTZ5Wk0xRXBMNHZ1dHBrbFVJM3FwQy1tUnZ4SU5VVTlxbldQcDZtNl9JRzdYUnRPaFR2TXAtWHJYWGZfUVRUWHVKRXAyVmlSMDFxcnRnRThlVGhkNURiVjhK?oc=5) ⭐️ 8.0/10

The Federal Reserve left interest rates unchanged as the new chairman faces renewed inflation challenges, according to NBC News.

google\_news · NBC News · Jun 17, 07:00

**「Background」** The Federal Reserve left its key interest rate unchanged in a 9-3 vote on July 29, 2026, at Chairman Kevin Warsh&\#x27;s first rate-setting meeting, with three regional presidents dissenting in favor of higher rates amid persistent inflation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members voted to hike</a></li>
<li><a href="https://www.nbcnews.com/business/economy/inflation-kevin-warsh-fed-fomc-meeting-rcna350411">Federal Reserve holds interest rates steady as Trump’s new chairman faces fresh inflation woes</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rate decision`, `#monetary policy`, `#inflation`, `#US economy`

---

<a id="item-finance-news-11"></a>
### [Fed&\#x27;s preferred inflation gauge rises at fastest pace in 3 years](https://news.google.com/rss/articles/CBMiigFBVV95cUxNODJpSG0zUXZ3T3JiemstZEM0ek55U3NHQVh2YlVSdG1WZnBwdEFMQUhmemQ5NnlmVk0teWFqV2lsRXJ2XzB0ZjJ5YW91ejZWUjRzZ2RkdzdCekdGNjAya2VIRnVPbmdSODE4WlEyR1BVY3hBeXhyTDV4NmZBVE9ybkpkbERKTnh2cFE?oc=5) ⭐️ 8.0/10

The Federal Reserve&\#x27;s preferred inflation gauge, the Personal Consumption Expenditures \(PCE\) price index, reportedly rose at its fastest pace in three years, according to CBS News. No specific rate was provided in the available article summary.

google\_news · CBS News · Jun 25, 07:00

**「Background」** The Personal Consumption Expenditures \(PCE\) price index is the Federal Reserve&\#x27;s preferred inflation measure, and the central bank seeks a 2% annual increase over time. According to CBS News, the May 2026 reading rose at a 4.1% annual rate, the fastest pace in about three years.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/pce-report-report-may-2026-federal-reserve-inflation/">The Fed&#x27;s preferred inflation gauge shows prices rising at ...</a></li>

</ul>
</details>

**Tags**: `#inflation`, `#Federal Reserve`, `#PCE price index`, `#monetary policy`, `#economy`

---

<a id="item-finance-news-12"></a>
### [US, Japan, and South Korea Sign Nuclear Cooperation Deal on Small Reactors](https://oilprice.com/Alternative-Energy/Nuclear-Power/Japan-South-Korea-and-the-US-Forge-a-New-Nuclear-Alliance.html) ⭐️ 7.0/10

The United States, Japan, and South Korea have signed a trilateral cooperation agreement to deploy small modular reactors \(SMRs\), aiming to position their nuclear industries as competitive alternatives to Chinese and Russian reactor suppliers in the region.

rss · OilPrice.com · Sep 5, 21:00

**「Background」** The deal follows a broader nuclear revival in Northeast Asia: Japan has reversed its post-Fukushima plan to phase out nuclear power, South Korea has continued expanding its nuclear industry across changes in government, and Washington has sought closer trilateral security and energy cooperation with both allies.

**Tags**: `#nuclear energy`, `#geopolitics`, `#US-Japan-South Korea`, `#energy security`, `#trilateral cooperation`

---

<a id="item-finance-news-13"></a>
### [U.S. Army’s $2.2 Billion Microreactor Plan Targets 2028 Deployment](https://oilprice.com/Alternative-Energy/Nuclear-Power/America-Is-Betting-Big-on-a-New-Generation-of-Small-Nuclear-Reactors.html) ⭐️ 7.0/10

The U.S. Army announced plans to award up to $2.2 billion to five companies to build microreactors at military bases, targeting at least one operational reactor by the third quarter of 2028. In July, Texas-based Aalo said its test reactor had achieved criticality—the point at which it can sustain a controlled chain reaction.

rss · OilPrice.com · Sep 5, 19:00

**「Background」** Microreactors are compact nuclear reactors, typically designed to produce 1–20 MW of thermal energy, that are meant to be factory-built and small enough to be transported by truck, boat, or plane.

**Tags**: `#nuclear energy`, `#microreactors`, `#small modular reactors`, `#U.S. Army`, `#energy policy`

---

<a id="item-finance-news-14"></a>
### [Anthropic Reportedly Plans IPO Valuing It Up to $2 Trillion](https://www.ft.com/content/9536c7b9-c600-48ec-8fe2-453b0ca187e9) ⭐️ 7.0/10

Anthropic is reportedly planning an initial public offering that could value it at up to $2 trillion.

telegram · zaihuapd · Sep 5, 01:26

**「Background」** The company’s long-term benefit trust \(LTBT\), an external trust that does not hold Anthropic equity, can appoint or remove a majority of board members and has already chosen four of the seven directors. The trust must be told in advance about major actions, including releases of new AI models, and regularly talks with management.

**Tags**: `#Anthropic`, `#IPO`, `#AI`, `#corporate governance`, `#valuation`

---

<a id="item-finance-news-15"></a>
### [US Auto Alliance Urges Permanent Ban on Chinese Connected Vehicles and Software](https://www.rfi.fr/tw/%E5%9C%8B%E9%9A%9B/20260904-%E6%B1%BD%E8%BB%8A%E8%A3%BD%E9%80%A0%E5%95%86%E6%95%A6%E4%BF%83%E7%BE%8E%E5%9C%8B%E5%9C%8B%E6%9C%83%E6%B0%B8%E4%B9%85%E7%A6%81%E6%AD%A2%E4%B8%AD%E5%9C%8B%E7%B6%B2%E8%81%AF%E6%B1%BD%E8%BB%8A%E9%80%B2%E5%85%A5%E7%BE%8E%E5%9C%8B) ⭐️ 7.0/10

The Alliance for Automotive Innovation, representing most automakers selling in the US, urged Congress to pass legislation before the current session ends on January 3 that would permanently bar the sale, import, and production of Chinese connected vehicles and their software/hardware in the US, citing below-cost dumping by Chinese automakers such as BYD and Geely.

telegram · zaihuapd · Sep 5, 10:04

**「Background」** The Alliance for Automotive Innovation, a U.S. trade group representing major automakers, sent the letter as part of an ongoing push to harden existing U.S. limits on Chinese vehicle technology. The group argues that Chinese connected vehicles and software are subsidized and pose risks to manufacturing and personal data privacy, and it wants Congress to act before the current session ends on Jan. 3.

**「Impact」** If enacted, the ban would directly affect automakers and suppliers that use Chinese-made connected-car software or hardware in the US; a bill advancing in the Senate Commerce Committee could also exclude Mercedes-Benz from the US market because Chinese investors hold nearly 20% of the company.

<details><summary>References</summary>
<ul>
<li><a href="https://www.autosinnovate.org/posts/press-release/automakers-to-congress-ban-chinese-connected-vehicles">Alliance for Automotive Innovation</a></li>
<li><a href="https://www.consumeraffairs.com/news/automakers-urge-congress-to-permanently-ban-chinese-vehicles-090426.html">Automakers urge Congress to permanently ban Chinese vehicles</a></li>

</ul>
</details>

**Tags**: `#US auto industry`, `#China connected vehicles`, `#trade regulation`, `#legislation`, `#Mercedes`

---