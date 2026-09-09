---
layout: default
title: "Horizon Summary: 2026-09-09 (EN)"
date: 2026-09-09
lang: en
---

> From 237 items, 22 important content pieces were selected

---

**Technology News**
1. [OpenAI Claims Navier–Stokes Prize Result Amid Scooping Accusations](#item-tech-news-1) ⭐️ 9.0/10
2. [Google DeepMind launches AlphaGenome Atlas, a predictive map of every human DNA letter change](#item-tech-news-2) ⭐️ 8.0/10
3. [NeurIPS Desk-Rejects 178 Papers Using AI Detector That Flags Its Own Chairs](#item-tech-news-3) ⭐️ 8.0/10
4. [ASML and TSMC Plan High NA EUV Shift to 12-Inch Photomasks](#item-tech-news-4) ⭐️ 8.0/10
5. [Meta Announces Muse, a Personal AI Agent](#item-tech-news-5) ⭐️ 7.0/10
6. [Qwen3.8 27B Quantization Benchmark: 4-bit Safe, 1-bit Collapses](#item-tech-news-6) ⭐️ 7.0/10
7. [Malaysia Eyes Huawei Ascend Chips for $494M Sovereign AI Project](#item-tech-news-7) ⭐️ 7.0/10
8. [Zhang Yiming Oversees ByteDance Real-Time Spatial Video Model](#item-tech-news-8) ⭐️ 7.0/10
9. [China targets 9,800 EFLOPS intelligent computing by 2030](#item-tech-news-9) ⭐️ 7.0/10
10. [OpenAI Launches Faster ChatGPT Images 2.5](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Iran’s Oil Exports Plummet Under U.S. Strait of Hormuz Blockade](#item-finance-news-1) ⭐️ 9.0/10
2. [US Federal Reserve Holds Rates Steady Under New Chair Warsh](#item-finance-news-2) ⭐️ 9.0/10
3. [Copper Hits Record Above $14,500 as Expected U.S. Tariffs Squeeze Supply](#item-finance-news-3) ⭐️ 8.0/10
4. [U.S.-Saudi Nuclear Deal Clears IAEA Hurdle as Congress Review Continues](#item-finance-news-4) ⭐️ 8.0/10
5. [Oil Prices Near $100, European Gas Doubles on Supply Fears](#item-finance-news-5) ⭐️ 8.0/10
6. [NVIDIA and ASML Join Mistral AI’s €3 Billion Funding Round](#item-finance-news-6) ⭐️ 8.0/10
7. [Amkor Announces $12B Arizona Expansion](#item-finance-news-7) ⭐️ 8.0/10
8. [Stock Market Falls on US-Iran Tensions; Qualcomm Rises on Amazon Deal](#item-finance-news-8) ⭐️ 8.0/10
9. [Brent crude nears $100 after Houthi strikes hit Saudi oil sites](#item-finance-news-9) ⭐️ 8.0/10
10. [Oil Prices Climb as U.S. Renews Strikes on Iran](#item-finance-news-10) ⭐️ 8.0/10
11. [Federal Reserve holds rates steady but signals possible hikes](#item-finance-news-11) ⭐️ 8.0/10
12. [Fed holds interest rate steady; Powell holds press briefing](#item-finance-news-12) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Claims Navier–Stokes Prize Result Amid Scooping Accusations](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI stated that one of its unreleased internal models produced a claimed resolution of the Navier–Stokes existence and smoothness problem, one of the $1,000,000 Clay Millennium Prize Problems. According to OpenAI&\#x27;s account, rumors heard on September 1 and the internal model&\#x27;s performance prompted an evaluation of all open Millennium Prize problems; agents reached the Navier–Stokes result on September 5 after about 88 hours, with Lean formalization and verification taking another 17 hours via GPT-6 Astra. The effort consumed 4.9 million agent messages and roughly 300 billion output tokens across all problems, including 2.7 million messages and about 130 billion tokens for Navier–Stokes. The announcement is clouded by NYU mathematician Tristan Buckmaster, who published an urgent preprint with Anthropic mathematician Levent Alpöge and accused OpenAI of scooping their year-long effort; OpenAI said it did not access their user data but could not rule out that de-identified data from their product use helped improve models, and it declined to add Alpöge as co-author because of his employer.

rss · Simon Willison · Sep 8, 23:55

**「Background」** The Navier–Stokes existence and smoothness problem asks whether the fluid-flow equations always have global, smooth solutions from smooth initial data or can develop singularities in finite time; it is one of seven Clay Mathematics Institute Millennium Prize Problems announced in 2000 with a $1,000,000 prize for each. No solution has been officially accepted, and an accepted solution would require rigorous verification, usually by publication and peer review.

**「Impact」** For anyone using commercial AI coding tools for sensitive research — as Buckmaster and Alpöge did — the episode makes concrete the previously abstract worry that private work entered into products like Codex might later influence models and help others reach the same result first, even if outright data access is denied.

**「Community Discussion」** Hacker News commenters linked to Tristan Buckmaster&\#x27;s statement and asked whether OpenAI&\#x27;s claimed proof was derived from his and Alpöge&\#x27;s private work and prompts, while quoting Terence Tao&\#x27;s warning that rumors of a solution can now trigger large AI-powered races that discourage sharing research directions. Others noted the buried claim that an internal model trained for under two weeks was reportedly more than twice as capable mathematically as the just-released GPT-6 Astra, quoted the announcement&\#x27;s finite-time-singularity result, and expressed ambivalence about the capability being developed without public oversight.

**Tags**: `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize`, `#AI research`, `#mathematics`

---

<a id="item-tech-news-2"></a>
### [Google DeepMind launches AlphaGenome Atlas, a predictive map of every human DNA letter change](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 8.0/10

Google DeepMind has released AlphaGenome Atlas, a predictive map of every possible DNA letter change in the human genome, announced on Google&\#x27;s blog and made available through a dedicated DeepMind science page. The model is designed to help researchers understand both coding and non-coding genetic variation, and it can be accessed by anyone, with users reporting that no formal affiliation is required. It builds on DeepMind&\#x27;s track record of applying deep learning to biology, though its practical impact in genomics remains to be demonstrated. The resource provides a high-resolution map of human DNA changes, which could support research into pathogenic mutations and broader genetic science.

hackernews · utiiiD · Sep 8, 14:55 · [Discussion](https://news.ycombinator.com/item?id=49611251)

**「Background」** AlphaGenome Atlas is a catalogue from Google DeepMind that predicts molecular effects and AVI scores for 9 billion single-nucleotide variants—single DNA letter changes—across the human genome. The AlphaGenome model debuted in June 2025, and DeepMind has since applied it to every location in the genome to generate this predictive map, including non-coding DNA where many disease-associated variants lie.

**「Impact」** AlphaGenome Atlas now gives researchers free, searchable access to AlphaGenome’s precomputed regulatory-effect predictions for roughly 9 billion possible single-letter DNA changes in the human genome, which can accelerate variant interpretation and hypothesis generation in genomics and genetic-disease research. The database catalogs molecular effects of variants rather than providing clinical diagnoses, so downstream validation is still required.

**「Community discussion」** Commenters asked whether the tool can be used with consumer genetic tests such as 23andMe to find pathogenic mutations, while others sought more detail on how promoter sequences and transcription regulation are represented. Some commenters noted that not all DeepMind biology models have had lasting impact in their fields, suggesting the value of AlphaGenome Atlas will depend on real-world adoption and validation.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas : Molecular predictions for 9 Billion human DNA ...</a></li>
<li><a href="https://theoutpost.ai/news-story/google-deep-mind-unveils-alpha-genome-atlas-with-9-billion-human-genome-mutation-predictions-30577/">Google DeepMind &#x27;s AlphaGenome Atlas Maps 9 Billion Human ...</a></li>
<li><a href="https://www.techeblog.com/google-deepmind-alphagenome-atlas-human-dna-map/">Google DeepMind &#x27;s AlphaGenome Atlas Places a Score... - TechEBlog</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">AlphaGenome Atlas: a high-resolution map of human DNA</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA variants — Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#genomics`, `#deep learning`, `#bioinformatics`, `#research`

---

<a id="item-tech-news-3"></a>
### [NeurIPS Desk-Rejects 178 Papers Using AI Detector That Flags Its Own Chairs](https://www.reddit.com/r/MachineLearning/comments/1wakf62/neurips_deskrejected_178_papers_for_being/) ⭐️ 8.0/10

NeurIPS&\#x27;s Position Paper Track desk-rejected 178 papers, 18.4% of the track&\#x27;s submissions, using the proprietary AI detector Pangram with no human review and no appeal. Independent researchers found the same detector would have flagged the track chairs&\#x27; own recent papers as containing 24% to 69% AI text, placing them at risk under the rules applied. Pangram&\#x27;s default settings originally flagged 42.7% of the track as 90-100% AI-generated, and the flag rate was reduced to 12.7% only after the text windows used for evaluation were shortened. Twenty-two of the rejected papers scored above 0.5 and were treated as proof that the authors&\#x27; denial of AI use was false. A Stanford study shows 61.22% of human-written TOEFL essays are misclassified, and NeurIPS published no demographic calibration data, so the process was particularly risky for non-native English authors; the write-up notes that rejected papers carry no blacklist and can be resubmitted to ICLR \(deadline September 25\) or ICML.

reddit · r/MachineLearning · /u/tughanbulut · Sep 8, 10:19

**「Background」** NeurIPS is a leading machine learning conference; its position paper track had a policy requiring authors to disclose or avoid AI-generated content, enforced this June by the proprietary Pangram AI detector. Desk rejection means manuscripts were removed without human peer review or appeal, based solely on detector scores. Independent analyses and community posts have since questioned the detector&\#x27;s calibration, noting that even the track chairs&\#x27; own papers were flagged at high percentages.

**「Impact」** For the 178 rejected authors, the decision was final with no human review or appeal, but it carries no blacklist; the affected papers may be resubmitted to ICLR \(deadline September 25\) or ICML.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.neurips.cc/2026/06/02/ai-generated-papers-in-the-neurips-2026-position-paper-track/">AI-Generated Papers in the NeurIPS 2026 Position Paper Track – NeurIPS Blog</a></li>
<li><a href="https://casrai.org/news/neurips-2026-pangram-ai-detector-desk-rejection-controversy">NeurIPS 2026: Pangram AI-Detector Desk Rejections — CASRAI</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1tvwctd/neurips_used_uncalibrated_ai_detector_for_desk/">r/MachineLearning on Reddit: NeurIPS used uncalibrated AI detector for desk rejections [D]</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#AI detection`, `#academic publishing`, `#research ethics`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [ASML and TSMC Plan High NA EUV Shift to 12-Inch Photomasks](https://www.nrc.nl/nieuws/2026/09/08/asml-gaat-samenwerken-met-taiwanese-chipgigant-tsmc-om-zijn-nieuwste-chipmachines-te-upgraden-a4936073) ⭐️ 8.0/10

On September 7, ASML and TSMC launched an industry collaboration to shift High NA EUV lithography from the current 6-inch photomask format to 12-inch reticles, aiming to improve productivity, lower chip manufacturing costs, and reduce stitching constraints. The companies plan to establish a 12-inch photomask pilot production line by 2031 and introduce the associated systems for advanced-node volume production around 2033. TSMC intends to begin using High NA EUV for large-scale manufacturing at advanced nodes starting in 2030. The transition would affect reticle infrastructure and the EUV tooling roadmap for next-generation semiconductor production.

telegram · zaihuapd · Sep 8, 06:55

**「Background」** High NA EUV, or high numerical aperture extreme ultraviolet lithography, is the successor to current EUV systems and offers better resolution for shrinking chip features without increasing reliance on multiple patterning. Today&\#x27;s EUV tools use 6-inch photomasks to carry the circuit pattern onto wafers; moving to a larger 12-inch mask format would enlarge the printable field and reduce the need to stitch multiple fields together. ASML is the leading supplier of EUV lithography equipment, and TSMC is one of the most advanced chipmakers using such systems for leading-edge production.

**Tags**: `#semiconductor`, `#photolithography`, `#ASML`, `#TSMC`, `#High NA EUV`

---

<a id="item-tech-news-5"></a>
### [Meta Announces Muse, a Personal AI Agent](https://ai.meta.com/muse/) ⭐️ 7.0/10

Meta has introduced Muse, a personal AI agent, with a dedicated page at ai.meta.com/muse. The launch matters because it moves the AI-agent race toward mainstream consumers rather than just power users and developers, leveraging Meta&\#x27;s large existing user base. The available source does not include release date, model information, or feature specifications for Muse. Community reaction already focuses on whether Meta can secure such an agent against prompt injection and whether users will trust it with sensitive personal data.

hackernews · yks · Sep 8, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49615537)

**「Background」** Meta announced Muse, a personal AI agent built on the latest generation of models developed under chief AI officer Alexandr Wang, and is rolling it out in the United States on iOS, Android, and the web at muse.ai. The product was touted by CEO Mark Zuckerberg as a key next step in Meta&\#x27;s AI strategy, with the company emphasizing safety and privacy in its launch materials. This represents Meta&\#x27;s push into the personal assistant space, following broader industry trends toward AI agents that can perform tasks on behalf of users.

**「Community Discussion」** Commenters are split: some believe Muse is Meta&\#x27;s attempt to serve mainstream users who do not follow model releases closely, while others say they would never let Meta run a personal agent and prefer building their own. One commenter cites Meta engineering lead David Singleton&\#x27;s description of layered prompt-injection defenses, and another says they want to use Muse to scrape Facebook groups after Meta&\#x27;s earlier API shutdown.

<details><summary>References</summary>
<ul>
<li><a href="https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/">Introducing Muse : The World’s First Personal AI Agent Built for...</a></li>
<li><a href="https://www.axios.com/2026/09/08/meta-debuts-muse-personal-ai-agent">Meta debuts Muse personal AI agent</a></li>
<li><a href="https://www.bnnbloomberg.ca/business/company-news/2026/09/08/meta-launches-personal-ai-agent-muse-emphasizes-safety-and-privacy/">Meta launches Muse , personal AI agent emphasizing safety &amp; privacy</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#AI agent`, `#personal assistant`, `#prompt injection`, `#tech industry`

---

<a id="item-tech-news-6"></a>
### [Qwen3.8 27B Quantization Benchmark: 4-bit Safe, 1-bit Collapses](https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/) ⭐️ 7.0/10

A benchmark of quantized Qwen3.8 27B models found that 4-bit quantizations preserve output quality, while 1-bit quantization collapses and 2-bit scores somewhat lower. The results offer actionable guidance for local model deployment, helping users balance quality against memory and compute constraints. The analysis emphasizes caution when interpreting differences, noting Wilson 95% confidence intervals are conservative for run-to-run noise. Community responses also call for more testing of KV cache quantization and of 3-bit models for sub-16 GB GPUs.

hackernews · stared · Sep 8, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49611128)

**「Background」** Qwen 3.8 27B is a dense, multimodal model from Alibaba&\#x27;s Qwen 3.8 family that can run locally on a 24 GB GPU or 32 GB Mac at 4-bit quantization; the full BF16 version weighs about 55 GB, too large for most consumer hardware. Quantization reduces numerical precision \(e.g., from 16-bit to 4-bit or 1-bit\) to shrink model files, and GGUF formats like Q4\_K\_M are common for local inference. This benchmark compares those quantized versions of the model on the agentic coding benchmark Terminal-Bench 2.1, reporting that a 17 GB Q4\_K\_M matches the full model while lower-bit versions degrade.

**「Impact」** Developers deploying Qwen3.8 27B locally can rely on 4-bit quantizations to retain most model quality, while 1-bit should be avoided because it degrades output drastically. Users with GPUs below 16 GB may still need benchmarks around the 3-bit range to find their practical quality knee.

**「Community Discussion」** Commenters theorize that Qwen3.8 27B compensates for quantization-induced probability shifts by thinking longer, which may explain why lower quant levels lose little benchmark quality. Others request KV cache quantization benchmarks for long-context coding use, point out a missing Q3 datapoint for sub-16 GB cards, and a newcomer asks about safely running such models on personal PCs.

<details><summary>References</summary>
<ul>
<li><a href="https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/">Benchmarking Qwen 3 . 8 27 B quantizations : 4-bit... - Quesma Blog</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#qwen`, `#benchmarking`, `#llm-inference`, `#local-models`

---

<a id="item-tech-news-7"></a>
### [Malaysia Eyes Huawei Ascend Chips for $494M Sovereign AI Project](https://www.businesstimes.com.sg/international/malaysia-eyes-huawei-chips-ai-project-despite-us-warning) ⭐️ 7.0/10

Malaysia is seriously evaluating Huawei&\#x27;s Ascend 910C AI accelerator chips for a sovereign AI project budgeted at 2 billion ringgit \(about $494 million\). If the plan materializes, it would be the first case in which a foreign government officially selects Chinese AI accelerators over US alternatives. The number of chips Malaysia would procure remains unclear, according to people familiar with the matter. The Trump administration warned last year that using the Huawei AI accelerator could violate US export rules, but the Malaysian government views the decision as purely commercial. The Business Times reported the development, citing unnamed sources.

telegram · zaihuapd · Sep 8, 03:35

**「Background」** The Huawei Ascend 910C is an AI accelerator processor developed by Huawei and its chip designer HiSilicon, positioned as a Chinese alternative to U.S. AI chips such as those from Nvidia. Washington has warned that using the 910C could breach U.S. export controls, which were tightened against advanced semiconductor exports to China. Malaysia’s potential RM2 billion sovereign AI project would mark a notable geopolitical shift by exploring Chinese AI chips for the first time, despite U.S. warnings and regional supply-chain tensions.

**「Impact」** Should Malaysia follow through, it would become the first foreign government publicly to choose Huawei&\#x27;s Chinese AI chips over US options for a state AI project, a precedent that could heighten US export-control scrutiny of the deal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.globalsources.com/sourcing-digest/malaysia-evaluates-huawei-ascend-910c-chips-for-a-landmark-sovereign-ai-initiative/?source=GSOLHP_SKC_5">Malaysia evaluates Huawei Ascend 910 C chips for... | Global Sources</a></li>
<li><a href="https://www.scmp.com/week-asia/politics/article/3366792/will-malaysias-potential-huawei-ai-deal-risk-clash-over-us-trade-pact">Will Malaysia ’s potential Huawei AI deal risk clash with US trade pact?</a></li>
<li><a href="https://techwireasia.com/2026/09/kirin-9050-pro-logicfolding-malaysia-ascend-910c/">Kirin 9050 Pro proves Huawei &#x27;s workaround. Malaysia is buying the...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#AI chips`, `#Malaysia`, `#export controls`, `#sovereign AI`

---

<a id="item-tech-news-8"></a>
### [Zhang Yiming Oversees ByteDance Real-Time Spatial Video Model](https://www.bloomberg.com/news/articles/2026-09-07/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models) ⭐️ 7.0/10

According to Bloomberg, people familiar with the matter say ByteDance founder Zhang Yiming is personally overseeing development of a real-time spatial video generation model that could launch as early as October 2026, though the timeline may shift. The model is built on ByteDance&\#x27;s Seedance foundation and is designed to generate interactive virtual worlds that respond to voice or actions from users of Pico VR headsets. It reportedly produces video at roughly 0.05 seconds of latency and 20 frames per second, offloading heavy computation to the cloud to lower hardware requirements for VR devices. The move signals ByteDance&\#x27;s and Zhang Yiming&\#x27;s deeper push into world models and interactive AR/VR experiences, but the report cites unnamed insiders and no official confirmation or detailed technical specifications have been released.

telegram · zaihuapd · Sep 8, 04:05

**「Background」** Zhang Yiming, the founder of ByteDance, has stepped back from day-to-day operations but is personally steering the company&\#x27;s development of a real-time &\#x27;world model&\#x27; built on its Seedance video AI. Spatial-video or world models aim to place a user inside an interactive three-dimensional environment, similar to Google&\#x27;s Genie. The project reportedly links ByteDance&\#x27;s AI models and cloud resources with its content platforms and Pico VR hardware.

**「Impact」** If the model ships as reported, it would let Pico VR headset users interact with real-time, cloud-rendered virtual worlds without requiring high-end local hardware, positioning ByteDance against existing world-model efforts such as World Labs&\#x27; Atlas. The October 2026 timeline remains unconfirmed and could shift, so its competitive impact is still conditional.

<details><summary>References</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models">ByteDance founder joins AI elite in race to perfect world models</a></li>
<li><a href="https://technode.com/2026/09/08/bytedance-real-time-spatial-video-model-zhang-yiming/">ByteDance is reportedly developing a real-time spatial video model ...</a></li>
<li><a href="https://startupfortune.com/zhang-yiming-is-personally-building-bytedances-real-time-world-model/">Zhang Yiming Is Personally Building ByteDance &#x27;s Real-Time World...</a></li>
<li><a href="https://www.worldlabs.ai/blog/atlas">Atlas: A World Model for Spatial Intelligence | World Labs</a></li>
<li><a href="https://www.straitstimes.com/business/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models">ByteDance founder joins AI elite in race to perfect world models</a></li>

</ul>
</details>

**Tags**: `#ByteDance`, `#spatial video`, `#world models`, `#real-time AI`, `#VR/AR`

---

<a id="item-tech-news-9"></a>
### [China targets 9,800 EFLOPS intelligent computing by 2030](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 7.0/10

China&\#x27;s Ministry of Industry and Information Technology has issued a five-year industrial plan targeting 9,800 EFLOPS of intelligent computing capacity by 2030, according to a South China Morning Post report. The plan calls for cumulative information-infrastructure investment of 3.8 trillion yuan from 2026 to 2030, orderly deployment of intelligent computing clusters at the 10,000-card scale and above 100,000 cards, and stronger adaptation of infrastructure to domestically produced AI chips. According to data cited in the report, China&\#x27;s intelligent computing capacity stood at 2,185 EFLOPS as of the end of June, up 177% year on year, so the 2030 target implies growth of more than four times. The policy gives Chinese data-center operators and domestic chip suppliers a concrete multi-year planning benchmark, though its capacity and investment figures are goals rather than binding outcomes.

telegram · zaihuapd · Sep 8, 11:23

**「Background」** China&\#x27;s Ministry of Industry and Information Technology \(MIIT\) oversees industrial policy and has published a five-year plan for the information and communications sector covering 2026–2030. Intelligent computing \(智能算力\) refers to computing capacity oriented toward artificial intelligence workloads and is measured in EFLOPS, or exafloating-point operations per second \(10^18 operations per second\). As of the end of June, China&\#x27;s intelligent computing capacity stood at 2,185 EFLOPS, up 177% year on year, so the 2030 target of 9,800 EFLOPS represents more than a fourfold increase from that base.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/miit-plan-targets-9800-eflops-of-intelligent-compute-by-2030/">MIIT Plan Targets 9,800 Eflops of Intelligent Compute by 2030</a></li>
<li><a href="https://aiweekly.co/alerts/miit-targets-9800-eflops-of-ai-compute-by-2030-532b-plan">MIIT Targets 9,800 Eflops of AI Compute by 2030 , $532B Plan</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#China`, `#policy`, `#EFLOPS`, `#compute`

---

<a id="item-tech-news-10"></a>
### [OpenAI Launches Faster ChatGPT Images 2.5](https://openai.com/index/introducing-chatgpt-images-2-5/) ⭐️ 7.0/10

On September 8, OpenAI announced ChatGPT Images 2.5, its updated image generation model offering sharper detail, more precise editing, and generation latency up to 50% lower than ChatGPT Images 2.0. The model is rolling out to ChatGPT, ChatGPT Work, and Codex users, accompanied by new ChatGPT features such as Sketch hand-drawn guidance, templates, image comments, and prompt sharing. The API also gains two new model variants: GPT-Image-2.5 Flare and GPT-Image-2.5 Sunburst. This update is significant because it gives a broad set of OpenAI customers and developers immediate access to an improved image model with faster performance.

telegram · zaihuapd · Sep 8, 18:45

**「Background」** OpenAI has been rolling out successive versions of its ChatGPT image-generation models, with the 2.0 release establishing a baseline for image clarity, editing, and generation speed. ChatGPT Images 2.5 is the next incremental update, introduced with two API model variants: GPT-Image-2.5 Flare, which inherits the quality, editing, and speed improvements, and GPT-Image-2.5 Sunburst, which adds extra precision for detailed creative work at the cost of longer generation times. OpenAI says the new model reduces image-generation latency by up to 50% compared with 2.0 and adds features like Sketch-guided creation, templates, image comments, and prompt sharing across ChatGPT products.

**「Impact」** For developers and organizations using the image API, the addition of GPT-Image-2.5 Flare and Sunburst provides two new endpoint options to integrate the upgraded model into their applications.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2 . 5 | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#image-generation`, `#ChatGPT`, `#API`, `#AI-models`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Iran’s Oil Exports Plummet Under U.S. Strait of Hormuz Blockade](https://oilprice.com/Energy/Crude-Oil/Irans-Oil-Exports-Collapse-as-Hormuz-Standoff-Drags-On.html) ⭐️ 9.0/10

Ship-tracking estimates show Iran’s oil export loadings collapsed in August to roughly 260,000 barrels per day, down 80% from 1.7 million barrels per day a year earlier, according to data from Kpler cited by CNBC. The reinstated U.S. blockade has also cut actual Iranian oil flows out of the Persian Gulf to zero last month, several trackers estimate.

rss · OilPrice.com · Sep 9, 00:00

**「Background」** Washington reimposed its naval blockade in mid-July after only a three-week pause, preventing Iranian tankers from reaching the Strait of Hormuz, a key route for Gulf oil shipments.

**「Impact」** The standoff is already showing up at U.S. pumps: the report says diesel has hit a record high and average gasoline prices were above $4 per gallon last weekend.

**Tags**: `#Iran`, `#oil exports`, `#Strait of Hormuz`, `#U.S. sanctions`, `#oil prices`

---

<a id="item-finance-news-2"></a>
### [US Federal Reserve Holds Rates Steady Under New Chair Warsh](https://news.google.com/rss/articles/CBMipgFBVV95cUxOM3c5cXgydnhwSFlrWmlyVjJobnRCbFkxaHg2c3NtTEl6Z2VLSGNIMXN3dmlKS2JZSF9Gc2p1TTVrd1hEcVdxSzBRaU13RVh1eTJRLW1pRkp0cHdKbk9FSU5SZ2FncC1ZangzQzZkZjFSaHNRWm94TlNROExtSm56Zk1qckpwT1JweWVKV1daY0tUMk03eFZJakRpMjNBVzl5N1NEQzFn0gGrAUFVX3lxTE1wYkYxa2NtTktYZkMyQ3VCSG5vYkw3UkE1cGpqaTRwOXE1MVpsd1ZfbDA2X3lGOEF5WG51SHFBbEhXbWs1enFfS1k2ZWRDMzVUU21sT2RMbC04VkoxUXk0Z1pYMVpWejF0ZGNyaUpiVWxjLWZYWVVBU28tb082QWlwT29PX1o3ekFTUk1fdTdGb3drUm5FOEIzZEc3UGlCRjhaUDlsS3Y0Yk8wMA?oc=5) ⭐️ 9.0/10

The US Federal Reserve, under its new Chair Warsh, held interest rates steady, according to Al Jazeera. The decision signals continuity in the central bank&\#x27;s monetary policy.

google\_news · aljazeera.com · Jun 17, 07:00

**「Background」** The decision came at the Fed&\#x27;s first policy meeting under Chair Kevin Warsh, who took office amid heightened inflation and rising market interest rates driven partly by U.S. government deficits and heavy corporate borrowing for AI infrastructure. The central bank held its benchmark range at 3.5–3.75 percent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh | Inflation News | Al Jazeera</a></li>
<li><a href="https://apnews.com/article/inflation-federal-reserve-interest-rates-a8661a4be7fcf3076891382cf9df1a5e">New Fed chair Kevin Warsh under pressure to clarify views on inflation, interest rates | AP News</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#US economy`, `#central bank`

---

<a id="item-finance-news-3"></a>
### [Copper Hits Record Above $14,500 as Expected U.S. Tariffs Squeeze Supply](https://oilprice.com/Metals/Commodities/Copper-Surges-Above-14500-as-Supply-Squeeze-Deepens.html) ⭐️ 8.0/10

London copper futures hit a record high on Tuesday, reaching $14,533 a ton, as expectations of U.S. tariffs pulled record volumes into American warehouses and tightened availability elsewhere. The metal has risen 17% this year and 47% over the past 12 months, according to Bloomberg data.

rss · OilPrice.com · Sep 8, 21:00

**「Background」** Copper is used in power grids, data centers, and industrial supply chains; global mining constraints and tariff-driven shifts have left large amounts of metal in the United States rather than where it is needed.

**「Impact」** Projects that depend on copper—such as data centers, grid expansions, and industrial electrification—could face higher costs and slower availability because of regional shortages.

**Tags**: `#copper`, `#commodities`, `#tariffs`, `#supply chain`, `#industrial metals`

---

<a id="item-finance-news-4"></a>
### [U.S.-Saudi Nuclear Deal Clears IAEA Hurdle as Congress Review Continues](https://oilprice.com/Alternative-Energy/Nuclear-Power/US-Saudi-Nuclear-Deal-Clears-Vienna-Hurdle-As-Congress-Review-Continues.html) ⭐️ 8.0/10

IAEA chief Rafael Grossi said Monday that Saudi Arabia will not sign the Additional Protocol—the inspection tool that allows surprise visits to undeclared sites—but will give the agency monitoring powers over uranium enrichment, conversion, and reprocessing that are “very, very similar” to it. The U.S.-Saudi nuclear agreement is now in a 90-day congressional review that began in late August, meaning it can take effect unless lawmakers pass a resolution of disapproval that survives a presidential veto.

rss · OilPrice.com · Sep 8, 17:00

**「Background」** The pact is a “123 agreement”—named for the section of the U.S. Atomic Energy Act governing nuclear exports—signed on July 22; it would allow American firms to build reactors in the kingdom and study domestic uranium enrichment under U.S. supervision, a contrast with the 2009 U.S.-UAE deal that permanently gave up enrichment and reprocessing.

**「Impact」** If Congress lets the agreement take effect, U.S. nuclear vendors such as Westinghouse could compete for reactor contracts in Saudi Arabia worth billions, while critics in Congress and nonproliferation groups warn it could encourage a Middle East enrichment race.

**Tags**: `#nuclear energy`, `#Saudi Arabia`, `#IAEA`, `#US foreign policy`, `#nonproliferation`

---

<a id="item-finance-news-5"></a>
### [Oil Prices Near $100, European Gas Doubles on Supply Fears](https://oilprice.com/Energy/Crude-Oil/Oil-Prices-Are-Once-Again-on-the-Brink-of-100.html) ⭐️ 8.0/10

Oil prices rose above $99 a barrel, the highest in three months, after Houthi attacks on Saudi energy facilities and U.S. strikes on Iranian tankers raised supply concerns. European natural gas prices jumped to €75 per megawatt-hour, more than double their level a year earlier, as low gas storage stoked winter-supply fears.

rss · OilPrice.com · Sep 8, 15:13

**「Background」** The rises follow Houthi strikes that forced shutdowns at Saudi sites such as the 400,000-barrel-a-day Jazan refinery and U.S. attacks on Iranian tankers, while European gas storage at 66% capacity leaves Germany and the Netherlands especially exposed ahead of winter.

**「Impact」** European households and businesses face higher gas heating and power costs this winter, because Germany and the Netherlands have low storage levels and the EU has not imported Qatari LNG since April, reducing the buffer against supply disruptions.

**Tags**: `#oil prices`, `#geopolitical risk`, `#European gas`, `#energy markets`, `#OPEC+`

---

<a id="item-finance-news-6"></a>
### [NVIDIA and ASML Join Mistral AI’s €3 Billion Funding Round](https://finance.yahoo.com/technology/ai/articles/nvidia-asml-back-mistral-3-230147307.html) ⭐️ 8.0/10

NVIDIA and ASML are backing Mistral AI’s new €3 billion funding round, according to the report. The two hardware companies’ expected payoffs could differ due to their distinct strategic interests in the AI industry.

openbb · NVDA · Sep 8, 23:01

**「Background」** Mistral, a French AI startup focused on open-weight AI models, announced the Series D round on September 8 at a post-money valuation above €21 billion \(about $24.4 billion\). Existing backers NVIDIA and ASML joined the round, which the company says is the largest equity fundraising by a European technology firm.

**「Impact」** ASML’s roughly $1.5 billion investment would help build sovereign high-performance computing infrastructure in France, potentially reducing Europe’s reliance on US and Chinese AI models while shifting some chip demand to the region.

<details><summary>References</summary>
<ul>
<li><a href="https://ca.finance.yahoo.com/news/nvidia-asml-back-mistral-3-230147307.html">NVIDIA and ASML Back Mistral’s €3 Billion Round. Their Payoffs Could Look Very Different</a></li>
<li><a href="https://ventureburn.com/mistral-raises-3-billion-sovereign-open-weight-ai/">Mistral Raises €3 Billion To Build The Future of Secure Open-Weight AI</a></li>
<li><a href="https://www.cryptopolitan.com/mistral-raise-asml-chip-deal-europe-ai-push/">Mistral raises €3B as ASML seals chip deals in European AI push - Cryptopolitan</a></li>
<li><a href="https://ioplus.nl/en/posts/why-asml-is-investing-15b-in-mistral---and-why-it-makes-sense">Why ASML is investing $1.5B in Mistral - and why it makes sense</a></li>
<li><a href="https://finance.yahoo.com/news/asml-invests-billions-nvidia-backed-095358773.html">ASML Invests Billions In Nvidia-Backed Mistral AI To Power Next Era Of Semiconductors</a></li>

</ul>
</details>

**Tags**: `#Mistral AI`, `#NVIDIA`, `#ASML`, `#Venture Capital`, `#AI Industry`

---

<a id="item-finance-news-7"></a>
### [Amkor Announces $12B Arizona Expansion](https://finance.yahoo.com/markets/stocks/articles/amkr-stock-gains-hours-amkor-234207542.html) ⭐️ 8.0/10

Amkor announced plans for a $12 billion expansion of its Arizona campus to increase US chip manufacturing, and its shares gained in after-hours trading.

openbb · NVDA · Sep 8, 23:42

**「Background」** Amkor Technology is an outsourced semiconductor assembly and test \(OSAT\) company. Its earlier Phase 1 work in Arizona is being followed by Phase 2, which expands the company&\#x27;s total planned investment in the campus to about $12 billion; construction for Phase 2 is expected to begin in late 2027 and be completed by the end of 2029.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stocktitan.net/news/AMKR/amkor-technology-announces-phase-2-of-arizona-advanced-packaging-and-m19aoplwpjtk.html">A roughly $12B expansion to package chips is planned in Arizona. Construction is anticipated to begin late 2027.</a></li>
<li><a href="https://newsable.asianetnews.com/markets/amkr-stock-gains-after-hours-amkor-doubles-down-on-us-chip-manufacturing-with-12b-arizona-campus-expansion-articleshow-uq2pq4z">AMKR Stock Gains After-Hours — Amkor Doubles Down On US Chip Manufacturing With $12B Arizona Campus Expansion | Asianet Newsable</a></li>
<li><a href="https://lifestyle.middletownlifemagazine.com/story/676376/amkor-technology-announces-phase-2-of-arizona-advanced-packaging-and-test-campus-expands-investment-to-12-billion/">Amkor Technology Announces Phase 2 of Arizona Advanced Packaging and Test Campus; Expands Investment to $12 Billion | Middletown Life</a></li>

</ul>
</details>

**Tags**: `#Semiconductors`, `#Capital Expenditure`, `#Manufacturing`, `#Amkor`, `#US Supply Chain`

---

<a id="item-finance-news-8"></a>
### [Stock Market Falls on US-Iran Tensions; Qualcomm Rises on Amazon Deal](https://www.investors.com/market-trend/stock-market-today/dow-jones-sp500-nasdaq-us-iran-attacks-oil-prices-jump-brent-crude/?src=A00220&amp;yptr=yahoo) ⭐️ 8.0/10

U.S. stocks fell, with the Dow dropping, as US-Iran tensions pushed oil prices higher; Qualcomm shares cleared a key level after an Amazon deal and a fertilizer leader rose.

openbb · BRK-B · Sep 8, 20:51

**「Background」** Trading resumed after the Labor Day holiday with oil prices spiking toward $100 a barrel following an attack on Saudi Arabia by Iran-backed Houthis, stoking inflation fears and dragging the Dow down 511 points.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hindustantimes.com/business/stock-market-today-dow-falls-511-points-as-oil-nears-100-us-iran-war-fuels-inflation-fears-101788881180215.html">Stock market today: Dow falls 511 points as oil nears $100, US-Iran war fuels inflation fears | Business News</a></li>
<li><a href="https://www.europesays.com/us/1051686/">Stock Market Today: Dow Dives, Qualcomm Clears Key Level On Amazon Deal; Fertilizer Leader Rises - United States</a></li>

</ul>
</details>

**Tags**: `#stock market`, `#Dow Jones`, `#oil prices`, `#Qualcomm`, `#geopolitical risk`

---

<a id="item-finance-news-9"></a>
### [Brent crude nears $100 after Houthi strikes hit Saudi oil sites](https://finance.yahoo.com/energy/articles/brent-crude-nears-100-houthi-122207804.html) ⭐️ 8.0/10

Houthi strikes on Saudi oil sites pushed Brent crude — the main international oil price benchmark — close to $100 a barrel, highlighting the risk of supply disruptions.

openbb · BRK-B · Sep 8, 12:22

**「Background」** Houthi attacks on Saudi energy facilities are part of renewed fighting after the militants declared a maritime blockade, threatening the Bab al-Mandeb strait—a key Red Sea shipping chokepoint—and forcing Riyadh to suspend some operations.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/energy/articles/brent-crude-nears-100-houthi-122207804.html">Brent crude nears $ 100 as Houthi strikes hit Saudi oil sites</a></li>
<li><a href="https://walletinvestor.com/news/trading-news/oil-nears-100-after-houthi-strikes-hit-saudi-energy-facilities/">Oil Nears $ 100 After Houthi Strikes Hit Saudi ... - WalletInvestor.com</a></li>

</ul>
</details>

**Tags**: `#oil`, `#geopolitics`, `#energy`, `#supply disruption`, `#crude`

---

<a id="item-finance-news-10"></a>
### [Oil Prices Climb as U.S. Renews Strikes on Iran](https://news.google.com/rss/articles/CBMingFBVV95cUxPX1k2M25nYzF5bW1Db3RnMldRZ19jWklIUWthSDVPNkhIRk5QQXZfd2dCMHdvNmdrbU1KMlVwYjJZaEtPZzhEa3R3bTBvTEl4MDJ6Q2dWby1NZlJsYi15TzdnWVZLcmg2TTBkVm1NNWhWYlgtM3VFa3RieUJMN2V6NTBSQTFvck1HVkU5NzQ0aHQ2eXJDNGZIVmVKZVNRZw?oc=5) ⭐️ 8.0/10

The United States renewed strikes on Iran, and oil prices climbed, NBC News reported, reviving worries that the conflict could disrupt supplies and push inflation higher.

google\_news · nbcnews.com · Sep 1, 17:26

**「Background」** The U.S. military announced further strikes against Iran, deepening concerns over supply disruptions through the Strait of Hormuz. This led the global Brent crude benchmark to climb nearly 4% to $94 a barrel, stoking inflation fears.

**「Impact」** Consumers and businesses could feel the effect through higher fuel and transportation costs if oil prices stay elevated, since those costs often feed into broader inflation.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/bond-yields-surge-stocks-tumble-143402187.html">Oil prices surge after U . S . renews Iran strikes , heightening ...</a></li>
<li><a href="https://www.puprime.com/oil-surges-as-hormuz-disruption-deepens-dma260902/">Oil Surges as Hormuz Disruption Deepens</a></li>

</ul>
</details>

**Tags**: `#oil prices`, `#Iran`, `#inflation`, `#geopolitical risk`, `#energy markets`

---

<a id="item-finance-news-11"></a>
### [Federal Reserve holds rates steady but signals possible hikes](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

The Federal Reserve left its benchmark interest rate unchanged but kept the possibility of a future rate hike open, according to CBS News. No specific rate level or timing was reported in this item.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The Federal Reserve left its benchmark interest rate unchanged on Wednesday, but a significant number of policymakers signaled they would support another rate increase later this year if inflation stays high.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aol.com/articles/federal-holds-interest-rates-steady-181753000.html">Federal Reserve holds interest rates steady but leaves door open ...</a></li>
<li><a href="https://www.kzyx.org/npr-news/2026-07-29/a-divided-federal-reserve-holds-interest-rates-steady-despite-high-inflation">A divided Federal Reserve holds interest rates steady despite high...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-12"></a>
### [Fed holds interest rate steady; Powell holds press briefing](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 8.0/10

The Federal Reserve left its benchmark interest rate unchanged, and Chair Jerome Powell held a news briefing after the decision.

google\_news · PBS · Mar 18, 07:00

**「Background」** The Federal Reserve kept its benchmark rate in a range of 4.25% to 4.5%, marking the second straight meeting without a change after three cuts in 2024. Chair Jerome Powell said he plans to remain on the board after his term leading the central bank ends.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fox7austin.com/money/feds-interest-rate-steady-jerome-powell">Fed holds rates steady in Powell ’s possible final chair... | FOX 7 Austin</a></li>
<li><a href="https://www.iheart.com/content/2025-03-19-federal-reserve-leaves-benchmark-interest-rate-unchanged/">Federal Reserve Leaves Benchmark Interest Rate Unchanged</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Jerome Powell`, `#Economy`

---