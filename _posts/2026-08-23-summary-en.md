---
layout: default
title: "Horizon Summary: 2026-08-23 (EN)"
date: 2026-08-23
lang: en
---

> From 153 items, 21 important content pieces were selected

---

**Technology News**
1. [SGLang v0.5.18 adds models, faster startup and decode](#item-tech-news-1) ⭐️ 8.0/10
2. [MCP Roadmap Focuses on Agent Auth and HTTP Simplicity](#item-tech-news-2) ⭐️ 8.0/10
3. [Evaluation Resolution Flips Which Learning Rule Looks Brain-Like at V1](#item-tech-news-3) ⭐️ 8.0/10
4. [Open Models Halve Catch-Up Time Each Generation, SemiAnalysis Finds](#item-tech-news-4) ⭐️ 8.0/10
5. [US Advocacy Groups Urge FTC to Investigate AI Firms Over Book Destruction](#item-tech-news-5) ⭐️ 8.0/10
6. [Munder Difflin: Local Agent Harness for Deterministic Multi-Agent Office Workflows](#item-tech-news-6) ⭐️ 7.0/10
7. [Developer Trains 250M LLM, Quantizes Under 2 Bits for 60 MB Deployment](#item-tech-news-7) ⭐️ 7.0/10
8. [Open-source DelveRL roguelike built for training RL agents](#item-tech-news-8) ⭐️ 7.0/10
9. [RTX 5090 runs Qwen3.8-27B NVFP4 at real 262K context in vLLM](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Fed holds interest rates for fifth straight meeting](#item-finance-news-1) ⭐️ 9.0/10
2. [Rhine Low Water Still Chokes Europe’s River Trade, Cushioned Only by Weak Demand](#item-finance-news-2) ⭐️ 8.0/10
3. [Gas Turbine Backlogs to 2031 Emerge as Key Constraint on AI Data Centers](#item-finance-news-3) ⭐️ 8.0/10
4. [US Clean Energy Spending on Track for Record $180 Billion in 2026](#item-finance-news-4) ⭐️ 8.0/10
5. [Alphabet and Amazon Plan $420B AI Infrastructure Investment](#item-finance-news-5) ⭐️ 8.0/10
6. [Apple Announces Largest-Ever Stock Buyback Under Tim Cook](#item-finance-news-6) ⭐️ 8.0/10
7. [Five oil chokepoints beyond Hormuz now under strain](#item-finance-news-7) ⭐️ 7.0/10
8. [IEA: Southeast Asia Must Nearly Quadruple Grid Investment by 2050](#item-finance-news-8) ⭐️ 7.0/10
9. [Ross Stores&\#x27; Comparable Sales Jump 10% While TJX Rose 4%](#item-finance-news-9) ⭐️ 7.0/10
10. [Berkshire Hathaway makes $1.6 billion move on major bank](#item-finance-news-10) ⭐️ 7.0/10
11. [Dow Jones Futures Rebound Ahead of Nvidia Earnings and Canada Tariffs](#item-finance-news-11) ⭐️ 7.0/10
12. [Treasury Buyback Surprise: Bond Market Analysis](#item-finance-news-12) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SGLang v0.5.18 adds models, faster startup and decode](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 is a major release with 710 merged PRs from 212 contributors. It adds support for Muse Glimmer, Intern-S2-Mobius, SANA-Video, LingBot-Video-MoE, LTX-2.5, Cosmos3 Edge &amp; Distilled, and LongCat-Image, plus cookbook recipes for Qwen3.8, Ling-3.0, Nemotron 3.5 Lightning, Dots3-Note, and DeepSeek-V4-Pro-0813. Performance optimizations include overlapped checkpoint staging that starts Qwen3-32B on H100 up to 2.38x faster than the default \(35.6s vs 84.8s\), a TP LMHead all-to-all that cuts DeepSeek-V4-Pro B200 decode LMHead time from 320us to 169us, and FlashInfer MNNVL pure allreduce gains up to +6.9% on Blackwell at small batches. The release also moves all compiled-kernel caches under SGLANG\_CACHE\_DIR, so the first launch after upgrading recompiles once, and updates dependencies to torch 2.13.0, triton 3.7.1, flashinfer 0.6.17, and sgl-kernel 0.4.6.post1.

github · Fridge003 · Aug 22, 00:09

**「Background」** SGLang is an open-source serving framework for large language and multimodal models, designed for low-latency, high-throughput inference from a single GPU to large distributed clusters. It originated from research affiliated with LMSYS and other institutions, combining structured generation and runtime optimizations. This release continues that trajectory by integrating new autoregressive and diffusion models and adding performance improvements for startup, decoding, and kernel caching.

**「Impact」** Users can expect faster startup and decode on supported H100/Blackwell configurations and new model coverage, but should plan for a one-time recompile after installing v0.5.18.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SGLang">SGLang - Wikipedia</a></li>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/sglang: SGLang is a high-performance serving ...</a></li>

</ul>
</details>

**Tags**: `#SGLang`, `#LLM inference`, `#model support`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [MCP Roadmap Focuses on Agent Auth and HTTP Simplicity](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

The Model Context Protocol \(MCP\) project published a roadmap that prioritizes standardized authorization for agent identities, improvements for cloud workloads acting on behalf of users, and simplification of the protocol to align with ordinary HTTP workloads. The roadmap reflects a shift from the initial browser-based approval model toward recognizing delegated authority for agents and sub-agents that run without a present user. It also signals that remote MCP servers are being positioned as no different from any other HTTP workload rather than relying on a bespoke transport standard. These changes matter for developers building AI agents and MCP-compatible servers, since near-term releases will likely alter how servers authenticate callers and how clients communicate.

hackernews · pentagrama · Aug 22, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49399591)

**「Background」** The Model Context Protocol \(MCP\) is an open standard that lets AI clients connect to external tools and data through a common interface. The new roadmap focuses on replacing person-in-the-browser authorization with standardized agent identity, finalizing DPoP \(Demonstrating Proof of Possession\), and aligning MCP with HTTP by removing protocol-level session tracking. A 2026-07-28 revision makes remote MCP servers stateless at the protocol layer and effectively like other HTTP workloads, while authorization follows OAuth 2.1 conventions.

**「Impact」** Developers building agent-based tools and MCP servers will need to plan for new standardized agent identity and authorization flows, and may need to adapt clients as the protocol converges on plain HTTP behavior.

**「Community Discussion」** Commenters were divided: one praised MCP for dropping a bespoke transport in favor of standard HTTP, while others questioned whether many servers will actually implement the auth changes, argued that REST endpoints plus a skills.md file are simpler, and expressed frustration over repeated pivots. At least one commenter underscored lingering skepticism by translating &quot;MCP&quot; as &quot;Master Control Program.&quot;

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://blog.modelcontextprotocol.io/posts/mcp-roadmap/">The New MCP Roadmap | Model Context Protocol Blog</a></li>

</ul>
</details>

**Tags**: `#mcp`, `#protocols`, `#ai-agents`, `#developer-tools`, `#api-evolution`

---

<a id="item-tech-news-3"></a>
### [Evaluation Resolution Flips Which Learning Rule Looks Brain-Like at V1](https://www.reddit.com/r/MachineLearning/comments/1vvdxwt/the_evaluation_resolution_has_been_shown_to_have/) ⭐️ 8.0/10

A new preprint argues that the widely cited result of untrained convolutional neural networks matching or surpassing backpropagation-trained CNNs at the early visual cortex \(V1\) in representational similarity analysis is largely an artifact of evaluation resolution. Using a small CNN trained on a CIFAR-10 subset at 32px, five learning rules \(random init, backprop, feedback alignment, predictive coding, STDP\), and THINGS-fMRI stimuli evaluated at six resolutions from 32px to 224px, the study finds that the V1 gap between trained and untrained backprop networks is non-monotonic, shifting from -0.001±0.007 at 32 pixels to +0.044±0.006 at 224 pixels across five seeds. The authors rule out train/eval resolution matching, low-level Gabor/pixel structure, uncalibrated batch-norm, and convergence to global brightness, and a content-vs-pooling control indicates the resolution effect depends primarily on image content rather than pooled positions. Notably, the backprop &gt; untrained effect at the lateral occipital complex \(LOC\) persisted at every tested resolution. The preprint also notes that this work uncovered a batch-norm evaluation-mode bug in three earlier preprints, now corrected, and the code is openly available.

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · Aug 22, 14:30

**「Background」** Model-brain comparisons often use Representational Similarity Analysis \(RSA\) to measure how closely a neural network&\#x27;s internal representations align with human fMRI responses, particularly in the early visual cortex \(V1\). A prior preprint reported that untrained convolutional neural networks achieve V1 alignment indistinguishable from backpropagation-trained networks, suggesting that random initializations already contain non-trivial visual structure. The new study systematically re-examines this claim by varying the evaluation image resolution across multiple learning rules, testing whether the apparent untrained-network match is an artifact of the chosen evaluation conditions.

**「Impact」** Researchers performing model-brain comparisons with RSA should treat resolution as a critical methodological variable and verify results across multiple evaluation resolutions before claiming that untrained networks rival trained ones at V1.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.16875v1">Untrained CNNs Match Backpropagation at V1: A Systematic RSA Comparison of Four Learning Rules Against Human fMRI</a></li>
<li><a href="https://arxiv.org/abs/2604.16875">[2604.16875] Untrained CNNs Match Backpropagation at V1: A Systematic RSA Comparison of Four Learning Rules Against Human fMRI</a></li>

</ul>
</details>

**Tags**: `#computational neuroscience`, `#convolutional neural networks`, `#learning rules`, `#evaluation methodology`, `#brain-like models`

---

<a id="item-tech-news-4"></a>
### [Open Models Halve Catch-Up Time Each Generation, SemiAnalysis Finds](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis measures that open-source model catch-up time is halving per generation, dividing LLM history into three eras: early scaling, reasoning, and agentic. In the current agent era, Kimi K2.6 surpassed Opus 4.5 in 4.8 months, and GLM-5.2 surpassed GPT-5.2 in 6 months. The analysis warns that open models such as GLM 5.3 and Kimi K3 can now handle coding and agent tasks that it says once underpinned Anthropic&\#x27;s reported annualized revenue of over $65 billion, raising concerns about model-layer commoditization. However, benchmarks are not everything; the analysis notes Anthropic&\#x27;s productization capabilities still provide a competitive advantage.

telegram · zaihuapd · Aug 22, 08:26

**「Background」** SemiAnalysis, a technology research firm, divides large language model history into three eras—early scaling, reasoning, and the current agent era—and measures how long open-weight models take to match closed frontier models. According to its analysis, this catch-up time is halving with each generation: Kimi K2.6 surpassed Opus 4.5 in 4.8 months, and GLM-5.2 cleared GPT-5.2 in 6 months. This context explains why recent open-weight models, such as those mentioned in the analysis, are increasingly seen as commoditizing model-layer capabilities once dominated by proprietary systems.

**「Impact」** The SemiAnalysis findings imply that open-source models \(e.g., Kimi K2.6, GLM-5.2\) have caught up to closed frontier models in agentic tasks within as little as 4.8–6 months, accelerating commoditization of the model layer and undercutting the pricing advantage of proprietary API providers; Anthropic&\#x27;s counterweight is productization, as reflected in its open-sourced Model Context Protocol.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/are-open-models-catching-up">Are Open Models Catching Up?</a></li>
<li><a href="https://www.linkedin.com/pulse/standardizing-commoditization-anthropics-model-context-sam-bobo-n8tse">Standardizing for Commoditization — Anthropic ’s Model Context...</a></li>

</ul>
</details>

**Tags**: `#open-source AI`, `#large language models`, `#AI industry analysis`, `#model commoditization`, `#SemiAnalysis`

---

<a id="item-tech-news-5"></a>
### [US Advocacy Groups Urge FTC to Investigate AI Firms Over Book Destruction](https://www.axios.com/2026/08/21/ftc-ai-companies-book-destruction-investigate) ⭐️ 8.0/10

On August 21, a coalition of more than a dozen U.S. advocacy groups, including the Demand Progress Education Fund and the Consumer Federation of America, urged the Federal Trade Commission \(FTC\) to investigate AI companies that buy, scan, and destroy physical books for AI training. The letter argues that this &quot;hoard and destroy&quot; practice may constitute an unfair method of competition under Section 5 of the Federal Trade Commission Act, because it removes scarce materials from the market and could make some rare volumes permanently unavailable. It cites Anthropic as spending millions of dollars to buy books, cut off the spines, and feed the scanned pages to Claude, and notes that Google, Microsoft, and OpenAI face similar copyright litigation. The groups say the practice raises rivals&\#x27; costs and builds a moat, while stopping short of opposing AI training generally. If the FTC takes up the matter, the battle over AI training data would extend from copyright law into competition regulation.

telegram · zaihuapd · Aug 22, 15:40

**「Background」** AI companies have increasingly sought copyrighted books as training data, often preferring physical copies when digital collections are not licensed or otherwise available. Some firms have purchased books and destroyed them after scanning, which critics say prevents the same copies from being reused or resold and can remove rare works from public availability. The letter follows existing copyright lawsuits against leading AI companies over their use of books to train models.

**「Impact」** The letter creates a concrete signal that AI training-data practices may face scrutiny under U.S. competition law, adding potential regulatory exposure for Anthropic, Google, Microsoft, and OpenAI beyond their pending copyright disputes.

**Tags**: `#AI regulation`, `#FTC`, `#competition policy`, `#copyright`, `#AI training data`

---

<a id="item-tech-news-6"></a>
### [Munder Difflin: Local Agent Harness for Deterministic Multi-Agent Office Workflows](https://munderdiffl.in/) ⭐️ 7.0/10

Munder Difflin is a local multi-agent harness that runs an office of simulated clones on top of existing coding agents such as Claude Code and Codex, with support for most major coding-agent harnesses. Its simulations are deterministic and do not consume tokens, and early users report reduced token consumption; the project reports 20K+ users within a week. The tool aims to enable deterministic multi-agent workflows while reusing existing subscriptions, but it is a niche developer tool rather than a major breakthrough.

hackernews · simonpure · Aug 22, 09:49 · [Discussion](https://news.ycombinator.com/item?id=49398152)

**「Background」** A multi-agent harness coordinates several AI coding agents into one team, differing from a single agent or a framework by managing orchestration and communication. Munder Difflin is an open-source local harness by Chaitanya Giri that wraps existing CLI coding agents, such as Claude Code and Codex, to run deterministic simulations that do not consume tokens, aiming to reduce overall token usage.

**「Impact」** For developers already paying for Claude Code or Codex, Munder Difflin offers a local way to run deterministic multi-agent simulations without additional token costs, potentially making multi-agent workflows more practical and cheaper.

**「Community Discussion」** Commenters were split: some praised The Office theme for capturing the dysfunction of agent swarms, while a long-running user critique called it pipelines and roles rather than true agents, wanting more explicit pipeline stages like plan, approval gate, develop, and code review. The builder answered questions, emphasizing deterministic simulations and token savings.

<details><summary>References</summary>
<ul>
<li><a href="https://munderdiffl.in/blog/what-is-a-multi-agent-harness/">What Is a Multi- Agent Harness ? (Plain-English... — Munder Difflin Blog</a></li>
<li><a href="https://www.stork.ai/en/munder-difflin">Munder Difflin Review (2026) | Stork.AI</a></li>
<li><a href="https://www.aitoolnet.com/munder-difflin">Munder Difflin - Clones for you and your team, working 24/7 - Aitoolnet</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#multi-agent`, `#developer-tools`, `#llm`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [Developer Trains 250M LLM, Quantizes Under 2 Bits for 60 MB Deployment](https://www.reddit.com/r/MachineLearning/comments/1vv2nkh/i_developed_my_own_quantized_llm_from_scratch/) ⭐️ 7.0/10

A developer trained SHADOW-250M, a 250M-parameter LLM from scratch on 30B tokens of FineWeb, then quantized it to under 2 bits per weight so the full deployment is 60 MB and runs at about 400 tokens/s on a normal laptop CPU with roughly 80 MB RAM and no GPU. The model keeps the most recent 2048 tokens in FP16 as a normal KV cache and compresses older tokens to about 1 bit for an external disk cache, allowing retrieval \(but not reasoning\) over up to 100M tokens; 1M tokens occupy about 320 MB on disk. Instead of a trained embedding table, it maps tokens to fixed 512-bit codes \(8.4 MB for 131k tokens, zero trained parameters\), achieving 0.619 Spearman correlation on WordSim-353 versus 0.029 for random codes. On held-out English web text it reports cross entropy 3.15 nats/token, perplexity 23.3, and 0.99 bits per byte, with reproducible sample outputs in the repository. The author frames it as a demonstration of extreme quantization and efficient edge deployment, not a competitor to large models.

reddit · r/MachineLearning · /u/Final-Data-1410 · Aug 22, 04:39

**「Background」** Large language models are typically measured in billions of parameters and require GPUs to run quickly, but quantization compresses weights so models run on less powerful hardware. KV caches store previous tokens for attention, but their memory grows with context length; this project combines aggressive weight quantization with a disk-backed cache that exceeds normal context windows.

**「Impact」** For developers deploying LLMs on low-resource edge devices, this shows a feasible 60 MB model with 400 tok/s CPU inference and a disk-based long-context retrieval mechanism that can reach 100M tokens, though the model explicitly cannot reason over that retrieved history. Users should expect mistakes on open facts since it is only a 250M model.

**Tags**: `#quantization`, `#efficient inference`, `#long context`, `#edge AI`, `#from-scratch training`

---

<a id="item-tech-news-8"></a>
### [Open-source DelveRL roguelike built for training RL agents](https://www.reddit.com/r/MachineLearning/comments/1vvii1j/i_built_an_opensource_roguelike_specifically_for/) ⭐️ 7.0/10

DelveRL is a new open-source, human-playable roguelike designed specifically for training game-playing agents. It provides a structured API, deterministic simulation, procedural levels, partial observability, and strategic depth for exploration, resource management, and combat. The project includes batched renderer-free environments that run locally and a recurrent PPO trainer, with a baseline agent reaching a median floor of 18 and extended runs reaching floor 33. The game, training code, checkpoint, bridge documentation, and raw benchmarks are all open source. This addresses the common difficulty of integrating commercial games with agent harnesses, offering a purpose-built environment inspired by DeepMind and OpenAI projects.

reddit · r/MachineLearning · /u/SnyderConsulting · Aug 22, 17:32

**「Background」** Reinforcement learning \(RL\) trains agents by interacting with an environment, and standard APIs like OpenAI Gym define observation and action spaces to make that interaction reproducible. Researchers often build custom environments for specific challenges, and the roguelike genre—turn-based games with procedurally generated maps, resource management, and permanent death—offers a testbed for partial observability and long-term planning. DelveRL is one such custom environment, developed with a structured API and deterministic simulation to simplify training game-playing agents.

**「Impact」** Researchers and reinforcement learning developers can use DelveRL to benchmark agents in a lightweight, fully local procedural environment with a built-in PPO baseline and complete open resources, lowering the barrier to reproducible game-agent training experiments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=bD6V3rcr_54">Building a Custom Environment for Deep Reinforcement Learning ...</a></li>
<li><a href="https://openai.com/index/openai-gym-beta/">OpenAI Gym Beta | OpenAI</a></li>
<li><a href="https://github.com/topics/openai-gym-environments?l=python">openai -gym- environments · GitHub Topics · GitHub</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#roguelike`, `#open source`, `#game environments`, `#PPO`

---

<a id="item-tech-news-9"></a>
### [RTX 5090 runs Qwen3.8-27B NVFP4 at real 262K context in vLLM](https://www.reddit.com/r/LocalLLaMA/comments/1vvl7pc/single_rtx_5090_qwen3827b_nvfp4_at_a_real_262k/) ⭐️ 7.0/10

A Reddit user documented a reproducible vLLM setup that runs the 27B Qwen3.8-27B NVFP4 ModelOpt checkpoint \(joshebbs/qwen3.8-27b-uncensored-nvfp4-modelopt, revision e5ff4986938dcd0dd05ab4cce89da1b052be6ce3, 19.18 GiB\) on a single 32 GB RTX 5090 with a real 262,144-token context window alongside vision, FP8 KV, prefix caching, tool calling, and a KDE desktop. The hybrid 64-layer model \(48 Gated DeltaNet, 16 full-attention layers\) achieves 77.2 tok/s short-context decode after a 1K prompt and 64.7 tok/s with 128K resident tokens, while a 262,000-token prefill completed in 166 seconds. Prefix caching delivered a 22.3x cold-to-cached TTFT speedup in a fresh 36,864-token shared-prefix test, though vLLM places hybrid cache in experimental align mode when prefix caching is enabled and corrupted output should first be checked by disabling it. The measured VRAM budget shows 29,322 MiB for the vLLM EngineCore process and only about 1.6-1.8 GiB free on the card, so the fit is real but not headroom-heavy; runtime also pins the KV pool via --kv-cache-memory-bytes so --gpu-memory-utilization acts only as an admission gate. Exact versions include vLLM 0.27.1, PyTorch 2.13.0+cu130, driver 610.57.04, and CUDA 13.3.1 on Arch Linux.

reddit · r/LocalLLaMA · /u/Fz1zz · Aug 22, 19:16

**「Background」** Qwen3.8-27B is a 27B-parameter multimodal hybrid-attention model: 48 of its 64 layers use linear Gated DeltaNet attention and the remaining 16 use full attention, with a native 262K-token context window and a vision tower \(tool-1-1\). NVFP4 is a 4-bit floating-point quantization scheme from NVIDIA ModelOpt that shrinks such a model to about 19 GiB of safetensors while retaining the vision and MTP-draft components. vLLM must therefore combine quantized weights, hybrid-attention cache handling, prefix caching, and GPU memory pinning to fit a full 262K-window context on a 32GB-class Blackwell GPU like the RTX 5090.

**「Impact」** For RTX 5090 owners, this gives a tested reference point for running a 27B hybrid-attention model with genuine 262K context, showing about 64.7 tok/s at 128K resident context and only about 1.6 GB free VRAM, with the caveat that prefix caching may need to be disabled if output corruption appears.

<details><summary>References</summary>
<ul>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-27B">Qwen/ Qwen 3 . 8 - 27 B | vLLM Recipes</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#Qwen`, `#NVFP4`, `#RTX 5090`, `#long context`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed holds interest rates for fifth straight meeting](https://news.google.com/rss/articles/CBMinwFBVV95cUxNbVA1MzJGNXllN1RjSG43b0xUam1seWRjUmI2bHdXdlZndHhEQ1pRZDI5WVE3MGg1NnBCMk9Gcm42MUZab29ZRFY3OTd3OTZERlZmLUtFbGhUOG5jQXlDREFuMGVkSmtyTlJvVzJhS1A0OG5zaGhWZkZ1VHlQRXNGcGcxczNOMW82ckdRdVJmRUZzRDI4OEV4SHRfSjh6Wms?oc=5) ⭐️ 9.0/10

The Federal Reserve kept its benchmark interest rate unchanged for a fifth consecutive meeting, underscoring persistent inflation concerns.

google\_news · NBC News · Jul 29, 07:00

**「Background」** The Federal Reserve&\#x27;s rate-setting committee, the FOMC, uses its benchmark federal funds rate as a guide for borrowing costs across the economy; after five straight meetings of holding that rate at 3.50%-3.75%, Chair Kevin Warsh and colleagues are waiting for clearer inflation and economic trends before changing course.

<details><summary>References</summary>
<ul>
<li><a href="https://www.livemint.com/market/stock-market-news/us-federal-reserve-holds-rates-steady-for-fifth-consecutive-meeting-11785346712831.html">US Federal Reserve holds rates steady for fifth consecutive meeting</a></li>
<li><a href="https://www.advisorperspectives.com/dshort/updates/2026/07/29/feds-interest-rate-decision-july-29-2026">Fed&#x27;s Interest Rate Decision: July 29, 2026 - dshort - Advisor Perspectives</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#economy`

---

<a id="item-finance-news-2"></a>
### [Rhine Low Water Still Chokes Europe’s River Trade, Cushioned Only by Weak Demand](https://oilprice.com/Energy/Energy-General/Europe-Dodges-a-Rhine-Crisis-for-the-Worst-Possible-Reason.html) ⭐️ 8.0/10

The Rhine has recovered slightly from its mid-August record low, but barges still cannot carry normal loads through the critical Kaub chokepoint, and Europe is avoiding a deeper disruption only because factories and consumers are demanding less. Freight on the ARA-Karlsruhe route has risen about five-fold to €215/t from roughly €45/t at the end of June, according to the analysis.

rss · OilPrice.com · Aug 22, 23:00

**「Background」** Kaub&\#x27;s navigable water depth fell below 10 cm in mid-August, making the waterway only about 1.2 meters deep versus roughly 2.3 meters a year ago, and has since recovered to about 45 cm—still below the 77-cm benchmark for normal commercial traffic.

**「Impact」** The restricted river capacity is hitting chemical and fuel transport, with examples including LyondellBasell&\#x27;s force majeure at its Wesseling butadiene unit and localised gasoline shortages in eastern France; if industrial demand recovers, low-water levels would be far harder to absorb.

**Tags**: `#Rhine river`, `#European chemicals`, `#supply chain`, `#transport disruption`, `#energy`

---

<a id="item-finance-news-3"></a>
### [Gas Turbine Backlogs to 2031 Emerge as Key Constraint on AI Data Centers](https://oilprice.com/Energy/Energy-General/The-Gas-Turbine-Shortage-Just-Became-AIs-Biggest-Constraint.html) ⭐️ 8.0/10

GE Vernova is taking reservations for new heavy-duty gas turbines with 2031 delivery, underscoring how turbine supply has become a constraint on AI data center power plans. Goldman Sachs forecasts U.S. data center power demand will grow from 31 GW in 2025 to 66 GW in 2027.

rss · OilPrice.com · Aug 22, 21:00

**「Background」** Turbine makers are reluctant to expand capacity after the previous gas boom ended in cancellations and layoffs, so they now sell paid slot reservations that let customers shoulder the risk if projects are canceled.

**「Impact」** The gap is already visible in PJM’s capacity auction for 2028/2029, which cleared at the maximum allowed price and still fell about 6,831 MW short of the reliability requirement, with only 525 MW of new supply clearing.

**Tags**: `#gas turbines`, `#data centers`, `#energy demand`, `#supply chain`, `#AI infrastructure`

---

<a id="item-finance-news-4"></a>
### [US Clean Energy Spending on Track for Record $180 Billion in 2026](https://oilprice.com/Energy/Energy-General/Clean-Energy-Spending-Tracking-Toward-Record-180-Billion-in-2026.html) ⭐️ 8.0/10

US clean energy capital expenditures hit $74 billion in the first half of 2026 and are projected to reach a record $180 billion for the full year, according to fintech firm Crux.

rss · OilPrice.com · Aug 22, 19:00

**「Background」** The surge follows federal rollbacks of earlier clean-energy incentives; Crux’s CEO and energy executives point to AI-driven electricity demand and fossil-fuel market volatility as key drivers.

**「Impact」** Grid-level battery storage is expanding with the buildout: utility-scale capacity reached 52 gigawatts, 8.3 gigawatts were added in the first half of 2026, and grid operators have plans to add 54 gigawatts more by the end of 2028.

**Tags**: `#clean energy`, `#investment`, `#battery storage`, `#energy grid`, `#policy`

---

<a id="item-finance-news-5"></a>
### [Alphabet and Amazon Plan $420B AI Infrastructure Investment](https://finance.yahoo.com/technology/ai/articles/alphabet-amazon-investing-420-billion-103500198.html) ⭐️ 8.0/10

Alphabet and Amazon plan to invest $420 billion in AI infrastructure, a capital-expenditure commitment that could increase demand for hardware suppliers.

openbb · NVDA · Aug 22, 10:35

**「Background」** Alphabet and Amazon have announced large AI infrastructure spending plans for 2026, with Alphabet expecting to spend between $195 billion and $205 billion and Amazon expecting around $220 billion. This capital expenditure is directed at hardware suppliers such as Nvidia, Broadcom, and Micron.

**「Impact」** Hardware companies that make data-center chips, servers, and networking gear are the most directly affected, because the planned spending is meant to build the physical infrastructure for AI services.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/alphabet-amazon-investing-420-billion-103500198.html">Alphabet and Amazon Are Investing $ 420 Billion in Artificial...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#capital expenditure`, `#Alphabet`, `#Amazon`, `#hardware stocks`

---

<a id="item-finance-news-6"></a>
### [Apple Announces Largest-Ever Stock Buyback Under Tim Cook](https://finance.yahoo.com/markets/stocks/articles/apple-announced-largest-ever-stock-222000154.html) ⭐️ 8.0/10

Apple announced its largest-ever stock buyback under CEO Tim Cook, a significant capital return move affecting shareholders. No specific buyback amount was provided in the available source.

openbb · NVDA · Aug 22, 22:20

**「Background」** On May 2, 2024, Apple&\#x27;s board authorized a $110 billion stock buyback, the largest repurchase program in the company&\#x27;s history, alongside its fiscal second-quarter earnings report. The company also raised its quarterly dividend from 24 cents to 25 cents per share, continuing its practice of returning cash to shareholders by buying back its own stock, which increases the ownership stake of existing investors.

**「Impact」** Apple&\#x27;s record buyback reduces the number of shares outstanding, which can raise earnings per share for existing shareholders.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/apple-record-110-billion-stock-buyback/">Apple announces largest-ever stock buyback at $110 billion under Tim Cook</a></li>
<li><a href="https://ca.news.yahoo.com/live-updates-apple-report-quarterly-140852867.html">Apple earnings results: Tim Cook announces biggest-ever stock buyback ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#stock buyback`, `#capital return`, `#shareholder returns`, `#corporate action`

---

<a id="item-finance-news-7"></a>
### [Five oil chokepoints beyond Hormuz now under strain](https://oilprice.com/Energy/Energy-General/Every-Chokepoint-That-Isnt-Hormuz.html) ⭐️ 7.0/10

An analysis of oil logistics examines five chokepoints beyond Hormuz and identifies the Red Sea&\#x27;s Bab el-Mandeb as already disrupting traffic. Traceable transits through the strait fell to 200 in the week of Aug. 3, the lowest in a year, after the Houthis declared a maritime blockade of Saudi Arabia on July 20.

rss · OilPrice.com · Aug 22, 17:00

**「Background」** Hormuz has been effectively closed since late February, when the war between Iran and the U.S. and Israel started; the U.S. Energy Information Administration estimates only 4.9 million barrels a day of crude and liquids made it through in the second quarter, down from 21.6 million in the last quarter of 2025.

**「Impact」** The detours are raising costs for oil shippers and already disrupting Black Sea exports; Ukrainian drone strikes have idled a Russian terminal that had been moving about 650,000 barrels a day.

**Tags**: `#oil logistics`, `#chokepoints`, `#Bab el-Mandeb`, `#Houthi blockade`, `#energy markets`

---

<a id="item-finance-news-8"></a>
### [IEA: Southeast Asia Must Nearly Quadruple Grid Investment by 2050](https://oilprice.com/Energy/Energy-General/IEA-Southeast-Asia-Needs-Grid-Investment-to-Nearly-Quadruple-by-2050.html) ⭐️ 7.0/10

The International Energy Agency \(IEA\) says Southeast Asia must raise annual investment in electricity grids and storage from $13 billion today to $50 billion by 2050 to meet its clean-energy targets, with transmission and distribution lines needing to more than double in length by then.

rss · OilPrice.com · Aug 22, 15:00

**「Background」** Southeast Asia is projected to account for almost 20% of global energy demand growth to 2035, and its renewable capacity could almost triple by 2035 under current policies or grow fivefold if announced targets are met. Grid investment has lagged behind renewable additions, creating bottlenecks in power distribution.

**「Impact」** Without greater investment, grid constraints can force renewable curtailment and deter investment, as seen in Vietnam cutting solar and wind output and India reporting transmission-related renewable curtailment.

**Tags**: `#IEA`, `#Southeast Asia`, `#grid investment`, `#renewable energy`, `#energy transition`

---

<a id="item-finance-news-9"></a>
### [Ross Stores&\#x27; Comparable Sales Jump 10% While TJX Rose 4%](https://finance.yahoo.com/markets/stocks/articles/ross-stores-grew-comparable-sales-204301377.html) ⭐️ 7.0/10

Off-price retailers Ross Stores and TJX reported comparable-sales growth, with Ross up 10% versus TJX&\#x27;s 4%, yet only one of the two companies&\#x27; stocks rose. The contrasting stock moves highlight divergent market reactions despite Ross&\#x27;s faster sales growth.

openbb · NVDA · Aug 22, 20:43

**「Background」** Ross Stores and TJX are off-price retailers that sell brand-name goods at discounted prices; Ross has guided for 6%–7% comparable sales growth next quarter, while TJX guided for 2%–3%.

**「Impact」** Off-price retail investors saw the consequences immediately: Ross Stores shares jumped roughly 8% after the company guided to 6-7% comparable-sales growth next quarter, while TJX shares rose only about 1% to $141.45 after it guided to 2-3% with its flagship division near flat.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/22/ross-stores-grew-comparable-sales-10-tjx-grew-4-only-one-stock-went-up/">Ross Stores Grew Comparable Sales 10%. TJX Grew 4%. Only One Stock Went Up. | The Motley Fool</a></li>
<li><a href="https://www.fool.com/investing/2026/08/22/ross-stores-grew-comparable-sales-10-tjx-grew-4-only-one-stock-went-up/">Ross Stores Grew Comparable Sales 10%. TJX Grew 4%. Only One Stock Went Up. | The Motley Fool</a></li>
<li><a href="https://247wallst.com/investing/2026/08/21/ross-jumps-8-on-10-comp-growth-tjx-ticks-up-macys-edges-higher/">Ross Jumps 8% on 10% Comp Growth, TJX Ticks Up, Macy&#x27;s Edges Higher - 24/7 Wall St.</a></li>

</ul>
</details>

**Tags**: `#retail`, `#comparable sales`, `#earnings`, `#consumer discretionary`, `#Ross Stores`, `#TJX`

---

<a id="item-finance-news-10"></a>
### [Berkshire Hathaway makes $1.6 billion move on major bank](https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-berkshire-makes-1-000300036.html) ⭐️ 7.0/10

Warren Buffett&\#x27;s Berkshire Hathaway made a $1.6 billion investment move involving a major bank, according to a report; the specific bank and whether it was a purchase or sale were not disclosed.

openbb · BRK-B · Aug 22, 00:03

**「Background」** Berkshire Hathaway is Warren Buffett&\#x27;s conglomerate, and its quarterly 13F filing—a public list of large U.S. stock holdings—is closely watched. The latest filing reportedly shows Berkshire reduced its long-held Bank of America stake.

**「Impact」** Investors who follow Berkshire Hathaway’s quarterly 13F filings could see the $1.6 billion reduction in its Bank of America stake as caution on large consumer banks, though Berkshire kept its American Express position unchanged.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-berkshire-makes-1-000300036.html">Warren Buffett&#x27;s Berkshire makes $1.6 billion move on major bank</a></li>
<li><a href="https://www.fool.com/investing/2026/08/21/warren-buffett-successor-greg-abel-cut-berkshire-s-bank-of-america-stake-by-usd1-7-billion-he-added-usd1-6-billion-of-delta-air-lines/">Warren Buffett Successor Greg Abel Cut Berkshire&#x27;s Bank of America Stake by $1.7 Billion. He Added $1.6 Billion of Delta Air Lines. | The Motley Fool</a></li>
<li><a href="https://www.thestreet.com/investing/stocks/bac-bank-of-america-stock-berkshire-hathaway-sells-16-billion-stake">Warren Buffett&#x27;s Berkshire makes $1.6 billion move on major bank - TheStreet</a></li>
<li><a href="https://www.nationalmortgagenews.com/news/will-berkshire-stay-in-bank-stocks-after-buffetts-exit">Will Berkshire stay in bank stocks after Buffett&#x27;s exit? | National Mortgage News</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#Warren Buffett`, `#banking`, `#investment`, `#capital allocation`

---

<a id="item-finance-news-11"></a>
### [Dow Jones Futures Rebound Ahead of Nvidia Earnings and Canada Tariffs](https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-market-rally-nvidia-crowdstrike-warsh/?src=A00220&amp;yptr=yahoo) ⭐️ 7.0/10

Dow Jones futures pointed to a market rebound as investors focused on looming Nvidia earnings and new US tariffs on Canada announced by President Trump.

openbb · GC=F · Aug 22, 15:25

**「Background」** US tariffs on goods from Mexico, Canada, and China have taken effect, prompting retaliation and market declines, and Nvidia&\#x27;s next earnings report is expected around August 26, 2026, with investors watching for guidance.

**「Market impact」** Investors trading U.S. stock index futures, especially Nasdaq contracts, saw early gains on Thursday after a federal court blocked the new tariffs and Nvidia reported strong earnings, according to Investors.com.

<details><summary>References</summary>
<ul>
<li><a href="https://news.sky.com/story/donald-trump-confirms-mexico-and-canada-tariffs-sending-financial-markets-reeling-13321044">Canadian PM criticises Trump over tariffs - and sends... | Sky News</a></li>
<li><a href="https://www.tipranks.com/stocks/nvda/earnings">Nvidia Corporation (NVDA) Earnings Dates, Call... - TipRanks.com</a></li>
<li><a href="https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-nvidia-earnings-court-blocks-trump-tariffs/">Dow Jones Futures Rise As Court Blocks Trump Tariffs ; Nvidia ...</a></li>

</ul>
</details>

**Tags**: `#market futures`, `#tariffs`, `#Nvidia`, `#trade policy`, `#stock market`

---

<a id="item-finance-news-12"></a>
### [Treasury Buyback Surprise: Bond Market Analysis](https://news.google.com/rss/articles/CBMilgFBVV95cUxPUVJ6bXhzRjhidmNacEdxUTU1dTZ1X0lCZ2VITXJsbEpnQlVMX3dBNE5VdHpTRVBvalNZLUZKZ1c3X19ySVQtQWdsOVM5TW5pdW9FejFLUC1rN1J4V1hCc0ExRnV5MndzOThHS2phSVJjM2VBSkUya0ZVbm16Q1FneHJUWEZ1a2Uxb1VFcmItYmxRMUJQUGc?oc=5) ⭐️ 7.0/10

A Council on Foreign Relations analysis discusses an unexpected U.S. Treasury buyback and what it signals for the bond market, but the available excerpt does not include specific figures or policy details.

google\_news · Council on Foreign Relations · Aug 20, 16:30

**「Background」** U.S. Treasury bond buybacks are a long-standing tool, used at home and abroad, to ensure market liquidity and manage cash flows; the surprise is that the Treasury is now acting more forcefully to manage yields.

**「Impact」** The Treasury&\#x27;s move to at least double the size of some long-bond buyback operations, to at least $4 billion, sent bond yields sliding and Bitcoin surging within hours, and it eases borrowing-cost pressures on households, companies, and the federal budget, though analysts describe the scale as a &\#x27;drop in the bucket&\#x27; relative to total debt.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cfr.org/articles/what-the-treasurys-buyback-surprise-says-about-the-bond-market">What the Treasury ’s Buyback Surprise Says About the Bond Market</a></li>
<li><a href="https://en.cryptonomist.ch/2026/08/20/treasury-bond-buyback-impact/">Treasury Bond Buyback Impact Drives Bitcoin Surge</a></li>
<li><a href="https://www.politico.com/news/2026/08/19/treasury-buy-back-debt-bond-market-pain-01041461">‘Drop in the bucket’: Why Wall Street will shrug off Bessent’s bond ...</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-19/us-treasury-to-double-sizes-of-some-debt-buyback-operations-to-at-least-4-billion">Treasury Secretary Bessent Doubles US Long- Bond Buybacks in the...</a></li>

</ul>
</details>

**Tags**: `#Treasury`, `#bond market`, `#debt management`, `#monetary policy`, `#market impact`

---