---
layout: default
title: "Horizon Summary: 2026-09-02 (EN)"
date: 2026-09-02
lang: en
---

> From 234 items, 28 important content pieces were selected

---

**Technology News**
1. [Claude Fable 5.1 and Mythos 5.1 arrive with cheaper cache reads](#item-tech-news-1) ⭐️ 8.0/10
2. [A Data-Driven Check on Ed Zitron&\#x27;s AI Skeptic Predictions](#item-tech-news-2) ⭐️ 8.0/10
3. [Small Transformer Trained in 1.5 Hours Beats Many LLMs on ARC](#item-tech-news-3) ⭐️ 8.0/10
4. [EvoUndo: Framework for Recoverable LLM Agent Self-Evolution](#item-tech-news-4) ⭐️ 8.0/10
5. [Virtualizor Update Infrastructure BGP-Hijacked, Root Backdoor Delivered](#item-tech-news-5) ⭐️ 8.0/10
6. [AnkiDroid Hits Google Play Ban on Open Collective Donation Link](#item-tech-news-6) ⭐️ 7.0/10
7. [Jujutsu Creator Martin Joins ERSC to Build GitHub Competitor](#item-tech-news-7) ⭐️ 7.0/10
8. [Latent Reasoning in 2026: Mapping Five Families from Coconut to BDH-CQ](#item-tech-news-8) ⭐️ 7.0/10
9. [TontaubeV1: Open-Weight 2.9B Character-Level TTS Model](#item-tech-news-9) ⭐️ 7.0/10
10. [China&\#x27;s Solar Capacity Overtakes Coal to Become Largest Power Source](#item-tech-news-10) ⭐️ 7.0/10
11. [Google to Release Gemini 3.8 Flash, Coding Edge Reportedly Narrows Gap](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Asian Spot LNG Prices Hit 5-Month High as Hormuz Blockage Persists](#item-finance-news-1) ⭐️ 9.0/10
2. [U.S. and Iran Trade Strikes, Pushing Middle East Oil Benchmarks Above $100](#item-finance-news-2) ⭐️ 9.0/10
3. [Federal Reserve holds interest rates steady](#item-finance-news-3) ⭐️ 9.0/10
4. [Fed&\#x27;s Barr says he would support rate hike if inflation doesn&\#x27;t ease](#item-finance-news-4) ⭐️ 8.0/10
5. [Saudi Arabia Plans to Cut Domestic Oil Use by 1 Million b/d by 2030](#item-finance-news-5) ⭐️ 8.0/10
6. [Lithium Prices Surge as LG Signs 10-Year U.S. Supply Deal](#item-finance-news-6) ⭐️ 8.0/10
7. [Tanzania’s Mining Reforms Show Payoff With Record Gold Exports](#item-finance-news-7) ⭐️ 8.0/10
8. [UK Shop Prices Hit Two-Year High as Food Inflation Jumps](#item-finance-news-8) ⭐️ 8.0/10
9. [U.S. Energy Storage Installations Set Record in Q2 2026](#item-finance-news-9) ⭐️ 8.0/10
10. [Japan Relaxes Enforcement of Monthly Overtime Cap](#item-finance-news-10) ⭐️ 8.0/10
11. [TSMC&\#x27;s $269 Billion Expansion Highlights Its Strong Margin](#item-finance-news-11) ⭐️ 8.0/10
12. [Fed may hold rates after cooler inflation data](#item-finance-news-12) ⭐️ 8.0/10
13. [Fed Leaves Interest Rates Unchanged; Powell Holds News Briefing](#item-finance-news-13) ⭐️ 8.0/10
14. [Qualcomm Announces Double-Digit Chip Price Increases From September 1](#item-finance-news-14) ⭐️ 7.0/10
15. [China’s First Micro-Short-Drama Regulation Takes Effect](#item-finance-news-15) ⭐️ 7.0/10
16. [China Issues Guidelines on Overseas Competition and Compliance for Automakers](#item-finance-news-16) ⭐️ 7.0/10
17. [China imposes 20% dividend tax on foreign individuals from 2026](#item-finance-news-17) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Claude Fable 5.1 and Mythos 5.1 arrive with cheaper cache reads](https://www.anthropic.com/claude-fable-and-mythos-5-1) ⭐️ 8.0/10

Anthropic released Claude Fable 5.1 and Claude Mythos 5.1, new AI models with a published system card. The update emphasizes improved writing style, with an Anthropic employee saying Fable 5.1 sounds less stereotypically like earlier Claude models and follows style instructions more reliably, along with science performance gains. Pricing changes include cache-read costs dropping from $1/M to $0.25/M on Fable 5.1, which is half of Opus&\#x27;s $0.5/M. Community testing exercised thinking-effort settings from low through xhigh and max, with one generation taking just under 14 minutes. Critics argue Fable appears nerfed, that Mythos is being used as a marketing hook, and that removal of thought traces hurts prompt debugging.

hackernews · denysvitali · Sep 1, 17:53 · [Discussion](https://news.ycombinator.com/item?id=49525378)

**「Background」** Anthropic introduced Claude Fable 5.1 and Claude Mythos 5.1 as versions of the same underlying model with different safeguard levels: Fable 5.1 is generally available, while Mythos 5.1 is restricted to trusted access programs focused on cybersecurity and life sciences. Building on Anthropic&\#x27;s existing Claude model line, the release targets improvements in coding, knowledge work, and writing style, alongside adjustments to pricing and thinking-effort options. The accompanying system card documents safety evaluations for both variants.

**「Impact」** Developers using the Anthropic API can cut Fable 5.1 cache-read costs from $1/M to $0.25/M, making it cheaper per cached token than Opus&\#x27;s $0.5/M, though community members disagree on whether other model changes are regressions.

**「Community Discussion」** Early reactions split: an Anthropic employee praises Fable 5.1&\#x27;s more natural writing and science work, and a user shares thinking-effort pelican examples including a 14-minute max run. Another commenter calls Fable &\#x27;useless&\#x27; and &\#x27;nerfed,&\#x27; dismisses Mythos as a marketing stunt, and criticizes removed thought traces.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5.1 and Claude Mythos 5.1 \\ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/models/fable-5-1/whats-new-fable-5-1">What&#x27;s new in Claude Fable 5.1 - Claude Platform Docs</a></li>
<li><a href="https://www.datastudios.org/post/claude-fable-5-1-and-claude-mythos-5-1-anthropic-s-new-standard-for-coding-and-scientific-research">Claude Fable 5.1 and Claude Mythos 5.1: Anthropic&#x27;s New Standard for ...</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#claude`, `#ai-models`, `#machine-learning`, `#llm`

---

<a id="item-tech-news-2"></a>
### [A Data-Driven Check on Ed Zitron&\#x27;s AI Skeptic Predictions](https://danluu.com/zitron/) ⭐️ 8.0/10

Dan Luu&\#x27;s new post evaluates how accurately Ed Zitron&\#x27;s AI-skeptic predictions have held up, grounding the assessment in concrete cases rather than offering a blanket verdict. The analysis finds a mixed record, acknowledging that some of Zitron&\#x27;s criticisms have merit while highlighting a pattern of overstatement and selective framing. By publishing a data-driven counterweight to one of the most prominent AI-skeptic voices, Luu&\#x27;s piece gives industry watchers a more precise basis for judging such claims. The essay has generated substantial Hacker News discussion about Zitron&\#x27;s credibility and whether AI boosters should be held to similarly rigorous standards.

hackernews · jatins · Sep 1, 18:35 · [Discussion](https://news.ycombinator.com/item?id=49526069)

**「Context」** Ed Zitron is a tech commentator known for harshly skeptical takes on the AI industry, often framing developments as hero-villain narratives involving major tech companies and their leaders. Dan Luu, a programmer and writer who frequently analyzes tech industry claims with data, examined how accurate Zitron&\#x27;s specific predictions have been over time. This post appears amid ongoing debate about AI hype and skepticism, with Zitron sometimes surfacing leaked data but pairing it with strongly biased commentary.

**「Impact」** For AI industry watchers, the post offers a concrete baseline for testing prominent skeptic claims, and the ensuing debate shows strong demand for applying the same evidence-based scrutiny to AI company leaders&\#x27; predictions.

**「Community Discussion」** Hacker News commenters point out that Zitron has become the mirror image of AI boosters, trapped by an audience that expects him never to concede errors, and suggest holding leaders like Altman and Amodei to comparable standards. Several also caution that readers are projecting their own predictions onto Zitron instead of discussing the exact claims Luu evaluates.

<details><summary>References</summary>
<ul>
<li><a href="http://danluu.com/zitron/">How accurate have Ed Zitron&#x27;s AI skeptic predictions been?</a></li>
<li><a href="https://news.ycombinator.com/item?id=49526069">How accurate have Ed Zitron&#x27;s AI skeptic predictions been? | Hacker News</a></li>

</ul>
</details>

**Tags**: `#AI skepticism`, `#Ed Zitron`, `#predictions`, `#AI industry`, `#analysis`

---

<a id="item-tech-news-3"></a>
### [Small Transformer Trained in 1.5 Hours Beats Many LLMs on ARC](https://mvakde.github.io/blog/44-on-arc-1/) ⭐️ 8.0/10

A developer trained a small transformer from scratch in 1.5 hours and reports it beats many large language models on the ARC benchmark, challenging the assumption that massive LLMs are necessary. The work emphasizes sample efficiency and architectural improvements such as SwiGLU activations, RMSNorm, more data diversity, and scaling to 8 layers, rather than enormous training compute. The author clarifies that this is not an LLM but a small autoregressive transformer, and that ARC is a metalearning benchmark where learning from the evaluation puzzles is intended, though the labels are never trained on. The result is presented as evidence that extremely complex problems can be tackled without large language models.

hackernews · porridgeraisin · Sep 1, 09:52 · [Discussion](https://news.ycombinator.com/item?id=49519939)

**「Background」** ARC-AGI-1 is a benchmark designed to measure abstract reasoning and fluid intelligence with visual grid puzzles, requiring models to infer rules from a few demonstrations rather than memorize patterns. Traditionally, strong results on ARC came from large language models or specialized architectures trained with enormous compute, or from expensive fine-tunes. This item reports a small transformer trained from scratch in 1.5 hours on a single RTX 5090, using test-time training on the eval puzzles themselves, 3D RoPE embeddings, and per-task learned embeddings, achieving 44% on ARC-AGI-1 public eval for around 67 cents of compute, matching specialized models like TRM/HRM.

**「Impact」** The result suggests that appropriately designed small transformers can approach or beat large LLMs on reasoning benchmarks with dramatically lower compute, potentially lowering barriers for researchers and enabling more efficient deployment in specialized tasks. Independent replication and full validation of the claim are still lacking, so the result should be treated as a promising demonstration rather than a settled conclusion.

**「Community Discussion」** In the Hacker News thread, the author engaged with questions about sample efficiency and the use of evaluation puzzles, clarifying that ARC is a metalearning benchmark and the labels were not trained on. One commenter described the architectural improvements as &quot;squeezing the lemon,&quot; suggesting that new methods should aim for near-SOTA results before optimization, while others praised the work and expressed interest in the broader implications.

<details><summary>References</summary>
<ul>
<li><a href="https://mangodeveloper.com/articles/a-15-hour-transformer-beats-llms-on-arc-agi-and-it-costs-pocket-change">A 1.5-Hour Transformer Beats LLMs on ARC-AGI, And It Costs ...</a></li>
<li><a href="https://mvakde.github.io/blog/44-on-arc-1/">44% on ARC-AGI-1 in 67 cents - Mithil Vakde’s Homepage</a></li>
<li><a href="https://www.youtube.com/watch?v=tEfBCnyg5BQ">Small Transformer Model Beats LLMs on ARC-1 Benchmark Researcher trains small transformer from scratch in 1.5 hours ... A 67-cent transformer beats many LLMs on ARC-AGI-1 I trained a small transformer in 1.5hrs and it beats many ... 44% on ARC-AGI-1 in 67 cents</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#ARC`, `#efficiency`, `#training`, `#AI`

---

<a id="item-tech-news-4"></a>
### [EvoUndo: Framework for Recoverable LLM Agent Self-Evolution](https://www.reddit.com/r/MachineLearning/comments/1w4m0hq/evoundo_recoverabilityconstrained_selfevolution/) ⭐️ 8.0/10

EvoUndo is a new framework for representing, synthesizing, diagnosing, and independently verifying recoverability of LLM agents&\#x27; self-modifications across counterfactual states. In 600 unseen one-shot self-evolution tasks, the authors identified 197 capability-improving mutations that fail recoverability verification; conventional repair strategies recover 0/197, while a deterministic oracle recovers 48/197 under the original recovery language L0 and 191/197 with an extended recovery calculus. A protocol-locked 2x2 intervention showed that exact state-address grounding increases recovery from 0/48 to 38/48 \(79.2%\) when the original language suffices, while extending the language enables 142/143 \(99.3%\) in the oracle-defined S1 stratum. On the primary gpt-oss-120b backbone, adding exact-address diagnostics to the richer language reduces recovery to 133/143 \(93.0%\), and a Qwen3.8-27B replication preserves grounding and expressivity effects but not that negative interaction, indicating model dependence. The results demonstrate that reliable agent self-evolution requires co-designing verification, state grounding, witness semantics, and recovery-language expressivity rather than relying on iterative prompting alone.

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · Sep 1, 19:17

**「Background」** LLM agents increasingly modify their own prompts, tools, middleware, and execution harnesses at runtime to improve capability, a process known as self-evolution. Existing frameworks, such as EvolveR, focus on having agents iteratively refine problem-solving strategies through experience, but they do not address the safety issue that a successful mutation may leave persistent effects that cannot be safely reversed in different states. EvoUndo addresses this gap by introducing a framework for representing, synthesizing, diagnosing, and independently verifying the recoverability of model-generated self-modifications across counterfactual states, as described in the paper arXiv:2608.28363.

**「Impact」** Developers and researchers building LLM agent harnesses should adopt explicit recoverability verification with rich recovery languages and state grounding, since the results show that only a co-designed approach can reliably repair harmful self-modifications that iterative prompting cannot.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.28363">[2608.28363] EvoUndo: Recoverability-Constrained Self-Evolution for LLM Agent Harnesses</a></li>
<li><a href="https://arxiv.org/html/2608.28363">EvoUndo: Recoverability-ConstrainedSelf-Evolution for LLM Agent Harnesses</a></li>
<li><a href="https://arxiv.org/abs/2510.16079">[2510.16079] EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle</a></li>

</ul>
</details>

**Tags**: `#LLM agents`, `#AI safety`, `#self-evolution`, `#recoverability`, `#software engineering`

---

<a id="item-tech-news-5"></a>
### [Virtualizor Update Infrastructure BGP-Hijacked, Root Backdoor Delivered](https://www.virtualizor.com/blog/security-incident-bgp-hijacking/) ⭐️ 8.0/10

Virtualizor&\#x27;s update infrastructure was BGP-hijacked from August 28-30, 2026, allowing attackers to deliver malicious update packages with valid TLS certificates and install a root backdoor on servers that updated during that window. Virtualizor states this was a distribution-chain compromise, not a software code vulnerability, and that only a small number of installations updated during the affected period were impacted. Independent forensics found the malicious packages wrote root SSH keys, installed a Java payload, and established persistence services; AlbaHost reported indicators on 5 of its 34 hypervisors. Softaculous says it currently has no evidence that other products were affected.

telegram · zaihuapd · Sep 1, 06:05

**「Background」** BGP hijacking occurs when attackers corrupt internet routing to redirect traffic destined for a legitimate IP prefix to their own infrastructure. Because the attackers had a valid TLS certificate, their injected update payloads appeared authentic to systems trusting Virtualizor&\#x27;s update channel, making this a supply-chain attack rather than an exploit of a software bug.

**「Impact」** Virtualizor users who applied updates during the hijack window may face full root-level compromise and should treat affected systems as untrusted, rotate credentials, and audit for the reported SSH keys and Java persistence mechanisms.

**Tags**: `#security`, `#supply-chain attack`, `#BGP hijacking`, `#rootkit`, `#Virtualizor`

---

<a id="item-tech-news-6"></a>
### [AnkiDroid Hits Google Play Ban on Open Collective Donation Link](https://github.com/ankidroid/Anki-Android/issues/21656) ⭐️ 7.0/10

AnkiDroid developers reported in GitHub issue \#21656 that Google Play no longer allows their Open Collective donation link in the app. The policy change restricts how the open-source flashcard app can collect donations through its Play listing and reinforces concerns that app stores give a single distributor excessive control over software availability and funding. Commenters noted that Open Collective is a 501\(c\)\(6\) organization and that donations to hosted member projects like AnkiDroid are not tax-deductible, even though the organization is tax-exempt. The episode is being compared to Google&\#x27;s 2019 removal of WireGuard from the Play Store, underscoring ongoing tensions between platform payment policies and open-source sustainability.

hackernews · hexa555 · Sep 1, 10:11 · [Discussion](https://news.ycombinator.com/item?id=49520022)

**「Background」** AnkiDroid, an open-source flashcard app, reported that Google Play no longer allows its Open Collective donation link in the app&\#x27;s store listing. Google Play&\#x27;s policy permits in-app donations only for US foundations with 501\(c\)\(3\) tax-exempt status, but AnkiDroid&\#x27;s fiscal sponsor, Open Collective, operates under 501\(c\)\(6\) status, which is not accepted. This means the app cannot directly present its Open Collective funding page through Google Play, though the underlying donation platform remains available externally.

**「Impact」** AnkiDroid can no longer link its Open Collective donation page from the Google Play listing, which may reduce user donations and set a precedent that restricts how open-source projects solicit funding through Play. Developers of similar projects may need to find alternative donation channels or face removal of such links.

**「Community Discussion」** Commenters see the action as part of a recurring pattern, citing Google&\#x27;s 2019 ejection of WireGuard from the Play Store, and several debate the tax-exempt status of Open Collective donations. Others express gratitude for AnkiDroid and say the news reminds them to donate, while one argues that PWA installation should be easier so apps don&\#x27;t depend on store policies.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ankidroid/Anki-Android/issues/21656">[Community Help Needed] Google Play : no longer allowing our Open ...</a></li>
<li><a href="https://www.drweb.de/google-play-ankidroid-spendenlink/">Warum blockiert Google Play den Spendenlink von AnkiDroid ?</a></li>

</ul>
</details>

**Tags**: `#open source`, `#Google Play`, `#app stores`, `#software funding`, `#policy`

---

<a id="item-tech-news-7"></a>
### [Jujutsu Creator Martin Joins ERSC to Build GitHub Competitor](https://ersc.io/blog/martin-joins-ersc) ⭐️ 7.0/10

Martin, creator of the Jujutsu version control system, has joined ERSC, a startup aiming to compete with GitHub, according to an ERSC blog post shared on Hacker News by Steve Klabnik. Klabnik, who is now working with Martin, said the collaboration has been a pleasure and that more announcements are coming soon. Jujutsu is a Git-compatible VCS with an undo-first command model and a different user experience, which has inspired an active Hacker News thread. The hiring of its creator by a GitHub competitor could signal rising interest in developer-tooling alternatives, though ERSC has not yet disclosed its product roadmap.

hackernews · steveklabnik · Sep 1, 17:46 · [Discussion](https://news.ycombinator.com/item?id=49525297)

**「Background」** Jujutsu \(jj\) is an open-source, Git-compatible version control system created by Martin von Zweigbergk, who began it as a side project in late 2019 and later worked on it full-time at Google. ERSC \(East River Source Control\) is a startup building next-generation version control platforms, aiming to address scalability limits of Git-based remote development and compete with GitHub. The company has now appointed von Zweigbergk as its chief technology officer.

**「Impact」** Developers who are dissatisfied with Git&\#x27;s branching and rebase workflows may see Jujutsu become more tightly integrated into a new GitHub rival, but no concrete ERSC features or dates have been announced yet.

**「Community Discussion」** Commenters are divided: some praise jj&\#x27;s undo capabilities and smarter UX, while others say Git is sufficient for typical workflows and question what concrete value ERSC would offer over GitHub beyond Jujutsu&\#x27;s polish.

<details><summary>References</summary>
<ul>
<li><a href="https://ersc.io/blog/martin-joins-ersc">East River Source Control Names Jujutsu Creator Martin von ...</a></li>
<li><a href="https://zeli.app/story/49525297">Jujutsu Creator Martin von Zweigbergk Joins ERSC as CTO</a></li>

</ul>
</details>

**Tags**: `#jujutsu`, `#version-control`, `#ersc`, `#open-source`, `#developer-tools`

---

<a id="item-tech-news-8"></a>
### [Latent Reasoning in 2026: Mapping Five Families from Coconut to BDH-CQ](https://www.reddit.com/r/MachineLearning/comments/1w4evwo/latent_reasoning_landscape_in_2026_mapping_bdhcq/) ⭐️ 7.0/10

A Reddit analysis by /u/Typical-Scene-5794 maps the 2026 latent reasoning landscape, arguing that progress toward AGI may depend less on ever-longer verbalized chains of thought and more on architectures that reason in continuous or compressed hidden states. The author identifies five families: continuous thoughts in autoregressive LMs \(Coconut, Hao et al., 2024; Soft Thinking, Zhang et al., 2025\), compressed discrete non-linguistic tokens \(Abstract-CoT, Ramji et al., 2026\), recurrent-depth and looped models \(Geiping et al., 2025; Saunshi et al., 2025; Zhu et al., 2026\), task-trained recursive solvers \(HRM, Wang et al., 2025; TRM, Jolicoeur-Martineau, 2025\), and in-context recurrent latent solvers such as BDH-CQ \(Engdahl et al., 2026\) on the Dragon hatchling architecture \(Kosowski et al., 2025\). The post cites Kambhampati \(2025\) to argue that verbalized CoT is an imitation of reasoning because the trace does not track underlying computation, and highlights BDH-CQ&\#x27;s reported cost-accuracy Pareto improvement on public ARC-AGI-1 plus pretraining experiments with transformer-like scaling up to 600B parameters. It closes by asking whether readable CoT traces are a temporary artifact of scaling or a safety property worth an efficiency penalty.

reddit · r/MachineLearning · /u/Typical-Scene-5794 · Sep 1, 15:14

**「Background」** Latent reasoning is an alternative to chain-of-thought \(CoT\) prompting in which a model repeatedly transforms its continuous hidden state and decodes only the final answer, rather than emitting intermediate language tokens. The motivation comes from evidence that verbalized CoT can be flawed or fabricated while still leading to correct answers, suggesting that the token trace is not the actual reasoning mechanism. This matters because latent reasoning may offer efficiency and scaling advantages, but it removes the readable intermediate steps that current interpretability and evaluation tools rely on.

**「Impact」** For researchers building on public benchmarks such as ARC-AGI-1 or scaling latent-reasoning models, the reported BDH-CQ results suggest a possible shift away from CoT legibility, potentially requiring interpretability and evaluation tooling to adapt to opaque hidden-state computation. Because the post is an analysis of arXiv papers rather than a primary benchmark release, these are reported claims rather than independently verified results.

**Tags**: `#latent reasoning`, `#machine learning`, `#continual learning`, `#chain-of-thought`, `#arXiv`

---

<a id="item-tech-news-9"></a>
### [TontaubeV1: Open-Weight 2.9B Character-Level TTS Model](https://www.reddit.com/r/MachineLearning/comments/1w4afjn/we_released_tontaubev1_a_characterlevel_tts_model/) ⭐️ 7.0/10

TontaubeAI released TontaubeV1, an open-weight 2.9B-parameter text-to-speech model focused on expressive speech, long-form generation, and low-latency local inference for English and German. The model uses a character-level tokenization scheme built on Qwen3-1.7B, which the authors found outperformed the original BPE tokenizer by reducing out-of-distribution token sequences and simplifying character-to-sound mapping. It also employs a chunking and position scheme with separate logical position IDs for text and audio, keeping context bounded for very long passages while enabling streaming via overlapping DualCodec windows re-encoded into the VibeVoice acoustic space. TontaubeV1 supports zero-shot voice cloning from up to one minute of reference audio, was trained on 7 languages and roughly 200k hours of audio, and achieved 50.1% preference against ElevenLabs Flash v2.5 on a 400-passage LLM-as-a-judge audiobook benchmark, with human listening tests still considered the gold standard. The current release requires a GPU with at least 24 GB of VRAM for low-VRAM and balanced profiles or 32 GB for high-throughput, with quantized and fine-tuning support planned.

reddit · r/MachineLearning · /u/EAVDR · Sep 1, 12:23

**「Background」** Modern LLM-based TTS models often treat speech generation as next-token prediction, using the backbone LLM&\#x27;s tokenizer along with special audio tokens from a discrete audio codec. TontaubeV1 instead forces character-level tokenization of spoken text and uses a multi-codebook codec called DualCodec, combined with a position scheme that aligns text and audio timelines across chunks, to handle long-form narration and low-latency streaming without simple concatenation artifacts.

**「Impact」** Developers and researchers working on open TTS systems gain a permissively released 2.9B model with strong prosody results in English and German, though practical deployment is currently limited to GPUs with at least 24 GB VRAM until planned quantized versions arrive.

**Tags**: `#text-to-speech`, `#open-source`, `#machine-learning`, `#audio`, `#LLM`

---

<a id="item-tech-news-10"></a>
### [China&\#x27;s Solar Capacity Overtakes Coal to Become Largest Power Source](https://content-static.cctvnews.cctv.com/) ⭐️ 7.0/10

CCTV reports that as of July 2026, China&\#x27;s solar photovoltaic installed capacity reached 1.286 billion kilowatts, surpassing coal for the first time and becoming the country&\#x27;s largest power source, with solar accounting for 31.5% of total installed capacity. From January to July 2026, PV generation exceeded 802.4 terawatt-hours, a 15.5% year-on-year increase, equivalent to about 1 of every 8 kilowatt-hours of electricity coming from solar. The report also notes that 8 of 10 PV modules worldwide are made in China, and the industry expects over 2 trillion yuan in investment over the next five years. These figures are dated after the current date and could not be independently verified at the time of reporting.

telegram · zaihuapd · Sep 1, 02:42

**「Background」** Installed capacity measures a power plant&\#x27;s maximum possible output, not the amount of electricity it actually generates; coal has historically been China&\#x27;s dominant power source by this measure. The National Energy Administration announced that China&\#x27;s installed photovoltaic capacity surpassed coal-fired capacity for the first time, making solar the country&\#x27;s largest power source by installed capacity. This milestone reflects solar power&\#x27;s rapid expansion, but it does not by itself prove that solar generated more electricity than coal.

**「Impact」** If confirmed, the milestone would make solar the dominant installed power source in the world&\#x27;s largest electricity market, reinforcing China&\#x27;s industrial leadership in solar manufacturing and potentially accelerating the global energy transition.

<details><summary>References</summary>
<ul>
<li><a href="https://english.dbw.cn/system/2026/09/01/001566414.shtml">China &#x27;s photovoltaic power capacity overtakes coal -fired power for...</a></li>
<li><a href="https://www.globaltimes.cn/page/202609/1369526.shtml">China ’s installed solar power generating capacity surpasses coal ...</a></li>

</ul>
</details>

**Tags**: `#solar energy`, `#China`, `#energy transition`, `#photovoltaics`, `#technology industry`

---

<a id="item-tech-news-11"></a>
### [Google to Release Gemini 3.8 Flash, Coding Edge Reportedly Narrows Gap](https://www.wsj.com/tech/ai/new-google-ai-model-said-to-narrow-gap-on-coding-ability-264c6052) ⭐️ 7.0/10

Google DeepMind is reportedly planning to release a new model called Gemini 3.8 Flash, internally codenamed Skimaki, as early as this Wednesday. The model is said to deliver a significant upgrade in coding ability, with engineers in internal comparisons using the Jetski programming tool reportedly preferring it over Anthropic&\#x27;s Opus model. This could help close the gap Google has faced against OpenAI and Anthropic in coding performance. The information comes from insider sources cited by The Wall Street Journal, so the details are not yet officially confirmed.

telegram · zaihuapd · Sep 2, 00:35

**「Background」** Google&\#x27;s Gemini family includes Flash variants designed to be smaller and faster than the flagship models, focusing on efficiency and lower latency. In recent coding benchmarks and developer evaluations, Google&\#x27;s models have generally trailed those from OpenAI and Anthropic, making coding capability a key competitive battleground.

**「Impact」** If the internal preference holds up publicly, Gemini 3.8 Flash could become a competitive option for developers using AI coding assistants, potentially challenging the current market leaders.

**Tags**: `#artificial intelligence`, `#Google`, `#Gemini`, `#coding`, `#machine learning`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Asian Spot LNG Prices Hit 5-Month High as Hormuz Blockage Persists](https://oilprice.com/Latest-Energy-News/World-News/Asia-Spot-LNG-Prices-Hit-5-Month-High-as-Hormuz-Blockage-Drags-On.html) ⭐️ 9.0/10

Asian spot LNG prices hit a five-month high of $24.614 per million British thermal units \(MMBtu\) on Tuesday, up from $23.388 on Friday, as stalled LNG traffic through the Strait of Hormuz and U.S.-Iran hostilities tightened supply, according to traders.

rss · OilPrice.com · Sep 1, 15:30

**「Background」** QatarEnergy extended force majeure on its LNG deliveries into November because of blocked Hormuz transits, and the U.S. and Iran exchanged fire for the first time in more than a month.

**「Impact」** Buyers in Pakistan, Bangladesh, South Korea, India, and Taiwan are seeking spot cargoes for October and November to replace Qatari term supply that cannot leave the Persian Gulf.

**Tags**: `#LNG`, `#Energy Prices`, `#Strait of Hormuz`, `#Geopolitics`, `#Natural Gas`

---

<a id="item-finance-news-2"></a>
### [U.S. and Iran Trade Strikes, Pushing Middle East Oil Benchmarks Above $100](https://finance.yahoo.com/video/us-iran-exchange-strikes-renewing-194217817.html) ⭐️ 9.0/10

The U.S. and Iran exchanged direct strikes, reigniting fears of a prolonged Middle East conflict and pushing Middle Eastern oil benchmarks above $100 per barrel, while ICE Brent traded around $92.

openbb · CL=F · Sep 1, 19:42

**「Background」** The escalation follows a month of direct U.S.-Iran attacks and Washington&\#x27;s sanctions on Tehran, which have made transits through the Strait of Hormuz more difficult; two very large crude carriers carrying Saudi oil were hit by projectiles while exiting the strait.

**「Impact」** The renewed conflict adds to inflation worries that have pushed global bond yields to their highest since 2008, raising borrowing costs for households and companies and potentially slowing spending on vehicles, air travel, and manufacturing.

**Tags**: `#oil prices`, `#geopolitics`, `#Iran`, `#US foreign policy`, `#energy markets`

---

<a id="item-finance-news-3"></a>
### [Federal Reserve holds interest rates steady](https://news.google.com/rss/articles/CBMipAFBVV95cUxOY1hWQlVSY2RxeHd1dGdaVHQ0RWFHWXVOWWdNTmhuNktNVVc2bGE1S29PbW95dHd6Ml9Da05XTEpzNW92aVFEdlY1MUVPaTBtaV9ENDhxNjFYU0FQcFRXZ0Y4TllqYXdOckd3VjhrM0hjWGJjWEJUcy1fOWFibENaNVdHcnNKaDhERE9lTTYyNTExczZWcXFkbjFURUpmMEFldzRMbA?oc=5) ⭐️ 9.0/10

The Federal Reserve left its benchmark interest rate unchanged at its latest policy meeting, pausing after a period of rate moves.

google\_news · Spectrum News · Jul 29, 07:00

**「Background」** The Federal Reserve kept its benchmark interest rate in a range of 3.5% to 3.75% at its June 16–17, 2026 meeting, the first policy decision under new Chair Kevin Warsh. The hold comes amid heightened inflationary pressures on the U.S. economy, including recent oil price spikes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-holds-interest-rates-steady-220059911.html?fr=sycsrp_catchall">Federal Reserve Holds Interest Rates Steady At 3.5%-3.75% In ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`

---

<a id="item-finance-news-4"></a>
### [Fed&\#x27;s Barr says he would support rate hike if inflation doesn&\#x27;t ease](https://www.cnbc.com/2026/09/01/fed-governor-barr-says-hell-support-rate-hike-if-inflation-doesnt-ease.html) ⭐️ 8.0/10

Federal Reserve Governor Michael Barr said Tuesday he would back an interest rate hike if inflation does not moderate, noting inflation is running at 3.7% over the past year, above the Fed&\#x27;s 2% target.

rss · CNBC Finance · Sep 1, 14:01

**「Background」** Barr is a permanent voting member of the Federal Open Market Committee, which held its benchmark rate at 3.5%-3.75% in July; markets now price about a 66% chance of a hike at the next meeting in two weeks after Chair Kevin Warsh&\#x27;s hawkish remarks.

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Monetary Policy`, `#Michael Barr`

---

<a id="item-finance-news-5"></a>
### [Saudi Arabia Plans to Cut Domestic Oil Use by 1 Million b/d by 2030](https://oilprice.com/Alternative-Energy/Nuclear-Power/Saudi-Arabia-Plans-To-Free-1-Mbd-As-it-Invests-in-Nuclear-Power.html) ⭐️ 8.0/10

Saudi Arabia aims to displace more than 1 million barrels per day \(b/d\) of domestic oil use by 2030, relying mainly on natural gas and renewables; nuclear is unlikely to contribute materially to that target by 2030. A 30-year U.S.-Saudi civil nuclear cooperation agreement signed on July 22 could support nuclear power after 2030.

rss · OilPrice.com · Sep 2, 00:00

**「Background」** The plan comes as the International Energy Agency estimates Saudi electricity demand grew 3.8% in 2025 and forecasts average annual growth of 3.1% through 2030.

**「Impact」** If achieved, the displacement could free oil currently burned domestically for export or other uses, potentially adding more Saudi supply to global oil markets.

**Tags**: `#Saudi Arabia`, `#Nuclear Power`, `#Oil Displacement`, `#Energy Policy`, `#US-Saudi Agreement`

---

<a id="item-finance-news-6"></a>
### [Lithium Prices Surge as LG Signs 10-Year U.S. Supply Deal](https://oilprice.com/Energy/Energy-General/US-Lithium-Miners-Finally-Have-a-Shot-at-Cashing-In.html) ⭐️ 8.0/10

Lithium prices are climbing: China’s closely watched spot price for the battery material rose 22% in the first half of 2026, according to Bloomberg. Meanwhile, LG Energy Solution signed a ten-year deal to buy 8,000 tons per year of battery-grade lithium carbonate from Smackover Lithium starting in 2029.

rss · OilPrice.com · Sep 1, 20:00

**「Background」** Most of the world’s refined lithium is controlled by China, Chile and Argentina, and the U.S. has long struggled to build domestic supply because volatile prices deterred investment.

**「Impact」** The deal could help U.S. lithium miners win a bigger share of global battery supply chains, but analysts at UBS and Jefferies warn that faster supply growth from 2027 may pressure prices.

**Tags**: `#lithium`, `#energy storage`, `#supply chain`, `#mining`, `#battery materials`

---

<a id="item-finance-news-7"></a>
### [Tanzania’s Mining Reforms Show Payoff With Record Gold Exports](https://oilprice.com/Energy/Energy-General/Tanzanias-Mining-Model-Is-Starting-to-Pay-Off.html) ⭐️ 8.0/10

Tanzania’s overhauled mining regime is showing results: mining-related tax and royalty revenue has more than doubled since 2021, and gold exports rose 38.2% last year to a record $4.7 billion.

rss · OilPrice.com · Sep 1, 17:00

**「Background」** Since 2017, Tanzania has rewritten its Mining Act, giving the government a 16% non-dilutive, free-carried interest in large-scale mining licenses and requiring Tanzanian firms to hold minimum equity stakes.

**「Impact」** The reforms have attracted roughly $3.3 billion in private mining investment over four years, and mining’s share of Tanzania’s GDP passed 10% for the first time.

**Tags**: `#Tanzania`, `#mining`, `#critical minerals`, `#gold exports`, `#mining policy`

---

<a id="item-finance-news-8"></a>
### [UK Shop Prices Hit Two-Year High as Food Inflation Jumps](https://oilprice.com/Energy/Energy-General/Food-Inflation-Jumps-as-Higher-Energy-Costs-Hit-UK-Retailers.html) ⭐️ 8.0/10

UK shop price inflation hit a two-year high in the year to August, rising to 1.5 percent from 0.9 percent in July, as the BRC said higher energy and commodity costs are filtering through; food inflation rose to 2.8 percent from 2.2 percent.

rss · OilPrice.com · Sep 1, 16:00

**「Background」** The British Retail Consortium \(BRC\) publishes the shop price index on behalf of major UK retailers; food price inflation had been on a downward trend for most of 2026 before this jump.

**「Impact」** The BRC warned the months ahead look challenging for households, and the Bank of England has said inflation could top 4 percent and lead to interest-rate hikes if the Strait of Hormuz stays closed, raising borrowing costs.

**Tags**: `#UK inflation`, `#food prices`, `#energy costs`, `#retail`, `#Bank of England`

---

<a id="item-finance-news-9"></a>
### [U.S. Energy Storage Installations Set Record in Q2 2026](https://oilprice.com/Latest-Energy-News/World-News/US-Energy-Storage-Capacity-Installations-Hit-Record-High-in-Q2.html) ⭐️ 8.0/10

U.S. energy storage installations hit a record 20.2 GWh in Q2 2026, bringing first-half 2026 total installations to 30.8 GWh, according to SEIA and Benchmark Mineral Intelligence, which also raised their 2030 installation forecast by 11.5%.

rss · OilPrice.com · Sep 1, 14:30

**「Background」** Utility-scale projects drove the surge with 18 GWh installed, including a record 6.2 GWh in Arizona, as grid operators and utilities turned to storage to improve reliability and meet rising power demand from data centers.

**「Impact」** The additions already contribute to power supply: battery storage delivered more electricity to the U.S. grid in the first eight months of 2026 than in all of 2025.

**Tags**: `#energy storage`, `#grid reliability`, `#utility-scale`, `#U.S. market`, `#renewable energy`

---

<a id="item-finance-news-10"></a>
### [Japan Relaxes Enforcement of Monthly Overtime Cap](https://www.orientaldaily.com.my/news/international/2026/09/01/844683) ⭐️ 8.0/10

Japan began easing overtime rules on September 1, when labor standards inspectors stopped enforcing the monthly 45-hour overtime cap; about 40% of Japanese companies now allow up to 100 overtime hours per month.

telegram · zaihuapd · Sep 1, 12:56

**「Background」** The policy comes from a growth strategy adopted by Prime Minister Takaichi Sanae&\#x27;s government in July, and critics say it reverses earlier work-style reform.

**「Impact」** Officials warn that exceeding 45 hours raises the risk of karoshi \(death from overwork\), posing a potential risk to workers at companies that allow the higher limit.

**Tags**: `#Japan labor policy`, `#overtime regulation`, `#economic stimulus`, `#workplace reform`, `#labor market`

---

<a id="item-finance-news-11"></a>
### [TSMC&\#x27;s $269 Billion Expansion Highlights Its Strong Margin](https://finance.yahoo.com/markets/stocks/articles/tsmcs-269-billion-expansion-puts-170918317.html) ⭐️ 8.0/10

TSMC is planning a $269 billion expansion, putting focus on its 67.7% margin and its strategic importance to the global semiconductor market.

openbb · NVDA · Sep 1, 17:09

**「Background」** The 67.7% gross margin came from TSMC&\#x27;s Q2 2026 results, where net profit rose 77.4% year over year and margins exceeded the company&\#x27;s own guidance; TSMC also raised its capital expenditure guidance to as much as $64 billion while expanding facilities in Arizona and Germany.

**「Impact」** The additional U.S. fabs for 2nm and advanced packaging are set to increase advanced chipmaking capacity, directly affecting semiconductor supply chains and companies that rely on leading-edge chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/9062197/tsmcs-269-billion-expansion-puts-its-677-margin-in-focus">TSMC&#x27;s $269 Billion Expansion Puts Its 67.7% Margin in Focus</a></li>
<li><a href="https://xenospectrum.com/en/tsmc-q2-2026-record-margin-capex/">TSMC Posts 77% Profit Growth with 67.7% Gross Margin: Capex ...</a></li>
<li><a href="https://www.semiconreport.org/en/articles/tsmc-100-billion-us-chipmaking-expansion">TSMC&#x27;s $100 Billion US Expansion: In-depth Analysis of ...</a></li>
<li><a href="https://www.semiconreport.org/en/articles/tsmc-100-billion-usa-chipmaking-expansion">TSMC invests another $100 billion to expand production in the ...</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductors`, `#capital expenditure`, `#margins`, `#expansion`

---

<a id="item-finance-news-12"></a>
### [Fed may hold rates after cooler inflation data](https://news.google.com/rss/articles/CBMisAFBVV95cUxQbDJaOWp0UVZZRVd3MUp5UGNUVk1EOXNybWFfeXRKR2FQYzJsUnJCN3VEU1I2bldJWHFodHlUWXQxcUdzXzVtaTN4RmEyaHlwREhvdVpialZycTYyaFozME5kWWV3MGFqT1hGS00zTnMyQmVDZkZXZTFvT0VGR0RSMU1FMnBiT3dyZFlSQmx5RDRXX0JsZ1dPMy1KOTNteGVOaVJRemdUaDhtWkpmRndEeQ?oc=5) ⭐️ 8.0/10

Reuters reports that softer inflation data may lead the Federal Reserve, under Kevin Warsh, to keep interest rates unchanged despite divisions among policymakers.

google\_news · Reuters · Aug 14, 07:00

**「Background」** Fed Chair Kevin Warsh has previously said inflation remains too high and hinted that interest rates might need to rise unless price growth slows. Newly cooler inflation data could now support holding rates steady instead.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/28/kevin-warsh-jackson-hole-federal-reserve-inflation.html">Fed Chairman Warsh warns on inflation at Jackson Hole - CNBC</a></li>
<li><a href="https://www.npr.org/2026/08/28/nx-s1-5947903/federal-reserve-inflation-jackson-hole-interest-rates">Fed Chair Kevin Warsh warns inflation is still too high : NPR</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Monetary Policy`, `#Economy`

---

<a id="item-finance-news-13"></a>
### [Fed Leaves Interest Rates Unchanged; Powell Holds News Briefing](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 8.0/10

The Federal Reserve left its benchmark interest rate unchanged, and Chair Jerome Powell held a news briefing after the decision. Powell&\#x27;s remarks are the central bank&\#x27;s latest public guidance on its monetary policy stance.

google\_news · pbs.org · Mar 18, 07:00

**「Background」** In its latest policy decision, the Federal Reserve held its benchmark interest rate at about 3.6% for a second straight meeting, after cutting it three times last year. Chair Jerome Powell’s briefing explains that decision.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-powell-holds-news-briefing-after-latest-interest-rate-decision">WATCH: Fed Chair Powell holds news briefing after interest rate left unchanged | PBS News</a></li>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-powell-holds-news-conference-on-interest-rate-decision">WATCH: Powell holds news conference after Federal Reserve leaves interest rate unchanged | PBS News</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Jerome Powell`, `#Press Conference`

---

<a id="item-finance-news-14"></a>
### [Qualcomm Announces Double-Digit Chip Price Increases From September 1](https://www.macrumors.com/2026/08/31/qualcomm-chip-price-increase/) ⭐️ 7.0/10

Qualcomm said it will raise prices by double digits for all chips shipped after September 1, 2026, with the exact increase negotiated per customer, citing rising supplier costs it can no longer absorb. Apple still buys Qualcomm modem chips for the iPhone 17 series.

telegram · zaihuapd · Sep 1, 04:10

**「Background」** Qualcomm supplies processors and modem chips to smartphone makers; a modem chip handles cellular connections. The price increase applies to the company&\#x27;s full product lineup.

**「Impact」** The price rise could raise component costs for smartphone makers such as Apple, which uses Qualcomm modems in the iPhone 17.

**Tags**: `#Qualcomm`, `#semiconductor pricing`, `#supply chain`, `#Apple`, `#chip costs`

---

<a id="item-finance-news-15"></a>
### [China’s First Micro-Short-Drama Regulation Takes Effect](https://content-static.cctvnews.cctv.com/snow-book/index.html?item_id=13099489542770738243) ⭐️ 7.0/10

China’s first departmental regulation specifically for micro short dramas took effect today, establishing a three-tier classification review system based on investment size and genre, and requiring AI-generated episodes to display a visible label in each episode.

telegram · zaihuapd · Sep 1, 05:19

**「Background」** China&\#x27;s National Radio and Television Administration issued the Management Measures for Micro Short Dramas on July 31, 2026, and they took effect September 1, 2026. It is the country&\#x27;s first formal departmental regulation for micro short dramas, replacing earlier notifications and regulatory notices, and introduces a three-tier classification review based on investment size and subject matter plus AI-content labeling.

**「Impact」** Producers and distribution platforms of micro short dramas in China now face tiered filing and approval requirements, while AI-assisted works must carry a clear notice to viewers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nrta.gov.cn/art/2026/7/31/art_113_73785.html">国家广播电视总局 公告公示 国家广播电视总局令第16号：《微短剧发展管理办法》</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33691660">广电总局重磅发布!《微短剧发展管理办法》来了!AI剧纳入监管!9月实施!_澎湃号·湃客_澎湃新闻-The Paper</a></li>
<li><a href="https://www.news.cn/legal/20260731/4b8eea40226644d0a347c72ea1b21b75/c.html">9月1日起，《微短剧发展管理办法》正式施行 - 新华网</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#micro-short-dramas`, `#China`, `#AI-content-labeling`, `#media-industry`

---

<a id="item-finance-news-16"></a>
### [China Issues Guidelines on Overseas Competition and Compliance for Automakers](https://weibo.com/1664176597/Rg5PKzXXE) ⭐️ 7.0/10

China’s Ministry of Commerce, Ministry of Industry and Information Technology, and State Administration for Market Regulation jointly issued the Guidelines on Overseas Competition Behavior and Compliance for the Automotive Industry, telling automakers to base export prices on costs and international supply and demand while avoiding unfair practices such as low-price dumping. The guidelines are a policy directive rather than a mandatory regulation.

telegram · zaihuapd · Sep 1, 08:15

**「Background」** The guidelines are a non-binding reference document from China&\#x27;s Ministry of Commerce, Ministry of Industry and Information Technology, and State Administration for Market Regulation, issued to help Chinese carmakers follow fair competition and compliance practices in overseas markets.

**「Impact」** Chinese automakers selling overseas will face clearer compliance expectations on pricing, marketing, and local supply-chain cooperation, which may prompt them to adjust export strategies to avoid unfair-competition findings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stcn.com/article/detail/4167297.html">三部门发布《汽车行业境外竞争行为与合规建设指引》</a></li>
<li><a href="https://www.bjnews.com.cn/detail/1788246415129046.html">三部门发布《汽车行业境外竞争行为与合规建设指引》 — 新京报</a></li>
<li><a href="https://cn.investing.com/news/stock-market-news/article-3546202">三部门发布《汽车行业境外竞争行为与合规建设指引》 提供者 智通财经</a></li>
<li><a href="https://www.ithome.com/0/996/965.htm">ithome.com/0/996/965.htm</a></li>
<li><a href="https://news.smm.cn/news/104091526">news.smm.cn/news/104091526</a></li>
<li><a href="https://www.news.cn/fortune/20260901/b55704c5d68c4a72af88fb675de2efcb/c.html">三部门发布《 汽 车 行 业 境 外 竞 争 行 为 与 合 规 建设 指 引 》-新华网</a></li>

</ul>
</details>

**Tags**: `#汽车行业`, `#境外合规`, `#产业政策`, `#反倾销`, `#商务部`

---

<a id="item-finance-news-17"></a>
### [China imposes 20% dividend tax on foreign individuals from 2026](https://m.cnfin.com/wx/share?url=//m.cnfin.com/yw-lb//zixun/20260901/4463424_1.html) ⭐️ 7.0/10

China’s Ministry of Finance and State Taxation Administration said foreign individuals must pay 20% individual income tax on dividends they receive from foreign-invested enterprises, effective September 1, 2026. The rule replaces a previous exemption.

telegram · zaihuapd · Sep 1, 09:33

**「Background」** Since 1994, Finance Ministry document Cai Shui Zi \[1994\] No. 20 had temporarily exempted foreign individuals from individual income tax on dividends received from foreign-invested enterprises. The new announcement ends that longstanding exemption and replaces the relevant clause.

**「Impact」** Foreign shareholders of foreign-invested enterprises in China will receive lower net dividend payments from September 2026, because these enterprises must withhold the 20% tax from distributions.

<details><summary>References</summary>
<ul>
<li><a href="https://tg.okhk.net/posts/11131">tg.okhk.net/posts/11131</a></li>

</ul>
</details>

**Tags**: `#China tax policy`, `#dividend tax`, `#foreign individuals`, `#personal income tax`, `#foreign-invested enterprises`

---