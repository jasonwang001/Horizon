---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 237 items, 27 important content pieces were selected

---

**Technology News**
1. [Qwen3.8-2.4T-A95B: Open 2.4T MoE Model Released](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 Draws Cost-Efficiency Tests and Mixed Reviews](#item-tech-news-2) ⭐️ 8.0/10
3. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-tech-news-3) ⭐️ 8.0/10
4. [xAI Releases Grok 4.6 Amid API and Benchmark Debate](#item-tech-news-4) ⭐️ 8.0/10
5. [What Mathematics Are LLMs Good At? Gowers Weighs In](#item-tech-news-5) ⭐️ 8.0/10
6. [Adam&\#x27;s Basis-Dependent Scaling Destroys Implicit Low-Rank Bias](#item-tech-news-6) ⭐️ 8.0/10
7. [WeChat launches resource-efficient WeLM LLM family](#item-tech-news-7) ⭐️ 8.0/10
8. [Zed announces Delta with collaborative AI editing features](#item-tech-news-8) ⭐️ 7.0/10
9. [Why Tiny JPEGs Look Different in Chrome and Firefox](#item-tech-news-9) ⭐️ 7.0/10
10. [uBlock Origin Stops Filtering Facebook Ads](#item-tech-news-10) ⭐️ 7.0/10
11. [Grok 4.6 Scores 61 on AI Index; Coding Praise and Pricing Concerns](#item-tech-news-11) ⭐️ 7.0/10
12. [LTX-2.5 Open Source Video Model Runs on a Single RTX 5090](#item-tech-news-12) ⭐️ 7.0/10
13. [Counterpoint: enterprise SSDs hit 48% of NAND shipments; YMTC enters top three](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [Federal Reserve holds interest rates steady in 9-3 vote](#item-finance-news-1) ⭐️ 9.0/10
2. [Fed Chair Kevin Warsh Testifies on Inflation and Monetary Policy](#item-finance-news-2) ⭐️ 9.0/10
3. [Bank of England publishes July 2026 Monetary Policy Report](#item-finance-news-3) ⭐️ 9.0/10
4. [CME plans AI-compute futures tied to GPU rental costs](#item-finance-news-4) ⭐️ 8.0/10
5. [Ukrainian Attack Halts Operations at Russian Black Sea Grain Terminals](#item-finance-news-5) ⭐️ 8.0/10
6. [EIA Forecasts 600,000 bpd of Middle East Oil Offline by End-2027](#item-finance-news-6) ⭐️ 8.0/10
7. [Refinery Attacks Worsen Global Diesel Supply Crunch](#item-finance-news-7) ⭐️ 8.0/10
8. [Putin Threatens to Seize EU Ships Over Shadow-Fleet Sanctions](#item-finance-news-8) ⭐️ 8.0/10
9. [Ukraine Reportedly Halts Oil Tanker and Pipeline Attacks After JD Vance Request](#item-finance-news-9) ⭐️ 8.0/10
10. [Aluminum Stockpiles Fall to Lowest Since 1990](#item-finance-news-10) ⭐️ 8.0/10
11. [Tencent Q2 revenue beats, but AI capex surge turns free cash flow negative](#item-finance-news-11) ⭐️ 8.0/10
12. [TSMC and Sony Set Up Japan Joint Venture for Smartphone Image Sensors](#item-finance-news-12) ⭐️ 8.0/10
13. [TSMC July Revenue Up 45% Year-Over-Year; Stock Still 13% Below High](#item-finance-news-13) ⭐️ 8.0/10
14. [Report: Microsoft to Raise Windows Preinstall Licensing Fees 7–10% in July 2026](#item-finance-news-14) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen3.8-2.4T-A95B: Open 2.4T MoE Model Released](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen has released Qwen3.8-2.4T-A95B, an open-weight mixture-of-experts model with 2.4T total parameters and 95B active parameters, available on Hugging Face in BF16 and FP8 formats. The model has a native context length of 262,144 tokens, extendable to 1,010,000 tokens, and is the open-weights version of Qwen3.8-Max, though it lacks vision input, non-thinking support, and built-in tools. The model card reportedly claims performance between Opus 4.8 and Fable 5, and community commenters position it as a competitor to Kimi k3. Community discussions note that the full BF16 model is roughly 4.9TB, while a 1-bit quantized variant from Unsloth is about 397GB, potentially bringing high-end performance to consumer hardware. Licensing is similar to Kimi k3 with free use for internal or under-$50M revenue scenarios, but restrictions apply above that threshold.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**「Background」** Qwen3.8-2.4T-A95B is an open-weight mixture-of-experts large language model released by the Qwen team, with 2.4 trillion total parameters and 95 billion active parameters per token. It is part of the Qwen3.8 family and supports vision and thinking capabilities, a native 262,144-token context window extendable to 1,010,000 tokens. The model weights are available in Hugging Face Transformers format on Hugging Face and ModelScope, with variants including BF16, FP8, and heavily quantized local-run options such as a 397GB 1-bit version.

**「Impact」** The open release means developers can run near-Opus-level performance locally via quantized versions, but commercial serving above $50M annual revenue will require a different license, and the lack of vision/1M context in the open model limits direct replacement of Qwen3.8-Max.

**「Community Discussion」** Commenters praise the quantized 1-bit version \(~397GB\) for putting high-end performance on consumer hardware, but they also flag that the BF16/FP8 release is harder to serve than Kimi k3 at launch and that the open model lacks vision input, non-thinking mode, and 1M context, so it is not a complete equivalent of Qwen3.8-Max. There is also debate over licensing thresholds and comparisons to DeepSeek V4-Pro-0813.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B">Qwen / Qwen 3 . 8 - 2 . 4 T - A 95 B · Hugging Face</a></li>
<li><a href="https://modelscope.ai/models/Qwen/Qwen3.8-2.4T-A95B">Qwen 3 . 8 - 2 . 4 T - A 95 B</a></li>
<li><a href="https://unsloth.ai/docs/models/qwen3.8">Qwen 3 . 8 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**Tags**: `#qwen`, `#llm`, `#mixture-of-experts`, `#model-release`, `#artificial-intelligence`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813 Draws Cost-Efficiency Tests and Mixed Reviews](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

The Hacker News submission links to OpenRouter for DeepSeek V4 Pro 0813, a newly released model, though commenters noted the page lacks useful details and pointed to the official API docs and benchmark reposts. In community testing on Codex CLI, DeepSeek V4 Pro 0813 completed a new feature development task in 12 minutes 2 seconds at $0.12 but produced a bug, while Grok 4.6 finished in 3 minutes 18 seconds at $1.41 with no bug. Another commenter reported being impressed by the previous DeepSeek Flash update for heavy development at low cost and was eager to try the new model. Overall, the discussion highlights DeepSeek&\#x27;s positioning as a low-cost option for development tasks, with trade-offs in correctness and runtime.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**「Background」** DeepSeek V4 Pro 0813 is the flagship large language model from Chinese AI lab DeepSeek, released on August 12, 2026, and accessible through APIs such as OpenRouter and Together AI. It is a 1.6-trillion-parameter mixture-of-experts \(MoE\) model that activates roughly 49 billion parameters per token, combining hybrid attention, three reasoning modes, a 1,048,576-token context window, and up to 384,000 output tokens. Its API pricing—$0.435 per million input tokens and $0.87 per million output tokens—continues DeepSeek&\#x27;s pattern of very low-cost inference relative to leading Western models, which is central to its appeal for development tasks.

**「Impact」** For developers using Codex CLI, DeepSeek V4 Pro 0813 can cut per-task costs by roughly an order of magnitude compared with Grok 4.6 \($0.12 vs $1.41\), at the cost of much longer runtime and a higher chance of shipping buggy code in this single anecdotal test.

**「Community discussion」** Comments showed split reactions: one user&\#x27;s test favored correctness \(Grok 4.6\) despite higher cost, while another praised DeepSeek&\#x27;s cost-effectiveness for heavier development and prioritized getting the job done cheaply over maximum intelligence. There was also minor criticism of linking to OpenRouter instead of official sources.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://lmmarketcap.com/model/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - Pricing &amp; Benchmarks 2026 | LM Market Cap</a></li>
<li><a href="https://www.together.ai/models/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 API: Pricing, Benchmarks &amp; Docs | Together AI</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#artificial-intelligence`, `#cost-efficiency`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale has documented how it traced database corruption to a 16-year-old race condition in SQLite&\#x27;s WAL-reset logic. The post-mortem explains the investigation and the subtle conditions that let the bug corrupt databases. As part of the debugging effort, Tailscale funded an open-source SQLite VFS shim that isolated the race condition almost immediately and can help find similar issues in the future. The story matters because it shows how even mature, heavily tested software can hide long-lived concurrency bugs and how targeted open-source funding can help close them.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**「Background」** SQLite is an embedded database that can run in write-ahead logging \(WAL\) mode, which normally allows concurrent readers alongside a single writer. Tailscale&\#x27;s post-mortem centers on a rare 16-year-old SQLite bug named &quot;WAL-Reset&quot; that could corrupt databases when WAL mode was active and multiple database connections were open to the same file, with reading and writing occurring concurrently. The bug was so difficult to trigger that the SQLite developers had to add deliberately unusual code to reproduce it; Tailscale funded an open-source SQLite VFS shim and supported the investigation to isolate the race condition.

**「Impact」** SQLite users and developers now have a detailed post-mortem and an open-source diagnostic shim for identifying WAL-reset race conditions.

**「Community Discussion」** Commenters praised the article and Tailscale&\#x27;s decision to fund open-source debugging tooling, with one noting that the race was surprising given SQLite&\#x27;s intended single-writer usage. Several expressed appreciation for the write-up and hoped Tailscale would maintain its SQLite support contract; a few wanted the story to reach the point faster, but the overall response was positive.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.theregister.com/databases/2026/08/12/tailscale-says-deeply-buried-16-year-old-sqlite-bug-caused-last-years-outages/5287004">Tailscale says deeply buried 16-year-old SQLite bug caused last year&#x27;s outages</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#database`, `#bug-fix`, `#postmortem`, `#tailscale`

---

<a id="item-tech-news-4"></a>
### [xAI Releases Grok 4.6 Amid API and Benchmark Debate](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI released Grok 4.6, a new version of its AI model, according to the announcement at x.ai/news/grok-4-6. The release has sparked early community discussion about API behavior, benchmark performance, and competition with other frontier models. Some developers report that the API injects a default system prompt that overrides custom instructions and can cause the model to refuse discussion of system prompts. Other users highlight Grok 4.6’s speed and concise responses in agentic workflows, while some question how major labs achieved comparable benchmark scores so quickly. Specific technical specifications, benchmark numbers, and pricing details were not provided in the available source material.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**「Background」** Grok 4.6 is xAI&\#x27;s latest frontier AI model, a 2-trillion-parameter system that matches GPT-5.6 Sol on the Artificial Analysis Intelligence Index, a composite of nine benchmarks, while targeting Kimi K3-level capability at Grok 4.5 speed. It is optimized for agentic coding and knowledge work, with a 500,000-token context window and API pricing of $2 per million input tokens and $6 per million output tokens. The model is expected to be available through the xAI API, Grok app, SuperGrok, and X Premium+, with closed weights, continuing xAI&\#x27;s expansion of its inference capabilities.

**「Impact」** For developers using the Grok API, the reported default system prompt that overrides user instructions could disrupt applications relying on custom system prompts.

**「Community Discussion」** Commenters are split: some criticize the API&\#x27;s injected system prompt for overriding custom instructions and causing refusals, while others praise Grok 4.6 for being fast, concise, and pleasant to use in agentic contexts. A few question how multiple labs reached Fable-level performance within two months, suggesting benchmark gaming or rapid technique circulation.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>
<li><a href="https://kie.ai/blog/what-is-grok-4-6">What Is Grok 4 . 6 ? xAI &#x27;s 2T-Param Model Explained</a></li>
<li><a href="https://openrouter.ai/x-ai/grok-4.6">Grok 4 . 6 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#machine-learning`, `#LLM`, `#xAI`, `#technology-industry`

---

<a id="item-tech-news-5"></a>
### [What Mathematics Are LLMs Good At? Gowers Weighs In](https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/) ⭐️ 8.0/10

Timothy Gowers, a Fields Medalist, examines which mathematical tasks LLMs handle well, arguing in a blog post that much of their apparent success reflects test-time scaling — letting models sample or talk to themselves longer — rather than deep reasoning. He proposes that a convincing sign of human-level theorem proving would be methods that are new, surprising, and beautiful with hindsight, yet hard to stumble on by accident. Commenters connect this to AlphaCode&\#x27;s 2022 result, which beat the average human programmer by generating millions of candidate programs and filtering them, and note LLMs&\#x27; apparent strength in searching for counterexamples and examples. The discussion highlights uncertainty about whether current approaches will extend to harder mathematical reasoning.

hackernews · ColinWright · Aug 12, 10:04 · [Discussion](https://news.ycombinator.com/item?id=49270022)

**「Background」** Timothy Gowers is a Fields Medalist and mathematician at the Collège de France who has written extensively about the capabilities of large language models \(LLMs\) in mathematics. LLMs are statistical text predictors rather than symbolic theorem provers, so their mathematical competence varies widely: they can excel at pattern recognition, generation, and search, yet still struggle with rigorous, creative proofs. This blog post builds on recent demonstrations of LLMs solving olympiad-style problems and other mathematical tasks, while noting that they have not yet outpaced human mathematicians across all aspects of the field.

**「Impact」** Mathematicians and AI researchers evaluating LLM theorem proving now have a sharper, albeit informal, benchmark — proofs that are new, surprising, beautiful in hindsight, and hard to discover by accident — although the excerpted material does not provide Gowers&\#x27; full inventory of LLM strengths and weaknesses.

**「Community Discussion」** Commenters largely agree that the post is really about test-time scaling, and they cite AlphaCode&\#x27;s 2022 sampling-based approach as an early illustration that generating and filtering many candidates is where LLMs shine. Others note an observed affinity for finding counterexamples or examples, and one commenter wonders whether models might crash on temporal logic given coding agents&\#x27; difficulties with concurrent code.

<details><summary>References</summary>
<ul>
<li><a href="https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/">What sort of maths are LLMs good at? | Gowers&#x27;s Weblog</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#mathematics`, `#AI research`, `#test-time scaling`, `#theorem proving`

---

<a id="item-tech-news-6"></a>
### [Adam&\#x27;s Basis-Dependent Scaling Destroys Implicit Low-Rank Bias](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

Adam&\#x27;s per-coordinate second-moment scaling is not rotation-invariant in factored models W=UV^T, and this anisotropy—not adaptivity in general—determines whether optimizers retain gradient descent&\#x27;s implicit low-rank bias. Across nine update rules tested on underdetermined matrix sensing at matched training loss, GD, shared-scalar Adam, Muon, and Shampoo preserved the bias while Adam, RMSProp, Lion, signum, and Adafactor lost it; a one-parameter interpolation from per-coordinate to shared-scalar denominators monotonically improved recovery. Muon was exact on truly low-rank targets but degraded fastest as spectral tail energy was added, ceding to GD near 4% tail energy, which reconciles previously conflicting Muon results. The author also found their own optimizer&\#x27;s per-coordinate clip was breaking its intended structure, and switching to a global norm clip reduced recovery error from 0.347 to 0.220. The reported 43–44% held-out error reduction on hyperspectral data relies on a train-only learning-rate rule that hands Adam its worst rate; allowing each method its own best rate shrinks the gap considerably, so the mechanism rather than the headline number is the claim.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**「Background」** Many neural-network optimizers inherit an implicit bias toward low-rank solutions when training factored weights W = UV^T, a structure whose loss is unchanged by rotating the factors with an orthogonal matrix Q \(U→UQ, V→VQ\). Gradient descent preserves this rotation invariance, but Adam&\#x27;s second-moment estimate is computed per coordinate, so the update depends on the basis in which the factors are written; the supplied paper argues this anisotropy is the mechanism that makes Adam-style optimizers lose the implicit low-rank bias. Related optimizers are not all alike: Muon and Shampoo are linked through matrix preconditioning and orthogonalization, and recent work treats Muon as an approximate Shampoo, yet the paper reports that Muon and Shampoo retain the bias while Adam, RMSProp, Lion, signum, and Adafactor do not.

**「Impact」** This work implies that Adam-family optimizers lose GD&\#x27;s implicit low-rank bias in factored models, so practitioners should consider common-scalar or global-norm updates—though the reported 43-44% hyperspectral improvement is partly an artifact of the train-only learning-rate rule and shrinks after per-method tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>
<li><a href="https://arxiv.org/html/2608.05136">The Loss Does Not See the Basis, but Adam Does</a></li>
<li><a href="https://arxiv.org/pdf/2502.04664">Implicit Bias of Spectral Descent and Muon on Multiclass Separable Data</a></li>
<li><a href="https://arxiv.org/abs/2608.05136">[2608.05136] The Loss Does Not See the Basis , but Adam Does</a></li>
<li><a href="https://deeplearn.org/arxiv/802261/the-loss-does-not-see-the-basis,-but-adam-does">The Loss Does Not See the Basis , but Adam Does - Paper Detail</a></li>

</ul>
</details>

**Tags**: `#optimizers`, `#implicit-bias`, `#low-rank`, `#Adam`, `#machine-learning`

---

<a id="item-tech-news-7"></a>
### [WeChat launches resource-efficient WeLM LLM family](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 8.0/10

WeChat&\#x27;s team announced WeLM, a general-purpose large language model family centered on resource efficiency, and confirmed that the WeLM-80B model—which activates only 3B parameters—already powers the in-WeChat AI agent Xiaowei for dialogue, search, native WeChat operations, and mini-program services. The team is also developing WeLM-617B, a mixture-of-experts \(MoE\) model with 23B active parameters, intended to deliver stronger general understanding and reasoning at a moderate active scale for complex WeChat ecosystem tasks such as mini-program intelligent development and Xiaowei small-tool generation. The announcement signals Tencent&\#x27;s push to deploy large models in production across its massive WeChat user base while emphasizing lower inference costs through sparse activation.

telegram · zaihuapd · Aug 12, 13:58

**「Background」** WeLM is a family of general-purpose large language models developed by WeChat/Tencent, designed with a strong emphasis on resource efficiency by activating only a subset of parameters during inference. The series includes the production-ready WeLM-80B \(3B active parameters\) and the under-development WeLM-617B \(23B active parameters\) which uses a mixture-of-experts \(MoE\) architecture. The models were previously documented in a July paper by the WeChat team, and the 80B model was pre-trained on 11T tokens followed by an annealing phase on 1.4T high-quality tokens.

**「Impact」** WeChat users can already interact with the WeLM-80B-backed agent inside the app for search, conversation, and mini-program access, while developers may later benefit from the planned WeLM-617B model for mini-program development and tool generation, though its release timeline is not yet announced.

<details><summary>References</summary>
<ul>
<li><a href="https://www.weex.com/news/detail/wechat-launches-welm-large-model-series-to-drive-ai-application-implementation-c0pmz8w994lglikkdnsi3ndr">WeChat Launches WeLM Large Model Series to... | WEEX Crypto News</a></li>
<li><a href="https://en.theblockbeats.news/flash/361266">WeChat Introduces WeLM Dual Model : 80 B Model Empowering Mini...</a></li>
<li><a href="https://welm.weixin.qq.com/en/posts/building-effective-sparse-moe-models-with-moderate-resources/">Building Effective Sparse MoE Models with Moderate... | WeLM Blog</a></li>

</ul>
</details>

**Tags**: `#WeLM`, `#large language models`, `#mixture-of-experts`, `#resource efficiency`, `#WeChat AI`

---

<a id="item-tech-news-8"></a>
### [Zed announces Delta with collaborative AI editing features](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed has announced Delta, a new set of features for its editor that introduces realtime collaborative multiplayer conversations and conversation-as-document functionality, allowing users to comment inline within an AI agent&\#x27;s conversation. The update also reportedly includes AI-assisted code summaries, building on Zed&\#x27;s existing built-in AI agent. These features aim to bring multi-user editing and more interactive AI assistance into the development workflow, though the announcement has generated mixed reactions about their practical value. Specific release details, version numbers, and technical specifications were not included in the available information.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**「Background」** Zed is a high-performance, multiplayer code editor from the creators of Atom and Tree-sitter, designed for speed and collaborative editing. Delta is a new, separate application built on the same performance-focused principles instead of being added to Zed directly, and it introduces features such as real-time collaborative multiplayer conversations and inline comments within agent conversations. The project&\#x27;s longer-term plan is to integrate Delta&\#x27;s underlying DeltaDB capabilities into Zed itself.

**「Impact」** Zed users who collaborate on code or mentor less experienced contributors may gain new ways to work together in real time and review AI agent decisions, while developers who prefer single-player coding workflows may find little immediate use for the multiplayer features.

**「Community discussion」** Commenters are sharply divided: some praise Zed&\#x27;s speed and built-in AI but see no need for multi-user editing, others express frustration with verbose or incomplete AI-generated code summaries, and a few find the collaborative conversation features useful for mentoring and reviewing pull requests. A separate commenter also criticized the post&\#x27;s low-contrast design for hurting readability.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-delta">Introducing Delta — Zed &#x27;s Blog</a></li>
<li><a href="https://github.com/zed-industries/zed">GitHub - zed -industries/ zed : Code at the speed of thought – Zed is...</a></li>

</ul>
</details>

**Tags**: `#Zed`, `#collaborative-editing`, `#AI-code-assist`, `#software-engineering`, `#editor`

---

<a id="item-tech-news-9"></a>
### [Why Tiny JPEGs Look Different in Chrome and Firefox](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 7.0/10

This post explains why tiny JPEG images render differently in Chrome and Firefox, attributing the difference to the browsers’ downscaling algorithms and Chrome’s JPEG decoding/optimization path. The issue matters for web developers, because small icons and thumbnails can end up visibly blurrier in Chrome than in Firefox. The author advises against using JPEG for icons and recommends supplying images at an appropriate resolution, with formats like PNG to avoid compression artifacts. The post also points to ongoing Firefox work on lower-scale decompression and acknowledges that browser behavior in this area is not fully consistent.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**「Background」** Browser engines resample images when the display size is smaller than the source dimensions, and each engine uses its own scaling algorithm with different trade-offs. JPEG’s lossy compression can amplify artifacts when images are heavily downscaled. Chrome and Firefox have diverged in how they handle these very small rendered images, leading to the visual discrepancy described in the post.

**「Impact」** Developers who use tiny images for icons or UI assets may see inconsistent visuals across Chrome and Firefox, which can be hard to diagnose; switching to appropriately sized PNG or other lossless images is the concrete fix recommended by the article.

**「Community Discussion」** Commenters confirm the discrepancy also affects PNGs and note that it once disrupted an Electron app upgrade, and they observe that Chrome tends to be blurrier while Firefox is sharper but has ringing artifacts, with one commenter preferring Firefox’s output. They link to Firefox’s Bugzilla work on decompressing at lower scales \(bug 2033250\) and mention \`image-rendering\` CSS as a partial workaround, while agreeing that using appropriately sized images is the best approach.

**Tags**: `#web development`, `#browser rendering`, `#image scaling`, `#JPEG`, `#Chrome`

---

<a id="item-tech-news-10"></a>
### [uBlock Origin Stops Filtering Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 7.0/10

According to a Neowin report shared on Reddit&\#x27;s r/uBlockOrigin, the open-source ad blocker uBlock Origin has stopped filtering ads on Facebook because Facebook&\#x27;s countermeasures made the cat-and-mouse effort unsustainable. The decision means Facebook users running uBlock Origin can expect ads to appear again on the platform, at least until community filters or new approaches step in. The move marks a notable escalation in the ad-blocking arms race, though the original article provides few additional technical details.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**「Background」** uBlock Origin is a widely used open-source browser extension that blocks ads and trackers through community-maintained filter lists. It has spent years in a back-and-forth technical battle with Facebook, which continually changes how ads are served to avoid filtering. According to a development team member on the uBlockOrigin subreddit, the project has now decided to stop filtering Facebook ads entirely, citing the difficulty of keeping up.

**「Impact」** Users who rely on uBlock Origin on Facebook will lose ad-blocking coverage there, and the project is signaling it will not spend more engineering effort on that specific arms race.

**「Community Discussion」** Commenters in the Reddit thread largely accepted the decision as pragmatic, while some predicted ad-blocking will eventually turn to computer-vision models that detect ads on screen. A few said the only reliable alternative is limiting or leaving Facebook; others questioned why advertisers keep pursuing users who block ads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.resetera.com/threads/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them.1601830/">Facebook ads are so hard to block that uBlock Origin stopped ...</a></li>

</ul>
</details>

**Tags**: `#ad-blocking`, `#uBlock Origin`, `#Facebook`, `#privacy`, `#open source`

---

<a id="item-tech-news-11"></a>
### [Grok 4.6 Scores 61 on AI Index; Coding Praise and Pricing Concerns](https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis) ⭐️ 7.0/10

Grok 4.6 has scored 61 on the Artificial Analysis Intelligence Index, according to an Artificial Analysis article. The result positions the model among frontier AI systems and has drawn community attention to its coding performance, speed, and pricing changes. In particular, users have praised the interactive coding experience and compared access costs with competitors. The release appears to represent an incremental improvement over previous versions rather than a major paradigm shift.

hackernews · wertyk · Aug 12, 16:54 · [Discussion](https://news.ycombinator.com/item?id=49275385)

**「Background」** Grok 4.6 is SpaceXAI&\#x27;s latest frontier model, scoring 61 on the Artificial Analysis Intelligence Index, a composite benchmark that evaluates models across reasoning, knowledge, mathematics, and coding. The index aggregates nine benchmarks; on it, Grok 4.6 matches GPT-5.6 Sol, while on the separate AA-Briefcase agentic benchmark it reaches an Elo of 1577, behind the Claude Opus 5 family.

**「Impact」** For heavy coding users, a reported increase in cache-read pricing from $0.30 to $0.50 between Grok 4.5 and 4.6 could materially raise token costs in long sessions.

**「Community Discussion」** Commenters largely praised Grok for its communication style and speed in coding, noting Cursor&\#x27;s bundled access makes it a strong value, but one user flagged that cache-read pricing nearly doubled from $0.30 in Grok 4.5 to $0.50 in Grok 4.6, which could affect heavy coding bills.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis">Grok 4 . 6 returns SpaceXAI to the intelligence frontier and leads on...</a></li>
<li><a href="https://artificialanalysis.ai/models/grok-4-6">Grok 4 . 6 (high) - Intelligence , Performance &amp; Price Analysis</a></li>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Grok`, `#benchmarks`, `#LLM`, `#machine learning`

---

<a id="item-tech-news-12"></a>
### [LTX-2.5 Open Source Video Model Runs on a Single RTX 5090](https://ltx.io/model/ltx-2-5) ⭐️ 7.0/10

LTX released its open-source video generation foundation model LTX-2.5, making the weights, training code, and inference pipeline fully available. The model can run locally on a single RTX 5090, and commercial use is free for companies with annual revenue below $10 million. LTX-2.5 supports both text-to-video and image-to-video generation, with improved multi-shot coherence and prompt following, and uses a new diffusion video decoder alongside the Gemma 4 12B text encoder. In a 98-prompt text-to-video defect evaluation, LTX 2.5 Pro ranked first among ten models. The announcement provides the model&\#x27;s capabilities and licensing terms but lacks deep technical details and independent validation.

telegram · zaihuapd · Aug 12, 02:15

**「Background」** LTX is the open video generation model family from Lightricks, which previously released LTX Video in November 2024 and an upgraded 13B-parameter LTXV in May 2025. LTX-2.5 is the latest open-weights foundation model, positioned to run locally on consumer hardware and to allow fine-tuning, with multi-shot scene generation, 4K output, and free commercial use for companies under $10M in annual recurring revenue.

**「Impact」** Developers and smaller companies can now generate video locally on a high-end consumer GPU without per-use API costs, while the revenue-based licensing threshold enables free commercial use for most independent creators.

<details><summary>References</summary>
<ul>
<li><a href="https://ltx.io/model/ltx-2-5">LTX - 2 . 5 : LTX &#x27;s Latest AI Open - Source Foundation Model | LTX</a></li>
<li><a href="https://www.dreampixelforge.com/blog/ltx-2-5">LTX 2 . 5 : Open Weights, Specs, and How to Run It | Dream Pixel Forge</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#open source`, `#LTX`, `#AI models`, `#local inference`

---

<a id="item-tech-news-13"></a>
### [Counterpoint: enterprise SSDs hit 48% of NAND shipments; YMTC enters top three](https://china.counterpointresearch.com/%e6%9c%8d%e5%8a%a1%e5%99%a8%e9%9c%80%e6%b1%82%e6%8e%a8%e5%8d%87%e4%bc%81%e4%b8%9a%e7%ba%a7-ssd-%e5%8d%a0-nand-%e5%87%ba%e8%b4%a7%e9%87%8f%e7%99%be%e5%88%86%e4%b9%8b-48/) ⭐️ 7.0/10

According to Counterpoint, enterprise SSDs accounted for 48% of global NAND shipments in Q2 2026, nearly double the share from a year earlier, driven by AI inference workloads, and industry revenue in the segment grew fivefold year over year. By shipment share, Samsung led with 25%, SK hynix followed with 22%, and YMTC reached third place with 14%, overtaking Kioxia for the first time. However, YMTC ranked only fifth by revenue because its products skew toward consumer-grade NAND. The report expects enterprise SSDs to consume more than half of all NAND bits by the end of the year.

telegram · zaihuapd · Aug 12, 11:00

**「Background」** NAND flash memory is the storage component in solid-state drives; enterprise SSDs are built for servers and data-center workloads, offering higher endurance and performance than consumer drives. AI inference and training increase demand for fast storage, and YMTC is a Chinese NAND manufacturer that competes in both consumer and enterprise segments.

**「Impact」** The trend makes enterprise SSD demand the primary driver of NAND bit consumption, with implications for memory suppliers&\#x27; product mix and AI infrastructure procurement; YMTC&\#x27;s lower revenue rank shows that shipment leadership does not automatically mean revenue leadership.

**Tags**: `#NAND`, `#Enterprise SSD`, `#AI workloads`, `#Memory market`, `#YMTC`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Federal Reserve holds interest rates steady in 9-3 vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

The Federal Reserve voted 9-3 to leave interest rates unchanged, according to ABC7 Los Angeles.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Open Market Committee \(FOMC\), the Fed&\#x27;s policy-setting committee, held the federal funds rate at 3.50%-3.75% in June, and this is Chair Kevin Warsh&\#x27;s second meeting leading the committee.

**「Impact」** The decision keeps borrowing costs for households and businesses at the unchanged federal funds rate of 3.50%–3.75%, preserving the current level of financing expenses for loans tied to the benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://nypost.com/2026/07/29/business/fed-holds-interest-rates-steady-as-dissent-mounts-over-whether-to-hike-rates-soon/">Fed holds interest rates steady as dissent mounts over whether to...</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#central bank`

---

<a id="item-finance-news-2"></a>
### [Fed Chair Kevin Warsh Testifies on Inflation and Monetary Policy](https://news.google.com/rss/articles/CBMitwFBVV95cUxNNGoza1B1bFlYakZUZTlfMDZXQW5lak5PUUJmazNOUTZXdzZsb0ZfaUdNRmRZSmRHQmVLM1YweXBYaG5QWko3UE9pWk13MThsazJXZnAxZXQzdjFBNS1JQndtTU5WYzNjbExBWFVmaHRiUGlzNVB6WW9yTmdwQWdyWGNvWktMMWpQcXZrVWFtVGxwYW5WUEY1WEhJUWw2MTFfaFFBREMxQkVfUmx6WGVsNzZoU1AwYjjSAbwBQVVfeXFMTmJaLU9CcDhYZjVFbnJ1OEk5MFdNTzNNNlNQcjZTNnBndmtVMUFaaGVhYVZaR05MMnVKekp6NmlLdXZRbUwyUEdmLUZvT3h1bkVsVEZoR0k3MFN2QXIxTmY5bUtPdVVBODgwMHBiSDlqbl96VU9xSHppMGY4Q1M1VTVRVXl3VldVQ1dMTHoxNndVcDd5VEUySWZhSmU1RWtsSVpvUFVWWkI5T3Bfdy1FWHN2Zy1GT0R4UnhmN1M?oc=5) ⭐️ 9.0/10

Federal Reserve Chair Kevin Warsh testified before a House hearing on inflation and monetary policy, according to live coverage from PBS.

google\_news · PBS · Jul 13, 07:00

**「Background」** Warsh was appearing before the House Financial Services Committee for the semiannual Monetary Policy Report to Congress, his first such testimony as Fed chair, where he pledged to make high inflation &\#x27;a thing of the past&\#x27; but gave no signal about the central bank&\#x27;s next steps.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/politics/watch-live-fed-chair-kevin-warsh-testifies-on-monetary-policy-in-house-hearing">WATCH: Fed chair Kevin Warsh testifies on inflation and monetary policy in House hearing | PBS News</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/testimony/warsh20260714a.htm">Testimony by Chairman Warsh on the semiannual Monetary Policy Report to Congress - Federal Reserve Board</a></li>
<li><a href="https://www.cnbc.com/2026/07/14/warsh-promises-inflation-will-be-a-thing-of-the-past-cites-benefits-of-ai-investment-boom.html">Warsh pledges Fed policy &#x27;regime change&#x27; to rid inflation &#x27;tax&#x27; on American people</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Congress`, `#Kevin Warsh`

---

<a id="item-finance-news-3"></a>
### [Bank of England publishes July 2026 Monetary Policy Report](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

The Bank of England released its July 2026 Monetary Policy Report, presenting its latest policy stance and economic outlook for the UK, including projections for inflation and growth. No specific policy change or forecast figures were included in this item.

google\_news · Bank of England · Jul 30, 07:00

**「Background」** The Bank of England’s quarterly Monetary Policy Report explains the economic analysis and inflation projections behind the Monetary Policy Committee’s interest rate decisions. In its July 2026 decision, the Committee voted 6–3 to keep Bank Rate at 3.75%, with three members preferring to raise it by 0.25 percentage points to 4%.

**「Impact」** Bank of England&\#x27;s Monetary Policy Committee voted 6–3 to keep Bank Rate at 3.75%, so UK households and businesses with variable-rate loans or mortgages will continue to face the same borrowing costs for now, even though three members wanted a 0.25 percentage point rise to 4%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/2026/july-2026">Monetary Policy Report - July 2026 (to be published at 12pm) | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-summary-and-minutes/2026/july-2026">Bank Rate maintained at 3.75% - July 2026 Monetary Policy Summary and Minutes | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-summary-and-minutes/2026/july-2026">Bank Rate maintained at 3.75% - July 2026 Monetary Policy Summary and Minutes | Bank of England</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#inflation`, `#economic outlook`

---

<a id="item-finance-news-4"></a>
### [CME plans AI-compute futures tied to GPU rental costs](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 8.0/10

CME Group plans to launch the first futures contracts tied to AI computing power on Oct. 5, pending regulatory approval, based on Silicon Data indexes that track hourly rental prices for Nvidia’s H100 and Blackwell B200 GPUs. Each contract represents one month’s rent for an H100 and would create a public, tradable benchmark for AI computing costs, according to the exchange and Silicon Data.

rss · CNBC Finance · Aug 12, 14:14

**「Background」** CME Group and Silicon Data first announced their partnership on May 12, 2026. Silicon Data, backed by trading firm DRW, provides the underlying GPU rental-rate indexes that the futures will track, including a new GPU Forward Curve launched last month.

**「Impact」** The contracts could let investors gain exposure to AI compute prices without buying chips or data centers, while AI developers and data-center operators could use them to hedge rental costs and revenue.

<details><summary>References</summary>
<ul>
<li><a href="https://siliconangle.com/2026/05/12/cme-group-silicon-data-launch-ai-compute-futures-market/">CME Group and Silicon Data to launch AI compute futures market</a></li>
<li><a href="https://cryptobriefing.com/cme-group-compute-futures-launch/">CME Group launches compute futures for trading on October 5</a></li>

</ul>
</details>

**Tags**: `#AI`, `#futures`, `#CME`, `#Nvidia`, `#financial innovation`

---

<a id="item-finance-news-5"></a>
### [Ukrainian Attack Halts Operations at Russian Black Sea Grain Terminals](https://oilprice.com/Geopolitics/Europe/Ukrainian-Attack-Halts-Operations-at-Key-Russian-Black-Sea-Grain-Terminals.html) ⭐️ 8.0/10

Reuters reports, citing four industry sources, that a Ukrainian drone and missile strike on Novorossiysk on Wednesday suspended operations at two of Russia&\#x27;s biggest Black Sea grain terminals; three people were killed, including a child, and 24 were injured.

rss · OilPrice.com · Aug 12, 23:00

**「Background」** Novorossiysk is a key export hub for Russia, the world&\#x27;s largest wheat exporter, and most exports leave via Black Sea ports; last month Russia&\#x27;s main grain lobby warned such attacks could shut down grain exports and cause hunger in Africa and the Middle East.

**「Impact」** The attack threatens global food supplies, especially for African importers, and Novorossiysk residents now face restricted water delivery after the strike damaged water mains.

**Tags**: `#Grain Exports`, `#Black Sea`, `#Ukraine Conflict`, `#Russia`, `#Food Security`

---

<a id="item-finance-news-6"></a>
### [EIA Forecasts 600,000 bpd of Middle East Oil Offline by End-2027](https://oilprice.com/Energy/Crude-Oil/EIA-Sees-600000-Bpd-of-Middle-East-Oil-Still-Offline-by-End-2027.html) ⭐️ 8.0/10

The U.S. Energy Information Administration \(EIA\) forecasts that about 600,000 barrels per day \(bpd\) of Middle East oil output will remain offline by the end of 2027 because of prolonged constraints in the Strait of Hormuz. The agency also raised its third-quarter Brent crude price forecast by $11 per barrel to about $85.

rss · OilPrice.com · Aug 12, 22:00

**「Background」** The Strait of Hormuz, a vital route for Gulf oil exports, has been severely constrained by Middle East tensions since late July. The EIA estimated Middle East production shut-ins averaged 5.5 million bpd in July, down from 10.1 million bpd in March-May.

**Tags**: `#oil supply`, `#Strait of Hormuz`, `#EIA forecast`, `#Middle East`, `#crude oil prices`

---

<a id="item-finance-news-7"></a>
### [Refinery Attacks Worsen Global Diesel Supply Crunch](https://oilprice.com/Energy/Energy-General/Refinery-Attacks-Deepen-Global-Diesel-Supply-Crunch.html) ⭐️ 8.0/10

Fresh Ukrainian and Houthi attacks on refining facilities in Russia and Saudi Arabia deepened the global diesel supply crunch, with U.S. diesel futures jumping 7.4% to $4.19 per gallon on Monday and average U.S. retail diesel at $5.32 per gallon on Tuesday, according to AAA data cited in the article.

rss · OilPrice.com · Aug 12, 20:00

**「Background」** Diesel is used for freight, farming and heating, and global fuel supply was already tight because of the Middle East conflict, Ukrainian drone strikes on Russian refineries, and Russia&\#x27;s diesel export ban, which the article says is not expected to be lifted until 2027.

**「Impact」** Because diesel powers transport, farming and heating, sustained high fuel prices can be passed on to consumers and feed broader inflation; U.S. diesel inventories are also at their lowest for this time of year in 30 years, according to Reuters data cited in the article.

**Tags**: `#diesel supply`, `#refinery attacks`, `#refining margins`, `#energy markets`, `#inflation`

---

<a id="item-finance-news-8"></a>
### [Putin Threatens to Seize EU Ships Over Shadow-Fleet Sanctions](https://oilprice.com/Latest-Energy-News/World-News/Putin-Opens-New-Front-in-Shadow-Fleet-Fight-With-Threat-to-Seize-EU-Ships.html) ⭐️ 8.0/10

Russian President Vladimir Putin threatened Wednesday to respond in kind and seize European ships if EU countries confiscate Russian vessels or sell their cargo, saying retaliation would not necessarily be limited to the same waters. The warning follows the EU&\#x27;s 21st sanctions package, adopted July 23, which added 41 vessels to the shadow-fleet blacklist for a total of 673, and comes as European countries had seized nine suspected shadow-fleet tankers by late June.

rss · OilPrice.com · Aug 12, 17:30

**「Background」** The shadow fleet is made up of tankers used to move Russian oil outside Western sanctions; the latest EU package also expanded restrictions on bunkering services and on entities working for Russian oil producers.

**Tags**: `#Russia`, `#Sanctions`, `#Oil`, `#Shipping`, `#Energy`

---

<a id="item-finance-news-9"></a>
### [Ukraine Reportedly Halts Oil Tanker and Pipeline Attacks After JD Vance Request](https://oilprice.com/Latest-Energy-News/World-News/Ukraine-Halts-Oil-Tanker-Attacks-on-JD-Vance-Request.html) ⭐️ 8.0/10

Ukraine has reportedly suspended drone attacks on oil tankers and the CPC pipeline at Novorossiysk after a request by U.S. Vice-President JD Vance, according to the Financial Times citing unnamed Ukrainian officials. The attacks had cut Kazakhstan&\#x27;s daily crude output to about 1 million barrels in late July, down from over 2 million barrels in June.

rss · OilPrice.com · Aug 12, 14:30

**「Background」** The Caspian Pipeline Consortium \(CPC\) carries most of Kazakhstan&\#x27;s crude exports to the Black Sea port of Novorossiysk and had been shut down twice by drone attacks over the past two months, with Ukrainian forces also targeting tankers at the port.

**「Impact」** Kazakhstan, which sends about 80% of its oil exports through CPC, said it is considering alternative export routes via Azerbaijan, including the Baku-Tbilisi-Ceyhan system and the Baku-Supsa route.

**Tags**: `#Oil Markets`, `#Geopolitics`, `#Kazakhstan Exports`, `#Ukraine Conflict`, `#Energy Supply`

---

<a id="item-finance-news-10"></a>
### [Aluminum Stockpiles Fall to Lowest Since 1990](https://oilprice.com/Metals/Commodities/LME-Aluminum-Stockpiles-Sink-to-Lowest-Level-Since-1990.html) ⭐️ 8.0/10

Aluminum stockpiles in London Metal Exchange warehouses fell to 250,000 metric tons, their lowest since November 1990, after Norsk Hydro halved output at its Alunorte alumina refinery in Brazil because of natural gas shortages.

rss · OilPrice.com · Aug 12, 14:00

**「Background」** Alunorte, in Barcarena, Brazil, is the world&\#x27;s largest single-site alumina refinery, with annual capacity of 6.3 million metric tons. It needs natural gas for high-temperature heat and steam in the refining process, so gas outages force lower throughput.

**「Impact」** The article says higher aluminum and copper prices will make electrification and decarbonization more expensive for manufacturers and grid developers that depend on these metals.

**Tags**: `#aluminum`, `#Norsk Hydro`, `#LME inventories`, `#supply disruption`, `#copper`

---

<a id="item-finance-news-11"></a>
### [Tencent Q2 revenue beats, but AI capex surge turns free cash flow negative](https://wallstreetcn.com/articles/3779275) ⭐️ 8.0/10

Tencent reported Q2 2026 revenue of 204.8 billion yuan, up 11% year over year and slightly above Bloomberg estimates, but net profit rose only 0.7% to 56 billion yuan, missing expectations, as capital expenditure almost tripled to 52.8 billion yuan and free cash flow turned negative at -13.8 billion yuan.

telegram · zaihuapd · Aug 12, 10:30

**「Background」** Excluding prepayments for AI computing power, Tencent said free cash flow was 37.6 billion yuan, showing the spending surge was concentrated in AI infrastructure.

**Tags**: `#Tencent`, `#earnings`, `#capital expenditure`, `#free cash flow`, `#AI investment`

---

<a id="item-finance-news-12"></a>
### [TSMC and Sony Set Up Japan Joint Venture for Smartphone Image Sensors](https://finance.yahoo.com/technology/articles/tsmc-sony-establish-jv-japan-133700498.html) ⭐️ 8.0/10

TSMC and Sony have established a joint venture in Japan to develop smartphone image sensors, marking a strategic collaboration in the semiconductor supply chain.

openbb · NVDA · Aug 12, 13:37

**「Background」** Sony and TSMC have agreed to form a joint venture to develop and make smartphone image sensors in Kumamoto, Japan, with mass production expected to start in 2029. Sony will own about 60% and be the controlling shareholder; TSMC will own about 40%. Reports put the planned investment at roughly $4.7 billion, though another report cites $6.3 billion.

**「Impact」** Reports say the companies plan to invest $6.3 billion, with production of next-generation sensors targeted for 2029, which would strengthen Sony&\#x27;s position as the largest image sensor maker and TSMC&\#x27;s leading contract chipmaker role.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marketscreener.com/news/sony-group-tsmc-to-form-4-7-billion-image-sensor-joint-venture-ce7859dad081f523">Sony Group, TSMC to Form $4.7 Billion Image - Sensor Joint Venture</a></li>
<li><a href="https://www.mobileworldlive.com/devices/sony-tsmc-agree-4-7b-image-sensor-jv/">Sony , TSMC agree $4.7B image sensor JV - Mobile World Live</a></li>
<li><a href="https://www.khaleejtimes.com/business/sony-tsmc-to-spend-63-billion-to-jointly-make-image-sensors-nikkei-says">Sony , TSMC to spend $6.3 billion to jointly make image sensors ...</a></li>
<li><a href="https://www.nigeriaprivateschools.com/index.php/en/post-detail/3169/Sony-and-TSMC-to-Spend-$6.3-Billion-to-Jointly-Make-Image-Sensors">Sony and TSMC to Spend $6.3 Billion to Jointly Make Image Sensors</a></li>
<li><a href="https://asia.nikkei.com/business/tech/semiconductors/sony-tsmc-to-invest-6.3bn-in-advanced-image-sensor-plant-in-kumamoto">Sony , TSMC to invest $6.3bn in advanced image sensor... - Nikkei Asia</a></li>
<li><a href="https://aninews.in/news/business/tsmc-sony-semiconductor-solutions-to-establish-image-sensor-joint-venture-in-kumamoto20260509142020/">TSMC , Sony Semiconductor Solutions to establish image sensor...</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#Sony`, `#joint venture`, `#semiconductors`, `#image sensors`

---

<a id="item-finance-news-13"></a>
### [TSMC July Revenue Up 45% Year-Over-Year; Stock Still 13% Below High](https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductors-july-revenue-rose-075800266.html) ⭐️ 8.0/10

Taiwan Semiconductor \(TSMC\) reported July revenue rose 45% from a year earlier, an actual company result, while its stock remains about 13% below its all-time high, according to the report.

openbb · NVDA · Aug 12, 07:58

**「Background」** TSMC, the world&\#x27;s largest contract chipmaker, has been expanding production capacity, including a new plant in Japan slated for 2027, and its recent sales growth is attributed to strong demand for AI chips.

**「Impact」** TSMC’s July revenue reached 467.58 billion new Taiwan dollars, up 45% from a year earlier, fueled by continued demand for AI-related chips. This points to sustained strength in AI infrastructure spending, which supports the company’s growth and is closely watched by semiconductor investors.

<details><summary>References</summary>
<ul>
<li><a href="https://ru.wikipedia.org/wiki/TSMC">TSMC — Википедия</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lFNU5MakVSRUhyQkh1dHBfZkJDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Strong AI demand drives TSMC sales up 45 % in July ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lFNU5MakVSRUhyQkh1dHBfZkJDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Strong AI demand drives TSMC sales up 45% in July ...</a></li>
<li><a href="https://www.osoulmisrmagazine.com/445176">World&#x27;s biggest chipmaker TSMC &#x27;s sales surge 45% amid buoyant AI...</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductor`, `#revenue`, `#stock market`, `#Taiwan`

---

<a id="item-finance-news-14"></a>
### [Report: Microsoft to Raise Windows Preinstall Licensing Fees 7–10% in July 2026](https://www.techspot.com/news/113430-microsoft-raises-windows-oem-fees-pc-makers-7.html) ⭐️ 7.0/10

According to a TechSpot report, Microsoft plans to raise the per-device licensing fees PC makers pay to preinstall Windows by 7% to 10% starting July 2026, a steeper increase than past single-digit percentage hikes. Microsoft has not confirmed the change, and retail Windows 11 prices are reported to stay unchanged.

telegram · zaihuapd · Aug 12, 02:32

**「Background」** PC makers pay these Windows OEM license fees at rates that vary by vendor and product line. The reported increase would add cost pressure as some $600–$800 PCs are already nearing $1,000 because of higher memory component prices.

**Tags**: `#Microsoft`, `#Windows OEM`, `#licensing fees`, `#PC market`, `#price increase`

---