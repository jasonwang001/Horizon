---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 225 items, 24 important content pieces were selected

---

**Technology News**
1. [Spaghettifying DRAM: New AMD Privilege-Escalation Research](#item-tech-news-1) ⭐️ 9.0/10
2. [GPT-5.6 Sol Ultrafast claims 7x faster inference without accuracy loss](#item-tech-news-2) ⭐️ 8.0/10
3. [DeepSeek Harness Developer Preview Brings Full Agent Session Traceability](#item-tech-news-3) ⭐️ 8.0/10
4. [Choose Boring Technology and Spend Innovation Tokens Wisely](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepSeek V4 Pro 0813 Released with 1.7T Open Weights](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepMind SL2T Brings Sign-to-Text AI to Pixel 11 Gboard and Live Transcribe](#item-tech-news-6) ⭐️ 8.0/10
7. [Gemini 3.7 Flash: Pricing, Benchmarks, and Vision Quality Debated](#item-tech-news-7) ⭐️ 7.0/10
8. [Gloomberb: Bloomberg-style terminal UI for financial data](#item-tech-news-8) ⭐️ 7.0/10
9. [City2Graph Python library turns urban data into heterogeneous graphs for GNNs](#item-tech-news-9) ⭐️ 7.0/10
10. [WorldProof diagnoses world-model failures and shows pixel metrics can&\#x27;t rank models on robot video](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Hormuz Stalemate Keeps Oil Price Risk Elevated](#item-finance-news-1) ⭐️ 9.0/10
2. [Federal Reserve keeps interest rates unchanged in 9-3 vote](#item-finance-news-2) ⭐️ 9.0/10
3. [Bank of England Publishes July 2026 Monetary Policy Report](#item-finance-news-3) ⭐️ 9.0/10
4. [S&amp;P 500 profit margins on track for record 16.9% in Q2, FactSet says](#item-finance-news-4) ⭐️ 8.0/10
5. [YMTC overtakes Micron and Kioxia in NAND chip shipments](#item-finance-news-5) ⭐️ 8.0/10
6. [Solar Overtakes Wind in Global Electricity Generation for First Time](#item-finance-news-6) ⭐️ 8.0/10
7. [U.S. Backs X-Energy Reactor With Up to $2.15 Billion](#item-finance-news-7) ⭐️ 8.0/10
8. [Russian Diesel Exports Hit Multi-Year Low](#item-finance-news-8) ⭐️ 8.0/10
9. [Diesel Shortage Highlights Oil Market Squeeze](#item-finance-news-9) ⭐️ 8.0/10
10. [Ukraine Strikes 200,000-bpd Russian Refinery in Urals](#item-finance-news-10) ⭐️ 8.0/10
11. [CXMT Overtakes Tencent as China’s Most Valuable Company](#item-finance-news-11) ⭐️ 8.0/10
12. [Aboitiz Equity Ventures Reports 65% Net Income Jump in Q2 2026](#item-finance-news-12) ⭐️ 8.0/10
13. [Stocks Rise as Inflation Cools, Workday Jumps 18%](#item-finance-news-13) ⭐️ 8.0/10
14. [China’s Gig Workforce Hits 53 Million, Yet Oversupply Squeezes Incomes](#item-finance-news-14) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Spaghettifying DRAM: New AMD Privilege-Escalation Research](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas has released a GitHub repository titled &quot;skitter-creek-bath-salts&quot; describing a DRAM manipulation technique, dubbed &quot;Spaghettifying DRAM,&quot; that can escalate to ring-0 privileges on certain AMD processors. The README identifies AMD Jaguar, a low-power architecture from 2013, as a working target, while noting that Zen 3 has a different base address for memory controller registers. The technique is notable because it targets physical memory addressing and DRAM behavior rather than a conventional software bug, potentially exposing data usually hidden in privileged &quot;negative ring&quot; territory. Observers expect an accompanying Black Hat talk from Domas, who is known for his clear explanations of complex hardware and reverse-engineering topics. The full scope of affected CPU families remains unclear from the repository, with no direct evidence yet of impact on newer AMD processors.

hackernews · matt\_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**「Background」** Modern CPUs enforce security through privilege rings, with ring 0 \(kernel\) having the highest access and negative rings \(e.g., System Management Mode\) reserved for firmware. DRAM addressing is mediated by the memory controller, which can apply address scrambling for reliability and security; if an attacker can manipulate the controller&\#x27;s registers, they may remap physical memory to bypass protections. This research targets AMD&\#x27;s 16h family \(e.g., Jaguar\) and builds on prior work by Christopher Domas, a security researcher known for hardware and low-level exploit research.

**「Impact」** The most concrete consequence is that AMD Jaguar-based systems may be vulnerable to a DRAM-level attack that grants ring-0 privileges, potentially undermining protections normally reserved for the most privileged software layers; newer AMD families such as Zen 3 may have mitigations or altered register layouts, but the repository does not yet clarify their exposure.

**「Community Discussion」** Commenters praised Domas&\#x27;s presentation style and eagerly awaited the accompanying Black Hat talk, while others noted that the growing complexity and proprietary nature of modern DRAM controllers create an expansive attack surface. Some speculated that the technique could threaten console security if it reaches current hardware, and one commenter questioned the range of affected CPUs, observing that Jaguar is a 2013 design and asking what newer processors the attack actually works on.

<details><summary>References</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/amd-hardware-vulnerability-exposed-by-dram-address-scrambling-research">AMD DRAM Scrambling Exploit Bypasses Security Fences | Linxi News</a></li>
<li><a href="https://github.com/xoreaxeaxeax">xoreaxeaxeax (domas) · GitHub</a></li>

</ul>
</details>

**Tags**: `#hardware security`, `#DRAM`, `#privilege escalation`, `#AMD`, `#exploit`

---

<a id="item-tech-news-2"></a>
### [GPT-5.6 Sol Ultrafast claims 7x faster inference without accuracy loss](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras and OpenAI have announced GPT-5.6 Sol Ultrafast, a faster inference mode for OpenAI&\#x27;s GPT-5.6 Sol model, claiming a roughly 7x speedup without accuracy loss. In their evaluations, the model answered all 2,500 Humanity&\#x27;s Last Exam \(HLE\) questions in 11 hours and 11 minutes, compared with 78 hours and 27 minutes for Claude Fable 5. However, neither company explicitly confirmed that Ultrafast produces identical results to the regular GPT-5.6 Sol, and no pricing information was released. The announcement matters because faster inference could enable more iterative reasoning and higher throughput for users of frontier models.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**「Background」** Ultrafast is a newly announced service tier in the OpenAI API that runs GPT-5.6 Sol up to 14x faster than Standard processing, powered by Cerebras hardware and generating up to 750 output tokens per second. Cerebras, which builds wafer-scale chips for AI inference, says the mode is initially available to a select group of customers and claims no quality compromise; the announcement sparked community debate over whether the faster model truly matches the standard version&\#x27;s performance.

**「Impact」** For developers and organizations using GPT-5.6 Sol, Ultrafast could meaningfully reduce latency and cost per reasoning task if the accuracy-parity claim holds, but the lack of explicit equivalence testing and pricing details leaves the practical benefit uncertain.

**「Community Discussion」** Commenters were enthusiastic about speed&\#x27;s potential to improve iterative reasoning, but several noted that neither Cerebras nor OpenAI explicitly stated that Ultrafast matches regular GPT-5.6 Sol&\#x27;s accuracy, and the absence of pricing information left adoption costs unclear. Others welcomed the speed comparisons against Claude Fable 5 and Opus 4.8 but asked for more rigorous head-to-head benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT‑5.6 Sol at up to ... - OpenAI</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI - cerebras.ai</a></li>

</ul>
</details>

**Tags**: `#AI`, `#inference speed`, `#OpenAI`, `#Cerebras`, `#large language models`

---

<a id="item-tech-news-3"></a>
### [DeepSeek Harness Developer Preview Brings Full Agent Session Traceability](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek released an MIT-licensed developer preview of Harness, an open-source framework for building and observing AI agents with full session traceability. The tool records everything the model sees in an append-only session log, including system prompts, reasoning, tool calls and results, subagent scheduling, and context injections, and provides a Trajectory view for inspecting records by source. Users can resume, fork, search, and replay runs from the same event stream. An author notes the preview is early, with rough edges and compatibility-breaking changes expected, so developers should treat it as an unstable foundation rather than a production-ready release.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**「Background」** AI agents often chain multiple model calls, tool invocations, and subagent runs, making it difficult to understand why an agent made a particular decision or to reproduce a failure. DeepSeek Harness is a framework designed to address this by providing structured instrumentation for agent runs, and it builds on a plugin architecture that can hot-load and unload components without restarting the process. DeepSeek is primarily known for open-weight models, so this developer preview extends its open-source presence into agent tooling and observability.

**「Impact」** Developers building AI agents can now experiment with a fully traceable, MIT-licensed agent runtime that exposes complete run histories, but they should expect breaking changes and rough edges until a stable version is released.

**「Community Discussion」** Commenters largely welcomed the append-only traceability and hot-reload plugin architecture, with one praising traceability as a &quot;killer feature&quot; that US models&\#x27; obfuscated traces do not provide. Others tempered expectations, noting that the underlying Cordis system has existed for years, that the preview is early with potential compatibility-breaking changes, and that plugin-centric designs can feel burdensome; one reader summarized it as &quot;useful, but not that useful.&quot;

**Tags**: `#AI`, `#open-source`, `#agent-tooling`, `#observability`, `#DeepSeek`

---

<a id="item-tech-news-4"></a>
### [Choose Boring Technology and Spend Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

This 2015 essay argues that engineering organizations should deliberately choose boring, well-understood technologies for most of their stack, reserving novelty for areas where it provides a clear advantage. It introduces the framework of a fixed supply of about three &\#x27;innovation tokens&\#x27; per company, which should be spent sparingly because adopting unfamiliar technology carries long-term costs. The essay has remained influential, and in current discussions it is often cited to suggest that AI agents themselves should be the focus of innovation while the surrounding technology should be boring and familiar. The core tradeoff is between the benefits of new technology and the operational and cognitive burden it adds to a team.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**「Background」** Dan McKinley&\#x27;s essay &\#x27;Choose Boring Technology,&\#x27; published March 30, 2015, argues that engineering organizations should prefer mature, well-understood technologies and spend limited &\#x27;innovation tokens&\#x27; only on problems where novelty provides a distinct business advantage. The framework treats innovation as a finite budget: every new or exotic component consumes a token, and the supply is fixed for a long time. The essay became a widely cited engineering principle, later adapted into talks and a spoken-word version at venues such as the Wikimedia Foundation&\#x27;s developer conference.

**「Impact」** The innovation-token framework has become a practical decision-making tool for engineering leaders and product managers evaluating technology choices. In the current AI-agent era, it is being used to argue that teams should standardize on familiar &\#x27;in-distribution&\#x27; tools for agent infrastructure rather than chase otherwise attractive alternatives.

**「Community Discussion」** Commenters widely praise the essay, with one saying it is one of the most useful concepts they have used as a PM and engineering leader for explaining tradeoffs. Others extend the idea to AI agents, recommending that teams push their innovation tokens into agents while making the surrounding technology boring, though some push back and note caveats such as cases where previously &\#x27;boring&\#x27; technology is actually a poor fit for a new use case.

<details><summary>References</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Choose Boring Technology - Dan McKinley</a></li>
<li><a href="https://boringtechnology.club/">Choose Boring Technology</a></li>
<li><a href="https://www.laws-of-software.com/laws/choose-boring-technology/">Choose Boring Technology - Laws of Software</a></li>

</ul>
</details>

**Tags**: `#boring-technology`, `#engineering-culture`, `#technology-choice`, `#innovation-tokens`, `#software-architecture`

---

<a id="item-tech-news-5"></a>
### [DeepSeek V4 Pro 0813 Released with 1.7T Open Weights](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 is now available via API and on OpenRouter, and its open weights have been published on Hugging Face at 1.7 trillion parameters and 893 GB. The release appears with no official announcement page from DeepSeek, with availability confirmed through third-party listings and Hugging Face. Notably, Simon Willison observed very different pelican images generated for the low, medium, and high reasoning levels, an inconsistency he has not seen from other models. Benchmark figures, as far as can be determined, were released in the Official DeepSeek WeChat Group, then copied to a Reddit post that was removed by moderators and later reproduced in an ASCII-art table on Hacker News. The model follows prior DeepSeek open-weight releases including the April V4 Pro and July V4 Flash variants.

rss · Simon Willison · Aug 12, 23:59

**「Background」** DeepSeek has previously released open-weight language models, including the April DeepSeek-V4-Pro and the July DeepSeek-V4-Flash-0731, both available on Hugging Face. These releases are part of the broader trend of large open-weights models that can be downloaded and hosted locally, though the 893 GB size of the newest model makes local deployment practical only for organizations with substantial infrastructure.

**「Impact」** For developers and organizations, the immediate consequence is the ability to access DeepSeek V4 Pro 0813 through major API providers like OpenRouter and to download the 1.7T-parameter open weights for self-hosting, enabling local customization and inference without relying solely on a proprietary API endpoint. The lack of officially published benchmarks leaves its performance relative to other models uncertain, especially given the unusual distribution path for benchmark data.

**Tags**: `#deepseek`, `#llm`, `#open-weights`, `#huggingface`, `#api`

---

<a id="item-tech-news-6"></a>
### [DeepMind SL2T Brings Sign-to-Text AI to Pixel 11 Gboard and Live Transcribe](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind introduced SL2T, a large multilingual sign language-to-text model, and deployed it for the first time in consumer products: Pixel 11&\#x27;s Gboard keyboard and Live Transcribe, initially supporting American Sign Language to English. The model was trained on more than 100,000 hours of signing data across 50+ sign languages and achieves a zero-shot score of 70 BLEURT on the FLEURS-ASL benchmark, far exceeding previous records. To protect privacy, SL2T processes only hand and body keypoints rather than raw video frames. Google says support will expand to more devices and languages, making this a notable step toward accessible real-time sign language understanding.

telegram · zaihuapd · Aug 13, 08:55

**「Background」** Sign language recognition has traditionally been difficult because models must capture continuous motion, grammar, and facial expressions across many distinct sign languages. BLEURT is a learned metric for evaluating translation quality, and FLEURS-ASL is a benchmark for ASL-to-text translation; SL2T&\#x27;s 70 zero-shot score represents a large jump over prior reported results. DeepMind&\#x27;s approach uses pose keypoints to reduce privacy risk while still enabling translation.

**「Impact」** Pixel 11 owners using ASL now get sign-to-English text in Gboard and real-time Live Transcribe captions without raw video leaving the device, though other devices and sign languages are not yet supported.

**Tags**: `#DeepMind`, `#sign language AI`, `#accessibility`, `#machine learning`, `#Pixel 11`

---

<a id="item-tech-news-7"></a>
### [Gemini 3.7 Flash: Pricing, Benchmarks, and Vision Quality Debated](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google has introduced Gemini 3.7 Flash, a new model in its Gemini API lineup that arrives roughly three weeks after Gemini 3.6 Flash. The release has sparked community discussion over its introductory pricing, which commenters say is scheduled to double on December 31, 2026 \(or January 1, 2027\) to $1.50 per 1M input tokens and $7.50 per 1M output tokens. Developers also report mixed hands-on results: an image-to-HTML test shows strong vision performance for its price class, though Anthropic&\#x27;s Opus 5 remains the best-in-class for that task, and a DeepSWE 1.1 benchmark run places it behind OpenAI&\#x27;s GPT-5.6 Luna \(Max\). The API reference is available at ai.google.dev.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**「Background」** Google&\#x27;s Gemini Flash line is a lower-cost, high-volume series of AI models positioned for tasks like summarization, parsing, and coding assistance. Gemini 3.7 Flash launched with introductory pricing of $0.75 per million input tokens and $3.75 per million output tokens through December 31, 2026, after which it reverts to $1.50 and $7.50 per million tokens; that intro pricing matches the half-price launch deal Google used for Gemini 3.6 Flash. The new model is aimed at coding and agentic workflows and is benchmarked against rivals such as GPT-5.6 Terra and Claude.

**「Impact」** For developers choosing models for low-cost, high-volume text tasks, Gemini 3.7 Flash offers a competitively priced option with capable vision-to-HTML conversion, but the scheduled price increase and stronger benchmark results from cheaper rivals like GPT-5.6 Luna may limit its appeal.

**「Community Discussion」** Reactions are mixed: jjcm found Gemini 3.7 Flash&\#x27;s image-to-HTML output strong relative to comparable models, though Opus 5 still led, while Alifatisk and wxw argued that GPT-5.6 Luna undercuts Flash on both cost and DeepSWE benchmarks. Simon Willison called the introductory pricing &\#x27;really weird&\#x27; and questioned why users would still rely on the model when the price doubles.

<details><summary>References</summary>
<ul>
<li><a href="https://venturebeat.com/technology/googles-gemini-3-7-flash-targets-coding-and-agents-with-a-50-introductory-price-cut">Google’s Gemini 3.7 Flash targets coding and agents with a 50% introductory price cut | VentureBeat</a></li>
<li><a href="https://www.techtimes.com/articles/324387/20260813/google-cuts-gemini-37-flash-price-half-it-claims-top-claude-business-workflows.htm">Google Cuts Gemini 3.7 Flash Price in Half as It Claims to Top Claude on Business Workflows</a></li>
<li><a href="https://officechai.com/ai/gemini-3-7-flash-benchmarks/">Google Releases Gemini 3.7 Flash, Competes With GPT 5.6 Terra &amp; Muse Spark 1.2 On Benchmarks</a></li>

</ul>
</details>

**Tags**: `#gemini`, `#google`, `#ai-models`, `#machine-learning`, `#release`

---

<a id="item-tech-news-8"></a>
### [Gloomberb: Bloomberg-style terminal UI for financial data](https://gloom.sh/) ⭐️ 7.0/10

Gloomberb is an open-source terminal UI that presents financial data in a Bloomberg-like tiling interface, drawing attention from developers interested in TUI applications and financial tools. The project is hosted at gloom.sh and was submitted to Hacker News, where discussion centered on its usability, installation method, and comparison with Bloomberg&\#x27;s data services. Community members noted that Bloomberg&\#x27;s value comes from its proprietary data connections rather than its terminal interface, while Gloomberb appears to rely on free or alternative data sources. The project uses a curl-based install script for convenience, which sparked debate about dependency management and stack transparency. No official source content was provided, so specific versions, data sources, and installation details remain unspecified.

hackernews · rbanffy · Aug 13, 13:52 · [Discussion](https://news.ycombinator.com/item?id=49285982)

**「Background」** The Bloomberg Terminal is a computer software system provided by Bloomberg L.P. that lets finance professionals monitor and analyze real-time market data, place trades, and access news, and it has been a standard in the industry for decades. Gloomberb is an open-source terminal UI that mimics the Bloomberg Terminal&\#x27;s tiled, amber-on-black look for financial data, but it does not include Bloomberg&\#x27;s proprietary data feed, making it relevant to developers interested in terminal-based dashboards and open-source alternatives to expensive commercial systems.

**「Impact」** For developers and hobbyist traders who want a Bloomberg-style dashboard without paying Bloomberg&\#x27;s roughly $31,980 annual fee, Gloomberb offers a free, terminal-based alternative, though it does not provide Bloomberg&\#x27;s data connections. The discussion also highlights a broader concern about curl install scripts obscuring dependencies, which may affect how users evaluate the project&\#x27;s trustworthiness.

**「Community discussion」** Commenters expressed interest in the tool&\#x27;s tiling UI and general usefulness, while also criticizing the lack of stack transparency in its install script and noting that many competitors exist, such as the proprietary Godel Terminal. One user wondered how to make panes dynamically follow a selected ticker, a feature that works in the default research panes but was not obvious for custom panes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bloomberg_Terminal">Bloomberg Terminal - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#terminal`, `#open source`, `#finance`, `#TUI`, `#developer tools`

---

<a id="item-tech-news-9"></a>
### [City2Graph Python library turns urban data into heterogeneous graphs for GNNs](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph is a new open-source Python library that converts urban geospatial data into analysis-ready heterogeneous graphs for spatial analysis, network analysis, and Graph Neural Networks \(GeoAI\). The library supports morphological graphs of buildings, streets, and urban fabric from OpenStreetMap and Overture Maps; transportation graphs from GTFS and GBFS feeds loaded through DuckDB; mobility data from origin-destination matrices and flow datasets; and proximity/contiguity graphs using KNN, Delaunay, Gilbert, Waxman, and queen/rook methods under multiple distance metrics. It also enables heterogeneous graphs with multiple node and edge types plus metapath-derived edges, and provides round-trip conversion between GeoDataFrames, NetworkX, rustworkx, and PyTorch Geometric Data/HeteroData while preserving geometries and attributes. The peer-reviewed paper describing the library was published in Computers, Environment and Urban Systems, volume 130, article 102492, authored by Sato, Pietrostefani, Mahabir, and Arribas-Bel \(2026\). The repository is available at https://github.com/c2g-dev/city2graph.

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · Aug 13, 11:59

**「Background」** Heterogeneous graphs contain multiple types of nodes and edges, such as buildings, street segments, and transit stops, which lets urban data be modeled with richer relational structure than flat feature tables. Graph Neural Networks operate on such graphs to learn from geospatial and urban data, but constructing these graphs from raw sources like OSM or transit feeds is often a manual, error-prone step. City2Graph aims to automate and standardize that graph construction pipeline.

**「Impact」** Researchers and practitioners in GeoAI and urban computing can now use City2Graph to build heterogeneous graph representations of cities directly from common open data sources, with a published citation and an open invitation for contributions and feature requests.

**Tags**: `#graph-neural-networks`, `#geospatial`, `#urban-computing`, `#python-library`, `#GeoAI`

---

<a id="item-tech-news-10"></a>
### [WorldProof diagnoses world-model failures and shows pixel metrics can&\#x27;t rank models on robot video](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 7.0/10

WorldProof, a new open-source diagnostic tool for world models, compares rollout predictions against ground truth and physical invariants to pinpoint where and why predictions fail. Validating it on real robot video revealed that pixel metrics like SSIM and PSNR often cannot rank models at all: a last-frame copy baseline achieved 0.983 SSIM and 53.9 dB PSNR on 30fps SO-101 arm recordings with flat error across a 6-step horizon, meaning every model ties and the evaluation lacks discriminative power. On DROID footage at 15fps over 48 steps, the baseline showed three regimes—near-perfect ties through step 3, a separable steep decline from steps 4 to 24, and a decorrelated floor around 0.20 SSIM and 10.3 dB after step 28—indicating a usable evaluation window of roughly 8 to 24 steps that depends on frame rate and task speed. The tool is Apache-2.0, installable via pip, reads LeRobotDataset v3.0 directly, and includes multiple fidelity, calibration, and invariant metrics, with caveats that LPIPS diverges from other pixel metrics and that the default FVD extractor differs from published I3D numbers.

reddit · r/MachineLearning · /u/georgia\_bucea · Aug 13, 19:58

**「Background」** World models are machine learning systems that predict future video frames from a starting context and action sequence, often evaluated by comparing predicted frames to ground truth with pixel-level metrics like SSIM and PSNR. On real robot video, those metrics can lose discriminative power because a static background or unsuitable horizons can make naive baselines score as well as sophisticated models. To improve reliability of such evaluations, recent methodology promotes interquartile mean \(IQM\) and stratified bootstrap confidence intervals instead of simple mean/standard deviation, as popularized by Agarwal et al.&\#x27;s rliable package \(NeurIPS 2021\).

**「Impact」** Practitioners evaluating world models on real robot video should measure horizon curves on their own data rather than inheriting defaults, because both short horizons and long horizons can produce ties that hide model quality. The 8-to-24-step usable window identified for DROID-style footage provides a concrete starting point for designing evaluations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/google-research/rliable">GitHub - google-research/rliable: [NeurIPS&#x27;21 Outstanding ...</a></li>
<li><a href="https://research.google/blog/rliable-towards-reliable-evaluation-reporting-in-reinforcement-learning/">RLiable: Towards Reliable Evaluation &amp; Reporting in ...</a></li>

</ul>
</details>

**Tags**: `#world models`, `#evaluation metrics`, `#video prediction`, `#robotics`, `#open source`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Hormuz Stalemate Keeps Oil Price Risk Elevated](https://oilprice.com/Energy/Oil-Prices/Hormuz-Stalemate-Raises-Risk-of-120-Oil.html) ⭐️ 9.0/10

The Strait of Hormuz remains mostly closed after months of U.S.-Iran tensions, and analysts warn that if the stalemate lasts into early Q4, oil prices could spike to $120-140 per barrel, according to Kieran Tompkins, senior climate and commodities economist at Capital Economics. Brent crude rose above $89 per barrel this week, while tanker traffic in the strait hit two-month lows.

rss · OilPrice.com · Aug 13, 15:00

**「Background」** The U.S.-Iran war began on February 28, and since then both sides have claimed control of the Strait of Hormuz, a narrow waterway through which much of the world&\#x27;s oil passes. After five and a half months of negotiations and threats, the talks are at a stalemate, with Iran saying the strait will remain closed unless the U.S. ends the war and meets its conditions, and President Trump saying the U.S. has total control.

**「Impact」** Refined fuels such as diesel, gasoil, and jet fuel are already significantly tighter than crude, and global inventories are depleting. If the strait stays closed, businesses and consumers could face higher fuel prices and shortages as refining margins hit records and product supply bottlenecks persist.

**Tags**: `#Oil prices`, `#Strait of Hormuz`, `#Geopolitical risk`, `#Supply disruption`, `#Energy markets`

---

<a id="item-finance-news-2"></a>
### [Federal Reserve keeps interest rates unchanged in 9-3 vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

The Federal Reserve, the U.S. central bank, voted 9-3 to keep its benchmark interest rate unchanged, leaving borrowing costs steady for now.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Reserve, the U.S. central bank, kept its benchmark interest rate at 3.5%-3.75%, with three of the 12 voters dissenting in favor of a hike, and signaled another possible increase at its next meeting in September.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-leaves-interest-rate-unchanged-180102302.html">Federal Reserve leaves interest rate unchanged in 9 - 3 vote , but...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pJbTlyVkVSSHUzb3dpdmpXX2dpZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Fed&#x27;s interest rate meeting - Overview</a></li>
<li><a href="https://news.meaww.com/video/30-07-2026-lfc-02-ms6xuygf">Kevin Warsh: Fed Votes 9 - 3 to Keep Interest Rates Unchanged</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#economy`

---

<a id="item-finance-news-3"></a>
### [Bank of England Publishes July 2026 Monetary Policy Report](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

The Bank of England has published its July 2026 Monetary Policy Report, which sets out UK monetary policy decisions and the central bank’s latest economic outlook. No specific interest-rate changes or forecast figures were included in the available announcement.

google\_news · Bank of England · Jul 30, 07:00

**「Background」** The UK&\#x27;s central bank, the Bank of England, publishes a quarterly Monetary Policy Report that sets out economic analysis and inflation projections. Its Monetary Policy Committee uses this report to decide interest rate changes, aiming to keep inflation low and stable.

**「Impact on UK borrowers」** UK households and businesses with variable-rate loans tied to Bank Rate will keep their current borrowing costs after the Bank of England held the rate at 3.75% in July 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/monetary-policy-report">Monetary Policy Reports | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/monetary-policy">Monetary policy | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/">Home | Bank of England</a></li>
<li><a href="https://www.forexfactory.com/news/1410968-bank-of-england-holds-uk-interest-rate-steady">Bank of England holds UK interest rate steady at 3.75... | Forex Factory</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#economic outlook`, `#UK`

---

<a id="item-finance-news-4"></a>
### [S&amp;P 500 profit margins on track for record 16.9% in Q2, FactSet says](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 8.0/10

S&amp;P 500 companies are on track for a record 16.9% net profit margin in the second quarter, according to FactSet, up from 14.8% in the first quarter and 12.9% a year earlier.

rss · CNBC Finance · Aug 13, 20:21

**「Background」** Net profit margin is the share of revenue a company keeps after all expenses; FactSet has tracked the S&amp;P 500 measure since 2009, and while Alphabet and Amazon are the biggest contributors, the margin is also a record 15% without them.

**Tags**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#stock market`, `#FactSet`

---

<a id="item-finance-news-5"></a>
### [YMTC overtakes Micron and Kioxia in NAND chip shipments](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 8.0/10

Yangtze Memory Technologies \(YMTC\) rose to third place in global NAND memory chip shipments in the second quarter with a 14% share, overtaking Micron and Kioxia and trailing only Samsung and SK hynix, according to Counterpoint Research.

rss · CNBC Finance · Aug 13, 02:59

**「Background」** NAND chips are memory that retains data when devices are powered off, and YMTC had narrowly beaten Kioxia a year ago before falling back in following months, according to Counterpoint.

**「Impact」** Counterpoint projects YMTC will pull further ahead in 2027 and 2028, which could intensify competitive pressure on Micron and Kioxia in the NAND segment even though YMTC still lags them in revenue.

**Tags**: `#NAND memory`, `#semiconductors`, `#YMTC`, `#market share`, `#competition`

---

<a id="item-finance-news-6"></a>
### [Solar Overtakes Wind in Global Electricity Generation for First Time](https://oilprice.com/Alternative-Energy/Solar-Energy/Solar-Surpasses-Wind-In-Global-Electricity-Generation-For-The-First-Time.html) ⭐️ 8.0/10

Solar overtook wind in global electricity generation for the first time in 2025, with solar producing 2,811 terawatt-hours \(8.7% of the world total\) versus wind&\#x27;s 2,714 TWh \(8.4%\), according to the Energy Institute&\#x27;s Statistical Review. Renewables supplied about 33.4% of global electricity, up 9.1% from the prior year.

rss · OilPrice.com · Aug 13, 20:00

**「Background」** The figures come from the Energy Institute’s Statistical Review of World Energy, the long-running annual energy data review formerly published by bp. As recently as 2015, global wind generation was 832 terawatt-hours \(TWh\), more than three times solar’s 257 TWh, making solar’s 2025 milestone particularly notable.

**「Impact」** China drove much of the solar leap, generating nearly 42% of global solar electricity, but the review notes that renewable supply met only about 40% of the increase in total global energy demand in 2025, so renewables are still largely adding new supply rather than displacing fossil fuels at a global scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.energyinst.org/__data/assets/pdf_file/0004/1822009/Statistical-Review-of-World-Energy-2026-Summary-version.pdf">2026 | th edition Statistical Review of World Energy</a></li>
<li><a href="https://www.energyinst.org/statistical-review">Home | Statistical Review of World Energy</a></li>

</ul>
</details>

**Tags**: `#solar energy`, `#wind energy`, `#global electricity`, `#renewable energy`, `#energy transition`

---

<a id="item-finance-news-7"></a>
### [U.S. Backs X-Energy Reactor With Up to $2.15 Billion](https://oilprice.com/Latest-Energy-News/World-News/US-Backs-X-Energy-Reactor-With-Up-to-215-Billion.html) ⭐️ 8.0/10

The U.S. Department of Energy has told X-energy it will provide up to $2.15 billion in cost-shared funding for an advanced nuclear reactor at Dow’s Seadrift, Texas, industrial complex, including $1 billion in additional money on top of earlier support since 2021. Federal funds must be matched by private spending, and the companies target operation in the early 2030s.

rss · OilPrice.com · Aug 13, 19:30

**「Background」** The project is part of the U.S. Advanced Reactor Demonstration Program, which helps move next-generation reactor designs toward commercial deployment; X-energy and Dow submitted a construction permit application to U.S. regulators last year.

**「Impact」** The developers expect it to become the first grid-scale advanced nuclear reactor serving a North American industrial site, supplying electricity and industrial steam to Dow’s Seadrift petrochemical and plastics complex.

**Tags**: `#Nuclear Energy`, `#Government Funding`, `#Energy Policy`, `#X-energy`, `#Dow`

---

<a id="item-finance-news-8"></a>
### [Russian Diesel Exports Hit Multi-Year Low](https://oilprice.com/Energy/Energy-General/Russias-Diesel-Exports-Crash-to-Multiyear-Low-amid-Tight-Global-Market.html) ⭐️ 8.0/10

Russia’s diesel and gasoil exports fell to an estimated 80,000 barrels per day \(bpd\) in the first seven days of August, a multiyear low and down from about 1 million bpd last year, according to data compiled by Bloomberg and cited by Oilprice, as Ukrainian drone attacks and Russian export restrictions squeezed global fuel markets.

rss · OilPrice.com · Aug 13, 19:00

**「Background」** Russia has faced gasoline and diesel shortages for more than three months after Ukrainian drone strikes forced many refineries offline, prompting Moscow to extend restrictions on diesel exports.

**「Impact」** The International Energy Agency said tighter refined-fuel markets boosted profit margins for refineries in the Atlantic Basin to record highs.

**Tags**: `#Russia`, `#diesel exports`, `#Ukraine drone attacks`, `#global oil market`, `#IEA`

---

<a id="item-finance-news-9"></a>
### [Diesel Shortage Highlights Oil Market Squeeze](https://oilprice.com/Energy/Crude-Oil/Jefferies-Diesel-Cracks-Reveal-the-Real-Oil-Market-Squeeze.html) ⭐️ 8.0/10

Record diesel refining margins—the profit from turning crude into diesel—point to a global oil-market squeeze, and the International Energy Agency has raised its forecast for this quarter&\#x27;s supply deficit to 1.8 million barrels a day, more than double its previous estimate. Brent crude futures held near $90 per barrel before easing to around $87 early Thursday.

rss · OilPrice.com · Aug 13, 17:00

**「Background」** Diesel cracks, the gap between diesel and crude prices, are above their prior record highs, meaning tightness is showing up in refined fuels rather than crude itself; analysts and the IEA warn the squeeze could persist while US-Iran talks remain stalled and the Strait of Hormuz stays blockaded.

**「Impact」** Trucking, shipping, farming, and other diesel-dependent businesses could face continued high fuel costs, as Bank of America warned the diesel market is likely to stay tight, volatile, and expensive into next year.

**Tags**: `#oil`, `#diesel`, `#geopolitics`, `#IEA`, `#supply`

---

<a id="item-finance-news-10"></a>
### [Ukraine Strikes 200,000-bpd Russian Refinery in Urals](https://oilprice.com/Latest-Energy-News/World-News/Ukraine-Strikes-Gazproms-200000-Bpd-Salavat-Refinery-in-the-Urals.html) ⭐️ 8.0/10

Ukraine struck Gazprom&\#x27;s 200,000-barrel-per-day Salavat refinery in the Urals on Thursday, causing a fire, as part of attacks that have forced Russia to curb fuel exports and import gasoline. Russian refinery runs averaged about 3.6 million bpd in July, more than 30% below seasonal levels, according to EA Analytics estimates cited by Bloomberg.

rss · OilPrice.com · Aug 13, 15:30

**「Background」** Another Urals refinery, the 120,000-bpd Orsknefteorgsintez plant, has completely stopped operations after earlier drone strikes, with repairs potentially taking up to six months, according to regional governor Yevgeny Solntsev.

**「Impact」** The outages have contributed to gasoline shortages, prompting Russia to restrict exports of gasoline, diesel and jet fuel and to import gasoline; a 42,000-ton cargo from India arrived on August 5, according to Kpler.

**Tags**: `#Ukraine conflict`, `#Russian oil`, `#refinery attack`, `#energy markets`, `#fuel exports`

---

<a id="item-finance-news-11"></a>
### [CXMT Overtakes Tencent as China’s Most Valuable Company](https://www.bloomberg.com/news/articles/2026-08-13/cxmt-overtakes-tencent-to-become-most-valuable-chinese-company) ⭐️ 8.0/10

CXMT overtook Tencent to become China’s most valuable listed company, with a market capitalization of $524 billion as of Thursday versus Tencent’s $510 billion, after the memory-chip maker’s Shanghai listing last month and as Tencent’s shares fell on higher AI investment.

telegram · zaihuapd · Aug 13, 10:10

**「Background」** CXMT, founded in 2016 and based in Hefei, is China&\#x27;s top maker of DRAM memory chips used in phones, PCs and servers; it listed on the Shanghai stock exchange in July 2026. Tencent&\#x27;s shares have fallen this year as the company increases spending on artificial intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://chinabizinsider.com/tencent-isolates-ai-costs-in-q1-2026-revealing-resilient-core-bankrolling-generative-pivot/">Tencent Q1 2026: Core Profits Bankroll AI Pivot</a></li>

</ul>
</details>

**Tags**: `#CXMT`, `#Tencent`, `#market cap`, `#semiconductor`, `#Chinese tech`

---

<a id="item-finance-news-12"></a>
### [Aboitiz Equity Ventures Reports 65% Net Income Jump in Q2 2026](https://finance.yahoo.com/markets/stocks/articles/aboitiz-equity-ventures-inc-aboif-010543098.html) ⭐️ 8.0/10

Aboitiz Equity Ventures reported that its net income for the second quarter of fiscal 2026 surged 65%, according to the company&\#x27;s earnings call highlights.

openbb · PG · Aug 13, 01:05

**「Background」** Aboitiz Equity Ventures Inc. is a Philippine holding company whose businesses include power, banking and financial services, food, infrastructure, and real estate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Aboitiz_Equity_Ventures">Aboitiz Equity Ventures - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#net income`, `#Aboitiz Equity Ventures`, `#Philippines`, `#earnings call`

---

<a id="item-finance-news-13"></a>
### [Stocks Rise as Inflation Cools, Workday Jumps 18%](https://finance.yahoo.com/markets/stocks/articles/stock-market-today-aug-13-213637440.html) ⭐️ 8.0/10

U.S. stocks rose on Aug. 13 after a report showed inflation cooling, and Workday shares climbed 18% in the session.

openbb · GC=F · Aug 13, 21:36

**「Background」** The market was reacting to softer wholesale and consumer inflation figures, which reinforced expectations that the Federal Reserve will not raise interest rates at its next meeting; lower rates tend to support stock prices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/coverage/stock-market-today/2026/08/13/stock-market-today-aug-13-stocks-rise-as-inflation-cools-workday-soars-18/">Stock Market Today , Aug . 13 : Stocks Rise as Inflation Cools ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-12/stock-market-today-dow-s-p-live-updates">Stock Market Today : Dow, S&amp;P Live Updates for August 13</a></li>

</ul>
</details>

**Tags**: `#inflation`, `#stock market`, `#Federal Reserve`, `#Workday`, `#economic data`

---

<a id="item-finance-news-14"></a>
### [China’s Gig Workforce Hits 53 Million, Yet Oversupply Squeezes Incomes](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 7.0/10

China’s economic slowdown is squeezing employment: as of 2025, food-delivery and ride-hailing drivers exceed 53 million, up 10 million in two years, but the gig labor market is oversupplied.

telegram · zaihuapd · Aug 13, 06:40

**「Background」** A real-estate slump, weak consumption, manufacturing contraction and automation have pushed surplus workers into gig roles, which are now attracting more workers than there is demand.

**「Impact」** For the drivers affected, the glut means thinner earnings and longer idle times—at Shanghai Pudong, Beijing Daxing and Chengdu Tianfu airports, queues can last up to 7, 8 and 10 hours.

**Tags**: `#China economy`, `#employment`, `#gig economy`, `#labor market`, `#ride-hailing`

---