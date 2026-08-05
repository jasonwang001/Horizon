---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 206 items, 22 important content pieces were selected

---

**Technology News**
1. [Mistral Releases Shieldstral, a 3B Open-Weight Multimodal Moderation Model](#item-tech-news-1) ⭐️ 8.0/10
2. [Keyv and related npm packages hit by active Shai-Hulud supply chain attack](#item-tech-news-2) ⭐️ 8.0/10
3. [MiniMax-H3 MLX port brings local omni-modal video generation to Apple Silicon](#item-tech-news-3) ⭐️ 8.0/10
4. [US drafts ban on Chinese optical modules for AI data centers](#item-tech-news-4) ⭐️ 8.0/10
5. [China Issues First Mandatory L3/L4 Autonomous Driving Standard, Effective July 2027](#item-tech-news-5) ⭐️ 8.0/10
6. [A Custom Color Space for Generating Diverse Skin Tones](#item-tech-news-6) ⭐️ 7.0/10
7. [Waymo Opens Driverless Ride-Hailing to Everyone in Dallas](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek V4 Flash Runs on a Single AMD MI300X at 150+ Tokens/s](#item-tech-news-8) ⭐️ 7.0/10
9. [Oxide Computer raises $445M in new funding round](#item-tech-news-9) ⭐️ 7.0/10
10. [Huawei scientist warns Nvidia chip scaling will hit physical limits](#item-tech-news-10) ⭐️ 7.0/10
11. [Cloudflare Ditches Third-Party Security Tools for $58/Month AI Bounty Triage](#item-tech-news-11) ⭐️ 7.0/10
12. [White House Reverses on Open-Source AI Restrictions Amid Valley Split](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [Caterpillar and Palantir Lead Premarket Moves After Strong Earnings](#item-finance-news-1) ⭐️ 8.0/10
2. [Google builds $200bn financing structure to deliver AI chips to Anthropic](#item-finance-news-2) ⭐️ 8.0/10
3. [Procter &amp; Gamble to Acquire Thorne for $3.8 Billion](#item-finance-news-3) ⭐️ 8.0/10
4. [BP profit more than doubles on Middle East conflict](#item-finance-news-4) ⭐️ 8.0/10
5. [Goldman Sachs Equities Revenue Jumps 72% to Record $7.42 Billion in Q2](#item-finance-news-5) ⭐️ 7.0/10
6. [China Postal Regulator Opens Investigation into STO Express](#item-finance-news-6) ⭐️ 7.0/10
7. [NVIDIA Invests in Secretive AI Lab Chasing Superintelligence](#item-finance-news-7) ⭐️ 7.0/10
8. [AMD Beats Q2 Earnings and Reports Large Capital Expenditure Program](#item-finance-news-8) ⭐️ 7.0/10
9. [Chip Investors Remain Unsatisfied Despite Big Profits](#item-finance-news-9) ⭐️ 7.0/10
10. [McDonald&\#x27;s Earnings Beat Comes With Warning Sign](#item-finance-news-10) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Mistral Releases Shieldstral, a 3B Open-Weight Multimodal Moderation Model](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral announced Shieldstral, a 3B-parameter open-weights model for multimodal content moderation. The model is positioned as a small, cost-effective approach to moderation, fitting the company&\#x27;s newer strategy of releasing smaller, more fine-tuned models for specific use cases. Shieldstral is intended to help developers integrate moderation capabilities into platforms without relying on frontier-scale systems. The announcement did not include benchmark details, performance data, or specifics about support for arbitrary custom rulesets.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**「Background」** Shieldstral is a 3 billion parameter multimodal safety classifier released by Mistral AI under the open Apache 2.0 license, designed to moderate text and images for harmful content. Unlike classifiers that memorize fixed harm categories, it takes a moderation policy as input, allowing adaptivity to different rulesets without retraining. It reportedly outperforms models up to 7x its size and matches the text safety benchmark performance of the much larger GPT-OSS-Safeguard-20B, scoring 91.3% F1 on a policy-adaptability evaluation against a different taxonomy.

**「Impact」** Developers and platform operators now have a self-hostable 3B open-weight moderation model that adapts across policies via binary question answering, potentially reducing reliance on hosted endpoints such as OpenAI&\#x27;s free Omni Moderation. Independent production benchmarks are not yet available, so real-world reliability remains uncertain.

**「Community Discussion」** Commenters welcomed Shieldstral as a realistic and cost-effective first-pass moderation filter, while cautioning that non-deterministic models still require human review for sensitive decisions. Some questioned whether it can enforce arbitrary rulesets or only standard big-tech moderation policies, and compared it with OpenAI&\#x27;s omni-moderation model.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral’s Shieldstral Packs Policy-Adaptive Safety Screening ...</a></li>
<li><a href="https://cctest.ai/en/articles/shieldstral-turns-content-moderation-into-a-yes-or-no-multimodal-safety-task">Shieldstral : A 3B Adaptive Multimodal Safety Classifier - CCTest</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/moderation">Moderation | OpenAI API</a></li>

</ul>
</details>

**Tags**: `#Mistral`, `#content moderation`, `#open-weights`, `#multimodal`, `#AI safety`

---

<a id="item-tech-news-2"></a>
### [Keyv and related npm packages hit by active Shai-Hulud supply chain attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

An active npm supply chain attack dubbed Shai-Hulud has compromised Keyv and related packages, according to a report from Aikido.dev. The incident underscores the fragility of the JavaScript dependency ecosystem, where a compromise of a widely depended-on library can cascade through many downstream applications. Because it is active, users should treat affected installs as untrusted, audit their dependency trees, and be suspicious of new preinstall or postinstall hooks. Concrete remediation details were not available in the supplied item.

hackernews · cimi\_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**「Background」** Keyv is a popular key-value storage library on npm with roughly 127 million weekly downloads. The Shai-Hulud campaign is a supply-chain attack that began on August 4, 2023, after threat actors gained access to the maintainer&\#x27;s GitHub account and used that access to publish malicious updates across the maintainer&\#x27;s package portfolio. The attack has compromised more than 1,280 npm packages with a combined 2+ billion monthly installs, and the malware executes during npm install to steal credentials and other sensitive data.

**「Impact」** Developers depending on Keyv or the affected related packages should audit their lockfiles and CI pipelines now, and consider blocking install scripts until the scope of compromise is clarified.

**「Community discussion」** Commenters largely agree that package lifecycle hooks are a major attack vector, with some urging a moratorium on new preinstall/postinstall hooks. Practical suggestions included using devcontainers to isolate installs, running behavioral analysis tools like Packj, and asking GitHub to automatically block Shai-Hulud exfiltration repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package with 127M Weekly Downloads Compromised in ...</a></li>
<li><a href="https://devops.com/fast-moving-shai-hulud-attack-infects-npm-packages-with-2-billion-monthly-downloads/">Fast-Moving Shai-Hulud Attack Infects npm Packages with 2 ...</a></li>
<li><a href="https://gbhackers.com/shai-hulud-supply-chain-attack-compromises-keyv/">Shai-Hulud Supply Chain Attack Compromises Keyv and Hundreds ...</a></li>

</ul>
</details>

**Tags**: `#supply-chain-attack`, `#npm`, `#security`, `#open-source`, `#dependency-management`

---

<a id="item-tech-news-3"></a>
### [MiniMax-H3 MLX port brings local omni-modal video generation to Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax released MiniMax-H3, described as a general-purpose, omni-modal generative system that accepts text, images, audio, and video, and can generate up to 15-second video clips with audio included. Simon Willison highlights PipeNetwork/minimax-h3-mlx, a Python package that ports MiniMax-H3 to MLX for running on Apple Silicon. Willison successfully ran the model on an M5 Max MacBook Pro by downloading roughly 115 GB of model files and using the provided generation script, with video generation taking just under 45 minutes for a single prompt. In his test, the generated video for the prompt &quot;a rainbow colored skunk leaps over a mossy log in a supermarket&quot; was impressive, but the audio was speech-like and poor because he did not follow the prompting guide&\#x27;s guidance for audio. The repository provides concrete installation and generation commands using uv, huggingface\_hub, and the scripts/generate.py entry point.

rss · Simon Willison · Aug 4, 19:10

**「Background」** MiniMax-H3 is a general-purpose omni-modal generative model released by MiniMax that can jointly understand and generate across text, images, video, and audio, including 15-second 2K video clips with native stereo audio. This Python package from PipeNetwork ports the model to MLX, Apple&\#x27;s machine learning framework, so it can run locally on Apple Silicon hardware. The source post demonstrates running it on an M5 Max MacBook Pro with an 8-bit quantized MLX version of the model.

**「Impact」** Apple Silicon users can now run MiniMax-H3 locally for text-, image-, audio-, and video-conditioned video generation, but the practical barriers are significant: roughly 115 GB of downloads, near-45-minute generation times per clip on high-end hardware, and audio quality that depends heavily on following the vendor&\#x27;s prompt-writing guidance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/MiniMax-H3 · Hugging Face</a></li>
<li><a href="https://www.marktechpost.com/2026/08/01/minimax-releases-minimax-h3-an-omni-modal-video-model-that-generates-15-second-2k-clips-with-native-stereo-audio/">MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio - MarkTechPost</a></li>

</ul>
</details>

**Tags**: `#omni-modal`, `#MLX`, `#MiniMax`, `#video generation`, `#Apple Silicon`

---

<a id="item-tech-news-4"></a>
### [US drafts ban on Chinese optical modules for AI data centers](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

Reuters reports, citing four sources, that the Trump administration is drafting a ban on imports of new Chinese data center components, with a focus on optical modules, and that the FCC is advancing the measure with hopes of issuing it this year to protect infrastructure underpinning the AI boom. Officials say the ban is intended to prevent China from stealing data, implanting malware, or disrupting services, but sources caution it could still be modified or shelved. China&\#x27;s embassy in Washington said it will take all necessary measures against actions that harm China&\#x27;s interests. If enacted, the ban could hit global optical module leader Zhongji Innolight, which holds about 27% of the market. The FCC has previously imposed similar import restrictions on Chinese drones, routers, robots, and inverters.

telegram · zaihuapd · Aug 4, 11:29

**「Background」** Optical modules \(also called optical transceivers\) are key components in data center networks, converting electrical signals to optical signals for high-speed communication, especially in AI infrastructure. The U.S. Federal Communications Commission \(FCC\) has previously imposed import restrictions on Chinese-made drones, routers, robots, and inverters, and is now reportedly considering a similar ban on new Chinese optical modules and data center devices. While the draft is still subject to modification or shelving, U.S. cloud providers such as AWS might need to turn to alternative suppliers like Coherent and Lumentum, potentially raising costs and prompting pre-ban stockpiling.

**「Impact」** If enacted, the reported ban would most directly hurt China&\#x27;s Zhongji Innolight, which holds roughly 27% of the global data-center transceiver market and earns over 90% of its revenue outside China, while U.S. rivals Coherent and Lumentum stand to gain. The company was also added to the Pentagon&\#x27;s Chinese military-linked companies list in June, adding to regulatory pressure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/04/fcc-ban-china-datacenter-devices">Trump administration reportedly drafting ban on Chinese datacenter...</a></li>
<li><a href="https://www.gate.com/news/detail/fcc-drafts-ban-on-chinese-data-center-optical-modules-xinyuan-faces-27-23200496">FCC Drafts Ban on Chinese Data Center Optical Modules ; Xinyuan...</a></li>
<li><a href="https://www.networkworld.com/article/4205228/with-fcc-ban-on-new-chinese-made-optical-transceivers-for-dcs-likely-it-may-be-time-to-stock-up.html">With FCC ban on new Chinese -made optical ... | Network World</a></li>
<li><a href="https://wccftech.com/the-fcc-mulls-banning-china-sourced-optical-transceivers-threatening-innolights-27-global-market-share-as-coherent-and-lumentum-prepare-to-pounce/">The FCC Mulls Banning China-Sourced Optical Transceivers ...</a></li>
<li><a href="https://aiweekly.co/alerts/fcc-drafts-import-ban-on-chinese-data-center-transceivers">FCC Drafts Import Ban on Chinese Data-Center Transceivers</a></li>
<li><a href="https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/">Trump administration drafting ban on Chinese data center ...</a></li>

</ul>
</details>

**Tags**: `#US-China tech policy`, `#optical modules`, `#AI infrastructure`, `#hardware supply chain`, `#data centers`

---

<a id="item-tech-news-5"></a>
### [China Issues First Mandatory L3/L4 Autonomous Driving Standard, Effective July 2027](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

China&\#x27;s Ministry of Industry and Information Technology has released the national mandatory standard GB 44721-2026, &quot;Safety Requirements for Autonomous Driving Systems of Intelligent Connected Vehicles,&quot; the country&\#x27;s first compulsory standard for L3 conditionally and L4 highly automated driving systems. It will take effect on July 1, 2027, and applies to M-class passenger and N-class cargo vehicles equipped with L3/L4 systems, excluding automatic parking systems. The standard upgrades the 2024 recommended national standard to a binding requirement, establishing safety requirements across four dimensions: enterprise full-lifecycle safety assurance, system dynamic driving capability, human-machine interaction and user notification, and multi-dimensional testing. It requires that autonomous driving systems achieve at least the safety level of a competent and attentive human driver.

telegram · zaihuapd · Aug 4, 13:06

**「Background」** L3 and L4 are levels of driving automation defined by SAE: L3 lets the driver hand over all driving tasks under certain conditions but must remain able to take back control, while L4 can operate without driver intervention within its operational design domain. The new rule replaces a voluntary 2024 recommended national standard with a mandatory one, making compliance a legal requirement for vehicles sold in China.

**「Impact」** The mandatory standard will bind automakers, suppliers, and testing organizations to formally verify L3/L4 safety performance before deployment in China, with all affected M and N class vehicles required to meet the specified safety level by July 2027.

**Tags**: `#autonomous-driving`, `#regulations`, `#China`, `#standards`, `#L3-L4`

---

<a id="item-tech-news-6"></a>
### [A Custom Color Space for Generating Diverse Skin Tones](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

The author built and shared a color picker and procedural generation algorithm based on a custom color space designed to make it easier to choose plausible yet diverse skin tones for digital art and game development. The page includes interactive JavaScript demos and detailed explanations of the equations and space properties, plus a Future Work section. The author acknowledges the methodology is &\#x27;a bit shaky&\#x27; but reports the result has been helpful in their own projects. The work is relevant to procedural character generation and inclusive color palettes.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**「Background」** The tool introduces a custom color space specifically designed to make it easier to generate and pick diverse but plausible skin tones for digital art and game development. Typical RGB or HSV color pickers do not naturally separate skin-tone variations in an intuitive way, which is why the author developed a dedicated space with a procedural generation algorithm. The project&\#x27;s stated goal is to build inclusive color tools for contexts such as character creators or digital art.

**「Impact」** Digital artists and game developers can now use the included algorithm and demos to generate diverse skin tones without manual palette selection, though the author recommends treating the methodology as exploratory because it is based on hand-fitted functions rather than a formal perceptual model.

**「Community Discussion」** Commenters praised the visual presentation and the hand-fitted function approach, while also noting that skin color modeling is complex and that some generated samples appear green, blue, or purple. Several referenced complementary data such as Pantone Skin Tones and The Pudding&\#x27;s foundation shade mapping to validate the resulting color crescent.

<details><summary>References</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>

</ul>
</details>

**Tags**: `#color-science`, `#procedural-generation`, `#digital-art`, `#game-development`, `#javascript`

---

<a id="item-tech-news-7"></a>
### [Waymo Opens Driverless Ride-Hailing to Everyone in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo has opened its autonomous ride-hailing service to all users in Dallas, expanding its driverless operations to one of the top five US metroplexes by population. The service is now widely available there without a waitlist, adding Dallas to Waymo&\#x27;s roster of public driverless cities. The announcement marks another step in the commercialization of Level 4 autonomous vehicle technology in a market known for low density, heavy sprawl, and limited public transit. Specific details such as service area boundaries, fleet size, pricing, and any initial operational restrictions were not included in the available item.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**「Background」** Waymo is Alphabet&\#x27;s self-driving car company, operating commercial robotaxi services in cities including Phoenix, San Francisco, Los Angeles, Atlanta, Austin, and Miami. On August 4, 2026, Waymo announced that its Dallas service is now open to all users, removing the waitlist for the fully autonomous ride-hailing service. This expansion is part of Waymo&\#x27;s broader push to scale its driverless technology across the United States and internationally.

**「Impact」** Dallas-area residents and visitors can now directly use Waymo&\#x27;s driverless cars, gaining a new mobility option in a car-centric region with few public transit alternatives.

**「Community Discussion」** Commenters generally praised Waymo&\#x27;s driving behavior and predictability, with one Los Angeles-area resident reporting far fewer incidents than human drivers, while another raised economic concerns about money flowing out of local communities instead of to local drivers. A commercial real estate professional argued driverless fleets could serve as an effective affordable housing policy, and a Dallas–Fort Worth resident welcomed the addition as a positive change for the low-density metroplex.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Self-Driving_Car_Project">Waymo - Wikipedia</a></li>
<li><a href="https://waymo.com/blog/shorts/dallas-open-to-all/">August 4, 2026 - From the road - Waymo</a></li>
<li><a href="https://techcrunch.com/2026/08/04/waymo-opens-up-robotaxi-service-in-dallas-to-everyone/">Waymo opens up robotaxi service in Dallas to everyone | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#Waymo`, `#Dallas`, `#transportation`, `#AI-deployment`

---

<a id="item-tech-news-8"></a>
### [DeepSeek V4 Flash Runs on a Single AMD MI300X at 150+ Tokens/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

Ryan Zhou&\#x27;s GitHub project demonstrates running DeepSeek V4 Flash on a single AMD MI300X with fast inference, using native MXFP4 quantization and the GPU&\#x27;s large HBM capacity to exceed 150 tokens per second. The practical configuration reduces the context window from DeepSeek V4 Flash&\#x27;s full 1M-token support to 256k tokens, a tradeoff that makes single-card execution feasible. The project builds on earlier work that targeted two MI300X cards and is intended to make high-performance local inference of this model viable on AMD hardware.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**「Background」** DeepSeek-V4-Flash-0731 is an open-weights mixture-of-experts model whose official checkpoint is quantization-aware-trained: the routed experts, about 96% of the model, are stored natively in MXFP4 with the rest in FP8/BF16, so inference can load it as shipped without additional weight quantization or offload \(tool-1-1, tool-1-3\). The AMD MI300X accelerator offers a large HBM capacity that makes single-device serving feasible, but it is an OAM module rather than a standard PCIe card; a PCIe alternative such as the MI350P has 144GB and is still expected to fit the model. Prior work demonstrated this model on two MI300X modules, while this single-device project trades the original 1M-token context window for 256k tokens to stay within memory limits \(tool-1-2\).

**「Impact」** For AI teams running DeepSeek V4 Flash, this lowers the hardware requirement to a single MI300X while delivering over 150 tokens per second, but they must accept a 256k-token context instead of the full 1M.

**「Community Discussion」** Commenters largely welcomed the result and the MI300X&\#x27;s high HBM capacity, and they discussed the 150+ tokens/s throughput. However, they flagged that a single MI300X is generally not sold separately \(often only in ~€250K eight-card boxes\), that the 1M-to-256k context reduction is the main sacrifice, and that alternatives such as DwarfStar or the PCIe MI350P \(144GB\) may also run the model.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/deepseek-v4-flash-mi300x · GitHub</a></li>
<li><a href="https://fergusfinn.com/blog/deepseek-v4-flash-mi300x/">Bringing up DeepSeek-V4-Flash on AMD MI300X - Fergus Finn</a></li>
<li><a href="https://unsloth.ai/docs/models/deepseek-v4">DeepSeek-V4: How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#amd-mi300x`, `#llm-inference`, `#quantization`, `#moE`

---

<a id="item-tech-news-9"></a>
### [Oxide Computer raises $445M in new funding round](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 7.0/10

Oxide Computer has raised $445 million in a new funding round, according to a SEC Form D filing. The round, described by community members as a Series D, follows earlier rounds of $44 million \(Series A\), $100 million \(Series B\), and $200 million \(Series C\). The funding indicates strong investor confidence in the company&\#x27;s hardware and cloud computing efforts, though the filing itself provides limited technical or product details.

hackernews · depr · Aug 4, 20:13 · [Discussion](https://news.ycombinator.com/item?id=49174407)

**「Background」** Oxide Computer Company is a hardware startup building rack-scale cloud compute systems, essentially offering on-premise cloud infrastructure. The company has previously raised a $44 million Series A in 2023, a $100 million Series B in 2025, and a $200 million Series C in 2026, according to community-supplied blog posts and a Data Center Dynamics report. This new $445 million round, reported via SEC Form D, follows those earlier financing milestones and signals continued growth for the company.

**「Community Discussion」** Commenters celebrate Oxide&\#x27;s funding momentum and enthusiasm for its product concept, with some expressing hope that the company continues to succeed. However, questions remain about whether Oxide has actually shipped hardware in volume, and one potential customer reports filling out a sales form and never receiving a response while spending $900,000 per year on AWS.

<details><summary>References</summary>
<ul>
<li><a href="https://modernorange.io/item/49174407">Oxide Computer raises $ 445 M ( SEC Form D ) | Modern Orange</a></li>
<li><a href="https://www.datacenterdynamics.com/en/news/oxide-computer-company-secures-200m-in-funding/">Oxide Computer Company secures $200m in funding - DCD</a></li>

</ul>
</details>

**Tags**: `#funding`, `#hardware`, `#cloud computing`, `#tech industry`

---

<a id="item-tech-news-10"></a>
### [Huawei scientist warns Nvidia chip scaling will hit physical limits](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 7.0/10

Huawei Chief Semiconductor Scientist Liao Heng warned in a rare four-hour public interview in late July that chip giants such as Nvidia, which scale by adding more compute chips and high-bandwidth memory, will eventually hit physical limits, and that crossing those limits could trigger an avalanche-like breakdown. He also laid out Huawei&\#x27;s alternative path, described as Tay&\#x27;s Law or Tao&\#x27;s Law, and said the first phone chip using the LogicFolding technology framework will appear later this year. Liao further asserted that the U.S. and Chinese semiconductor industries are splitting into two independent ecosystems, requiring each side to build complete manufacturing and supply capabilities to survive.

telegram · zaihuapd · Aug 4, 08:04

**「Background」** Conventional chip progress has long followed the approach of shrinking transistors on a flat die so more compute fits in the same area. Huawei proposes an alternative scaling law, the τ \(Tao\) law, built around a 3D architecture called LogicFolding that rethinks chip layout instead of relying on ever-smaller lithography. Huawei says its first smartphone chip using this LogicFolding framework is scheduled to appear later this year, while the company publicly warns that approaches such as Nvidia&\#x27;s—adding ever more compute silicon and high-bandwidth memory—will eventually hit physical limits.

**「Impact」** Huawei&\#x27;s stated plan to ship its first LogicFolding-based phone chip later this year gives the industry a concrete alternative to watch as Nvidia-style scaling runs into physical constraints, although its real impact will depend on actual delivery and performance evidence.

<details><summary>References</summary>
<ul>
<li><a href="https://csdnnews.blog.csdn.net/article/details/162423752">超越炒作：科普 华 为 LogicFolding 芯 片 背后残酷的数学与 物 理 -CSDN...</a></li>
<li><a href="https://www.pcpop.com/article/6938810.shtml">晶体管密度暴涨55%！ 华 为 LogicFolding 架构突破制程枷锁-泡泡网</a></li>
<li><a href="https://laoyaoba.com/n/1076242">华 为 首席科学家警告：英伟达等巨头即将面临 芯 片 性能瓶颈</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#chip scaling`, `#Huawei`, `#NVIDIA`, `#AI hardware`

---

<a id="item-tech-news-11"></a>
### [Cloudflare Ditches Third-Party Security Tools for $58/Month AI Bounty Triage](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare has largely replaced third-party security tools with in-house applications and 200+ autonomous security agents, according to Chief Security Officer Grant Bourzikas at a recent Sydney event. The company automates vulnerability bounty triage with Anthropic&\#x27;s Claude Sonnet, spending only $58/month to deduplicate and assess reports, versus roughly $200,000/month for the same workload on the specialized Mythos security model. Bourzikas cautioned other organizations not to copy the approach, emphasizing that Cloudflare has rare in-house security software engineering capabilities. Chief Strategy Officer Stephanie Cohen added that AI will fundamentally reshape vendor-customer relationships, tied the company&\#x27;s 1,100-person layoffs to AI-driven automation, and outlined plans to serve as a micro-payment intermediary between AI companies and publishers for content access.

telegram · zaihuapd · Aug 4, 09:24

**「Background」** In bug bounty programs, triage means deduplicating and evaluating incoming vulnerability reports to decide whether they warrant attention. Anthropic&\#x27;s Claude Sonnet is a general-purpose large language model, while Claude Mythos is a specialized model designed to fix vulnerabilities in software and includes safety variants such as Claude Fable 5 with extra safeguards. Cloudflare&\#x27;s public comparison between using Claude Sonnet for this triage versus a security-specialized model like Mythos highlights the significant cost difference between general-purpose and specialized AI systems.

**「Impact」** Cloudflare&\#x27;s public move — replacing most third-party security tools with 200+ in-house AI agents running on Claude Sonnet for about $58/month — is a concrete signal that AI-native security operations are becoming practical, even if not yet broadly replicable. For Cloudflare customers, the immediate consequence is likely deeper integration of AI-driven security functions into products like Cloudflare One and the AI Cloud, though the company itself warns other enterprises not to try fully self-developed security software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos \ Anthropic</a></li>
<li><a href="https://www.techrepublic.com/article/cloudflare-one-new-ai-security-tools/">Cloudflare releases new AI security tools with Cloudflare One</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI security`, `#security automation`, `#Anthropic Claude`, `#vulnerability management`

---

<a id="item-tech-news-12"></a>
### [White House Reverses on Open-Source AI Restrictions Amid Valley Split](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

According to a New York Times report, the Trump administration has pivoted from considering restrictions on Chinese open-source AI models to focusing on boosting U.S. AI competitiveness, after strong opposition from Silicon Valley. White House Chief of Staff Susie Wiles and Treasury Secretary Scott Bessent had weighed sanctions, trade blacklists, and even banning U.S. companies from cooperating with Chinese firms, but the White House instead invited technology companies on August 4 to discuss a new framework that would require cybersecurity review before model release. The reported trigger was the Chinese open-source model Kimi matching some performance of OpenAI&\#x27;s top models. OpenAI and Anthropic pushed for restrictions on Chinese rivals on national security grounds, while Nvidia and Meta defended open ecosystems; Nvidia CEO Jensen Huang posted on X for the first time last month in defense of open source and helped form a safety coalition with more than 230 member companies.

telegram · zaihuapd · Aug 4, 15:22

**「Background」** Open-source AI models are released with publicly available weights, allowing anyone to download, modify, and deploy them, which has created tension between innovation and national security concerns. U.S. officials have debated whether Chinese open-source models such as Kimi pose risks that require trade restrictions, while American tech companies are divided over whether limiting open ecosystems would undermine U.S. leadership or leave security vulnerabilities unaddressed.

**「Impact」** The reported policy shift could ease near-term restrictions on U.S. cooperation with Chinese AI developers, but the proposed pre-release cybersecurity review framework may still impose new compliance costs on both proprietary and open-source model builders.

**Tags**: `#AI policy`, `#open-source AI`, `#regulation`, `#Silicon Valley`, `#national security`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Caterpillar and Palantir Lead Premarket Moves After Strong Earnings](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-premarket-mcd-cat-pltr-mrk.html) ⭐️ 8.0/10

In premarket trading, Caterpillar and Palantir led earnings-driven moves after reporting second-quarter results that beat analyst estimates. Caterpillar earned an adjusted $8.17 per share on revenue of $20.54 billion, above the LSEG consensus of $6.20 per share and $19.34 billion, while Palantir shares rose 15% on a nearly 150% surge in U.S. commercial revenue.

rss · CNBC Finance · Aug 4, 11:42

**「Background」** These moves follow the release of second-quarter earnings by a broad set of companies, with adjusted per-share figures commonly compared against LSEG consensus expectations.

**Tags**: `#Earnings`, `#Stock Market`, `#Premarket Trading`, `#Corporate Results`, `#Technology Stocks`

---

<a id="item-finance-news-2"></a>
### [Google builds $200bn financing structure to deliver AI chips to Anthropic](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

A Financial Times investigation found Google has quietly built a roughly $200 billion Wall Street financing structure intended to deliver more than $150 billion of AI chips to Anthropic, with the first deals worth about $35 billion in hardware completed in June.

telegram · zaihuapd · Aug 4, 10:52

**「Background」** Anthropic, an AI startup, has no credit rating, so the financing is structured to spread risk. Google and Anthropic have a longstanding partnership; in April 2026, the companies confirmed Google plans to invest up to $40 billion in Anthropic.

**「Impact」** The financing model lets Google and Anthropic avoid carrying hundreds of billions of dollars of AI hardware on their own balance sheets, shifting that exposure to financial firms and chip suppliers that participate in the deals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/04/24/google-to-invest-up-to-40-billion-in-anthropic-as-search-giant-spreads-its-ai-bets.html">Google to invest up to $40 billion in Anthropic as search ...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#corporate finance`, `#Wall Street`

---

<a id="item-finance-news-3"></a>
### [Procter &amp; Gamble to Acquire Thorne for $3.8 Billion](https://finance.yahoo.com/healthcare/articles/procter-gamble-pg-agrees-buy-221007357.html) ⭐️ 8.0/10

Procter &amp; Gamble has agreed to acquire health and wellness company Thorne for $3.8 billion. The acquisition price was disclosed as part of the agreement, though no other deal terms were provided.

openbb · PG · Aug 4, 22:10

**「Background」** Thorne makes dietary supplements and is being acquired from private equity firm L Catterton. P&amp;G already sells Metamucil, Align Probiotic, and New Chapter, so the deal adds to its existing supplement portfolio.

**「Impact」** The acquisition adds Thorne&\#x27;s wellness and supplement products to P&amp;G&\#x27;s personal health care portfolio, giving P&amp;G a stronger position in the premium wellness market.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/procter-gamble-acquiring-thorne-supplements-3-8-billion-080426">P&amp;G to acquire supplement brand Thorne for $ 3 . 8 billion</a></li>
<li><a href="https://www.axios.com/pro/merger-deals/2026/08/04/procter-gamble-thorne-3b">Procter &amp; Gamble buying Thorne for $ 3 . 8 billion</a></li>
<li><a href="https://www.thorne.com/press-releases/thorne-enters-definitive-agreement-to-be-acquired-by-procter-gamble">Thorne Enters into Definitive Agreement to Be Acquired by ...</a></li>
<li><a href="https://wwd.com/beauty-industry-news/wellness/procter-gamble-acquire-thorne-personal-health-care-1239093305/">Procter &amp; Gamble Acquires Thorne for $3.8 Billion - WWD</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#Consumer Goods`, `#Healthcare`, `#Procter &amp; Gamble`, `#Thorne`

---

<a id="item-finance-news-4"></a>
### [BP profit more than doubles on Middle East conflict](https://finance.yahoo.com/energy/articles/bp-profit-more-doubles-middle-093317262.html) ⭐️ 8.0/10

BP reported that its profit more than doubled, driven by higher oil prices related to the Middle East conflict.

openbb · BRK-B · Aug 4, 17:18

**「Background」** The current results follow a first-quarter profit of $3.2bn \(£2.4bn\), which BP said was helped by an &\#x27;exceptional&\#x27; performance in its oil trading business after the Middle East conflict broke out.

**「Impact」** Higher oil prices from the Middle East conflict are projected to spill over into natural gas and fertilizer costs, affecting households and businesses through higher energy and food prices, and could strain countries that rely on energy imports.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/c2eveyvgn9no">BP profits more than double as Iran war sends oil prices higher</a></li>
<li><a href="https://www.worldbank.org/en/news/press-release/2026/04/28/commodity-markets-outlook-april-2026-press-release">Middle East War to Spark Biggest Energy Price Surge in Four Years</a></li>
<li><a href="https://www.imf.org/en/blogs/articles/2026/03/30/how-the-war-in-the-middle-east-is-affecting-energy-trade-and-finance">How the War in the Middle East Is Affecting Energy, Trade ...</a></li>

</ul>
</details>

**Tags**: `#BP`, `#earnings`, `#oil prices`, `#Middle East conflict`, `#energy sector`

---

<a id="item-finance-news-5"></a>
### [Goldman Sachs Equities Revenue Jumps 72% to Record $7.42 Billion in Q2](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 7.0/10

Goldman Sachs reported a 72% surge in second-quarter equities trading revenue to a record $7.42 billion, putting the bank on pace for a record trading year. Investment banking revenue rose 55% to $3.4 billion, including fees from SpaceX&\#x27;s IPO and Alphabet&\#x27;s $85 billion equity raise.

rss · CNBC Finance · Aug 4, 19:38

**「Background」** Goldman&\#x27;s equities business sits inside its largest division, Global Banking &amp; Markets, which brought in $15.5 billion in revenue last quarter, over 75% of the bank&\#x27;s total, after a strategy shift to cross-sell equities services to banking and wealth clients.

**Tags**: `#Goldman Sachs`, `#equities trading`, `#investment banking`, `#earnings`, `#trading revenue`

---

<a id="item-finance-news-6"></a>
### [China Postal Regulator Opens Investigation into STO Express](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 7.0/10

China’s State Post Bureau announced on August 4 that it has opened a formal investigation into STO Express, saying the company failed to enforce unified safety management for businesses using its brand. The regulator said that since 2026, operations using the STO Express trademark, name, and waybills have experienced multiple production safety accidents and repeated discoveries of safety hazards.

telegram · zaihuapd · Aug 4, 12:07

**「Background」** On August 4, China&\#x27;s State Post Bureau announced it had opened an investigation into STO Express after saying businesses using the STO brand had multiple production safety accidents and found hidden hazards this year; the regulator said STO Express had failed to exercise unified safety management over these businesses.

**「Impact」** This is the second major courier investigation in 2026, after J&amp;T Express was probed in June, signaling tighter regulatory scrutiny of franchise-based delivery networks. STO says it will immediately rectify problems and fully cooperate, but could face fines or corrective orders if safety-management violations are confirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://news.cctv.com/2026/08/04/ARTIxQDXIvTHcdHsMaU2kzU0260804.shtml">国家邮政局依法对申通快递有限公司立案调查_新闻频道_央视网 (cctv.co...</a></li>
<li><a href="https://www.guancha.cn/politics/2026_08_04_826154.shtml">国家邮政局依法对申通快递有限公司立案调查</a></li>
<li><a href="https://www.chinanews.com.cn/cj/2026/08-04/10671916.shtml">国家邮政局依法对申通快递有限公司立案调查-中新网</a></li>
<li><a href="https://news.qq.com/rain/a/20260804A0DLI600">国家邮政局依法对申通快递立案调查 申通回应：立行立改、全力配合各项...</a></li>
<li><a href="https://finance.sina.com.cn/stock/s/2026-08-04/doc-inimeknx4006837.shtml">申通快递被立案调查，加盟制度弊病集中爆发，被指总部收钱、网点担责...</a></li>

</ul>
</details>

**Tags**: `#regulatory investigation`, `#STO Express`, `#logistics industry`, `#safety management`, `#China postal regulator`

---

<a id="item-finance-news-7"></a>
### [NVIDIA Invests in Secretive AI Lab Chasing Superintelligence](https://finance.yahoo.com/technology/ai/articles/secretive-ai-lab-chasing-superintelligence-180821241.html) ⭐️ 7.0/10

NVIDIA announced a major investment in a secretive AI lab focused on superintelligence. The size and terms of the investment were not disclosed.

openbb · NVDA · Aug 4, 18:08

**「Background」** Safe Superintelligence is an AI lab co-founded by former OpenAI chief scientist Ilya Sutskever; Nvidia reportedly plans to invest $5 billion in it as part of a long-term collaboration, according to a person briefed on the deal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.resultsense.com/news/2026-07-28-nvidia-safe-superintelligence-investment/">Nvidia to put £3.8bn into Sutskever&#x27;s Safe Superintelligence</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#Artificial Intelligence`, `#Investment`, `#Superintelligence`, `#AI Lab`

---

<a id="item-finance-news-8"></a>
### [AMD Beats Q2 Earnings and Reports Large Capital Expenditure Program](https://finance.yahoo.com/video/amd-beats-q2-earnings-estimates-202804476.html) ⭐️ 7.0/10

AMD beat analyst estimates for Q2 earnings and reported a large capital expenditure \(capex\) program, or spending on long-term assets such as factories and equipment.

openbb · NVDA · Aug 4, 20:28

**「Background」** On August 5, 2025, AMD reported second-quarter results that beat analyst estimates, with revenue of $11.5 billion \(up about 50% year over year\) and diluted earnings per share of $0.54, but also disclosed capital expenditures of $808 million in the quarter, far above the estimated $298 million and up roughly 108% quarter over quarter.

**「Impact」** AMD&\#x27;s large capital expenditure program signals a major investment push at a time when the global semiconductor market is forecast to exceed $1 trillion in 2026, driven by AI infrastructure; this could affect AMD&\#x27;s future production capacity and competitive positioning.

<details><summary>References</summary>
<ul>
<li><a href="https://ir.amd.com/news-events/press-releases/detail/1257/amd-reports-second-quarter-2025-financial-results">AMD Reports Second Quarter 2025 Financial Results :: Advanced Micro Devices, Inc. (AMD)</a></li>
<li><a href="https://finance.yahoo.com/technology/article/amd-tops-q2-earnings-estimates-and-provides-strong-outlook-but-leaves-investors-unimpressed-110000620.html">AMD tops Q2 earnings estimates and provides strong outlook, but leaves investors unimpressed</a></li>
<li><a href="https://breakingthenews.net/Article/AMD-posts-Q2-revenue-of-dollar11.5B-up-50/66850343">AMD posts Q2 revenue of $11.5B, but capex soars</a></li>
<li><a href="https://stockdividendscreener.com/technology/semiconductor/amd/amd-capital-expenditures/">AMD Capital Expenditures vs Operating Cash Flow</a></li>
<li><a href="https://www.idc.com/resource-center/blog/semiconductor-market-to-surge-past-the-trillion-dollar-threshold-ai-infrastructure-drives-market-growth/">IDC - Semiconductor Market Forecast 2026: The AI Supercycle ...</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#Earnings`, `#Capital Expenditure`, `#Semiconductors`, `#Q2`

---

<a id="item-finance-news-9"></a>
### [Chip Investors Remain Unsatisfied Despite Big Profits](https://www.wsj.com/finance/stocks/even-big-profits-arent-enough-to-keep-chip-investors-happy-36acfc66?siteid=yhoof2&amp;yptr=yahoo) ⭐️ 7.0/10

A Wall Street Journal article reports that semiconductor companies have posted large profits, but investors are still unhappy, reflecting unusually high expectations in the sector.

openbb · NVDA · Aug 4, 21:23

**「Background」** Nvidia, whose stock is up roughly 200% this year, has been a key driver of the AI-chip boom, but its shares recently fell sharply after Chinese startup DeepSeek spooked markets, and its new inference chip has been seen as expensive relative to its performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cityam.com/nvidia-sinks-as-chinese-ai-startup-deepseek-spooks-global-markets/">Nvidia tanks as Chinese AI startup Deepseek spooks global markets</a></li>
<li><a href="https://www.tastylive.com/news-insights/nvidia-earnings-preview-up-over-200-this-year">Nvidia (NVDA) Q3 Earnings Preview: 8% Stock Move... | tastylive</a></li>
<li><a href="https://investingnews.com/nvidia-weak-demand-new-chip/">NVIDIA Facing Weak Demand for New Chip as Chinese Firms Turn to...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Nvidia`, `#earnings`, `#investor sentiment`, `#stock market`

---

<a id="item-finance-news-10"></a>
### [McDonald&\#x27;s Earnings Beat Comes With Warning Sign](https://finance.yahoo.com/markets/stocks/articles/mcdonalds-earnings-win-comes-warning-200519881.html) ⭐️ 7.0/10

McDonald&\#x27;s reported an earnings beat for the quarter, but the report also included a warning sign about future performance.

openbb · PG · Aug 4, 20:05

**「Background」** McDonald’s had just posted a strong second-quarter profit that beat expectations, but sales in the U.S. continue to be affected by Americans’ cautious spending, and the company named a new head of its U.S. market.

**「Impact」** The warning matters most for investors and economists who watch McDonald’s as a bellwether for consumer spending, since the company has said lower-income households are spending less amid inflation.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/mcdonalds-profit-economy-9b9ef2da69dc72451928176f17051126">McDonald&#x27;s reports strong profit and names new head for US ...</a></li>
<li><a href="https://www.nytimes.com/2026/08/04/business/mcdonalds-earnings-consumers-inflation.html">McDonald’s U.S. Sales Slow as Diners Spend More Cautiously</a></li>
<li><a href="https://www.cnbc.com/2026/02/11/mcdonalds-mcd-q4-2025-earnings.html">McDonald&#x27;s (MCD) Q4 2025 earnings - CNBC</a></li>
<li><a href="https://fortune.com/article/mcdonalds-earnings-first-quarter-economic-uncertainty/">McDonald&#x27;s CEO warns the fast-food giant is &#x27;not immune&#x27; to ...</a></li>

</ul>
</details>

**Tags**: `#McDonald&\#x27;s`, `#earnings`, `#consumer spending`, `#outlook`, `#fast food`

---