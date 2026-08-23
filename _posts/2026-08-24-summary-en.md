---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 140 items, 22 important content pieces were selected

---

**Technology News**
1. [How Complex Systems Fail: Still Essential for Reliability Engineering](#item-tech-news-1) ⭐️ 8.0/10
2. [ShardFlow hits 28 TPS on Qwen2.5-7B across cloud WAN with speculative decoding](#item-tech-news-2) ⭐️ 8.0/10
3. [Nvidia Spends $6B to License Poolside AI, Build US Open-Weight Rival](#item-tech-news-3) ⭐️ 8.0/10
4. [Understanding Harnesses in LLM Agent Systems](#item-tech-news-4) ⭐️ 7.0/10
5. [Malware in Android Head Unit OTA Updates](#item-tech-news-5) ⭐️ 7.0/10
6. [Wi-Fi 8 shifts focus from speed to reliability and efficiency](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic&\#x27;s Revenue Grows to $65B Despite Weak Adoption of New Models](#item-tech-news-7) ⭐️ 7.0/10
8. [Ulanqab Becomes China&\#x27;s AI Compute Hub with 12.5 GW of Capacity](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Federal Reserve holds interest rates unchanged in 9-3 vote](#item-finance-news-1) ⭐️ 9.0/10
2. [Diesel Supply Crisis Is Expected to Outlast the Middle East War](#item-finance-news-2) ⭐️ 8.0/10
3. [Nvidia Notifies Big AI Server Customers of Price Hikes Over 15%](#item-finance-news-3) ⭐️ 8.0/10
4. [Alibaba Plans HKD 80 Billion Share Placement for AI Investment](#item-finance-news-4) ⭐️ 8.0/10
5. [AMD Plans Over $10 Billion Taiwan Investment for Advanced Chip Packaging With TSMC](#item-finance-news-5) ⭐️ 8.0/10
6. [Berkshire Hathaway Sits on Nearly $400B in Cash Under Greg Abel](#item-finance-news-6) ⭐️ 8.0/10
7. [Forecast &\#x27;Super El Niño&\#x27; Could Disrupt Food, Water and Trade, NOAA Warns](#item-finance-news-7) ⭐️ 7.0/10
8. [Private Equity Circles Utilities as AI Power Demand Spurs Asset Sales](#item-finance-news-8) ⭐️ 7.0/10
9. [China&\#x27;s big three telecom operators report H1 2026 profit declines](#item-finance-news-9) ⭐️ 7.0/10
10. [Walmart Stock Drops 9%](#item-finance-news-10) ⭐️ 7.0/10
11. [Johnson &amp; Johnson&\#x27;s $5.5 Billion Talc Settlement and Legal Risk](#item-finance-news-11) ⭐️ 7.0/10
12. [Greg Abel Invests $23.5 Billion in Nine Stocks, Report Says](#item-finance-news-12) ⭐️ 7.0/10
13. [Sinopec H1 2026 Profit Jumps 19%](#item-finance-news-13) ⭐️ 7.0/10
14. [Inflation Hits 2.9%, Raising Worries About Interest Rate Hike](#item-finance-news-14) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [How Complex Systems Fail: Still Essential for Reliability Engineering](https://how.complexsystems.fail/) ⭐️ 8.0/10

The Hacker News thread revisits the 1998 essay &\#x27;How Complex Systems Fail,&\#x27; treating it as foundational for understanding why complex software and operational systems break. Commenters emphasize the essay&\#x27;s warning that root cause analysis is a fool&\#x27;s errand for such systems, since accidents emerge from interacting components rather than a single cause. A recurring point is that failure-free operations require experience with failure, which one commenter ties directly to the origins of Chaos Engineering. Others recommend John Gall&\#x27;s Systemantics as complementary reading and quote the essay&\#x27;s observation that interesting systems are inherently and unavoidably hazardous. The discussion reflects the essay&\#x27;s continued relevance for modern reliability engineering and incident analysis.

hackernews · shortcrct · Aug 23, 15:13 · [Discussion](https://news.ycombinator.com/item?id=49409473)

**「Background」** How Complex Systems Fail is a 1998 essay by patient-safety researcher Dr. Richard Cook, originally written to explain why complex systems such as healthcare, transportation, and power generation are inherently hazardous and fail in recognizable patterns. It outlines principles like the idea that complex systems are heavily defended against failure, that failure occurs when multiple small disturbances align, and that post-accident &\#x27;root cause&\#x27; analysis often oversimplifies the true dynamic nature of system operations. The essay has since become a touchstone in resilience engineering and software operations, where practitioners apply its lessons to distributed systems and chaos engineering.

**「Impact」** For engineers and SREs, the essay&\#x27;s framing pushes incident reviews away from single root causes toward systemic resilience and failure experimentation, a perspective that underpins Chaos Engineering practices.

**「Community Discussion」** Commenters broadly agree the essay is essential reading, with tptacek stressing that its critique of root cause analysis becomes clear only after watching real systems fail; jedberg connects the essay&\#x27;s core insight to the creation of Chaos Engineering, and others point to John Gall&\#x27;s Systemantics as complementary material. One minor thread questions whether the essay&\#x27;s phrase &\#x27;by their own nature&\#x27; is a typo, adding a small note of textual curiosity.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@wilmertezen/the-hidden-cost-of-good-enough-what-distributed-systems-teach-us-about-accountability-8cb59e05928b">The Hidden Cost of Good Enough: What Distributed Systems teach us...</a></li>
<li><a href="https://www.zdnet.com/article/18-truths-the-long-fail-of-complexity/">18 truths: The long fail of complexity | ZDNET</a></li>

</ul>
</details>

**Tags**: `#complex systems`, `#resilience engineering`, `#root cause analysis`, `#chaos engineering`, `#systems thinking`

---

<a id="item-tech-news-2"></a>
### [ShardFlow hits 28 TPS on Qwen2.5-7B across cloud WAN with speculative decoding](https://www.reddit.com/r/MachineLearning/comments/1vw5ysj/28_tps_on_qwen257b_across_two_separate_cloud/) ⭐️ 8.0/10

ShardFlow, a distributed LLM inference framework, splits any HuggingFace transformer across N GPU machines and uses neural speculative decoding to tolerate WAN latency. In a benchmark on Qwen2.5-7B, two GCP T4 nodes in Iowa and Oregon communicated over public internet through an AWS EC2 TCP relay in Ohio, with about 86ms RTT. With K=8 drafting and 4.07 tokens committed per round trip, average throughput rose from 4.92 TPS \(non-speculative\) to 14.3 TPS peak with an eager neural drafter, and to 28.10 TPS peak / 20.31 TPS average after capturing the 0.5B drafter&\#x27;s forward pass as a CUDA Graph. The CUDA Graph change cut draft latency from 112ms to 25ms by replacing roughly 1,500 Python-launched kernels with one driver call; the same two-node setup reached 14.43 TPS average on Qwen2.5-14B with NF4 4-bit quantization. The project is available at https://github.com/rautaditya2606/Shardflow.

reddit · r/MachineLearning · /u/katua\_bkl · Aug 23, 12:30

**「Background」** Speculative decoding runs a small draft model to generate several candidate tokens, then the larger target model verifies them in parallel, so multiple tokens can be accepted per forward pass. In distributed inference, token generation normally pays WAN round-trip latency for every token; treating that latency as a per-round cost and using CUDA Graphs to shrink per-round overhead are the key mechanisms ShardFlow uses.

**「Impact」** For developers building latency-sensitive multi-node inference, the technique demonstrates a roughly 5.7x speedup over the non-speculative baseline on a ~86ms public WAN link, while also reducing GPU idle time caused by Python kernel launch overhead.

**Tags**: `#distributed-inference`, `#speculative-decoding`, `#LLM-inference`, `#CUDA-Graphs`, `#Qwen`

---

<a id="item-tech-news-3"></a>
### [Nvidia Spends $6B to License Poolside AI, Build US Open-Weight Rival](https://www.wsj.com/tech/ai/nvidia-is-spending-6-billion-to-build-a-powerful-u-s-alternative-to-chinese-ai-c51c38cc) ⭐️ 8.0/10

Nvidia has reached a deal with AI startup Poolside to invest $1 billion at a $12 billion pre-money valuation and pay $6 billion to license Poolside&\#x27;s technology, while absorbing most of its engineers—over 100 employees—into Nvidia&\#x27;s Nemotron open-weight model project. The company aims to build one of the world&\#x27;s most powerful open-weight models, positioning it to compete directly with Chinese open-source models like DeepSeek and Kimi K3, as well as U.S. closed-source AI firms such as OpenAI and Anthropic. The agreement was reported by The Wall Street Journal and marks a significant strategic move by Nvidia to strengthen its presence in the open-weight AI space.

telegram · zaihuapd · Aug 23, 04:20

**「Background」** Poolside is an AI startup building large language models, and Nvidia has traditionally sold the chips that power AI while also developing its own open-weight model line called Nemotron. Under the reported agreement, Nvidia will pay $6 billion for a non-exclusive license to Poolside&\#x27;s models and will make job offers to more than 100 Poolside employees, alongside a $1 billion investment at a $12 billion pre-money valuation, according to Bloomberg and Newcomer. This reflects intensifying competition between U.S. companies and Chinese open-source model developers such as DeepSeek and Kimi K3, as well as against closed-source U.S. rivals like OpenAI and Anthropic.

**「Impact」** The $6 billion license plus $1 billion investment lets Nvidia absorb Poolside&\#x27;s model-building software and most of its engineers—over 100 employees, with one report citing 109 staff—to power its Nemotron open-weight models, which it says will compete with China&\#x27;s DeepSeek and Kimi K3 and challenge U.S. closed rivals. The structured deal is the third of its kind for Nvidia and may help it avoid regulatory scrutiny while expanding beyond chip supply into AI model development.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/nvidia-pay-poolside-6-billion-181448803.html">Nvidia to Pay Poolside a $6 Billion License, Tap Startup’s Staff</a></li>
<li><a href="https://www.newcomer.co/p/sources-poolside-strikes-6-billion">SOURCES: Poolside Strikes $6 Billion Licensing Deal with Nvidia &amp; Raises $1 Billion for Remaining Company at $12 Billion Valuation</a></li>
<li><a href="https://theoutpost.ai/news-story/nvidia-pays-poolside-6-billion-for-ai-model-development-software-in-third-structured-deal-30028/">Nvidia Pays $6bn for Poolside AI Model Development Tech</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI`, `#open-source models`, `#Poolside`, `#investment`

---

<a id="item-tech-news-4"></a>
### [Understanding Harnesses in LLM Agent Systems](https://earendil.com/posts/what-is-a-harness/) ⭐️ 7.0/10

A post on Earendil.com, &\#x27;What Is a Harness?&\#x27;, defines a harness in LLM-based agent systems as the scaffolding that connects models to tools, interfaces, and workflows, separating it from the model itself. The author offered the analogy harness = chassis, model = engine, tokens = fuel, agent = car to illustrate the relationship. Although aimed at a non-technical audience, the post resonated with practitioners: one commenter details building an accounting-agent harness with an internal CLI, and another asks for harness handoff across terminals, devices, teams, and model providers. The concept matters because as LLM agents proliferate, the harness layer—not the raw model—is becoming the main source of practical value and developer experience.

hackernews · tosh · Aug 23, 14:24 · [Discussion](https://news.ycombinator.com/item?id=49409092)

**「Background」** In LLM-based agent systems, a harness is the supporting layer between the model and the real world—providing rules, restrictions, routing, checkpoints, state management, and recovery. It is often described as a chassis around the engine or the &quot;electronics&quot; that turn raw model capability into useful, controlled behavior. Without a harness, an agent is typically unpredictable or unsafe.

**「Impact」** For developers building LLM agents, harnesses such as Pi provide a concrete, extensible runtime \(with skills, AGENTS.md files, and a minimal system prompt for token efficiency\) plus a unified multi-provider API, but the tradeoff is that Pi extensions run in process with full system access, requiring greater trust than plugin models like OpenCode.

**「Community Discussion」** Practitioners broadly agree harnesses are the layer that will define LLM agent value: Syntaf reports an internal CLI as &\#x27;extremely useful&\#x27; for accounting agents but finds hand-built skills too prescriptive, and xrd wants better handoff across CLI/Web UI, teams, modalities, and model providers. Another commenter calls harnesses &\#x27;the next frontier&\#x27; and praises Pi&\#x27;s extension system, while another predicts &\#x27;harness&\#x27; will be the 2026 buzzword after &\#x27;agent&\#x27;.

<details><summary>References</summary>
<ul>
<li><a href="https://earendil.com/posts/what-is-a-harness/">What is a Harness ? | EARENDIL</a></li>
<li><a href="https://momentic.ai/blog/the-harness-will-not-save-you">The Harness Will Not Save You | Momentic</a></li>
<li><a href="https://mzyag.github.io/writing/engineering-the-harness.html">Engineering the Harness : Governing Agent Behavior Without Slowing...</a></li>
<li><a href="https://pi.dev/">Pi Coding Agent</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/ pi : AI agent toolkit: unified LLM API, agent ...</a></li>
<li><a href="https://composio.dev/content/pi-vs-opencode">Pi vs OpenCode: After 100 Hours, Which Open-Source Coding Agent ...</a></li>

</ul>
</details>

**Tags**: `#LLM agents`, `#agent harness`, `#AI tooling`, `#software engineering`, `#developer experience`

---

<a id="item-tech-news-5"></a>
### [Malware in Android Head Unit OTA Updates](https://securelist.com/android-head-unit-malware/121106/) ⭐️ 7.0/10

Securelist has reported malware that is delivered through official first-party OTA updates on inexpensive Chinese aftermarket Android head units. The malware is targeted and non-self-propagating; it cannot spread to other Android-based head units and does not affect Android Auto, which runs primarily on the connected phone rather than the head unit. Because head units often contain little of value, a likely goal is botnet recruitment, although many users pair their phones with the unit, suggesting potential for lateral movement in future variants. Many vehicles also give the head unit access to the CAN bus, which raises safety concerns, but the immediate impact is limited to the specific aftermarket units receiving the malicious updates.

hackernews · campuscodi · Aug 23, 13:05 · [Discussion](https://news.ycombinator.com/item?id=49408550)

**「Background」** Android-based automotive head units are aftermarket car stereos that run the Android operating system and often rely on automatic over-the-air \(OTA\) firmware updates supplied by their manufacturers. Kaspersky researchers identified a multi-stage downloader delivered through the legitimate update service for DoFun head units, making it the first documented case of malware spread to head units via an automatic firmware-update service; the malware&\#x27;s purpose is ad fraud and creation of a proxy botnet. This is distinct from Android Auto, which is a screen-mirroring protocol where apps run on the connected phone rather than on the head unit itself.

**「Impact」** The concrete consequence is compromised devices among owners of cheap Chinese aftermarket Android head units that accept official OTA updates; Android Auto and other standard head units are not affected.

**「Community discussion」** Commenters clarified that the malware only arrives via official OTA updates on cheap Chinese aftermarket units and cannot self-propagate, but they raised concerns about lateral movement through paired phones and about head units with CAN bus access potentially enabling physical safety risks. The broader discussion also noted the automotive industry&\#x27;s poor security track record, citing keyless entry, OBD port, and unsecured CAN bus vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://securelist.com/android-head-unit-malware/121106/">First Android malware targeting automotive head units | Securelist</a></li>
<li><a href="https://www.kaspersky.com/blog/car-botnet-malware-for-head-units-with-android/56296/">Malware in car infotainment systems: how... | Kaspersky official blog</a></li>
<li><a href="https://malwaretips.com/threads/kaspersky-expert-finds-the-invisible-passenger-in-your-car.142890/">Malware News - Kaspersky expert finds the... | MalwareTips Forums</a></li>

</ul>
</details>

**Tags**: `#malware`, `#android`, `#automotive`, `#security`, `#OTAs`

---

<a id="item-tech-news-6"></a>
### [Wi-Fi 8 shifts focus from speed to reliability and efficiency](https://www.xda-developers.com/wi-fi-8-first-wireless-upgrade-years-isnt-chasing-speed-home-networks-need-it/) ⭐️ 7.0/10

An XDA article describes the upcoming Wi-Fi 8 standard, also known as IEEE 802.11bn, as the first major wireless upgrade in years that prioritizes reliability and efficiency over raw speed. Instead of chasing theoretical peak throughput, the standard is said to target real-world networking pain points such as unstable connections, poor roaming, and interference. The article notes that Wi-Fi 8 is not yet finalized, and coverage is preliminary with limited technical depth. This focus matters because home and warehouse networks often suffer more from unreliable links and stubborn clients than from a lack of headline gigabit speeds.

hackernews · taubek · Aug 23, 06:41 · [Discussion](https://news.ycombinator.com/item?id=49406539)

**「Background」** Wi-Fi generations are defined by IEEE 802.11 amendments, with Wi-Fi 7 \(IEEE 802.11be\) having introduced features like multi-link operation \(MLO\) to increase capacity across 2.4 GHz, 5 GHz, and 6 GHz bands. Wi-Fi 8 is the marketing label for the in-progress IEEE 802.11bn Ultra-High Reliability \(UHR\) amendment, which shifts the design focus from peak data-rate gains toward improving reliability and efficiency in real-world conditions. This contrasts with earlier standards that primarily chased speed, as Wi-Fi 8 aims to address issues like interference, roaming, and consistent performance rather than theoretical maximum throughput.

**「Impact」** If Wi-Fi 8 delivers on its reliability-focused design, users in congested or mixed-device environments could see steadier real-world throughput and better roaming, though actual benefits will depend on final standards approval and client adoption.

**「Community discussion」** Commenters broadly welcomed the reliability focus, citing practical needs like warehouse scanners that require dependable 20Mbit/s links and residential networks where many devices remain on older 2.4GHz connections. One commenter questioned whether Wi-Fi should be replaced by 5G/6G technology, while another asked about the spectrum-sharing mechanism behind the proposed resource units.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wi-Fi_7">Wi - Fi 7 - Wikipedia</a></li>
<li><a href="https://www.compoundlearn.ai/topics/wifi-8-80211bn-ultra-high-reliability">802 . 11 bn UHR: Wi - Fi 8 Ultra High Reliability ... — CompoundLearn</a></li>
<li><a href="https://lrc.perdanauniversity.edu.my/sdi/how-ieee-802-11bn-delivers-ultra-high-reliability-for-wi-fi-8/">How IEEE 802 . 11 bn Delivers Ultra-High Reliability for Wi - Fi ...</a></li>

</ul>
</details>

**Tags**: `#Wi-Fi`, `#networking`, `#IEEE 802.11bn`, `#wireless`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [Anthropic&\#x27;s Revenue Grows to $65B Despite Weak Adoption of New Models](https://simonwillison.net/2026/Aug/23/anthropics-best-ai-model-struggles-to-attract-users-as-cheaper-t/) ⭐️ 7.0/10

According to FT reporting cited by Simon Willison, Anthropic&\#x27;s annualized revenue rose to $65bn in July 2026, up from $47bn in May, and the company told investors it expects Q3 to be profitable using the same model that declared Q2 profitable, with 6,000 customers spending $100,000 or more annually. OpenAI&\#x27;s annualized revenue has jumped 35 percent in the quarter to date to over $40bn, boosted by July&\#x27;s GPT-5.6 launch after a sluggish start to the year. Ramp&\#x27;s AI index, based on billing data from 70,000 companies, shows Anthropic model spend in July 2026 still led by Opus 4.8 at 28.0 percent, followed by Sonnet 4.6 at 8.3 percent, while the newer Fable 5 and Opus 5 captured only 8.0 percent and 3.5 percent, respectively. This suggests Anthropic&\#x27;s newest flagship models, including Fable 5, have struggled to attract users, partly because of cost, even as overall Anthropic revenue grows rapidly.

rss · Simon Willison · Aug 23, 20:24

**「Background」** Anthropic and OpenAI are leading commercial AI labs competing for enterprise and developer usage of large language models. Anthropic&\#x27;s Claude lineup uses tiered models such as Opus, Sonnet, and Haiku, with newer generations like Opus 5 released on July 24, 2026; Fable 5 appears to be a new flagship whose cost has reportedly limited adoption. Ramp&\#x27;s AI index tracks model adoption by analyzing billing data from 70,000 companies that use Ramp credit cards.

**Tags**: `#AI industry`, `#Anthropic`, `#OpenAI`, `#revenue`, `#AI models`

---

<a id="item-tech-news-8"></a>
### [Ulanqab Becomes China&\#x27;s AI Compute Hub with 12.5 GW of Capacity](https://www.wired.com/story/the-unlikely-place-at-the-center-of-chinas-ai-boom/) ⭐️ 7.0/10

According to a Goldman Sachs report, Ulanqab, Inner Mongolia, has opened or begun construction on nearly 100 data centers since 2016, with Chinese companies committing 12.5 GW of total capacity—over 70% announced in the past year and exceeding the 10 GW planned for OpenAI&\#x27;s Stargate. DeepSeek, ByteDance, Alibaba, and Xiaohongshu have all built AI data centers there. The region&\#x27;s cold climate, low electricity prices, and proximity to Beijing attract operators, but water scarcity is an emerging constraint: annual precipitation is only about 14 inches, and last month the local water plant shut off supply for seven hours each night. Roughly 37% of electricity still comes from coal-fired power, highlighting environmental limits.

telegram · zaihuapd · Aug 23, 00:55

**「Background」** Ulanqab is a prefecture-level city in Inner Mongolia known for its cool, dry weather and cheap energy, which helps cool power-hungry AI data centers. It has become a preferred location for Chinese cloud and AI companies seeking scalable compute capacity, especially as domestic AI demand has surged.

**「Impact」** For the Chinese AI industry, the concentrated build-out gives DeepSeek, ByteDance, Alibaba, and Xiaohongshu access to massive, relatively low-cost compute capacity, but operators face growing water-supply and coal-dependency risks that could constrain expansion.

**Tags**: `#AI infrastructure`, `#data centers`, `#China`, `#cloud computing`, `#energy`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Federal Reserve holds interest rates unchanged in 9-3 vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

The Federal Reserve voted 9-3 to leave interest rates unchanged, holding its benchmark rate steady at its latest policy meeting.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Reserve held its benchmark interest rate in a 3.5%–3.75% range for the fifth straight meeting, with three officials voting for a hike as inflation concerns persist.

**「What it means」** Because the Fed held its benchmark rate at 3.50%–3.75% for a fifth straight meeting, households and businesses with variable-rate loans will continue facing elevated borrowing costs, and investors remain uncertain about the next policy move.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members voted to hike</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Central Banks`, `#Economy`

---

<a id="item-finance-news-2"></a>
### [Diesel Supply Crisis Is Expected to Outlast the Middle East War](https://oilprice.com/Energy/Energy-General/Diesel-Crisis-Threatens-to-Outlast-the-Middle-East-War.html) ⭐️ 8.0/10

A global diesel shortage, driven by Middle East hostilities, refinery damage, and Ukrainian drone strikes on Russian refineries, is expected to outlast the war by months, with European diesel prices up 70% from pre-war levels and U.S. diesel crack spreads reaching a record $102 per barrel this week.

rss · OilPrice.com · Aug 23, 23:00

**「Background」** The squeeze follows months of Middle East hostilities that, according to the IEA, knocked out roughly a fifth of regional refining capacity \(9.6 million barrels daily\), while Ukrainian drone attacks on Russian refineries and record U.S. fuel exports have tightened inventories.

**「Impact」** Households and businesses face higher diesel and heating costs this winter as global inventories are drawn down, adding to inflation that has already picked up in the U.S. and eurozone.

**Tags**: `#diesel crisis`, `#refining capacity`, `#energy prices`, `#inflation`, `#Middle East conflict`

---

<a id="item-finance-news-3"></a>
### [Nvidia Notifies Big AI Server Customers of Price Hikes Over 15%](https://www.bloomberg.com/news/articles/2026-08-22/nvidia-customers-notified-about-ai-related-price-hikes-above-15) ⭐️ 8.0/10

Nvidia has told some of its largest customers that most AI servers using its chips will cost more than 15% extra, blaming a surge in memory-chip costs, people familiar with the matter said.

telegram · zaihuapd · Aug 23, 01:45

**「Background」** The increase applies to systems shipping early next year and covers Nvidia&\#x27;s flagship Vera Rubin and Grace Blackwell chips. Manufacturers that assemble servers for Microsoft, Google and Oracle have already notified their customers, while memory suppliers Samsung, SK Hynix and Micron, which dominate global DRAM production, have gained pricing power as shortages persist.

**Tags**: `#Nvidia`, `#AI servers`, `#memory chips`, `#DRAM`, `#price increase`

---

<a id="item-finance-news-4"></a>
### [Alibaba Plans HKD 80 Billion Share Placement for AI Investment](https://www.jwview.com/jingwei/html/m/08-23/684731.shtml) ⭐️ 8.0/10

Alibaba announced on Aug. 23 a proposed placement of new shares totaling HKD 80 billion to non-US investors outside the United States, its first such placement since its 2019 Hong Kong listing; the company said all net proceeds would go toward AI infrastructure investment.

telegram · zaihuapd · Aug 23, 08:19

**「Background」** Alibaba has not launched a new-share placement since its 2019 Hong Kong listing, and the proposed HK$80 billion deal would be the largest primary follow-on offering by a Hong Kong-listed company.

**「Impact」** Existing Alibaba shareholders face dilution from the planned HK$80 billion \(about $10.2 billion\) new-share placement. The net proceeds are earmarked for AI infrastructure, a spending area that already contributed to a 75% quarterly net profit drop and a 45% year-over-year rise in cloud/AI revenue.

<details><summary>References</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/alibaba-proposes-hong-kong-share-placement-worth-13-billion">Alibaba launches $13 billion Hong Kong share placement to fund AI spending | The Straits Times</a></li>
<li><a href="https://thenextweb.com/news/alibaba-10-2bn-share-placement-ai-infrastructure">Alibaba is raising $10.2bn and spending all of it on AI</a></li>
<li><a href="https://finance.biggo.com/news/f913b299-46f7-4ba2-9b08-90a608ee3c01">Alibaba Raises $10.2 Billion in Hong Kong&#x27;s Largest-Ever Share Sale — BigGo Finance</a></li>

</ul>
</details>

**Tags**: `#Alibaba`, `#share placement`, `#AI investment`, `#Hong Kong`, `#corporate finance`

---

<a id="item-finance-news-5"></a>
### [AMD Plans Over $10 Billion Taiwan Investment for Advanced Chip Packaging With TSMC](https://finance.yahoo.com/technology/articles/amd-investing-more-10-billion-155000045.html) ⭐️ 8.0/10

AMD plans to invest more than $10 billion in Taiwan to expand advanced chip packaging capacity with TSMC, a move aimed at securing supply for AI and high-performance chips.

openbb · NVDA · Aug 23, 15:50

**「Background」** AMD is investing over $10 billion in Taiwan to expand advanced chip packaging and manufacturing capacity with TSMC, as CEO Lisa Su cited surging global AI infrastructure demand and tight CPU supply.

**「Impact」** Advanced chip packaging is a bottleneck for AI chip output, so this investment is meant to secure the packaging capacity AMD needs for its AI and high-performance processors.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.biggo.com/news/XiWKTp4BrAZSr0oSuxOL">AMD Pours $10 Billion Into Taiwan to Ease Global CPU Crunch and Challenge Nvidia — BigGo Finance</a></li>
<li><a href="https://finance.biggo.com/news/XOzBTJ4BYH_ypPqOCx7e">AMD to Invest Over $10 Billion in Taiwan; Lisa Su Says Teaming Up with TSMC to Accelerate AI System-Level Production — BigGo Finance</a></li>
<li><a href="https://www.linkedin.com/posts/simon-higgins-6169bb25a_semiconductor-advancedpackaging-tsmc-activity-7490404914959933440-CNGW">TSMC &#x27;s EMIB Challenge to Intel&#x27;s Packaging Lead | LinkedIn</a></li>
<li><a href="https://kr-asia.com/semiconductor-investment-rebounds-on-ai-but-not-everyone-is-winning">Semiconductor investment rebounds on AI , but not everyone is...</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#TSMC`, `#Semiconductor`, `#Chip Packaging`, `#Investment`

---

<a id="item-finance-news-6"></a>
### [Berkshire Hathaway Sits on Nearly $400B in Cash Under Greg Abel](https://finance.yahoo.com/markets/stocks/articles/berkshire-ceo-greg-abel-sitting-153500037.html) ⭐️ 8.0/10

Berkshire Hathaway, now led by Greg Abel, holds nearly $400 billion in cash; an analysis suggests his deal-making approach will differ from Warren Buffett’s.

openbb · BRK-B · Aug 23, 15:35

**「Background」** Warren Buffett, Berkshire&\#x27;s longtime CEO, generally used a hands-off approach, buying strong companies and keeping their managers, which created overlapping businesses. Greg Abel, who led Berkshire Hathaway Energy before becoming CEO, appears more willing to treat those overlaps as opportunities, such as in the Taylor Morrison Home deal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/12/berkshire-ceo-greg-abel-is-sitting-on-more-than-36/">Berkshire CEO Greg Abel Is Sitting on More Than $360 Billion in Cash. Here&#x27;s How His Deal-Making Approach Differs From Warren Buffett&#x27;s. | The Motley Fool</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/berkshire-ceo-greg-abel-sitting-153500037.html">Berkshire CEO Greg Abel Is Sitting on Nearly $400 Billion in Cash. Here&#x27;s How His Deal-Making Approach Differs From Warren Buffett&#x27;s.</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#Greg Abel`, `#cash management`, `#M&amp;A strategy`, `#Warren Buffett`

---

<a id="item-finance-news-7"></a>
### [Forecast &\#x27;Super El Niño&\#x27; Could Disrupt Food, Water and Trade, NOAA Warns](https://oilprice.com/Energy/Energy-General/Super-El-Nio-Threatens-Food-Water-and-Trade-Worldwide.html) ⭐️ 7.0/10

Meteorologists forecast a possible &\#x27;Super El Niño&\#x27; in 2026, with NOAA estimating a greater than 90% probability that it becomes &\#x27;very strong&\#x27; in the second half of the year; the UN World Food Programme estimates that nearly 50 million more people could face acute hunger.

rss · OilPrice.com · Aug 23, 19:00

**「Background」** El Niño is a periodic warming of the tropical Pacific Ocean that can shift weather patterns, causing drought in some regions and heavy rain in others; a &\#x27;Super El Niño&\#x27; means sea surface temperatures rise at least 2 degrees Celsius above average.

**「Impact」** If the forecast materializes, rain-fed crops in areas such as Central America and Southeast Asia could be disrupted, and shipping through the Panama Canal could face restrictions—the canal authority has already imposed stricter load limits; poorer regions with less ability to adapt would be most exposed.

**Tags**: `#El Niño`, `#climate`, `#food security`, `#trade`, `#Panama Canal`

---

<a id="item-finance-news-8"></a>
### [Private Equity Circles Utilities as AI Power Demand Spurs Asset Sales](https://oilprice.com/Energy/Energy-General/Private-Equity-Is-Circling-Utilities-as-AI-Reshapes-the-Grid.html) ⭐️ 7.0/10

Private equity firms are buying stakes in U.S. utilities as AI-driven electricity demand pushes utilities to sell non-core regulated assets to raise cash for grid buildout, a shift an industry investor says is unprecedented in 20 years.

rss · OilPrice.com · Aug 23, 18:00

**「Background」** AI data centers are sharply increasing power demand, and the Trump administration has pushed tech firms to supply their own energy; meanwhile, utilities face higher grid investment costs and are selling assets, according to the article.

**「Impact」** If the buildout proceeds, ordinary ratepayers could still bear grid upgrade costs even when data centers self-supply, and private investors could face a bubble once utilities resume buying assets, experts cited in the article warn.

**Tags**: `#private equity`, `#utilities`, `#artificial intelligence`, `#data centers`, `#energy infrastructure`

---

<a id="item-finance-news-9"></a>
### [China&\#x27;s big three telecom operators report H1 2026 profit declines](https://www.guancha.cn/economy/2026_08_21_828161.shtml) ⭐️ 7.0/10

China Mobile, China Telecom, and China Unicom all reported lower net profit attributable to shareholders for the first half of 2026, with declines of 6.3%, 14.9%, and 34.8%, respectively. Their combined average daily profit fell to 567 million yuan from 628 million yuan a year earlier, or about 61 million yuan less per day.

telegram · zaihuapd · Aug 23, 07:34

**「Background」** China Unicom said its near-halved profit reflected value-added tax policy adjustments and the timing of labor cost spending, while the new cloud and AI-focused businesses of all three carriers continued to grow quickly.

**Tags**: `#中国移动`, `#中国电信`, `#中国联通`, `#盈利下滑`, `#电信运营商`

---

<a id="item-finance-news-10"></a>
### [Walmart Stock Drops 9%](https://finance.yahoo.com/markets/stocks/articles/walmart-fell-9-m-not-153057565.html) ⭐️ 7.0/10

Walmart&\#x27;s stock fell 9%, raising concerns that the decline may signal broader economic weakness beyond the retailer itself.

openbb · PG · Aug 23, 15:30

**「Background」** Walmart reported its slowest comparable-sales growth in six years, with U.S. comparable sales up 2.6% against the 3.8% analysts expected. The 9% stock drop erased more than $80 billion in market value, raising questions about whether the weakness signals a broader consumer-spending slowdown rather than a Walmart-specific issue.

**「Broader impact」** Walmart&\#x27;s slump signals a broader pullback in U.S. consumer spending, weighed down by tariffs, high fuel costs, and geopolitical tensions, which could pressure other retailers and consumer-dependent businesses.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/quote/WMT/">Walmart Inc. (WMT) Stock Price, News, Quote &amp; History - Yahoo Finance</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/walmart-fell-9-m-not-153057565.html">Walmart Fell 9%. I’m Not Sure This Is Just a Walmart Problem</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/8/20/walmart-sees-sales-drop-as-us-consumer-spending-retreats">Walmart sees sales drop as US consumer spending ... | Al Jazeera</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2kzdmZYcUVSRmZnVTd4WXpqRmFDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Walmart reports slowest US sales growth since 2020...</a></li>

</ul>
</details>

**Tags**: `#Walmart`, `#Retail`, `#Stock Market`, `#Consumer Spending`, `#Market Analysis`

---

<a id="item-finance-news-11"></a>
### [Johnson &amp; Johnson&\#x27;s $5.5 Billion Talc Settlement and Legal Risk](https://finance.yahoo.com/markets/stocks/articles/johnson-johnson-5-5-billion-230104916.html) ⭐️ 7.0/10

Johnson &amp; Johnson has reached a $5.5 billion settlement to resolve talc-related lawsuits, a major step toward addressing its legal liabilities. The article also questions whether the legal risk is fully resolved for the company and its shareholders.

openbb · BRK-B · Aug 23, 23:01

**「Background」** Johnson &amp; Johnson has fought talc-related lawsuits for over a decade, alleging that its baby powder caused ovarian cancer, including failed bankruptcy tactics. The company now proposes a $5.5 billion settlement, conditioned on at least 95% of remaining claimants agreeing. Payments are expected to begin with $3 billion in 2027, with additional payments in 2028, and the total could exceed $5.5 billion depending on participation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tovima.com/world/jj-reaches-5-5-billion-talc-settlement-over-cancer-claims/">J&amp;J Reaches $ 5 . 5 Billion Talc Settlement Over Cancer... - tovima.com</a></li>
<li><a href="https://www.ksat.com/business/2026/07/28/johnson-johnson-proposes-55-billion-talc-settlement-to-end-marathon-legal-fight/">Johnson &amp; Johnson proposes $ 5 . 5 billion talc settlement to end...</a></li>
<li><a href="https://easternherald.com/2026/07/28/johnson-johnson-talc-settlement-5-billion-cancer-lawsuits/">J&amp;J $ 5 . 5 Billion Talc Settlement Ends Cancer Lawsuits</a></li>

</ul>
</details>

**Tags**: `#Johnson &amp; Johnson`, `#talc lawsuit`, `#legal settlement`, `#pharmaceutical`, `#investor analysis`

---

<a id="item-finance-news-12"></a>
### [Greg Abel Invests $23.5 Billion in Nine Stocks, Report Says](https://finance.yahoo.com/markets/stocks/articles/greg-abel-just-spent-23-162000632.html) ⭐️ 7.0/10

An article reports that Berkshire Hathaway&\#x27;s Greg Abel spent $23.5 billion across nine stocks, a major capital-allocation move. The article says one of the nine was the best of the bunch, but the available item does not name the individual stocks.

openbb · BRK-B · Aug 23, 16:20

**「Background」** Berkshire Hathaway is led by CEO Greg Abel, who took over after Warren Buffett retired at the end of 2025; the company has recently reworked its equity portfolio, cutting holdings from about 42 to 26 stocks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Greg_Abel">Greg Abel - Wikipedia</a></li>
<li><a href="https://simplywall.st/stocks/us/diversified-financials/nyse-brk.a/berkshire-hathaway">Berkshire Hathaway (NYSE:BRK.A) - Stock Analysis - Simply Wall St</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#Greg Abel`, `#capital allocation`, `#stock portfolio`, `#investment strategy`

---

<a id="item-finance-news-13"></a>
### [Sinopec H1 2026 Profit Jumps 19%](https://finance.yahoo.com/energy/articles/sinopec-reports-19-profit-jump-113126453.html) ⭐️ 7.0/10

Sinopec reported a 19% jump in profit for the first half of 2026, despite the Middle East crisis.

openbb · CL=F · Aug 23, 11:31

**「Background」** Sinopec is a Chinese state-owned oil refiner. In the first half of 2026 it operated amid a Middle East conflict involving Iran and falling domestic fuel demand, cutting crude processing by 5.6% and writing down 16 billion yuan in inventories, while refining margins rose 44.1% as it sourced more crude from outside the Middle East and benefited from procurement timing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/chinese-oil-refiner-sinopecs-half-year-profit-grows-19-3-despite-iran-war-falling-demand">Chinese oil refiner Sinopec ’s half-year profit grows 19 .3% despite Iran...</a></li>
<li><a href="https://www.technotime.net/16205">Sinopec H 1 2026 Net Profit Jumps 19 .3% to $3.81... | Techno Time</a></li>
<li><a href="https://nl.investing.com/news/earnings/sinopec-rapporteert-19-winstgroei-in-h1-2026-ondanks-crisis-in-middenoosten-897588">Sinopec rapporteert 19 % winstgroei in H 1 2026 ondanks crisis in...</a></li>

</ul>
</details>

**Tags**: `#Sinopec`, `#earnings`, `#energy sector`, `#oil &amp; gas`, `#profit jump`

---

<a id="item-finance-news-14"></a>
### [Inflation Hits 2.9%, Raising Worries About Interest Rate Hike](https://news.google.com/rss/articles/CBMijAFBVV95cUxNU2Vib0FIUXVTS2ZiZlBXbkxpdjNTVWRSaU5nQjE4ZktjOFlGTkdFWGFPeU1oQUhwSWViUWYybllXWHNOb1VwSzlMQXdscHd6eHlLX2NZbjVSRWIwRjhERGctOUVSMGRJUDFDYkhZcjM4a0dvUVhsYnVBdGtlYmlkRlU4WU81RmpyQjFYdg?oc=5) ⭐️ 7.0/10

Forbes reports inflation reached 2.9%, stoking fears that the central bank may raise interest rates. The rate hike is not confirmed and remains a concern rather than an announced policy change.

google\_news · Forbes · Aug 19, 11:50

**「Background」** Central banks often raise interest rates to combat high inflation, as higher borrowing costs tend to cool spending and price growth. In past surges, the U.S. Federal Reserve has increased rates by half a percentage point, and the latest 2.9% inflation figure has intensified market fears of a similar tightening.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=hDazaQ_RStQ">Interest Rate Hike : Why The Federal Reserve Is Increasing... - YouTube</a></li>

</ul>
</details>

**Tags**: `#inflation`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---