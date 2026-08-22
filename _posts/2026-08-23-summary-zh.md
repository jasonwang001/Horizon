---
layout: default
title: "Horizon Summary: 2026-08-23 (ZH)"
date: 2026-08-23
lang: zh
---

> 从 153 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [SGLang v0.5.18：710 个合并 PR、新增多模型并优化性能](#item-tech-news-1) ⭐️ 8.0/10
2. [MCP 路线图：代理授权与 HTTP 简化](#item-tech-news-2) ⭐️ 8.0/10
3. [评估分辨率显著影响 V1 脑相似学习规则识别](#item-tech-news-3) ⭐️ 8.0/10
4. [SemiAnalysis：开源模型追平闭源时间每代减半](#item-tech-news-4) ⭐️ 8.0/10
5. [美国团体促 FTC 调查 AI 公司买书销毁行为](#item-tech-news-5) ⭐️ 8.0/10
6. [Munder Difflin：用编码代理运行办公室式克隆协作](#item-tech-news-6) ⭐️ 7.0/10
7. [从零训练 250M 量化模型，60MB 部署与磁盘长上下文](#item-tech-news-7) ⭐️ 7.0/10
8. [开源 Roguelike DelveRL 用于训练游戏代理](#item-tech-news-8) ⭐️ 7.0/10
9. [单张 RTX 5090 实测 Qwen3.8-27B NVFP4：262K 真实窗口与 77 tok/s](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [美联储连续第五次会议维持利率不变，凸显通胀担忧](#item-finance-news-1) ⭐️ 9.0/10
2. [莱茵河低水位仍限制运输，欧洲靠疲弱需求避免更大危机](#item-finance-news-2) ⭐️ 8.0/10
3. [燃气轮机交期排到 2031 年，成为 AI 数据中心最大瓶颈](#item-finance-news-3) ⭐️ 8.0/10
4. [清洁能源支出有望在 2026 年创下 1800 亿美元纪录](#item-finance-news-4) ⭐️ 8.0/10
5. [Alphabet 与亚马逊拟投 4200 亿美元建 AI 基础设施，硬件股或受益](#item-finance-news-5) ⭐️ 8.0/10
6. [苹果宣布库克任内最大规模股票回购](#item-finance-news-6) ⭐️ 8.0/10
7. [霍尔木兹之外：五个正受影响的石油咽喉点](#item-finance-news-7) ⭐️ 7.0/10
8. [IEA：东南亚电网投资到 2050 年需增至近四倍](#item-finance-news-8) ⭐️ 7.0/10
9. [罗斯百货与 TJX 同店销售额增长分化](#item-finance-news-9) ⭐️ 7.0/10
10. [伯克希尔·哈撒韦对一家大型银行进行 16 亿美元投资动作](#item-finance-news-10) ⭐️ 7.0/10
11. [道琼斯期货显示市场反弹，英伟达财报与加拿大新关税成焦点](#item-finance-news-11) ⭐️ 7.0/10
12. [美国财政部意外回购国债 债券市场影响受关注](#item-finance-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SGLang v0.5.18：710 个合并 PR、新增多模型并优化性能](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 已发布，这是一个包含 212 位贡献者提交的 710 个合并 PR 的重要版本，新增 Muse Glimmer、Intern-S2-Mobius、SANA-Video、LingBot-Video-MoE、LTX-2.5、Cosmos3 Edge &amp; Distilled 和 LongCat-Image 等模型支持，覆盖自回归与扩散模型。启动时新增重叠 checkpoint 暂存机制，通过 \`--startup-weight-load-mode overlap\` 启用，使 H100 上 Qwen3-32B 的启动速度比串行 prefetch 快 8.6%–11.7%，比默认方式快 2.38 倍（35.6 秒对 84.8 秒）。TP LMHead 改为 All-to-All 后，DeepSeek-V4-Pro 在 B200 解码的 LMHead 耗时从 320 微秒降至 169 微秒，TPOT 从 36.97 毫秒改善至 35.67 毫秒；FlashInfer MNNVL 纯 allreduce 路径使 DeepSeek-V4-Flash 在 Blackwell TP4 小 batch 解码最多提升约 6.9%。依赖升级至 torch 2.13.0、triton 3.7.1、flashinfer 0.6.17 等，并统一将 Triton、FlashInfer、Inductor、DeepGEMM 和 CUDA 驱动缓存收归 \`SGLANG\_CACHE\_DIR\`，升级后首次启动会重新编译一次。

github · Fridge003 · 8月22日 00:09

**「背景」** SGLang（Structured Generation Language）是由 LMSYS 等研究机构提出的开源大语言模型与多模态模型推理/服务框架，以 Python 嵌入式结构化生成语言和高吞吐运行时为特点，支持从单 GPU 到大规模分布式集群的低延迟推理。本次 v0.5.18 是继此前版本之后的一次大规模聚合更新，包含 710 个合并 PR，新增多种自回归与扩散模型支持，并引入启动加速、LMHead 通信优化、统一编译内核缓存目录等性能与工程改进。该框架被广泛用于 LLM 推理场景，这些更新对依赖高性能推理服务的开发者和组织具有直接影响。

**「影响」** 对依赖 SGLang 进行推理的开发者，升级到 v0.5.18 后首次启动会因统一缓存目录触发一次性重新编译，同时可借新增的启动重叠暂存和 LMHead all-to-all 优化在特定模型上获得启动与解码延迟改善。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SGLang">SGLang - Wikipedia</a></li>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/sglang: SGLang is a high-performance serving ...</a></li>

</ul>
</details>

**标签**: `#SGLang`, `#LLM inference`, `#model support`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [MCP 路线图：代理授权与 HTTP 简化](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

模型上下文协议（MCP）官方发布新路线图，计划在代理授权、代理身份识别和 HTTP 简化方面推进协议变更。路线图的目标是让远程 MCP 服务器不再有别于普通 HTTP 工作负载，从而降低 AI 代理与工具集成的复杂度。该消息在 Hacker News 上获得 167 分和 120 条评论，显示开发者对 MCP 演进方向高度关注。

hackernews · pentagrama · 8月22日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=49399591)

**「背景」** 模型上下文协议（MCP）是一种开放协议，旨在为 AI 代理提供标准化的方式连接工具和数据源。此前 MCP 的设计包含自定义的协议层、协议级会话追踪以及依赖浏览器的人工授权流程；新路线图以 2026-07-28 版本为节点，推动 MCP 在协议层变成无状态的 HTTP 工作负载，并基于 OAuth 2.1 与 DPoP 等现有标准支持代理身份和授权，以减少对粘贴式 API 密钥和长期令牌的依赖。

**「影响」** 对正在构建 AI 代理、MCP 服务器或依赖 MCP 的工具链的开发者，路线图意味着需要跟进授权与身份模型的标准化调整，并评估 HTTP 简化对现有集成的兼容性影响。

**「社区讨论」** 社区反应分化。部分开发者赞同 HTTP 简化，认为取消专有协议是改进；另一些人质疑服务器是否会完整实现新规范，或认为 REST 加 skills.md 已足够，还有人因早期标准反复而失去信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://blog.modelcontextprotocol.io/posts/mcp-roadmap/">The New MCP Roadmap | Model Context Protocol Blog</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/tutorials/security/authorization">Understanding Authorization in MCP - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#mcp`, `#protocols`, `#ai-agents`, `#developer-tools`, `#api-evolution`

---

<a id="item-tech-news-3"></a>
### [评估分辨率显著影响 V1 脑相似学习规则识别](https://www.reddit.com/r/MachineLearning/comments/1vvdxwt/the_evaluation_resolution_has_been_shown_to_have/) ⭐️ 8.0/10

一项预印本研究表明，评估分辨率会显著改变哪种学习规则在 V1 上显得最像人脑，并推翻了“未训练 CNN 能匹配甚至超过反向传播训练 CNN”的常见说法。作者使用 CIFAR-10 子集训练的 32px 小 CNN、五种学习规则（随机初始化、反向传播、反馈对齐、预测编码、STDP）在 THINGS-fMRI 刺激上于 32px 至 224px 六种分辨率下评估，并固定权重和归一化。反向传播与未训练网络在 V1 上的差距随分辨率非单调变化，从 32 像素的−0.001±0.007 变为 224 像素的+0.044±0.006（n=5 种子），且排除了训练/评估分辨率匹配、低层结构、批归一化校准、池化特征收敛至全局亮度等伪影。内容 vs 池化对照表明该依赖主要来自图像内容；反向传播优于未训练的 LOC 效应在所有分辨率下都存在，另外作者还修正了三篇早期预印本中的批归一化评估模式 bug。代码已开源（GitHub），意味着此类模型-大脑比较结论需要按分辨率仔细检验。

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · 8月22日 14:30

**「背景」** 在模型-大脑比较中，代表相似性分析（RSA）通过比较神经网络与人类视觉皮层对刺激的表征距离来评估对齐程度。此前于 2026 年 4 月发布的一项系统性比较（arXiv:2604.16875）显示，未训练的 CNN 在 V1 上与反向传播训练网络的脑对齐表现无法区分（差异 d=-0.01），并认为这一结果扩展了随机网络具有非平凡视觉结构的观察。本预印本正是针对这一被广泛引用的结论，提出该现象主要源于评估分辨率造成的假象，并通过固定权重、在 32 像素至 224 像素六个分辨率下比较五种学习规则来检验这一假设。

**「影响」** 对模型-大脑比较研究者而言，评估分辨率必须作为关键变量报告和控制，否则“未训练 CNN 更像 V1”的结论可能只是低分辨率伪影；本次工作还修正了三篇早期预印本中的批归一化评估 bug，为后续复现提供了更可靠的基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.16875v1">Untrained CNNs Match Backpropagation at V1: A Systematic RSA Comparison of Four Learning Rules Against Human fMRI</a></li>
<li><a href="https://arxiv.org/abs/2604.16875">[2604.16875] Untrained CNNs Match Backpropagation at V1: A Systematic RSA Comparison of Four Learning Rules Against Human fMRI</a></li>

</ul>
</details>

**标签**: `#computational neuroscience`, `#convolutional neural networks`, `#learning rules`, `#evaluation methodology`, `#brain-like models`

---

<a id="item-tech-news-4"></a>
### [SemiAnalysis：开源模型追平闭源时间每代减半](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis 的分析指出，开源与闭源前沿模型的能力差距呈周期性变化，且每一代开源模型追平闭源的时间减半。文章将大模型发展划分为扩展、推理和智能体三个时代，其中智能体时代追赶最快：Kimi K2.6 用 4.8 个月超越 Opus 4.5，GLM-5.2 用 6 个月超过 GPT-5.2。GLM 5.3、Kimi K3 等开源模型已能胜任许多曾帮助 Anthropic 获得 650 亿美元以上年化收入的编程与智能体任务，引发模型层商品化的担忧。不过基准测试并非全部，Anthropic 的产品化能力仍是其优势。

telegram · zaihuapd · 8月22日 08:26

**「背景」** SemiAnalysis 将大模型发展划分为早期扩展、推理和智能体三个时代，并测算开源模型与闭源前沿的能力差距呈周期性变化，且每一代开源模型追平闭源的时间都在减半。在智能体时代，追赶速度最快，例如 Kimi K2.6 在 4.8 个月内以 56.3 分超越 Opus 4.5，GLM-5.2 在 6 个月内以 72.4 分超过 GPT-5.2。这些进展引发对模型层商品化的担忧，但基准测试之外，闭源厂商的产品化能力仍被视为优势。

**「影响」** 开源模型追赶时间每代减半的实证意味着，Kimi K3、GLM-5.3 等开源权重模型已可覆盖此前支撑 Anthropic 650 亿美元年化收入的编程与智能体任务，且已有平台支持私有化托管 Kimi K3，企业能以更低成本和更强数据管控复制同类能力，进一步压低模型层定价；这使 Anthropic 等闭源厂商更依赖产品化与标准（如 MCP）来维持护城河。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/are-open-models-catching-up">Are Open Models Catching Up?</a></li>
<li><a href="https://www.linkedin.com/pulse/standardizing-commoditization-anthropics-model-context-sam-bobo-n8tse">Standardizing for Commoditization — Anthropic ’s Model Context...</a></li>
<li><a href="https://synthetic.new/">Synthetic | Chat with open - source models privately</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#large language models`, `#AI industry analysis`, `#model commoditization`, `#SemiAnalysis`

---

<a id="item-tech-news-5"></a>
### [美国团体促 FTC 调查 AI 公司买书销毁行为](https://www.axios.com/2026/08/21/ftc-ai-companies-book-destruction-investigate) ⭐️ 8.0/10

8 月 21 日，美国十余家民间团体联名致信联邦贸易委员会（FTC），要求调查 AI 公司购买、扫描并销毁实体书以训练模型的行为是否构成《联邦贸易委员会法》第 5 条下的不公平竞争手段。联名团体包括 Demand Progress 教育基金、美国消费者联合会等，称这种「囤积并销毁」的做法让市场丧失关键素材，部分珍本可能永久消失。信件特别指出，Anthropic 曾耗资数百万美元购书并切除书脊，将扫描页喂给 Claude；谷歌、微软和 OpenAI 也面临类似版权诉讼。团体认为该做法抬高对手成本、构筑护城河，但不主张限制 AI 训练本身。若 FTC 受理，AI 训练数据之争将从版权领域延伸至竞争监管。

telegram · zaihuapd · 8月22日 15:40

**「背景」** AI 公司为训练大语言模型需要海量高质量文本，实体书是重要的数据来源之一，但大规模扫描和复制书籍引发了版权争议。此次联名信在已有版权诉讼基础上，寻求通过竞争法规制 AI 公司获取训练数据的方式，将争议焦点从侵犯著作权转向是否存在不公平竞争。

**「影响」** 若 FTC 受理该调查请求，AI 公司购买并销毁书籍的训练数据获取模式可能面临新的监管压力，并有可能将 AI 训练数据之争扩展至反垄断和竞争执法领域，同时增加珍稀实体书永久灭失的风险。

**标签**: `#AI regulation`, `#FTC`, `#competition policy`, `#copyright`, `#AI training data`

---

<a id="item-tech-news-6"></a>
### [Munder Difflin：用编码代理运行办公室式克隆协作](https://munderdiffl.in/) ⭐️ 7.0/10

Munder Difflin 是一个本地多代理协调工具，可以在现有编码代理（如 Claude Code、Codex 及几乎所有主流 harness）之上运行一组“克隆”模拟，目标是让多代理工作流可确定化并降低令牌消耗。该项目由开发者 Chaitanya 构建，发布一周内已有 2 万多名用户；它的模拟不消耗令牌，用户普遍反映减少了令牌使用。它借用《办公室》（The Office）主题来呈现多个代理各自追求小目标、彼此竞争并最终导致结果崩溃的“办公室式”协作状态。该工具定位为面向 AI 代理开发者的本地辅助工具，而非重大技术突破。

hackernews · simonpure · 8月22日 09:49 · [社区讨论](https://news.ycombinator.com/item?id=49398152)

**「背景」** Munder Difflin 是一个开源的多智能体（multi-agent）协调工具，能够将现有的编码智能体（如 Claude Code 和 Codex 命令行工具）组织成一个自协调的团队，用于自动处理 PR 审查、规格撰写和 CRM 更新等任务。这种“多智能体协调工具”与单个智能体或框架不同，它通过安排多个 AI 编码智能体协同工作来模拟一个办公团队，并且其模拟过程是确定性的，不消耗 token，同时可以降低整体 token 使用量。该工具由 Chaitanya Giri 开发，目前已在开发者社区中流行。

**「影响」** 对于已使用 Claude Code、Codex 等编码代理的开发者，Munder Difflin 提供一种本地、确定性且可节约令牌的多代理编排方式；发布一周超过 2 万用户采用，说明它确实解决了部分人的真实需求，但目前仍是小众开发工具，影响范围局限在 AI 代理与开发者工具社区。

**「社区讨论」** 社区整体认可其“办公室”主题，因为它准确反映了多代理系统常见的功能失调：不同代理各自追求小目标、相互竞争，最终让预期结果崩溃。开发者 Chaitanya 现身回答问题并强调模拟确定性、不消耗令牌；也有用户（如 joshstrange）认为它更像“管道和角色”而非真正的代理，希望支持按角色动态创建 N 个代理以及“计划→审查计划→审批门→开发→代码审查”的流水线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://munderdiffl.in/blog/what-is-a-multi-agent-harness/">What Is a Multi- Agent Harness ? (Plain-English... — Munder Difflin Blog</a></li>
<li><a href="https://www.stork.ai/en/munder-difflin">Munder Difflin Review (2026) | Stork.AI</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#multi-agent`, `#developer-tools`, `#llm`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [从零训练 250M 量化模型，60MB 部署与磁盘长上下文](https://www.reddit.com/r/MachineLearning/comments/1vv2nkh/i_developed_my_own_quantized_llm_from_scratch/) ⭐️ 7.0/10

一位开发者从零开始在 30B tokens 的 FineWeb 数据上训练了 250M 参数的 LLM，并将其量化到低于 2 比特，使整个部署仅 60MB，运行时约需 80MB 内存，在普通笔记本 CPU 上可达约 400 tok/s 且无需 GPU。模型通过磁盘缓存实现长上下文：最近的 2048 个 token 以 fp16 KV cache 保存，更早的 token 被压缩至 1 比特并以约 320 字节/token 写入磁盘，因此 100 万 token 历史约占用 320MB 磁盘空间，模型被训练为从该磁盘缓存中检索最多 1 亿 token 的内容。基座模型在未见过的英文网页测试集上交叉熵为 3.15 nats/token，困惑度 23.3，0.99 bits/byte；词表采用固定 512 比特编码（共 131k token，仅 8.4MB，无训练参数），在 WordSim-353 相似度任务上斯皮尔曼相关系数为 0.619，而随机编码为 0.029。该项目提供了完整微调工具、演示和权重，展示了一种面向边缘设备的极端量化与检索式长上下文方案。

reddit · r/MachineLearning · /u/Final-Data-1410 · 8月22日 04:39

**「背景」** 大语言模型在处理长文本时通常依赖 KV cache 保存历史 token 的键值表示，随上下文增长会占用大量内存，因此不少方案通过量化或压缩 KV cache 来降低资源消耗。该项目的创新在于把更早的历史 token 压缩到 1 比特并写入磁盘，只在需要时检索相关内容，同时从训练阶段就让模型适应这种磁盘检索机制，这使其能在极低资源设备上维持很长的有效上下文。

**「影响」** 该方案可能让开发者在内存受限的边缘设备上部署具有极大上下文窗口的小型模型，尤其适合基于档案或知识库的检索问答场景；但模型仅有 250M 参数且未训练对检索内容进行复杂推理，因此不能取代具备完整长上下文推理能力的大模型，只能作为高效轻量替代方案。

**标签**: `#quantization`, `#efficient inference`, `#long context`, `#edge AI`, `#from-scratch training`

---

<a id="item-tech-news-8"></a>
### [开源 Roguelike DelveRL 用于训练游戏代理](https://www.reddit.com/r/MachineLearning/comments/1vvii1j/i_built_an_opensource_roguelike_specifically_for/) ⭐️ 7.0/10

DelveRL 是一个从零构建的开源 Roguelike 游戏环境，专为训练游戏代理设计，解决了多数游戏难以与代理训练框架集成的问题。它提供结构化 API、确定性模拟、程序化关卡和部分可观测性，并以无限回合制玩法要求代理探索、管理风险与资源、战斗并逃离每层。项目包含无渲染器的批量并行环境和循环 PPO 训练器，基线代理中位成绩为第 18 层，延长运行可达第 33 层。游戏代码、训练代码、检查点、接口文档和原始基准均开放，便于社区直接复现和提出新方法。

reddit · r/MachineLearning · /u/SnyderConsulting · 8月22日 17:32

**「背景」** 强化学习（RL）是机器学习中让智能体通过与环境互动学习决策的子领域。OpenAI Gym 等框架提供了标准化的环境接口，但许多现有游戏环境难以与智能体训练框架集成。DelveRL 是一个专为 RL 设计的终端回合制 roguelike 环境，具备确定性模拟、程序化生成关卡和部分可观测性，使研究者能在受控条件下训练智能体完成探索、资源管理和风险规避等任务。

**「影响」** 对从事游戏代理强化学习的研究者和开发者而言，DelveRL 提供了一个开箱即用的开源环境与基准，可立即用于训练、评估和比较新算法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-gym-beta/">OpenAI Gym Beta | OpenAI</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#roguelike`, `#open source`, `#game environments`, `#PPO`

---

<a id="item-tech-news-9"></a>
### [单张 RTX 5090 实测 Qwen3.8-27B NVFP4：262K 真实窗口与 77 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1vvl7pc/single_rtx_5090_qwen3827b_nvfp4_at_a_real_262k/) ⭐️ 7.0/10

一位用户分享了在单张 RTX 5090 上通过 vLLM 0.27.1 日常运行 Qwen3.8-27B NVFP4（joshebbs/qwen3.8-27b-uncensored-nvfp4-modelopt，固定修订版）的可复现配置，声称完整 262,144 token 上下文窗口可与视觉、FP8 KV、前缀缓存、工具调用及 KDE 桌面共存。模型为 64 层混合架构（48 层 Gated DeltaNet + 16 层全注意力），检查点 19.18 GiB；在实际运行中，短上下文（1K 提示）解码达 77.2 tok/s，128K 已驻留时降至 64.7 tok/s，262K 预填充耗时 166 秒。前缀缓存测试显示冷 TTFT 6.437 秒，四次缓存命中约 0.288 秒（加速 22.3 倍），但 vLLM 在启用前缀缓存时会将混合 Mamba/DeltaNet 缓存置于实验性对齐模式，若输出损坏应先关闭该功能。硬件为 600 W 功耗限制的 RTX 5090、i7-14700K、32 GiB 内存、Arch Linux、NVIDIA 驱动 610.57.04；vLLM 报告 KV 容量 268,170 token，KV 池被手动固定为 8.52 GiB，整卡占用 30,532 MiB，剩余约 1.6 GiB，说明可运行但余量不大。

reddit · r/LocalLLaMA · /u/Fz1zz · 8月22日 19:16

**「背景」** Qwen3.8-27B 是阿里巴巴推出的 27B 参数多模态混合注意力模型：64 层中 48 层使用线性注意力（Gated DeltaNet），16 层保留全注意力，原生支持 262,144 token 上下文并可扩展至 1M token，同时带有视觉塔和 MTP 草稿头。NVFP4 是 NVIDIA ModelOpt 的 4 位浮点量化格式，该模型的 NVFP4 权重约 19.18 GiB。vLLM 是一个高性能推理引擎，配合单张 32GB 显存的 RTX 5090，用户实测可在真实 262K 上下文窗口下运行该模型并保留视觉、前缀缓存、工具调用等能力。

**「影响」** 对于拥有 RTX 5090 的本地大模型用户，该配置证明 27B 模型可带视觉和工具调用在 262K 窗口下真实完成推理，但约 1.6 GiB 的空闲显存意味着同时运行第二个大型 CUDA 工作负载会失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-27B">Qwen/ Qwen 3 . 8 - 27 B | vLLM Recipes</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#Qwen`, `#NVFP4`, `#RTX 5090`, `#long context`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储连续第五次会议维持利率不变，凸显通胀担忧](https://news.google.com/rss/articles/CBMinwFBVV95cUxNbVA1MzJGNXllN1RjSG43b0xUam1seWRjUmI2bHdXdlZndHhEQ1pRZDI5WVE3MGg1NnBCMk9Gcm42MUZab29ZRFY3OTd3OTZERlZmLUtFbGhUOG5jQXlDREFuMGVkSmtyTlJvVzJhS1A0OG5zaGhWZkZ1VHlQRXNGcGcxczNOMW82ckdRdVJmRUZzRDI4OEV4SHRfSjh6Wms?oc=5) ⭐️ 9.0/10

美联储连续第五次会议决定维持利率不变，此举凸显其仍担忧通胀压力。

google\_news · NBC News · 7月29日 07:00

**「背景」** 美联储在连续第五次会议上决定维持利率不变，将联邦基金利率保持在 3.50%-3.75%区间；本次决议以 9 票赞成、3 票反对通过，主要反映对通胀持续影响家庭财务的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/fed-chair-kevin-warsh-faces-090000540.html">The Fed holds interest rates for a fifth consecutive meeting ...</a></li>
<li><a href="https://www.livemint.com/market/stock-market-news/us-federal-reserve-holds-rates-steady-for-fifth-consecutive-meeting-11785346712831.html">US Federal Reserve holds rates steady for fifth consecutive meeting</a></li>
<li><a href="https://www.advisorperspectives.com/dshort/updates/2026/07/29/feds-interest-rate-decision-july-29-2026">Fed&#x27;s Interest Rate Decision: July 29, 2026 - dshort - Advisor Perspectives</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#economy`

---

<a id="item-finance-news-2"></a>
### [莱茵河低水位仍限制运输，欧洲靠疲弱需求避免更大危机](https://oilprice.com/Energy/Energy-General/Europe-Dodges-a-Rhine-Crisis-for-the-Worst-Possible-Reason.html) ⭐️ 8.0/10

莱茵河水位从 8 月中旬的创纪录低位略有回升，但关键瓶颈考布河段当前约 45 厘米，仍低于 77 厘米的正常通航基准，内河运输仍受限。报道认为，欧洲未出现更严重中断，主要是因为工厂和消费者需求疲软，而非运输能力恢复。

rss · OilPrice.com · 8月22日 23:00

**「背景」** 考布是莱茵河中游的瓶颈航段，连接鹿特丹、安特卫普等港口与德国南部等工业区；水深不足时，驳船只能装载很少货物，化工和燃料运输首先承压。

**「影响」** 影响已显现：LyondellBasell 和 Covestro 已宣布部分化工产品因无法正常交货而遭遇不可抗力，法国东部出现局部汽油短缺，瑞士进口成本上升。

**标签**: `#Rhine river`, `#European chemicals`, `#supply chain`, `#transport disruption`, `#energy`

---

<a id="item-finance-news-3"></a>
### [燃气轮机交期排到 2031 年，成为 AI 数据中心最大瓶颈](https://oilprice.com/Energy/Energy-General/The-Gas-Turbine-Shortage-Just-Became-AIs-Biggest-Constraint.html) ⭐️ 8.0/10

GE Vernova 表示，现在订购的重型燃气轮机要到 2031 年才能交付；高盛估计，美国数据中心用电需求将从 2025 年的 31 吉瓦增至 2027 年的 66 吉瓦，而整个行业一年的燃气轮机产量远低于这一增量。

rss · OilPrice.com · 8月22日 21:00

**「背景」** GE Vernova、西门子能源和三菱重工的燃气轮机积压订单合计约 220 吉瓦（统计口径不同，不能直接相加），交货周期普遍在三年以上；瓶颈主要来自特种铸件、焊工和工厂排期，而非天然气价格。

**「影响」** 这意味着依赖新建燃气电厂供电的 AI 数据中心在 2027 年前后可能面临电力缺口和成本上升；PJM 电力市场 2028/29 年容量拍卖已触及价格上限，但仍比可靠性要求低约 6.8 吉瓦。

**标签**: `#gas turbines`, `#data centers`, `#energy demand`, `#supply chain`, `#AI infrastructure`

---

<a id="item-finance-news-4"></a>
### [清洁能源支出有望在 2026 年创下 1800 亿美元纪录](https://oilprice.com/Energy/Energy-General/Clean-Energy-Spending-Tracking-Toward-Record-180-Billion-in-2026.html) ⭐️ 8.0/10

美国清洁能源资本支出在 2026 年上半年已达到 740 亿美元，据金融科技公司 Crux 的报告，全年有望创下 1800 亿美元的纪录。尽管联邦政府取消了部分清洁能源激励措施，但数据中心和人工智能带来的用电需求仍推动投资持续增长。

rss · OilPrice.com · 8月22日 19:00

**「背景」** 可再生能源和储能被认为是快速增加电网供电能力的最快方式，因此投资热潮正在持续。目前美国公用事业级电池储能容量已达 52 吉瓦，仅今年上半年就新增 8.3 吉瓦，电网运营商还计划到 2028 年底再增加 54 吉瓦。

**标签**: `#clean energy`, `#investment`, `#battery storage`, `#energy grid`, `#policy`

---

<a id="item-finance-news-5"></a>
### [Alphabet 与亚马逊拟投 4200 亿美元建 AI 基础设施，硬件股或受益](https://finance.yahoo.com/technology/ai/articles/alphabet-amazon-investing-420-billion-103500198.html) ⭐️ 8.0/10

Alphabet 和亚马逊计划投入 4200 亿美元用于人工智能基础设施建设（投资金额为计划数，非实际支出）。有分析认为，这一大规模资本开支可能利好相关硬件供应商。

openbb · NVDA · 8月22日 10:35

**「背景」** Alphabet 预计 2026 年资本支出在 1950 亿至 2050 亿美元之间，亚马逊预计约 2200 亿美元，这些 AI 基础设施投资将直接流向英伟达、博通、美光等硬件公司。

**「影响」** 上述投入可能提升对 AI 服务器、芯片和网络设备等硬件的需求，从而为相关硬件公司带来订单机会，但这些影响仍取决于计划的实际执行情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/alphabet-amazon-investing-420-billion-103500198.html">Alphabet and Amazon Are Investing $ 420 Billion in Artificial...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#capital expenditure`, `#Alphabet`, `#Amazon`, `#hardware stocks`

---

<a id="item-finance-news-6"></a>
### [苹果宣布库克任内最大规模股票回购](https://finance.yahoo.com/markets/stocks/articles/apple-announced-largest-ever-stock-222000154.html) ⭐️ 8.0/10

苹果宣布在蒂姆·库克领导下规模最大的股票回购计划，这是一项影响股东的重大资本回馈举措。

openbb · NVDA · 8月22日 22:20

**「背景」** 苹果在 2024 年 5 月 2 日发布季度财报时，宣布授权 1100 亿美元的股票回购计划，这是该公司历史上规模最大的回购；同时将季度现金股息从每股 24 美分提高到 25 美分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cryptobriefing.com/apple-record-110-billion-stock-buyback/">Apple announces largest-ever stock buyback at $110 billion under Tim Cook</a></li>
<li><a href="https://ca.news.yahoo.com/live-updates-apple-report-quarterly-140852867.html">Apple earnings results: Tim Cook announces biggest-ever stock buyback ...</a></li>
<li><a href="https://appleinsider.com/articles/24/05/02/apple-trying-to-charm-investors-with-biggest-stock-buyback-yet-increased-dividend">Apple to buy back record $110B in stock, raise dividend</a></li>

</ul>
</details>

**标签**: `#Apple`, `#stock buyback`, `#capital return`, `#shareholder returns`, `#corporate action`

---

<a id="item-finance-news-7"></a>
### [霍尔木兹之外：五个正受影响的石油咽喉点](https://oilprice.com/Energy/Energy-General/Every-Chokepoint-That-Isnt-Hormuz.html) ⭐️ 7.0/10

霍尔木兹海峡自 2 月底因伊朗与美国/以色列战争实际关闭，美国能源信息署估计第二季度通过量仅日均 490 万桶，远低于去年第四季度的 2160 万桶；绕道运输正在抬高油价，布伦特约 91.62 美元、WTI 约 85.56 美元。

rss · OilPrice.com · 8月22日 17:00

**「背景」** 为绕开海峡，沙特将原油转向东-西管道至红海延布港，但胡塞武装 7 月 20 日宣布对沙特实施海上封锁，红海曼德海峡过境量一度降至一年最低。

**「影响」** 受影响的油轮和出口商正被迫绕行好望角，单批沙特原油约增加 160 万美元燃油费和 100 万美元运河费；黑海新罗西斯克等码头遭无人机袭击后，哈萨克斯坦已开始减产。

**标签**: `#oil logistics`, `#chokepoints`, `#Bab el-Mandeb`, `#Houthi blockade`, `#energy markets`

---

<a id="item-finance-news-8"></a>
### [IEA：东南亚电网投资到 2050 年需增至近四倍](https://oilprice.com/Energy/Energy-General/IEA-Southeast-Asia-Needs-Grid-Investment-to-Nearly-Quadruple-by-2050.html) ⭐️ 7.0/10

国际能源署（IEA）表示，按各国已宣布的气候承诺，东南亚电网和储能投资须从目前的约 130 亿美元增至 2050 年的约 500 亿美元，以支持可再生能源增长和电力需求上升。该地区可再生能源装机容量 2024 年为 120 吉瓦，按当前政策到 2035 年预计接近三倍。

rss · OilPrice.com · 8月22日 15:00

**「背景」** 东南亚占全球人口约 9%、全球 GDP 约 4%，但在当前政策下到 2035 年将贡献全球能源需求增长的近 20%；其电网老化且扩容滞后，已成为可再生能源并网的瓶颈。

**「影响」** 电网投资不足可能延缓新可再生能源项目接入，削弱投资者信心，进而影响东南亚减排目标和电力供应安全。

**标签**: `#IEA`, `#Southeast Asia`, `#grid investment`, `#renewable energy`, `#energy transition`

---

<a id="item-finance-news-9"></a>
### [罗斯百货与 TJX 同店销售额增长分化](https://finance.yahoo.com/markets/stocks/articles/ross-stores-grew-comparable-sales-204301377.html) ⭐️ 7.0/10

罗斯百货公布同店销售额增长 10%，超过 TJX 的 4%；尽管两家折扣零售商均实现增长，但两只股票中只有一只上涨。

openbb · NVDA · 8月22日 20:43

**「背景」** 罗斯百货（Ross Stores）与 TJX 同属“折价零售”行业，主要低价销售品牌尾货。同店销售额指开业至少一年门店的销售额变化，是衡量零售商业绩的重要指标。本季罗斯百货同店销售额增长 10%，并预计下一季度增长 6%至 7%；TJX 增长 4%，预计下一季度增长 2%至 3%，其中旗舰部门接近持平。

**「影响」** 投资者当天给予 Ross Stores 约 8%的股价涨幅，而 TJX 仅上涨约 1%，表明市场更看重 Ross 更高的同店销售增速及其给出的 6%至 7%的下一季度增长指引。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/22/ross-stores-grew-comparable-sales-10-tjx-grew-4-only-one-stock-went-up/">Ross Stores Grew Comparable Sales 10%. TJX Grew 4%. Only One Stock Went Up. | The Motley Fool</a></li>
<li><a href="https://www.pymnts.com/news/retail/2026/off-price-retailer-ross-stores-seizes-mainstream-market-share/">Off-Price Retailer Ross Stores Seizes Mainstream Market Share | PYMNTS.com</a></li>
<li><a href="https://www.fool.com/investing/2026/08/22/ross-stores-grew-comparable-sales-10-tjx-grew-4-only-one-stock-went-up/">Ross Stores Grew Comparable Sales 10%. TJX Grew 4%. Only One Stock Went Up. | The Motley Fool</a></li>
<li><a href="https://247wallst.com/investing/2026/08/21/ross-jumps-8-on-10-comp-growth-tjx-ticks-up-macys-edges-higher/">Ross Jumps 8% on 10% Comp Growth, TJX Ticks Up, Macy&#x27;s Edges Higher - 24/7 Wall St.</a></li>
<li><a href="https://www.aol.com/articles/ross-jumps-8-10-comp-133357000.html">Ross Jumps 8% on 10% Comp Growth, TJX Ticks Up, Macy’s Edges Higher - AOL</a></li>

</ul>
</details>

**标签**: `#retail`, `#comparable sales`, `#earnings`, `#consumer discretionary`, `#Ross Stores`, `#TJX`

---

<a id="item-finance-news-10"></a>
### [伯克希尔·哈撒韦对一家大型银行进行 16 亿美元投资动作](https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-berkshire-makes-1-000300036.html) ⭐️ 7.0/10

沃伦·巴菲特旗下伯克希尔·哈撒韦对一家大型银行执行了 16 亿美元的投资动作；目前尚不清楚具体银行名称以及是买入还是卖出。

openbb · BRK-B · 8月22日 00:03

**「背景」** 伯克希尔·哈撒韦是沃伦·巴菲特的投资公司，他曾用十多年时间建立对美国银行（Bank of America）的大额持股，并将其视为标志性持仓。最新的 13F 监管申报文件显示，伯克希尔正在减持这部分银行股份。

**「影响」** 伯克希尔·哈撒韦在最新监管申报文件（13F）中显示卖出约 16 亿美元的美国银行股份；该行曾是其长期标志性金融持股。由于伯克希尔的仓位变化常被市场关注，这一减持可能令投资者加强对大型银行股前景的谨慎判断；不过伯克希尔仍持有美国运通等金融股的大额仓位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-berkshire-makes-1-000300036.html">Warren Buffett&#x27;s Berkshire makes $1.6 billion move on major bank</a></li>
<li><a href="https://www.thestreet.com/investing/stocks/bac-bank-of-america-stock-berkshire-hathaway-sells-16-billion-stake">Warren Buffett&#x27;s Berkshire makes $1.6 billion move on major bank - TheStreet</a></li>
<li><a href="https://www.nationalmortgagenews.com/news/will-berkshire-stay-in-bank-stocks-after-buffetts-exit">Will Berkshire stay in bank stocks after Buffett&#x27;s exit? | National Mortgage News</a></li>

</ul>
</details>

**标签**: `#Berkshire Hathaway`, `#Warren Buffett`, `#banking`, `#investment`, `#capital allocation`

---

<a id="item-finance-news-11"></a>
### [道琼斯期货显示市场反弹，英伟达财报与加拿大新关税成焦点](https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-market-rally-nvidia-crowdstrike-warsh/?src=A00220&amp;yptr=yahoo) ⭐️ 7.0/10

道琼斯指数期货显示市场出现反弹，投资者同时等待英伟达即将发布的财报，并关注美国对加拿大实施的新关税。

openbb · GC=F · 8月22日 15:25

**「背景」** 美国已对来自墨西哥、加拿大和中国的商品加征关税，加拿大总理批评此举并预告报复；税务基金会估计这些关税长期将使美国 GDP 减少约 0.4%。同时，英伟达（Nvidia）即将公布财报，市场关注其数据中心收入及对华 H20 芯片出口前景。

**「影响」** 据外媒报道，美国股市期货周四早盘上涨，尤其是纳斯达克期货，原因是联邦法院阻止了特朗普的新关税，且英伟达财报表现强劲，给相关市场投资者带来一定缓解；不过股指期货已从高位回落。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.sky.com/story/donald-trump-confirms-mexico-and-canada-tariffs-sending-financial-markets-reeling-13321044">Canadian PM criticises Trump over tariffs - and sends... | Sky News</a></li>
<li><a href="https://taxfoundation.org/research/federal-tax/trump-tariffs-trade-war/">Trump Tariffs Tracker: Rates, Revenue, and Impact | 2026 Tariffs</a></li>
<li><a href="https://au.finance.yahoo.com/news/nvidia-earnings-live-stock-falls-on-data-center-revenue-miss-also-snowflake-pops-crowdstrike-drops-202724450.html">Nvidia earnings live: Stock falls on data center revenue miss.</a></li>
<li><a href="https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-nvidia-earnings-court-blocks-trump-tariffs/">Dow Jones Futures Rise As Court Blocks Trump Tariffs ; Nvidia ...</a></li>

</ul>
</details>

**标签**: `#market futures`, `#tariffs`, `#Nvidia`, `#trade policy`, `#stock market`

---

<a id="item-finance-news-12"></a>
### [美国财政部意外回购国债 债券市场影响受关注](https://news.google.com/rss/articles/CBMilgFBVV95cUxPUVJ6bXhzRjhidmNacEdxUTU1dTZ1X0lCZ2VITXJsbEpnQlVMX3dBNE5VdHpTRVBvalNZLUZKZ1c3X19ySVQtQWdsOVM5TW5pdW9FejFLUC1rN1J4V1hCc0ExRnV5MndzOThHS2phSVJjM2VBSkUya0ZVbm16Q1FneHJUWEZ1a2Uxb1VFcmItYmxRMUJQUGc?oc=5) ⭐️ 7.0/10

美国财政部出人意料地宣布回购国债，即从市场买回部分未到期债券。外交关系委员会（CFR）的分析认为，这一举动可能反映出债券市场流动性和供需压力，并可能影响后续美债发行与收益率走势。

google\_news · Council on Foreign Relations · 8月20日 16:30

**「背景」** 美国财政部近期扩大国债回购，表明其愿意并有能力主动干预以管理收益率；国债回购是美国和海外多年用来确保市场流动性、管理现金流的常用工具之一。

**「影响」** 美国财政部长贝森特宣布将部分期限至少 10 年的国债回购规模至少翻倍至 40 亿美元后，长期国债收益率一度下行，比特币等风险资产短线走高；但一些分析师认为，相对于整体国债市场，这一规模仍是“杯水车薪”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cfr.org/articles/what-the-treasurys-buyback-surprise-says-about-the-bond-market">What the Treasury ’s Buyback Surprise Says About the Bond Market</a></li>
<li><a href="https://en.cryptonomist.ch/2026/08/20/treasury-bond-buyback-impact/">Treasury Bond Buyback Impact Drives Bitcoin Surge</a></li>
<li><a href="https://www.politico.com/news/2026/08/19/treasury-buy-back-debt-bond-market-pain-01041461">‘Drop in the bucket’: Why Wall Street will shrug off Bessent’s bond ...</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-19/us-treasury-to-double-sizes-of-some-debt-buyback-operations-to-at-least-4-billion">Treasury Secretary Bessent Doubles US Long- Bond Buybacks in the...</a></li>

</ul>
</details>

**标签**: `#Treasury`, `#bond market`, `#debt management`, `#monetary policy`, `#market impact`

---