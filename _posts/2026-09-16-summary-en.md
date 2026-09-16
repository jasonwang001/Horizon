---
layout: default
title: "Horizon Summary: 2026-09-16 (EN)"
date: 2026-09-16
lang: en
---

> From 251 items, 26 important content pieces were selected

---

**Technology News**
1. [AI agent found leaked Baseten GitHub token granting admin access](#item-tech-news-1) ⭐️ 8.0/10
2. [Typesafe.ai launches System One Models and Jev for fast typed structured inference](#item-tech-news-2) ⭐️ 7.0/10
3. [Show HN: E-ink frame listens for birds and draws 1800s illustrations](#item-tech-news-3) ⭐️ 7.0/10
4. [Google announces Gemini 3.8 Live and Extended Thinking models](#item-tech-news-4) ⭐️ 7.0/10
5. [Capsule packs web apps and data into one SQLite file](#item-tech-news-5) ⭐️ 7.0/10
6. [Show HN: Hacking a $20 4G Hotspot into a Texting Device](#item-tech-news-6) ⭐️ 7.0/10
7. [SHADOW-50M: 44M-parameter ternary LLM runs offline in 19.8 MB](#item-tech-news-7) ⭐️ 7.0/10
8. [TabPFN-3.5 Released as SOTA Tabular Foundation Model](#item-tech-news-8) ⭐️ 7.0/10
9. [Sanders Bill Would Ban Superintelligent AI With 20-Year Penalties](#item-tech-news-9) ⭐️ 7.0/10
10. [Google Reportedly Opens Anthropic&\#x27;s Claude to All Its Engineers](#item-tech-news-10) ⭐️ 7.0/10
11. [MediaTek launches Dimensity 9600 Pro on TSMC 2nm, plus 9600M](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI Contractors Read Real ChatGPT Chats in &\#x27;Project Lily&\#x27;](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [Saudi East-West Pipeline Shutdown Squeezes Oil Market](#item-finance-news-1) ⭐️ 9.0/10
2. [Hormuz Risk Splits Crude Prices as Brent Tops $107](#item-finance-news-2) ⭐️ 9.0/10
3. [Federal Reserve Holds Interest Rates Steady, Signals Possible Hike](#item-finance-news-3) ⭐️ 9.0/10
4. [China&\#x27;s August retail sales miss forecast as investment slump deepens](#item-finance-news-4) ⭐️ 8.0/10
5. [U.S. Diesel Sets New Weekly Price Record, 2026 Annual Record Within Reach](#item-finance-news-5) ⭐️ 8.0/10
6. [China&\#x27;s industry and planning ministries issue 15th Five-Year Plan for electronics manufacturing](#item-finance-news-6) ⭐️ 8.0/10
7. [Chinese Solar Panels at 12 Cents a Watt Drive Global Rooftop Boom](#item-finance-news-7) ⭐️ 7.0/10
8. [ADNOC Buys Discounted Iraqi Crude, Freeing UAE Barrels for Export](#item-finance-news-8) ⭐️ 7.0/10
9. [Libya&\#x27;s NOC Threatens Force Majeure After Oilfield Shutdowns](#item-finance-news-9) ⭐️ 7.0/10
10. [FERC Orders Mandatory Reliability Standards for AI Data Centers](#item-finance-news-10) ⭐️ 7.0/10
11. [中国发布共享单车服务新国标，2026年11月起实施](#item-finance-news-11) ⭐️ 7.0/10
12. [10-year Treasury Yield Reaches 2007 High as Oil Stays Above $100](#item-finance-news-12) ⭐️ 7.0/10
13. [Coca-Cola plans $10B US manufacturing spend by 2030](#item-finance-news-13) ⭐️ 7.0/10
14. [Fed&\#x27;s preferred inflation gauge shows fastest price rise in three years](#item-finance-news-14) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AI agent found leaked Baseten GitHub token granting admin access](https://www.strix.ai/blog/baseten-harbor-github-pat-takeover) ⭐️ 8.0/10

Strix researchers say they used an AI pen-testing agent to find a live GitHub personal access token for basetenbot in Baseten&\#x27;s Docker build history, gaining admin access to Baseten&\#x27;s production GitHub in 25 minutes. According to comment quotes, the token had admin and push access to Baseten&\#x27;s main product repo, the GitOps repo that drives its clusters, and its Homebrew tap, plus read/write access to other private repositories, including some per-customer repos. The disclosure timeline says Strix reported the token, public Harbor project, and repository permissions on July 13 at 11:10 PM; Baseten made Harbor private the morning of July 14 but the token still worked, and Baseten Security&\#x27;s Anton confirmed the issue as critical and said the project was private and the token rotated at 4:34 PM that day. Strix disclosed the incident in a vendor-authored blog post, which commenters characterized as strong marketing for Strix and a damaging story for Baseten. The post is a security-tool vendor&\#x27;s account, so details beyond the quoted timeline and permissions should be treated with that framing in mind.

hackernews · bearsyankees · Sep 15, 18:11 · [Discussion](https://news.ycombinator.com/item?id=49716476)

**「Background」** Strix is an autonomous AI penetration-testing agent built by the company of the same name, which was evaluating Baseten — a platform for running model inference — as a potential vendor before running its own tool against it. The incident centers on a GitHub personal access token \(PAT\), a credential that grants API-level access to repositories, found exposed in the build history of a publicly available Docker image dating back to March 2023. Because Docker images retain build layers and metadata, secrets embedded during a build can remain retrievable long after they were introduced.

**「Impact」** For Baseten, the exposure forced the Harbor project private and the basetenbot token to be rotated, while showing security and DevOps teams that secrets in Docker build history can grant broad production access.

**「Community discussion」** Commenters saw the post as highly effective marketing for Strix and damaging for Baseten, with some saying they would try or add Strix to their stack. Others questioned the legality of the agent-driven access and criticized Strix for naming a real vendor as a victim and pulling its image in what read like a promotional account.

<details><summary>References</summary>
<ul>
<li><a href="https://www.strix.ai/blog/baseten-harbor-github-pat-takeover">We wanted to use Baseten for inference. We ended up with ...</a></li>
<li><a href="https://elsolitario.org/en/2026/09/15/github-token-admin-baseten-harbor/">GitHub Token: How Strix Found Admin Access at Baseten</a></li>
<li><a href="https://vuink.com/post/fgevk-d-dnv/blog/baseten-harbor-github-pat-takeover">We wanted to use Baseten for inference. We ended up with ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#github`, `#ai-agents`, `#secrets-management`, `#penetration-testing`

---

<a id="item-tech-news-2"></a>
### [Typesafe.ai launches System One Models and Jev for fast typed structured inference](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 7.0/10

Typesafe.ai has introduced System One Models and Jev, a fast typed structured-inference approach that drew 701 points and 240 comments on Hacker News. According to commenters, Jev trades general-purpose generation for fast typed inference and can only produce structured output, making it suited to tasks such as classification rather than open-ended code generation. A commenter citing the documentation said the model accepts arbitrary text input, including complex JSON, plus questions in formats such as yes/no, multiple-choice, or score, answering in milliseconds at a cost of $0.042 per million tokens. The announcement itself did not explain these details, and commenters pointed readers to the Typesafe.ai documentation for a clearer explanation. While the approach was called genuinely interesting and new, the speed comparison was questioned because a generative model in a Turing-complete language can do anything a computer can do.

hackernews · albelfio · Sep 15, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49717558)

**「Background」** Jev is a model from TypeSafe AI, introduced alongside its System One Models, designed to make structured software decisions rather than generate free-form text. It is a specialized structured-inference tool—commenters describe it as taking arbitrary text or JSON and answering constrained questions—in contrast to general-purpose generative LLMs that can output code or unstructured prose. TypeSafe reports response times of a fraction of a second and says that in its own business-workflow tests Jev was nearly 200 times faster than chatbots.

**「Impact」** If the documented millisecond latency and $0.042 per million token cost hold, Jev could give developers a cheap structured-inference primitive for classification, CI flake triage, and observability triggers, while remaining unsuitable as a general-purpose code-generation replacement.

**「Community Discussion」** Hacker News commenters broadly welcomed the launch as genuinely interesting and new, with one describing possible CI and observability uses and another connecting it to Python design-by-contract work with LLMs. The main disagreement centered on the speed comparison: critics argued Jev is a specialized structured-output tool rather than a general-purpose breakthrough, though several commenters still found the documentation promising.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49717558">Introducing System One Models and Jev | Hacker News</a></li>
<li><a href="https://daily.dev/posts/jev-skips-token-generation-entirely-and-the-speed-numbers-are-hard-to-ignore-nv8tizgl7">Jev skips token generation entirely, and the speed... - daily.dev</a></li>
<li><a href="https://www.facebook.com/marius.comper/posts/most-chatbots-are-built-to-write-a-new-ai-called-jev-is-built-to-chooseand-its-m/10164926577444621/">Jev ai makes business decisions faster and cheaper than chatbots</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#structured output`, `#type systems`, `#developer tools`, `#AI models`

---

<a id="item-tech-news-3"></a>
### [Show HN: E-ink frame listens for birds and draws 1800s illustrations](https://github.com/arnegiacomo/fugleramme) ⭐️ 7.0/10

A Show HN project presents an e-ink frame that continuously listens for bird calls using the BirdNET classifier and renders detected birds as 1800s-style illustrations. The open-source build is published on GitHub as arnegiacomo/fugleramme and combines on-device audio classification, embedded hardware, and generative illustration on an e-ink display. On Hacker News it drew 1,271 points and 178 comments, with commenters praising it as a polished and inspiring maker project. A commenter clarified that BirdNET is a traditional neural network, not an LLM, linking to its paper in Ecological Informatics \(doi.org/10.1016/j.ecoinf.2021.101236\).

hackernews · arnemunthekaas · Sep 15, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49711544)

**「Background」** Fugleramme is an open-source e-ink frame built around a Raspberry Pi that listens continuously for bird calls and, rather than listing species names, composes a collage of natural-history illustrations that changes as the local birdlife does. Its recognition step relies on BirdNET, a convolutional neural network developed at the Cornell K. Lisa Yang Center for Conservation Bioacoustics that processes raw acoustic data to detect species-specific patterns — a traditional classifier rather than a large language model. The illustrations themselves are not AI-generated: the developer hand-curated public-domain natural-history plates dating back to the 1800s.

**「Impact」** Developers building on the open-source BirdNET classifier gain a concrete hardware reference for pairing local audio inference with a low-power e-ink display, which matters as continuous home-listening setups shift away from the shelved BirdNET-Pi project toward community forks and alternatives such as BirdNET-Go.

**「Community Discussion」** Commenters overwhelmingly praised the project as magical and inspiring, with one noting it is &\#x27;pure art&\#x27; by Norwegian developer Arne Munthe-Kaas. Discussion added technical context that BirdNET is a traditional neural network and shared practical e-ink experience, including ESP32/BTLE frames that can run for years on a 2000mAh battery even with multiple daily refreshes, alongside observations about the recent surge in bird-detection projects such as birdnet-go.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/arnegiacomo/fugleramme">GitHub - arnegiacomo/fugleramme: E-ink bird frame for Raspberry Pi - real-time bird detection by audio, fully local AI, rendered as real, hand-cut 1800s bird illustrations. · GitHub</a></li>
<li><a href="https://blog.circuit.rocks/a-raspberry-pi-5-e-ink-frame-that-paints-the-birds-it-hears">Raspberry Pi 5 E Ink Bird Frame Powered by BirdNET</a></li>
<li><a href="https://www.hackster.io/news/this-smart-picture-frame-shows-you-which-birds-are-outside-92a9b10bfddb">This Smart Picture Frame Shows You Which Birds Are Outside - Hackster.io</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/ birdnet - go : Self-hosted realtime soundscape...</a></li>
<li><a href="https://tech.yahoo.com/computing/articles/open-source-app-raspberry-pi-130013626.html">This open - source app and Raspberry Pi helped me identify every bird ...</a></li>

</ul>
</details>

**Tags**: `#e-ink`, `#embedded-hardware`, `#edge-machine-learning`, `#open-source`, `#audio-classification`

---

<a id="item-tech-news-4"></a>
### [Google announces Gemini 3.8 Live and Extended Thinking models](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 7.0/10

Google announced Gemini 3.8 Live and Gemini 3.8 Live Extended Thinking, according to a blog post surfaced on Hacker News. The supplied item contains no article body, benchmarks, technical specifications, or availability details, so the capabilities of the Extended Thinking variant and the &quot;3.8&quot; version numbering cannot be independently verified from the available evidence. Commenters who tried the release reported solid results, describing it as coping well with thick accents, offering pleasant voices, and exhibiting low latency. One user noted the release is usable on a workspace account, which they said had been difficult for several recent Gemini releases.

hackernews · leumon · Sep 15, 17:38 · [Discussion](https://news.ycombinator.com/item?id=49715947)

**「Background」** Gemini Live is Google&\#x27;s real-time conversational voice mode inside the Gemini app, designed for spoken back-and-forth dialogue rather than typed prompts. Extended Thinking refers to a variant built for more deliberate reasoning, and Google describes the 3.8 Live models as its &quot;most advanced live dialogue models yet,&quot; with the Extended Thinking version adding precision and narrating task progress to keep the dialogue going. Google says the models are available in Gemini Live in the Gemini app and for developers through the Gemini API via Google AI Studio.

**「Impact」** For users of Gemini Live voice mode, early anecdotal reports point to improved latency and accent handling, and at least one Workspace account holder reports access where previous releases were unavailable; no published performance data accompanies these impressions. One commenter also said Gemini 3.8 had not yet been released for Google AI Plus subscribers.

**「Community Discussion」** Commenters were largely positive about voice quality and latency, with one calling it &quot;very solid&quot; and another saying Gemini Live already beats GPT Voice in their personal experience despite previously being weaker at reasoning, while one praised Gemini&\#x27;s prose as the most bearable to read and another described using it for Afrikaans conversation and grammar practice. Skepticism centered on Google&\#x27;s competitive position, with a commenter noting that despite Google&\#x27;s data, TPUs, and advertising revenue it remains behind rivals such as Fable and Astra, and the thread offered little technical analysis of the release itself.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3 . 8 Live &amp; Gemini 3 . 8 Live Extended Thinking</a></li>
<li><a href="https://9to5google.com/2026/09/15/gemini-3-8-live-announced/">Gemini 3 . 8 Live Extended Thinking powers Gemini Live , Gmail</a></li>
<li><a href="https://www.linkedin.com/posts/googledeepmind_meet-gemini-38-live-and-38-live-extended-activity-7505673159484887041-kOy1">Meet Gemini 3 . 8 Live and 3 . 8 Live Extended Thinking : our best...</a></li>

</ul>
</details>

**Tags**: `#Google Gemini`, `#voice AI`, `#LLM release`, `#AI assistants`, `#Hacker News`

---

<a id="item-tech-news-5"></a>
### [Capsule packs web apps and data into one SQLite file](https://withcapsule.app/) ⭐️ 7.0/10

Capsule is a Rust and Tauri 2.0 tool that packages an HTML app, its assets, and user data into a single portable SQLite file, aiming to make local-first HTML applications without hosted storage easier to build and share. The HTML file and related assets are embedded directly in the database, while user data can be stored as localStorage key/value pairs or through a MongoDB-inspired collections API as document rows; PDFs, images, and other assets can also be saved in the file and exported to CSV or JSON. Capsule says documents have no direct file-system access and need permission to access the internet, though the permission model is still being improved, and documents can use local or remote AI models for document-specific features. A known limitation is that multiple people working on the same file create separate copies; to support merging, each data entry carries a unique UUID and timestamp. The author plans to publish the file-format specification with version 1.0 so other applications can read or write Capsule files, and says migrations should prevent data loss when newer app versions are used.

hackernews · bashtian · Sep 15, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49712278)

**「Background」** SQLite is a self-contained embedded database format that can store tables and binary blobs in one file, which is why Capsule uses it as both application archive and data store. Tauri 2.0 is a Rust framework that builds desktop applications around web frontends. Local-first software generally aims to keep user data on the user&\#x27;s device and under their control, but it faces challenges around sharing, synchronization, and merge conflicts.

**「Impact」** Developers can distribute small local tools as a single SQLite file that contains both UI and data, simplifying sharing compared with hosted backends, but Capsule remains an early-stage project and its lack of built-in device sync and app/data separation limits collaborative and update-heavy workflows. The planned 1.0 file-format specification is not yet available, so third-party read/write support is still prospective.

**「Community Discussion」** Commenters liked the local-first packaging idea, noted parallels to sqlar-based or executable-as-SQLite approaches, and one pointed to a similar project called uapp that runs in browsers and Tauri on desktop and Android, but others questioned whether Capsule adds value over the File System Access API or simply sharing the initial application. Additional requested features included device-to-device sync, separation of app code from user data for sharing, and app updates that preserve existing data.

**Tags**: `#SQLite`, `#local-first`, `#Tauri`, `#Rust`, `#web apps`

---

<a id="item-tech-news-6"></a>
### [Show HN: Hacking a $20 4G Hotspot into a Texting Device](https://bkovac.github.io/modem-thing/) ⭐️ 7.0/10

A Show HN project demonstrates turning a $20 4G wireless hotspot into a functional texting device. The provided analysis characterizes it as a detailed hardware-hacking effort that repurposes cheap mobile hardware, with positive technical discussion around its practical use as a dumbphone. Because the linked source content was not supplied, specific implementation details such as the exact hotspot model, firmware changes, and messaging stack cannot be verified from the available material. The item is not framed as a major industry breakthrough, but it is notable for embedded-systems and hardware enthusiasts interested in low-cost device modding.

hackernews · bobili1234 · Sep 15, 13:20 · [Discussion](https://news.ycombinator.com/item?id=49712102)

**「Background」** A portable 4G hotspot is a battery-powered LTE modem that shares its cellular data connection over Wi-Fi and usually exposes only a minimal web interface for SIM and network settings, so it has no way to display incoming SMS. Thanks to supply-chain economics, fully unlocked units that pack Wi-Fi, Bluetooth, a display, and a battery can be bought for under $20 shipped, which makes them cheap raw material for hardware repurposing. The project exploits that gap: the hardware already contains the radio and SIM slot needed to send and receive texts, and the challenge is adding an interface and software layer for them. Several such hotspots are built on older Qualcomm MSM8916-series smartphone silicon, a chipset the hobbyist community has adapted to run Linux or Android, giving hackers a familiar software base to build on.

**「Impact」** Owners of the same MSM8916-based $20 hotspot can follow this project and the OpenStick Linux flashing route to turn the modem into a standalone texting device, giving users who want to leave their smartphone behind a working dumbphone for SMS and OTP retrieval. The approach stays limited to that specific modem family and still depends on added components such as the Clicks keyboard and Sharp memory display, so it is not a general-purpose fix for other hotspots.

**「Community Discussion」** Commenters were positive about the project, with one saying they had just bought a $10 4G dongle and might inspect it, and another describing the modified hotspot as a workable dumbphone for viewing texts and OTPs without moving the SIM into a phone. Others suggested extending battery life by adding two high-quality 18650 cells in parallel, praised the reuse of a Clicks keyboard, speculated about running an agent system such as Hermes if an OpenStick build has enough RAM and storage, and noted that some MSM8916-based dongles run an Android UI despite lacking a display.

<details><summary>References</summary>
<ul>
<li><a href="https://vuink.com/post/oxbinp-d-dtvguho-d-dvb/modem-thing">Converting a $20 4G wireless hotspot into a texting device</a></li>
<li><a href="https://blog.adafruit.com/2026/09/15/converting-a-20-4g-wireless-hotspot-into-a-texting-device/">Converting a $20 4G wireless hotspot into a texting device</a></li>
<li><a href="https://github.com/Muhammad-Yunus/OpenStick-MSM8916">GitHub - Muhammad-Yunus/OpenStick-MSM8916: Repurpose your USB ...</a></li>

</ul>
</details>

**Tags**: `#hardware-hacking`, `#embedded-systems`, `#4g-lte`, `#modding`, `#show-hn`

---

<a id="item-tech-news-7"></a>
### [SHADOW-50M: 44M-parameter ternary LLM runs offline in 19.8 MB](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

A Reddit author \(/u/Final-Data-1410\) released SHADOW-50M, a 44M-parameter LLM trained from scratch on 45B tokens that ships as a 19.8 MB complete model and runs offline at about 1,900 tok/s on a laptop CPU and roughly 500 tok/s in a browser via a WebAssembly build of the same 159 KB compiled kernel. The model uses ternary \{-1,0,+1\} weights, a 73,880-token vocabulary represented by fixed 512-bit fingerprints instead of a trained embedding, and fixed readout circuits for arithmetic, percentages, dates, weekdays, units, counting, sorting, comparisons, and a small program machine; when it encounters something like \[calc\]347\*86\[eq\], a circuit fills in the digits in the same token stream without a calculator API or tool call. For persistent memory, SHADOW stores each record’s attention state to disk at 1 bit \(288 bytes/token\) with a 22-byte/token index, allowing retrieval in roughly a microsecond and reinjection in about 0.03 ms without re-reading text; at 100M tokens the archive is 28.8 GB plus a 2.2 GB index while the process uses about 28 MB RAM via memory mapping. The author reports SHADOW underperforms a 51.8M-parameter Llama-style bf16 model, Supra-50M-Reasoning, on every standard benchmark tested—ARC-Easy 0.307 vs 0.435, PIQA 0.570 vs 0.600, and WikiText-2 perplexity 186 vs 165—but shows side-by-side examples where SHADOW answers jokes, arithmetic, percentages, dates, and record-retrieval questions while Supra fails, and notes that a frozen fingerprint-table update added 8,600 missing English word pieces without training while keeping 34/34 previously published answers unchanged. The work is a proof of concept, not a product, released under the MIT license with public weights, code, and browser demo; documented weaknesses include thin general knowledge, poor creative writing, occasional mis-copying of seven-digit operands, and large archives sometimes pulling an unrelated record into a numeric question.

reddit · r/MachineLearning · /u/Final-Data-1410 · Sep 15, 12:59

**「Background」** Ternary-weight language models constrain every weight to \{-1, 0, +1\}, which sharply reduces model size and suits fast CPU inference at some cost in quality. SHADOW-50M is the smaller follow-up to the author&\#x27;s earlier SHADOW-250M, a 60 MB model that ran roughly 400 tok/s on CPU, and its repository describes it as a 44M-parameter ternary model with exact circuits plus a 100M-token archive held on disk. Unlike a conventional LLM, it replaces the trained embedding with a frozen fingerprint table and stores retrieved attention state as bytes on disk rather than re-reading text, which is what makes the 19.8 MB offline footprint possible.

**「Impact」** For local and edge inference developers, this proof of concept shows a 19.8 MB ternary model can run entirely offline on CPU and in WebAssembly at high token rates with disk-backed persistent memory, but its weaker standard benchmarks and single-source, unverified status mean it should be treated as an experiment rather than a drop-in replacement for larger models.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/QLNI/SHADOW-50M-Instruct">GitHub - QLNI/SHADOW-50M-Instruct: SHADOW 50M Instruct: a 44M ...</a></li>
<li><a href="https://github.com/QLNI/SHADOW-50M-Instruct/blob/main/ROADMAP.md">SHADOW-50M-Instruct/ROADMAP.md at main · QLNI ... - GitHub</a></li>
<li><a href="https://trendshift.io/repositories/235132">QLNI/SHADOW-50M-Instruct — GitHub trending stats &amp; insights</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#CPU inference`, `#ternary weights`, `#WebAssembly`

---

<a id="item-tech-news-8"></a>
### [TabPFN-3.5 Released as SOTA Tabular Foundation Model](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 7.0/10

Prior Labs announced the release of TabPFN-3.5, claiming it is the top model on both TabArena and BeyondArena and state-of-the-art for datasets with 1M rows and up to 20k features. The release includes three variants: TabPFN-3.5-Fast, which is in alpha and claimed to run 6x faster than the base model; TabPFN-3.5-Thinking, which trades compute for better accuracy and is available via API; and TabPFN-3.5-Plus. On BeyondArena, Prior Labs says TabPFN-3.5 leads on text-rich, high-cardinality, and high-dimensional data, with +250 Elo points over the strongest previous baseline and +150 Elo points ahead of the previous overall leader. The company also claims TabPFN-3.5-Thinking improves on the base model by +20 Elo on BeyondArena and +44 Elo on TabArena. The item is a Reddit announcement, so these benchmark and performance claims have not been independently verified in the supplied content.

reddit · r/MachineLearning · /u/tuanacelik · Sep 15, 16:18

**「Background」** TabPFN is a transformer-based machine learning model for tabular datasets introduced in 2022, designed for supervised classification and regression and originally focused on small- to medium-sized tables. Prior Labs develops the model, and its code and TabPFN-2 weights are released under a Prior Labs License \(Apache 2.0 with an additional attribution requirement\). TabPFN-3.5 arrives after the earlier TabPFN-3 generation, which Prior Labs presents as its tabular foundation model for state-of-the-art predictions on structured data.

**「Impact」** Practitioners choosing a tabular baseline gain a stronger default: TabPFN-3.5 claims top placement on TabArena and BeyondArena while scaling to 1M rows and up to 20k features, and the Fast \(6x faster, alpha\), Thinking \(API-based compute-for-accuracy, +20 Elo on BeyondArena, +44 Elo on TabArena\), and Plus variants give explicit latency-versus-accuracy tradeoffs — a meaningful shift for the ecosystem that already builds on TabPFN and TabPFNv2. These results are vendor-reported in a Reddit announcement with no independent verification, so the benchmark and speedup claims should be treated as provisional until reproduced.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TabPFN">TabPFN - Wikipedia</a></li>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/ TabPFN : TabPFN : Foundation Model for Tabular ...</a></li>
<li><a href="https://priorlabs.ai/tabpfn">TabPFN | Prior Labs</a></li>
<li><a href="https://www.researchgate.net/publication/397555905_TabPFN-25_Advancing_the_State_of_the_Art_in_Tabular_Foundation_Models">(PDF) TabPFN -2.5: Advancing the State of the Art in Tabular ...</a></li>
<li><a href="https://arxiv.org/html/2511.08667">1 TabPFN -2.5 performance on the standard TabArena -lite benchmark ...</a></li>

</ul>
</details>

**Tags**: `#tabular data`, `#foundation models`, `#machine learning`, `#benchmarks`, `#model release`

---

<a id="item-tech-news-9"></a>
### [Sanders Bill Would Ban Superintelligent AI With 20-Year Penalties](https://www.techspot.com/news/113831-new-bernie-sanders-bill-would-ban-superintelligent-ai.html) ⭐️ 7.0/10

A reported U.S. bill backed by Senator Bernie Sanders and Representative Casar would permanently ban the development and deployment of superintelligent AI and pause advanced AI development until federal regulators set safety rules. It also pushes for an international agreement to stop superintelligence from emerging globally. Violations would carry up to 20 years in prison, companies could face a &quot;corporate death penalty,&quot; and the measure would create a cabinet-level agency to monitor dangerous capabilities across stages of frontier AI systems and oversee their removal. The bill is a proposal, not enacted law, and its practical impact remains uncertain.

telegram · zaihuapd · Sep 15, 04:26

**「Background」** Superintelligent AI generally refers to systems whose capabilities match or exceed human cognitive performance across a wide range of tasks; the Sanders-Casar proposal would permanently ban developing or deploying such systems and temporarily pause advanced AI development until federal safety rules are in place. The measure, announced in a Sept. 3, 2026 press release from Sanders&\#x27; office, would impose up to 20 years in prison for violations and create a cabinet-level body to monitor and remove dangerous frontier capabilities. It remains a bill proposal, not enacted law, so its requirements and penalties are not currently in force.

**「Impact」** If enacted, U.S. frontier AI developers would face a permanent legal prohibition on creating or deploying superintelligent systems, with individuals exposed to up to 20 years&\#x27; imprisonment and companies to a corporate &quot;death penalty,&quot; alongside an open-ended pause on advanced AI development until federal safety rules are in place and a new cabinet-level agency is monitoring and removing dangerous frontier capabilities. Because the Sanders-Casar Ban Artificial Superintelligence Act is a forthcoming proposal rather than enacted law, no compliance obligation or enforcement risk currently applies to developers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sanders.senate.gov/press-releases/news-sanders-casar-introduce-legislation-to-ban-artificial-superintelligence-and-temporarily-pause-advanced-ai-development/">NEWS: Sanders, Casar to Introduce Legislation to Ban Artificial ...</a></li>
<li><a href="https://garymarcus.substack.com/p/the-new-sanders-casar-ban-artificial">The new Sanders-Casar Ban Artificial Superintelligence Act - Marcus on AI</a></li>
<li><a href="https://www.sanders.senate.gov/press-releases/news-sanders-casar-introduce-legislation-to-ban-artificial-superintelligence-and-temporarily-pause-advanced-ai-development/">NEWS: Sanders, Casar to Introduce Legislation to Ban Artificial ...</a></li>
<li><a href="https://garymarcus.substack.com/p/the-new-sanders-casar-ban-artificial">The new Sanders-Casar Ban Artificial Superintelligence Act - Marcus on AI</a></li>
<li><a href="https://forum.effectivealtruism.org/posts/vt5nzkkjecXH4yYf7/sen-bernie-sanders-i-vt-and-rep-greg-casar-d-tx-introduce">Sen. Bernie Sanders (I-VT) and Rep. Greg Casar (D-TX) introduce ...</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#superintelligence`, `#AI safety`, `#technology policy`, `#legislation`

---

<a id="item-tech-news-10"></a>
### [Google Reportedly Opens Anthropic&\#x27;s Claude to All Its Engineers](https://www.businessinsider.com/google-finally-lets-all-engineers-use-anthropics-claude-2026-9) ⭐️ 7.0/10

Google has reportedly opened Anthropic&\#x27;s strongest coding model, Claude \(Opus 5\), to engineers across the company for internal development, but access is limited to Google&\#x27;s internal development platform, Antigravity. Previously, Google generally barred most employees from using external coding tools such as Claude Code and OpenAI&\#x27;s Codex, directing them to its own Gemini instead. A Google spokesperson said Gemini remains the primary model for internal development, while Claude is offered on a per-employee quota as a supplement. The change is being read as a response to competitive pressure in AI coding tools. Google is an investor in Anthropic and earlier this year announced plans to invest up to $40 billion in the company, according to Business Insider&\#x27;s report.

telegram · zaihuapd · Sep 15, 05:31

**「Background」** Antigravity is Google&\#x27;s internal agentic development environment, designed around AI agents taking on substantial portions of software work rather than acting as a code-completion layer alone. Before this change, Google&\#x27;s long-standing internal policy directed engineers to build with its own Gemini model and to avoid external coding tools such as Anthropic&\#x27;s Claude Code and OpenAI&\#x27;s Codex. Google is also an investor in Anthropic, having announced plans to put up to $40 billion into the company, a relationship that also locks Anthropic in as a major customer for Google&\#x27;s TPUs.

**「Impact」** Google engineers who were previously required to use Gemini for internal development can now reportedly run Anthropic&\#x27;s Claude Opus 5 inside the Antigravity platform, subject to per-employee quotas, while Gemini remains the primary model. The arrangement is limited to that internal platform, so it does not extend to unrelated external coding tools.

<details><summary>References</summary>
<ul>
<li><a href="https://promtime.net/c/en/post/googlers-finally-get-claude-but-only-inside-antigravity">Googlers finally get Claude , but only inside Antigravity · News</a></li>
<li><a href="https://fourweekmba.com/ai-google-claude-opus-5-antigravity-harness-theory/">Google Opens Anthropic&#x27;s Claude Opus 5 to All Engineers — and ...</a></li>
<li><a href="https://www.clauder-navi.com/en/google-claude-anthropic">Google Invests Up to $40 Billion in Anthropic | Impact on Claude</a></li>

</ul>
</details>

**Tags**: `#AI coding tools`, `#Google`, `#Anthropic`, `#enterprise AI adoption`, `#developer tooling`

---

<a id="item-tech-news-11"></a>
### [MediaTek launches Dimensity 9600 Pro on TSMC 2nm, plus 9600M](https://www.reuters.com/business/media-telecom/mediatek-launches-new-mobile-chip-using-tsmcs-most-advanced-technology-2026-09-15/) ⭐️ 7.0/10

On September 15, MediaTek announced the Dimensity 9600 Pro, its first smartphone processor manufactured using TSMC&\#x27;s 2nm process, alongside the Dimensity 9600M, which uses a 3nm process. MediaTek said the first phones carrying both chips will launch soon. The Dimensity 9600 Pro includes a dedicated AI processor and is claimed to improve performance by 51% over the previous generation when processing user prompts before model generation begins. The launch is notable as MediaTek&\#x27;s first mobile processor on TSMC&\#x27;s 2nm node. The announcement did not include benchmarks, detailed specifications, or independent verification.

telegram · zaihuapd · Sep 15, 08:57

**「Background」** MediaTek&\#x27;s Dimensity line is its flagship smartphone system-on-chip family, and node names such as 3nm and 2nm describe the manufacturing process used by the foundry — here TSMC — where a smaller node generally allows more transistors per area and better power efficiency. MediaTek says it is the first company to announce a mobile chip at the 2nm node, making the Dimensity 9600 Pro a generational step for on-device AI and performance work, while the Dimensity 9600M launches alongside it on the more mature 3nm process. Both chips were announced on September 15, 2026, with MediaTek stating that the first phones carrying them will arrive soon.

**「Impact」** Smartphone makers adopting the Dimensity 9600 Pro can ship the first 2nm flagship phones with MediaTek&\#x27;s claimed 51% faster AI prompt processing and reported on-device 30B-parameter LLM capability, with first devices promised soon. Those gains and the 2nm milestone currently rest on MediaTek&\#x27;s own launch figures rather than independent benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mediatek.com/press-room/mediatek-dimensity-9600-pro-sets-new-standard-for-flagship-smartphone-chips">MediaTek Dimensity 9600 Pro Sets New Standard for Flagship ...</a></li>
<li><a href="https://shattered.io/mediatek-dimensity-9600-pro-2nm-launch-2026/">MediaTek Dimensity 9600 Pro: 2nm Chip Cuts Power 61%</a></li>
<li><a href="https://9to5google.com/2026/09/15/mediatek-dimensity-9600-pro-chip/">MediaTek Dimensity 9600 Pro debuts with 2nm, performance gains</a></li>
<li><a href="https://www.mediatek.com/press-room/mediatek-dimensity-9600-pro-sets-new-standard-for-flagship-smartphone-chips">MediaTek Dimensity 9600 Pro Sets New Standard for Flagship ...</a></li>
<li><a href="https://hothardware.com/news/mediatek-dimensity-9600-pro-30b-ai-up-to-185fps-gaming">MediaTek Dimensity 9600 Pro Goes 2nm With 30B-Parameter AI ...</a></li>
<li><a href="https://9to5google.com/2026/09/15/mediatek-dimensity-9600-pro-chip/">MediaTek Dimensity 9600 Pro debuts with 2nm, performance gains</a></li>

</ul>
</details>

**Tags**: `#MediaTek`, `#Dimensity 9600 Pro`, `#TSMC 2nm`, `#mobile SoC`, `#on-device AI`

---

<a id="item-tech-news-12"></a>
### [OpenAI Contractors Read Real ChatGPT Chats in &\#x27;Project Lily&\#x27;](https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/) ⭐️ 7.0/10

A 404 Media report says OpenAI is employing hundreds of contract workers to read large volumes of real ChatGPT prompts and full conversations, score the model&\#x27;s replies, and suggest revisions. The work may expose sensitive personal information. OpenAI said it tries to delete personal information before reviewers see it, but acknowledged that sensitive details may still be visible. Anthropic also confirmed that it uses human review to improve its models.

telegram · zaihuapd · Sep 15, 11:56

**「Background」** AI developers commonly use human reviewers and data annotation—often described as reinforcement learning from human feedback—to evaluate and improve model responses. According to 404 Media&\#x27;s reporting, based on leaked internal documents and real prompts it reviewed, &quot;Project Lily&quot; is OpenAI&\#x27;s internal codename for a program in which hundreds of contractors review real ChatGPT conversations, summarizing user requests, comparing four responses, and scoring response quality on a 1–7 scale. Contractors were reportedly recruited by Crossing Hurdles and paid via Mercor, with one worker reporting over $50 per hour.

**「Impact」** The people most directly affected are ChatGPT consumers whose prompts and full conversations may be read by hundreds of contract reviewers, since OpenAI acknowledges sensitive details can still be visible after its redaction attempts — and reporting on the case notes that the duty to tell users sits with the company collecting their data. For organizations, the exposure is compounded because employee use of consumer AI accounts falls outside enterprise agreements that limit training and review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/">Inside ‘Project Lily’: The Humans Reading Your ChatGPT Chats</a></li>
<li><a href="https://aiweekly.co/alerts/404-media-openai-project-lily-hires-hundreds-of-contractors-to-read-real">404 Media: OpenAI &#x27;Project Lily&#x27; Hires Hundreds of ...</a></li>
<li><a href="https://letsdatascience.com/news/openai-reportedly-uses-contractors-to-review-chatgpt-convers-afe1c797">OpenAI Reportedly Uses Contractors to Review ChatGPT ...</a></li>
<li><a href="https://thenextweb.com/news/chatgpt-human-reviewers-gdpr">Hundreds of contractors are reportedly reading real ChatGPT ...</a></li>
<li><a href="https://cryptobriefing.com/openai-anthropic-enterprise-data-privacy/">OpenAI and Anthropic address enterprise data privacy concerns ...</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#OpenAI`, `#human review`, `#data annotation`, `#AI industry`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Saudi East-West Pipeline Shutdown Squeezes Oil Market](https://oilprice.com/Energy/Crude-Oil/Saudi-Pipeline-Outage-Hits-an-Oil-Market-Running-Out-of-Buffers.html) ⭐️ 9.0/10

Drone attacks have shut Saudi Arabia&\#x27;s East-West oil pipeline, cutting a route that had been moving roughly 4 million barrels per day of Saudi crude to the Red Sea port of Yanbu. U.S. Energy Secretary Chris Wright said Tuesday repairs could take days rather than weeks, after earlier estimates that the outage might last several weeks.

rss · OilPrice.com · Sep 16, 00:00

**「Background」** The 1,200-kilometer pipeline let Saudi Arabia bypass the Strait of Hormuz, which has been largely closed to tanker traffic since March, and the International Energy Agency says global observed oil inventories have fallen by a cumulative 507 million barrels since February, leaving little cushion.

**「Impact」** Saudi Aramco has already canceled or delayed late-September crude cargoes to European refiners, with Poland&\#x27;s Orlen buying North Sea crude and seeking U.S. and Kazakh grades, while Asian refiners scramble for October supply.

**Tags**: `#oil markets`, `#Saudi Arabia`, `#energy supply disruption`, `#Strait of Hormuz`, `#IEA inventories`

---

<a id="item-finance-news-2"></a>
### [Hormuz Risk Splits Crude Prices as Brent Tops $107](https://oilprice.com/Energy/Crude-Oil/Hormuz-Risk-Opens-40-Plus-Price-Gap-Between-Crude-Grades.html) ⭐️ 9.0/10

Brent crude is trading above $107 a barrel and WTI near $103, while Iraq&\#x27;s Basrah Medium is offered at a $43.06-a-barrel discount to the Murban benchmark, which trades above $127. Per Reuters&\#x27; Clyde Russell, citing Argus and Windward data, the gap reflects the different prices for oil that must pass through the Strait of Hormuz and oil that does not.

rss · OilPrice.com · Sep 15, 22:00

**「Background」** The Strait of Hormuz is the narrow waterway through which most Gulf crude must pass, making it the world&\#x27;s most important oil transit chokepoint; the war between the U.S. and Israel and Iran disrupted shipping there, and a U.S. naval blockade is also cited in the source. Because oil loaded inside the Gulf carries attack and insurance risk that oil loaded outside it does not, buyers are demanding steep discounts on Gulf-loaded grades while freely traded blends command premiums.

**「Impact」** Asian refiners are already adapting: Chinese independent refiners and Indian buyers have bought more Russian ESPO crude, which traded up to $10 a barrel above Brent this month, to replace Iranian barrels blocked in the Gulf.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eia.gov/todayinenergy/detail.php?id=61002">The Strait of Hormuz is the world&#x27;s most important oil transit...</a></li>

</ul>
</details>

**Tags**: `#oil markets`, `#Strait of Hormuz`, `#crude prices`, `#geopolitical risk`, `#energy supply`

---

<a id="item-finance-news-3"></a>
### [Federal Reserve Holds Interest Rates Steady, Signals Possible Hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

The Federal Reserve left its benchmark interest rate unchanged, according to CBS News, while indicating it could still raise rates later. The decision keeps borrowing costs for households and businesses at their current level, with the possibility of an increase rather than a cut ahead.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The federal funds rate is the benchmark for overnight lending between banks and anchors borrowing costs on mortgages, credit cards and business loans. It has been held in a target range of 3.5% to 3.75%, and this decision came in a 9–3 vote in which three officials favored a quarter-point increase — the first such meeting under chair Kevin Warsh, who took office on May 22, 2026.

**「Impact」** With the federal funds rate held at 3.50%–3.75% for a fifth consecutive meeting, households and businesses with variable-rate debt get no relief: Fed minutes describe borrowing costs as still elevated relative to their post-2008 average, while core inflation ran at 3.3% in June 2026 versus the Fed&\#x27;s 2% goal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anews.com.tr/americas/2026/07/29/us-federal-reserve-holds-rates-steady-as-3-policymakers-back-hike">US Federal Reserve holds rates steady as 3 policymakers back hike</a></li>
<li><a href="https://www.federalreserve.gov/aboutthefed/bios/board/warsh.htm">Federal Reserve Board - Kevin Warsh, Chairman</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-tapering-asset-purchases.html">Federal Reserve Monetary Policy | U.S. Bank</a></li>
<li><a href="https://www.federalreserve.gov/monetarypolicy/fomcminutes20251029.htm">FOMC Minutes, October 28-29, 2025</a></li>
<li><a href="https://pgpf.org/article/higher-interest-rates-will-raise-interest-costs-on-the-national-debt/">The Fed Held Its Target Range For the Fifth Meeting in a Row but Interest Costs Remain High</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#US economy`

---

<a id="item-finance-news-4"></a>
### [China&\#x27;s August retail sales miss forecast as investment slump deepens](https://www.cnbc.com/2026/09/15/china-august-retail-sales-industrial-output-investment-exports-.html) ⭐️ 8.0/10

China&\#x27;s retail sales grew 0.4% in August from a year earlier, slowing from 0.6% in July and below the 0.8% economists had forecast in a Reuters poll. Urban fixed-asset investment, which covers property and infrastructure, fell 7.2% in January–August from a year earlier, steeper than the 6.7% decline in January–July, the National Bureau of Statistics said.

rss · CNBC Finance · Sep 15, 09:46

**「Background」** China&\#x27;s economy grew 4.3% in the second quarter, its weakest pace in more than three years, and Beijing has so far relied on incremental measures rather than aggressive stimulus to reach its 2025 target of 4.5% to 5% growth.

**「Impact」** Weak borrowing appetite is adding to Beijing&\#x27;s problem: new bank loans rose just 60 billion yuan \($8.95 billion\) in August against a forecast of about 400 billion yuan, with outstanding loan growth at a record-low 4.9%, and analysts at ANZ Research said September could be an important policy window for more fiscal support.

**Tags**: `#China economy`, `#retail sales`, `#fixed-asset investment`, `#credit growth`, `#macro policy`

---

<a id="item-finance-news-5"></a>
### [U.S. Diesel Sets New Weekly Price Record, 2026 Annual Record Within Reach](https://oilprice.com/Energy/Energy-General/US-Diesel-Prices-on-Track-for-Record-Year.html) ⭐️ 8.0/10

U.S. on-highway diesel prices rose 36.8 cents to $5.967 a gallon for the week of Sept. 7, surpassing the previous nominal weekly record of $5.810 set in June 2022, according to EIA data. Using EIA weekly prices, the article&\#x27;s author calculates a 2026 year-to-date average of about $4.895 a gallon versus the 2022 annual record of $4.989, meaning diesel would need to average about $5.20 over the remaining 16 weeks to set an annual record — a result the author calls possible but not assured.

rss · OilPrice.com · Sep 15, 16:00

**「Background」** The 2022 records followed pandemic-era refining closures, low inventories and Russia&\#x27;s invasion of Ukraine, while the article attributes the 2026 squeeze to the conflict involving Iran, reduced flows through the Strait of Hormuz and damage to Russian refineries.

**「Impact」** Because diesel powers trucking, farming, construction and rail equipment, sustained high prices raise operating costs for those businesses and can feed into broader consumer prices.

**Tags**: `#diesel prices`, `#energy inflation`, `#EIA data`, `#U.S. economy`, `#oil markets`

---

<a id="item-finance-news-6"></a>
### [China&\#x27;s industry and planning ministries issue 15th Five-Year Plan for electronics manufacturing](https://www.secrss.com/articles/93961) ⭐️ 8.0/10

China&\#x27;s Ministry of Industry and Information Technology and the National Development and Reform Commission have jointly issued the 15th Five-Year Plan for the electronic information manufacturing industry, laying out 17 tasks that include raising advanced chipmaking process capability, developing high-end smartphone core chips and high-performance PC chips, and expanding the use of domestic operating systems such as OpenHarmony. The plan targets combined revenue of more than 30 trillion yuan for industrial enterprises above a designated size by 2030, with research and development spending reaching 3.5% of revenue, and also covers RISC-V, AI chips and devices, and the BeiDou satellite system.

telegram · zaihuapd · Sep 15, 03:10

**「Background」** Five-year plans are China&\#x27;s top-level planning documents, which set direction for ministries, state-owned firms and local governments; this one covers the 2026–2030 period but is itself a policy framework rather than an implemented subsidy or regulation.

**「Impact」** The plan points policy support toward domestic chip designers, PC and smartphone manufacturers, and developers of domestic operating-system ecosystems, though it does not specify the funding or enforcement measures that would follow.

**Tags**: `#中国半导体政策`, `#十五五规划`, `#国产芯片`, `#鸿蒙操作系统`, `#产业政策`

---

<a id="item-finance-news-7"></a>
### [Chinese Solar Panels at 12 Cents a Watt Drive Global Rooftop Boom](https://oilprice.com/Alternative-Energy/Solar-Energy/Chinese-Solar-Panels-Drop-to-12-Cents-a-Watt-Rooftop-Installs-Surge-Worldwide.html) ⭐️ 7.0/10

Chinese-made solar panels cost 12 cents a watt in 2026, down from $5–$6 at the turn of the millennium, according to the Financial Times, and that price collapse is spurring rooftop and small-scale solar adoption worldwide. The report cites a Pakistani cement maker cutting power costs by up to 40%, Philippine rooftop capacity nearly doubling in a year, Africa on pace for a record 17 GW of solar in 2026 \(a 45% year-on-year increase\), and panels on more than 4 million Australian homes.

rss · OilPrice.com · Sep 15, 23:00

**「Background」** The price collapse stems largely from severe manufacturing overcapacity in China, which has pushed down costs across the solar supply chain.

**「Who is affected」** Australian households and electricity grid operators face growing strain from that adoption: rooftop solar now provides 14.2% of the country&\#x27;s electricity generation, nearly double its 2020 share, and its 28.3 GW of rooftop capacity exceeds the national coal fleet&\#x27;s 22.5 GW, making it harder to balance supply on the grid.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/solar-shakeout-why-panel-prices-crashed-50-what-means-sydney-westrick-nvxzc">The Solar Shakeout: Why Panel Prices Crashed 50% and What It...</a></li>
<li><a href="https://dimensionmarketresearch.com/report/china-solar-module-manufacturing-equipment-market/">China Solar Module Manufacturing Equipment Market 2026 -2035</a></li>
<li><a href="https://cosmicrenewableenergy.com.au/articles/rooftop-solar-surpasses-coal-28gw-australia-2025/">Australia&#x27;s Rooftop Solar Hits 28.3 GW — Now Bigger Than the ...</a></li>
<li><a href="https://cleanenergycouncil.org.au/news-resources/rooftop-solar-and-storage-report-july-to-dec-2025">Clean Energy Council Rooftop solar and storage report - July ...</a></li>

</ul>
</details>

**Tags**: `#solar panels`, `#China manufacturing`, `#distributed energy`, `#energy transition`, `#India subsidies`

---

<a id="item-finance-news-8"></a>
### [ADNOC Buys Discounted Iraqi Crude, Freeing UAE Barrels for Export](https://oilprice.com/Latest-Energy-News/World-News/ADNOC-Scoops-Up-Iraqi-Crude-at-25-Per-Barrel-Discount.html) ⭐️ 7.0/10

ADNOC agreed to buy 32 million barrels of Iraqi crude for August at discounts of $24.90 to $27 per barrel and another 40 million barrels for September, according to sources cited by Reuters, though actual August liftings reached only about 20 million barrels because Iraqi export constraints limited supply. ADNOC plans to process much of the crude at its Ruwais refinery and sell more of its own UAE crude abroad, which can be shipped from Fujairah outside the Strait of Hormuz.

rss · OilPrice.com · Sep 15, 18:30

**「Background」** Iraq has historically exported most of its crude through the Persian Gulf and the Strait of Hormuz, a chokepoint that averaged about 20 million barrels per day of crude and oil products in 2025. ADNOC&\#x27;s Ruwais complex is one of the world&\#x27;s largest refineries and can process heavier, higher-sulfur crudes.

**「Who is affected」** Iraq, whose exports fell to 1.374 million bpd in July, is effectively selling at $24.90–$27 per barrel below market to move volumes, squeezing the oil revenue its budget depends on, while buyers with logistics that bypass the Strait of Hormuz — ADNOC, which will run the crude through its Ruwais refinery, plus PetroChina, Zhenhua Oil, TotalEnergies, Vitol, Trafigura, Mercuria and Cathay Petroleum — secure cheaper feedstock.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ruwais_refinery">Ruwais refinery - Wikipedia</a></li>
<li><a href="https://www.spglobal.com/energy/en/news-research/latest-news/crude-oil/050724-uaes-adnoc-transforms-ruwais-refinery-as-murban-exports-hit-eight-year-high">UAE&#x27;s ADNOC transforms Ruwais refinery as Murban exports hit eight ...</a></li>
<li><a href="https://www.iea.org/about/oil-security-and-emergency-response/strait-of-hormuz">Strait of Hormuz - About - IEA</a></li>
<li><a href="https://energynews.oedigital.com/crude-oil/2026/09/15/sources-say-that-adnoc-the-uaes-oil-company-buys-millions-barrels-of-iraqi-crude">Sources say that ADNOC , the UAE&#x27;s oil company , buys millions...</a></li>
<li><a href="https://thecradle.co/articles/uae-state-oil-company-buys-up-discounted-iraqi-oil">UAE state oil company buys up discounted Iraqi oil</a></li>

</ul>
</details>

**Tags**: `#oil-markets`, `#Iraqi-crude`, `#ADNOC`, `#Strait-of-Hormuz`, `#commodity-trading`

---

<a id="item-finance-news-9"></a>
### [Libya&\#x27;s NOC Threatens Force Majeure After Oilfield Shutdowns](https://oilprice.com/Latest-Energy-News/World-News/Libya-Threatens-Force-Majeure-as-Oil-Guards-Shut-Fields.html) ⭐️ 7.0/10

Libya&\#x27;s National Oil Corporation said it could declare force majeure after members of the Petroleum Facilities Guard closed a valve on the Hamada-Zawiya crude pipeline, halting output at the Hamada and Tahara oilfields and a pumping station. The Guard said it would impose partial production cuts for one week at the Wafa, Al-Khamsa and El Feel fields, escalating to a full shutdown if its demand is not met: a financial and administrative transfer from the defense ministry to the NOC with a timetable.

rss · OilPrice.com · Sep 15, 16:30

**「Background」** Political groups, armed factions and workers have repeatedly used oilfields, pipelines and terminals as leverage since the 2011 uprising that toppled Muammar Gaddafi. The disruption comes as Libya&\#x27;s output has reached roughly 1.4 million barrels per day, its highest in more than a decade, against an NOC target of 1.6 million bpd by the end of 2026.

**Tags**: `#Libya`, `#oil production`, `#force majeure`, `#National Oil Corporation`, `#oil markets`

---

<a id="item-finance-news-10"></a>
### [FERC Orders Mandatory Reliability Standards for AI Data Centers](https://oilprice.com/Energy/Energy-General/Can-The-Power-Grid-Handle-AI-And-Wildfires-At-The-Same-Time.html) ⭐️ 7.0/10

On July 16, the Federal Energy Regulatory Commission ordered the North American Electric Reliability Corporation to write mandatory reliability standards for AI data centers, with a deadline of Dec. 31. The order responds to forecasts cited in the article that U.S. data center IT load will rise from roughly 80 gigawatts today toward 150 gigawatts by 2028, according to Bloom Energy&\#x27;s latest power report, with Gartner expecting power shortages to constrain 40 percent of existing AI data centers by 2027.

rss · OilPrice.com · Sep 15, 15:00

**「Background」** FERC oversees interstate electricity reliability through the North American Electric Reliability Corporation, the federally certified body that writes the mandatory standards grid operators must follow — rules that have historically applied to generators and transmission owners rather than to customers such as data centers. On the wildfire side, the Oregon Court of Appeals reversed a roughly $1 billion verdict against utility PacifiCorp in April over the 2020 Labor Day fires, ruling that the trial judge&\#x27;s jury instruction wrongly required causation to be decided for all the fires at once.

**「Who Is Affected」** AI data center operators would face new interconnection obligations — including supplying utilities with dynamic models, workload profiles and operational telemetry for grid stability analysis — while the regional grids absorbing that load, and their ratepayers, bear the reliability and firm-power costs the Energy Department attributes to rapid, geographically concentrated demand growth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nelsonmullins.com/insights/alerts/megawatt-minute/all/could-data-centers-become-the-next-nerc-regulated-entities">Could Data Centers Become the Next NERC -Regulated Entities?</a></li>
<li><a href="https://www.oregonlive.com/business/2026/04/oregon-appeals-court-hands-big-victory-to-pacificorp-in-wildfire-class-action-suit.html">Oregon appeals court hands big victory to PacifiCorp in ...</a></li>
<li><a href="https://arxiv.org/html/2509.07218v3">Electricity Demand and Grid Impacts of AI Data Centers: Challenges and Prospects</a></li>
<li><a href="https://www.energy.gov/oe/clean-energy-resources-meet-data-center-electricity-demand">Clean Energy Resources to Meet Data Center Electricity Demand | Department of Energy</a></li>

</ul>
</details>

**Tags**: `#AI data centers`, `#Power grid reliability`, `#FERC regulation`, `#Wildfire liability`, `#Utilities`

---

<a id="item-finance-news-11"></a>
### [中国发布共享单车服务新国标，2026年11月起实施](https://ysxw.cctv.cn/article.html?toc_style_id=feeds_default&amp;amp;t=1789434965546&amp;amp;item_id=10192909235938930936&amp;amp;channelId=1119) ⭐️ 7.0/10

中国市场监管总局发布共享单车服务新国家标准，将于2026年11月实施，对运营企业提出人员管理、设施配置、租还车服务、用户信息保护和车辆投放停放五方面要求。标准要求车辆配备唯一性编码和车载智能终端、平台设置24小时服务热线、用户实名登记，并利用电子围栏等技术引导规范停车和及时清理违规停放车辆。

telegram · zaihuapd · Sep 15, 02:40

**「Background」** A national standard \(国标\) is a technical rule for an industry; this one was issued by the State Administration for Market Regulation and takes effect in November 2026. Because shared bikes are unlocked and returned through apps and left on public streets, the rules cover the whole operating chain — staffing, equipment, renting and returning, user data and vehicle deployment.

**「Impact」** Shared-bike operators would face higher staffing, equipment and compliance costs, since the standard requires dedicated parking-order, redistribution, repair, maintenance and cleaning staff plus a unique code and on-board smart terminal for every bike and a 24-hour service hotline.

<details><summary>References</summary>
<ul>
<li><a href="https://m.gmw.cn/2026-09/15/content_1304564036.htm">共享单车新国标发布！将于今年11月实施！</a></li>
<li><a href="https://m.gmw.cn/2026-09/15/content_1304563985.htm">一车一码、24小时热线……共享单车新国标来了，这些变化与你有关</a></li>
<li><a href="https://news.futunn.com/post/79265394">共享单车新国标落地：一车一码，重点整治乱停放</a></li>

</ul>
</details>

**Tags**: `#共享单车`, `#新国标`, `#市场监管总局`, `#行业监管`, `#运营服务`

---

<a id="item-finance-news-12"></a>
### [10-year Treasury Yield Reaches 2007 High as Oil Stays Above $100](https://finance.yahoo.com/markets/article/10-year-treasury-hits-2007-high-as-oil-stays-above-100-alphacheck-140049622.html) ⭐️ 7.0/10

The 10-year U.S. Treasury yield rose to its highest level since 2007 while oil prices remained above $100 a barrel, according to a market roundup reported by Yahoo Finance. The item gives no specific yield level, price figure, or stated cause beyond those headline developments.

openbb · NVDA · Sep 15, 14:00

**「Background」** The 10-year Treasury yield last reached 5% in 2007; it climbed as high as 5.04% before easing to 5.01%.

**「Impact」** Because the 10-year Treasury yield serves as a benchmark for US mortgage and corporate borrowing, its rise to 5.04% points to higher loan costs for homebuyers and businesses, while oil above $100 adds to household and business energy costs.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/article/10-year-treasury-hits-2007-high-as-oil-stays-above-100-alphacheck-140049622.html">10-year Treasury hits 2007 high as oil stays above $100: AlphaCheck</a></li>
<li><a href="https://tradingeconomics.com/united-states/government-bond-yield">US 10 Year Treasury Note Yield - Quote - Chart - Historical Data - News</a></li>
<li><a href="https://finance.yahoo.com/markets/article/10-year-treasury-hits-2007-high-as-oil-stays-above-100-alphacheck-140049622.html">10 - year Treasury hits 2007 high as oil stays above $ 100 : AlphaCheck</a></li>
<li><a href="https://www.cnbc.com/2026/09/15/10-year-treasury-yield-rises-to-highest-since-2007.html">10 - year Treasury yield hits highest level since 2007</a></li>

</ul>
</details>

**Tags**: `#US Treasury yields`, `#oil prices`, `#bond market`, `#macroeconomy`, `#markets`

---

<a id="item-finance-news-13"></a>
### [Coca-Cola plans $10B US manufacturing spend by 2030](https://finance.yahoo.com/economy/articles/coca-cola-spend-10b-us-160200407.html) ⭐️ 7.0/10

Coca-Cola plans to spend $10 billion on U.S. manufacturing by 2030, according to a report. The report did not specify how the money would be allocated across plants, suppliers, or years, and no baseline for comparison was provided.

openbb · PG · Sep 15, 16:02

**「Background」** Much of Coca-Cola&\#x27;s U.S. manufacturing and distribution is handled by independent bottling partners, so the bulk of the $10 billion represents those partners&\#x27; local investments rather than the company&\#x27;s own capital spending, according to its CFO.

**「Who is affected」** The commitment is system-wide, covering Coca-Cola and its bottlers rather than the parent company alone, so the spending runs through the U.S. bottling network that a company-commissioned study said contributed $85 billion to U.S. GDP and supported nearly 1 million jobs in 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://fortune.com/2026/09/15/coca-cola-invest-10-billion-us-growth-through-2030-cfo/">Coca-Cola to invest $10 billion in U.S. growth through 2030, says CFO | Fortune</a></li>
<li><a href="https://www.fooddive.com/news/coca-cola-us-manufacturing-10-billion-investment/830468/">Coca-Cola to spend $10B on US manufacturing by 2030</a></li>
<li><a href="https://qz.com/coca-cola-10-billion-us-infrastructure-investment-2030-091526">Coca-Cola plans $10 billion in U.S. infrastructure investment ...</a></li>

</ul>
</details>

**Tags**: `#Coca-Cola`, `#US manufacturing`, `#corporate investment`, `#capex`

---

<a id="item-finance-news-14"></a>
### [Fed&\#x27;s preferred inflation gauge shows fastest price rise in three years](https://news.google.com/rss/articles/CBMiigFBVV95cUxNODJpSG0zUXZ3T3JiemstZEM0ek55U3NHQVh2YlVSdG1WZnBwdEFMQUhmemQ5NnlmVk0teWFqV2lsRXJ2XzB0ZjJ5YW91ejZWUjRzZ2RkdzdCekdGNjAya2VIRnVPbmdSODE4WlEyR1BVY3hBeXhyTDV4NmZBVE9ybkpkbERKTnh2cFE?oc=5) ⭐️ 7.0/10

CBS News reports that the Federal Reserve&\#x27;s preferred inflation gauge showed prices rising at the fastest pace in three years, indicating persistent inflationary pressure. The report does not provide the specific figures or period in the excerpt.

google\_news · CBS News · Jun 25, 07:00

**「Background」** The Personal Consumption Expenditures index is the Federal Reserve’s preferred inflation measure, and the Fed aims for 2% annual inflation over the longer run. It rose at a 4.1% annual rate in May 2026, the fastest pace in three years, CBS News reported.

**「Impact」** The report is likely to keep the Fed holding interest rates steady with an eye toward hiking if inflation doesn&\#x27;t dissipate, meaning households and businesses may continue to face elevated borrowing costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/pce-report-report-may-2026-federal-reserve-inflation/">The Fed&#x27;s preferred inflation gauge shows prices rising at ...</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/article/pce-report-feds-preferred-inflation-measure-hits-3-year-high-keeping-talk-of-possible-rate-hike-in-play-124158491.html?fr=sycsrp_catchall">PCE report: Fed&#x27;s preferred inflation measure hits 3-year ...</a></li>
<li><a href="https://www.federalreserve.gov/economy-at-a-glance-inflation-pce.htm">The Fed - Inflation (PCE) - Federal Reserve Board</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/article/pce-report-feds-preferred-inflation-measure-hits-3-year-high-keeping-talk-of-possible-rate-hike-in-play-124158491.html">PCE report: Fed&#x27;s preferred inflation measure hits 3-year high, keeping talk of possible rate hike in play</a></li>

</ul>
</details>

**Tags**: `#inflation`, `#Federal Reserve`, `#PCE`, `#economic data`, `#monetary policy`

---