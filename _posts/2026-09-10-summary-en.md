---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 242 items, 19 important content pieces were selected

---

**Technology News**
1. [vLLM v0.29.0 makes Model Runner V2 default, adds models](#item-tech-news-1) ⭐️ 8.0/10
2. [Shopify acquires Tailwind amid AI business pressure debate](#item-tech-news-2) ⭐️ 8.0/10
3. [Analysis: GPT-6 Astra, Looped Transformers, and Hidden Reasoning](#item-tech-news-3) ⭐️ 8.0/10
4. [How I advertise malicious software on Google Ads](#item-tech-news-4) ⭐️ 8.0/10
5. [OpenAI reports sharp drop in GPT-6 Astra chain-of-thought monitorability](#item-tech-news-5) ⭐️ 8.0/10
6. [IEEE Spectrum reports growing evidence autonomous cars save lives](#item-tech-news-6) ⭐️ 7.0/10
7. [Pentagon Sought OpenAI Model With Low Military Refusal Rate, Leaks Show](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [Brent Crude Tops $100 as U.S.-Iran Fighting Disrupts Strait of Hormuz Flows](#item-finance-news-1) ⭐️ 8.0/10
2. [Negative Power Prices Spread Across Europe as Storage Lags Renewables](#item-finance-news-2) ⭐️ 8.0/10
3. [U.S. Sanctions Iran&\#x27;s Remaining Airlines in Aviation Crackdown](#item-finance-news-3) ⭐️ 8.0/10
4. [Google to Invest €13 Billion in Finnish AI Infrastructure and Signs 22-Year Nuclear Deal](#item-finance-news-4) ⭐️ 8.0/10
5. [Bank of England Warns Iran Conflict Could Push UK Inflation Above 4%](#item-finance-news-5) ⭐️ 8.0/10
6. [Copper Hits Record High as Smelter Fees Fall to Zero](#item-finance-news-6) ⭐️ 8.0/10
7. [Federal Reserve holds rates steady but leaves door open to hike](#item-finance-news-7) ⭐️ 8.0/10
8. [Adani Airport unit signs $1 billion fundraising deal; Adani Enterprises shares rise](#item-finance-news-8) ⭐️ 7.0/10
9. [China&\#x27;s EV makers turn to humanoid robots as car sales slow](#item-finance-news-9) ⭐️ 7.0/10
10. [Analysis Disputes UK Report&\#x27;s £500 Household Saving From Scrapping Net Zero](#item-finance-news-10) ⭐️ 7.0/10
11. [Belarusian Refineries Claim Decade-High Profitability as Russia&\#x27;s Fuel Crisis Drives Record Exports](#item-finance-news-11) ⭐️ 7.0/10
12. [Uganda Prepares Pearl Sweet Crude for First Exports](#item-finance-news-12) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vLLM v0.29.0 makes Model Runner V2 default, adds models](https://github.com/vllm-project/vllm/releases/tag/v0.29.0) ⭐️ 8.0/10

vLLM released v0.29.0, a release spanning 594 commits from 277 contributors, including 91 new contributors. The headline change makes Model Runner V2 the default for all models, completing a rollout that began with pooling models; MRV2 also gained CUDA graph memory profiling for KV cache auto-sizing, batch-sharded sampling that cuts per-step logits memory by 1/TP, prompt embeds, and \`extract\_hidden\_states\` speculation, while MRV1 remains in use for a few ROCm models and features MRV2 does not yet support. New model support includes Hy4-preview \(Tencent&\#x27;s 770B/49B-active MoE with Gated DeepSeek Sparse Attention and native MTP\), Qwen3.8-Flash-Next with BF16/FP8/NVFP4 and MTP, GraniteSWA and GraniteMoeSWA, NemotronH\_Omni\_Reasoning\_V3 with MTP, and Kimi K3 NVFP4 checkpoints. Performance work targets Kimi-K3 and DeepSeek V4 \(including a fused MXFP4 top-k finalization in the K3 latent tail worth about 5% E2E latency and K3 Mamba metadata preparation in one Triton launch at 6.6-7.6x kernel speedup\), alongside Mamba prefix-caching prefill checkpoints that deliver a 9%-25% TTFT improvement; new defaults enable FlashInfer all-reduce for TP CUDA groups \(opt out with \`VLLM\_ALLREDUCE\_USE\_FLASHINFER=0\`\), make prefix-cache \`NONE\_HASH\` deterministic so distributed KV cache users need not pin \`PYTHONHASHSEED\`, and add \`--max-num-queued-reqs\` / \`--max-num-queued-tokens\` admission-control flags. Breaking changes remove ten deprecated model architectures, migrate FlexOlmo, Olmo3 and Hunyuan V1/VL to the Transformers modeling backend, remove the PyAV video decoder backend, deprecate \`python -m vllm.entrypoints.openai.api\_server\` in favor of \`vllm serve\`, and drop the \`VLLM\_TEST\_FORCE\_FP8\_MARLIN\` and \`VLLM\_ROCM\_USE\_AITER\_FP4\_ASM\_GEMM\` environment variables.

github · khluu · Sep 9, 08:54

**「Background」** vLLM is an open-source, high-throughput inference and serving engine for large language models, built around techniques such as PagedAttention, continuous batching, and CUDA/HIP graph execution. Model Runner V2 \(MRV2\), announced in March 2026, is a ground-up re-implementation of vLLM&\#x27;s model runner intended to be cleaner, more modular, and faster without API changes, though the project has noted it was not yet feature-complete or rigorously tested at introduction. Its rollout began with pooling models before v0.29.0 made it the default for all models, while MRV1 remains in use for a few ROCm models and for features MRV2 does not yet support.

**「Impact」** Users upgrading to v0.29.0 must audit breaking changes — ten deprecated model architectures removed, FlexOlmo/Olmo3/Hunyuan V1/VL moved to the Transformers modeling backend, the PyAV video decoder backend removed, and the \`python -m vllm.entrypoints.openai.api\_server\` entrypoint deprecated — and should verify existing workloads against the new Model Runner V2 default, which vLLM&\#x27;s own design documentation describes as not yet feature-complete.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory ... Model Runner V2 Design Document - vLLM Model Runner V2: A Modular and Faster Core for vLLM vllm-project-vllm-inference/docs/design/model_runner_v2.md at ... V1 Engine &amp; Model Runner V2 (MRV2) | vllm-project/vllm ...</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#open source`, `#model serving`, `#performance optimization`

---

<a id="item-tech-news-2"></a>
### [Shopify acquires Tailwind amid AI business pressure debate](https://tailwindcss.com/blog/tailwind-is-joining-shopify) ⭐️ 8.0/10

Shopify has acquired Tailwind, according to the linked Tailwind blog post announcing that Tailwind is joining Shopify, as discussed on Hacker News. The deal brings the widely used open source CSS framework and its commercial ecosystem under Shopify&\#x27;s ownership, raising questions about how Tailwind&\#x27;s open source project and business model will be maintained. In the Hacker News thread \(870 points, 348 comments\), commenters cited a January GitHub pull request excerpt claiming that 75% of Tailwind Labs&\#x27; engineering team lost their jobs and that traffic to Tailwind&\#x27;s docs fell about 40% from early 2023, attributing the decline to AI&\#x27;s impact on the business; those figures are secondhand and are not verified by the supplied source content. The discussion also debated whether Tailwind remains necessary for new projects and whether open source and commercial developer-tool companies can survive as AI coding tools improve. No technical version, licensing, roadmap, or pricing details were available in the supplied item or comments.

hackernews · EdwinHoksberg · Sep 9, 13:27 · [Discussion](https://news.ycombinator.com/item?id=49626190)

**「Background」** Tailwind CSS is an open-source, utility-first CSS framework developed by Tailwind Labs that is used to style modern websites directly within HTML. Shopify, the Ottawa-based commerce company, has acquired Tailwind Labs, the Canadian company behind Tailwind CSS, in a deal reported to secure the framework’s future under the MIT license. The acquisition was announced by Tailwind on Wednesday via X and a blog post.

**「Impact」** For developers and organizations relying on Tailwind CSS, the acquisition places the framework under Shopify and, according to external reports, keeps the project alive after Tailwind Labs lost 75% of its engineering team and 80% of revenue, while confirming that the commercial ecosystem around the open-source tool has been severely eroded. Those revenue and layoff figures come from external reports and secondhand excerpts rather than an official statement in the supplied material.

**「Community discussion」** Commenters disagreed about whether new sites still need Tailwind, with one asking whether modern vanilla CSS plus AI-assisted editing could avoid dependency and build-pipeline complexity, while others valued Tailwind&\#x27;s role in learning CSS, HTML, and design. Several commenters framed the acquisition as Shopify buying Tailwind&\#x27;s people and brand, and expressed concern that open source and commercial dev-tool businesses are increasingly hard to sustain when LLMs can help reproduce the commercial layer; the cited layoffs and docs-traffic decline were offered as evidence for that pressure.

<details><summary>References</summary>
<ul>
<li><a href="https://seekingalpha.com/news/4641301-shopify-acquires-tailwind-labs">Shopify acquires Tailwind Labs (SHOP:NASDAQ) | Seeking Alpha</a></li>
<li><a href="https://www.tradingview.com/news/seekingalpha:72d53b6e5094b:0-shopify-acquires-tailwind-labs/">Shopify acquires Tailwind Labs — TradingView News</a></li>
<li><a href="https://betakit.com/tailwind-finds-stable-long-term-home-with-shopify-acquisition/">Tailwind finds “stable, long-term home” with Shopify acquisition | BetaKit</a></li>
<li><a href="https://byteiota.com/tailwind-labs-joins-shopify-what-developers-must-know/">Tailwind Labs Joins Shopify: What Developers Must Know | byteiota</a></li>
<li><a href="https://socket.dev/blog/tailwind-css-announces-layoffs">Tailwind CSS Announces 75% Layoffs as LLMs Reshape OSS Business Models | Socket</a></li>
<li><a href="https://devclass.com/2026/01/08/tailwind-labs-lays-off-75-percent-of-its-engineers-thanks-to-brutal-impact-of-ai/">Tailwind Labs lays off 75 percent of its engineers thanks to &#x27;brutal impact&#x27; of AI</a></li>

</ul>
</details>

**Tags**: `#tailwind-css`, `#acquisitions`, `#open-source-business-models`, `#ai-impact-on-devtools`, `#web-development`

---

<a id="item-tech-news-3"></a>
### [Analysis: GPT-6 Astra, Looped Transformers, and Hidden Reasoning](https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and) ⭐️ 8.0/10

An analysis on Sebastian Raschka&\#x27;s magazine examines reported GPT-6 Astra developments alongside looped transformers and hidden reasoning, and the Hacker News discussion adds expert debate and references. Much of the thread responds to a recent The Information article that described GPT-6 Astra as using &quot;recurrent depth&quot; or &quot;looped transformers,&quot; making the approach sound like a secret technique that would hinder chain-of-thought monitoring. Commenters counter that looping is essentially the same as stacking more transformer layers, except weights are reused, which saves GPU memory, and that feeding a model&\#x27;s output back into itself at inference time can by definition make the reasoning trace hidden. The discussion also points to prior research on universal transformers and on what computational problems minimally require chain-of-thought to solve.

hackernews · ModelForge · Sep 9, 14:37 · [Discussion](https://news.ycombinator.com/item?id=49627370)

**「Background: Looped Transformers」** GPT-6 Astra refers to reported OpenAI work described as using &quot;recurrent depth,&quot; also called looped transformers — an approach that reuses the same transformer weights over repeated computational iterations rather than stacking distinct layers, saving GPU memory while increasing effective depth. The idea traces back to earlier work on universal transformers, and the surrounding discussion cites research on how much chain-of-thought computation is minimally required to solve particular classes of problems. As Sebastian Raschka frames it, Astra — like other reasoning models — is trained with reinforcement learning with verifiable rewards \(RLVR\) and produces intermediate reasoning traces, which is the context in which &quot;hidden reasoning&quot; concerns about the architecture arise.

**「Impact」** Developers and AI-safety teams that rely on inspecting a model&\#x27;s emitted chain of thought to audit its behavior may face harder monitoring if production models adopt looped/recurrent-depth transformers, which can fold the reasoning trace back into the model rather than outputting it. Commenters caution that the reported novelty is limited—looped transformers largely reuse weights across depth instead of introducing a fundamentally new opacity mechanism—so the practical monitoring consequence remains contested.

**「Community Discussion」** Commenters largely agree that &quot;looped transformers&quot; are not a fundamentally new class of model: as one puts it, the approach is just stacking more transformer layers while reusing weights to save GPU memory, though another notes that looping an entire model on itself may inherently hide its reasoning trace unless that trace is deliberately extracted. Practical impressions vary, with one user saying Astra felt dramatically better until a Tuesday change made it feel like &quot;Sol&quot; and expressing hope the original returns, while another describes a real-time MSPAINT computer-use demo as jaw-dropping and comparable to earlier SVG pelican examples.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT - 6 Astra , Looped Transformers , and Hidden Reasoning</a></li>
<li><a href="https://www.hackaigc.com/blog/gpt-6-astra-everything-we-know-2026">GPT - 6 Astra : Everything We Know in 2026</a></li>
<li><a href="https://www.youtube.com/watch?v=XvmixEXPT3Q">GPT - 6 Astra .. full analysis.. - YouTube</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT-6 Astra, Looped Transformers, and Hidden Reasoning</a></li>
<li><a href="https://tech.yahoo.com/ai/chatgpt/articles/openai-astra-uses-hidden-reasoning-154630586.html">OpenAI’s Astra Uses Hidden Reasoning Loops: Experts Are Alarmed</a></li>
<li><a href="https://arxiv.org/html/2502.17416">Reasoning with Latent Thoughts: On the Power of Looped ...</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#transformers`, `#hidden reasoning`, `#AI research`, `#Hacker News`

---

<a id="item-tech-news-4"></a>
### [How I advertise malicious software on Google Ads](https://xlii.space/eng/malicious-software-on-google-ads/) ⭐️ 8.0/10

A first-hand account describes how the author exploited Google Ads&\#x27; review process to place malicious software through the advertising platform. The piece sparked a Hacker News discussion \(351 points, 211 comments\) about automated platform moderation and the difficulty of challenging opaque decisions. In the comments, the author reports that their Google account was reinstated after the issue was made visible on Hacker News, saying it was a shame that public complaining was needed to fix the problem. No source content was supplied for this evaluation, so the write-up&\#x27;s specific techniques and claims could not be independently verified here.

hackernews · xlii · Sep 9, 11:43 · [Discussion](https://news.ycombinator.com/item?id=49624856)

**「Background」** Google Ads policies require advertisers and any software their sites or apps host or link to to comply with rules against malicious software, including intentional distribution of malware that may harm or gain unauthorized access to a computer, device, or network. In the account, the author says they set up a Google Ads campaign, spent $500, and then had the account suspended for “Malicious software.” The write-up is a first-hand account of attempting to abuse Google Ads’ review process to place malicious software, making ad review and enforcement the backdrop for the incident.

**「Impact」** Google Ads users and advertisers face a demonstrated risk that the platform&\#x27;s review pipeline can be abused to distribute malware, increasing pressure on Google to make automated moderation and appeals more accountable. The author&\#x27;s reinstatement suggests enforcement may respond to public pressure rather than the original appeal path.

**「Community Discussion」** Commenters broadly criticized large platforms for hiding behind automated systems that are hard to appeal, citing examples such as a legitimate Tesla Supercharger Map edit rejected within six minutes and a YouTube session in which every ad seen was a scam. A counterpoint noted that an earlier incident involved a site that was actually compromised, and the author confirmed the account reinstatement after Hacker News visibility.

<details><summary>References</summary>
<ul>
<li><a href="https://xlii.space/eng/malicious-software-on-google-ads/">How I advertise malicious software on Google Ads</a></li>
<li><a href="https://support.google.com/adspolicy/answer/15939580?hl=en">Malicious Software - Advertising Policies Help</a></li>

</ul>
</details>

**Tags**: `#ad-fraud`, `#google-ads`, `#malware-distribution`, `#platform-moderation`, `#security`

---

<a id="item-tech-news-5"></a>
### [OpenAI reports sharp drop in GPT-6 Astra chain-of-thought monitorability](https://deploymentsafety.openai.com/gpt-6-astra) ⭐️ 8.0/10

OpenAI has disclosed that GPT-6 Astra shows a &quot;significant&quot; decline in chain-of-thought \(CoT\) monitorability compared with previous models. Chief scientist Jakub Pachocki said the ability to rely on CoT monitoring is &quot;gradually weakening,&quot; partly because models are increasingly able to control their own reasoning and can complete more complex tasks with less — or no — verbalized reasoning. OpenAI&\#x27;s development documentation also warns that Astra&\#x27;s inter-agent messages may contain grammar or spacing errors. An external evaluation by the UK AI Safety Institute additionally found that Astra&\#x27;s raw reasoning is more compressed and contains more phrases with unclear meaning. The item originates from a Telegram aggregation channel, so the specific claims should be verified against OpenAI&\#x27;s primary materials.

telegram · zaihuapd · Sep 9, 09:45

**「Background」** Chain-of-thought \(CoT\) monitoring is a safety technique in which a model&\#x27;s written reasoning trace is read by humans or automated monitors to catch misaligned or deceptive intent before it turns into actions, and OpenAI has described preserving CoT monitorability as a core goal of its research program. GPT-6 Astra is OpenAI&\#x27;s newest broadly deployed frontier model, released on September 3, and in its safety overview and system card the company compared it directly with the previous generation, GPT-5.6 Sol, stating that Astra&\#x27;s monitorability had decreased relative to Sol. Because CoT monitoring is treated as a key line of defense for the highest-risk capability tiers, including Critical-tier cybersecurity, external evaluators such as the UK AI Safety Institute were brought in to test Astra in agentic and cyber-offense-like scenarios.

**「Impact」** For AI safety researchers and evaluators who use CoT monitoring to surface deceptive or unsafe reasoning, this weakens a key visibility channel, as reflected in the UK AI Safety Institute&\#x27;s finding of more compressed and less legible raw reasoning. Because the account comes from a Telegram aggregation channel rather than verified primary documentation, the scope of the decline remains unconfirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/safety-overview-gpt-6-astra/">Safety overview: GPT - 6 Astra | OpenAI</a></li>
<li><a href="https://claypier.com/en/gpt-6-astra-cot-monitorability/">OpenAI Says GPT - 6 Astra Is Harder to Monitor , and... | claypier</a></li>
<li><a href="https://www.transformernews.ai/p/openai-gpt-6-astra-might-be-too-powerful-to-understand-or-control">OpenAI’s GPT - 6 Astra might be too powerful to understand or control</a></li>
<li><a href="https://www.techtimes.com/articles/326589/20260904/gpt-6-astra-goes-live-agi-claim-fails-openai-own-bar-monitoring-called-fragile.htm">GPT-6 Astra Goes Live: AGI Claim Fails OpenAI Own Bar, Monitoring Called Fragile</a></li>

</ul>
</details>

**Tags**: `#AI安全`, `#思维链可监测性`, `#OpenAI`, `#可解释性`, `#模型评估`

---

<a id="item-tech-news-6"></a>
### [IEEE Spectrum reports growing evidence autonomous cars save lives](https://spectrum.ieee.org/are-self-driving-cars-safe) ⭐️ 7.0/10

IEEE Spectrum&\#x27;s article argues there is growing proof that autonomous cars save lives, and the item frames the evidence as sufficient to prompt renewed debate about road safety. The accompanying Hacker News discussion focuses on how autonomous-vehicle fatality rates are measured, particularly whether they should be compared with average human drivers or with the rideshare drivers they may replace. Commenters also raise broader transportation questions, including whether better driver education, stricter testing, alcohol restrictions, or public transit investment could save more lives. The supplied item does not include the full article or establish a major paradigm shift or breakthrough.

hackernews · bookofjoe · Sep 9, 17:14 · [Discussion](https://news.ycombinator.com/item?id=49629886)

**「Background」** Autonomous vehicles have moved from testing to commercial operation, with driverless services such as Waymo and Zoox carrying riders in cities including San Francisco and Atlanta and thereby generating the crash data now under scrutiny. Safety assessments typically compare self-driving crash and injury rates against those of human drivers, and mounting research suggests self-driving cars crash significantly less often than people, with advanced driver assistance systems also showing safety benefits. A central complication is the choice of baseline: comparing against average drivers rather than the rideshare drivers these vehicles actually replace can make the safety numbers look more or less impressive.

**「Impact」** The practical consequence for autonomous-vehicle operators such as Waymo is that their safety record will be judged against the most relevant human baseline—likely the rideshare services they displace—rather than the average driver, a distinction that could alter how persuasive their safety claims are.

**「Community Discussion」** Commenters largely accepted the potential safety benefit but challenged the comparison baseline, with giantg2 noting Waymo compares against average drivers rather than the rideshare drivers its cars replace, and mostly\_harmless arguing fatality data is skewed by factors such as seatbelt non-use \(44%\), speeding \(29%\), alcohol involvement \(~30%\), and vulnerable road users \(20% pedestrians or bicyclists, plus 16% motorcyclists\). Others debated priorities and consequences, with cbondurant favoring public transit investment over autonomous cars and alexpotato predicting that insurance costs could shift in favor of autonomy, making human driving a prestige activity.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrum.ieee.org/are-self-driving-cars-safe">Are Self Driving Cars Safe as Early Data Suggests? - IEEE ...</a></li>
<li><a href="https://publichealth.jhu.edu/2026/the-safety-data-on-autonomous-vehicles">The Safety Data on Autonomous Vehicles | Johns Hopkins ...</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#road safety`, `#AI systems`, `#Waymo`, `#public transit`

---

<a id="item-tech-news-7"></a>
### [Pentagon Sought OpenAI Model With Low Military Refusal Rate, Leaks Show](https://theintercept.com/2026/09/08/pentagon-openai-military-contract/) ⭐️ 7.0/10

Leaked documents reported by The Intercept indicate that the Pentagon asked OpenAI to supply the U.S. military with a special version of its AI technology that would decline military commands as infrequently as possible. The &quot;minimum refusal rate&quot; language reportedly appeared in an updated contract version designated &quot;P00003,&quot; which expanded the original deal between the Defense Department and OpenAI arranged last summer. Both OpenAI and the Pentagon deny agreeing to such &quot;minimum refusal&quot; wording, saying the leaked &quot;P00003&quot; document was a draft rather than a final version. OpenAI spokesperson Nate Evans said the company &quot;never agreed to contract language requiring a &\#x27;minimum refusal rate&\#x27;&quot; and that no such language appeared in its executed contract.

telegram · zaihuapd · Sep 9, 09:02

**「Background」** Refusal rate is a measurable property in AI safety and security research, indicating how often a model declines requests; it can be evaluated and defended against manipulation. OpenAI&\#x27;s contract with the U.S. Department of War \(the Pentagon\), described by the company in February 2026, covers deployment in classified environments and includes stated safety red lines and legal protections. That agreement followed a political shift in which the Trump administration banned Anthropic from federal contracts, making OpenAI&\#x27;s military work a subject of public controversy.

**「Impact」** The reported &quot;minimal refusal rates&quot; language, if adopted, would push OpenAI&\#x27;s military-facing models toward suppressing safety-based refusals for national security use cases, directly shaping how the company&\#x27;s policies constrain defense applications. Both OpenAI and the Pentagon deny the wording appeared in an executed contract, saying the leaked P00003 file was a draft, so the practical effect remains contested.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.05794v1">Bait-and-Recover: Poisoning Internal Refusal Signalsto Defend LLMs...</a></li>
<li><a href="https://www.techtimes.com/articles/315025/20260311/openai-pentagon-ai-controversy-military-deployment-public-backlash-ethics.htm">OpenAI Pentagon AI Controversy: Military Deployment, Public ...</a></li>
<li><a href="https://openai.com/index/our-agreement-with-the-department-of-war/">Our agreement with the Department of War - OpenAI</a></li>
<li><a href="https://theintercept.com/2026/09/08/pentagon-openai-military-contract/">The Pentagon Asked OpenAI for Artificial Intelligence ...</a></li>
<li><a href="https://www.unite.ai/openai-pentagon-contract-defines-mission-models-by-minimal-refusal-rates/">OpenAI Pentagon Contract Defines ‘Mission Models’ by Minimal ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#military AI`, `#OpenAI`, `#defense contracts`, `#AI refusal alignment`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Brent Crude Tops $100 as U.S.-Iran Fighting Disrupts Strait of Hormuz Flows](https://oilprice.com/Energy/Crude-Oil/Oil-Breaks-100and-This-Rally-Has-Legs.html) ⭐️ 8.0/10

Brent crude rose above $100 per barrel on Wednesday for the first time since late July after renewed U.S.-Iran fighting cut oil flows through the Strait of Hormuz to below 2 million barrels per day from 6-9 million in August, according to estimates from Rystad Energy and Kpler. The International Energy Agency reported that global oil inventories fell by 69 million barrels in July, an average daily decline of 2.7 million barrels, while 8.3 million barrels per day of Middle Eastern production remained shut in.

rss · OilPrice.com · Sep 10, 00:00

**「Background」** The Strait of Hormuz is a narrow chokepoint where Iran&\#x27;s strikes on vessels have disrupted oil trade, and the collapse of the June 2025 ceasefire between Washington and Tehran had already left regional shipping at risk. Recovering tanker traffic through the strait had been holding prices down before this week&\#x27;s escalation.

**「Impact」** If the conflict continues to disrupt flows, the ongoing draw on global oil inventories could keep upward pressure on fuel and energy costs for households and businesses.

<details><summary>References</summary>
<ul>
<li><a href="https://mezha.net/eng/bukvy/eab38bd6_iran_tightens_grip/">Iran tightens grip on Strait of Hormuz as attacks threaten... - #Mezha</a></li>
<li><a href="https://www.firstpost.com/business/houthi-attacks-red-sea-shipping-bab-el-mandeb-hormuz-traffic-us-iran-conflict-14034057.html">Two oil chokepoints under threat: Houthi attacks hit Red Sea shipping...</a></li>

</ul>
</details>

**Tags**: `#oil`, `#Brent crude`, `#Strait of Hormuz`, `#US-Iran conflict`, `#IEA`

---

<a id="item-finance-news-2"></a>
### [Negative Power Prices Spread Across Europe as Storage Lags Renewables](https://oilprice.com/Energy/Energy-General/Negative-Power-Prices-Are-Piling-Up-Across-Europe.html) ⭐️ 8.0/10

Negative wholesale electricity prices have become widespread across Europe as wind and solar generation outpaces energy storage, with Germany recording 573 negative-price hours in 2025 — above its 2024 record — and Spain, Sweden, the Netherlands and France each exceeding 500 hours by the end of October 2025, according to the article. In June, EU energy ministers agreed to triple the bloc&\#x27;s storage capacity by adding roughly 30-35 GW by 2028, against about 55 GW today, while the article cites an estimated need for 200 gigawatt-hours of storage by 2030.

rss · OilPrice.com · Sep 9, 21:00

**「Background」** Russia&\#x27;s February 2022 invasion of Ukraine exposed the EU&\#x27;s reliance on Russian gas for about 40 percent of its supply, prompting a rapid buildout of wind and solar whose output varies with weather; storage capacity has not grown at the same pace. Negative wholesale prices arise when generation outpaces demand and the surplus cannot be stored or exported.

**「Impact」** Falling solar farm values and negative peak-hour prices push some renewable developers toward exiting the market, which the article says discourages further investment in the sector.

<details><summary>References</summary>
<ul>
<li><a href="https://oilprice.com/Energy/Energy-General/Negative-Power-Prices-Are-Piling-Up-Across-Europe.html">Negative Power Prices Are Piling Up Across Europe | OilPrice.com</a></li>

</ul>
</details>

**Tags**: `#European energy`, `#negative power prices`, `#energy storage`, `#renewables`, `#EU energy policy`

---

<a id="item-finance-news-3"></a>
### [U.S. Sanctions Iran&\#x27;s Remaining Airlines in Aviation Crackdown](https://oilprice.com/Energy/Energy-General/US-Moves-to-Isolate-Irans-Aviation-Sector-From-the-Global-Economy.html) ⭐️ 8.0/10

The U.S. Treasury on September 8 sanctioned 36 targets, including 27 Iranian airlines and foreign companies accused of helping Mahan Air obtain aircraft and parts, the first use of an August 24 determination aimed at Iran&\#x27;s aviation sector. Treasury Secretary Scott Bessent said anyone doing business with Iran&\#x27;s remaining airlines risks being cut off from the global financial system.

rss · OilPrice.com · Sep 9, 18:00

**「Background」** Mahan Air, Iran’s largest airline, has been under U.S. sanctions since 2011 over allegations that it provides logistical support to the Islamic Revolutionary Guard Corps, including transporting personnel and weapons. The September 8 measures are part of Operation Economic Outcast, a campaign announced by Treasury Secretary Scott Bessent on August 24 to cut off what Washington describes as Iran’s remaining economic lifelines.

**「Impact」** Foreign airlines flying U.S.-origin aircraft into Iran, along with fuel suppliers, ground handlers, cargo firms and banks that still serve sanctioned Iranian carriers, face possible loss of access to the U.S. financial system under secondary sanctions.

<details><summary>References</summary>
<ul>
<li><a href="https://home.treasury.gov/news/press-releases/sb0623/">Treasury Grounds Iranian Airlines with Sweeping Sanctions Action | U.S. Department of the Treasury</a></li>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/09/operation-economic-outcast-grounds-irans-aviation-sector">Operation Economic Outcast Grounds Iran’s Aviation Sector - United States Department of State</a></li>
<li><a href="https://www.rvmnews.com/2026/09/treasury-unleashes-sweeping-sanctions-to-ground-irans-terror-linked-airline-network-watch/">Treasury Unleashes Sweeping Sanctions to Ground Iran’s Terror-Linked Airline Network [WATCH]</a></li>

</ul>
</details>

**Tags**: `#Iran sanctions`, `#aviation`, `#Mahan Air`, `#OFAC/Treasury`, `#secondary sanctions`

---

<a id="item-finance-news-4"></a>
### [Google to Invest €13 Billion in Finnish AI Infrastructure and Signs 22-Year Nuclear Deal](https://oilprice.com/Latest-Energy-News/World-News/Google-Bets-13-Billion-on-Finland-to-Power-AI-Boom-With-Nuclear-Energy.html) ⭐️ 8.0/10

Google said Wednesday it will invest at least €13 billion \($15.1 billion\) in Finnish AI infrastructure in 2027 and 2028, alongside a 22-year power purchase agreement with Fortum for up to 50% of the output from the Loviisa nuclear plant — the company&\#x27;s first nuclear power contract outside the United States. The Fortum deal funds upgrades that keep Loviisa, which supplies about 10% of Finland&\#x27;s electricity, running through 2050 instead of shutting down after 2030, the companies said.

rss · OilPrice.com · Sep 9, 16:30

**「Background」** Loviisa is Fortum&\#x27;s two-reactor nuclear plant in Finland; it supplies about 10% of the country&\#x27;s electricity, and Fortum had proposed extending its life to 2050. Fortum said that without a new agreement the plant would have had to shut down after 2030.

**「Impact」** The nuclear contract keeps Finland&\#x27;s Loviisa plant — which supplies about 10% of the country&\#x27;s electricity and employs nearly 600 people — operating through 2050 instead of shutting down after 2030, preserving that generation and those jobs for the Finnish grid and the plant&\#x27;s host community.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Loviisa_Nuclear_Power_Plant">Loviisa Nuclear Power Plant - Wikipedia</a></li>
<li><a href="https://www.fortum.com/energy-production/nuclear-power/plants/loviisa">Loviisa Nuclear Power Plant | Fortum</a></li>
<li><a href="https://www.googlecloudpresscorner.com/2026-09-09-Google-Deepens-Commitment-to-Finland-with-Two-Year-EUR13-Billion-investment-in-AI-Infrastructure">Google Deepens Commitment to Finland with Two-Year €13 ...</a></li>

</ul>
</details>

**Tags**: `#Google-Alphabet`, `#Nuclear energy`, `#AI infrastructure`, `#Finland`, `#Corporate investment`

---

<a id="item-finance-news-5"></a>
### [Bank of England Warns Iran Conflict Could Push UK Inflation Above 4%](https://oilprice.com/Energy/Energy-General/Bank-of-England-Warns-Iran-War-Could-Push-UK-Inflation-Above-4.html) ⭐️ 8.0/10

Bank of England Governor Andrew Bailey told MPs on Tuesday that inflation risks are &quot;to the upside&quot; and energy prices &quot;could be higher still&quot; if the conflict with Iran continues. The Bank&\#x27;s summer scenario warned inflation could top 4% — double its 2% target — if oil prices stay near $100 a barrel for several months; UK inflation was 2.9% in the year to July, and rate-setters decide on interest rates next week.

rss · OilPrice.com · Sep 9, 16:00

**「Background」** UK inflation was 2.9% in the year to July, and the Bank of England&\#x27;s summer report estimated it could exceed 4% — double the Bank&\#x27;s 2% target — if oil prices stayed around $100 a barrel for several months.

**「Impact」** Because UK government bond yields reflect fears of an inflation spike, the country is already paying its highest borrowing costs on new debt in nearly 30 years, and traders have priced in an extra premium for prolonged disruption in the Strait of Hormuz that could mean higher prices for households.

**Tags**: `#Bank of England`, `#UK inflation`, `#Iran conflict`, `#oil prices`, `#interest rates`

---

<a id="item-finance-news-6"></a>
### [Copper Hits Record High as Smelter Fees Fall to Zero](https://oilprice.com/Metals/Commodities/Copper-Hits-Record-Highs-While-Smelters-Lose-Money-on-Every-Ton.html) ⭐️ 8.0/10

Three-month copper on the London Metal Exchange hit a record $14,779 a ton on Tuesday, its fourth straight session of gains, and is up nearly 18% this year. The 2026 benchmark treatment and refining charge — the fee miners pay smelters to turn concentrate into finished metal — settled at zero dollars a ton, the lowest annual benchmark on record, down from $21.25 in 2025, with spot rates falling to roughly negative $127 a ton by midyear.

rss · OilPrice.com · Sep 9, 15:00

**「Background」** Treatment and refining charges are the fees miners pay smelters to turn copper concentrate into refined metal; the 2026 annual benchmark settled at zero dollars a ton, down from $21.25 in 2025 and $80 in 2024, and spot charges turned negative as smelters competed for scarce concentrate.

**「Impact」** Smelters, about half of which are in China, are processing copper at a loss while buyers of refined metal face record prices.

<details><summary>References</summary>
<ul>
<li><a href="https://skillings.net/coppers-smelting-crisis-global-activity-hits-decade-low-as-treatment-charges-collapse-to-zero/">Copper Smelting Crisis 2026 : TC/RCs Hit Zero</a></li>
<li><a href="https://discoveryalert.com/analysis/copper-concentrate-scarcity-negative-tcrc/">What Record Negative TCRCs Reveal About Copper ... - Discovery Alert</a></li>

</ul>
</details>

**Tags**: `#copper`, `#commodity markets`, `#smelters`, `#supply constraints`, `#US tariffs`

---

<a id="item-finance-news-7"></a>
### [Federal Reserve holds rates steady but leaves door open to hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

The Federal Reserve left interest rates unchanged while keeping open the possibility of a future increase, CBS News reported; ABC7 Los Angeles reported the decision came in a 9-3 vote.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The federal funds rate — the benchmark the Federal Reserve uses to steer borrowing costs across the economy — has been held in a 3.5%–3.75% range for a fifth consecutive meeting, with inflation still running above the central bank&\#x27;s 2% target.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members ...</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady | Fox Business</a></li>
<li><a href="https://www.linkedin.com/posts/hilltop-securities_hilltopsecurities-economiccommentart-julyfomc-activity-7485401527298228224-zcE5">July FOMC Meeting Outlook Worsens Inflation Concerns | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest rates`, `#Monetary policy`, `#US economy`

---

<a id="item-finance-news-8"></a>
### [Adani Airport unit signs $1 billion fundraising deal; Adani Enterprises shares rise](https://www.cnbc.com/2026/09/09/adani-enterprises-airport-fundraise-shares.html) ⭐️ 7.0/10

Adani Enterprises shares rose nearly 5% Wednesday after its airport unit said it signed a binding deal to raise about 98.25 billion rupees \($1 billion\) from global and domestic investors, valuing Adani Airport Holdings at about $18 billion before the investment, according to the company statement. The investors — Alpha Wave Global, Premji Invest, Temasek and BlackRock-managed funds — will subscribe to new shares in three tranches and collectively own about 5.54% after the final tranche, expected to be completed by July 2027, subject to regulatory approvals.

rss · CNBC Finance · Sep 9, 06:26

**「Background」** Adani Airport Holdings is the airport arm of Adani Enterprises, operating eight Indian airports — including Mumbai, Navi Mumbai, Ahmedabad and Guwahati — that together handle more than 23% of the country&\#x27;s passenger traffic. The airport deal follows Adani Enterprises&\#x27; 150 billion rupee qualified institutional placement, a share sale to large institutional investors, in July.

**「Who is affected」** The money is earmarked for expanding and modernizing Adani Airport Holdings&\#x27; eight Indian airports and its airport-city and ground-handling businesses, with the company targeting capacity for about 200 million passengers a year — a change that mainly affects Indian air travelers and the airports&\#x27; commercial partners.

<details><summary>References</summary>
<ul>
<li><a href="https://startupfox.in/company/adani-airport-holdings">Adani Airport Holdings — News, Funding &amp; Updates | StartupFox</a></li>
<li><a href="https://timesofindia.indiatimes.com/business/india-business/adani-airports-to-raise-1-billion-primary-equity-from-marquee-global-investors/articleshow/133952109.cms">Adani Airports to raise $1 billion primary equity... - The Times of India</a></li>
<li><a href="https://legal.economictimes.indiatimes.com/news/industry/adani-enterprises-raises-inr-150-billion-in-record-qip-with-cam-and-trilegal/132331254">Adani Enterprises Raises INR 150 Billion in Record QIP with CAM...</a></li>
<li><a href="https://www.ndtv.com/india-news/adani-airport-holdings-secures-1-billion-investment-from-global-funds-12021189">Adani Airport Holdings Secures $1 Billion Investment From ...</a></li>
<li><a href="https://www.adani.com/newsroom/media-releases/adani-airports-to-raise-usd-1-billion-of-primary-equity-from-marquee-global-investors">Adani Airports to raise ~USD 1 billion of primary equity from ...</a></li>

</ul>
</details>

**Tags**: `#Adani Enterprises`, `#airport infrastructure`, `#private fundraising`, `#India`, `#equity investment`

---

<a id="item-finance-news-9"></a>
### [China&\#x27;s EV makers turn to humanoid robots as car sales slow](https://www.cnbc.com/2026/09/09/chinas-ev-makers-shift-gears-to-focus-on-humanoids-as-car-market-slows.html) ⭐️ 7.0/10

Chinese electric-vehicle makers including Xpeng are expanding into humanoid robots as China&\#x27;s EV sales head for their worst year since 2021, with Xpeng raising $900 million for its robotics unit — a round the company says is China&\#x27;s largest in &quot;embodied&quot; AI, or hardware-connected artificial intelligence. Xpeng said it plans to begin mass production of its robots by the end of this year, starting in its own stores and business venues, though analysts say firm external orders and robotics revenue guidance are still missing.

rss · CNBC Finance · Sep 9, 04:12

**「Background」** Chinese automakers spent the past decade pouring money into electric cars, but slowing domestic sales and fierce price competition have squeezed the industry — the average profit margin in China&\#x27;s vehicle manufacturing sector was 1.5% in the first half of 2026, according to China Association of Automobile Manufacturers data cited by Counterpoint Research. Xpeng&\#x27;s robotics unit raised more than $900 million in August 2026, described by the company as China&\#x27;s largest funding round in &quot;embodied AI&quot; \(hardware-connected artificial intelligence\), to mass-produce its IRON humanoid robot.

**「Impact」** The pivot is most consequential for the automakers&\#x27; investors and for China&\#x27;s robotics sector, since Jefferies estimates Xpeng can reuse 85% of its motors, chips and smart-driving software in humanoids, giving carmakers a cost advantage over pure-play robot startups even as the sector&\#x27;s commercial viability remains unproven.

<details><summary>References</summary>
<ul>
<li><a href="https://www.xpeng.com/pressroom/news/01a03797fccda01e0de68a02a256006a">XPENG Robotics Raises US$900M for Humanoid Robots</a></li>
<li><a href="https://tbreak.com/chinese-ev-makers-humanoid-robots/">Chinese humanoid robots : why EV makers are expanding</a></li>

</ul>
</details>

**Tags**: `#China EV industry`, `#humanoid robotics`, `#Xpeng`, `#corporate strategy`, `#financing`

---

<a id="item-finance-news-10"></a>
### [Analysis Disputes UK Report&\#x27;s £500 Household Saving From Scrapping Net Zero](https://oilprice.com/Energy/Energy-General/Britain-Can-Save-500-by-Scrapping-Net-Zero-If-It-Ignores-Most-of-the-Bill.html) ⭐️ 7.0/10

An analysis by Leon Stille published on Oilprice.com challenges a report by the UK think tank Onward, which estimates that abandoning Britain&\#x27;s statutory 2050 net-zero target after 2029 would save households more than £500 a year, based on £320 billion in cumulative power-system savings from 2030 to 2050 spread over roughly 30 million households and 20 years. The critique argues that figure comes from modelling only Great Britain&\#x27;s power-system costs, which the report itself says excludes heat, transport and wider-economy impacts, and that the lower cost partly reflects 43 TWh—about 10%—less electricity demand in 2050 because support for electric vehicles, heat pumps and hydrogen is reduced.

rss · OilPrice.com · Sep 9, 19:00

**「Background」** The £500 figure traces to Onward&\#x27;s Firm Foundations report, which compares current policy with an &quot;Alternative Policy Pathway&quot; that would drop Britain&\#x27;s statutory 2050 net-zero target after 2029 in favour of heavier reliance on gas and nuclear, and estimates that pathway saves £320 billion in power-system costs between 2030 and 2050 — about £530 per household a year when spread over roughly 30 million homes.

**「Who is affected」** Under the report&\#x27;s alternative pathway, UK households would see a smaller electricity system but keep buying more petrol, diesel and gas, because reduced support for electric vehicles and heat pumps shifts spending outside the power bill the £500 figure measures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yahoo.com/news/world/articles/britain-save-500-scrapping-net-190000216.html">Britain Can Save £ 500 by Scrapping Net Zero , If It Ignores Most of the...</a></li>

</ul>
</details>

**Tags**: `#UK energy policy`, `#net zero`, `#household energy bills`, `#electrification`, `#policy analysis`

---

<a id="item-finance-news-11"></a>
### [Belarusian Refineries Claim Decade-High Profitability as Russia&\#x27;s Fuel Crisis Drives Record Exports](https://oilprice.com/Latest-Energy-News/World-News/Belarus-Refineries-Post-Decade-High-Profits-Amid-Russias-Fuel-Crisis.html) ⭐️ 7.0/10

Belarusian refineries recorded their highest profitability in a decade in 2026, according to Belneftekhim&\#x27;s own assessment relayed by the independent Pozirk news agency, as gasoline shipments to Russia rose 25-fold to nearly 665,000 tons in the first seven months of 2026 from the same period in 2025, Reuters trade data show.

rss · OilPrice.com · Sep 9, 18:30

**「Background」** Belarus has only two refineries, Naftan and Mozyr, and they process Russian crude on a tolling basis — converting Russian oil for the Russian market rather than for Belarusian use. Ukrainian drone strikes this summer knocked out a large share of Russia&\#x27;s refining capacity, creating the fuel shortage Belarus is now helping to fill.

**「Impact」** Russian households and businesses face fuel rationing, with gasoline available at fewer than a third of the country&\#x27;s gas stations by mid-August and purchase limits reinstated in at least a dozen regions after the Orsk refinery shut down, according to The Insider.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mozyr_Oil_Refinery">Mozyr Oil Refinery - Wikipedia</a></li>
<li><a href="https://www.twz.com/news-features/ukraine-carried-out-its-deepest-drone-strike-on-russia-ever">Ukraine Carried Out Its Deepest Drone Strike On Russia Ever</a></li>

</ul>
</details>

**Tags**: `#Belarus energy`, `#Russia fuel crisis`, `#oil refining`, `#export ban`, `#energy markets`

---

<a id="item-finance-news-12"></a>
### [Uganda Prepares Pearl Sweet Crude for First Exports](https://oilprice.com/Energy/Crude-Oil/Uganda-Launches-New-Crude-Grade-as-First-Oil-Exports-Near.html) ⭐️ 7.0/10

Uganda is preparing to export its new Pearl Sweet crude from Lake Albert fields, with the two projects expected to produce 230,000 barrels per day \(b/d\) at plateau after officials pushed first oil from an initial June 2026 target to December at Kingfisher \(25,000 b/d\) and the first quarter of 2027 at Tilenga.

rss · OilPrice.com · Sep 9, 17:00

**「Background」** Pearl Sweet is a blend from TotalEnergies&\#x27; Tilenga and CNOOC&\#x27;s Kingfisher fields, owned 56.67% by TotalEnergies, 28.33% by CNOOC and 15% by Uganda&\#x27;s UNOC; it is low-sulphur at about 0.16% but waxy, with a pour point—the temperature below which it stops flowing freely—of around 39°C, so it must be heated through the 1,443-km East African Crude Oil Pipeline to Tanzania&\#x27;s Tanga port.

**「Impact」** The crude is expected to sell at a discount to Brent because of above-average transport and heating costs—transport to Tanga alone is estimated at $12–13/bbl—so Uganda&\#x27;s eventual export revenue and the set of refiners able to handle it will depend on how wide that discount must be.

**Tags**: `#Uganda oil`, `#Pearl Sweet crude`, `#EACOP pipeline`, `#African oil exports`, `#TotalEnergies`

---