---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 180 items, 20 important content pieces were selected

---

**Technology News**
1. [OpenAI Highlights Ten AI Advances in Math and CS](#item-tech-news-1) ⭐️ 8.0/10
2. [Kimi K3 Architecture Analysis: Memory, Attention, Routing](#item-tech-news-2) ⭐️ 8.0/10
3. [DNA Analysis Devices in US Crime Labs Found Vulnerable to Evidence Tampering](#item-tech-news-3) ⭐️ 8.0/10
4. [US Officers Abused License-Plate Cameras to Watch Exes, Probe Finds](#item-tech-news-4) ⭐️ 8.0/10
5. [Researchers unlock NVIDIA CMP 170HX to 80GB VRAM, prices surge](#item-tech-news-5) ⭐️ 8.0/10
6. [Apple sues UK government over iCloud backdoor order](#item-tech-news-6) ⭐️ 8.0/10
7. [LLMs reward expertise](#item-tech-news-7) ⭐️ 7.0/10
8. [Devtools should be open source — LLMs make modification feasible](#item-tech-news-8) ⭐️ 7.0/10
9. [MiniMax H3 Gets Day-0 ComfyUI Support with Open Weights and 2K Video](#item-tech-news-9) ⭐️ 7.0/10
10. [Andy Pavlo joins ClickHouse to establish ClickHouse Labs](#item-tech-news-10) ⭐️ 7.0/10
11. [Jane Street&\#x27;s Bonsai brings typed OCaml UI to the frontend](#item-tech-news-11) ⭐️ 7.0/10
12. [Qwen Announces 3.8-Max: 2.4 Trillion Parameters, First Open Max-Level Weights](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [California Diesel Prices Jump as Iran War Adds to Nationwide Cost Pressures](#item-finance-news-1) ⭐️ 8.0/10
2. [Visa to Buy Fraud-Detection Firm BioCatch for $2.4 Billion](#item-finance-news-2) ⭐️ 8.0/10
3. [China&\#x27;s tourism slowdown turns hotels to price wars](#item-finance-news-3) ⭐️ 8.0/10
4. [Japan and U.S. Expected to Jointly Intervene to Support Yen](#item-finance-news-4) ⭐️ 8.0/10
5. [Broadcom Stock Slips After Losing EU Antitrust Case](#item-finance-news-5) ⭐️ 8.0/10
6. [Berkshire Hathaway, Led by Greg Abel, Closes Taylor Morrison Acquisition](#item-finance-news-6) ⭐️ 8.0/10
7. [After-hours stock movers: Palantir, On Semi, Snap gain; Whirlpool falls on earnings](#item-finance-news-7) ⭐️ 7.0/10
8. [Dow Reaches Record High Amid Iran Deal Hopes](#item-finance-news-8) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Highlights Ten AI Advances in Math and CS](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI published a post describing ten recent advances where artificial intelligence is making significant inroads into mathematics and theoretical computer science, drawing broad attention from the technical community. The source item does not include the full list of advances, but the discussion indicates the post covers topics such as sphere packing and multicolor Ramsey numbers. The announcement is notable because it signals AI&\#x27;s accelerating role in proof generation, disproof, and verification, a domain traditionally considered resistant to automation. Community reaction suggests the impact is now widely acknowledged rather than disputed.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**「Background」** OpenAI released a 249-page manuscript describing ten new results in mathematics and theoretical computer science, obtained with an internal AI model. The results target long-standing open problems and span geometry, cryptography, and complexity, and each comes with a machine-checkable certificate in the Lean 4 proof assistant. Lean is an interactive theorem prover that allows computers to independently verify formal proofs, making this a step toward using AI to generate results that can be machine-verified rather than relying only on human review.

**「Community Discussion」** Commenters largely agree that progress on mathematics via AI is real and accelerating, with some framing it as an exponential curve and others noting that LLMs make the generate-and-check loop far more practical. A few point to specific examples from the post, while one commenter notes that current models still cannot &\#x27;intuit&\#x27; conjectures but can disprove them through grinding work that humans can&\#x27;t match.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science</a></li>
<li><a href="https://cdn.openai.com/pdf/ten-proofs-oai.pdf">Ten Advances in Mathematics and Theoretical Computer Science</a></li>
<li><a href="https://beyondtmrw.org/article/ten-advances-in-mathematics-and-theoretical-computer-science">Ten advances in mathematics and theoretical computer science</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Kimi K3 Architecture Analysis: Memory, Attention, Routing](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

The SemiAnalysis article provides a technical deep-dive into Kimi K3&\#x27;s architecture, focusing on its compressed memory system, attention mechanisms across depth, and latent expert routing as key innovations. It evaluates how these design choices differ from standard transformer and mixture-of-experts approaches, with particular attention to their impact on inference performance and serving efficiency. The analysis is aimed at AI engineers and researchers, offering concrete architectural details rather than marketing hype. While the article explains the reasoning behind these design decisions, the available excerpt does not include specific benchmark numbers, version details, or performance comparisons.

rss · Semianalysis · Aug 3, 19:42

**「Background」** Kimi K3 is an open-weight, frontier-class AI model released by Moonshot AI in July 2026, with 2.8 trillion parameters, a 1-million-token context window, and native vision capabilities. Its architecture builds on Kimi Delta Attention \(KDA\), Attention Residuals \(AttnRes\), and a hybrid linear-full attention design, which are the technical foundations for the compressed memory, attention-across-depth mechanisms, latent expert routing, and inference performance discussed in the article.

**「Impact」** For AI researchers and engineers, Moonshot AI&\#x27;s open release of the 2.8-trillion-parameter Kimi K3 Mixture-of-Experts model \(104B active parameters, 1M-token context, native vision\) provides a frontier-class open alternative that outperforms most open and proprietary models in long-horizon coding, agentic, knowledge, reasoning, and vision tasks. However, it still trails the most powerful proprietary models, Claude Fable 5 and GPT-5.6 Sol, so organizations adopting Kimi K3 for the highest-stakes tasks should verify alignment and capability gaps against those proprietary baselines.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-K3/tree/main">GitHub - MoonshotAI/Kimi-K3: Open Frontier Intelligence</a></li>
<li><a href="https://dev.to/tony_dillard/what-is-kimi-k3-complete-2026-guide-to-moonshot-ais-open-source-model-565j">What Is Kimi K3? Complete 2026 Guide to Moonshot AI&#x27;s Open Source Model</a></li>
<li><a href="https://kimi-k3.dev/">Kimi K3 — Open Frontier AI Model Guide | kimi-k3.dev</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/kimi-k3-ai-breakthrough-wall-123003909.html?fr=sycsrp_catchall">Kimi K3 AI breakthrough: What Wall Street analysts say about ...</a></li>
<li><a href="https://arxiv.org/abs/2607.24653">[2607.24653] Kimi K3: Open Frontier Intelligence - arXiv.org</a></li>
<li><a href="https://arxiv.org/pdf/2607.24653">Kimi K3: Open Frontier Intelligence - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#AI`, `#model-architecture`, `#inference`, `#machine-learning`, `#memory`

---

<a id="item-tech-news-3"></a>
### [DNA Analysis Devices in US Crime Labs Found Vulnerable to Evidence Tampering](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

Researchers found security vulnerabilities in DNA analysis equipment used by most US crime labs, potentially exposing about 30 years of criminal DNA evidence since 1995 to tampering. Using AI-generated code, including Anthropic&\#x27;s Claude, they altered DNA scan data undetected; the first file modification took roughly 45 minutes and did not trigger alerts in common analysis software. Thermo Fisher Scientific, the equipment maker, privately acknowledged the vulnerability in July, issued a high-risk security advisory last Friday, and released a software update with digital signatures. The company said it is coordinating with the US Cybersecurity and Infrastructure Security Agency and that no exploit has been confirmed, while researchers noted more than 200 labs lack unified regulation and the impact on pending or closed cases remains unclear.

telegram · zaihuapd · Aug 3, 05:15

**「Background」** DNA analysis instruments convert biological samples into digital genetic profiles used as forensic evidence in criminal cases. The research highlights that these instruments run on software that can be locally or remotely manipulated, and altering the underlying scan data could compromise the integrity of evidence without detection by standard analysis tools.

**「Impact」** The affected US crime labs face a credible risk that up to 30 years of DNA evidence could be tampered with, prompting Thermo Fisher to ship a digital-signature software update; no confirmed exploit means immediate case-level impact remains uncertain.

**Tags**: `#security`, `#AI`, `#DNA-analysis`, `#vulnerability`, `#forensics`

---

<a id="item-tech-news-4"></a>
### [US Officers Abused License-Plate Cameras to Watch Exes, Probe Finds](https://www.washingtonpost.com/technology/2026/08/02/how-police-officers-used-vast-network-cameras-spy-their-exes/) ⭐️ 8.0/10

A Washington Post investigation published August 2, 2026 found that at least 50 U.S. law enforcement officers have been accused or sued for misusing license plate recognition systems such as Flock for illegal surveillance, with 26 cases involving spying on wives, girlfriends, exes, or women they were interested in and 46 cases involving Flock. One case involved Georgia police chief Michael Steffman, who conducted about 600 searches of his ex-girlfriend Bakely and her daughter&\#x27;s license plates before his arrest in November 2025; he died by suicide in April 2026 before trial. Flock says its network includes more than 120,000 cameras across over 6,000 communities and records 20 billion license plate scans monthly. The company says abuse is hard to fully prevent and has introduced an optional &quot;audit assistance&quot; feature, while privacy advocates criticize weak oversight: only 13 states require audits and at least 8 states criminalize this type of misuse.

telegram · zaihuapd · Aug 3, 09:03

**「Background」** Automated license plate recognition \(ALPR\) systems use networks of cameras to scan and record vehicle plates constantly, enabling police to track vehicles over time and location. Flock is a prominent ALPR provider whose systems are widely deployed by local law enforcement, and the investigation highlights how the same vast data can be queried for personal motives when departments lack controls.

**「Impact」** For U.S. police agencies operating plate readers, the report demonstrates that internal misuse can go undetected in the majority of states that do not mandate audits, leaving voluntary company tools and state criminalization laws as the primary safeguards. The findings also put pressure on Flock and other vendors to show whether their optional audit features are actually used by customer agencies.

**Tags**: `#surveillance`, `#privacy`, `#law enforcement`, `#license plate recognition`, `#technology ethics`

---

<a id="item-tech-news-5"></a>
### [Researchers unlock NVIDIA CMP 170HX to 80GB VRAM, prices surge](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

Arizona State University researchers publicly detailed a hack for NVIDIA&\#x27;s CMP 170HX mining card that exploits a stack overflow in the GPU security coprocessor to bypass the factory OTP fuse locks. The unlock increases usable VRAM to up to 80 GB and boosts FP32 performance from 0.39 TFLOPS to 94 TFLOPS. Following the announcement, secondhand prices jumped from 300–500 yuan to 3000–4000 yuan domestically, with overseas listings reportedly reaching $1,500. The card, launched in 2021, uses the same GA100 core as the A100 but was previously considered permanently locked via OTP fuses. Chinese community tests report the unlocked cards can run AI image generation and large language model inference on Windows and Linux, though long-term stability and per-batch unlock limits remain uncertain.

telegram · zaihuapd · Aug 3, 11:29

**「Background」** NVIDIA&\#x27;s CMP 170HX is a dedicated cryptocurrency mining card introduced in 2021, based on the GA100 GPU also found in the A100 but severely restricted through one-time programmable \(OTP\) fuses that limit compute, memory, and PCIe capabilities. These physical fuses were intended to make such restrictions irreversible, but the researchers demonstrated a way to overwrite the relevant registers by hijacking the Falcon security coprocessor through a DMA-bound overflow vulnerability.

**「Impact」** Budget AI hardware enthusiasts and researchers now have access to a potentially inexpensive high-VRAM inference card with 80 GB of memory and 94 TFLOPS FP32 performance, though the security bypass also raises concerns about silicon-level lock bypasses and the unlocked cards&\#x27; long-term stability.

**Tags**: `#NVIDIA`, `#GPU hardware`, `#security exploit`, `#AI inference`, `#mining card`

---

<a id="item-tech-news-6"></a>
### [Apple sues UK government over iCloud backdoor order](https://www.ft.com/content/2cc9c96a-0e5b-4c33-a95a-3d11072a145c?syn-25a6b1a6=1) ⭐️ 8.0/10

Apple has filed a legal challenge with the UK Investigatory Powers Tribunal against a Technical Capability Notice \(TCN\) that would require it to give UK authorities access to encrypted iCloud backups. Apple argues that any such backdoor would reduce security for all users, and both Apple and the UK Home Office declined to comment due to legal restrictions. The case continues a broader dispute: the UK withdrew an earlier notice after clashing with the US, then issued a new notice applying only to UK users, and Apple removed iCloud Advanced Data Protection in the UK in February 2025. Privacy International and Liberty have also challenged the TCN, and a case management hearing is scheduled for next month.

telegram · zaihuapd · Aug 3, 15:40

**「Background」** Under UK law, the Home Office can issue Technical Capability Notices \(TCNs\) compelling companies to remove forms of electronic protection, such as encryption. iCloud Advanced Data Protection \(ADP\) uses end-to-end encryption for iCloud backups, meaning even Apple cannot access the data; the UK notice would require Apple to undermine that protection for UK users. Apple has long maintained that creating a backdoor for one government would weaken security for everyone.

**「Impact」** Affected UK iCloud users have already lost access to Advanced Data Protection, Apple&\#x27;s strongest backup encryption option, and the lawsuit will determine whether the company must also build a backdoor into standard encrypted backups.

**Tags**: `#Apple`, `#iCloud`, `#encryption`, `#privacy`, `#UK`

---

<a id="item-tech-news-7"></a>
### [LLMs reward expertise](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 7.0/10

An analysis argues that large language models amplify existing expertise, making domain knowledge and codebase familiarity essential for effective use. It likens LLMs to an amplifying mirror that reflects the user&\#x27;s knowledge, tone, and focus. The piece contends that people who carefully use LLMs as an extension of their own mind and senses will thrive, while those who use them as a replacement for their minds will struggle. This matters because it shifts the emphasis from generic prompting skills to cultivating real expertise, with direct implications for software engineering practice and AI tool adoption.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**「Background」** The article &\#x27;LLMs reward expertise&\#x27; by Sean Goedecke responds to the popular idea that &\#x27;skilled prompters&\#x27; obtain the best results from large language models because everyone interacts with the same underlying models. Goedecke argues the opposite: the most important prompting skill is expertise in the domain being prompted, since users need enough knowledge to specify what &\#x27;good&\#x27; looks like and to judge the model&\#x27;s output. This context matters for software developers deciding how to allocate time between general AI prompting techniques and deep codebase or domain familiarity.

**「Impact」** The argument implies that developers and organizations should prioritize deep domain knowledge and codebase familiarity, since those factors largely determine how much value they get from LLM tools.

**「Community Discussion」** Commenters largely agree that expertise matters, citing experiences where signaling domain knowledge or having codebase familiarity changes the quality of LLM output. One commenter warns that taking for granted that prompting skill alone will dominate could lead to losing domain experts in a generation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/llms-reward-expertise/">LLMs reward expertise</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#expertise`, `#software-development`, `#human-AI interaction`, `#prompting`

---

<a id="item-tech-news-8"></a>
### [Devtools should be open source — LLMs make modification feasible](https://blog.exe.dev/devtools-must-be-open-source) ⭐️ 7.0/10

In &quot;Devtools must be open source,&quot; bryanmikaelian argues that developer tools should be open source and that LLMs make direct source modification practical, envisioning users changing hardcoded values or automatically rebasing local forks instead of relying on config files, option systems, or plugin APIs. The post contends that LLMs lower the cost of reading, patching, and maintaining local code changes, reviving the original open-source freedom to examine and modify software. Commenters offer counterarguments, including the inefficiency of rebuilding a tool just to change an editor font size, the risk of nightly AI-driven rebases breaking workflows, and the real maintenance burden of downstream forks. The discussion highlights a substantive split over whether LLMs truly transform devtool customization or create new overhead.

hackernews · bryanmikaelian · Aug 3, 14:15 · [Discussion](https://news.ycombinator.com/item?id=49156111)

**「Background」** The blog post argues that developer tools should be open source, and that LLMs make it more practical for users to customize tools by modifying source code directly rather than relying on configuration options. This taps into a long-standing debate about open source software: while the freedom to inspect and modify code has always been a core principle, in practice few users invest the time to do so. Simon Willison&\#x27;s comment, linked from Hacker News, notes that LLMs may change this calculus by making code modification more feasible for ordinary programmers, while other commenters raise concerns about maintenance burden and energy waste.

**「Community Discussion」** Commenters are divided: simonw sees LLMs making the open-source dream more feasible, but kelnos calls source edits inefficient and wasteful, theamk describes nightly automated rebases as &quot;hell,&quot; and maintainer lalitmaganti warns that maintaining a fork is real work, especially when upstream features clash with local changes.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49156111">Devtools must be open source | Hacker News</a></li>
<li><a href="https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/">Comment: Devtools must be open source (exe.dev)</a></li>
<li><a href="https://stacker.news/items/1539390">Devtools must be open source \ stacker news</a></li>

</ul>
</details>

**Tags**: `#open source`, `#LLMs`, `#developer tools`, `#software engineering`, `#opinion`

---

<a id="item-tech-news-9"></a>
### [MiniMax H3 Gets Day-0 ComfyUI Support with Open Weights and 2K Video](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 7.0/10

ComfyUI has added day-0 support for MiniMax H3, bringing open weights, native audio, and 2K video generation to the node-based interface. The model&\#x27;s modulation weights, roughly 40% of total parameters, can be pruned and replaced with a lookup table without output-quality loss, cutting memory footprint by 66% from 123.6 GB to 42.5 GB with the smallest variants. This enables local 2K video generation on a GPU such as an RTX 3060 via dynamic VRAM offloading. Community testing shows strong text-to-video results, with 10-second 480p generation taking about 10 minutes on a 16 GB RTX 4070 Ti Super, though unusual scenarios still exhibit artifacts.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**「Background」** ComfyUI is an open-source, node-based interface for AI image and video generation that lets users build and share custom workflows. MiniMax H3 is a recently released open-weights video model that accepts text, images, video, or audio inputs and generates video with native stereo audio at up to 2K resolution, 24 fps, and roughly 15 seconds per clip. Day-0 support means ComfyUI added native integration the same day the model was released, so users can run MiniMax H3 workflows immediately without waiting for third-party adaptations.

**「Impact」** Practitioners can now run a next-generation 2K video model locally in ComfyUI on consumer GPUs like the RTX 3060, dramatically lowering hardware requirements for open-weight video generation, though generation speed remains slow on mid-range hardware.

**「Community Discussion」** Commenters show enthusiasm for the results, noting the mouse render as a &\#x27;big leap&\#x27; and surprisingly good overall text-to-video quality, but also report jank and &\#x27;AI smoothing&\#x27; artifacts in unconventional scenarios. Several users question whether the pruning technique could apply to LLMs and debate the tradeoff between the substantial memory savings and the still-significant generation times.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui">MiniMax H3 Day-0 Support in ComfyUI: Open Weights, Native Audio, and 2K Video</a></li>

</ul>
</details>

**Tags**: `#comfyui`, `#video-generation`, `#open-weights`, `#minimax`, `#ai-tools`

---

<a id="item-tech-news-10"></a>
### [Andy Pavlo joins ClickHouse to establish ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 7.0/10

ClickHouse announced that database researcher Andy Pavlo is joining the company to establish ClickHouse Labs, a new research-focused initiative. The lab is intended to drive long-term research and collaboration for ClickHouse and the broader OLAP community. No technical details about the lab&\#x27;s agenda or products were provided in the announcement.

hackernews · nikolay\_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**「Background」** ClickHouse is an open-source columnar OLAP database known for high-performance analytical queries. Andy Pavlo is a prominent database researcher and professor at Carnegie Mellon University, widely recognized for his work on database systems and teaching. On August 3, 2026, ClickHouse announced that Pavlo would join the company as Vice President of Database Research and lead a new research group called ClickHouse Labs.

**「Community Discussion」** Commenters welcomed the news, with several recalling Pavlo&\#x27;s widely watched database lectures and hoping ClickHouse will fund academic database research. Others discussed potential technical directions, including decoupled compute/storage, integration with engines like Trino, and future ingestion and indexing standards such as Iceberg and Paimon.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/andy-pavlo-founding-clickhouse-labs">ClickHouse launches ClickHouse Labs with Andy Pavlo as VP of...</a></li>

</ul>
</details>

**Tags**: `#ClickHouse`, `#database`, `#OLAP`, `#research`, `#open-source`

---

<a id="item-tech-news-11"></a>
### [Jane Street&\#x27;s Bonsai brings typed OCaml UI to the frontend](https://github.com/janestreet/bonsai) ⭐️ 7.0/10

Jane Street&\#x27;s Bonsai is an OCaml UI library for building type-safe frontends, hosted on GitHub, and it enables developers to use OCaml on both backend and frontend. The project has generated substantial community interest, including a Signals and Threads podcast episode and practical questions about production adoption. Community members are comparing it with Melange, which also brings OCaml to the frontend, and asking whether using Bonsai means losing access to the JavaScript/React ecosystem. The supplied item did not include release versions, API details, or performance benchmarks.

hackernews · KolmogorovComp · Aug 3, 08:29 · [Discussion](https://news.ycombinator.com/item?id=49152842)

**「Background」** Bonsai is Jane Street&\#x27;s OCaml UI library for building performant, reactive web applications, partly inspired by Elm. It is built on Js\_of\_ocaml, which compiles OCaml to JavaScript, and is used extensively inside Jane Street for internal web tools and trading-system interfaces. Because Bonsai is written in OCaml, it can share types and logic between the backend and frontend, a capability that has long been a goal for functional-programming web development.

**「Impact」** For OCaml and frontend engineers, Bonsai offers a typed UI stack with shared backend/frontend types, but its adoption outside Jane Street is not yet evidenced in the discussion.

**「Community discussion」** Comments mix excitement about shared OCaml types with practical skepticism, including a request for production-use reports and a comparison to Melange&\#x27;s JavaScript ecosystem compatibility; one user also criticized the default look as ugly despite likely performance.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet / bonsai : A library for building dynamic webapps...</a></li>
<li><a href="https://awesomeopensource.com/project/janestreet/bonsai">A library for building dynamic webapps, using Js_of_ ocaml</a></li>

</ul>
</details>

**Tags**: `#OCaml`, `#UI framework`, `#functional programming`, `#Jane Street`, `#frontend development`

---

<a id="item-tech-news-12"></a>
### [Qwen Announces 3.8-Max: 2.4 Trillion Parameters, First Open Max-Level Weights](https://qwen.ai/blog?id=qwen3.8) ⭐️ 7.0/10

According to an announcement on a Telegram channel, the Qwen team released Qwen 3.8-Max, a Mixture-of-Experts model with 2.4 trillion total parameters and 95 billion active parameters, described as the strongest Qwen model to date. The post says the model weights will be open-sourced next week, marking the first time a Max-level Qwen model has been released with open weights, and that it is built on the Qwen 3.5 architecture with improvements in coding, work, research, and long-horizon tasks. It claims the model ran autonomously for over 10 days to complete project building and self-evolution in code tests, and beat 458 of 526 teams in a WWW2025 multimodal dialogue intent recognition competition within 24 hours. The model is allegedly available via API through QwenCloud. This announcement has not been independently verified, so these details should be treated with caution.

telegram · zaihuapd · Aug 3, 02:31

**「Background」** Qwen \(通义千问\) is Alibaba Cloud’s open-source large language model family, with the flagship &\#x27;Max&\#x27; line historically offered as a hosted API rather than downloadable weights. A Mixture-of-Experts \(MoE\) architecture activates only a subset of parameters per token, which is why a 2.4-trillion-parameter model can run with roughly 95 billion active parameters. QwenCloud lists Qwen3.8-Max as a MoE flagship, and Alibaba has promised open weights, though the announcement does not include published benchmarks.

**「Impact」** If the unverified announcement holds, Qwen 3.8-Max&\#x27;s open-source weight release next week would let developers self-host a 2.4-trillion-parameter MoE model with 95B active parameters, currently available only through QwenCloud&\#x27;s paid API. This would make Alibaba&\#x27;s claimed strongest Qwen model accessible for local deployment and fine-tuning for the first time.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen">GitHub - QwenLM/Qwen: The official repo of Qwen (通义千问) chat ....</a></li>
<li><a href="https://www.qwencloud.com/models/qwen3.8-max">Qwen3.8-Max - QwenCloud</a></li>
<li><a href="https://techsy.io/en/blog/qwen-3-8">Qwen3.8: 2.4T Parameters, Open Weights, No Benchmarks</a></li>
<li><a href="https://openlm.ai/qwen3.8/">Qwen3.8 | OpenLM.ai</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#large language models`, `#open source`, `#Mixture of Experts`

---

## Financial News

<a id="item-finance-news-1"></a>
### [California Diesel Prices Jump as Iran War Adds to Nationwide Cost Pressures](https://www.cnbc.com/2026/08/03/californias-diesel-prices-have-jumped-since-the-iran-war-started-with-ripple-effects-across-the-country.html) ⭐️ 8.0/10

California diesel prices have jumped since the Iran war began, with the state averaging $6.92 per gallon, up from $5.10 before the war, compared with the $5.36 national average, according to AAA. The increase threatens higher costs for goods nationwide because California is a major entry point for U.S. container trade.

rss · CNBC Finance · Aug 3, 19:20

**「Background」** California already had the highest U.S. fuel prices and hosts the San Pedro Bay port complex, through which nearly one-third of U.S. containership imports and exports move. Diesel powers the trucks and trains that carry goods across the country, and analysts estimate the war plus attacks on Russian refineries has left the world short about 8% of global diesel demand.

**「Impact」** Because a meaningful share of America&\#x27;s supply chain pays West Coast fuel prices, higher California diesel costs can raise freight costs and ultimately the delivered cost of goods nationwide, according to JPMorgan analysts.

**Tags**: `#diesel prices`, `#California`, `#supply chain`, `#Iran war`, `#inflation`

---

<a id="item-finance-news-2"></a>
### [Visa to Buy Fraud-Detection Firm BioCatch for $2.4 Billion](https://www.cnbc.com/2026/08/03/visa-buys-biocatch-fraud-detection.html) ⭐️ 8.0/10

Visa said it will acquire fraud-detection startup BioCatch for $2.4 billion in cash, a deal expected to close by the end of Visa&\#x27;s fiscal second quarter in 2027 pending regulatory approvals. Visa says scams and account takeovers cost the global economy more than $1 trillion annually, and BioCatch&\#x27;s behavioral biometrics platform analyzes signals like keystroke timing and touch-screen pressure to help stop AI-powered fraud.

rss · CNBC Finance · Aug 3, 16:44

**「Background」** BioCatch is a Tel Aviv-based provider of behavioral biometrics—software that analyzes how users interact with devices, such as keystroke timing and mouse movements, to detect fraud—and had a last known valuation of about $1.3 billion.

**「Impact」** Banks and other financial institutions on Visa&\#x27;s network could gain broader access to BioCatch&\#x27;s behavioral biometrics fraud detection, since Visa connects about 14,500 institutions and BioCatch currently protects 760 million users at roughly 350 banks.

<details><summary>References</summary>
<ul>
<li><a href="https://tracxn.com/d/companies/biocatch/__KSbRciAK_u_oL4tH4o8Kpq1yWMAWrV2Pmq1GVXBpQrI">BioCatch - 2026 Company Profile, Team, Funding &amp; Competitors - Tracxn</a></li>
<li><a href="https://startupintros.com/orgs/biocatch">BioCatch: Funding, Team &amp; Investors</a></li>
<li><a href="https://investor.visa.com/news/news-details/2026/Visa-to-Acquire-BioCatch/default.aspx">Visa to Acquire BioCatch - Visa - Investor Relations</a></li>

</ul>
</details>

**Tags**: `#Visa`, `#BioCatch`, `#Cybersecurity`, `#Fraud Detection`, `#M&amp;A`

---

<a id="item-finance-news-3"></a>
### [China&\#x27;s tourism slowdown turns hotels to price wars](https://www.cnbc.com/2026/08/03/china-price-demand-tourism-hotel.html) ⭐️ 8.0/10

China&\#x27;s domestic tourism is weakening faster than expected: industry data show hotel revenue per available room \(RevPAR\) fell 6% year on year through late July, and Hilton now forecasts its full-year RevPAR to fall by a low single-digit percentage after a 2.2% drop in the second quarter.

rss · CNBC Finance · Aug 3, 10:32

**「Background」** China&\#x27;s post-pandemic travel rebound is fading as consumer spending stays weak, and per-capita tourism spending has declined since the third quarter of 2025.

**「Impact」** Domestic hotel operators face revenue pressure from lower occupancy and room rates, while visa-free inbound travel is helping lift the luxury segment.

**Tags**: `#China economy`, `#tourism`, `#hotels`, `#consumer spending`, `#RevPAR`

---

<a id="item-finance-news-4"></a>
### [Japan and U.S. Expected to Jointly Intervene to Support Yen](https://www.zaobao.com.sg/news/world/story20260802-9457369) ⭐️ 8.0/10

Japan and the U.S. are expected to jointly intervene in foreign-exchange markets to stop the yen from sliding to a 40-year low, with Japanese Finance Minister Katayama expected to announce the action on Aug. 3. Market reports say authorities have repeatedly bought yen, including Treasury Secretary Bessent’s meeting notes indicating purchases of between US$5 billion and US$10 billion worth of yen.

telegram · zaihuapd · Aug 3, 01:29

**「Background」** The yen had weakened to near 164 per dollar, its lowest since 1986, and the rare U.S. role is seen as an effort to make intervention more effective, curb short-selling expectations, and prevent excessive yen depreciation from amplifying global financial volatility. Economists widely say intervention alone is unlikely to reverse the yen’s long-term decline without changes in Japan’s economic fundamentals and monetary policy.

**Tags**: `#foreign exchange intervention`, `#yen depreciation`, `#Japan-US policy`, `#currency markets`, `#monetary policy`

---

<a id="item-finance-news-5"></a>
### [Broadcom Stock Slips After Losing EU Antitrust Case](https://finance.yahoo.com/markets/stocks/articles/broadcom-stock-slips-losing-major-182425517.html) ⭐️ 8.0/10

Broadcom’s stock slipped after the company lost a major European Union antitrust case, a regulatory setback for the semiconductor maker.

openbb · NVDA · Aug 3, 18:24

**「Background」** Europe&\#x27;s second-highest court, the General Court, rejected Broadcom&\#x27;s attempt to suspend an EU antitrust request for U.S.-based VMware legal documents, allowing the European Commission to continue its investigation.

**「Impact」** The EU antitrust case centers on Broadcom&\#x27;s VMware licensing changes, which removed most European cloud providers from its VMware Cloud Service Provider program, so an adverse ruling could force Broadcom to adjust those practices and affect European cloud providers that rely on VMware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/8998953/broadcom-stock-slips-after-losing-major-eu-antitrust-fight">Broadcom Stock Slips After Losing Major EU Antitrust Fight</a></li>
<li><a href="https://finance.yahoo.com/technology/articles/broadcom-loses-court-bid-suspend-155709395.html">Broadcom loses court bid to suspend EU antitrust request for US legal papers</a></li>
<li><a href="https://ca.finance.yahoo.com/news/broadcom-facing-eu-antitrust-scrutiny-over-market-dominance-235623916--finance.html">Broadcom facing EU antitrust scrutiny over market dominance...</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-03-19/cloud-industry-group-calls-for-eu-interim-measure-against-broadcom-over-vmware">Broadcom Hit With EU Antitrust Complaint and Request for Interim...</a></li>

</ul>
</details>

**Tags**: `#Broadcom`, `#EU antitrust`, `#regulatory`, `#stock movement`, `#semiconductors`

---

<a id="item-finance-news-6"></a>
### [Berkshire Hathaway, Led by Greg Abel, Closes Taylor Morrison Acquisition](https://finance.yahoo.com/markets/stocks/articles/greg-abel-closed-berkshire-hathaways-145000102.html) ⭐️ 8.0/10

Berkshire Hathaway, led by Greg Abel, closed its acquisition of homebuilder Taylor Morrison on July 24, expanding the company’s real estate-related holdings.

openbb · BRK-B · Aug 3, 14:50

**「Background」** Berkshire Hathaway completed its acquisition of homebuilder Taylor Morrison on July 24, 2026, paying $72.50 per share in cash, for a total equity value of about $6.8 billion and an enterprise value of about $8.5 billion. The deal was announced in June 2026 and is one of the first major strategic acquisitions under Greg Abel, Berkshire&\#x27;s designated successor to Warren Buffett.

**「Impact」** Berkshire Hathaway’s completion of the $8.5 billion Taylor Morrison purchase expands its homebuilding business by folding Taylor Morrison’s residential communities and financial services into the existing Clayton Properties ecosystem, increasing Berkshire’s direct exposure to the U.S. housing market.

<details><summary>References</summary>
<ul>
<li><a href="https://berkshirehathaway.com/news/jul2426.pdf">Berkshire Hathaway Completes Acquisition of Taylor Morrison</a></li>
<li><a href="https://www.cnbc.com/2026/06/01/berkshire-hathaway-taylor-morrison-home-acquisition-housing-market.html">Berkshire Hathaway buys Taylor Morrison for $6.8 ... - CNBC</a></li>
<li><a href="https://www.e-a-a.com/berkshire-hathaway-officially-acquires-taylor-morrison-for-8-5-billion/">Berkshire Hathaway Officially Acquires Taylor Morrison for $8.5 Billion – Engineers and Architects of America</a></li>
<li><a href="https://www.reuters.com/legal/transactional/berkshire-hathaway-buy-us-homebuilder-taylor-morrison-85-billion-2026-05-31/">Berkshire Hathaway to buy Taylor Morrison for $6.8 billion in cash to expand in housing | Reuters</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#Taylor Morrison`, `#M&amp;A`, `#Homebuilding`, `#Greg Abel`

---

<a id="item-finance-news-7"></a>
### [After-hours stock movers: Palantir, On Semi, Snap gain; Whirlpool falls on earnings](https://www.cnbc.com/2026/08/03/stocks-making-the-biggest-moves-after-hours-pltr-on-snap.html) ⭐️ 7.0/10

After the bell, Palantir rose 10% after blowout second-quarter results and Snap gained 11% after revenue beat estimates. On Semi rose 5% after earning 74 cents per share versus 71 cents expected, while Whirlpool fell 3% after losing 21 cents versus a 5-cent loss expected and cutting full-year guidance.

rss · CNBC Finance · Aug 3, 20:45

**「Background」** The moves came as these companies reported quarterly earnings after the market closed, a period when investors can trade on fresh results and immediately adjust prices based on beats or misses.

**Tags**: `#Earnings`, `#Stock Movers`, `#Palantir`, `#Semiconductors`, `#Snap`

---

<a id="item-finance-news-8"></a>
### [Dow Reaches Record High Amid Iran Deal Hopes](https://finance.yahoo.com/markets/stocks/articles/dow-hits-record-high-oil-203727254.html) ⭐️ 7.0/10

The Dow Jones Industrial Average hit a record high as oil prices slid on hopes that a nuclear deal with Iran could boost global crude supply, according to the article.

openbb · NVDA · Aug 3, 20:37

**「Background」** The market move reflects rising expectations of a US-Iran nuclear or peace deal, which traders see as reducing geopolitical risk and potentially increasing Iranian oil exports. Such a deal would likely ease global supply concerns, putting downward pressure on oil prices and lifting stock indexes.

<details><summary>References</summary>
<ul>
<li><a href="https://tradeedgepro.net/us-iran-deal-stock-impact/">US-Iran Peace Deal: Major Stock Gains, Sharp Oil Price Drop</a></li>

</ul>
</details>

**Tags**: `#Dow Jones`, `#Oil Prices`, `#Iran Nuclear Deal`, `#Market Update`, `#Geopolitics`

---