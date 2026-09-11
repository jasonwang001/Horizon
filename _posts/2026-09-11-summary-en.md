---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 247 items, 21 important content pieces were selected

---

**Technology News**
1. [Shopify moves from React Native to Swift and Kotlin](#item-tech-news-1) ⭐️ 8.0/10
2. [Microsoft Recognizes Rust as a Tier-1 Language](#item-tech-news-2) ⭐️ 8.0/10
3. [Calif Research says AI helped build WeChat zero-click worm](#item-tech-news-3) ⭐️ 8.0/10
4. [trynix.dev runs any Nix package in a browser via qemu-wasm](#item-tech-news-4) ⭐️ 7.0/10
5. [Real fly connectome fails to learn Pong; synapse-level audit explains why](#item-tech-news-5) ⭐️ 7.0/10
6. [Ant International, Visa, Mastercard to Build AI-Agent Payment Standards](#item-tech-news-6) ⭐️ 7.0/10
7. [Tencent Hunyuan releases open-source AuK audio editing model and AuK-Flash](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [IEA Projects Record Global Coal Demand in 2026 as LNG Prices Rise](#item-finance-news-1) ⭐️ 8.0/10
2. [Fed holds interest rates steady in a 9-3 vote](#item-finance-news-2) ⭐️ 8.0/10
3. [Kalshi Launches CFTC-Approved Gold and Silver Perpetual Futures in the U.S.](#item-finance-news-3) ⭐️ 7.0/10
4. [U.S. Pledges $3 Billion for Critical Minerals as China&\#x27;s Lead Persists](#item-finance-news-4) ⭐️ 7.0/10
5. [Mexico Plans to Cut Pemex Support by About 70% Next Year](#item-finance-news-5) ⭐️ 7.0/10
6. [EIA Projects Record US Natural Gas Output and LNG Exports Through 2027](#item-finance-news-6) ⭐️ 7.0/10
7. [Permian Gas Benchmark Waha Turns Negative for 118 Days This Year](#item-finance-news-7) ⭐️ 7.0/10
8. [印度严重欺诈调查局建议详查小米在印业务](#item-finance-news-8) ⭐️ 7.0/10
9. [Chinese AI chipmakers raise prices as HBM shortage bites](#item-finance-news-9) ⭐️ 7.0/10
10. [TSMC Stock Slips Despite 53% August Revenue Growth](#item-finance-news-10) ⭐️ 7.0/10
11. [TSMC September Revenue Reportedly Jumps 53%](#item-finance-news-11) ⭐️ 7.0/10
12. [OpenAI Picks Broadcom for First Custom AI Chip](#item-finance-news-12) ⭐️ 7.0/10
13. [Trump Reportedly Voices No Regrets on Iran War as Oil Tops $100](#item-finance-news-13) ⭐️ 7.0/10
14. [Bond Selloff Pushes 10-Year Treasury Yield Near 5%](#item-finance-news-14) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Shopify moves from React Native to Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify Engineering has detailed its migration from React Native back to native Swift and Kotlin, according to the post and the accompanying Hacker News discussion. The shift is notable because it comes from a major commerce platform and reverses a previously cross-platform approach, making it a high-profile data point in the long-running native-versus-cross-platform mobile debate. The discussion covers LLM-assisted migration, native performance and maintenance tradeoffs, and the strategic value of dedicated iOS and Android engineers. In the thread, some iOS engineers said the move validated their skepticism about shared codebases, while others described similar React Native-to-native migrations. The post&\#x27;s author, fnthawar2, said LLMs changed a core assumption behind Shopify&\#x27;s 2020 decision, prompting reevaluation rather than sticking with a past successful choice.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**「Background」** React Native is a cross-platform framework that lets companies share one mobile codebase across iOS and Android, and Shopify had relied on it for its mobile apps following an earlier 2020 decision. Shopify now says coding agents changed the economics of mobile development, making separate native Swift and Kotlin apps more attractive than maintaining a shared React Native codebase. According to Shopify, its Shop app was migrated from React Native to Swift and Kotlin, going from proof-of-concept to publishing in 12 weeks with AI assistance, and the company is moving its other mobile apps in the same direction.

**「Impact」** For teams evaluating mobile architecture, Shopify&\#x27;s reversal provides a concrete example of a major company moving away from React Native and reconsidering native development, especially as LLM-assisted migration is debated as a cost-lowering factor. The community discussion suggests that the extent to which LLMs actually enabled the migration remains contested.

**「Community Discussion」** Commenters broadly debated native versus cross-platform development: some iOS engineers felt validated by Shopify&\#x27;s move, while others described their own React Native-to-native migrations, and at least one disputed that LLMs were the key enabler. Another commenter reported rapid LLM-assisted progress on a smaller app, while the Shopify author responded that LLMs changed a core assumption behind the company&\#x27;s 2020 decision.

<details><summary>References</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://shopify.engineering/shop-app-migration">Migrating Shop app from React Native to native (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding Agents Made It Cheaper to Build Twice Than to Share One Codebase. - DEV Community</a></li>

</ul>
</details>

**Tags**: `#React Native`, `#mobile development`, `#Swift/Kotlin`, `#engineering strategy`, `#LLM-assisted migration`

---

<a id="item-tech-news-2"></a>
### [Microsoft Recognizes Rust as a Tier-1 Language](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

A guest post published by the Rust Foundation states that Rust is a tier-1 language at Microsoft, framing the designation as an industry adoption milestone for systems programming and open-source ecosystems. The item is a foundation guest post rather than a primary Microsoft engineering announcement, and the supplied material includes no source content describing Microsoft&\#x27;s tiering criteria, affected products, or migration timeline. The announcement drew substantial Hacker News engagement: 590 points and 331 comments, according to the analysis summary. Its significance lies in Microsoft&\#x27;s long-standing role in C and C++ tooling and in Rust&\#x27;s memory-safety guarantees, though the practical scope of the tier-1 designation remains unspecified in the available material.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**「Background」** Rust 1.0, the first stable release, arrived in May 2015, and the language has been sponsored by the Rust Foundation since February 2021. Microsoft&\#x27;s designation of Rust as a tier-1 language means it is treated as a first-class option in production engineering workflows, even though C++ remains dominant at the company after decades of use. The Rust Foundation guest post frames this shift as part of native platform evolution for both Rust and C++.

**「Impact」** For Microsoft engineers and Rust developers targeting Windows, the tier-1 designation points to sustained investment across tooling, quality, security, platform integration, production deployment, and long-term support, with repository rollouts continuing weekly as more teams adopt it.

**「Community Discussion」** Commenters broadly welcomed the news as evidence that Rust is mature enough to compete with C++ and C\#, with one five-year professional Rust developer saying they see no technical use case for another language in high-level application development. Others highlighted related efforts and rumors, including a cited Microsoft goal to convert 1 billion lines of code to Rust by 2030, DARPA-funded C-to-Rust conversion work, and unconfirmed MSVC integration news, while noting Rust&\#x27;s memory-safety advantage for reducing CVEs in large Microsoft product portfolios.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rust_%28programming_language%29">Rust (programming language ) - Wikipedia</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post : Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Microsoft`, `#programming languages`, `#open source`, `#systems programming`

---

<a id="item-tech-news-3"></a>
### [Calif Research says AI helped build WeChat zero-click worm](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 8.0/10

Calif Research released a demo of WeWorm, which it describes as the first zero-click worm to spread through WeChat calls across iOS and Android. The victim does not need to answer the call or interact with the phone at all, and even if they answer, they hear nothing while the exploit still succeeds. Calif Research says that working with AI, its team found the bug and wrote the first remote code execution \(RCE\) exploit in about two days, then built the worm in one more week. It claims a worm at this scale used to take a larger team months, and that AI can already do most of the work while the team provided judgment about what to target and how to test safely. These claims are unverified in the supplied content, which offers no technical detail, methodology, or independent verification.

rss · Simon Willison · Sep 10, 00:56

**「Background」** A zero-click exploit compromises a target with no user interaction, and a worm is malicious code that self-propagates; in this case WeChat calls are the vector, so a victim need not answer for their account to be hijacked and used to call contacts. Calif Research says it discovered and weaponized the flaw and privately reported it to Tencent, warning the attack path could affect over a billion phones or accounts. The claimed novelty is speed of development: AI assistance reportedly helped compress bug discovery and the first RCE exploit to about two days and the worm build to one additional week, work that Calif says previously required a larger team and months.

**「Impact」** The claim, if independently confirmed, would indicate that AI-assisted development can sharply lower the time and team size required for zero-click RCE exploits and cross-platform worms affecting WeChat users on iOS and Android.

<details><summary>References</summary>
<ul>
<li><a href="https://calif.io/research/weworm">WeWorm | Calif</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://blog.calif.io/p/weworm">WeWorm</a></li>

</ul>
</details>

**Tags**: `#ai-security-research`, `#exploit-development`, `#zero-click-worm`, `#llm-assisted-coding`, `#wechat`

---

<a id="item-tech-news-4"></a>
### [trynix.dev runs any Nix package in a browser via qemu-wasm](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 7.0/10

Farid Zakaria has launched trynix.dev, which he calls his &quot;magnum opus&quot; of Nix work. The site provides a qemu-wasm-powered x86\_64 Linux virtual machine that runs entirely in the browser through WebAssembly and can boot any Nix package from the past 13 years. Packages are URL-addressable: visiting https://trynix.dev/?pkg=python3%403.6.2 and clicking &quot;Load&quot; opens an interactive shell in a VM running Python 3.6.2 from 2017. Zakaria also introduced the trynix-preview GitHub Action, which comments a link on a pull request so the PR&\#x27;s build can be booted in the browser; its description says &quot;No servers, just browsers.&quot;

rss · Simon Willison · Sep 10, 23:44

**「Background」** Nix is a package manager whose nixpkgs collection pins each package together with its full dependency closure, and Nix binary caches serve those prebuilt artifacts over plain HTTP, which is what makes historical packages addressable years later. QEMU-WASM is a patched QEMU whose TCG just-in-time compiler backend translates IR into WebAssembly, relying on browser APIs such as WebAssembly.Module and WebAssembly.Instance to execute a full x86\_64 Linux guest inside a browser tab without a server. trynix.dev combines the two: an in-memory Nix store holds the package closure downloaded from the binary caches, and a Ghostty terminal emulator supplies the interactive shell interface.

**「Impact」** For Nix users and maintainers, trynix.dev makes specific package versions and pull-request builds shareable as browser-bootable URLs, while trynix-preview lets reviewers open a PR build in a browser without local Nix setup or hosted servers.

<details><summary>References</summary>
<ul>
<li><a href="https://trynix.dev/">trynix</a></li>
<li><a href="https://techaiwire.com/articles/trynix-nix-packages-in-browser-wasm/">TryNix runs Nix packages in your browser - techaiwire.com</a></li>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>

</ul>
</details>

**Tags**: `#Nix`, `#WebAssembly`, `#QEMU`, `#reproducible builds`, `#browser VMs`

---

<a id="item-tech-news-5"></a>
### [Real fly connectome fails to learn Pong; synapse-level audit explains why](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

A Reddit author reports that a subgraph of the real MaleCNS v1.0 fly connectome \(166k neurons from EM reconstruction\) failed to learn Pong using dopamine-style plasticity and a per-frame binary hit-or-miss signal. An audit of the failure uncovered a neuPrint regex bug—full-match versus substring semantics—that silently zeroed out two neuron populations, and showed the original neuron selection had no path from photoreceptors to anything else because real photoreceptors do not synapse directly onto motion detectors and a whole intermediate layer was missing. After rebuilding a working pipeline, learning-on and learning-off runs produced bit-for-bit identical results across multiple seeds even though weights were verifiably changing, traced to half of the four available motor neurons having zero synapses from any sensory pathway in the model; those neurons had been assigned to the &\#x27;paddle down&\#x27; group by array index and could never fire. A rebuilt circuit based on a courtship-pursuit visual tracking hypothesis was refuted by data, but a different descending neuron connected end to end and produced the first divergence between learning-on and learning-off, though the effect appeared to quiet the whole system rather than improve skill because misses outnumbered hits so punishment dominated and shrank the motor response. The author also notes that larger viral projects had not solved this: the Doom project&\#x27;s repo says it failed its own validation gates after six iterations, the Minecraft mod&\#x27;s limitations section admits the real motion-detection pathway stays silent with escape and foraging behaviors hand-injected or reflex-layer fallbacks, and the Beat Saber creator&\#x27;s replies admit overfitting to one track with replay data mixed into the input.

reddit · r/MachineLearning · /u/oPeraza2007 · Sep 10, 02:28

**「Background」** MaleCNS v1.0 is Janelia FlyEM&\#x27;s electron-microscopy reconstruction of the full Drosophila male central nervous system — 166k neurons in the experiment&\#x27;s framing — distributed as segment-to-segment connectivity tables \(a 1.1 GB full connection graph at minimum confidence 0.5\) and queried through neuPrint-based tools, including the malecns package, with release notes on the project site dated Nov 7, 2025. In neuPrint, queries can be run with regex enabled so that neuron type and instance criteria are interpreted as regular expressions rather than exact-match strings, which is the mechanism behind the described failure where full-match versus substring semantics silently returned no neurons for two populations. The surrounding approach combines fixed connectome wiring with dopamine-style plasticity and reinforcement learning, a way of testing whether biological structure alone can support a task like Pong without hand-coded behavior.

**「Impact」** Developers and researchers who reuse the MaleCNS v1.0 connectome should verify synapse-level connectivity paths before running plasticity experiments, since the author&\#x27;s audit found neuron populations silently zeroed by a neuPrint regex full-match/substring bug and motor neurons with zero synapses from any sensory pathway. The viral Doom and Minecraft demos offer limited reassurance here, as outside coverage characterizes them as approximations of fly neural activity rather than a fly brain actually learning.

<details><summary>References</summary>
<ul>
<li><a href="https://male-cns.janelia.org/">Male CNS Connectome - MaleCNS connectome</a></li>
<li><a href="https://male-cns.janelia.org/download/">Download - MaleCNS connectome</a></li>
<li><a href="https://natverse.org/malecns/">Access to the Latest Janelia FlyEM Datasets • malecns</a></li>
<li><a href="https://connectome-neuprint.github.io/neuprint-python/docs/neuroncriteria.html">NeuronCriteria — neuprint-python 0.6.2 documentation</a></li>
<li><a href="https://neuprint.janelia.org/public/neuprintuserguide.pdf">NeuPrint Manual</a></li>
<li><a href="https://www.virtualflybrain.org/docs/tutorials/4_neuprint/">neuprint | Virtual Fly Brain</a></li>
<li><a href="https://hothardware.com/news/google-mapped-a-fruit-fly-brain-so-engineers-taught-it-to-play-doom">Google Mapped A Fruit Fly Brain, So Engineers Taught It To Play Doom</a></li>
<li><a href="https://www.msn.com/en-us/gaming/general/google-used-ai-to-reconstruct-a-fly-brain-so-people-made-it-play-doom/ar-AA2bTTZ8">Google used AI to reconstruct a fly brain, so people made it play Doom</a></li>
<li><a href="https://github.com/evnsnclr/neurocraft-fly-public">GitHub - evnsnclr/neurocraft- fly -public: NeuroCraft Fly by Evan Sinclair...</a></li>

</ul>
</details>

**Tags**: `#connectomics`, `#computational neuroscience`, `#reinforcement learning`, `#reproducibility`, `#bio-inspired AI`

---

<a id="item-tech-news-6"></a>
### [Ant International, Visa, Mastercard to Build AI-Agent Payment Standards](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 7.0/10

Ant International announced it is partnering with Visa and Mastercard to develop common standards for payments made by AI agents. The three parties plan to establish a &quot;Know Your Agent&quot; mechanism that links an agent to a valid legal entity, evaluates its behavior, and monitors risk, with the aim of improving interoperability and security across different payment systems. They cited a McKinsey forecast that AI agents could handle between $3 trillion and $5 trillion of global consumer commerce transactions by 2030. The announcement, reported by CNBC, describes the initiative&\#x27;s scope and rationale but does not provide technical specifications or confirm that any standard has been implemented.

telegram · zaihuapd · Sep 10, 03:00

**「Background」** AI agents are increasingly being used to shop, book services, and transact on a user&\#x27;s behalf, but the protocols for identifying and authorizing those agents remain fragmented across payment networks, creating friction and fraud risk. Ant International, Visa, and Mastercard announced a &quot;Know Your Agent&quot; \(KYA\) interoperability framework in São Paulo on September 10, 2026, modeled on familiar Know Your Customer checks, to establish whether an AI agent is authorized to transact for a given user. The announcement covers a proposed framework rather than a deployed, enforceable standard.

**「Impact」** If the joint effort yields a shared standard, merchants, issuers and AI-agent developers would likely need to register and verify agents before they can initiate payments across Visa and Mastercard rails, since comparable industry efforts such as Mastercard&\#x27;s Agent Pay already tie authorization to registered, verified agents and permission-bound tokens. Because the announcement describes a proposed mechanism rather than a confirmed, implemented standard, the scope, timeline and mandatory nature of any &quot;Know Your Agent&quot; requirements remain uncertain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html">Ant International, Visa and Mastercard team up on AI payment standard</a></li>
<li><a href="https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/">Ant International, Visa, and Mastercard Agree on Agent Identity Standard. Now Comes the Hard Part. – Forkast</a></li>
<li><a href="https://www.hokanews.com/2026/09/visa-and-mastercard-back-ant.html">Visa and Mastercard Back Ant International’s ‘Know Your Agent’ Standard for AI Payments - Hokanews</a></li>
<li><a href="https://www.pymnts.com/opinion/2026/fis-says-agentic-commerce-needs-proof-not-promises/">PYMNTS | FIS Says Agentic Commerce Needs Proof, Not Promises</a></li>
<li><a href="https://www.linkedin.com/pulse/5-ai-protocols-every-commerce-practitioner-must-know-aditya-chaudhari-sgmee">5 AI Protocols Every Commerce Practitioner Must Know for Agentic ...</a></li>

</ul>
</details>

**Tags**: `#AI payments`, `#AI agents`, `#payment standards`, `#fintech`, `#Visa/Mastercard`

---

<a id="item-tech-news-7"></a>
### [Tencent Hunyuan releases open-source AuK audio editing model and AuK-Flash](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

Tencent Hunyuan announced the release of AuK, an open-source audio editing model that unifies speech generation and editing through natural-language instructions and reference audio. It supports zero-shot text-to-speech, voice, style, and emotion editing, accent removal, and multi-speaker separation. Alongside it, Tencent released AuK-Flash, which uses 4-step inference and is approximately 4.5 times faster under matching conditions. The code, model weights, and demos have been made available online. The announcement did not include technical details, benchmarks, or independent evaluation.

telegram · zaihuapd · Sep 10, 11:56

**「Background」** AuK is Tencent Hunyuan&\#x27;s 1.5-billion-parameter foundation model for speech generation and editing, trained on millions of hours of diverse audio and exposed through a unified natural-language instruction interface \(tool-1-2\). In this context, zero-shot text-to-speech means generating a voice from a short reference clip without task-specific fine-tuning, while instruction-based editing lets users alter content, timbre, style, or emotion through text prompts \(tool-1-2\). The release lands amid growing interest in open-weight speech models, with external coverage reporting a score of 49.73 on SpeechEditBench and describing AuK as an &quot;audio version of Nano Banana&quot; \(tool-1-3\).

**「Impact」** Developers and speech engineers gain a single 1.5B open-weight model that consolidates zero-shot and instruction-based TTS, acoustic and paralinguistic editing, speech enhancement, and source separation behind one natural-language interface, reducing the need to chain separate tools for pitch, emotion, denoising, or speaker separation. AuK-Flash&\#x27;s 4-step inference at roughly 4.5× the speed of the base model under matched conditions lowers the barrier to interactive or high-throughput deployment, though the release notice includes no independent evaluation of quality or latency claims.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Tencent-Hunyuan/AuK">GitHub - Tencent-Hunyuan/AuK: AuK: An Open-Source ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/tencent-open-sources-1-5b-parameter-audio-model-auk-for-voice-editing-and-generation">Tencent open-sources the 1.5-billion-parameter audio model ...</a></li>
<li><a href="https://arxiv.org/html/2609.08936v1">AuK Technical Report: An Open-Source Foundational Model for ...</a></li>
<li><a href="https://github.com/davahiatak1/AuK-tss-voice">GitHub - davahiatak1/AuK-tss-voice: AuK: An Open-Source ...</a></li>
<li><a href="https://www.aimodeling.com/en/news/slug/tencent-hunyuan-auk-speech-editing">AuK: Tencent&#x27;s Open 1.5B Speech Generation and Editing Model</a></li>

</ul>
</details>

**Tags**: `#audio-editing`, `#open-source`, `#text-to-speech`, `#speech-synthesis`, `#Tencent-Hunyuan`

---

## Financial News

<a id="item-finance-news-1"></a>
### [IEA Projects Record Global Coal Demand in 2026 as LNG Prices Rise](https://oilprice.com/Latest-Energy-News/World-News/IEA-Global-Coal-Demand-Set-to-Hit-Record-High-as-Iran-War-Chokes-LNG-Supply.html) ⭐️ 8.0/10

The International Energy Agency projects global coal demand will rise 1.2% in 2026 to a record 8.94 billion tons, reversing its pre-war expectation of a slight drop, as higher LNG prices linked to the Strait of Hormuz disruption push economies including China and India to use more coal-fired power.

rss · OilPrice.com · Sep 10, 14:30

**「Background」** The Strait of Hormuz is the shipping route for roughly a fifth of globally traded liquefied natural gas \(gas chilled to liquid form so it can be carried by tanker\), and those LNG shipments have slumped since the Iran war began more than six months ago. Before that disruption, the IEA had expected global coal demand to edge slightly lower in 2026.

**「Who is affected」** Utilities and electricity users in China, India, Japan, South Korea and Europe are the immediate channel: with LNG and gas prices pushed up by the Strait of Hormuz disruption, power systems are running coal-fired plants harder, a shift that can feed through to power tariffs in those Asian markets.

<details><summary>References</summary>
<ul>
<li><a href="https://dinardetectives.com/iea-global-coal-demand-record-high-iran-lng/">IEA: Global Coal Demand Set for Record High</a></li>
<li><a href="https://www.linkedin.com/pulse/strait-hormuz-lng-oil-new-energy-security-shock-md-nasiruddin-evohf">Strait of Hormuz , LNG &amp; Oil | The New Energy Security Shock</a></li>
<li><a href="https://eecc.energy/insights/blog-and-updates/asias-energy-chokepoint-how-the-hormuz-disruption-is-impacting-energy-markets">Asia&#x27;s energy chokepoint: How the Hormuz disruption is ...</a></li>
<li><a href="https://finance.yahoo.com/energy/articles/iea-strait-hormuz-blockade-driving-111835908.html?fr=sycsrp_catchall">IEA: Strait of Hormuz blockade driving up global use of coal</a></li>

</ul>
</details>

**Tags**: `#IEA`, `#coal demand`, `#LNG supply`, `#Strait of Hormuz`, `#energy markets`

---

<a id="item-finance-news-2"></a>
### [Fed holds interest rates steady in a 9-3 vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 8.0/10

The Federal Reserve left its benchmark interest rate unchanged, according to ABC7 Los Angeles, with the decision drawing three dissenting votes in a 9-3 split. The report did not include the current rate level, the reasoning behind the vote, or any guidance on future policy moves.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Reserve’s rate-setting committee left its target range for the federal funds rate—the overnight rate banks charge one another—at 3.5% to 3.75% on July 29, 2026, according to the Fed’s statement. Spectrum News reported that this was the fifth straight meeting without a change and that the decision came amid persistently high inflation and an energy-price spike tied to the Iran war.

**「Impact」** With the benchmark rate held — U.S. Bank puts the range at 3.50%–3.75% for the July 2026 decision — households and businesses carrying variable-rate debt, such as credit cards and many business credit lines, see no immediate reduction in their borrowing costs.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrumlocalnews.com/us/snplus/business/2026/07/29/federal-reserve-interest-rate-announcement">Federal Reserve leaves interest rate unchanged - Spectrum News</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Federal Reserve Holds Rates at 3.50%-3.75% in July 2026 | U.S ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#US economy`

---

<a id="item-finance-news-3"></a>
### [Kalshi Launches CFTC-Approved Gold and Silver Perpetual Futures in the U.S.](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

Kalshi launched perpetual futures tied to gold and silver on Thursday after the Commodity Futures Trading Commission approved the listings this week, making them the first non-crypto perpetual futures cleared for U.S. trading. Perpetual futures are contracts that track an asset&\#x27;s price without an expiration date and without requiring the buyer to own the underlying asset.

rss · CNBC Finance · Sep 10, 14:00

**「Background」** Kalshi first won approval for crypto-linked perpetual futures in late May, and those contracts have since recorded $44 billion in notional volume, according to the platform&\#x27;s website. Kalshi says it picked metals next because of client interest in inflation-linked commodities, and it is also seeking approval for perpetuals tied to U.S. equities, copper and currencies.

**「Impact」** The approval is being contested by incumbents: CME Group has sued the CFTC to block U.S. perpetual futures, arguing the agency improperly permitted them, and shares of traditional futures exchanges CME and CBOE fell on concern the contracts could disrupt their business models.

**Tags**: `#Kalshi`, `#CFTC`, `#perpetual futures`, `#gold and silver`, `#CME`

---

<a id="item-finance-news-4"></a>
### [U.S. Pledges $3 Billion for Critical Minerals as China&\#x27;s Lead Persists](https://oilprice.com/Metals/Commodities/Why-The-United-States-Belated-Critical-Minerals-Gambit-Wont-Stop-China.html) ⭐️ 7.0/10

The U.S. government has committed $3 billion to domestic critical minerals projects, including a $1.4 billion conditional loan from the Pentagon&\#x27;s Office of Strategic Capital to California battery-materials startup Sila Nanotechnologies, as part of efforts to counter China&\#x27;s dominance of the sector.

rss · OilPrice.com · Sep 10, 23:00

**「Background」** China accounts for roughly 60% of global critical minerals mining and more than 90% of the refining and processing of materials such as rare earths, graphite and gallium, a lead the article attributes to decades of state subsidies and overseas infrastructure financing.

**「Impact」** The article reports that U.S. electric vehicle sales fell 27% year over year in the first quarter of 2026 after the $7,500 federal EV tax credit was eliminated, a shrinking home market for the battery-materials makers the new funding is meant to support.

**Tags**: `#critical minerals`, `#rare earths`, `#US-China relations`, `#supply chain`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [Mexico Plans to Cut Pemex Support by About 70% Next Year](https://oilprice.com/Energy/Energy-General/Higher-Oil-Prices-Let-Mexico-Pull-Back-Billions-in-Pemex-Support.html) ⭐️ 7.0/10

Mexico&\#x27;s government plans to cut financial support for the state oil company Pemex by about 70% next year, to 81 billion pesos \(about $4.8 billion\), based on expectations of a roughly 95 billion peso \($5.63 billion\) cash surplus from higher oil prices, according to a Bloomberg report cited by Oilprice.com. Pemex posted an actual first-quarter loss of 45.99 billion pesos \(about $2.6 billion\) despite government aid, and the budget figures are government forecasts rather than results.

rss · OilPrice.com · Sep 10, 22:00

**「Background」** The reduction follows the Sheinbaum administration&\#x27;s 2025–2035 strategic plan for Pemex, which is designed to cut the company&\#x27;s debt and stabilize production while weaning it off government financial support, with that goal set for as soon as 2027.

<details><summary>References</summary>
<ul>
<li><a href="https://mexicobusiness.news/oilandgas/news/mexico-unveils-10-year-plan-reform-revive-pemex">Mexico Unveils 10-Year Plan to Reform, Revive PEMEX</a></li>
<li><a href="https://momentsinmexico.substack.com/p/what-is-sheinbaums-pemex-strategic-plan">What is Sheinbaum&#x27;s Strategic Plan for Pemex?</a></li>

</ul>
</details>

**Tags**: `#Pemex`, `#Mexico energy policy`, `#oil prices`, `#sovereign support`, `#corporate debt`

---

<a id="item-finance-news-6"></a>
### [EIA Projects Record US Natural Gas Output and LNG Exports Through 2027](https://oilprice.com/Energy/Natural-Gas/US-Natural-Gas-Market-Verging-on-Record-Growth.html) ⭐️ 7.0/10

The US Energy Information Administration forecasts record US natural gas production of 111.7 billion cubic feet per day \(bcfd\) in 2026, up from 107.6 bcfd in 2025, and 115.9 bcfd in 2027, alongside record LNG exports rising from 15.1 bcfd in 2025 to 17.4 bcfd in 2026 and 18.6 bcfd in 2027. The agency cites higher drilling efficiency, rising electricity demand and expanding LNG export capacity, and says US gas inventories are on track to start winter about 5% above the five-year average on Oct. 31.

rss · OilPrice.com · Sep 10, 19:00

**「Background」** A separate Ernst &amp; Young study of the 30 largest publicly traded US exploration and production companies found total capital expenditures fell 49% year over year and M&amp;A spending dropped 70%, while oil reserve additions from extensions and discoveries declined 11% and failed to fully replace production for the first time since 2021. \(The article reports domestic consumption rising to the same 111.7 and 115.9 bcfd figures it gives for production, after a record 91.9 bcfd in 2025 — demand and supply figures that are identical in the source.\)

**「Impact」** If the projections hold, US gas producers in the Permian and Haynesville regions and LNG exporters would handle rising volumes, while the EY findings suggest those producers are funding growth with restrained capital spending rather than new drilling budgets.

**Tags**: `#US natural gas`, `#EIA forecasts`, `#LNG exports`, `#oil &amp; gas M&amp;A`, `#reserve replacement`

---

<a id="item-finance-news-7"></a>
### [Permian Gas Benchmark Waha Turns Negative for 118 Days This Year](https://oilprice.com/Energy/Energy-General/Permian-Gas-Has-Been-Worth-Less-Than-Nothing-for-118-Days-This-Year.html) ⭐️ 7.0/10

The Permian Basin’s natural gas benchmark, Waha, traded below zero on 118 of the first 131 trading days this year, as the region produces more gas than its pipelines can carry. The U.S. Energy Information Administration expects Permian gas production to average a record 29.2 billion cubic feet per day this year, up 6% and a record for the region.

rss · OilPrice.com · Sep 10, 15:00

**「Background」** Permian gas is mostly produced alongside oil, so when pipeline capacity is insufficient, producers may pay to have the gas taken away rather than shut in the oil wells that generate most of their revenue.

**「Impact」** Chevron’s subsidiary signed a 20-year agreement with Microsoft in June to build a gas-fired plant of up to about 2.67 gigawatts beside a data center near Pecos, Texas, part of a behind-the-meter trend that RBC Capital Markets says totals about 38 gigawatts of announced gas capacity in Texas.

**Tags**: `#Permian Basin`, `#Natural Gas Prices`, `#Energy Infrastructure`, `#Data Centers`

---

<a id="item-finance-news-8"></a>
### [印度严重欺诈调查局建议详查小米在印业务](https://www.zaobao.com.sg/news/china/story20260909-9652945) ⭐️ 7.0/10

印度严重欺诈调查局建议对小米在印度的业务展开详细调查，涉及商业模式、资金流向及外资法规合规情况；印度政府正在审查相关备忘录。小米回应称尚未收到通知，并强调始终遵守当地法律。

telegram · zaihuapd · Sep 10, 04:09

**「Background」** India&\#x27;s Serious Fraud Investigation Office is a government agency that investigates suspected corporate fraud, and a recommendation for a probe is not itself an enforcement action. Xiaomi already faces separate tax and royalty-payment disputes in India, which reporting links to the current scrutiny.

**「Who is affected」** If the recommendation leads to a formal investigation, it would deepen regulatory scrutiny of Xiaomi&\#x27;s India operations and add pressure on other Chinese companies doing business there, with Beijing already urging India to provide a fair and just business environment.

<details><summary>References</summary>
<ul>
<li><a href="https://english.gujaratsamachar.com/news/science-technology/serious-fraud-investigation-office-recommends-detailed-probe-into-xiaomis-india-business-over-foreign-investment-compliance-68723015972">Serious Fraud Investigation Office Recommends... | Gujarat Samachar</a></li>
<li><a href="https://economictimes.indiatimes.com/industry/cons-products/electronics/indias-serious-fraud-office-recommends-detailed-probe-into-xiaomis-business-in-country/articleshow/133963640.cms">India &#x27;s Serious Fraud Office recommends &#x27;detailed&#x27; probe into...</a></li>
<li><a href="https://www.businesstoday.in/latest/corporate/story/sfio-recommends-investigation-into-xiaomis-india-business-over-alleged-irregularities-report-554432-2026-09-10">SFIO recommends investigation into Xiaomi’s India business over alleged irregularities: Report - BusinessToday</a></li>
<li><a href="https://www.firstpost.com/tech/xiaomi-probe-report-china-urges-india-to-provide-fair-just-business-environment-14044680.html">Xiaomi probe report: China urges India to &#x27;provide fair, just business environment&#x27;</a></li>
<li><a href="https://www.chinamoneynetwork.com/2026/09/09/investigation-recommended-for-xiaomis-business-in-india-amid-alleged-irregularities">Investigation Recommended for Xiaomi’s Business in India Amid Alleged Irregularities</a></li>

</ul>
</details>

**Tags**: `#Xiaomi`, `#India`, `#regulatory investigation`, `#foreign exchange compliance`, `#corporate governance`

---

<a id="item-finance-news-9"></a>
### [Chinese AI chipmakers raise prices as HBM shortage bites](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

Chinese AI chipmakers including Huawei and Cambricon are raising prices as a shortage of high-bandwidth memory \(HBM\) constrains domestic production. Huawei&\#x27;s Ascend 950DT chip is being quoted roughly 20%–50% higher than two months ago, with some older chips up about 30%, while Cambricon&\#x27;s new SiYuan 690 is expected to cost about 20%–30% more, according to Reuters.

telegram · zaihuapd · Sep 10, 09:29

**「Background」** Advanced high-bandwidth memory \(HBM\), the fast memory stacked next to AI chips, is supplied mainly by SK Hynix, Samsung and Micron, and U.S. export limits have restricted China’s access, making HBM a bottleneck for domestic AI chip expansion.

**「Who is affected」** Chinese technology companies building AI computing infrastructure face higher costs, because the HBM shortage and the resulting chip price increases make the domestic accelerators and memory needed to train and run AI models more expensive to buy.

<details><summary>References</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-09-10/exclusive-chinas-ai-chipmakers-raise-prices-as-high-bandwidth-memory-shortage-bites">Exclusive- China &#x27;s AI Chipmakers Raise Prices as High-Bandwidth...</a></li>
<li><a href="https://www.freemalaysiatoday.com/category/business/2026/09/10/china-s-ai-chipmakers-raise-prices-as-high-bandwidth-memory-shortage-bites">China’s AI chipmakers raise prices as HBM shortage bites | FMT</a></li>
<li><a href="https://www.itp.net/ai-automation/chinas-ai-chipmakers-raise-prices-as-hbm-shortage-drives-up-costs">China’s AI Chipmakers Raise Prices as HBM Shortage Drives Up Costs - ITP.net</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#HBM`, `#semiconductor supply chain`, `#China tech`, `#export controls`

---

<a id="item-finance-news-10"></a>
### [TSMC Stock Slips Despite 53% August Revenue Growth](https://finance.yahoo.com/markets/stocks/articles/tsmc-stock-slips-despite-53-122227013.html) ⭐️ 7.0/10

TSMC stock slipped even as the company reported 53% August revenue growth, a notable indicator for the semiconductor industry.

openbb · NVDA · Sep 10, 12:22

**Tags**: `#TSMC`, `#semiconductor industry`, `#revenue growth`, `#stock market reaction`, `#monthly revenue`

---

<a id="item-finance-news-11"></a>
### [TSMC September Revenue Reportedly Jumps 53%](https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductor-september-revenue-surges-151224109.html) ⭐️ 7.0/10

Taiwan Semiconductor Manufacturing Co.&\#x27;s September revenue reportedly rose 53%, which the report links to demand the chipmaker cannot fully meet. The available information does not specify the comparison baseline for the 53% figure or give the underlying revenue amount, so the growth rate should be treated as a reported headline figure rather than a confirmed detail.

openbb · NVDA · Sep 10, 15:12

**「Background」** TSMC, founded in 1987, was the first company to make chips exclusively for other firms&\#x27; designs — a &quot;pure-play foundry&quot; — rather than selling its own branded chips, which makes its monthly sales a broad gauge of semiconductor demand. Reports attribute the recent surge to AI data-center buildout demand outpacing the industry&\#x27;s ability to supply chips.

**「Who feels the squeeze」** Because advanced chips from designers such as Nvidia and AMD are produced largely at TSMC&\#x27;s foundries, demand that exceeds TSMC&\#x27;s capacity can mean longer lead times and tighter chip allocations for the electronics and AI hardware that depend on them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TSMC">TSMC - Wikipedia</a></li>
<li><a href="https://www.tsmc.com/english/aboutTSMC">About TSMC - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-10/tsmc-revenue-rises-53-as-ai-chip-demand-outstrips-supply">TSMC Revenue Rises 53 % as AI Chip Demand Outstrips Supply</a></li>
<li><a href="https://siliconanalysts.com/analysis">Industry Analysis - Semiconductor Market Intelligence</a></li>
<li><a href="https://theboard.world/articles/geopolitics/tsmc-semiconductor-supply-chain-risk-factors/">TSMC: Semiconductor Supply Chain Risk Factors | The Board</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductors`, `#revenue growth`, `#supply constraints`, `#Taiwan`

---

<a id="item-finance-news-12"></a>
### [OpenAI Picks Broadcom for First Custom AI Chip](https://finance.yahoo.com/technology/ai/articles/openai-picked-broadcom-first-custom-164039569.html) ⭐️ 7.0/10

OpenAI has selected Broadcom to build its first custom AI chip, according to reports, a step that could sharpen competition in the AI semiconductor market. The available excerpt gives no deal terms, chip specifications, production timeline, or confirmation from either company.

openbb · NVDA · Sep 10, 16:40

**「Background」** OpenAI announced a partnership with Broadcom in October 2025 to build its own AI processors, with plans to produce 10 gigawatts of chips — roughly enough to power 8 million homes, according to Cybernews. Eight months later, the two companies unveiled Jalapeno, described as OpenAI&\#x27;s first custom AI inference chip \(a chip built specifically to run trained AI models\), a project the Yahoo Finance report calls one of Broadcom&\#x27;s most valuable customer relationships in semiconductors.

**「Impact」** Reports of a roughly $10 billion OpenAI–Broadcom custom-chip agreement point to the largest AI buyers using in-house accelerators as an alternative to Nvidia&\#x27;s merchant GPUs, with Broadcom as the supplier — a competitive shift for Nvidia and the data-center chip market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/24/openai-and-broadcom-reveal-jalapeno-first-ai-chip-in-partnership.html">OpenAI and Broadcom reveal Jalapeno, first AI chip in ... - CNBC</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/openai-picked-broadcom-first-custom-164039569.html?fr=sycsrp_catchall">OpenAI Picked Broadcom for Its First Custom AI Chip. The Race ...</a></li>
<li><a href="https://cybernews.com/ai-news/openai-broadcom-build-first-ai-processor-chip-deal/">OpenAI, Broadcom join forces on AI chips | Cybernews</a></li>
<li><a href="https://intellectia.ai/blog/openai-broadcom-jalapeno-ai-chip-2026">OpenAI Broadcom Jalapeno Chip : AI Hardware Revolution 2026</a></li>
<li><a href="https://www.linkedin.com/posts/auria-asadsangabi-98b608143_openai-broadcom-make-10-billion-deal-for-activity-7369854557390147584-s5wn">Broadcom and OpenAI partner on custom AI chip deal | LinkedIn</a></li>
<li><a href="https://opentools.ai/news/broadcom-and-openai-announce-landmark-dollar10-billion-deal-for-custom-ai-chips">Broadcom and OpenAI Announce Landmark $10 Billion... | OpenTools</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Broadcom`, `#OpenAI`, `#semiconductor competition`

---

<a id="item-finance-news-13"></a>
### [Trump Reportedly Voices No Regrets on Iran War as Oil Tops $100](https://finance.yahoo.com/energy/articles/trump-reportedly-says-no-regrets-233654584.html) ⭐️ 7.0/10

President Trump reportedly said he has no regrets over the Iran war even as oil prices topped $100 a barrel, according to a headline account that provides no confirmed date, price source, or size for the associated moves in energy exchange-traded funds USO and UCO. The report also links the situation to rising stakes for the midterm elections, but no further details on either the market moves or the political consequences were available.

openbb · CL=F · Sep 10, 23:36

**「Background」** U.S. crude oil, the benchmark known as West Texas Intermediate that the USO fund tracks, had last traded above $100 a barrel in May, and prices have climbed as the U.S.–Iran war escalated, CNBC reported; Iran targeted a U.S. base in Jordan with missiles in retaliation for the U.S. military destroying five Iranian oil tankers.

**「Impact」** With crude above $100, fuel costs rise for households and fuel-dependent businesses such as airlines and truckers, while USO and UCO — ETFs that track crude oil futures rather than physical barrels — are the main listed vehicles through which traders take that exposure, and Trump&\#x27;s reported remark that relief would come only after the midterms points to those costs persisting through the election period.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.com/en-in/money/general/trump-reportedly-says-he-has-no-regrets-over-iran-war-even-as-oil-tops-100-uso-and-uco-jump-while-midterm-stakes-get-higher/ar-AA2bYGJc">Trump reportedly says he has no regrets over Iran war even as ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/10/iran-us-oil-hormuz-supply-trump-military-brent-wti.html">U.S. crude oil tops $100 again as market braces for ... - CNBC Oil prices climb over $100 per barrel as US war in Iran ... Oil Hits $100 a Barrel for First Time Since July as U.S. and ... Oil Price Surges Toward $100 as Markets Fail to Share Trump’s ... US oil tops $100 a barrel as Iran war rages; Donald Trump ...</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/trump-reportedly-says-oil-prices-wont-tumble-until-after-midterms-while-iran-signals-more-intense-war-uso-uco-rise/cZt7k6WRJC2">Trump Reportedly Says Oil Prices Won’t Tumble Until After Midterms ...</a></li>
<li><a href="https://etfdb.com/tool/etf-comparison/UCO-USO/">UCO vs. USO : Head-To-Head ETF Comparison | ETF Database</a></li>

</ul>
</details>

**Tags**: `#oil prices`, `#Iran conflict`, `#energy ETFs`, `#geopolitical risk`, `#midterm elections`

---

<a id="item-finance-news-14"></a>
### [Bond Selloff Pushes 10-Year Treasury Yield Near 5%](https://www.wsj.com/finance/investing/the-unrelenting-bond-selloff-puts-the-10-year-yield-on-the-cusp-of-5-78bfb4db?siteid=yhoof2&amp;yptr=yahoo) ⭐️ 7.0/10

The Wall Street Journal reports that an ongoing selloff in bonds has pushed the 10-year U.S. Treasury yield close to 5%. The report does not specify the exact current yield, the prior level it is being compared with, or what is driving the move.

openbb · CL=F · Sep 10, 23:10

**「Background」** The 10-year Treasury yield is the interest rate the U.S. government pays to borrow for a decade and a benchmark for mortgages, corporate borrowing and stock valuations; it had risen to about 4.79%, its highest since November 2023, as bond prices fell in a broad selloff, and market participants treat the 5% level as a psychologically important threshold.

**「Who feels it」** Treasury yields serve as a benchmark for home mortgages, auto loans, and corporate borrowing, so a 10-year yield near 5% — recently about 4.79%, and up roughly 13.5% over the past year — points to higher funding costs for households and companies that borrow, and to paper losses for existing bondholders.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-11/global-bond-selloff-sends-10-year-treasury-yields-to-cusp-of-5">Global Bond Selloff Sends 10 - Year Treasury Yields to... - Bloomberg</a></li>
<li><a href="https://www.ibtimes.com/higher-bond-yields-havent-broken-stock-rally-yet-wall-street-sees-5-benchmark-big-test-3807057">Higher Bond Yields Haven&#x27;t Broken The Stock Rally Yet. Wall Street ...</a></li>
<li><a href="https://www.tradingview.com/symbols/TVC-US10Y/">10 Year Treasury Yield (US10Y) Price and Chart — TradingView</a></li>
<li><a href="https://tradingeconomics.com/united-states/government-bond-yield">US 10 Year Treasury Note Yield - Quote - Chart - Historical Data - News</a></li>

</ul>
</details>

**Tags**: `#Treasury yields`, `#bonds`, `#market selloff`, `#interest rates`, `#fixed income`

---