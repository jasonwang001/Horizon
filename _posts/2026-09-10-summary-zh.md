---
layout: default
title: "Horizon Summary: 2026-09-10 (ZH)"
date: 2026-09-10
lang: zh
---

> 从 242 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [vLLM v0.29.0 发布：Model Runner V2 全面成为默认](#item-tech-news-1) ⭐️ 8.0/10
2. [Shopify 收购 Tailwind：开源商业模式受关注](#item-tech-news-2) ⭐️ 8.0/10
3. [GPT-6 Astra、循环 Transformer 与隐藏推理分析](#item-tech-news-3) ⭐️ 8.0/10
4. [利用 Google Ads 审核流程投放恶意软件的第一手记录](#item-tech-news-4) ⭐️ 8.0/10
5. [OpenAI 披露 GPT-6 Astra 思维链可监测性显著下降](#item-tech-news-5) ⭐️ 8.0/10
6. [IEEE Spectrum：自动驾驶汽车安全证据增加，社区讨论比较基准](#item-tech-news-6) ⭐️ 7.0/10
7. [美防部被指要求 OpenAI 降低军事任务拒绝率，双方否认](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [布伦特原油突破每桶 100 美元，霍尔木兹海峡运量骤降](#item-finance-news-1) ⭐️ 8.0/10
2. [欧洲负电价激增，欧盟承诺到 2028 年新增 30-35 吉瓦储能](#item-finance-news-2) ⭐️ 8.0/10
3. [美国制裁伊朗全部剩余航空公司，收紧其航空通道](#item-finance-news-3) ⭐️ 8.0/10
4. [谷歌在芬兰投资至少 130 亿欧元建 AI 基础设施，并签 22 年核电协议](#item-finance-news-4) ⭐️ 8.0/10
5. [英国央行行长警告：伊朗冲突或使英国通胀升破 4%](#item-finance-news-5) ⭐️ 8.0/10
6. [铜价创历史新高，而铜冶炼厂加工费降至零甚至负值](#item-finance-news-6) ⭐️ 8.0/10
7. [美联储维持利率不变，保留加息可能](#item-finance-news-7) ⭐️ 8.0/10
8. [阿达尼机场业务获约 10 亿美元融资，阿达尼企业股价上涨近 5%](#item-finance-news-8) ⭐️ 7.0/10
9. [中国电动车企转向人形机器人，小鹏为机器人业务融资 9 亿美元](#item-finance-news-9) ⭐️ 7.0/10
10. [分析质疑英国放弃净零可为每户年省 500 英镑的说法](#item-finance-news-10) ⭐️ 7.0/10
11. [白俄罗斯炼油厂借俄罗斯燃料短缺创十年最高盈利](#item-finance-news-11) ⭐️ 7.0/10
12. [乌干达推出新原油品级“珍珠甜油”，首次出口临近](#item-finance-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [vLLM v0.29.0 发布：Model Runner V2 全面成为默认](https://github.com/vllm-project/vllm/releases/tag/v0.29.0) ⭐️ 8.0/10

vLLM v0.29.0 发布，本版本包含 594 个提交，来自 277 位贡献者（其中 91 位是新贡献者）。最核心的变化是 Model Runner V2（MRV2）成为所有模型的默认实现（\#53183），完成了此前从 pooling 模型开始的迁移（\#48290）；MRV1 仍用于少数 ROCm 模型以及 MRV2 尚未支持的功能。MRV2 同时新增了用于 KV cache 自动定容的 CUDA graph 显存分析（\#53306）、把每步 logits 显存降低 1/TP 的 batch-sharded sampling（\#50465）、prompt embeds（\#42963）以及 extract\_hidden\_states 投机解码（\#49811）等能力。模型支持方面新增腾讯 770B/49B 激活的 MoE 模型 Hy4-preview（\#54160）、Qwen3.8-Flash-Next（\#53896）、GraniteSWA/GraniteMoeSWA（\#52706）、NemotronH\_Omni\_Reasoning\_V3（\#52929）和 Kimi K3 NVFP4 权重（\#53132），并带有 K3 Mamba 元数据单次 Triton 启动（6.6–7.6 倍 kernel 加速，\#52388）等性能优化。破坏性变更包括移除十个已弃用的模型架构（\#53608）、移除 PyAV 视频解码后端（\#54231）、弃用 \`python -m vllm.entrypoints.openai.api\_server\` 而改用 \`vllm serve\`（\#52131）；此外 FlashInfer all-reduce 在 TP CUDA group 上默认启用，可用 \`VLLM\_ALLREDUCE\_USE\_FLASHINFER=0\` 关闭（\#52998）。

github · khluu · 9月9日 08:54

**「背景」** vLLM 是一个面向大语言模型的高吞吐、内存高效的推理与服务引擎，采用 PagedAttention 和连续批处理等技术。Model Runner V2（MRV2）是对 vLLM 模型执行器的从底层重新实现，目标是更清晰、更模块化且更高效，并且不改变 API；其设计文档也指出 MRV2 当时尚未功能完备、未经过严格测试，仍有开放设计决策。v0.29.0 将原本从池化模型开始的 MRV2 推广为所有模型的默认执行路径，同时保留 MRV1 用于少量 ROCm 模型和 MRV2 尚未支持的功能。

**「影响」** 对 vLLM 用户而言，升级到 v0.29.0 后 Model Runner V2 成为所有模型的默认执行路径，可直接获得 CUDA 图显存分析用于 KV cache 自动定容、批量分片采样（每步 logits 显存降至 1/TP）等优化，但必须同步处理移除十个废弃模型架构、删除 PyAV 视频解码后端、弃用 \`python -m vllm.entrypoints.openai.api\_server\` 以及删除 \`VLLM\_TEST\_FORCE\_FP8\_MARLIN\`、\`VLLM\_ROCM\_USE\_AITER\_FP4\_ASM\_GEMM\` 等破坏性变更。少数 ROCm 模型以及 MRV2 尚未覆盖的特性仍走 MRV1，且 MRV2 官方文档自述尚未完全功能完备，因此升级前需按自身模型与特性组合做验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory ... Model Runner V2 Design Document - vLLM Model Runner V2: A Modular and Faster Core for vLLM vllm-project-vllm-inference/docs/design/model_runner_v2.md at ... V1 Engine &amp; Model Runner V2 (MRV2) | vllm-project/vllm ...</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open source`, `#model serving`, `#performance optimization`

---

<a id="item-tech-news-2"></a>
### [Shopify 收购 Tailwind：开源商业模式受关注](https://tailwindcss.com/blog/tailwind-is-joining-shopify) ⭐️ 8.0/10

Shopify 已收购 Tailwind，这一消息在 Hacker News 上引发 870 分、348 条评论的讨论。现有材料没有披露交易金额、具体条款，以及 Tailwind CSS 开源项目的治理和许可安排。社区讨论主要围绕 AI 对 Tailwind Labs 商业模式的冲击、开源加商业双轨制的前景，以及新项目是否仍有必要采用 Tailwind。评论中引用的二手 PR 摘录称，Tailwind Labs 约 75% 的工程团队成员被裁，文档流量较 2023 年初下降约 40%，但这些数字来自评论转述，需谨慎对待。

hackernews · EdwinHoksberg · 9月9日 13:27 · [社区讨论](https://news.ycombinator.com/item?id=49626190)

**「背景」** Tailwind CSS 是一个开源、采用“功能类优先”（utility-first）理念的 CSS 框架，允许开发者直接在 HTML 中编写样式，由加拿大的 Tailwind Labs 开发并维护。Shopify 是总部位于渥太华的加拿大电商与建站服务平台，此次收购 Tailwind Labs 旨在为 Tailwind CSS 提供稳定、长期的归属，并承诺其继续以 MIT 许可证开源。该交易于周三通过博客文章及社交媒体对外公布。

**「影响」** 对于依赖 Tailwind CSS 的开发者来说，Shopify 的收购意味着这个被广泛使用的开源框架及其维护团队短期内获得了存续保障，项目不至于因原公司经营困难而停摆。不过外部报道指出，AI 编码助手已使 Tailwind Labs 的收入大幅萎缩并导致工程团队大规模裁撤，因此其商业产品线、文档站点与后续维护节奏仍存在不确定性。

**「社区讨论」** 评论者一方面感谢 Tailwind 对 CSS 与设计实践的影响，并猜测 Shopify 看重的是团队与品牌；另一方面，simonw 引用一份二手 PR 摘录称 AI 已重创 Tailwind Labs 业务，pil0u 认为出售 UI 模板在当前环境下可能难以为继。jedberg 则指出，LLM 让“开源+商业”DevTools 公司更难存活，只有提供大规模托管等难以复制的服务才更有护城河；fg137 也质疑新项目是否还需要 Tailwind，而非使用带最新特性的原生 CSS。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seekingalpha.com/news/4641301-shopify-acquires-tailwind-labs">Shopify acquires Tailwind Labs (SHOP:NASDAQ) | Seeking Alpha</a></li>
<li><a href="https://www.tradingview.com/news/seekingalpha:72d53b6e5094b:0-shopify-acquires-tailwind-labs/">Shopify acquires Tailwind Labs — TradingView News</a></li>
<li><a href="https://betakit.com/tailwind-finds-stable-long-term-home-with-shopify-acquisition/">Tailwind finds “stable, long-term home” with Shopify acquisition | BetaKit</a></li>
<li><a href="https://byteiota.com/tailwind-labs-joins-shopify-what-developers-must-know/">Tailwind Labs Joins Shopify: What Developers Must Know | byteiota</a></li>
<li><a href="https://socket.dev/blog/tailwind-css-announces-layoffs">Tailwind CSS Announces 75% Layoffs as LLMs Reshape OSS Business Models | Socket</a></li>
<li><a href="https://devclass.com/2026/01/08/tailwind-labs-lays-off-75-percent-of-its-engineers-thanks-to-brutal-impact-of-ai/">Tailwind Labs lays off 75 percent of its engineers thanks to &#x27;brutal impact&#x27; of AI</a></li>

</ul>
</details>

**标签**: `#tailwind-css`, `#acquisitions`, `#open-source-business-models`, `#ai-impact-on-devtools`, `#web-development`

---

<a id="item-tech-news-3"></a>
### [GPT-6 Astra、循环 Transformer 与隐藏推理分析](https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and) ⭐️ 8.0/10

Sebastian Raschka 的技术分析文章讨论 GPT-6 Astra、循环 Transformer（looped transformers）与隐藏推理，并在 Hacker News 上引发专家讨论。文章和相关评论将《The Information》报道中所谓 GPT-6 Astra 使用的“recurrent depth”或“looped transformers”解释为并非全新神秘机制，而是与堆叠更多 Transformer 层类似，区别在于复用权重以降低 GPU 显存占用。关于隐藏推理，有评论者认为，若在推理时把整个 Transformer 循环作用于自身，并将中间推理轨迹反馈给模型而非直接输出，就按定义构成隐藏推理，但中间轨迹与最终输出轨迹在原则上仍可被提取。讨论还涉及思维链所需计算步骤的参考文献、通用 Transformer 的既有工作，以及 MSPAINT 计算机使用演示等实例。另有用户报告称 Astra 在周一表现惊人、周二之后感觉像 Sol，并担心生产力受影响；由于条目未附原文正文，具体技术主张无法从源内容独立核实。

hackernews · ModelForge · 9月9日 14:37 · [社区讨论](https://news.ycombinator.com/item?id=49627370)

**「背景」** 循环 Transformer（又称循环深度，recurrent depth）指在推理时反复复用同一组 Transformer 层权重，而不是像常规做法那样堆叠各不相同的层，由此在增加有效深度的同时节省显存。围绕 GPT-6 Astra 的讨论源自媒体报道称其采用了这种架构，而 Sebastian Raschka 等分析者指出，Astra（以及可预见的任何 LLM）仍是推理模型，即经过可验证奖励的强化学习（RLVR）训练并输出中间推理轨迹（思维链）。也正因如此，「隐藏推理」才成为争议焦点：当模型把中间输出重新喂回自身而不外显时，这一推理过程对外部监控而言就变得不可见。

**「影响」** 对从事 AI 安全与思维链监控的研究者和团队而言，若 GPT-6 Astra 采用的循环（recurrent depth/looped transformer）推理不再对外输出可读的推理轨迹，标准的思维链监控将更难实施，相关治理风险随之上升；不过专家指出循环 Transformer 本质上是复用权重的多层堆叠，主要收益是节省显存，而非一种刻意隐藏推理的新技术。

**「社区讨论」** 评论区的共识倾向于认为循环 Transformer 不是神秘突破，而是以权重共享换取显存优势的架构选择；分歧主要在于它是否必然等同于隐藏推理，以及这种推理轨迹能否被完整监控。还有用户分享了 CoT 复杂度与通用 Transformer 的研究链接，并有人报告 Astra 模型行为在周一后发生变化的实际体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT - 6 Astra , Looped Transformers , and Hidden Reasoning</a></li>
<li><a href="https://www.hackaigc.com/blog/gpt-6-astra-everything-we-know-2026">GPT - 6 Astra : Everything We Know in 2026</a></li>
<li><a href="https://www.youtube.com/watch?v=XvmixEXPT3Q">GPT - 6 Astra .. full analysis.. - YouTube</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT-6 Astra, Looped Transformers, and Hidden Reasoning</a></li>
<li><a href="https://tech.yahoo.com/ai/chatgpt/articles/openai-astra-uses-hidden-reasoning-154630586.html">OpenAI’s Astra Uses Hidden Reasoning Loops: Experts Are Alarmed</a></li>
<li><a href="https://arxiv.org/html/2502.17416">Reasoning with Latent Thoughts: On the Power of Looped ...</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#transformers`, `#hidden reasoning`, `#AI research`, `#Hacker News`

---

<a id="item-tech-news-4"></a>
### [利用 Google Ads 审核流程投放恶意软件的第一手记录](https://xlii.space/eng/malicious-software-on-google-ads/) ⭐️ 8.0/10

一篇题为《How I advertise malicious software on Google Ads》的第一人称文章，记录了作者如何滥用 Google Ads 的审核流程来投放恶意软件。该文在 Hacker News 引发关于自动化平台审核与申诉机制的讨论，相关帖子获得 351 分、211 条评论。由于没有可用的正文内容，目前只能确认文章主题和社区反应，无法核验其具体技术手法、影响范围或 Google 的回应。对广告平台用户与更广泛的广告生态而言，该案例凸显了恶意软件借合法广告渠道触达用户、而自动化审核难以完全拦截的风险。

hackernews · xlii · 9月9日 11:43 · [社区讨论](https://news.ycombinator.com/item?id=49624856)

**「背景」** Google Ads 的广告政策明确禁止有意分发可能损害、或未经授权访问他人电脑、设备或网络的恶意软件（malware），并规定该要求同时适用于广告本身以及网站或应用所托管或链接的软件，无论这些软件是否通过 Google 广告网络推广（tool-1-3）。作为本文所述事件的背景，作者在首次尝试投放 Google Ads 广告、花费 500 美元后，其账户即因“恶意软件”被暂停（tool-1-1）。

**「影响」** 对 Google Ads 用户和依赖广告审核防线的平台生态而言，该案例表明一旦审核流程可被规避，恶意软件就可能通过广告触达用户，从而增加平台在人工复核、申诉与追责机制上的压力。

**「社区讨论」** 评论区批评 Google 等大公司用自动化系统取代申诉渠道：有人称 YouTube 广告几乎全是诈骗，另有用户分享向 Google Maps 提交新 Tesla Supercharger 信息却迅速被拒的经历，并建议大公司至少保留人工联系点和对封号等决定给出具体说明；也有人提醒，网站被入侵并托管跳转页面可能让审核判断更复杂。作者 xlii 在评论中更新称其账号已恢复，并感叹问题要靠 Hacker News 放大关注后才得到解决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xlii.space/eng/malicious-software-on-google-ads/">How I advertise malicious software on Google Ads</a></li>
<li><a href="https://support.google.com/adspolicy/answer/15939580?hl=en">Malicious Software - Advertising Policies Help</a></li>

</ul>
</details>

**标签**: `#ad-fraud`, `#google-ads`, `#malware-distribution`, `#platform-moderation`, `#security`

---

<a id="item-tech-news-5"></a>
### [OpenAI 披露 GPT-6 Astra 思维链可监测性显著下降](https://deploymentsafety.openai.com/gpt-6-astra) ⭐️ 8.0/10

OpenAI 披露，GPT-6 Astra 较前代模型出现“显著”的思维链（CoT）可监测性下降。首席科学家 Jakub Pachocki 称，依赖 CoT 监测的能力正“逐步减弱”，原因之一是模型越来越能控制自身推理过程，并能在更少甚至无需语言化推理的情况下完成更复杂任务。官方开发文档同时提醒，Astra 的代理间消息可能出现语法或空格错误。英国 AI Safety Institute 的外部评估还发现，Astra 的原始推理更加压缩，含义不清的短语有所增加。上述说法来自 Telegram 聚合频道，具体主张仍需以一手材料核实。

telegram · zaihuapd · 9月9日 09:45

**「背景」** 思维链（CoT）可监测性是指通过模型显式写出的推理轨迹来观察其意图与行为的能力；OpenAI 将保留并利用 CoT 监测列为其研究计划的核心目标。其安全概览称，GPT-6 Astra 的可监测性相对 GPT-5.6 Sol 有所下降。英国 AI 安全研究所的外部评估还发现，Astra 的原始推理更加压缩、含义不清的短语增多，并能在明显缺少扩展可见推理轨迹的情况下解决高难数学问题，其估计任务时间跨度达到 30.9 分钟，而 Sol 为 3.6 分钟。

**「影响」** 对依赖思维链监测进行安全评估的研究者与开发者而言，这一下降削弱了现有透明度工具的有效性，可能需转向其他可解释性与评估手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/safety-overview-gpt-6-astra/">Safety overview: GPT - 6 Astra | OpenAI</a></li>
<li><a href="https://www.remio.ai/post/gpt-6astra-leads-the-benchmarks-but-is-it-really-the-smartest-ai-model">GPT 6 Astra Leads the Benchmarks, but Is It Really the Smartest AI ...</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#思维链可监测性`, `#OpenAI`, `#可解释性`, `#模型评估`

---

<a id="item-tech-news-6"></a>
### [IEEE Spectrum：自动驾驶汽车安全证据增加，社区讨论比较基准](https://spectrum.ieee.org/are-self-driving-cars-safe) ⭐️ 7.0/10

IEEE Spectrum 一篇题为“Growing proof that autonomous cars save lives”的文章认为，越来越多证据显示自动驾驶汽车能够挽救生命；由于未提供全文，具体数据与结论细节无法核实。Hacker News 的讨论集中于如何比较自动驾驶与人类驾驶的事故和死亡率，有评论者指出 Waymo 选择与普通司机而非其取代的网约车司机对比，而后者严重事故更少，因此对比结果可能显得更有利。还有评论者称交通死亡数据高度偏斜，涉及未系安全带、超速、酒精以及行人/自行车骑行者等弱势道路使用者。另一些评论者主张把资源投向公共交通，并比较公交、轻轨等成熟出行方式的死亡率。讨论还延伸到保险经济：若自动驾驶事故更少，保险费率可能向自动驾驶倾斜，使人工驾驶变成更昂贵的偏好或“炫耀性”行为。

hackernews · bookofjoe · 9月9日 17:14 · [社区讨论](https://news.ycombinator.com/item?id=49629886)

**「背景」** 自动驾驶汽车的安全性通常靠与传统人类驾驶的对比来评估：IEEE Spectrum 汇总的研究显示，自动驾驶汽车的碰撞频率明显低于人类驾驶员，造成伤害也少得多，高级驾驶辅助系统（ADAS）的证据也被纳入同一讨论。随着 Waymo、Zoox 等无人驾驶车辆陆续进入旧金山、亚特兰大等城市，早期数据被认为表明它们可以作为网约车出行的一种安全选择。不过这类结论高度依赖比较基准的选择——是与全体平均驾驶员对比，还是与其实际替代的网约车司机对比，会直接影响数据呈现出的差距。

**「影响」** 对 Waymo 等自动驾驶运营商和保险公司而言，事故率比较基准和数据口径将直接影响监管接受度与保险定价；若自动驾驶确实更安全，人工驾驶的相对成本可能上升，但这一后果目前仍属基于讨论的推测。

**「社区讨论」** 讨论未就如何衡量自动驾驶安全性达成一致：有人质疑 Waymo 用普通司机而非网约车司机作基准，有人强调死亡数据受未系安全带、超速、酒精和弱势道路使用者比例影响，也有人主张优先投资公共交通。另有评论者从保险经济角度推测，自动驾驶若事故更少，保险费率变化可能使人工驾驶变成昂贵爱好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrum.ieee.org/are-self-driving-cars-safe">Are Self Driving Cars Safe as Early Data Suggests? - IEEE ...</a></li>
<li><a href="https://publichealth.jhu.edu/2026/the-safety-data-on-autonomous-vehicles">The Safety Data on Autonomous Vehicles | Johns Hopkins ...</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#road safety`, `#AI systems`, `#Waymo`, `#public transit`

---

<a id="item-tech-news-7"></a>
### [美防部被指要求 OpenAI 降低军事任务拒绝率，双方否认](https://theintercept.com/2026/09/08/pentagon-openai-military-contract/) ⭐️ 7.0/10

据 The Intercept 报道，最新泄露文件显示，美国国防部曾要求 OpenAI 向美国军方提供其人工智能技术的特殊版本，使其尽可能不频繁地拒绝军事指挥。文件称，寻求 OpenAI“最低拒绝率”的条款出现在合同更新版本“P00003”中，该版本扩展了去年夏天美国国防部与 OpenAI 的原订交易。但 OpenAI 和五角大楼否认同意这种“最低拒绝”语言，称泄露的“P00003”文件是草稿而非最终版本。OpenAI 发言人 Nate Evans 表示：“OpenAI 从未同意要求‘最低拒绝率’的合同语言。这种东西没有出现在我们执行的合同中。”这一争议凸显了军事 AI 合同中模型拒绝行为条款的敏感性，以及泄露草案与执行合同之间的关键差别。

telegram · zaihuapd · 9月9日 09:02

**「背景」** 背景上，OpenAI 与美国国防部/战争部（Department of War）在 2026 年公开过一份军事合作安排，涉及安全红线、法律保护以及 AI 系统在机密环境中的部署，该合作此前已因签署时机和伦理问题引发争议。所谓“拒绝率”通常指模型面对特定请求（如军事任务）时触发安全拒答的频率，而合同是否写入“最低拒绝率”要求正是此次泄露文件争议的核心。泄露的 P00003 版本被描述为对去年夏天原协议的扩展，但 OpenAI 和五角大楼称其只是草稿，并非已执行合同。

**「影响」** 该争议使 OpenAI 国防合约的实际条款成为外部审视焦点：泄露的 P00003 修改文本将“OpenAI 任务模型”定义为面向国家安全用例、“具有最低拒绝率”的模型，若该语言确实进入最终执行合同，将意味着相关军事部署中的模型被系统性要求减少对军事任务的拒答，并直接影响用户与开发者对其安全承诺的预期；但 OpenAI 与五角大楼均称该文件为草稿、执行合同中不含此类条款，最终文本仍有待澄清。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/315025/20260311/openai-pentagon-ai-controversy-military-deployment-public-backlash-ethics.htm">OpenAI Pentagon AI Controversy: Military Deployment, Public ...</a></li>
<li><a href="https://openai.com/index/our-agreement-with-the-department-of-war/">Our agreement with the Department of War - OpenAI</a></li>
<li><a href="https://theintercept.com/2026/09/08/pentagon-openai-military-contract/">The Pentagon Asked OpenAI for Artificial Intelligence ...</a></li>
<li><a href="https://www.unite.ai/openai-pentagon-contract-defines-mission-models-by-minimal-refusal-rates/">OpenAI Pentagon Contract Defines ‘Mission Models’ by Minimal ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#military AI`, `#OpenAI`, `#defense contracts`, `#AI refusal alignment`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [布伦特原油突破每桶 100 美元，霍尔木兹海峡运量骤降](https://oilprice.com/Energy/Crude-Oil/Oil-Breaks-100and-This-Rally-Has-Legs.html) ⭐️ 8.0/10

布伦特原油周三升破每桶 100 美元，为 7 月下旬以来首次，原因是美伊冲突再度升级令霍尔木兹海峡的石油外运量从此前报道的每日 600 万至 800 万桶降至不足 200 万桶（路透社援引 Rystad Energy 数据）。

rss · OilPrice.com · 9月10日 00:00

**「背景」** 霍尔木兹海峡是波斯湾原油外运的关键咽喉，其通行船只数量一直被市场当作油价的风向标；今年 6 月美伊停火破裂后，海峡油轮流量一度仍高于春季水平，这压住了油价，直到本周冲突再度升级——这也是布伦特原油自 7 月下旬以来首次突破每桶 100 美元。

**「影响」** 国际能源署（IEA）报告显示，7 月全球石油库存减少 6900 万桶（日均约 270 万桶），这意味着用于缓冲供应冲击的库存余量正在收窄，依赖进口原油的经济体和企业可能更快感受到燃料成本压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mezha.net/eng/bukvy/eab38bd6_iran_tightens_grip/">Iran tightens grip on Strait of Hormuz as attacks threaten... - #Mezha</a></li>
<li><a href="https://www.firstpost.com/business/houthi-attacks-red-sea-shipping-bab-el-mandeb-hormuz-traffic-us-iran-conflict-14034057.html">Two oil chokepoints under threat: Houthi attacks hit Red Sea shipping...</a></li>

</ul>
</details>

**标签**: `#oil`, `#Brent crude`, `#Strait of Hormuz`, `#US-Iran conflict`, `#IEA`

---

<a id="item-finance-news-2"></a>
### [欧洲负电价激增，欧盟承诺到 2028 年新增 30-35 吉瓦储能](https://oilprice.com/Energy/Energy-General/Negative-Power-Prices-Are-Piling-Up-Across-Europe.html) ⭐️ 8.0/10

2025 年负批发电价在欧洲多国大范围出现：据该报道，德国全年累计 573 小时负电价，超过其 2024 年的纪录，西班牙、瑞典、荷兰和法国截至 2025 年 10 月底也都超过 500 小时。为应对可再生能源发电过剩，欧盟能源部长已于 6 月达成协议，承诺到 2028 年新增约 30 至 35 吉瓦（GW）的储能容量，把欧盟储能规模提高到目前的三倍。

rss · OilPrice.com · 9月9日 21:00

**「背景」** 2022 年俄罗斯入侵乌克兰前，欧盟约 40%的天然气依赖俄罗斯进口，此后欧盟大力建设风电和光伏以摆脱这种依赖，但配套的储能设施没有跟上。风能和太阳能发电随天气波动，在阳光强、风力大的高峰时段电力供过于求，批发电价便会跌到零以下，而目前欧盟可再生能源已占其用电量的 44%。

**「影响」** 报道援引彭博的说法称，负电价已使西班牙太阳能电站价值大幅下跌，部分投资者寻求退出、一些开发商被迫停业，而储能跟不上也意味着欧盟仍需进口化石天然气来填补无风或日落时的供电缺口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oilprice.com/Energy/Energy-General/Negative-Power-Prices-Are-Piling-Up-Across-Europe.html">Negative Power Prices Are Piling Up Across Europe | OilPrice.com</a></li>

</ul>
</details>

**标签**: `#European energy`, `#negative power prices`, `#energy storage`, `#renewables`, `#EU energy policy`

---

<a id="item-finance-news-3"></a>
### [美国制裁伊朗全部剩余航空公司，收紧其航空通道](https://oilprice.com/Energy/Energy-General/US-Moves-to-Isolate-Irans-Aviation-Sector-From-the-Global-Economy.html) ⭐️ 8.0/10

美国财政部 9 月 8 日对 36 个目标实施制裁，其中包括伊朗全部 27 家仍在运营的航空公司，以及被指帮助伊朗航空网络采购飞机、零部件和技术的外国公司与一名个人；这是华盛顿首次动用其 8 月 24 日针对伊朗航空业的定向授权。财政部称，伊朗政府利用该行业运输武器、人员和违禁货物。

rss · OilPrice.com · 9月9日 18:00

**「背景」** 美国自 2011 年起就以反恐为由制裁马汉航空，指其向伊朗伊斯兰革命卫队提供人员、武器和军事装备运输等后勤支持。本轮措施依据的是 8 月 24 日启动的“经济弃儿行动”（Operation Economic Outcast）以及同日出台的一项针对伊朗航空业的新认定，9 月 8 日的制裁是该认定首次被用来制裁伊朗剩余航空公司。

**「影响」** 由于全球几乎所有商用飞机都是美国原产，或使用美国控制的发动机和航电系统，继续为伊朗航空公司供油、提供地面服务、货运代理或金融结算的第三方企业，将面临业务与被排除在美国金融体系之外的取舍——这是前美国财政部外国资产控制办公室高级官员 Kerri Bitsoff 对 RFE/RL 作出的评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://home.treasury.gov/news/press-releases/sb0623/">Treasury Grounds Iranian Airlines with Sweeping Sanctions Action | U.S. Department of the Treasury</a></li>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/09/operation-economic-outcast-grounds-irans-aviation-sector">Operation Economic Outcast Grounds Iran’s Aviation Sector - United States Department of State</a></li>

</ul>
</details>

**标签**: `#Iran sanctions`, `#aviation`, `#Mahan Air`, `#OFAC/Treasury`, `#secondary sanctions`

---

<a id="item-finance-news-4"></a>
### [谷歌在芬兰投资至少 130 亿欧元建 AI 基础设施，并签 22 年核电协议](https://oilprice.com/Latest-Energy-News/World-News/Google-Bets-13-Billion-on-Finland-to-Power-AI-Boom-With-Nuclear-Energy.html) ⭐️ 8.0/10

谷歌宣布将在 2027 至 2028 年向芬兰人工智能基础设施投资至少 130 亿欧元（约 151 亿美元），并与芬兰能源公司 Fortum 签署为期 22 年的购电协议，购买 Loviisa 核电站最多 50%的发电量；两家公司称，这是谷歌在美国境外的首份核电合同。Fortum 表示，该协议为其核电站的延寿和升级提供资金，使其运营至 2050 年，否则该电站将在 2030 年后关闭——该电站供应芬兰约 10%的电力，雇佣近 600 人。

rss · OilPrice.com · 9月9日 16:30

**「背景」** 洛维萨（Loviisa）核电站位于芬兰同名城镇附近，装有两座苏联设计的压水反应堆，各约 507 兆瓦，发电量占芬兰电力供应的约 10%，电站运营方 Fortum 已于 2022 年提交了将反应堆寿命延长至 2050 年的计划。此次签署的 22 年购电协议（即长期约定买电价格与数量的合同）为延寿和升级提供资金，否则该电站须在 2030 年后关闭。

**「影响」** 该协议为洛维萨核电站的延寿与升级提供资金，使这座供应芬兰约 10%电力、雇佣近 600 人的电厂能运营至 2050 年，而不是在 2030 年后被迫关停，直接影响芬兰的电力供应和该厂员工。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Loviisa_Nuclear_Power_Plant">Loviisa Nuclear Power Plant - Wikipedia</a></li>
<li><a href="https://www.fortum.com/energy-production/nuclear-power/plants/loviisa">Loviisa Nuclear Power Plant | Fortum</a></li>

</ul>
</details>

**标签**: `#Google-Alphabet`, `#Nuclear energy`, `#AI infrastructure`, `#Finland`, `#Corporate investment`

---

<a id="item-finance-news-5"></a>
### [英国央行行长警告：伊朗冲突或使英国通胀升破 4%](https://oilprice.com/Energy/Energy-General/Bank-of-England-Warns-Iran-War-Could-Push-UK-Inflation-Above-4.html) ⭐️ 8.0/10

英国央行行长安德鲁·贝利周二警告称，伊朗冲突和能源价格高企给英国通胀带来上行风险。英国央行夏季报告预测，若油价在每桶 100 美元附近持续数月，通胀可能升破 4%，而 7 月通胀年率为 2.9%（6 月为 2.6%），央行目标为 2%。

rss · OilPrice.com · 9月9日 16:00

**「背景」** 英国央行为通胀设定的目标是 2%，其货币政策委员会定于下周决定利率水平。自伊朗封锁霍尔木兹海峡、掐断部分主要产油国的石油出口以来，能源价格成为推高英国物价的上行压力；央行夏季报告曾测算，若油价在每桶 100 美元附近维持数月，通胀率可能超过 4%。

**「影响」** 若能源冲击持续，英国家庭可能面临更高物价，而英国政府新发债务的借贷成本已处于近 30 年最高水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/graphics/2026-iran-war-hormuz-closure-oil-shock/">Iran War: How High Could Oil Prices Get with Strait of Hormuz ...</a></li>

</ul>
</details>

**标签**: `#Bank of England`, `#UK inflation`, `#Iran conflict`, `#oil prices`, `#interest rates`

---

<a id="item-finance-news-6"></a>
### [铜价创历史新高，而铜冶炼厂加工费降至零甚至负值](https://oilprice.com/Metals/Commodities/Copper-Hits-Record-Highs-While-Smelters-Lose-Money-on-Every-Ton.html) ⭐️ 8.0/10

伦敦金属交易所三个月期铜周二创下每吨 14,779 美元的历史新高，今年累计上涨近 18%。与此同时，2026 年铜精矿年度加工精炼费基准降至每吨 0 美元，创历史最低，现货费用年中更跌至约每吨负 127 美元，意味着冶炼厂实际上要为加工矿石向矿商付费。

rss · OilPrice.com · 9月9日 15:00

**「背景」** 加工精炼费（TC/RC）指矿商为把铜精矿加工成精铜而付给冶炼厂的费用，历来是冶炼厂的主要利润来源；2026 年度基准加工费由安托法加斯塔与一家中国冶炼厂谈定为每吨 0 美元，是有记录以来的最低水平，随后现货加工费更转为负值，冶炼厂要倒付钱才能拿到原料。

**「影响」** 由于美国可能对精炼铜进口加征关税的预期，铜正被大量运往美国，COMEX 库存升至近 70 万吨，而 LME 与上海仓库合计仅约 30 万吨，美国以外买家因此面对更紧供应和更高溢价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://skillings.net/coppers-smelting-crisis-global-activity-hits-decade-low-as-treatment-charges-collapse-to-zero/">Copper Smelting Crisis 2026 : TC/RCs Hit Zero</a></li>
<li><a href="https://discoveryalert.com/analysis/copper-concentrate-scarcity-negative-tcrc/">What Record Negative TCRCs Reveal About Copper ... - Discovery Alert</a></li>

</ul>
</details>

**标签**: `#copper`, `#commodity markets`, `#smelters`, `#supply constraints`, `#US tariffs`

---

<a id="item-finance-news-7"></a>
### [美联储维持利率不变，保留加息可能](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

据 CBS 新闻报道，美联储决定维持利率不变，同时保留未来加息的可能性；ABC7 报道称，这一决定以 9 比 3 的投票结果通过。

google\_news · CBS News · 6月17日 07:00

**「背景」** 这是美联储连续第五次会议维持利率不变；据 CNBC 和美联储声明，本次会议以 9 比 3 的投票结果将联邦基金利率（银行间隔夜拆借的基准利率）目标区间维持在 3.5%至 3.75%，三位委员支持加息。据福克斯商业新闻，通胀仍顽固高于美联储 2%的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members ...</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady | Fox Business</a></li>
<li><a href="https://www.linkedin.com/posts/hilltop-securities_hilltopsecurities-economiccommentart-julyfomc-activity-7485401527298228224-zcE5">July FOMC Meeting Outlook Worsens Inflation Concerns | LinkedIn</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest rates`, `#Monetary policy`, `#US economy`

---

<a id="item-finance-news-8"></a>
### [阿达尼机场业务获约 10 亿美元融资，阿达尼企业股价上涨近 5%](https://www.cnbc.com/2026/09/09/adani-enterprises-airport-fundraise-shares.html) ⭐️ 7.0/10

阿达尼企业（Adani Enterprises）股价周三上涨近 5%，此前其机场业务签署了一项具有约束力的协议，拟向 Alpha Wave Global、Premji Invest、淡马锡以及贝莱德管理的基金募集约 982.5 亿卢比（约 10 亿美元）。公司声明称，该交易对阿达尼机场控股（Adani Airport Holdings）的投前估值约为 180 亿美元，投资者将分三批认购新股，在预计 2027 年 7 月完成的最后一批之后合计持股约 5.54%，交易仍需满足惯例条件并通过监管审批。

rss · CNBC Finance · 9月9日 06:26

**「背景」** 阿达尼机场控股是阿达尼企业旗下的机场业务平台，在印度运营 8 座机场（包括孟买、新孟买、艾哈迈达巴德等），承运该国超过 23%的旅客；阿达尼企业此前已于 7 月完成 1500 亿卢比的定向增发（QIP，即向合格机构投资者配售新股）。

**「影响」** 公司表示这笔资金将用于机场扩建与现代化改造以及“机场城市”等项目，目标是把年旅客接待能力提升至约 2 亿人次；若按计划推进，将影响使用其旗下 8 个机场的旅客以及印度机场基础设施行业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://startupfox.in/company/adani-airport-holdings">Adani Airport Holdings — News, Funding &amp; Updates | StartupFox</a></li>
<li><a href="https://www.billionaires.africa/2026/09/09/indian-billionaire-gautam-adanis-airport-arm-raises-1-billion-at-an-18-billion-valuation/">Billionaire Gautam Adani &#x27;s airport arm raises $1 billion</a></li>
<li><a href="https://legal.economictimes.indiatimes.com/news/industry/adani-enterprises-raises-inr-150-billion-in-record-qip-with-cam-and-trilegal/132331254">Adani Enterprises Raises INR 150 Billion in Record QIP with CAM...</a></li>
<li><a href="https://www.gurutrade.com/news/india-s-adani-enterprises-upsizes-share-sale-to-1-75b-1783088796.html">India&#x27;s Adani Enterprises Upsizes Share Sale to $1.75B</a></li>
<li><a href="https://www.ndtv.com/india-news/adani-airport-holdings-secures-1-billion-investment-from-global-funds-12021189">Adani Airport Holdings Secures $1 Billion Investment From ...</a></li>
<li><a href="https://www.adani.com/newsroom/media-releases/adani-airports-to-raise-usd-1-billion-of-primary-equity-from-marquee-global-investors">Adani Airports to raise ~USD 1 billion of primary equity from ...</a></li>

</ul>
</details>

**标签**: `#Adani Enterprises`, `#airport infrastructure`, `#private fundraising`, `#India`, `#equity investment`

---

<a id="item-finance-news-9"></a>
### [中国电动车企转向人形机器人，小鹏为机器人业务融资 9 亿美元](https://www.cnbc.com/2026/09/09/chinas-ev-makers-shift-gears-to-focus-on-humanoids-as-car-market-slows.html) ⭐️ 7.0/10

随着中国电动车市场放缓，包括小鹏在内的中国车企正把重心转向人形机器人。小鹏上月为其机器人业务融资 9 亿美元，公司称这是中国“具身智能”（硬件与人工智能结合）行业最大单笔融资，该业务估值超过 63 亿美元，据花旗估算已与小鹏电动车业务约 65 亿美元的估值相当；小鹏股价今年累计下跌逾 45%，是主要电动车企中表现最差的一家，公司表示计划今年年底前开始量产机器人，先在自有门店和营业场所部署，明年再推向中国及海外市场。

rss · CNBC Finance · 9月9日 04:12

**「背景」** 约十年前，中国企业集中涌入电动汽车赛道，而如今这一市场在激烈竞争下增速明显放缓——据中国汽车工业协会数据（Counterpoint 引用），2026 年上半年中国汽车制造业平均利润率仅为 1.5%。正因为整车销售增长放慢、盈利变薄，车企才把机器人视为所谓“第二增长曲线”，借跨界布局重塑资本市场对其估值逻辑的看法。

**「影响」** 据 Jefferies 分析师介绍，小鹏可把 85%的电机、芯片和智能驾驶软件复用到人形机器人上，相关零部件与软件供应商由此获得新的需求来源；但该机构表示尚未看到车企获得明确的外部订单，机器人收入短期内仍主要来自车企自用场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tbreak.com/chinese-ev-makers-humanoid-robots/">Chinese humanoid robots : why EV makers are expanding</a></li>

</ul>
</details>

**标签**: `#China EV industry`, `#humanoid robotics`, `#Xpeng`, `#corporate strategy`, `#financing`

---

<a id="item-finance-news-10"></a>
### [分析质疑英国放弃净零可为每户年省 500 英镑的说法](https://oilprice.com/Energy/Energy-General/Britain-Can-Save-500-by-Scrapping-Net-Zero-If-It-Ignores-Most-of-the-Bill.html) ⭐️ 7.0/10

一篇对英国智库 Onward《Firm Foundations》报告的分析指出，该报告声称英国在 2029 年后放弃 2050 年法定净零目标可为每户家庭每年节省逾 500 英镑，但这一数字只计算电力系统成本。报告估算 2030 年至 2050 年电力系统累计节省 3200 亿英镑（按约 3000 万户、20 年折算约为每户每年 530 英镑），其替代路径假设 2050 年电力需求为 441 太瓦时，比现行政策情景的 484 太瓦时低约 10%，原因是减少了对电动车、热泵和电解制氢的支持。

rss · OilPrice.com · 9月9日 19:00

**「背景」** 英国智库 Onward 在《Firm Foundations》报告中比较了现行政策与一项 2029 年后放弃 2050 年净零目标的替代路径，估算后者在 2030 至 2050 年间可累计节省 3200 亿英镑电力系统成本，这是每户每年约 530 英镑说法的来源。

**「影响」** 英国议会已提交草案令，把 2038—2042 年的第七个碳预算定为 5.35 亿吨二氧化碳当量（较 1990 年水平约减少 87%），因此“放弃净零是否更省钱”的争论直接关系到英国电力、供暖和交通行业是继续按这一法定目标投资，还是转向更多依赖天然气和核能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/what-onward-report-gets-right-where-i-think-stops-too-shaun-sweeney-nxybf">What the Onward Report Gets Right — and Where I Think It Stops...</a></li>
<li><a href="https://www.yahoo.com/news/world/articles/britain-save-500-scrapping-net-190000216.html">Britain Can Save £ 500 by Scrapping Net Zero , If It Ignores Most of the...</a></li>
<li><a href="https://www.theccc.org.uk/publication/supplementary-analysis-of-the-seventh-carbon-budget/">Supplementary analysis of the Seventh Carbon Budget</a></li>
<li><a href="https://hansard.parliament.uk/lords/2026-06-10/debates/26060257000011/SettingTheSeventhCarbonBudget">Setting the Seventh Carbon Budget - Hansard - UK Parliament</a></li>

</ul>
</details>

**标签**: `#UK energy policy`, `#net zero`, `#household energy bills`, `#electrification`, `#policy analysis`

---

<a id="item-finance-news-11"></a>
### [白俄罗斯炼油厂借俄罗斯燃料短缺创十年最高盈利](https://oilprice.com/Latest-Energy-News/World-News/Belarus-Refineries-Post-Decade-High-Profits-Amid-Russias-Fuel-Crisis.html) ⭐️ 7.0/10

据独立媒体 Pozirk 报道，白俄罗斯炼油厂 2026 年录得十年来最高盈利；路透贸易数据显示，该国前七个月对俄罗斯汽油出口量达近 66.5 万吨，是 2025 年同期的 25 倍，柴油出口约 41.8 万吨，增长约七倍。这一“十年最高”是白俄罗斯国家石化企业 Belneftekhim 负责人伊利亚·伊坎的说法，Pozirk 未公布具体利润数字或经审计的同比数据。

rss · OilPrice.com · 9月9日 18:30

**「背景」** 白俄罗斯只有 Naftan 和 Mozyr 两座炼油厂，合计年加工能力约 2400 万吨，长期以“代加工”（tolling）方式把俄罗斯原油炼成成品油、再返销俄罗斯市场。乌克兰无人机对俄炼油设施的袭击压低了俄方自己的炼油产出，由此形成白俄罗斯此番填补的供应缺口。

**「影响」** 俄罗斯炼油产能下降已直接波及当地车主：据 The Insider 报道，8 月中旬全国不到三分之一加油站有油可加，至少十几个地区恢复限购。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oilprice.com/Latest-Energy-News/World-News/Belarus-Refineries-Post-Decade-High-Profits-Amid-Russias-Fuel-Crisis.html">Belarus Refineries Post Decade-High Profits Amid Russia &#x27;s Fuel Crisis</a></li>
<li><a href="https://www.twz.com/news-features/ukraine-carried-out-its-deepest-drone-strike-on-russia-ever">Ukraine Carried Out Its Deepest Drone Strike On Russia Ever</a></li>
<li><a href="https://themiddleeastinsider.com/2026/04/04/gulf-refinery-crisis-drone-attacks-energy-security-2026/">Gulf Refinery Crisis : How Drone Attacks... — The Middle East Insider</a></li>

</ul>
</details>

**标签**: `#Belarus energy`, `#Russia fuel crisis`, `#oil refining`, `#export ban`, `#energy markets`

---

<a id="item-finance-news-12"></a>
### [乌干达推出新原油品级“珍珠甜油”，首次出口临近](https://oilprice.com/Energy/Crude-Oil/Uganda-Launches-New-Crude-Grade-as-First-Oil-Exports-Near.html) ⭐️ 7.0/10

乌干达正准备出口产自阿尔伯特湖油田的新原油品级“珍珠甜油”（Pearl Sweet），两个项目在稳产期预计合计日产 23 万桶。原定 2026 年 6 月的首次出油目标已错过，官员现在预计 Kingfisher 油田 12 月以每日 2.5 万桶启动，Tilenga 则在 2027 年第一季度投产。

rss · OilPrice.com · 9月9日 17:00

**「背景」** 项目由 TotalEnergies（56.67%）、中国海油（28.33%）和乌干达国家石油公司 UNOC（15%）共同持有，原油需经投资 56 亿美元、全长 1443 公里的东非原油管道（EACOP）运往坦桑尼亚坦噶港，该管道仍在建设中。珍珠甜油含硫量约 0.16%，但蜡含量高、倾点约 39 摄氏度，从井口到油轮到岸全程需要加热输送。

**「影响」** 乌干达将因此获得新的石油出口收入，但输往坦噶港的运输成本预计为每桶 12 至 13 美元，加上可能出现的品质折价，会压缩其实际收益，同时要求炼厂和油轮承担额外的加热与处理成本。

**标签**: `#Uganda oil`, `#Pearl Sweet crude`, `#EACOP pipeline`, `#African oil exports`, `#TotalEnergies`

---