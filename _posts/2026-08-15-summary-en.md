---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 235 items, 27 important content pieces were selected

---

**Technology News**
1. [GLM-5.3: Frontier coding with emergent cyber capabilities](#item-tech-news-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B: local reasoning model draws praise and practical caveats](#item-tech-news-2) ⭐️ 8.0/10
3. [Doom&\#x27;s renderer compiled into a 21B-parameter transformer without training](#item-tech-news-3) ⭐️ 8.0/10
4. [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](#item-tech-news-4) ⭐️ 8.0/10
5. [PostgreSQL patches high-severity to\_char flaw allowing code execution](#item-tech-news-5) ⭐️ 8.0/10
6. [Why Opus 5 Feels Worse: Agent-First AI Communication](#item-tech-news-6) ⭐️ 7.0/10
7. [Google touts homomorphic encryption for private AI, but costs loom](#item-tech-news-7) ⭐️ 7.0/10
8. [Firefox becomes last major browser supporting uBlock Origin](#item-tech-news-8) ⭐️ 7.0/10
9. [Don&\#x27;t Classify. Hallucinate\! LLM Tagging with Embeddings](#item-tech-news-9) ⭐️ 7.0/10
10. [Open-source oncothresh evaluates oncology AI at clinical decision thresholds](#item-tech-news-10) ⭐️ 7.0/10
11. [torch-preflight: A Static Linter for PyTorch Training Bugs and VRAM Estimates](#item-tech-news-11) ⭐️ 7.0/10
12. [AI Robotic Labs Aim to Replace Animal Testing With 3M Human Tissue Tests a Year](#item-tech-news-12) ⭐️ 7.0/10
13. [Judge Orders Google to Remove Third-Party App Store Installation Friction](#item-tech-news-13) ⭐️ 7.0/10
14. [Apple Trains China-Specific AI Model with Alibaba Support](#item-tech-news-14) ⭐️ 7.0/10

**Financial News**
1. [Hormuz Attacks Lift Brent Toward $100 a Barrel](#item-finance-news-1) ⭐️ 9.0/10
2. [Federal Reserve Holds Interest Rates Steady in 9-3 Vote](#item-finance-news-2) ⭐️ 9.0/10
3. [Fed holds interest rates steady but signals possible future hike](#item-finance-news-3) ⭐️ 9.0/10
4. [Fed Holds Rates Steady, Signals Possible Future Hikes](#item-finance-news-4) ⭐️ 9.0/10
5. [Berkshire makes Alphabet a top-three holding, raises Delta and homebuilder bets](#item-finance-news-5) ⭐️ 8.0/10
6. [Goldman Sachs capitalizes on AI infrastructure funding deals](#item-finance-news-6) ⭐️ 8.0/10
7. [Premarket movers: Reddit, Applied Materials, Workday](#item-finance-news-7) ⭐️ 8.0/10
8. [Kazakhstan Accuses Kashagan Oil Consortium of $10.7 Billion Corruption](#item-finance-news-8) ⭐️ 8.0/10
9. [Iran’s Economy Buckles Under War, Sanctions, and Naval Blockade](#item-finance-news-9) ⭐️ 8.0/10
10. [Asian Refiners Buy U.S. Crude as Hormuz Disruption Limits Supply](#item-finance-news-10) ⭐️ 8.0/10
11. [Fed holds interest rates steady; Warsh holds news conference](#item-finance-news-11) ⭐️ 8.0/10
12. [Fed Holds Rates Steady After July Meeting](#item-finance-news-12) ⭐️ 8.0/10
13. [Apple Proposes Up to 15% Commission on Off-App Store Purchases](#item-finance-news-13) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GLM-5.3: Frontier coding with emergent cyber capabilities](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai announced GLM-5.3, a frontier coding model described as having emergent cyber capabilities including autonomous security research and vulnerability disclosure at scale. Early user reports describe it executing red-team security research through a Claude Code harness, including 0-day vulnerabilities in WordPress plugins, remote code execution, and adapting a 6.8 Linux kernel exploit, while playing defense against another GLM agent. The model is also reported to be scanning open-source and popular software at scale, with a CVE disclosure portal \(cvd.z.ai\) showing many under-embargo vulnerabilities rated critical or high. Commenters compared it favorably but slightly behind Mythos 5 and said it still feels close to GLM 5.2 with post-training improvements, with weights reportedly expected two weeks from release.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**「Background」** GLM-5.3 is the latest model in Z.ai&\#x27;s GLM series, a family of large language models positioned for Agentic Engineering. Released on August 14, 2026, GLM-5.3 keeps the same base model as GLM-5.2 and derives all improvements from post-training, achieving a 50% gain on Z.ai Code Bench and open-source state-of-the-art results on benchmarks such as Terminal-Bench 3.0 and Agents&\#x27; Last Exam \(CLI\). Its cyber capabilities, including autonomous security research, vulnerability discovery, and exploit adaptation, are described as emergent from this post-training process, and Z.ai has set up a coordinated vulnerability disclosure program at cvd.z.ai.

**「Impact」** For open-source maintainers and security teams, GLM-5.3&\#x27;s automated vulnerability discovery at scale could translate into a significant influx of newly disclosed high/critical CVEs across popular software, making urgent patching more likely; the full scope remains uncertain while embargoes are active.

**「Community Discussion」** Commenters report strong hands-on results, including seamless red-team scenarios and exploit adaptation, but also note the model is &quot;still shy of Sol and Fable&quot; and question the economics of running it locally versus OpenAI. One user praised Z.ai&\#x27;s writing as researcher-like rather than marketing hype.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber ...</a></li>

</ul>
</details>

**Tags**: `#GLM`, `#large language models`, `#cybersecurity`, `#AI coding`, `#vulnerability discovery`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B: local reasoning model draws praise and practical caveats](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B is a new open-weight FP8 local language model hosted on Hugging Face that has attracted attention for explicit, chain-of-thought style reasoning. Community reports say it is only the second local model, after Gemma 4, to correctly solve one private benchmark, although it needed about five times as many tokens and took 12m30s with multi-token prediction \(MTP\) enabled. Another user found it produced a surprisingly accurate pelican-on-bicycle image when running on an M5 Max laptop. Commenters also note real differences from Qwen 3.6: less efficient VRAM usage at 32K context and a note-style “caveman” thinking trace that may interfere with MTP prediction, plus unresolved no-thinking support in Ollama.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**「Background」** Qwen 3.8-27B is an open-weights model released by Alibaba&\#x27;s Qwen team under the Apache-2.0 license on August 14, 2026. It is a 27-billion-parameter native vision-language model with a native context length of 262,144 tokens, thinking enabled by default, and a configurable \`reasoning\_effort\` dial. It continues the Qwen series of accessible local models, offering dense reasoning performance for deployment on consumer-grade hardware.

**「Impact」** Developers running local models may now consider Qwen 3.8 27B a serious reasoning alternative to Gemma 4, but the higher VRAM footprint and lack of a straightforward way to disable thinking in Ollama could keep some users on Qwen 3.6 or force template workarounds.

**「Community Discussion」** Commenters agree that Qwen 3.8 27B reasons more explicitly and impressively than many local models, with one private-benchmark success and one strong pelican rendering, but they are divided on practicalities: the unusual thinking style may be hobbling MTP predictions, Ollama’s API lacks a simple no-think toggle, and broken Jinja templates need a community fix.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=Fvg8659WQDg">Qwen - 3 . 8 - 27 B Released : Everything you need to Know... - YouTube</a></li>

</ul>
</details>

**Tags**: `#llm`, `#open-source`, `#local-models`, `#reasoning`, `#qwen`

---

<a id="item-tech-news-3"></a>
### [Doom&\#x27;s renderer compiled into a 21B-parameter transformer without training](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

A developer known as /u/notforrob ported Doom&\#x27;s rendering algorithm into a 21B-parameter transformer using a custom compiler that converts computation graphs into transformer weights, with no training involved. The resulting checkpoint is a standard Hugging Face transformers model loadable without special code. To render a frame, the model receives a 3,614-token scene prompt and generates 53,747 tokens containing pixel-drawing commands; applying these commands reconstructs the iconic E1M1 frame. This process takes just over 40 minutes on an Nvidia B200, achieving roughly 35 frames per day compared to the original Doom&\#x27;s 35 frames per second on a 486. The project demonstrates a compiler-based approach to programming transformers, with potential implications for mechanistic interpretability and weight engineering, though it remains a proof-of-concept rather than a practical alternative to training.

reddit · r/MachineLearning · /u/notforrob · Aug 14, 15:50

**「Background」** Transformers are typically trained on data to learn tasks, but this project instead uses a custom compiler to directly set the weights of a standard transformer architecture \(similar to Phi-3\) so that autoregressive generation executes a specific algorithm: Doom&\#x27;s classic software renderer. This builds on earlier work by the same author that compiled calculators into transformer weights without training, demonstrating that transformer weights can be hand-crafted rather than learned.

**「Impact」** Researchers and developers interested in transformer interpretability and weight engineering gain a concrete example of embedding a real-world algorithm entirely within transformer weights without training, alongside an open-source compiler, host code, and checkpoint for experimentation.

<details><summary>References</summary>
<ul>
<li><a href="https://ood.dev/posts/doom/">Doom, compiled into a transformer — Out of Distribution</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#mechanistic interpretability`, `#compiler`, `#program synthesis`, `#neural rendering`

---

<a id="item-tech-news-4"></a>
### [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu&\#x27;s dots lab open-sourced dots3-note preview, the first open-weights model in the dots3 series. It is a 280B-parameter Mixture-of-Experts model with only 16B active parameters per inference, supports a 512K context window, and processes text, image, video, and audio inputs. The model introduces a new reinforcement learning method called TEMPO, which trains long-horizon agents through self-critique and test-time value estimation. Weights are available on Hugging Face, alongside two new agent benchmarks, VibeSearchBench and VibeLifeBench, for real-world evaluation.

telegram · zaihuapd · Aug 14, 08:27

**「Background」** Mixture-of-Experts \(MoE\) models activate only a subset of their total parameters per token, which is why a 280B-parameter model can have 16B active parameters and still offer a 512K-token context window for long and multimodal inputs. The dots3-note preview is the first open-weight model from Xiaohongshu&\#x27;s dots laboratory, and TEMPO is the new reinforcement-learning method it introduces for training long-horizon agents using self-critique and test-time value estimation, as confirmed by the Hugging Face repository and community posts.

**「Impact」** Developers and researchers can now deploy a 280B-class MoE model with relatively low inference cost due to its 16B active parameters, while also using the newly released VibeSearchBench and VibeLifeBench to evaluate long-horizon agent capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260814/2348931.html">小红书开源 dots3-note，280B MoE 仅 16B 激活参数 - 禁闻网</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>
<li><a href="https://x.com/BanghuaZ/status/2088088521882140734">Banghua Zhu on X: &quot;The first language model from Rednote dots studio lab! (Yes, rednote from China is also starting to release open model lol.)&quot; / X</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#Mixture-of-Experts`, `#multimodal`, `#reinforcement-learning`, `#agents`

---

<a id="item-tech-news-5"></a>
### [PostgreSQL patches high-severity to\_char flaw allowing code execution](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL disclosed and patched CVE-2026-14669, a high-severity heap buffer overflow in to\_char\(timestamptz\) when handling overly long POSIX timezone abbreviations. The flaw can let a database user with timezone-setting privileges execute arbitrary code with the OS privileges of the PostgreSQL server process. The vulnerability has a CVSS score of 8.8 and requires a low-privileged database account rather than unauthenticated access. Affected versions include releases before PostgreSQL 18.5, 17.11, 16.15, 15.19, and 14.24; since 18.5 was not officially released due to a regression, 18-series users should upgrade directly to 18.6. The minor update does not require dumping the database or running pg\_upgrade; admins can replace program files and restart the service.

telegram · zaihuapd · Aug 14, 14:35

**「Background」** PostgreSQL&\#x27;s to\_char function converts timestamp values into formatted strings, and timestamptz is the timezone-aware timestamp type. POSIX timezone abbreviations can be configured as long strings, and the bug manifests when to\_char processes an excessively long abbreviation, causing the heap overflow.

**「Impact」** Database administrators should upgrade affected PostgreSQL instances to 18.6, 17.11, 16.15, 15.19, or 14.24 to close the code-execution path. Because exploitation requires timezone-setting privileges, databases where only trusted users hold such privileges are at lower risk.

**Tags**: `#PostgreSQL`, `#CVE`, `#security`, `#database`, `#vulnerability`

---

<a id="item-tech-news-6"></a>
### [Why Opus 5 Feels Worse: Agent-First AI Communication](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

A Hacker News discussion examines why Anthropic&\#x27;s Opus 5 feels worse to work with despite being more capable, attributing it to an increasingly elliptical, agent-oriented communication style. Commenters describe the model writing abstract sentences that orbit a point, using inanimate nouns as subjects for stylistic variety, and treating humans as no longer the primary target audience of post-training. Some users report switching back to Claude 4.8 or to OpenAI&\#x27;s Sol because Opus 5 exhausts them and veers off-topic without strict, narrow instructions. The discussion frames this as a broader shift toward agent-to-agent communication at the expense of human readability, even as the model demonstrates greater raw capability.

hackernews · numeri · Aug 14, 10:12 · [Discussion](https://news.ycombinator.com/item?id=49296740)

**「Background」** Anthropic introduced Claude Opus 5 on July 24, 2026, as a powerful agentic coding model focused on long-running, multi-step work, with the largest gains over Claude Opus 4.8 in deep reasoning, agentic and long-horizon tasks, and test-time compute scaling. The community discussion centers on how this new model communicates, with users describing its style as elliptical, abstract, and seemingly optimized for other AI agents rather than for human readability. This context helps explain the criticism that Opus 5 feels worse to work with even though it is technically more capable.

**「Impact」** Heavy Claude users may need to adopt unusually strict and narrow prompts to keep Opus 5 on task, and some are already migrating to older models or competing offerings such as OpenAI&\#x27;s Sol, based on anecdotal reports rather than benchmark evidence.

**「Community Discussion」** Commenters largely agree that Opus 5&\#x27;s communication is exhausting and feels optimized for other agents, citing specific examples like verbose &\#x27;honesty&\#x27; confessions and obscure aphorisms. Disagreement remains over whether the capability gains justify the style, with some users finding alternatives like Sol or Claude 4.8 more pleasant for daily work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/whats-new-opus-5">What&#x27;s new in Claude Opus 5 - Claude Platform Docs</a></li>

</ul>
</details>

**Tags**: `#AI`, `#machine learning`, `#human-computer interaction`, `#LLM`, `#software engineering`

---

<a id="item-tech-news-7"></a>
### [Google touts homomorphic encryption for private AI, but costs loom](https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/) ⭐️ 7.0/10

Google announced progress toward making private AI practical using homomorphic encryption, a technique that permits computations on encrypted data without revealing the underlying inputs. The company frames this as a step toward privacy-preserving machine learning, though the announcement does not provide full technical details or performance benchmarks. The significance lies in the potential to protect user data during AI inference while keeping models functional in data centers. However, community experts note that homomorphic encryption still imposes very high overhead, often around 1000x on inference tasks, so commercial viability remains uncertain.

hackernews · u1hcw9nx · Aug 14, 15:43 · [Discussion](https://news.ycombinator.com/item?id=49300314)

**「Background」** Homomorphic encryption \(HE\) is a cryptographic technique that allows computations to be performed directly on encrypted data, so a cloud service can process sensitive inputs without ever seeing them in the clear. Google&\#x27;s announced work centers on HEIR, an open-source compiler toolchain that can convert pre-trained AI models operating on unencrypted data into versions that operate on encrypted inputs, aiming to make cryptographically secure private AI inference practical. However, HE and related privacy-preserving machine learning techniques traditionally incur high computational overhead, and the approach is intended to remove the need to trust the service provider, not to address broader privacy concerns about data collection.

**「Impact」** For AI and security practitioners, the development signals continued investment in homomorphic encryption, but the cited ~1000x overhead means private inference is unlikely to be commercially practical in the near term.

**「Community Discussion」** Comments are skeptical: some argue Google&\#x27;s privacy posture is hypocritical given its broader data practices, and others note that running models on local hardware already provides strong privacy without the energy cost of homomorphic encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/">How Google is Making Private AI Practical with Homomorphic ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49300314">Google Is Making Private AI Practical with Homomorphic Encryption</a></li>
<li><a href="https://www.linkedin.com/pulse/homomorphic-encryption-secure-computation-unlocking-agjzf">Homomorphic Encryption for Secure Computation: Unlocking the...</a></li>

</ul>
</details>

**Tags**: `#homomorphic encryption`, `#privacy-preserving ML`, `#AI`, `#Google`, `#security`

---

<a id="item-tech-news-8"></a>
### [Firefox becomes last major browser supporting uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 7.0/10

Firefox is now the only major browser that still fully supports uBlock Origin, after Google Chrome&\#x27;s switch to Manifest V3 restricted the extension APIs that made the ad blocker work. This change has practical consequences for anyone relying on uBlock Origin: Chrome can no longer offer the same blocking capabilities, while Firefox continues to support the extension and even vets it for malware on each update. The shift underscores a broader conflict between browser vendors&\#x27; control over extension systems and users&\#x27; desire for effective ad blocking and privacy tools. As a result, Firefox has become the default choice for users who want unrestricted, powerful ad blocking.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**「Background」** Google&\#x27;s Manifest V3 extension framework, which began rolling out in Chrome, places new restrictions on extension capabilities, particularly the webRequest API that ad blockers like uBlock Origin rely on for advanced filtering. As a result, the full version of uBlock Origin is no longer fully supported in Chrome, with Google&\#x27;s changes coming into force by June 2025, and Chrome users are now directed to uBlock Origin Lite instead. Firefox continues to support the older Manifest V2 extension model, which is why it remains the last major browser where the full uBlock Origin extension still works.

**「Impact」** Users who depend on uBlock Origin&\#x27;s full ad-blocking capability in Chrome will either need to migrate to Firefox or accept weaker protection under Manifest V3, which removes the blocking webRequest API that enabled the extension&\#x27;s filtering engine.

**「Community discussion」** Commenters praised Firefox for reviewing popular extensions like uBlock Origin on every update, while others criticized Google for building a gated extension store and destroying APIs that made ad blockers effective. Some noted workarounds such as side-loading an unpacked extension in Chrome, but acknowledged the difficulty, and at least one developer reported shutting down a Chrome search ad-blocking extension because of Manifest V3.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/zhangwei42/ublock-origin-in-chrome-navigating-the-new-manifest-v3-landscape-3ca3">uBlock Origin in Chrome: Navigating the New Manifest V3 ...</a></li>
<li><a href="https://ublockorigin.com/">uBlock Origin - Free, open-source ad blocker extension</a></li>

</ul>
</details>

**Tags**: `#Firefox`, `#uBlock Origin`, `#Manifest V3`, `#ad blocking`, `#browser extensions`

---

<a id="item-tech-news-9"></a>
### [Don&\#x27;t Classify. Hallucinate\! LLM Tagging with Embeddings](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Simon Willison highlights Doug Turnbull&\#x27;s &\#x27;Don&\#x27;t classify. Hallucinate\!&\#x27; technique for tagging his blog&\#x27;s older untagged posts, where the site has 1,856 tags too many to feed an LLM at once. Instead of asking the model to select from the existing vocabulary, the method asks it to generate novel, hypothetical tags, then uses vector embeddings to find the concrete existing tags closest to those imagined ones. Turnbull&\#x27;s example prompt includes several sample tag hierarchies so the model knows the shape of valid classifications, such as &\#x27;Furniture / Living Room Furniture / Coffee Tables &amp; End Tables / Coffee Tables.&\#x27; This approach is relevant to AI workflows because it sidesteps the context-window limit for large label sets while still mapping results to canonical tags.

rss · Simon Willison · Aug 14, 21:54

**「Context」** Traditional LLM classification into a large, fixed vocabulary is token-hungry and often inaccurate when there are thousands of possible tags, as with Simon Willison&\#x27;s 1,856 blog tags. The technique described by Doug Turnbull and highlighted by Willison draws on hypothetical document embeddings: instead of forcing the model to pick from the entire vocabulary, ask it to hallucinate plausible novel labels, then use vector embeddings to match those labels to the closest real tags in the existing taxonomy. This approach reduces token usage and accommodates very large tag sets without requiring the entire vocabulary to be included in the prompt.

**「Impact」** Developers and maintainers of large tag sets or taxonomies can use this technique to classify content without fitting every possible label into the prompt, relying on embeddings to connect hallucinated categories to existing vocabulary.

<details><summary>References</summary>
<ul>
<li><a href="https://softwaredoug.com/blog/2026/08/10/hypothetical-classifications">Don&#x27;t classify. Hallucinate!</a></li>
<li><a href="https://www.linkedin.com/posts/softwaredoug_dont-classify-hallucinate-activity-7492683478216560640-0xCh">Don’t classify. Hallucinate! | Doug Turnbull - LinkedIn</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#embeddings`, `#content tagging`, `#vector search`, `#AI`

---

<a id="item-tech-news-10"></a>
### [Open-source oncothresh evaluates oncology AI at clinical decision thresholds](https://www.reddit.com/r/MachineLearning/comments/1vod2c8/opensource_python_library_nocode_web_dashboard/) ⭐️ 7.0/10

The author released oncothresh, a dependency-light open-source Python library \(numpy/scipy/scikit-learn/pydantic\) for evaluating oncology AI models at a specific clinical cutoff rather than through global metrics like AUC, ICC, or MAE. It computes sensitivity, specificity, PPV, and NPV at the threshold, bootstrap confidence intervals, threshold-sensitivity curves, boundary-weighted calibration, decision-curve net benefit, and number-needed-to-test. The companion no-code dashboard oncothresh-web lets users upload a CSV of predictions and labels, choose a threshold, and receive charts plus a downloadable PDF report, running locally via docker compose up. Both projects, at v0.1 on GitHub, target pathologys tasks such as tumor cellularity, Ki-67, TMB, and PD-L1 scoring, and address a gap left by global benchmark suites like PathBench and PathBench-MIL.

reddit · r/MachineLearning · /u/adom2989 · Aug 14, 17:06

**「Background」** Oncology AI models often output continuous scores that are turned into clinical decisions at fixed cutoffs—for example, whether a tumor sample is flagged, biopsied, or treated. Traditional evaluation metrics summarize agreement over the full score range, so they do not directly quantify reliability at the threshold that matters in practice. oncothresh applies threshold-specific statistics and uncertainty quantification to fill that evaluation gap; existing pathology benchmarks such as PathBench and PathBench-MIL predominantly assess foundation models globally.

**Tags**: `#oncology AI`, `#model evaluation`, `#clinical decision thresholds`, `#open-source`, `#Python`

---

<a id="item-tech-news-11"></a>
### [torch-preflight: A Static Linter for PyTorch Training Bugs and VRAM Estimates](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 7.0/10

torch-preflight is a static linter for PyTorch that catches common training-loop bugs and estimates GPU memory usage before code is run. It currently implements 13 rules that detect issues such as appending losses to a list while retaining the autograd graph, missing zero\_grad\(\) calls, gradient accumulation without dividing the loss, and using DDP without a DistributedSampler so every rank trains on the same batches. The tool never imports or executes user code, so it requires no GPU and no torch installation. It also provides a VRAM estimation mode that reports whether a training script will fit on a specified GPU and lists code changes with the GiB each change saves; the author reports estimates landed within 4% of measured peaks, but only from four models on one T4. The project is still a work in progress, is published on PyPI as torch-preflight, and is available on GitHub at highwaterlabs/torch-preflight, with maintainers open to contributions and bug reports.

reddit · r/MachineLearning · /u/LeJanbandhu · Aug 14, 14:30

**「Background」** PyTorch training scripts often contain subtle bugs that only waste resources after long runs, such as holding the autograd graph from every step, forgetting to zero gradients, or misusing distributed data loading. A linter performs static analysis of source code without executing it, which lets developers identify these issues before paying for GPU instances or waiting through failed training runs.

**「Impact」** PyTorch developers can use torch-preflight to catch common training-loop bugs before launching expensive GPU jobs and to check whether a training script will fit into a target GPU&\#x27;s memory, with concrete GiB savings estimates for each suggested change.

**Tags**: `#PyTorch`, `#linter`, `#ML tooling`, `#debugging`, `#GPU memory`

---

<a id="item-tech-news-12"></a>
### [AI Robotic Labs Aim to Replace Animal Testing With 3M Human Tissue Tests a Year](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

Vivodyne, a biotech company south of San Francisco, is using closet-sized robotic laboratories to grow and test human tissue at unprecedented scale, with AI designing experiments to better predict drug efficacy and safety. The system currently comprises 12 hive-like robot labs capable of running controlled tests on more than 3 million human tissue samples per year, a capacity the company says is double the total capacity of all U.S. clinical trials combined. Roughly 90% of clinical trials still fail after passing animal testing, and Vivodyne&\#x27;s approach aims to make animal testing obsolete by providing more human-relevant data before trials begin. The platform represents a significant application of AI and robotics to drug discovery, though it has not yet been broadly validated as a replacement for established regulatory testing pathways.

telegram · zaihuapd · Aug 14, 01:48

**「Background」** Most drugs that pass animal tests still fail in human clinical trials—roughly 90% of candidates do not reach approval, often because animal models do not accurately predict human responses. Vivodyne is part of a broader organ-on-a-chip and human-tissue-modeling field that aims to replace or reduce animal testing using lab-grown tissues that mimic human biology. The company claims to have built autonomous robotic labs and AI-driven experimental design to test thousands of functional human tissues at scale, backed by $40 million in funding to address the high clinical trial failure rate.

**「Impact」** For drug developers and biotech researchers, this scale could allow many more candidate drugs to be screened on human tissue before costly clinical trials, potentially reducing late-stage failures and the reliance on animal testing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://www.vivodyne.com/human-tissues">Human Tissues - vivodyne.com</a></li>
<li><a href="https://www.businesswire.com/news/home/20250528498236/en/Vivodyne-to-Replace-Animal-Testing-With-$40-Million-Funding-to-Reverse-95-Clinical-Trial-Failure-Rate">Vivodyne to Replace Animal Testing With $40 Million Funding ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#biotech`, `#robotics`, `#drug discovery`, `#animal testing`

---

<a id="item-tech-news-13"></a>
### [Judge Orders Google to Remove Third-Party App Store Installation Friction](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

A U.S. district judge ordered Google to remove extra installation steps and warning popups for rival Android app stores in the Play Store within one week. Judge James Donato ruled the multi-step flow, requiring users to tap &quot;View&quot; before &quot;Install,&quot; was deliberate anticompetitive friction meant to deter ordinary users. The order follows the Epic v. Google antitrust case, in which a jury found Google illegally monopolized Android app distribution. Google must make installing third-party stores as straightforward as installing a normal Android app.

telegram · zaihuapd · Aug 14, 09:55

**「Background」** Epic v. Google is an antitrust case in which Epic Games challenged Google&\#x27;s Play Store dominance, and a jury ruled Google illegally monopolized Android app distribution. As a remedy, Judge James Donato has now ordered Google to strip away the extra confirmation steps and warnings that made installing rival app stores more intimidating.

**「Impact」** Android users and third-party app store operators will soon face fewer warnings and steps when installing stores, lowering the barrier to alternative app distribution on Android.

**Tags**: `#Android`, `#antitrust`, `#Google`, `#app stores`, `#regulation`

---

<a id="item-tech-news-14"></a>
### [Apple Trains China-Specific AI Model with Alibaba Support](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

Apple has reportedly trained a large language model tailored to the Chinese market with support from Alibaba, marking a shift from its previous reliance on third-party models. The move is aimed at giving Apple greater control over its AI experience in China, with Apple Intelligence expected to launch there in the coming months via an iOS update. China&\#x27;s Cyberspace Administration of China \(CAC\) filed Apple&\#x27;s generative AI service for registration last month, according to Reuters sources. If approval proceeds, Apple could become the first foreign company licensed to offer its own AI model in China.

telegram · zaihuapd · Aug 14, 14:47

**「Background」** Apple Intelligence is Apple&\#x27;s suite of AI features, and in China it previously planned to rely on Alibaba&\#x27;s Qwen model to power those features on compatible iPhone, iPad, Mac, and Vision Pro models. China&\#x27;s cyberspace regulator requires generative AI services to be registered or approved before they can be offered to the public. According to Reuters, Apple has now trained its own large language model specifically for the Chinese market with Alibaba&\#x27;s support, a departure from its earlier strategy of depending on third-party models.

**「Impact」** China&\#x27;s Cyberspace Administration registered Apple Intelligence on July 15, 2026, clearing the main regulatory hurdle for deployment, so mainland iPhone users are set to get Apple&\#x27;s AI features in upcoming iOS updates, and Apple&\#x27;s entry—with Alibaba and Baidu as partners—intensifies competition in China&\#x27;s on-device AI market.

<details><summary>References</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-14/exclusive-apple-trains-its-own-ai-model-for-china-market-with-alibabas-support-sources-say">Exclusive-Apple Trains Its Own AI Model for China Market With ...</a></li>
<li><a href="https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/">EXCLUSIVE: Apple trains its own AI model for China market ...</a></li>
<li><a href="https://www.digitaltrends.com/phones/china-approves-apple-intelligence-for-iphones-with-alibaba-baidu-emerging-as-partners/">China approves Apple Intelligence for iPhones, with Alibaba ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Large Language Models`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Hormuz Attacks Lift Brent Toward $100 a Barrel](https://oilprice.com/Energy/Crude-Oil/Hormuz-Attacks-Push-Oil-Toward-100-Despite-US-Crude-Build.html) ⭐️ 9.0/10

Renewed attacks on ships in the Strait of Hormuz pushed oil prices higher, putting Brent crude near $88 a barrel and on track for a 5% weekly gain, though a larger-than-expected 17 million barrel build in US crude inventories limited the move.

rss · OilPrice.com · Aug 14, 16:21

**「Background」** The Strait of Hormuz is a key route for global oil shipments; stalled talks between the US and Iran and Tehran’s increased strikes on tankers have raised supply fears, while Washington maintains a naval blockade of Iranian crude.

**「Impact」** The IEA forecasts that record fuel prices will destroy 1.6 million b/d of global oil demand in 2026, as households and businesses adjust to higher costs.

**Tags**: `#oil prices`, `#geopolitics`, `#Hormuz`, `#energy supply`, `#OPEC`

---

<a id="item-finance-news-2"></a>
### [Federal Reserve Holds Interest Rates Steady in 9-3 Vote](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

The Federal Reserve voted 9-3 to leave interest rates unchanged at its latest policy meeting, pausing further rate moves for now.

google\_news · ABC7 Los Angeles · Jul 29, 07:00

**「Background」** The Federal Reserve&\#x27;s policy committee voted 9-3 to keep its benchmark rate at 3.5%-3.75%, a range in place since January. The three dissenting votes favored a rate increase, and the decision comes amid inflation that has remained above the central bank&\#x27;s 2 percent target.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members voted to hike</a></li>
<li><a href="https://www.schwab.com/learn/story/fomc-meeting">Divided Fed Leaves Interest Rates Unchanged | Charles Schwab</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#FOMC`, `#central bank`

---

<a id="item-finance-news-3"></a>
### [Fed holds interest rates steady but signals possible future hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

The Federal Reserve kept interest rates unchanged but left the door open for a future increase, according to CBS News.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The Federal Reserve left its benchmark interest rate unchanged on Wednesday, but nearly half of its policymakers said they would support a rate hike later this year as inflation remains elevated.

**「Impact」** Borrowing costs for households and businesses are unchanged for now, but if inflation keeps accelerating, a future rate hike could make credit cards, mortgages, and other loans more expensive.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door open to hike - CBS News</a></li>
<li><a href="https://www.npr.org/2026/07/29/nx-s1-5910558/federal-reserve-interest-rates-inflation">A divided Federal Reserve holds interest rates steady despite high inflation</a></li>
<li><a href="https://www.detroitnews.com/story/business/2026/04/27/fed-likely-to-hold-rates-steady-as-powell-nears-possible-swan-song/89818844007/">Fed likely to hold rates steady as Powell nears possible swan song</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-4"></a>
### [Fed Holds Rates Steady, Signals Possible Future Hikes](https://news.google.com/rss/articles/CBMiiAFBVV95cUxOWlo2eWRfMHQzRGk2MTdTdkR4R3FLWHlxWjdRekZCOWRhWk42ajJxamdDcmZlbER4TzVxZlFMa0F5d0wycHVMejh1Qk1vTGtWQW1qV05HdXp6ZFFOd3FEOXdaRmw5ZC1HdDd6WGl1Q3NnOS0xc3Y0YUdyQ3htLUlzTVJqRG9oalZM?oc=5) ⭐️ 9.0/10

The Federal Reserve kept its benchmark interest rate unchanged and indicated it may raise rates in the future to continue fighting inflation.

google\_news · The New York Times · Jun 17, 07:00

**「Background」** In July 2026, the Federal Reserve held its benchmark interest rate at 3.50%–3.75% after keeping rates unchanged all year, with inflation still well above its 2% target and markets pricing in a high likelihood of a rate hike later in 2026.

**「Impact」** If the Fed follows through with future rate increases, borrowing costs for households and businesses would rise, adding pressure on affordability for mortgages, credit cards, and other loans.

<details><summary>References</summary>
<ul>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Federal Reserve Holds Rates at 3.50%-3.75% in July 2026 | U.S. Bank</a></li>
<li><a href="https://www.cnbc.com/2026/08/10/fed-rate-hike-prospects-higher-interest-rates.html">Fed rate hike prospects: What higher interest rates mean for your money</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`

---

<a id="item-finance-news-5"></a>
### [Berkshire makes Alphabet a top-three holding, raises Delta and homebuilder bets](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 8.0/10

Berkshire Hathaway’s second-quarter regulatory filing shows a shift from net selling to net buying: it made nearly $20 billion in net stock purchases, boosted Alphabet to its third-largest U.S.-listed holding with 106 million shares worth $37.9 billion at end-June, and increased stakes in Delta Air Lines and homebuilders.

rss · CNBC Finance · Aug 14, 21:06

**「Background」** The buying ended 14 straight quarters of net sales, and the Alphabet increase came mainly from a $10 billion private stock purchase in June to help fund Alphabet’s AI infrastructure. Berkshire had also returned to Delta after selling its airline holdings early in the pandemic.

**Tags**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#homebuilders`, `#equity investing`

---

<a id="item-finance-news-6"></a>
### [Goldman Sachs capitalizes on AI infrastructure funding deals](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 8.0/10

Goldman Sachs helped facilitate two major AI infrastructure financing deals this week: Nvidia&\#x27;s $500 billion funding initiative and Intel&\#x27;s upsized $20 billion common stock offering, earning fees as a joint book-running manager.

rss · CNBC Finance · Aug 14, 20:05

**「Background」** The Nvidia plan, supported by non-binding memorandums of understanding with Goldman and five other firms, treats data-center infrastructure as income-producing collateral similar to real estate or toll roads. Intel&\#x27;s offering is meant to fund expansion of its chip foundry, which manufactures chips for other companies.

**Tags**: `#Goldman Sachs`, `#AI infrastructure`, `#Nvidia`, `#Intel`, `#equity offering`

---

<a id="item-finance-news-7"></a>
### [Premarket movers: Reddit, Applied Materials, Workday](https://www.cnbc.com/2026/08/14/stocks-making-the-biggest-moves-premarket-rddt-amat-sndk-w.html) ⭐️ 8.0/10

Reddit shares rose about 12% in premarket trading after S&amp;P Dow Jones Indices said the company will join the S&amp;P 500 on Aug. 18, replacing AvalonBay Communities. Applied Materials fell more than 5% after reporting adjusted earnings of $3.50 per share on revenue of $9.12 billion, and Workday rose about 2% after Reuters reported Silver Lake was in talks to buy it.

rss · CNBC Finance · Aug 14, 10:46

**「Background」** Reuters reported Thursday that Silver Lake was in talks to buy Workday, which sent shares up nearly 18%. S&amp;P 500 index-tracking funds typically buy newly added stocks when a change takes effect.

**「Impact」** When the S&amp;P 500 change takes effect, index funds that track the benchmark will need to buy Reddit shares and sell AvalonBay Communities.

**Tags**: `#S&amp;P 500`, `#Earnings`, `#M&amp;A`, `#Stock Upgrades`, `#Premarket`

---

<a id="item-finance-news-8"></a>
### [Kazakhstan Accuses Kashagan Oil Consortium of $10.7 Billion Corruption](https://oilprice.com/Latest-Energy-News/World-News/Kazakhstan-Accuses-Big-Oil-of-107-Billion-Corruption-in-Kashagan-Oil-Project.html) ⭐️ 8.0/10

Kazakhstan has alleged in a confidential arbitration case that the international consortium behind the Kashagan oilfield awarded $10.7 billion in contracts through inflated costs or bribery, according to a report by the International Consortium of Investigative Journalists \(ICIJ\). The allegation is part of a larger $160 billion claim against the oil companies; no tribunal decision has been made.

rss · OilPrice.com · Aug 14, 14:30

**「Background」** Kashagan is operated by a consortium of international oil companies and Kazakhstan&\#x27;s state firm KazMunayGas, and the bribery allegations are part of a long-running arbitration dispute over cost overruns, delays, and environmental damage.

**「Impact」** Shell CEO Wael Sawan said the disputes have reduced its appetite to invest further in Kazakhstan, and the company is holding off on additional investment until it has better clarity on the outcome.

**Tags**: `#corruption`, `#oil industry`, `#Kazakhstan`, `#arbitration`, `#Big Oil`

---

<a id="item-finance-news-9"></a>
### [Iran’s Economy Buckles Under War, Sanctions, and Naval Blockade](https://oilprice.com/Geopolitics/Middle-East/Irans-Economy-Is-Buckling-Under-the-Weight-of-War.html) ⭐️ 8.0/10

Iran’s economy is buckling under the five-month-long war with the United States and Israel, compounded by sanctions and a US naval blockade; the IMF forecasts overall inflation will reach nearly 69% this year, the highest since the 1979 revolution, while basic food prices keep soaring.

rss · OilPrice.com · Aug 14, 14:00

**「Background」** Years of international sanctions and government mismanagement had already crippled Iran’s economy, and protests over inflation and living conditions broke out in late December before the war began; the bombing campaign and blockade have since intensified the crisis.

**「Impact」** Ordinary Iranians are bearing the brunt: an average family of four now spends about 70% of its income on basic food, and residents report running out of money before the end of the month.

**Tags**: `#Iran economy`, `#inflation`, `#sanctions`, `#war`, `#oil blockade`

---

<a id="item-finance-news-10"></a>
### [Asian Refiners Buy U.S. Crude as Hormuz Disruption Limits Supply](https://oilprice.com/Latest-Energy-News/World-News/Hormuz-Crisis-Pushes-Asian-Refiners-Toward-US-Oil.html) ⭐️ 8.0/10

Asian refiners have bought U.S. crude cargoes this week as an alternative to Middle Eastern oil constrained by the Strait of Hormuz disruption, with GS Caltex paying $13-14 over Dubai for Mars, Eneos paying over $10 over WTI for WTI, and CPC paying $8-9 over Dated Brent for WTI, according to Reuters trade sources.

rss · OilPrice.com · Aug 14, 12:30

**「Background」** The Strait of Hormuz, a narrow shipping lane between Iran and Oman, normally carries about 20% of the world&\#x27;s oil, but it has been effectively closed since the outbreak of the U.S.-Israel air war against Iran on Feb. 28, 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://research.cashugroup.com/research-reports/hormuz-chokepoint-oil-markets-crisis">Hormuz Chokepoint Crisis — Oil Supply Disruption Analysis ...</a></li>
<li><a href="https://www.dallasfed.org/research/economics/2026/0320">What the closure of the Strait of Hormuz means for the global ...</a></li>

</ul>
</details>

**Tags**: `#Oil markets`, `#Strait of Hormuz`, `#Asian refiners`, `#US crude`, `#Geopolitics`

---

<a id="item-finance-news-11"></a>
### [Fed holds interest rates steady; Warsh holds news conference](https://news.google.com/rss/articles/CBMivgFBVV95cUxNR1BZa2dPa1lOcjNBSmF2MHFHcTNBTV9mQzZOZ3BzR1ZrekhVWUhzLWszajBVWExhYWxJUWJDejh4SjBTdFdobFk1Y1NlMEpad0I4cUtrY0o1VzhMYmNOX2tuWjF3dXhGbkFVOWJncnZDdEt2dUEydkhhX2pwQXZlaF96QTZ3Z2l3OURfN2lLaVRRcEFLejhVTGZVSEl4XzJLWmE0RmxKRy16Mkh2ZGJvbm0wMUExTU83dHVJUlRn0gHDAUFVX3lxTE9kWHZBeUc3cjFTeGNrQk5QeGl2cHpycW5zR19kQl9vbEY3MzdUX0ZCa2pmV0RNT1VSUElKTEhhNmRmaVVnc1k5R0V2RkhTYkJROUZ3YXZmVjlPSWZ5MWVTWkxYS1B3ai1BZnRVeTE5bmR6Mm01eHlDYlpJblAta3hYSnN5Tnhzc19ZRjJwUWVTZzNRQXd0MUJGU29NRko2aVVuTTByMndYeWU3bTRXNWpEeFBlVDF5RTBUU1VaQUdlT1RlRQ?oc=5) ⭐️ 8.0/10

The Federal Reserve left interest rates unchanged, and Chair Kevin Warsh held a news conference after the decision, according to PBS.

google\_news · PBS · Jul 29, 07:00

**「Background」** This was the second rate-setting meeting under Fed Chair Kevin Warsh, who took over earlier in 2026; the committee voted 9-3 to hold the key rate, with three officials dissenting in favor of higher rates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-warsh-holds-news-conference-after-latest-interest-rate-decision">WATCH: Fed chair Warsh holds news conference after ... - PBS</a></li>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-new-fed-chair-kevin-warsh-holds-first-news-conference-after-interest-rate-decision">WATCH: New Fed chair Kevin Warsh holds first news conference ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/kevin-warsh-fed-treasury-yields-inflation-credibility-interest-rates.html">Fed&#x27;s Warsh&#x27;s credibility in question after rate decision ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#news conference`, `#economy`

---

<a id="item-finance-news-12"></a>
### [Fed Holds Rates Steady After July Meeting](https://news.google.com/rss/articles/CBMiiwFBVV95cUxNUVVUMW1Hb2g1N2cyQkJneFl4YXJ1aFVvOGQzX19Oc2IxZUFyVUcwOXI0VmlpaW04d0N0MWZxVFlhSkJLUTltY3VxOVVHVGFBZHc5eVRzUTRQN1FXSEQ1Qm16U1pJMC1rOHNSdFd6UTEyWTF4cUpjX3NJUGs1alI3VGtLSmdNZmpOdjM0?oc=5) ⭐️ 8.0/10

The Federal Reserve decided to leave interest rates unchanged after its July policy meeting, neither raising nor lowering its benchmark rate.

google\_news · Fortune · Jul 29, 07:00

**「Background」** The Federal Reserve&\#x27;s July meeting continued a pause on rate changes, leaving the federal funds rate at 3.5%–3.75% despite some predictions of a hike.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-meeting-today-live-updates.html">Fed meeting recap: July 2026</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady</a></li>
<li><a href="https://www.usatoday.com/story/money/economy/2026/07/29/fed-meeting-live-july-interest-rates--live/91061021007/">It wasn&#x27;t unanimous, but the Fed continued its pause on interest rates</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#economy`

---

<a id="item-finance-news-13"></a>
### [Apple Proposes Up to 15% Commission on Off-App Store Purchases](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

Apple has submitted to the court a proposal to charge commissions of up to 15% on purchases made outside the US App Store: 15% for standard apps, 10% for video/news partners and subscription renewals, and 5% for small business plan apps.

telegram · zaihuapd · Aug 14, 02:33

**「Background」** The filing comes in Apple’s ongoing antitrust litigation with Epic Games, after the US Supreme Court declined Apple’s request to pause lower-court proceedings over these fees; Epic will have a chance to respond, and Apple is expected to file written arguments by September 14.

**「Impact」** If approved, the proposal would affect US app developers who sell digital goods or subscriptions through external payment links, by requiring them to pay Apple commissions of 5–15% on those purchases.

**Tags**: `#Apple`, `#App Store`, `#commission fees`, `#regulation`, `#Epic Games`

---