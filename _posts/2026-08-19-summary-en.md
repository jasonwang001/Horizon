---
layout: default
title: "Horizon Summary: 2026-08-19 (EN)"
date: 2026-08-19
lang: en
---

> From 244 items, 24 important content pieces were selected

---

**Technology News**
1. [Mojo is now open source](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B Scores 52, Matching GPT-5.6 Luna](#item-tech-news-2) ⭐️ 8.0/10
3. [Turbovec brings Google&\#x27;s TurboQuant vector search to Rust](#item-tech-news-3) ⭐️ 7.0/10
4. [Recovering a Bricked Framework 13 With $20 Tools and Pogo Pins](#item-tech-news-4) ⭐️ 7.0/10
5. [Linux 7.3 VRAM overcommit performance improvement](#item-tech-news-5) ⭐️ 7.0/10
6. [Field Study Quantifies Local Heat Rise from Data Centers](#item-tech-news-6) ⭐️ 7.0/10
7. [Apple&\#x27;s Camera-Equipped AirPods with Visual Intelligence May Arrive in September](#item-tech-news-7) ⭐️ 7.0/10
8. [macOS 26.7 Code Reveals Apple Intelligence Writing Tool Restrictions in China](#item-tech-news-8) ⭐️ 7.0/10
9. [China Orders Early Uninstall of Custom Windows 10 in Some Agencies](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Gulf Oil Reroutes Around Hormuz via Ship-to-Ship Transfers](#item-finance-news-1) ⭐️ 9.0/10
2. [Federal Reserve Leaves Interest Rates Unchanged in 9-3 Vote](#item-finance-news-2) ⭐️ 9.0/10
3. [Fed Chair Powell Briefs Press After Holding Rates Steady](#item-finance-news-3) ⭐️ 9.0/10
4. [Bond-Market Sell-Off Is Squeezing U.S. Households](#item-finance-news-4) ⭐️ 8.0/10
5. [Shadow Tanker Network Moves 4 Million Barrels a Day Around Hormuz](#item-finance-news-5) ⭐️ 8.0/10
6. [Saudi Aramco Resumes Hormuz Crude Loadings After Three-Week Pause](#item-finance-news-6) ⭐️ 8.0/10
7. [Romania restarts coal plant after Danube drought shuts nuclear reactors](#item-finance-news-7) ⭐️ 8.0/10
8. [“先买后付”贷款覆盖水电和房租，2025 年美国借贷额达 1600 亿美元](#item-finance-news-8) ⭐️ 8.0/10
9. [Economy Week Ahead: Fed Decision, Tariffs, Iran &\#x27;Pause&\#x27;](#item-finance-news-9) ⭐️ 8.0/10
10. [Fed Faces One of Its Most Unpredictable Meetings in Years](#item-finance-news-10) ⭐️ 8.0/10
11. [After-Hours Moves: La-Z-Boy Drops, Keysight Gains on Earnings](#item-finance-news-11) ⭐️ 7.0/10
12. [Jeanie Buss opposes siblings&\#x27; sale of Lakers stake to Iger and Kushner](#item-finance-news-12) ⭐️ 7.0/10
13. [U.S. Builds Iraq&\#x27;s First LNG Import Terminal](#item-finance-news-13) ⭐️ 7.0/10
14. [Apple’s US App Store Revenue Drops After Regulatory Changes](#item-finance-news-14) ⭐️ 7.0/10
15. [TrendForce: Domestic AI Chips to Supply Nearly 90% of China Market by 2026](#item-finance-news-15) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Mojo is now open source](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Modular has released the Mojo programming language and its toolchain under an Apache 2 license, following through on a promise originally made in May 2023. The release comes after Mojo shipped its 1.0 version last week. Mojo was initially designed to become a superset of Python, but that plan changed around August 2025, and the language is now positioned as its own Python-inspired language optimized for GPU programming rather than being fully compatible with existing Python code. The open-source release is a major milestone for the developer community that has been anticipating Mojo since its initial announcement.

rss · Simon Willison · Aug 18, 21:39

**「Background」** Mojo is an AI-focused programming language created by Modular, a company founded by Chris Lattner, the original creator of Swift. Since its public debut in 2023, Mojo generated significant interest because it promised to combine Python&\#x27;s usability with high-performance computing capabilities, particularly for AI and GPU workloads. The original roadmap committed to making Mojo a superset of Python so existing Python code could bootstrap a new ecosystem, but that goal was later revised as the project evolved.

**「Impact」** Developers and organizations evaluating Mojo for AI and GPU-accelerated work can now inspect, modify, and build on the compiler and toolchain under the permissive Apache 2 license, lowering adoption barriers and enabling community contributions.

**Tags**: `#mojo`, `#open-source`, `#programming-language`, `#ai`, `#modular`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B Scores 52, Matching GPT-5.6 Luna](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B scored 52 on the Artificial Analysis Intelligence Index, matching the maximum configuration of GPT-5.6 Luna and coming one point behind GLM-5.2 \(753B parameters\) and DeepSeek V4 Pro 0813 \(1.7T parameters\). Luna&\#x27;s size is unknown but presumed much larger than 27B. Simon Willison reports the result, describing the model as truly astonishing and highlighting the efficiency breakthrough of a 27B model matching frontier benchmark scores.

rss · Simon Willison · Aug 17, 23:58

**「Background」** The Artificial Analysis Intelligence Index is a benchmark that attempts to measure the overall reasoning and problem-solving ability of large language models on a standardized scale. Qwen 3.8 27B is an open-weight model from the Qwen family that accepts text and image inputs, outputs text, and supports a 256k-token context window; its score of 52 places it well above the median of 9 among comparable models, which is especially notable because many top-scoring models, such as GLM-5.2 and DeepSeek V4 Pro, have hundreds of billions to trillions of parameters.

**「Impact」** The result gives developers concrete evidence that a 27B model can match or nearly match much larger frontier models on this benchmark, potentially expanding viable model choices for cost and hardware-constrained deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B Intelligence, Performance &amp; Price Analysis</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLMs`, `#Qwen`, `#benchmark`, `#model-efficiency`

---

<a id="item-tech-news-3"></a>
### [Turbovec brings Google&\#x27;s TurboQuant vector search to Rust](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec is a new Rust implementation of Google&\#x27;s TurboQuant vector search technique, designed to reduce memory overhead for vector indexes. The project reports compact memory usage of about 4GB for 10 million documents, making it attractive for local and private search and AI infrastructure. It has generated community interest in potential SQLite bindings and browser use via WebAssembly, though the README has been criticized as insufficiently human-friendly. TurboQuant itself is not new, and Qdrant has already been integrating it for months, so Turbovec&\#x27;s contribution is a Rust-native option rather than a novel algorithm.

hackernews · fittingopposite · Aug 18, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49349898)

**「Background」** TurboQuant is a vector quantization method proposed in 2025 by researchers associated with Google Research, Google DeepMind, and NYU, designed to compress data for LLM inference, KV cache compression, vector databases, and nearest neighbor search. It is notable for achieving high compression with zero accuracy loss and for performing quantization without needing dataset-specific codebooks, although a TQ+ calibration step can be added for real-world embeddings. Turbovec is a Rust implementation of this technique, providing compact memory usage for vector search workloads.

**「Impact」** Rust developers building local, privacy-first vector search can use Turbovec to index millions of documents in a few gigabytes, and the anticipated SQLite and WASM integrations could lower the barrier for embedded and browser-based deployments. However, because mature vector databases like Qdrant already ship TurboQuant support, Turbovec&\#x27;s practical advantage rests on its lightweight Rust footprint and future integrations rather than on the quantization technique itself.

**「Community Discussion」** Commenters were excited about the 4GB-per-10M-documents efficiency and the prospect of faster reverse indexing, debugging, and performance testing, especially once SQLite bindings arrive. Others questioned the project&\#x27;s positioning: some pointed to FAISS no longer being state-of-the-art according to ANN benchmarks, some asked about WASM compilation for browser extensions, and one noted that Qdrant has already integrated TurboQuant for months, making Turbovec less unique.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TurboQuant">TurboQuant - Wikipedia</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google’s TurboQuant Makes Vector Search Smaller, Faster, and Simpler | by Mehul Gupta | Data Science in Your Pocket | Medium</a></li>

</ul>
</details>

**Tags**: `#vector-search`, `#rust`, `#quantization`, `#ai-infrastructure`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Recovering a Bricked Framework 13 With $20 Tools and Pogo Pins](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 7.0/10

A developer documented recovering a Framework 13 laptop with an AMD 7040-series CPU that was bricked by a BIOS update, using about $20 worth of tools instead of sending it in for service. The write-up highlights that Framework does not provide a populated header for flashing the BIOS, so the repair required pogo pins and an external flash programmer. It also points to Framework&\#x27;s own debugger and JSPI documentation as a relevant resource. The case illustrates both that inexpensive recovery is possible and that manufacturer choices can make firmware repair unnecessarily difficult.

hackernews · jp\_sc · Aug 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49345220)

**「Background」** Framework Laptop 13 AMD Ryzen 7040 series devices have documented cases where a BIOS update fails mid-installation, leaving the laptop unbootable \(&quot;bricked&quot;\), as shown in a March 2025 community thread. The linked post describes recovering such a laptop with about US$20 of tools, rather than replacing the motherboard as Framework support suggested. BIOS updates are risky because they rewrite the low-level firmware the system needs to start, and on this model Framework does not provide an easily accessible flash header, so recovery may require pogo pins or similar workarounds.

**「Impact」** Framework 13 AMD 7040-series owners who brick their laptop during a BIOS update can attempt recovery with low-cost tools, but the absence of an onboard flashing header raises the skill and risk barrier significantly.

**「Community Discussion」** Commenters debated manufacturer liability, with one suggesting small-claims court for software-caused bricking and another describing a similar bricked ThinkPad Nano. Several also noted Framework&\#x27;s JSPI connector and that it is unpopulated for cost reasons, and one Framework owner expressed regret about buying the laptop.

<details><summary>References</summary>
<ul>
<li><a href="https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/">Fixing a bricked AMD 7040 series Framework 13” laptop with $20 tools | Quantum</a></li>
<li><a href="https://community.frame.work/t/success-in-recovering-from-bad-bios-upgrade-framework-13-amd-7040/66598">Success in recovering from bad BIOS upgrade - Framework 13 AMD 7040 - Community Support - Framework Community</a></li>
<li><a href="https://resources.frame.work/downloads/laptop-13/amd-ryzen-7040-series/">Framework Laptop 13 AMD Ryzen™ 7040 Series — BIOS &amp; Drivers | Resources</a></li>

</ul>
</details>

**Tags**: `#hardware repair`, `#BIOS update`, `#Framework laptop`, `#embedded systems`, `#electronics repair`

---

<a id="item-tech-news-5"></a>
### [Linux 7.3 VRAM overcommit performance improvement](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 7.0/10

An article by flaburgan highlights a Linux kernel improvement aimed at better handling VRAM overcommit, reducing performance issues when GPU memory is exhausted. The proposed change, described as &quot;Linux 7.3,&quot; focuses on improving virtual memory allocation and fragmentation handling so that the kernel can make better guesses about memory &quot;stickiness&quot; to VRAM. This matters for GPU-heavy Linux workloads because exhaustion of video memory can otherwise cause severe performance degradation. Community reaction is largely positive, with excitement about upcoming kernel releases, though Nvidia users note the lack of paging support as a remaining limitation.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**「Background」** VRAM overcommit happens when applications, especially games, allocate more GPU memory than the physical VRAM available, forcing the system to reuse or evict pages and causing performance drops. The Linux kernel has traditionally lacked robust support for managing this scenario. Earlier this year, Natalie Vock of Valve&\#x27;s Linux graphics team proposed patches to improve VRAM management for systems with limited video memory, and those patches have now been merged upstream and queued for the Linux 7.3 kernel.

**「Impact」** For Linux users with AMD GPUs and limited VRAM, the kernel improvements are expected to reduce performance loss when video memory is exhausted; earlier patches from the same work already increased performance on lower-VRAM AMD GPUs, according to OSnews.

**「Community Discussion」** Commenters are largely enthusiastic, praising the article and eagerly awaiting Linux 7.3 after 7.2&\#x27;s performance improvements. Some note remaining concerns: one commenter wishes for better behavior when system RAM is full, and another points out that Nvidia still lacks paging support for VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM</a></li>
<li><a href="https://www.osnews.com/story/145846/beyond-the-limits-of-physical-vram/">Beyond the limits of physical VRAM – OSnews</a></li>

</ul>
</details>

**Tags**: `#linux`, `#kernel`, `#vram`, `#performance`, `#gpu`

---

<a id="item-tech-news-6"></a>
### [Field Study Quantifies Local Heat Rise from Data Centers](https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban) ⭐️ 7.0/10

A peer-reviewed field study measured the neighborhood-scale air temperature impact of a data center and found a modest but measurable downwind warming effect. The mean air temperature rose from approximately 42.7 °C upwind to 43.5 °C near the eastern boundary of the campus, an observed ΔT of about 0.8 °C that extended roughly 500 meters downwind. This provides empirical evidence that data center waste heat can contribute to localized urban heat, a concern that has been discussed largely through modeling rather than direct measurements. The effect is significant for nearby residents and urban planning, but remains localized and small compared to broader urban heat island phenomena.

hackernews · cwwc · Aug 18, 17:24 · [Discussion](https://news.ycombinator.com/item?id=49349147)

**「Background」** Data centers consume large amounts of electricity, and nearly all of it is ultimately released as waste heat through cooling systems and exhaust air. This study provides what the authors describe as the first field evidence that operating data centers produce measurable air temperature increases in adjacent residential neighborhoods, finding a mean downwind increase of about 0.8°C extending roughly 500 meters. With U.S. data center capacity projected to more than double by 2030, the findings characterize data center waste heat as a previously undocumented urban thermal hazard.

**「Impact」** The findings offer concrete, peer-reviewed evidence that data center waste heat can raise neighborhood temperatures by roughly 0.8 °C downwind, giving urban planners and environmental reviewers a measurable basis for siting and mitigation decisions. The modest and localized nature of the effect means its policy significance is still open to interpretation, particularly when weighed against other urban heat sources.

**「Community Discussion」** Commenters expressed sharply differing views: some questioned whether data center heat concerns are exaggerated or politically motivated, while others compared the attention to oil refineries and called for objective, dispassionate analysis of the data. One commenter noted that the observed mean ΔT was smaller than the headline suggested and pointed to separate reports of up to 4 °C warming in Phoenix, underscoring the range of local conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban">Data Center Waste Heat as an Emerging Urban Thermal Hazard ...</a></li>
<li><a href="https://asu.elsevierpure.com/en/publications/data-center-waste-heat-as-an-emerging-urban-thermal-hazard-first-/">Data Center Waste Heat as an Emerging Urban Thermal Hazard ...</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#waste heat`, `#urban heat island`, `#environmental impact`, `#field measurements`

---

<a id="item-tech-news-7"></a>
### [Apple&\#x27;s Camera-Equipped AirPods with Visual Intelligence May Arrive in September](https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/) ⭐️ 7.0/10

Apple is reportedly developing camera-equipped AirPods, internally codenamed B790, according to MacRumors and Mark Gurman. A demo in the macOS Tahoe 26.7 RC video shows the cameras recognizing book titles via visual intelligence and saving the information, while Siri can answer questions about the wearer&\#x27;s surroundings and record details. The report suggests the new AirPods could launch as early as September, though the information remains unconfirmed. If released, the product would extend AirPods beyond audio into wearable visual AI hardware.

telegram · zaihuapd · Aug 18, 02:00

**「Background」** Apple has long been reported to be exploring camera-equipped AirPods as part of its push into AI-powered wearables. The leaked macOS Tahoe 26.7 release candidate video shows a man holding a book while the AirPods identify it and offer visual intelligence, with Siri able to answer questions about the wearer&\#x27;s surroundings. The internal codename B790 distinguishes this project from future AirPods models, and industry analyst Mark Gurman has suggested the devices could launch as soon as September, though Apple has not officially confirmed them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/113519-leak-suggests-next-apple-airpods-have-cameras-visual.html">Leaked video shows Apple&#x27;s camera-equipped AirPods ... - TechSpot</a></li>
<li><a href="https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/">Apple&#x27;s Camera-Equipped AirPods Confirmed: See Them in Action</a></li>
<li><a href="https://techgenyz.com/apple-camera-equipped-airpods-leak/">Apple Camera-Equipped AirPods Just Leaked: 5 Details Revealed</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AirPods`, `#Visual Intelligence`, `#AI Hardware`, `#macOS`

---

<a id="item-tech-news-8"></a>
### [macOS 26.7 Code Reveals Apple Intelligence Writing Tool Restrictions in China](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

macOS 26.7 code discovered via MacRumors indicates Apple&\#x27;s Writing Tools will launch in mainland China with a built-in content-safety system. The system will show a &quot;content security update&quot; prompt and require an automatic update before the iPhone&\#x27;s Writing Tools can be used, display &quot;Unable to edit this text&quot; for content Apple Intelligence cannot handle \(suggesting a third-party provider\), and temporarily restrict Writing Tools after multiple safety alerts. This suggests the China version of Apple Intelligence will have independent content filtering, blocking, and punitive mechanisms, with safety review rules remotely pushed by cloud controls. The feature has not shipped and the exact trigger criteria are not disclosed.

telegram · zaihuapd · Aug 18, 02:16

**「Background」** Apple Intelligence is Apple&\#x27;s suite of AI features announced in June 2024, relying on a combination of on-device and server processing, and includes Writing Tools for text composition and editing. Recent code references in macOS Tahoe 26.7 reportedly indicate that Writing Tools may be coming to mainland China, with mentions of safety alerts, temporary restrictions after repeated triggers, and cloud-delivered review rules. This context is necessary to understand the item&\#x27;s significance for AI deployment under regional content moderation requirements.

**「Impact」** For mainland China users, Apple&\#x27;s Writing Tools will include remote-updatable content-safety rules, temporary usage bans after repeated safety alerts, and handoff of uneditable text to third-party services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>
<li><a href="https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/">macOS Tahoe 26.7 is Full of References to Unreleased Apple Products - MacRumors</a></li>
<li><a href="https://www.gadgets360.com/laptops/news/apple-macos-tahoe-26-7-code-new-product-codenames-report-11924169">Apple’s macOS Tahoe 26.7 Reportedly Includes References to iPhone 18, New Macs and More | Technology News</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI censorship`, `#China`, `#macOS`, `#content moderation`

---

<a id="item-tech-news-9"></a>
### [China Orders Early Uninstall of Custom Windows 10 in Some Agencies](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

China&\#x27;s Ministry of State Security has ordered some government-related agencies to uninstall customized Windows 10, moving the planned retirement several months earlier than the original February 2027 deadline. The directive is driven by data security concerns, according to people familiar with the matter, though no specific vulnerability was cited. Microsoft responded that it has found no security incidents affecting the product and that it continues to receive regular security updates. The early phase-out affects only some agencies and highlights rising scrutiny of foreign software in Chinese government environments.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** The customized Windows 10 is a government-only edition of Microsoft&\#x27;s operating system adapted for Chinese state use. China originally planned to phase it out by 2027, but the Ministry of State Security has now instructed some state-linked agencies to uninstall it earlier, citing data security concerns. State-linked entities are shifting toward domestic alternatives, especially since standard Windows 10 reached end of official support in October 2024.

**「Impact」** The accelerated removal of the government-only Windows 10 edition cuts Microsoft&\#x27;s associated China revenue to zero and, according to analysts, has a relatively controlled impact compared with Azure and AI growth, while Chinese domestic OS vendors&\#x27; shares rose sharply after the report, with Hunan Kylinsec and Archermind hitting 20% daily limits and China National Software climbing 10%. Microsoft maintains it has found no security incident tied to the product and continues to ship security updates, so the disclosed reason remains Beijing&\#x27;s data-security concerns rather than a confirmed vulnerability.

<details><summary>References</summary>
<ul>
<li><a href="https://wccftech.com/china-state-agencies-uninstall-windows-10-cmit-government-edition/">China’s State-Linked Firms Are Moving Away From Windows 10 ...</a></li>
<li><a href="https://tech.yahoo.com/computing/articles/china-finally-pulling-windows-10-112000903.html">China is finally pulling Windows 10 from government machines ...</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its ...</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262114664-win10-government-removal-microsoft-china-headwinds-tradingkey">Win10 Government Edition Phased Out Early as Microsoft&#x27;s China Business Faces New Headwinds</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>
<li><a href="https://finance.yahoo.com/technology/articles/microsoft-walks-away-china-102131877.html">Microsoft Walks Away From China</a></li>

</ul>
</details>

**Tags**: `#Windows 10`, `#China`, `#government`, `#data security`, `#Microsoft`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Gulf Oil Reroutes Around Hormuz via Ship-to-Ship Transfers](https://oilprice.com/Energy/Crude-Oil/How-Gulf-Oil-Is-Escaping-the-Strait-of-Hormuz.html) ⭐️ 9.0/10

Gulf oil producers are bypassing the Strait of Hormuz by transferring crude onto other tankers off Fujairah, as assessed earnings for a Middle East-to-China voyage exceeded $500,000 per day and ICE Brent traded at $91 per barrel on August 18, 2026.

rss · OilPrice.com · Aug 18, 15:00

**「Background」** The Strait of Hormuz is the world’s largest oil chokepoint, and large-scale shipping through it has nearly stopped after a 60-day US-Iran memorandum expired and Houthi attacks intensified.

**「Impact」** Asian refiners and Chinese shippers, which previously relied on Hormuz, must now collect Gulf barrels from Fujairah and Oman at higher cost, while US diesel users face record-high refining margins and the lowest seasonal distillate inventories since 1996.

**Tags**: `#crude-oil`, `#strait-of-hormuz`, `#shipping-rates`, `#geopolitics`, `#oil-prices`

---

<a id="item-finance-news-2"></a>
### [Federal Reserve Leaves Interest Rates Unchanged in 9-3 Vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

The Federal Reserve voted 9-3 to leave interest rates unchanged.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Reserve is the U.S. central bank, and its rate-setting committee decides the benchmark interest rate that influences borrowing costs across the economy. In this vote, nine officials backed holding rates steady while three dissented, signaling internal disagreement about the next policy move.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-leaves-interest-rate-unchanged-180102302.html">Federal Reserve leaves interest rate unchanged in 9 - 3 vote , but...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-3"></a>
### [Fed Chair Powell Briefs Press After Holding Rates Steady](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 9.0/10

Federal Reserve Chair Jerome Powell held a news briefing after the Federal Open Market Committee \(FOMC\) decided to leave interest rates unchanged.

google\_news · PBS · Mar 18, 07:00

**「Background」** The Federal Reserve left its benchmark interest rate unchanged after three consecutive cuts in 2019, with two officials voting against the decision and amid pressure from President Trump to lower rates.

**「Impact」** Borrowers may see no near-term relief in borrowing costs, as the Fed paused its rate-cutting cycle and left the federal funds rate at 3.50%–3.75%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thehindu.com/news/international/us-federal-reserve-leaves-interest-rates-unchanged-even-as-trump-demands-cuts/article69875802.ece">FOMC keeps interest rates unchanged despite... - The Hindu</a></li>
<li><a href="https://au.finance.yahoo.com/news/federal-reserve-leaves-interest-rates-unchanged-after-three-straight-cuts-as-two-officials-vote-against-decision-140019034.html">Federal Reserve leaves interest rates unchanged after three straight...</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>
<li><a href="https://www.tiktok.com/discover/the-latest-federal-reserve-meeting">The Latest Federal Reserve Meeting | TikTok</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Powell`, `#FOMC`

---

<a id="item-finance-news-4"></a>
### [Bond-Market Sell-Off Is Squeezing U.S. Households](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 8.0/10

A recent bond-market sell-off has pushed the 10-year Treasury yield above 4.7%, lifting the typical 30-year mortgage rate to 6.75% and leaving diesel prices 48% higher than a year ago, according to CNBC&\#x27;s analysis.

rss · CNBC Finance · Aug 18, 16:48

**「Background」** Long-term Treasury yields have risen as investors sell government debt, widening the gap between 2- and 10-year yields by nearly 29 basis points since June 24; the article attributes the move to large U.S. budget deficits, the Iran war, and heavy borrowing for AI infrastructure. New Federal Reserve Chairman Kevin Warsh has signaled tolerance for higher rates, and traders are watching his scheduled Aug. 28 speech in Jackson Hole for any signal of a shift.

**「Impact」** Households are exposed through mortgages and fuel prices, while the article notes that the S&amp;P 500 has returned 77% over the past three years and stock holdings are concentrated among the wealthiest Americans.

**Tags**: `#bond market`, `#Treasury yields`, `#monetary policy`, `#consumer impact`, `#fiscal policy`

---

<a id="item-finance-news-5"></a>
### [Shadow Tanker Network Moves 4 Million Barrels a Day Around Hormuz](https://oilprice.com/Energy/Crude-Oil/A-4-Million-Bpd-Shadow-Oil-Highway-Is-Running-Through-Hormuz.html) ⭐️ 8.0/10

Gulf producers are moving more than 4 million barrels per day past the Strait of Hormuz using a shadow network of transponder-off shuttle tankers and ship-to-ship transfers, according to Bloomberg. The network has grown to about 150 vessels off Oman, up from about 40 in January.

rss · OilPrice.com · Aug 18, 19:00

**「Background」** The network began taking shape in early May, when the U.S. military started overseeing ship-to-ship transfers off Fujairah in the UAE and Sohar in Oman; before the war, nearly 20 million barrels per day of crude and refined products normally moved through the strait.

**「Impact」** For global oil buyers, the workaround is helping keep Gulf supply available in the market, but it adds cost and risk by pushing more vessels onto longer routes around Africa, where Somali piracy is resurging.

**Tags**: `#oil supply`, `#Strait of Hormuz`, `#tankers`, `#geopolitics`, `#energy markets`

---

<a id="item-finance-news-6"></a>
### [Saudi Aramco Resumes Hormuz Crude Loadings After Three-Week Pause](https://oilprice.com/Latest-Energy-News/World-News/Aramco-Puts-VLCCs-Back-Into-Hormuz-After-Three-Week-Pause.html) ⭐️ 8.0/10

Saudi Aramco resumed crude loadings from its Ras Tanura and Juaymah terminals inside the Strait of Hormuz after a three-week pause, with three very large crude carriers \(VLCCs\) loading roughly 2 million barrels each between August 12 and August 16, according to Kpler and Vortexa data cited by Reuters.

rss · OilPrice.com · Aug 18, 18:18

**「Background」** The halt followed attacks on Aramco’s tanker fleet during last month’s escalation in the U.S.-Iran conflict. Aramco had been using workarounds, including ship-to-ship transfers off Fujairah and exports via Yanbu on the Red Sea, but the Yanbu route is now blocked by a Houthi blockade.

**「Impact」** The resumption does not mean exports are back to normal: Aramco is still offering Arab Medium and Heavy crude to Asian refiners through ship-to-ship transfers off Fujairah, and only about 670,000 barrels per day is expected to load from Egypt’s Sidi Kerir terminal for Asia this month, versus roughly 4 million bpd previously exported through Yanbu.

**Tags**: `#Oil Markets`, `#Saudi Aramco`, `#Strait of Hormuz`, `#Shipping`, `#Geopolitics`

---

<a id="item-finance-news-7"></a>
### [Romania restarts coal plant after Danube drought shuts nuclear reactors](https://oilprice.com/Latest-Energy-News/World-News/Romania-Restarts-Coal-Plant-as-Danube-Drought-Forces-Nuclear-Shutdown.html) ⭐️ 8.0/10

Romania restarted a 300-megawatt \(MW\) coal-fired unit at Rovinari after record-low Danube water levels forced the shutdown of both reactors at the Cernavoda nuclear plant, which typically generate about 20% of the country&\#x27;s electricity.

rss · OilPrice.com · Aug 18, 14:30

**「Background」** Nuclearelectrica, the state-owned operator, shut one reactor at the end of July and began disconnecting the other on August 13 because the Danube&\#x27;s lowest water levels in 90 years left too little cooling water; the plant director said no restart was expected within ten days.

**Tags**: `#energy security`, `#nuclear power`, `#drought`, `#coal power`, `#Romania`

---

<a id="item-finance-news-8"></a>
### [“先买后付”贷款覆盖水电和房租，2025 年美国借贷额达 1600 亿美元](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 8.0/10

U.S. buy-now-pay-later borrowing hit $160 billion in 2025, nearly doubling since 2023, as lenders expand into essential bills like rent and utilities, raising debt-trap concerns.

telegram · zaihuapd · Aug 18, 01:41

**Tags**: `#consumer credit`, `#buy now pay later`, `#household debt`, `#financial regulation`, `#US economy`

---

<a id="item-finance-news-9"></a>
### [Economy Week Ahead: Fed Decision, Tariffs, Iran &\#x27;Pause&\#x27;](https://news.google.com/rss/articles/CBMixAFBVV95cUxQY3BZcHU3LV9UTzlXZUxGb2FuM0hyQ25FaE55bHVEbG1LZFV1ZS1HejlvbEhjcU51NDdXVlJPZGIwRzdLa1dhNG9ZT3BVZXNVUVlqcm9lbmI0Q192ZHJKX3UteGd5Rmk0cTZaT1daS0I4NlFCZW1xbmU1bS1oZV9JenB0WVkwT3N2Ym1rRmRjbjFfZVRGaWhzeEVSZlg0SThxdW5oMkpRbFdnNVRnWlVwQ25EZUtoOTNxOVBYMnZITHJhTmF1?oc=5) ⭐️ 8.0/10

A U.S. News preview says the coming week will be busy, with the Federal Reserve&\#x27;s rate decision, tariff developments, and an Iran-related &\#x27;pause&\#x27; all in focus.

google\_news · usnews.com · Jul 27, 07:00

**「Background」** The Federal Reserve, chaired by Kevin Warsh, is holding its interest-rate decision this week; Warsh has pledged to reduce inflation. Separately, the Supreme Court recently struck down much of the Trump administration&\#x27;s tariff regime, so tariff policy is also in focus.

**「Impact」** The new round of tariffs announced Friday is applying pressure on markets and the economy, affecting businesses, consumers, and investors as the Federal Reserve prepares its rate decision.

<details><summary>References</summary>
<ul>
<li><a href="https://www.usnews.com/news/national-news/articles/2026-07-27/fed-rate-decision-tariffs-iran-pause-make-for-busy-economic-week">Fed Rate Decision , Tariffs , Iran ‘ Pause ’ Make for Busy Economic ...</a></li>
<li><a href="https://www.semafor.com/article/02/24/2026/us-tariffs-decision-wont-heavily-impact-clean-tech-firms">US tariffs decision won’t heavily impact clean tech firms | Semafor</a></li>
<li><a href="https://www.usnews.com/news/national-news/articles/2026-07-27/fed-rate-decision-tariffs-iran-pause-make-for-busy-economic-week">Fed Rate Decision, Tariffs, Iran ‘Pause’ Make for Busy ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#tariffs`, `#Iran`, `#economic calendar`

---

<a id="item-finance-news-10"></a>
### [Fed Faces One of Its Most Unpredictable Meetings in Years](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 8.0/10

The Federal Reserve’s next meeting is expected to be one of its most unpredictable in years, according to The Wall Street Journal, though no specific policy decision or rate target has been reported.

google\_news · WSJ · Jul 23, 07:00

**「Background」** At its previous meeting in July, the Federal Reserve kept its key interest rate unchanged at 3.50%–3.75% after one of the most unpredictable meetings in years, with three officials dissenting. Traders now see the next decision as a close call: markets assign nearly a 30% probability to a rate hike, according to Trading Economics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnn.com/2026/07/29/business/live-news/federal-reserve-interest-rate-07-29-26">Fed holds interest rates steady after cliffhanger meeting, but three officials dissent | CNN Business</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Interest Rates`, `#Central Bank`, `#Economy`

---

<a id="item-finance-news-11"></a>
### [After-Hours Moves: La-Z-Boy Drops, Keysight Gains on Earnings](https://www.cnbc.com/2026/08/18/stocks-making-the-biggest-moves-after-hours-tol-keys-lzb.html) ⭐️ 7.0/10

Shares of La-Z-Boy fell 17% after the company forecast current-quarter revenue of $500 million to $520 million, below the $536.8 million FactSet consensus; Keysight Technologies rose 2% after reporting adjusted third-quarter earnings of $3.07 per share, above the $2.48 expected.

rss · CNBC Finance · Aug 18, 20:55

**「Background」** The moves came after companies released quarterly earnings and forward guidance following the U.S. market close.

**Tags**: `#earnings`, `#after-hours`, `#guidance`, `#stocks`, `#company results`

---

<a id="item-finance-news-12"></a>
### [Jeanie Buss opposes siblings&\#x27; sale of Lakers stake to Iger and Kushner](https://www.cnbc.com/2026/08/17/jeanie-buss-opposes-sale-family-stake.html) ⭐️ 7.0/10

Jeanie Buss, governor and controlling owner of the Los Angeles Lakers, is opposing her siblings&\#x27; plan to sell the family&\#x27;s 17.8% stake to Bob Iger and Joshua Kushner, saying no sale can occur without her consent under a 2017 court order.

rss · CNBC Finance · Aug 18, 21:29

**「Background」** Last week, Iger and Kushner agreed to buy Mark Walter&\#x27;s majority Lakers stake at a $12.5 billion valuation, and an ESPN report said the Buss family stake would have given them roughly 83% overall ownership.

**「Impact」** Jeanie Buss&\#x27;s opposition means the family&\#x27;s 17.8% stake cannot be sold to Iger and Kushner without her consent, leaving the reported $12.5 billion deal in dispute.

**Tags**: `#Los Angeles Lakers`, `#Buss family`, `#NBA`, `#ownership dispute`, `#mergers and acquisitions`

---

<a id="item-finance-news-13"></a>
### [U.S. Builds Iraq&\#x27;s First LNG Import Terminal](https://oilprice.com/Energy/Natural-Gas/The-US-Is-Quietly-Building-a-New-Energy-Foothold-in-Iraq.html) ⭐️ 7.0/10

Excelerate Energy, a U.S.-based company, announced it will build and operate Iraq&\#x27;s first LNG import terminal at the Port of Khor Al Zubair, with operations expected to start in Q2 2027, an initial budget of US$450m, and a guaranteed regasification capacity of 500 million standard cubic feet per day.

rss · OilPrice.com · Aug 18, 23:00

**「Background」** Iraq has no existing LNG import terminal, and the article says Washington sees the project as part of a broader effort to reduce Iranian and Chinese influence in Iraq.

**「Impact」** Iraq&\#x27;s government relies on oil and gas for more than 90% of its revenues, and the terminal is intended to give the country a new route for natural gas imports while shifting regional energy ties toward the U.S.

**Tags**: `#LNG`, `#Iraq`, `#energy infrastructure`, `#Excelerate Energy`, `#U.S. energy policy`

---

<a id="item-finance-news-14"></a>
### [Apple’s US App Store Revenue Drops After Regulatory Changes](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

Data from Appfigures shows Apple’s US App Store commission revenue fell 18% from early 2026, and Sensor Tower estimates US user spending in the second quarter fell 6% year over year after 9% growth a year earlier; Apple says regulatory changes have hurt its services business.

telegram · zaihuapd · Aug 18, 12:17

**「Background」** Appfigures data cited by the Financial Times shows Apple&\#x27;s U.S. App Store commission revenue has fallen 18% since the start of 2026, with declines also reported in Brazil and Japan after both countries introduced new regulations. Sensor Tower reports that U.S. user spending through the App Store fell 6% year-over-year in the second quarter, compared with 9% growth a year earlier. Apple has said regulatory changes are dragging on its services business growth.

**「Impact」** The slowdowns reduce revenue flowing through Apple’s US App Store, affecting both Apple’s services segment and app developers who sell through the store.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/">Apple&#x27;s US App Store Commission Revenue Down 18% This Year - MacRumors</a></li>
<li><a href="https://appleinsider.com/articles/26/08/18/apples-app-store-revenue-in-danger-of-being-regulated-away">Apple&#x27;s App Store revenue in danger of being regulated away</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#Regulatory Impact`, `#Services Revenue`, `#Antitrust`

---

<a id="item-finance-news-15"></a>
### [TrendForce: Domestic AI Chips to Supply Nearly 90% of China Market by 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 7.0/10

TrendForce forecasts that China&\#x27;s domestically produced AI accelerators will supply nearly 90% of the domestic market in 2026, up from about 45% in 2025, with Cambricon and Huawei expected to be the biggest winners.

telegram · zaihuapd · Aug 18, 13:03

**「Background」** AI accelerators are specialized chips used to train and run artificial-intelligence models; in 2025, Nvidia shipped about 2.2 million units in China for a 55% market share, while Huawei shipped 812,000 units for a 20.3% share.

**「Impact」** The forecast implies Chinese suppliers would need to raise high-end AI chip output by about 2.2 times, to roughly 1.96 million units a year, but it remains uncertain whether production capacity can keep pace.

**Tags**: `#AI accelerators`, `#China`, `#semiconductor`, `#Huawei`, `#market forecast`

---