---
layout: default
title: "Horizon Summary: 2026-09-17 (EN)"
date: 2026-09-17
lang: en
---

> From 258 items, 25 important content pieces were selected

---

**Technology News**
1. [Hackers Breach Flock Camera, Exposing Hardcoded Credentials](#item-tech-news-1) ⭐️ 8.0/10
2. [NVIDIA Announces Official Rust Tracks for CUDA GPU Kernels](#item-tech-news-2) ⭐️ 7.0/10
3. [4B Query Planner Claimed 81% Faster Than Postgres](#item-tech-news-3) ⭐️ 7.0/10
4. [Datasette 0.65.5 Fixes Trailing-Newline Table Permission Bypass](#item-tech-news-4) ⭐️ 7.0/10
5. [TMLR inquiry finds most authors of desk-rejected papers could not explain submissions](#item-tech-news-5) ⭐️ 7.0/10
6. [GoBench benchmarks LLMs on 9x9 Go against KataGo](#item-tech-news-6) ⭐️ 7.0/10
7. [Cloudflare adds AI training block setting while preserving search indexing](#item-tech-news-7) ⭐️ 7.0/10
8. [Apple 2nm A20 Pro in iPhone 18 Pro detailed by Geekerwan](#item-tech-news-8) ⭐️ 7.0/10
9. [Sina Cloud SAE shutdown threatens early Bilibili video source files](#item-tech-news-9) ⭐️ 7.0/10
10. [Micron Claims First 512GB DDR5 RDIMM, Targets 2027 Production](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Fed hikes rates a quarter point with unanimous vote](#item-finance-news-1) ⭐️ 9.0/10
2. [Fed raises rates 25 basis points, signals another hike this year](#item-finance-news-2) ⭐️ 9.0/10
3. [Tanker Rates Top $1 Million a Day as Hormuz Disruption Tightens Oil Shipping](#item-finance-news-3) ⭐️ 9.0/10
4. [Saudi Pipeline Attack Cuts Crude Exports to Europe](#item-finance-news-4) ⭐️ 9.0/10
5. [Bank of England Under Pressure to Raise Rates as Gilts Sell Off and Energy Prices Surge](#item-finance-news-5) ⭐️ 9.0/10
6. [US Fed raises interest rates for first time in three years](#item-finance-news-6) ⭐️ 9.0/10
7. [Federal Reserve Raises Interest Rates as Inflation Persists](#item-finance-news-7) ⭐️ 9.0/10
8. [Fed Raises Rates to 3.75%–4%, Times of India Headline Reports](#item-finance-news-8) ⭐️ 9.0/10
9. [Gold Pares Gains as Fed Raises Rates for First Time in Over Three Years](#item-finance-news-9) ⭐️ 9.0/10
10. [Fed raises interest rates for first time in three years](#item-finance-news-10) ⭐️ 9.0/10
11. [Fed raises rates 25 basis points, signals one more hike this year](#item-finance-news-11) ⭐️ 9.0/10
12. [Federal Reserve Holds Interest Rates Steady, Signals Possible Future Hike](#item-finance-news-12) ⭐️ 9.0/10
13. [Pinglu Canal Opens as New Southwest China–ASEAN Shipping Route](#item-finance-news-13) ⭐️ 8.0/10
14. [Hong Kong announces 11 measures to encourage childbirth](#item-finance-news-14) ⭐️ 7.0/10
15. [Unverified Post Claims Fed Raised Rates 25 Basis Points, First Hike Since 2023](#item-finance-news-15) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Hackers Breach Flock Camera, Exposing Hardcoded Credentials](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 8.0/10

A Wired report, discussed on Hacker News, describes hackers gaining access to a Flock license-plate-reader camera and finding hardcoded credentials and other security vulnerabilities in the widely deployed surveillance hardware. According to community analysis, the hardcoded value is an API key that can be used to request plaintext-stored credentials that appear to grant access to Flock&\#x27;s servers, though commenters note it remains unclear what an authenticated attacker could do as a camera. Commenters sharply criticized Flock&\#x27;s vulnerability disclosure policy, saying it appears to welcome reports only when researchers do not interact with the device or download its data, and faulted the company&\#x27;s secure-boot and key-management practices. The discussion also notes the reporting was done with 404 Media, that Distributed Denial of Secrets published partition images from the camera, and that one commenter argues the data is accessible to anyone with physical access and is not suitably encrypted.

hackernews · driverdan · Sep 16, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49726586)

**「Background」** Flock Safety builds automated license plate recognition \(ALPR\) cameras that are widely deployed by police departments and community groups to log vehicle movements in public spaces. Because the devices are physically accessible, their security depends on practices such as secure boot, encryption of stored keys and credentials, and a functioning vulnerability disclosure process; prior reporting has identified dozens of flaws in Flock hardware and software, including hardcoded passwords, and credentials tied to Flock have reportedly traded on dark web markets. Flock has said it takes security seriously, maintains a public vulnerability disclosure policy, and that unauthorized removal or tampering with a camera is illegal.

**「Impact」** For the police agencies and municipalities that deploy Flock&\#x27;s license-plate readers, the reported hardcoded API key and plaintext credentials mean anyone with brief physical access to a camera could extract secrets that appear to unlock Flock&\#x27;s servers, potentially exposing the nationwide vehicle-tracking data those agencies contribute to — a system already criticized by the EFF and ACLU. Commenters caution that it remains unproven what an attacker who successfully authenticates as a camera could ultimately do.

**「Community Discussion」** Commenters broadly agreed that hardcoded credentials and weak secure-boot/key management reflect poor security engineering, with some describing Flock&\#x27;s disclosure policy as performative because it excludes device interaction or data downloads. Several also stressed that deploying such hardware in public spaces makes local physical access part of the threat model, though they acknowledged uncertainty about the exact impact of authenticating as a camera.

<details><summary>References</summary>
<ul>
<li><a href="https://simeononsecurity.com/articles/flock-safety-camera-security-vulnerabilities-research-2026/">Flock Safety Camera Vulnerabilities: 50+ Flaws Found</a></li>
<li><a href="https://cybernews.com/privacy/hackers-flock-teardown-encryption-key-secrets/">Flock camera hacked: hackers crack open spy camera secrets ...</a></li>
<li><a href="https://byteiota.com/flock-safety-hardcoded-53-passwords-in-police-cameras/">Flock Safety Hardcoded 53 Passwords in Police Cameras</a></li>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.aclu.org/news/privacy-technology/tracking-alpr-cameras/despite-new-updates-flocks-creepy-cameras-remain-major-civil-liberties-threat">Despite &#x27;New&#x27; Updates, Flock&#x27;s Creepy Cameras Remain Major Civil Liberties Threat | American Civil Liberties Union</a></li>

</ul>
</details>

**Tags**: `#security-vulnerabilities`, `#surveillance`, `#IoT-hardware`, `#hardcoded-credentials`, `#privacy`

---

<a id="item-tech-news-2"></a>
### [NVIDIA Announces Official Rust Tracks for CUDA GPU Kernels](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 7.0/10

NVIDIA announced two tracks for writing CUDA GPU kernels in Rust on its official developer blog. The vendor-backed move brings Rust&\#x27;s safety guarantees to GPU kernel development, which could appeal to systems programmers seeking safer alternatives to CUDA C++. The announcement describes the effort as two tracks and is not yet a widely deployed release. The Hacker News discussion around the post drew 210 points and 72 comments, with debate about safety, lock-in, and existing Rust GPU tooling.

hackernews · nonmaskable · Sep 16, 11:15 · [Discussion](https://news.ycombinator.com/item?id=49724881)

**「Background」** GPU kernels for NVIDIA hardware have traditionally been written in CUDA C++ or CUDA Python, while Rust could only launch kernels whose code was authored in another language. NVIDIA&\#x27;s CUDA Rust effort aims to close that gap with two tracks: cuda-oxide, a custom rustc codegen backend that compiles Rust MIR through LLVM to PTX and requires a pinned nightly toolchain, and cutile-rs for the newer Tile model. The announcement, discussed in NVIDIA&\#x27;s developer blog and forums, positions Rust&\#x27;s safety guarantees as an alternative for kernel code that has historically been tied to CUDA&\#x27;s proprietary ecosystem.

**「Impact」** Developers adopting NVIDIA&\#x27;s Rust tracks can keep standard Rust tooling such as linters, formatters, and documentation generators, since the GPU-specific parts only matter at compile time, but the payoff stays unproven until projects like Candle or Burn land a Rust-authored kernel in a hot path and publish benchmarks against their C++ equivalents. It also remains unclear whether AMD will answer with a supported Rust path for HIP/ROCm, and a Rust-first GPU ecosystem locked to a single vendor would be strategically worse than the C++ status quo it replaces.

**「Community Discussion」** Commenters were divided: some welcomed Rust&\#x27;s compile-time safety as a potential improvement over CUDA C++ and connected it to Rust inference work such as Hugging Face&\#x27;s Candle, while others criticized CUDA&\#x27;s proprietary lock-in, argued for separate kernel files launched manually as in Metal, OpenCL, or D3D12, and pointed to DSL alternatives like Triton. Skepticism also surfaced about the quality of the announcement itself, including a claim that it read as LLM-written.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels | NVIDIA Technical Blog</a></li>
<li><a href="https://forums.developer.nvidia.com/t/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/382704">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels - Technical Blog - NVIDIA Developer Forums</a></li>
<li><a href="https://daily.dev/posts/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels-a7096aegg">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels | daily.dev</a></li>
<li><a href="https://ailearningguides.com/nvidia-cuda-rust-gpu-kernels-2026/">Nvidia CUDA Rust in 2026: GPU Kernels Without C++ - AI Learning Guides</a></li>
<li><a href="https://ai-beat.github.io/news/2026/05/cuda-oxide-rust-gpu-kernels/">NVIDIA&#x27;s cuda-oxide Wants GPU Kernels Written in Rust · AI Beat</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#CUDA`, `#GPU programming`, `#NVIDIA`, `#systems programming`

---

<a id="item-tech-news-3"></a>
### [4B Query Planner Claimed 81% Faster Than Postgres](https://rohanbansal.com/qorl) ⭐️ 7.0/10

A blog post describes training a 4B model to generate query plans that its author reports are 81% faster than Postgres. The benchmark reportedly uses an 8 GB in-memory dataset, constrains shared\_buffers to a fraction of that, warms read-only SELECTs before measuring, and lacks secondary indexes or additional statistics, according to community critique. Those conditions matter because Postgres planning leans on statistics, indexes, and workload shape, so the result may not generalize to realistic OLTP workloads at scale. Commenters also point to correlated columns and the possibility that the gains reflect overfitting or profile-guided optimization rather than a broadly better planner. The work is technically substantive, but the headline speedup remains bounded by a narrow benchmark setup.

hackernews · polyphilz · Sep 16, 18:50 · [Discussion](https://news.ycombinator.com/item?id=49731285)

**「Background」** Query planners such as PostgreSQL&\#x27;s decide how to execute SQL by choosing join orders and access paths, typically using cost estimates and table statistics. Machine-learning approaches try to improve those choices by learning from workloads or execution feedback, and this project evaluates that idea on the Join Order Benchmark. Qorl trains a distilled 4B Qwen3.8 model with LoRA and agentic reinforcement learning to hint PostgreSQL&\#x27;s planner, reporting a 1.81× geometric-mean speedup across 113 queries for $1,200.

**「Impact」** For PostgreSQL users and database engineers, the most concrete implication is that this result supports only a narrow claim: a 4B model can beat stock Postgres heuristics on a specific warmed, index-poor, in-memory workload, not that learned planners are ready to replace production query planning.

**「Community Discussion」** Commenters broadly caution that the 81% figure comes from a narrow setup—8 GB of in-memory data, constrained shared\_buffers, warmed read-only SELECTs, no secondary indexes or extra statistics, and correlated columns—so it may reflect overfitting or profile-guided optimization rather than general planning gains. They also disagree about the tool: some prefer AlphaGo-style neural heuristics over an LLM, and others warn that a nondeterministic planner that can hallucinate or miss an index would be unreliable in production.

<details><summary>References</summary>
<ul>
<li><a href="https://ai-tldr.dev/releases/rohan-bansal-qorl/">Qorl — a 4B model plans Postgres queries 1.81x… | AI/TLDR</a></li>
<li><a href="https://yanoai.tech/blog/2026-09-17-a-4b-model-beat-postgres-by-81-percent-what-a-1-200-training-run-means-for-philippine-ai">A 4B Model Beat Postgres by 81 Percent: What a $1,200 ...</a></li>

</ul>
</details>

**Tags**: `#query planning`, `#PostgreSQL`, `#machine learning`, `#database performance`, `#benchmarking`

---

<a id="item-tech-news-4"></a>
### [Datasette 0.65.5 Fixes Trailing-Newline Table Permission Bypass](https://simonwillison.net/2026/Sep/16/datasette-2/) ⭐️ 7.0/10

Datasette 0.65.5 has been released as a security patch addressing a flaw in which a trailing newline appended to a requested table name could bypass table permissions and expose private rows. The vulnerability was reported by dpfkdlemtp and is documented in advisory GHSA-h547-rmjf-5m2m. The release announcement provides no further technical detail, such as affected configurations or exploit preconditions, beyond the description of the bypass and its potential to leak data. Users running earlier versions that enforce table-level permissions should treat this as a prompt upgrade, since the defect undermines the permission checks intended to keep private rows inaccessible.

rss · Simon Willison · Sep 16, 23:51

**「Background」** Datasette is Simon Willison&\#x27;s open-source tool for exploring and publishing data, commonly used to serve SQLite databases over the web, and it supports permission rules that can restrict which tables and rows a given user is allowed to see. Version 0.65.5 is a patch release in the 0.65.x line, arriving shortly after 0.65.4 in September 2026, and it addresses a flaw documented in security advisory GHSA-h547-rmjf-5m2m.

**「Impact」** Anyone running a Datasette instance that serves both public and private tables should upgrade to 0.65.5, since the trailing-newline bypass let a request reach private rows despite table permissions. The same advisory notes a related risk in the 1.0 alpha series, where users holding table creation and alteration permissions can also rename protected tables.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/11/datasette/">Release: datasette 0.65.4 | Simon Willison ’s Weblog</a></li>
<li><a href="https://github.com/simonw/datasette/security/advisories/GHSA-h547-rmjf-5m2m">Table permission bypass using trailing newlines in table names</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#security`, `#vulnerability`, `#open-source`, `#release`

---

<a id="item-tech-news-5"></a>
### [TMLR inquiry finds most authors of desk-rejected papers could not explain submissions](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 7.0/10

According to a Reddit post linking to a TMLR Medium article, TMLR contacted the authors of 10 submissions slated for desk rejection to see whether they could explain the papers they submitted. The reported outcomes were that one paper was withdrawn, one set of authors said they were unavailable due to other commitments, and another scheduled a meeting but did not attend. Authors of three papers could not answer basic questions about their work, while authors of three others could discuss high-level ideas but struggled with technical details. One set of authors answered all questions, though the interviewer, TMLR&\#x27;s Co-Editor-in-Chief, identified a major flaw in that paper. The Reddit poster described the results as concerning for research integrity and peer review.

reddit · r/MachineLearning · /u/hihey54 · Sep 16, 23:20

**「Background」** Transactions on Machine Learning Research \(TMLR\) is a machine learning journal whose review process normally gives authors a chance to respond to reviewer feedback before a decision is made. TMLR has faced a deluge of submissions, prompting stricter desk-rejection policies because of limited reviewer capacity, and all 10 papers in this inquiry ended up being desk rejected. The outreach described here was carried out by TMLR Co-Editor-in-Chief Nihar Shah, who contacted authors of papers already slated for desk rejection to ask whether they could explain their own submissions.

**「Impact」** The reported results give TMLR and other ML venues a concrete case study for evaluating stronger authorship-verification or author-response requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://jmlr.org/tmlr/ae-guide.html">Transactions on Machine Learning Research</a></li>
<li><a href="https://x.com/tmlrorg/status/2100322125491966241">Transactions on Machine Learning Research on X: &quot;TMLR has ...</a></li>
<li><a href="https://www.linkedin.com/posts/transactions-on-machine-learning-research-tmlr_asking-authors-about-their-own-papers-activity-7506087797871697920-HbWc">Transactions on Machine Learning Research (TMLR)’s Post</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#peer review`, `#research integrity`, `#academic publishing`, `#TMLR`

---

<a id="item-tech-news-6"></a>
### [GoBench benchmarks LLMs on 9x9 Go against KataGo](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 7.0/10

GoBench is a new benchmark that evaluates LLMs on 9x9 Go games against a ladder of KataGo opponents ranging from random to superhuman, according to its Reddit announcement. It claims to measure general reasoning ability, strongly correlates with ARC-AGI 2 at r=0.83, and remains highly unsaturated. In reported results, GPT-6 Astra max reaches 2500 Elo, far below the best KataGo at 4400 Elo, while Codex with Astra reaches 3560 Elo when given coding tools and two hours of preparation before evaluation. The author says the leaderboard will be kept updated as long as it is not saturated, and links to the leaderboard, GitHub code, paper, and an X post are provided; the claims are self-reported and not yet independently verified.

reddit · r/MachineLearning · /u/Roland31415 · Sep 16, 18:54

**「Background」** KataGo is a free and open-source computer Go engine, first released on 27 February 2019 and developed by David Wu, which uses self-play-trained deep neural networks plus advanced search algorithms to reach superhuman play. ARC-AGI-2 is an upgraded version of the ARC-AGI benchmark that preserves the original input-output pair task format while aiming to measure fluid intelligence, i.e. adaptation to novel problems rather than memorization. GoBench connects the two by scoring LLMs against a ladder of KataGo opponents and reporting a correlation with ARC-AGI-2 results.

**「Impact」** Researchers and developers seeking unsaturated benchmarks for LLM reasoning may consider GoBench, but its reported ARC-AGI 2 correlation and Elo comparisons should be treated as provisional until independently reproduced.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo - Wikipedia</a></li>
<li><a href="https://www.stork.ai/en/katago">KataGo Review (2026): Pricing &amp; Alternatives | Stork.AI</a></li>
<li><a href="https://arxiv.org/abs/2505.11831">ARC - AGI - 2 : A New Challenge for Frontier AI Reasoning Systems</a></li>
<li><a href="https://www.linkedin.com/posts/dhdeans_reasoning-agi-benchmarks-activity-7314624032107073536-0sR9">&quot; ARC - AGI - 2 : A New AI Benchmark &quot; | David H. Deans... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#LLM evaluation`, `#Go`, `#benchmark`, `#AI reasoning`, `#KataGo`

---

<a id="item-tech-news-7"></a>
### [Cloudflare adds AI training block setting while preserving search indexing](https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/) ⭐️ 7.0/10

Cloudflare announced on September 15 a &quot;block AI training&quot; setting that lets websites remain indexed by search engines while blocking non-compliant AI training crawlers, with Apple, Google, and Microsoft stated to have met or committed to meet the requirements. The setting is configured per domain, and if a site chooses &quot;block,&quot; all crawlers—including mixed-purpose crawlers—are blocked, which also affects search indexing. Cloudflare plans early next year to let sites control the proportion of their content cited in AI summaries. The feature addresses site operators&\#x27; ability to separate search indexing from AI training data use, though it is an incremental policy and product control rather than a technical breakthrough.

telegram · zaihuapd · Sep 16, 05:46

**「Background」** Cloudflare&\#x27;s new domain-level “Disallow AI Training” setting is meant to separate two uses that mixed-use crawlers previously combined: indexing content for search and collecting it for AI model training. Because the same crawler can do both, blocking AI training used to risk also removing a site from search results. Cloudflare says Apple, Google, and Microsoft already honor or have committed to honor the setting, while leading mixed-use crawlers are offering or building controls to respect it.

**「Impact」** For site operators, the domain-level setting lets them keep search indexing while blocking non-compliant AI training crawlers, with Apple, Google, and Microsoft already compliant or committed; however, selecting “block” also intercepts mixed crawlers and therefore affects search inclusion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-helps-end-the-search-or-ai-training-tradeoff/">Cloudflare Helps End the Search-or-AI-Training Tradeoff</a></li>
<li><a href="https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/">Have it both ways: stay discoverable in search while ...</a></li>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-helps-end-the-search-or-ai-training-tradeoff/">Cloudflare Helps End the Search-or-AI-Training Tradeoff</a></li>
<li><a href="https://runtimewire.com/article/cloudflare-disallow-ai-training-search-crawler-controls">Cloudflare lets publishers block AI training without ...</a></li>

</ul>
</details>

**Tags**: `#AI crawlers`, `#Cloudflare`, `#web infrastructure`, `#search indexing`, `#AI training data`

---

<a id="item-tech-news-8"></a>
### [Apple 2nm A20 Pro in iPhone 18 Pro detailed by Geekerwan](https://www.bilibili.com/video/BV1oZeA6fERD) ⭐️ 7.0/10

The Telegram digest cites a Geekerwan video reporting that Apple has launched the iPhone 18 Pro series with the A20 Pro, described as the first 2nm flagship chip. The A20 Pro is said to pack a 6-core CPU with a 20% faster ultra core, a 7-core GPU that is 40% faster, dual 16-core neural engines, and 50% more memory bandwidth than the A19 Pro, which Apple reportedly calls the fastest of all smartphones. The chip allegedly uses a new M-series-inspired packaging design and a 3x larger VC vapor chamber, yielding up to 40% better sustained performance over the previous generation. Apple also reportedly introduced the custom C2 modem, with 50% faster uploads and 15% lower power consumption, plus the first custom N1 wireless chip supporting Wi-Fi 7 and Bluetooth 6. However, these claims come from a brief, unverified Telegram summary of a Geekerwan video rather than a primary Apple announcement or independent technical review.

telegram · zaihuapd · Sep 16, 13:24

**「Background」** Apple&\#x27;s A-series system-on-chip has powered iPhones since 2010, and the A20 Pro is the first Apple mobile chip built on a 2nm-class node after several generations on TSMC&\#x27;s 3nm-class processes; &quot;packaging&quot; here refers to how the die, memory and interconnect are assembled, an area where Apple has increasingly borrowed techniques from its M-series Mac chips, with the linked coverage describing a widened 96-bit LPDDR5X memory bus \(Borneo\) after a long-standing 64-bit width. The C-series modem and N-series wireless chip reflect Apple&\#x27;s effort to replace supplier components with its own silicon — C2 is described as a second-generation mass-produced in-house 5G baseband, and N1 would be its first custom Wi-Fi/Bluetooth chip. Geekerwan \(极客湾\) is a Chinese hardware-review channel known for detailed SoC benchmarking, and its accompanying videos frame the A20 Pro as an unusually large generational jump, variously pitched as Apple&\#x27;s strongest chip since the A15.

**「Impact」** If the reported launch holds, the A20 Pro would make Apple the first high-volume smartphone vendor shipping silicon on TSMC&\#x27;s 2nm \(N2\) node, with the in-house C2 modem reducing iPhone dependence on Qualcomm 5G modems. The claim comes from a brief, secondhand Telegram summary of a Geekerwan video rather than a primary Apple announcement, so these consequences remain unconfirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bilibili.com/video/BV1N6Yb65Ezu/">【极客湾】苹果发布会总结，看官网 iPhone Duo和18 Pro的参数和价格，...</a></li>
<li><a href="https://www.youtube.com/watch?v=DpDf5JKOtls">iPhone 18 Pro: The Biggest Chip Upgrade in 5 Years! - YouTube 极客湾给A20Pro定调“五年最强”：交卷当晚70万播放，排队iPhone 18 Pro... iPhone 18系列曝光搭载：A20系列芯片+苹果自研第二代5G基带C2芯片 iPhone 18 Pro 系列发布解读：可变光圈与 2nm 芯片上车，9999 元起的... iPhone 18 Pro A20 Pro芯片深度技术分析——96-bit LPDDR5X内存架构与2n...</a></li>
<li><a href="https://blogdoiphone.com/en/iphone/a20-pro-2nm-iphone-18-pro-chip/">2 nm A 20 Pro : Why the iPhone 18 Pro Chip Will Be Unlike Anything...</a></li>
<li><a href="https://tech-insider.org/apple-a20-pro-2nm-chip-specs-2026/">A 20 Pro Goes 2 nm : GPU Up 40%, Bandwidth Up 50% [2026]</a></li>
<li><a href="https://www.youtube.com/watch?v=S0WIwJdrEDc">A 20 Pro is Apple ’s first 2 nm iPhone chip , touting better... - YouTube</a></li>

</ul>
</details>

**Tags**: `#Apple Silicon`, `#2nm process`, `#mobile SoC`, `#custom modem`, `#hardware`

---

<a id="item-tech-news-9"></a>
### [Sina Cloud SAE shutdown threatens early Bilibili video source files](https://tracker.archiveteam.org/sinavideo/#show-all) ⭐️ 7.0/10

Sina Cloud SAE, launched in 2009 as China’s first PaaS cloud platform, is reportedly set to go permanently offline at the end of September 16, 2026, with all user data to be deleted; the item says this means early Bilibili video source files will disappear. About 420 TB of historical data reportedly remains in Sina Cloud S3 buckets, according to the post. Archive Team’s distributed archiving project has reportedly rescued roughly 680 TB in total and says the effort is 96.26% complete. The source is a brief Telegram aggregation post, and the reported figures have not been independently verified.

telegram · zaihuapd · Sep 16, 15:00

**「Background」** Sina Cloud SAE is a Chinese platform-as-a-service \(PaaS\) offering that provided cloud application hosting and related storage services such as SCS, and it was known as an early low-cost, no-ops option for developers after its 2009 launch. Bilibili, a major Chinese video-sharing platform, relied on it early on to store video source files, which is why the shutdown turns its remaining historical data into a digital-preservation problem. Archive Team is a volunteer distributed-archiving group that attempts to copy data before services disappear; public calls connected to this shutdown urged volunteers to rescue metadata and cited hundreds of terabytes of video at risk, though the figures and dates in those calls vary.

**「Impact」** Developers with workloads on Sina Cloud SAE face permanent deletion of all their user data at the platform&\#x27;s shutdown, while roughly 420 TB of early Bilibili video source files still stored in Sina Cloud S3 buckets remains at risk unless Archive Team&\#x27;s distributed archiving effort, reported at 96.26% complete, finishes before the deadline. The item provides no independent verification of the shutdown or of the preservation figures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sinacloud.com/">新 浪 云 计算</a></li>
<li><a href="https://www.mcbbs.co/thread-6307-1-1.html">来摇人了兄弟们，事态紧急，帮帮我们！ - 矿工茶馆 - MCBBS...</a></li>

</ul>
</details>

**Tags**: `#cloud computing`, `#PaaS shutdown`, `#digital preservation`, `#Bilibili`, `#Archive Team`

---

<a id="item-tech-news-10"></a>
### [Micron Claims First 512GB DDR5 RDIMM, Targets 2027 Production](https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027) ⭐️ 7.0/10

Micron says it demonstrated the world&\#x27;s first 512 GB DDR5 RDIMM for servers, with speeds up to 9200 MT/s, and says AMD and Intel are validating it for future server platforms. The module uses 3D-stacked DRAM chips, and 24 of them can be combined to form 12 TB of memory. Micron claims a single module consumes 16 W, compared with 44.2 W for four 128 GB modules, a reduction of more than 60%. Micron expects the module to be ready for mass production in 2027. The information comes from a Micron claim reported through secondary aggregation and has not been independently verified.

telegram · zaihuapd · Sep 16, 16:15

**「Background」** RDIMM \(registered DIMM\) modules place a register between the DRAM and the memory controller to buffer address and command signals, a design that lets servers host many high-capacity modules per system. Micron&\#x27;s 512 GB module uses 3D-stacked DRAM with through-silicon vias \(TSV\), stacking multiple dies vertically to fit more capacity into a single package. Micron announced the demonstration on September 15, 2026 across several server platforms, with production targeted for the second half of 2027.

**「Impact」** If Micron&\#x27;s claims hold through AMD and Intel platform validation, server and cloud operators could pack up to 12 TB of memory into a dual-socket, 24-channel system while cutting memory power by more than 60% per module, easing the capacity and energy constraints of AI and high-demand data-center workloads. Actual availability depends on Micron reaching its stated second-half 2027 production target and on independent verification of the performance and power figures.

<details><summary>References</summary>
<ul>
<li><a href="https://news.mydrivers.com/1/1151/1151460.htm">美 光 演示全球首款 512 GB DDR 5 RDIMM ... | 快科技</a></li>
<li><a href="https://news.cnyes.com/news/id/6573466">美 光 推 512 GB DDR 5 RDIMM 運作功耗降低逾6成 | 鉅亨網 - 美 股雷達</a></li>
<li><a href="https://www.unite.ai/ru/micron-demonstrates-512gb-ddr5-rdimm-targets-second-half-2027-production/">Micron демонстрирует 512 ГБ DDR 5 RDIMM , планирует...</a></li>
<li><a href="https://www.cool3c.com/article/252044">美光公布512GB DDR5 RDIMM伺服器記憶體，達9,200MT/s並降低60%能耗</a></li>
<li><a href="https://www.unite.ai/zh-cn/micron-demonstrates-512gb-ddr5-rdimm-targets-second-half-2027-production/">Micron展示512GB DDR5 RDIMM，目标在2027年下半年投产 – Unite.AI</a></li>

</ul>
</details>

**Tags**: `#DDR5`, `#服务器内存`, `#美光`, `#3D堆叠DRAM`, `#硬件`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed hikes rates a quarter point with unanimous vote](https://www.cnbc.com/2026/09/16/here-are-five-key-takeaways-from-wednesdays-fed-rate-hike.html) ⭐️ 9.0/10

The Federal Reserve raised its benchmark interest rate by a quarter of a percentage point on Wednesday, with all 12 Federal Open Market Committee voters in agreement. Fed Chair Kevin Warsh stressed the central bank&\#x27;s commitment to fighting inflation, and the Fed&\#x27;s own projections showed 16 of 18 participants expected at least one more hike in 2026; stocks fell after the decision, with the Dow Jones Industrial Average down 631 points.

rss · CNBC Finance · Sep 16, 21:23

**「Background」** Kevin Warsh has chaired the Federal Reserve since 2026, and the short post-meeting statement and brief news conference have been his pattern at recent meetings. The Fed has been raising rates to bring inflation down, while President Donald Trump has publicly pressured it to cut rates, even threatening to halt trade with countries that run surpluses with the U.S.

**「Impact」** Because credit card, auto and other variable-rate borrowing costs track the Fed&\#x27;s benchmark, households and businesses carrying such debt face higher interest payments, while the Fed&\#x27;s projections signal those costs may stay elevated longer than markets had assumed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kevin_Warsh">Kevin Warsh - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/09/04/trump-fed-rates-jobs-trade.html">Trump threatens to halt trade with top partners unless Fed ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Interest Rates`, `#Market Reaction`, `#Inflation`

---

<a id="item-finance-news-2"></a>
### [Fed raises rates 25 basis points, signals another hike this year](https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html) ⭐️ 9.0/10

The Federal Reserve raised its key interest rate by a quarter percentage point to a target range of 3.75%-4% on Wednesday — its first increase in more than three years — and signaled another hike is likely later this year. The Federal Open Market Committee voted 12-0, and officials nudged up their inflation forecasts to 3.7% for headline personal consumption expenditures and 3.4% for core inflation this year, each 0.1 percentage point above June&\#x27;s projection.

rss · CNBC Finance · Sep 16, 21:07

**「Background」** The Fed had held rates steady all year, but inflation has stayed above its 2% goal, which officials attribute partly to higher oil prices tied to the Iran war and to tariffs; the central bank&\#x27;s own projections do not show inflation reaching that 2% target until 2029.

**「Impact」** Borrowing costs are already elevated — a 30-year fixed mortgage stood at 7.19%, more than a full percentage point higher than a year earlier, according to Mortgage News Daily — so the move keeps pressure on households and businesses that borrow.

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#FOMC`

---

<a id="item-finance-news-3"></a>
### [Tanker Rates Top $1 Million a Day as Hormuz Disruption Tightens Oil Shipping](https://oilprice.com/Energy/Crude-Oil/Tanker-Rates-Smash-1-Million-a-Day-as-Oil-Shipping-Crisis-Deepens.html) ⭐️ 9.0/10

The daily rate to charter an oil tanker topped $1 million for the first time, with Bloomberg reporting up to $1.035 million a day for vessels loading inside the Persian Gulf, based on Baltic Exchange data. The spike reflects a shortage of tankers whose owners are willing to risk the Strait of Hormuz, and it is adding to the delivered cost of crude oil, according to the report.

rss · OilPrice.com · Sep 16, 23:00

**「Background」** Shipping through the Strait of Hormuz has been severely disrupted since March, and Saudi Arabia&\#x27;s East-West pipeline is out, potentially for weeks, after a drone attack — a combination that has cut the number of available vessels and driven freight and insurance costs sharply higher.

**「Impact」** Higher freight raises the end price buyers pay for physical crude, and second-hand tankers now sell above newbuild prices: an Argus analyst cited by El País put a used very large crude carrier at about $182 million versus $130 million for a new one.

**Tags**: `#oil shipping`, `#tanker rates`, `#Strait of Hormuz`, `#oil supply disruption`, `#energy cyber risk`

---

<a id="item-finance-news-4"></a>
### [Saudi Pipeline Attack Cuts Crude Exports to Europe](https://oilprice.com/Energy/Crude-Oil/Saudi-Oil-Crisis-Is-About-to-Hit-Europe.html) ⭐️ 9.0/10

Attacks on September 10 shut Saudi Arabia&\#x27;s East-West Petroline, the Red Sea export route that had been carrying roughly 4 million barrels per day, and state producer Aramco has told European customers that some September-loading cargoes are cancelled or postponed. Kpler estimates a prolonged outage could put 3.5–4 million bpd of Saudi crude exports at risk, while Argus reporting cited by Euronews says at least three European refiners have had late-September cargoes cancelled or delayed, in some cases until November.

rss · OilPrice.com · Sep 16, 18:32

**「Background」** The 1,200-kilometer East-West Pipeline \(Petroline\), designed to carry up to about 7 million barrels per day from eastern Saudi oil fields to the Red Sea port of Yanbu, became one of the world&\#x27;s most important pieces of energy infrastructure after the war effectively closed the Strait of Hormuz. The pipeline was attacked on September 10, 2026, amid a broader conflict that also saw Houthi forces capture a strategic island at the Red Sea&\#x27;s southern entrance.

**「Impact」** European refiners whose late-September Saudi cargoes were cancelled or delayed must replace them with pricier North Sea, U.S. Gulf Coast, West African or other Atlantic Basin crude, and the resulting higher wholesale diesel and gasoline costs can reach European filling stations within one to two weeks, according to the report.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_East%E2%80%93West_Crude_Oil_Pipeline_attack">2026 East–West Crude Oil Pipeline attack - Wikipedia</a></li>
<li><a href="https://apnews.com/article/yemen-houthis-iran-mokha-mandeb-shipping-saudi-025d052a14d9481258d51009a76d0bd6">Saudi Arabia shuts down a pipeline as Houthis seize an island, opening a new front in the Iran war</a></li>
<li><a href="https://www.hydrocarbonprocessing.com/news/2026/09/saudi-cancels-some-oil-cargoes-after-pipeline-hit-orlen-chasing-alternatives/">Saudi cancels some oil cargoes after pipeline hit, Orlen ...</a></li>
<li><a href="https://www.straitstimes.com/world/europe/saudi-cancels-some-oil-cargoes-after-pipeline-hit-top-buyer-chasing-alternatives">Saudi cancels some oil cargoes after pipeline hit, top buyer ...</a></li>

</ul>
</details>

**Tags**: `#Saudi Arabia`, `#Petroline pipeline`, `#oil supply disruption`, `#Europe energy security`, `#Houthi conflict`

---

<a id="item-finance-news-5"></a>
### [Bank of England Under Pressure to Raise Rates as Gilts Sell Off and Energy Prices Surge](https://oilprice.com/Energy/Energy-General/Energy-Shock-Puts-Bank-of-England-Under-Pressure-to-Raise-Rates.html) ⭐️ 9.0/10

Investors are pressing the Bank of England to raise interest rates at its Thursday meeting, after a historic global bond sell-off pushed the 30-year UK gilt yield close to 6%, its highest level since 1997, and Brent crude reached $107 a barrel, its highest since May. Shorter-term gilt prices imply the Bank could raise rates as many as four times over the next 12 months, while economists cited in the report disagree on whether it should hike or hold.

rss · OilPrice.com · Sep 16, 16:00

**「Background」** The Bank of England&\#x27;s Monetary Policy Committee sets &quot;Bank Rate&quot;, the UK&\#x27;s key interest rate used to steer inflation; Thursday&\#x27;s decision would be its sixth consecutive meeting without a change, after the Bank previously signalled it would raise rates. Gilts are UK government bonds, and their yields rise as their prices fall.

**「Who feels it first」** Higher gilt yields flow straight into the UK government&\#x27;s own borrowing costs: Britain sold £4.25 billion of 30-year gilts at a yield of 5.8168%, the highest on such a syndicated sale since the Debt Management Office was created in 1998.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/boeapps/database/Bank-Rate.asp">Bank Rate history and data | Bank of England Database</a></li>
<li><a href="https://invezz.com/news/2026/09/15/why-the-boe-may-stop-selling-long-gilts-as-britains-bond-stress-deepens/">Why the BoE may stop selling long gilts as Britain’s bond ...</a></li>

</ul>
</details>

**Tags**: `#Bank of England`, `#interest rates`, `#global bond selloff`, `#inflation`, `#oil prices`

---

<a id="item-finance-news-6"></a>
### [US Fed raises interest rates for first time in three years](https://news.google.com/rss/articles/CBMipgFBVV95cUxQMkVyU1l1M3VEcEg2TUZuemNacHp6X2hGbjdwYXlGV1FZdzhEbGtjdzlkd3BUS1RzUkVjNkZ1d3lMRl9TTUlMdFhuQlg5cnZKT1FCT2FyMXNzSzRsRzFtMVZIU1o1YURKTzRKUHdlOUxJdWdrRDYwS0JFTFd4WEhMRlpWRl9oWXRKUEJCVVdJM2xJemZCbEJ3eEw0WWExelctR2NLTXJR0gGrAUFVX3lxTE9pUXRTYm84MEp3U2xNby01Zm54cTNhSVNoaDRCRUdPNlNuN1B4NDFDV3FGcDU4M185c01LdnczeG43UFFHRUdSNndFS0k1NHlISW84MUJmSUV3R05mWnJDWC1iV2piUjB1dFZnNURjMi1nNUtLU1p1VjNsWkVFNHZsaktNd3pZMUdhWERQRlVmQjBHUVFDREluUkdPM2ZuTmlzWlh4M3NoTG51Yw?oc=5) ⭐️ 9.0/10

The US Federal Reserve raised interest rates for the first time in three years, a shift in monetary policy reported by Al Jazeera. The supplied item is only a headline and link, so the size of the rate increase, the new target range and the date of the decision are not available.

google\_news · Al Jazeera · Sep 16, 23:59

**「Background」** The Federal Reserve uses its benchmark interest rate as its main lever against inflation: raising it makes borrowing — for mortgages, credit cards and business loans — more expensive, which is intended to slow price growth. According to AP reporting, the Fed&\#x27;s last rate increase was in 2023, and this quarter-point move takes the benchmark rate to about 3.9%.

**「Who is affected」** Because Fed rate changes feed into borrowing costs, a rate increase makes mortgages, credit-card balances and business loans more expensive for households and firms, per Investopedia&\#x27;s explanation of how Fed moves pass through to borrowers.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/federal-reserve-warsh-trump-inflation-bab1bcb07e973bfb2dd0c3e5fbbb73b1">Federal Reserve hikes key rate for 1st time in 3 years ...</a></li>
<li><a href="https://www.investopedia.com/articles/investing/010616/impact-fed-interest-rate-hike.asp">How Federal Reserve Rate Changes Affect Borrowing</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#macroeconomics`

---

<a id="item-finance-news-7"></a>
### [Federal Reserve Raises Interest Rates as Inflation Persists](https://news.google.com/rss/articles/CBMipwFBVV95cUxPVzRmb0t4LU9yNWl6TEVsYnpQZ05wVjRIRlZYMmZEZXB2QllCTFNodmRPdl8yZmpjS0RTSmZWNmxyaERiR0JMcExCazgtMjFxekpwM3FYT3htY0pQOUQwZk1WRXpBYWhVUFhieEpUTk9NUXh0Vk42Wnd4WVVMbHo1VFh6ZzQ2NG1xVkNVSkhKWU0xNlBOa1dRRXh6a2pITGptSzg1dTYyOA?oc=5) ⭐️ 9.0/10

The Federal Reserve has raised interest rates, according to a headline from The Well News, which attributes the move to persistent inflation. The available source gives no figure for the size of the increase, the date, or the Fed&\#x27;s stated rationale, so those details remain unclear.

google\_news · The Well News · Sep 16, 19:54

**「Background」** The federal funds rate is the benchmark interest rate the Fed sets for overnight lending between banks, and it feeds into borrowing costs across the economy, from mortgages to credit cards. The reported 0.25-percentage-point increase took the target range to 3.75%–4.00%, the first rise since 2023, according to news reports on the move.

**「Impact」** Households and businesses can face higher borrowing costs because the Fed&\#x27;s benchmark rate influences other interest rates in the economy.

<details><summary>References</summary>
<ul>
<li><a href="https://newstalk1130.iheart.com/content/2026-09-16-federal-reserve-raises-interest-rates-as-inflation-pressures-grow/">Federal Reserve Raises Interest Rates As Inflation Pressures Grow</a></li>
<li><a href="https://www.cnn.com/2026/09/16/business/live-news/federal-reserve-interest-rate-september">Fed raises interest rates for the first time since 2023 | CNN Business</a></li>
<li><a href="https://www.sofi.com/learn/content/interest-rates-and-inflation/">How Does Raising Interest Rates Help Inflation? - SoFi</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#inflation`, `#monetary policy`, `#macroeconomics`

---

<a id="item-finance-news-8"></a>
### [Fed Raises Rates to 3.75%–4%, Times of India Headline Reports](https://news.google.com/rss/articles/CBMiowJBVV95cUxQcEpXMWRxQm0tVjRGS24zTEwxWGNYa3pvWGZRcmlhbDF6TTFBN1ZrWXppOGVHaWR1c1BLZnoyalcxZXRwdDcxMGJscWtqVDRCRGdwVjRlNnB1Tk9tR2lMeW83elB2VVVhTGRtblNCMFlaR2VPc2tuQUVReXY5UDdCc0VudG5sd1BqVFBVemVLNlRsMDdZbHk2V1BwZ05sX0VvQ2tqQXJzV2djcFpoaENjNHNhXzFhTUxFZUs5UGE0SXN0VFc5R1E4VW5VMzBKVDBJMFZXSWxwZE93MXVVMGVFMmtEY05xSjkwR2ZyUmk2cmRObjdnSlgtZE5pVkZJNVIxTHQ2ajkzYnBCQXJoR1NvdndCLUFCek9sRUh0ZzRXSnFvbVXSAagCQVVfeXFMT0E5bENZOUFtcnM4UkthQkVyZkpzT0hXSkZQV0Q2QUQxR1lyc09wazZDaDNBcm1PeDRHMHNTZzhZZmFYc3E0R0QxZzdJcW50QkFpNHRIZzlmdkhMOU52OUxBR2hOSUh0MEpSYTVqV0ZpRWpxNUJlcFpYaTNMYm5MdTRvMVBMOUI3MWZmZTY2SDhsU1pHU3U2TFNMcDdDelc3TUkzV2FuT0V0am9aRlcxb2hpTVBnRVNSc0RyWnVYd2tPZEhfY1haNlB3ZGpFUGd5bnBOUXAtUXRvbDExSWcwQURaR1hZdk40TzVVQ2VQZkRzNFExWVZ2OF9uTXZnYUFUOGtEaUdWblczZmdBZk9pU2RYdmdvRi12WTlKbWFoR2RaX0ZfRGYzNEo?oc=5) ⭐️ 9.0/10

A Times of India headline reports that the Federal Reserve&\#x27;s rate-setting committee, the FOMC, led by chair Kevin Warsh, raised its benchmark interest rate to a target range of 3.75%–4%, saying this is the first increase since 2023. Only the headline was available, so the vote, the reasoning and any further detail remain unconfirmed.

google\_news · timesofindia.indiatimes.com · Sep 16, 18:02

**「Background」** The federal funds rate is the benchmark rate banks charge each other for overnight loans, and it feeds into borrowing costs across the economy; the Fed had not raised it since 2023, and Wednesday&\#x27;s quarter-point increase — a unanimous decision, according to reports — was aimed at persistently high inflation.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/live/federal-reserve-meeting-live-updates-25-basis-point-interest-rate-hike-chairman-kevin-warsh-143452661.html?fr=sycsrp_catchall">Fed meeting live updates: Fed hikes interest rates by 25 ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html">Fed rate decision September 2026: Rates rise to 3.75%-4% - CNBC</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#FOMC`, `#US economy`

---

<a id="item-finance-news-9"></a>
### [Gold Pares Gains as Fed Raises Rates for First Time in Over Three Years](https://news.google.com/rss/articles/CBMiygFBVV95cUxQY0NDM01aZTE3OG1PN2dDUkUwcU5JbE9YUzgyUE40N0FpcFpzQkxnNDNqQU0zOVByNUd2VEVaak5HTzNzUXd3QTd1ajFjS1lsUnNIU2xnMmtmN1ZvOHN3aDZvQWYxNXFMNzU0WGo3VjNuNXJsaXQ2bEtGWlZYZl84OHZOajlNa3c1YllWOHkzaW1XemRadUR0QnExaDhFajJwc0tqdmloUXJRalBnV2pjVFRzYnB1TDVoeUJtWUNhcHZUQ25hTVk5ekpB?oc=5) ⭐️ 9.0/10

Gold gave up earlier gains after the Federal Reserve raised interest rates for the first time in more than three years, according to Investing.com. The report did not specify the size of the rate increase or the new target range.

google\_news · Investing.com · Sep 16, 02:11

**「Background」** The Fed&\#x27;s benchmark rate sets the cost of borrowing across the economy, and because gold pays no interest, higher rates make holding it less appealing compared with interest-bearing assets such as bonds. Before this increase, the Fed had last raised rates in December 2018, so this was its first hike in more than three years.

**「Impact」** Gold investors are the most directly affected: higher US interest rates raise the yield on competing assets such as Treasury bonds and tend to strengthen the dollar, a channel that has historically weighed on gold prices. One cited analysis notes the effect is not automatic — gold was still 2.4% higher a year after the aggressive tightening cycle that began in March 2022.

<details><summary>References</summary>
<ul>
<li><a href="https://adnamerica.com/en/united-states/federal-reserve-indicates-interest-rate-hike-arriving-march">Federal Reserve indicates interest rate hike arriving in March</a></li>
<li><a href="https://www.investopedia.com/articles/investing/100915/effect-fed-fund-rate-hikes-gold.asp">How Fed Funds Rate Hikes Influence Gold Prices</a></li>
<li><a href="https://www.researchgate.net/publication/377737869_Research_on_Gold_Price_Changes_and_Factors_Under_the_Background_of_Fed_Interest_Rate_Hike">(PDF) Research on Gold Price Changes and Factors Under the Background of Fed Interest Rate Hike</a></li>
<li><a href="https://www.benzinga.com/markets/commodities/26/09/61798255/gold-performance-after-fed-rate-hikes-history">Gold&#x27;s Performance After Fed Rate Hikes: What History Shows - SPDR Gold Shares (ARCA:GLD) - Benzinga</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#gold`, `#markets`

---

<a id="item-finance-news-10"></a>
### [Fed raises interest rates for first time in three years](https://news.google.com/rss/articles/CBMiuAFBVV95cUxNTnQtM3ZBS0Rlckk2eGFFSU9ReHRGVjh6R3pEa2NjeGJ1RFNhdHlUeVczQ3VSS0FkTzVzaWJScUNFZkxSUkZvdnZrX2ZBT1o0ZU96T2RfVjQ5dTRYTjQ5bEk5X2FabUFVWkZydGdyLVh1YTlvOVpFcmxvbVBjYkpNTUM3dldwWVNDREpPeElRZGZHVDlXdTdpVm9sV2VtT2RCNGI1QThPWDJ2RFlhR2VFM2swT2NTUzl6?oc=5) ⭐️ 9.0/10

The US Federal Reserve raised interest rates for the first time in three years and signaled more tightening ahead, The Straits Times reported.

google\_news · The Straits Times · Sep 16, 18:20

**「Background」** It was the Fed&\#x27;s first rate increase since 2018, and the central bank said it expects to keep raising rates through the end of the year as it grapples with high inflation and new uncertainty from the crisis in Ukraine.

**「Who is affected」** US households and businesses whose loans are tied to the Fed&\#x27;s policy rate — such as credit-card balances, home-equity lines and adjustable-rate mortgages — face higher repayment costs as the increase feeds through to lending rates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2022/03/16/federal-reserve-meeting.html">Federal Reserve approves first interest rate hike in more ...</a></li>
<li><a href="https://www.wsj.com/livecoverage/federal-reserve-meeting-inflation-march-2022">Fed Raises Interest Rates for First Time Since 2018: Latest News</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#Federal Reserve`, `#interest rates`, `#inflation`, `#macroeconomy`

---

<a id="item-finance-news-11"></a>
### [Fed raises rates 25 basis points, signals one more hike this year](https://news.google.com/rss/articles/CBMiuAFBVV95cUxPRm5HbHUxaXQ0MEV1SjlrcFphcEkydzVnc2V4SlNkNW5IZk1acEVXTjczbEc0ajVfQzZxN19MbzNPZU5md0U5SngtUW1YRU9pSFp1Mmk1SzRoT2I2U2dWbWV0WktWRW5Ib19sa0F4ZXM5T1F2WmRxODR4SmVwRUYtN1lhMF9pWi1jRW1oSDJhTGE2RUtEeEl1NGJFN3hGTnIxa2dqeTVvXy1hZVpjSkVNaU1TRGtrT2dI0gHLAUFVX3lxTE05WUNGek5RTzVsOU81ZXZWd1luVm51dDY3N0kzTFdXcHBreWNjeVNVU290cENmNkJEdkQ1TVNwSjVwaGZKTThIZUY2UXh3TXUxSTJMa2RnejNaMmh2WTZEdEx4N0I2SkRLTnZnSUpVOXZwUmNMSFI3RXlyUnVhU3J6ZUNfb29ON01yWHdkcHFFc0YzN1haeXdhVW13eUluaVNSX0lLc0o5M3hnZHdFdGxaek9jU2VjUzZIcDg4SUNZdGpDWmJ4RlpxWERV?oc=5) ⭐️ 9.0/10

The Federal Reserve raised its benchmark interest rate by 25 basis points — a quarter of a percentage point — and signaled that one more increase is likely this year, according to Gulf News. The report does not specify the new rate level, the timing of the next move, or the reasoning behind the decision.

google\_news · Gulf News · Sep 16, 18:09

**「Background」** The increase lifted the Fed&\#x27;s benchmark rate to a target range of 3.75%–4%, its first hike since 2023, as officials try to contain inflation pressure that reports link partly to higher oil prices caused by Middle East supply disruptions.

**「What it means」** Households and businesses with variable-rate debt, such as credit cards and business credit lines, face higher interest costs because those rates typically track the Fed&\#x27;s benchmark, which officials signaled could rise again this year.

<details><summary>References</summary>
<ul>
<li><a href="https://gulfnews.com/business/banking/fed-raises-rates-by-25-basis-points-signals-one-more-hike-this-year-1.500677303">Fed raises rates by 25 basis points, signals one more hike ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html">Fed rate decision September 2026: Rates rise to 3.75%-4% - CNBC</a></li>
<li><a href="https://www.thenationalnews.com/business/economy/2026/09/16/fed-rate-rise-25-basis-points-hike/">US Fed raises interest rates and signals one more this year ...</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-september-16-2026">September FOMC: Federal Reserve hikes interest rates for ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html">Fed rate decision September 2026: Rates rise to 3.75%-4% - CNBC</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#U.S. economy`

---

<a id="item-finance-news-12"></a>
### [Federal Reserve Holds Interest Rates Steady, Signals Possible Future Hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

The Federal Reserve left its benchmark interest rate unchanged, according to a CBS News headline. The same report says the central bank left the door open to raising rates in the future, meaning no specific rate level, timing, or hike size was given in the available account.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The Federal Reserve is the U.S. central bank, and its benchmark rate is a key tool for managing inflation; it left that rate unchanged amid resurgent inflation, with nearly half of its policymakers indicating they would support a rate hike later this year, according to reports.

**「Impact」** Households and businesses with variable-rate debt, such as credit cards, home-equity lines and many small-business loans, see no immediate change in borrowing costs because those rates track the Fed&\#x27;s benchmark, though the hint that a hike remains possible means those costs could rise if the Fed tightens later.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aol.com/articles/federal-holds-interest-rates-steady-181753000.html">Federal Reserve holds interest rates steady but leaves door open ...</a></li>
<li><a href="https://intellectia.ai/blog/fed-interest-rate-decision-march-2026">Fed Interest Rate Decision March 2026: Impact on Stock Market ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#US economy`

---

<a id="item-finance-news-13"></a>
### [Pinglu Canal Opens as New Southwest China–ASEAN Shipping Route](https://www.news.cn/politics/20260916/4d3b671357d14c8db202cbf6120f2c43/c.html) ⭐️ 8.0/10

China&\#x27;s Pinglu Canal has opened to navigation, a 134.2-kilometre waterway built at a cost of more than 70 billion yuan that can handle 5,000-tonne vessels, according to Xinhua. Xinhua reported that cargo from southwestern China using the canal shortens voyages by more than 560 kilometres and cuts logistics costs by 18% to 30% versus traditional routes, with two direct river-sea services to Vietnam and Hainan&\#x27;s Yangpu port making their first sailings the same day.

telegram · zaihuapd · Sep 16, 09:10

**「Background」** The canal is a key hub of the New Western Land-Sea Corridor, a national program meant to give landlocked southwest China a shorter route to the sea and to Southeast Asian markets; construction began in August 2022, and state media describe it as the first canal since the founding of the People&\#x27;s Republic in 1949 that links an inland river system directly to the sea.

**「Who is affected」** Exporters and manufacturers in Southwest China and their ASEAN trading partners are the groups most directly affected, because the canal shortens the sea route to the Beibu Gulf by more than 560 km and is reported to cut logistics costs by 18% to 30% on that corridor.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gxrd.gov.cn/data/uploadfile/2024/06/19/20240619570vr.pdf">标题</a></li>
<li><a href="https://h5.ifeng.com/c/vivoArticle/v002zoB8aFlEMxFRxLcYQJSmhTZR9aozOFp9BmXGROeOg-_M__?isNews=1&amp;showComments=0">投资超700亿，这条 运 河 开挖！ 100年前的构想实现，这个地区将腾飞</a></li>
<li><a href="https://m.bjnews.com.cn/detail/1781001305129549.html">“百年构想” 平 陆 运 河 通 航 在即，哪座城市最受益？｜城市论</a></li>
<li><a href="https://opinion.haiwainet.cn/n/2026/0617/c353596-32961168.html">海评面：“ 平 陆 运 河 将促进中国与 东 盟 的 贸 易 增长”_原创评论_海外网</a></li>

</ul>
</details>

**Tags**: `#infrastructure`, `#China-ASEAN trade`, `#logistics`, `#Pinglu Canal`, `#regional economy`

---

<a id="item-finance-news-14"></a>
### [Hong Kong announces 11 measures to encourage childbirth](https://www.info.gov.hk/gia/general/202609/16/P2026091600265.htm) ⭐️ 7.0/10

Hong Kong Chief Executive John Lee&\#x27;s policy address set out 11 measures to encourage childbirth, which he said reverses the government&\#x27;s past non-intervention approach. The HK$20,000 newborn baby bonus is extended for three years and rises to HK$30,000 for second and later children born from today, while the child tax allowance for second and subsequent children increases from HK$140,000 to HK$160,000 from the 2026/27 tax year.

telegram · zaihuapd · Sep 16, 08:01

**「Background」** Hong Kong has tried this before: after a 2023 policy package of tax breaks and extra childcare places, the number of newborns still fell to a record low in 2025, according to reporting by Initium Media.

**「Impact」** Households with a newborn who buy a home within the specified window qualify for up to HK$20,000 in stamp duty relief, and white-form Home Ownership Scheme applicants with a newborn can borrow up to 95% of the flat&\#x27;s value, lowering the upfront down payment.

<details><summary>References</summary>
<ul>
<li><a href="https://theinitium.com/20260715-initium-audio-reasons-behind-low-fertility-rates-among-women-zh-hans/">当 政 府大力“谷 生 育 ”， 香 港 女性为何选择不 生 ？｜端闻 Podcast</a></li>
<li><a href="https://www.stheadline.com/zh-hans/society/3615153/%E6%96%BD%E6%94%BF%E6%8A%A5%E5%91%8A%E5%8A%A0%E6%8E%A811%E9%A1%B9%E6%8E%AA%E6%96%BD%E7%BB%AD%E6%8E%A82%E4%B8%87%E5%85%83%E6%96%B0%E7%94%9F%E5%A9%B4%E5%84%BF%E5%A5%96%E5%8A%B1%E9%87%91-%E7%94%9F%E5%A4%9A%E4%B8%AA%E6%B4%BE3%E4%B8%87%E7%88%B6%E6%AF%8D%E4%B9%B0%E6%A5%BC%E5%8F%AF%E5%87%8F2%E4%B8%87%E5%8D%B0%E8%8A%B1%E7%A8%8E">施政报告︱加推11项措施：续推2万元新生婴儿奖励金 生多个派3万！父母买楼可减2万印花税</a></li>
<li><a href="https://www.stheadline.com/zh-hans/society/3615181/%E6%96%BD%E6%94%BF%E6%8A%A5%E5%91%8A2026-%E6%83%A0%E6%B0%91%E6%8E%AA%E6%96%BD%E9%BC%93%E5%8A%B1%E7%94%9F%E8%82%B2%E9%95%BF%E8%80%85%E7%85%A7%E9%A1%BE%E5%88%B8%E5%B1%85%E5%B1%8B%E6%96%B0%E8%AE%BE%E8%AE%A1-%E7%84%A6%E7%82%B9%E6%94%BF%E7%AD%96%E6%87%92%E4%BA%BA%E5%8C%85">施政报告2026 惠民措施︱鼓励生育/长者照顾券/居屋新设计 焦点政策懒人包</a></li>

</ul>
</details>

**Tags**: `#香港`, `#生育政策`, `#财政激励`, `#房屋与按揭`, `#税务减免`

---

<a id="item-finance-news-15"></a>
### [Unverified Post Claims Fed Raised Rates 25 Basis Points, First Hike Since 2023](https://www.federalreserve.gov/newsevents/pressreleases/monetary20260916a.htm) ⭐️ 7.0/10

An unverified Telegram post, citing a Federal Reserve press release, reports that the Fed raised its federal funds target range by 25 basis points to 3.75%–4.00%, with all 12 FOMC members voting in favor — which would be its first rate increase since July 2023. The post also says Fed projections put the median policy rate near 4.1% at the end of 2026, implying another 25-basis-point hike could come later this year, and attributes comments on stubborn underlying inflation to a new Fed chair, Kevin Warsh; none of these claims has been independently corroborated.

telegram · zaihuapd · Sep 16, 20:06

**「Background」** The Fed had held its benchmark rate at 3.50%–3.75% at its June 2026 meeting, the first chaired by Kevin Warsh, citing elevated inflation and solid growth. That made this week&\#x27;s move the first increase since July 2023.

<details><summary>References</summary>
<ul>
<li><a href="https://www.usbank.com/content/dam/usbank/en/documents/pdfs/wealth-management/situation-analysis-6-17-2026.pdf">Situation Analysis - Fed holds rates steady 6-17-2026 - POSTING</a></li>
<li><a href="https://www.policyrix.com/news/2026-06-19/us-federal-reserve-holds-rates-warsh-hawkish-dot-plot-june-2026">US Federal Reserve Holds Rates at 3.50%–3.75% in Warsh&#x27;s ...</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#Federal Reserve`, `#interest rates`, `#inflation`, `#source credibility`

---