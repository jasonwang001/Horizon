---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 235 条内容中筛选出 27 条重要资讯。

---

**科技新闻**
1. [GLM-5.3 涌现网络攻击能力](#item-tech-news-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B：本地推理强的开源模型](#item-tech-news-2) ⭐️ 8.0/10
3. [把 Doom 渲染器编译成 210 亿参数 Transformer](#item-tech-news-3) ⭐️ 8.0/10
4. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-tech-news-4) ⭐️ 8.0/10
5. [PostgreSQL 发布高危 to\_char 漏洞修复，可致任意代码执行](#item-tech-news-5) ⭐️ 8.0/10
6. [Opus 5 为何让人感觉更难用？](#item-tech-news-6) ⭐️ 7.0/10
7. [谷歌宣称同态加密让私有 AI 更实用，但质疑声不断](#item-tech-news-7) ⭐️ 7.0/10
8. [Firefox 成为仍支持 uBlock Origin 的唯一主流浏览器](#item-tech-news-8) ⭐️ 7.0/10
9. [不分类，先幻觉：用嵌入映射标签](#item-tech-news-9) ⭐️ 7.0/10
10. [肿瘤 AI 临床阈值评估：开源 Python 库与无代码仪表盘](#item-tech-news-10) ⭐️ 7.0/10
11. [torch-preflight：PyTorch 静态检查器，提前发现训练错误并估算显存](#item-tech-news-11) ⭐️ 7.0/10
12. [AI 机器人实验室年测 300 万人体组织，有望替代动物测试](#item-tech-news-12) ⭐️ 7.0/10
13. [美国法官责令谷歌一周内移除第三方应用商店安装障碍](#item-tech-news-13) ⭐️ 7.0/10
14. [苹果联手阿里自研中国专属 AI 大模型](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [霍尔木兹遇袭推涨油价：布伦特逼近 100 美元](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储以 9 比 3 投票维持利率不变](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储维持利率不变，暗示未来可能加息](#item-finance-news-3) ⭐️ 9.0/10
4. [美联储维持利率不变并倾向未来加息以遏制通胀](#item-finance-news-4) ⭐️ 9.0/10
5. [伯克希尔增持谷歌母公司 Alphabet 至第三大持仓，加码达美航空和住房板块](#item-finance-news-5) ⭐️ 8.0/10
6. [高盛在 AI 基建融资热潮中扮演关键角色](#item-finance-news-6) ⭐️ 8.0/10
7. [盘前：Reddit 大涨 12%将入标普 500，应用材料财报后下跌](#item-finance-news-7) ⭐️ 8.0/10
8. [哈萨克斯坦指控卡沙甘项目大型油企涉 107 亿美元腐败](#item-finance-news-8) ⭐️ 8.0/10
9. [伊朗经济在战争与制裁压力下濒临崩溃](#item-finance-news-9) ⭐️ 8.0/10
10. [霍尔木兹危机促使亚洲炼油商转向美国原油](#item-finance-news-10) ⭐️ 8.0/10
11. [美联储维持利率不变 主席沃什召开记者会](#item-finance-news-11) ⭐️ 8.0/10
12. [美联储 7 月会议决定维持利率不变](#item-finance-news-12) ⭐️ 8.0/10
13. [苹果提出 App Store 外部购买抽成方案，最高 15%](#item-finance-news-13) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GLM-5.3 涌现网络攻击能力](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.AI 发布了新前沿编码模型 GLM-5.3，宣称具备新兴网络能力，可自主进行安全研究并规模化披露漏洞。该模型基于 GLM 5.2 经后训练增强，社区用户报告其能够在红队场景中执行 WordPress 插件 0day 利用、远程代码执行和 6.8 内核漏洞适配等任务。Z.AI 还运行着活跃的 CVE 披露项目（cvd.z.ai），对大量流行软件进行扫描，并在保密期内披露漏洞。该公告被视为 AI 在软件工程与网络安全领域可能带来行业变化的进展。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**「背景」** GLM-5.3 是智谱（Z.AI）于 2026 年 8 月 14 日发布的前沿编码模型，它与 GLM-5.2 使用相同的基础模型，所有能力提升均来自规模化的后训练（post-training）。官方称其编码能力较 GLM-5.2 提升 50%，在 Terminal-Bench 3.0 和 Agents&\#x27; Last Exam \(CLI\) 等基准上取得开源模型最优结果。该模型还展现出“涌现”的网络安全能力，包括自主安全研究和漏洞披露，相关 CVE 披露项目位于 cvd.z.ai。Z.AI 将其定位为面向智能体工程（Agentic Engineering）的新一代基础模型，强调在复杂系统工程和长程智能体任务中的可靠性。

**「影响」** 早期采用者已将 GLM 官方订阅接入 Claude Code 并立即升级到更高付费档位，说明该模型已可实际用于安全研究类工作；同时其规模化漏洞扫描可能重塑 OSS 漏洞披露生态，但也引发对扫描成本与披露是否充分的讨论。

**「社区讨论」** 社区整体反应积极，有用户认为其能力接近 Sol 和 Fable，并称赞 Z.AI 公告更接近研究者写作而非营销宣传；但也有一些讨论指出 Mythos 5 在 181 和 247 个任务上仍领先，且对规模化漏洞扫描的成本效益和披露流程存疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5">GLM-5 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber ...</a></li>

</ul>
</details>

**标签**: `#GLM`, `#large language models`, `#cybersecurity`, `#AI coding`, `#vulnerability discovery`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B：本地推理强的开源模型](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B 是一个新的开源权重本地语言模型，凭借其推理性能和本地 AI 工作流集成受到关注。社区测试显示，它是继 Gemma 4 之后第二个能正确通过某用户私有基准的本地模型，但完成时消耗了约 5 倍的 token，并在启用 MTP 的情况下耗时 12 分 30 秒；用户还观察到它的推理痕迹更显式，而显存使用效率似乎不如 Gemma 4 或 Glimmer。另有用户展示它在笔记本上画出结构合理的“骑自行车鹈鹕”，认为这是本地模型罕见的绘图表现。模型也引发了关于如何在使用 Ollama 时关闭思考模式、以及思考痕迹风格是否影响 MTP 预测的讨论。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**「背景信息」** Qwen 3.8-27B 是阿里巴巴于 2026 年 8 月 14 日发布的开源权重模型，采用 Apache-2.0 许可。它是一款 270 亿参数的原生视觉-语言模型，原生上下文长度达 262,144 个 token，默认开启思考模式，并提供 reasoning\_effort 调节参数。该模型属于 Qwen 3 系列的重要更新，主打更高的智能密度，并面向本地部署场景。

**「影响」** 对于通过 Ollama 使用该模型的开发者，默认思考模式可能无法直接关闭，需要借助第三方模板（如 Qwen-F）来减少或关闭思考、修正工具调用并维持 KV 缓存命中率；这一额外配置成本可能影响其作为本地模型的部署体验。

**「社区讨论」** 社区普遍认可其推理和绘图能力，有用户称它是继 Gemma 4 之后第二个通过私有基准的本地模型，也有用户展示它画出的高质量鹈鹕骑自行车图；同时，一些用户指出它思考痕迹更“电报体”、显存使用效率较低，并询问在 Ollama 中关闭思考的方法。另有观点怀疑这种独特的思考痕迹模式可能影响 MTP 预测效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=Fvg8659WQDg">Qwen - 3 . 8 - 27 B Released : Everything you need to Know... - YouTube</a></li>
<li><a href="https://qwen3lm.com/">Qwen AI for Everyone | Qwen 3 , Qwen Studio &amp; Model</a></li>

</ul>
</details>

**标签**: `#llm`, `#open-source`, `#local-models`, `#reasoning`, `#qwen`

---

<a id="item-tech-news-3"></a>
### [把 Doom 渲染器编译成 210 亿参数 Transformer](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

作者用自研编译器将 Doom 渲染算法转换为一个约 210 亿参数的 Transformer 检查点，没有经过任何训练。该检查点是标准 Transformers 格式，可直接在 Hugging Face 加载；输入场景数据后，模型输出包含像素绘制命令的 token 序列，按命令执行即可还原 E1M1 画面。单帧需要 3,614 个输入 token 和 53,747 个生成 token，在 B200 上约需 40 分钟，而原版 Doom 在 486 上可达 35 FPS，这里约为每天 35 帧。项目展示了一种通过编译器把真实算法映射进 Transformer 权重的路线，对机制可解释性和权重工程有潜在意义，但目前只是概念验证。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**「背景」** 该项目的核心背景是作者此前开发的一种编译器，它能把计算图直接转换为 transformer 的权重，完全不需要训练；作者此前已用这种方法把四个精确计算器编译进 transformer。本次作品则将 Doom 的经典渲染算法移植成这种编译器可处理的计算图，并编译为一个基于标准 Phi-3 架构、可通过 Hugging Face 加载的 21B 参数检查点。在生成时，模型以场景数据为提示，自回归输出包含移动光标、绘制像素等指令的 token 序列，机械地执行这些指令即可还原出 E1M1 画面。

**「影响」** 该项目的直接意义是证明了无需训练即可将确定性算法编译为 Transformer 权重，但当前生成速度远低于原生渲染，尚不构成实用替代方案，主要影响限于对 Transformer 内部机制和人工权重设计的研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ood.dev/posts/doom/">Doom, compiled into a transformer — Out of Distribution</a></li>
<li><a href="https://ood.dev/posts/calculator/">A calculator, compiled into a transformer — Out of Distribution</a></li>

</ul>
</details>

**标签**: `#transformer`, `#mechanistic interpretability`, `#compiler`, `#program synthesis`, `#neural rendering`

---

<a id="item-tech-news-4"></a>
### [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室正式开源 dots3-note preview，这是 dots3 系列第一个开放权重模型。该模型总参数为 280B，每次推理仅激活 16B 参数，支持长达 512K 的上下文，并能够处理文字、图片、视频和音频等多模态输入。模型引入了名为 TEMPO 的强化学习方法，通过自批判和测试时价值估计来训练长程智能体，相关权重已发布到 Hugging Face。同时，团队还发布了 VibeSearchBench 和 VibeLifeBench 两个真实场景智能体基准，用于评估模型在搜索与生活场景中的智能体能力。

telegram · zaihuapd · 8月14日 08:27

**「背景」** 混合专家（MoE）模型将总参数划分为多个专家子网络，推理时只激活其中一部分，因此能用较少计算成本获得大模型容量；dots3-note preview 总参数量 280B、激活参数仅 16B，正属于这一架构。小红书 dots 实验室此前并未发布开放权重模型，此次是 dots3 系列首个开放权重版本，已在 Hugging Face 开源，并支持最多 512K 令牌的上下文和文本、图像、视频、音频等多模态输入。TEMPO 是该模型配套的强化学习方法，用于训练长程智能体任务。

**「影响」** 开发者可以基于这组开源权重和 TEMPO 方法构建长程、多模态智能体应用，同时借助 16B 激活参数显著降低推理成本。两个新基准也将为智能体模型的能力评测提供更贴近实际场景的参考标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260814/2348931.html">小红书开源 dots3-note，280B MoE 仅 16B 激活参数 - 禁闻网</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>

</ul>
</details>

**标签**: `#open-source`, `#Mixture-of-Experts`, `#multimodal`, `#reinforcement-learning`, `#agents`

---

<a id="item-tech-news-5"></a>
### [PostgreSQL 发布高危 to\_char 漏洞修复，可致任意代码执行](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 项目披露并修复了高危漏洞 CVE-2026-14669，该漏洞位于 to\_char\(timestamptz\) 函数处理超长 POSIX 时区缩写的过程中，可触发堆缓冲区溢出。CVSS 评分为 8.8，能够设置时区的低权限数据库用户可利用该漏洞以 PostgreSQL 服务进程的操作系统权限执行任意代码，但攻击并非无需认证。受影响版本包括 18.5、17.11、16.15、15.19 和 14.24 之前的版本；由于 18.5 因回归问题未正式发布，18 系列用户应升级到 18.6，其他用户应分别升级到 17.11、16.15、15.19 或 14.24。此次小版本更新不需要转储数据库或运行 pg\_upgrade，只需更新程序文件并重启服务即可完成修复。

telegram · zaihuapd · 8月14日 14:35

**「背景」** to\_char\(timestamptz\) 是 PostgreSQL 将带时区时间戳格式化为字符串的函数，会解析 POSIX 时区缩写以构造输出。CVE-2026-14669 属于堆缓冲区溢出，即程序在处理超长输入时越界写入堆内存，攻击者可以借此覆盖内存并劫持执行流程。

**「影响」** 受影响版本的所有 PostgreSQL 实例都应尽快应用各自对应的小版本更新，否则拥有低权限数据库账户的攻击者可能完全控制数据库服务进程并读取或篡改数据。

**标签**: `#PostgreSQL`, `#CVE`, `#security`, `#database`, `#vulnerability`

---

<a id="item-tech-news-6"></a>
### [Opus 5 为何让人感觉更难用？](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

一篇技术分析文章认为，Opus 5 之所以让人感觉更难用，主要在于其“省略式、面向智能体”的交流风格：句子绕开要点、把真实动作像揭示悬念一样放在句尾，并大量使用无生命名词作主语来变换动词。社区讨论进一步印证了这种感受，用户抱怨它说话过于抽象、冗长，不断“承认错误”和“坦诚”，甚至会偏离严格指令；有用户因此退回 4.8，也有人转向 OpenAI 的 Sol。真正的问题可能不是能力下降，而是模型的后训练目标已从服务人类转向服务其他智能体，导致人类体验被忽视。该讨论反映 LLM 交互设计中“人类是否仍是目标受众”的关切。

hackernews · numeri · 8月14日 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**「背景」** Claude Opus 5 是 Anthropic 于 2026 年 7 月发布的旗舰模型，定位为面向长期、多步骤任务的强智能体编码模型，相比 Opus 4.8 在深度推理、智能体任务和测试时计算扩展上提升显著。此次讨论并非针对模型能力，而是关注其沟通风格：评论者认为 Opus 5 的写作过于省略、抽象，并倾向于将人类用户当作非主要受众，转向面向智能体（agent-speak）的表达方式。

**「影响」** 对重度依赖 Claude 的开发者来说，Opus 5 的沟通风格会增加阅读和纠正成本，部分用户已明确选择回退旧版本或切换到 OpenAI Sol。

**「社区讨论」** 评论普遍认同作者判断，认为 Opus 5 更擅长但不讨喜，典型表现包括省略式表述、过度“坦诚”和跑题；有用户晒出实例，并有人将原因归结为模型在向“智能体语言”倾斜。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/whats-new-opus-5">What&#x27;s new in Claude Opus 5 - Claude Platform Docs</a></li>

</ul>
</details>

**标签**: `#AI`, `#machine learning`, `#human-computer interaction`, `#LLM`, `#software engineering`

---

<a id="item-tech-news-7"></a>
### [谷歌宣称同态加密让私有 AI 更实用，但质疑声不断](https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/) ⭐️ 7.0/10

谷歌在官方博客中宣布，正在通过同态加密技术让私有 AI 变得更加实用，旨在于加密状态下执行机器学习推理，从而保护用户数据隐私。这一进展被视为隐私保护机器学习领域的重要信号，但技术上的实际开销和商业可行性仍是关键问题。社区评论普遍指出，同态加密及其他隐私保护技术在当前推理任务上的开销可能高达约 10^3 倍，使其难以大规模商业化。此外，谷歌自身在隐私保护方面的记录（如密码管理器默认未启用端到端加密）也引发了不少质疑。总体而言，该公告展示了技术方向，但距离真正可落地的私有 AI 仍面临显著挑战。

hackernews · u1hcw9nx · 8月14日 15:43 · [社区讨论](https://news.ycombinator.com/item?id=49300314)

**「背景」** 同态加密（HE）允许在加密数据上直接进行计算而无需解密，从而使“加密安全的私有 AI 推理”成为可能——模型可以处理加密输入，服务提供商无需接触用户原始数据。完全同态加密（FHE）长期以来因巨大的计算开销（通常超过 1000 倍）而难以实用。Google 的 HEIR（同态加密中间表示）是一个开源编译器工具链和开发平台，能够将原本处理未加密数据的预训练 AI 模型转换为可处理加密输入，从而降低这一技术在实际应用中的门槛。

**「影响」** 对 AI 与安全领域的从业者而言，谷歌的声明意味着科技巨头仍在持续投入隐私保护机器学习，但同态加密的高昂计算与能源开销很可能继续限制其在现实商业场景中的采用，短期难以改变现有云 AI 服务的隐私模式。

**「社区讨论」** 评论中既有对同态加密实际开销的质疑（一位用户称其毕业论文研究显示推理开销约 1000 倍，商业可行性低），也有对谷歌自身隐私立场的讽刺，认为谷歌在匿名化访问方面并不友好。另有评论指出，最私密的 AI 是运行在用户自己硬件上的本地模型，而非依赖云数据中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/">How Google is Making Private AI Practical with Homomorphic ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49300314">Google Is Making Private AI Practical with Homomorphic Encryption</a></li>
<li><a href="https://www.linkedin.com/pulse/homomorphic-encryption-secure-computation-unlocking-agjzf">Homomorphic Encryption for Secure Computation: Unlocking the...</a></li>

</ul>
</details>

**标签**: `#homomorphic encryption`, `#privacy-preserving ML`, `#AI`, `#Google`, `#security`

---

<a id="item-tech-news-8"></a>
### [Firefox 成为仍支持 uBlock Origin 的唯一主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 7.0/10

由于 Chrome 的 Manifest V3 改动，uBlock Origin 所依赖的旧版扩展接口被逐步移除，Firefox 现在成为唯一仍支持完整版 uBlock Origin 的主流浏览器。Firefox 保留了相关扩展 API，并且 Mozilla 会对 uBlock Origin 等热门扩展的每次更新进行安全审查，以确认没有恶意代码。对用户和开发者来说，要继续使用完整广告拦截功能就需要转向 Firefox，而 Chrome 及多数基于 Chromium 的浏览器只能使用功能受限的替代方案。这一变化再次凸显了浏览器厂商限制与广告拦截扩展之间的持续矛盾。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**「背景」** Manifest V3 是谷歌为 Chrome 扩展制定的新规范，逐步限制了拦截网络请求所需的底层 API 能力。uBlock Origin 这类完整广告拦截扩展依赖旧版 Manifest V2 的接口，因此无法在 Chrome 中继续完整运行；据相关介绍，谷歌的 Manifest V3 变更到 2025 年 6 月全面生效，Chrome 用户只能改用精简版的 uBlock Origin Lite，或使用 Firefox、Brave 等仍支持完整扩展的浏览器。

**「影响」** 最直接的后果是，依赖 uBlock Origin 完整广告拦截能力的 Chrome 用户需要改用 Firefox，或接受替代扩展在过滤能力上的限制。

**「社区讨论」** 社区评论整体支持 Firefox，并批评 Google/Chrome 的 Manifest V3 限制了扩展自由度；有评论指出 Chrome 仍可通过本地加载未打包扩展来手动安装 uBlock Origin，但过程繁琐。另有开发者表示 Manifest V3 导致其关闭 Sitetruth 和 Ad Limiter，并认为移除 Google 搜索广告目前只能在 Firefox 中实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/zhangwei42/ublock-origin-in-chrome-navigating-the-new-manifest-v3-landscape-3ca3">uBlock Origin in Chrome: Navigating the New Manifest V3 ...</a></li>
<li><a href="https://ublockorigin.com/">uBlock Origin - Free, open-source ad blocker extension</a></li>

</ul>
</details>

**标签**: `#Firefox`, `#uBlock Origin`, `#Manifest V3`, `#ad blocking`, `#browser extensions`

---

<a id="item-tech-news-9"></a>
### [不分类，先幻觉：用嵌入映射标签](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Simon Willison 介绍了 Doug Turnbull 提出的一种内容打标方法：不让 LLM 直接在大规模标签集中做分类，而是让模型先“幻觉”出全新的、不存在的标签，再通过向量嵌入在已有标签库中寻找最接近的真实标签。Willison 指出自己的博客有 1,856 个标签，数量太多无法一次性交给 LLM 并让其选择匹配项，而这一方案正好解决了此类大标签词表的分类难题。Turnbull 的示例提示词会给出标签形态样例，例如“Furniture / Living Room Furniture / Coffee Tables &amp; End Tables / Coffee Tables”，并让模型为查询“brown coffee table”生成新颖分类。该技术结合了 LLM 的生成能力与向量搜索的相似度匹配，适用于需要处理海量标签或分类体系的内容自动标注场景。

rss · Simon Willison · 8月14日 21:54

**「背景」** 在标签数量很大的情况下，直接让大语言模型从整个词汇表中选择合适标签既消耗大量 token，也不够可靠。Doug Turnbull 提出的一种模式是先让模型自由生成可能合理的“虚构”标签，再借助向量嵌入（embeddings）将这些虚构标签与现有标签库中语义最接近的真实标签做匹配。这种方法与“假设文档嵌入”（hypothetical document embeddings）相关，本质上是用较小的 LLM 降低分类成本，同时让结果能落回真实的分类体系。

**「影响」** 拥有大规模标签库或商品分类体系的博客、电商和内容平台，可以在不重新训练模型或穷举所有标签的情况下，用这种方法自动为旧内容或新查询生成合理标签，降低人工标注成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://softwaredoug.com/blog/2026/08/10/hypothetical-classifications">Don&#x27;t classify. Hallucinate!</a></li>
<li><a href="https://www.linkedin.com/posts/softwaredoug_dont-classify-hallucinate-activity-7492683478216560640-0xCh">Don’t classify. Hallucinate! | Doug Turnbull - LinkedIn</a></li>
<li><a href="https://hitreader.com/post/dont-classifyhallucinate-then-match-a-cheaper-way-to-hit-your-real-taxonomy/">Don’t Classify—Hallucinate, Then Match with Embeddings</a></li>

</ul>
</details>

**标签**: `#LLM`, `#embeddings`, `#content tagging`, `#vector search`, `#AI`

---

<a id="item-tech-news-10"></a>
### [肿瘤 AI 临床阈值评估：开源 Python 库与无代码仪表盘](https://www.reddit.com/r/MachineLearning/comments/1vod2c8/opensource_python_library_nocode_web_dashboard/) ⭐️ 7.0/10

开发者发布了开源的 Python 库 oncothresh 及配套无代码网页仪表盘 oncothresh-web，用于在临床决策阈值上评估肿瘤 AI 模型，而非仅依赖 AUC、ICC、MAE 等全局指标。该库在指定截断值上计算敏感性、特异性、阳性预测值、阴性预测值，并提供 Bootstrap 置信区间、阈值敏感性曲线、边界加权校准、决策曲线净收益和所需检测数等指标。其依赖精简，基于 numpy、scipy、scikit-learn 和 pydantic，适用于肿瘤细胞百分比、Ki-67、TMB 和 PD-L1 评分等连续输出转二分类决策的任务。当前版本为 v0.1，可通过 Docker Compose 本地运行网页仪表盘，上传 CSV 即可生成图表和 PDF 报告。

reddit · r/MachineLearning · /u/adom2989 · 8月14日 17:06

**「背景」** 传统上的肿瘤 AI 模型评价常用 AUC、ICC、MAE 等指标衡量整体一致性，但这些指标无法回答临床最关注的问题：在决定患者是否需要标记、活检或治疗的具体阈值上，模型是否可靠。oncothresh 填补了病理基础模型基准如 PathBench 和 PathBench-MIL 未覆盖的空白——它们只在全局评估，不提供预定义临床阈值下的性能与不确定性量化。

**「影响」** 对从事肿瘤 AI 模型开发和临床转化的研究人员而言，oncothresh 提供了一种轻量、可复现的方式将模型性能直接落到临床决策点并附带不确定性估计。不过由于仍是 v0.1 早期版本，实际使用前需谨慎验证其数学实现和 API 适用性。

**标签**: `#oncology AI`, `#model evaluation`, `#clinical decision thresholds`, `#open-source`, `#Python`

---

<a id="item-tech-news-11"></a>
### [torch-preflight：PyTorch 静态检查器，提前发现训练错误并估算显存](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 7.0/10

torch-preflight 是一个面向 PyTorch 的静态 linter，通过读取代码来捕获常见的训练错误，例如 losses.append\(loss\) 导致每个 step 保留 autograd 图直至显存耗尽、训练循环中缺少 zero\_grad\(\)、梯度累积未除以 loss，以及使用 DDP 但未配合 DistributedSampler 导致每个 rank 训练相同批次。该工具目前包含 13 条规则，并且不会导入或执行用户代码，因此不需要 GPU 或安装 torch。它还能在运行前估算训练脚本在指定 GPU 上的显存占用，并给出可让运行适配的修改建议及每项修改节省的 GiB。作者称显存估算结果与实际测量峰值相差约 4%，但该结论仅基于四款模型和一张 T4 GPU。项目可通过 pip install torch-preflight 安装，代码仓库位于 highwaterlabs/torch-preflight，PyPI 页面也已上线。

reddit · r/MachineLearning · /u/LeJanbandhu · 8月14日 14:30

**「背景」** PyTorch 训练中许多耗时且昂贵的失败来自 autograd 图保留、梯度未清零、数据并行采样错误等可静态检测的问题，等到运行后才暴露往往浪费大量 GPU 时间。torch-preflight 采用静态分析手段，在代码运行之前扫描 PyTorch 源码中的潜在 bug，同时通过静态估算模型显存占用，帮助开发者在租用实例前判断训练任务是否能够正常执行。

**「影响」** 这个工具可以让 PyTorch 开发者减少因常见训练错误导致的失败任务和 GPU 费用浪费，并在购买或租用 GPU 实例前更准确地评估显存需求。不过作者也承认目前验证规模有限（四个模型、一张 T4），且 linter 的误报率仍是其需要关注的主要问题，实际效果需在更多代码库上检验。

**标签**: `#PyTorch`, `#linter`, `#ML tooling`, `#debugging`, `#GPU memory`

---

<a id="item-tech-news-12"></a>
### [AI 机器人实验室年测 300 万人体组织，有望替代动物测试](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

生物技术公司 Vivodyne 在旧金山南部部署了 12 个“蜂巢”机器人实验室，利用 AI 设计实验并在培养的人体组织上每年开展超过 300 万次受控试验，这一容量是美国全部临床试验总和的两倍。该系统旨在通过更接近人体的组织模型预测新药疗效与安全性，从而有望淘汰动物测试。目前约 90%的临床试验在通过动物测试后仍以失败告终，凸显该技术的潜在价值。

telegram · zaihuapd · 8月14日 01:48

**「背景」** 传统药物研发通常先在动物身上测试，但约 90%的候选药物在后续人体临床试验中仍告失败，部分原因是动物模型无法准确反映人体反应。Vivodyne 是一家生物技术公司，致力于用自主机器人平台和人工智能大规模培养功能性人体组织，并在芯片上构建肿瘤微环境等模型，用于药物筛选和免疫疗法测试。该公司于 2025 年 5 月宣布获得 4000 万美元融资，目标是让不准确的动物测试过时，并将临床失败率从 95%降至更低。

**「影响」** 对药物研发和生物技术行业而言，该技术可能显著减少对动物测试的依赖，并提高新药进入临床前的预测准确性，但大规模替代仍需验证和监管认可。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://www.vivodyne.com/human-tissues">Human Tissues - vivodyne.com</a></li>
<li><a href="https://www.businesswire.com/news/home/20250528498236/en/Vivodyne-to-Replace-Animal-Testing-With-$40-Million-Funding-to-Reverse-95-Clinical-Trial-Failure-Rate">Vivodyne to Replace Animal Testing With $40 Million Funding ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#biotech`, `#robotics`, `#drug discovery`, `#animal testing`

---

<a id="item-tech-news-13"></a>
### [美国法官责令谷歌一周内移除第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

美国地区法官 James Donato 下令谷歌简化竞品安卓应用商店的安装流程，删除 Play Store 中的多余步骤与警告弹窗。法院认定这些“查看”后才出现“安装”等多步操作是蓄意制造的“反竞争摩擦”，用于吓退普通用户。谷歌须在一周内完成修改，让安装第三方市场像安装普通安卓应用一样直接。该指令源自 Epic 诉谷歌反垄断案，此前陪审团裁定谷歌在安卓应用分发上构成非法垄断。

telegram · zaihuapd · 8月14日 09:55

**「背景」** Epic 诉谷歌反垄断案源于《堡垒之夜》开发商 Epic Games 对谷歌应用分发和支付政策的挑战。陪审团此前认定谷歌在安卓应用分发市场拥有非法垄断地位，而本项命令则是该案后续救济措施的一部分，针对 Play Store 中阻碍用户安装第三方应用商店的警告和额外步骤。

**「影响」** 这一裁决将降低用户安装 Epic Games Store 等第三方应用商店的阻力，可能加剧安卓应用分发渠道的竞争，并促使谷歌调整其平台治理方式。

**标签**: `#Android`, `#antitrust`, `#Google`, `#app stores`, `#regulation`

---

<a id="item-tech-news-14"></a>
### [苹果联手阿里自研中国专属 AI 大模型](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

苹果已专门为中国市场训练一款大语言模型，并获得阿里巴巴支持，取代此前依赖第三方模型的策略。Apple Intelligence 预计将在未来数月随 iOS 更新在中国上线，中国网信办已于上月备案其生成式 AI 服务。若落地，苹果或将成为首个获北京批准在华提供自有 AI 模型的外国公司。此举使苹果能更好地掌控中国市场的 AI 体验，并顺应监管要求。

telegram · zaihuapd · 8月14日 14:47

**「背景信息」** Apple Intelligence 是苹果推出的生成式 AI 功能套件，计划随 iOS 更新在中国上线。由于中国对生成式 AI 服务实行备案与安全评估，外国公司需获得批准后才能提供自有模型。此前苹果计划通过与阿里巴巴合作、在其设备中整合通义千问（Qwen）模型来满足要求，本轮报道则称苹果改为专门为中国市场训练自研大模型，并继续获得阿里巴巴支持。

**「影响」** 中国网信办已于 2026 年 7 月 15 日备案苹果 Apple Intelligence，为苹果在中国大陆 iPhone 上提供自研 AI 清除了主要监管障碍，使其成为首个获准在华提供自有生成式 AI 模型的外国公司；合作方还包括阿里巴巴与百度，分别参与大模型与搜索服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-14/exclusive-apple-trains-its-own-ai-model-for-china-market-with-alibabas-support-sources-say">Exclusive-Apple Trains Its Own AI Model for China Market With ...</a></li>
<li><a href="https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/">EXCLUSIVE: Apple trains its own AI model for China market ...</a></li>
<li><a href="https://www.digitaltrends.com/phones/china-approves-apple-intelligence-for-iphones-with-alibaba-baidu-emerging-as-partners/">China approves Apple Intelligence for iPhones, with Alibaba ...</a></li>
<li><a href="https://www.techtimes.com/articles/320811/20260717/apple-intelligence-wins-china-approval-after-22-months-qwen-handles-language-baidu-handles-search.htm">Apple Intelligence Wins China Approval After 22 Months: Qwen ...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Large Language Models`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [霍尔木兹遇袭推涨油价：布伦特逼近 100 美元](https://oilprice.com/Energy/Crude-Oil/Hormuz-Attacks-Push-Oil-Toward-100-Despite-US-Crude-Build.html) ⭐️ 9.0/10

霍尔木兹海峡航运遇袭和美国与伊朗谈判陷入僵局，推动 ICE 布伦特原油本周料上涨约 5%，现报每桶 88 美元；若袭击继续，价格可能逼近 100 美元。美国原油库存意外增加 1700 万桶，仅部分抵消看涨情绪。

rss · OilPrice.com · 8月14日 16:21

**「背景」** 美国对伊朗原油实施海上封锁，伊朗则袭击通过霍尔木兹海峡的船只；该海峡是全球重要石油运输通道。

**「影响」** 能源进口国和航运、化肥、食品行业首当其冲；国际能源署\(IEA\)预计 2026 年全球供应每日减少 430 万桶，第三季度缺口达 180 万桶/日，且乌克兰 8 月谷物出口受黑海袭击影响同比大降 76%，加剧全球粮食供应担忧。

**标签**: `#oil prices`, `#geopolitics`, `#Hormuz`, `#energy supply`, `#OPEC`

---

<a id="item-finance-news-2"></a>
### [美联储以 9 比 3 投票维持利率不变](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

美联储（美国中央银行）以 9 比 3 的投票结果决定维持利率不变，显示货币政策决策层内部存在分歧。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储的联邦公开市场委员会\(FOMC\)以 9 比 3 投票决定维持联邦基金利率在 3.5%至 3.75%不变，这一利率水平自 1 月以来一直保持。投反对票的三名委员主张加息，反映出对通胀持续高于 2%目标的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#FOMC`, `#central bank`

---

<a id="item-finance-news-3"></a>
### [美联储维持利率不变，暗示未来可能加息](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

据 CBS News 报道，美联储在最新一次政策会议上维持利率不变，同时暗示未来仍可能加息。

google\_news · CBS News · 6月17日 07:00

**「背景」** 美联储联邦公开市场委员会（FOMC）在周三决定维持基准利率不变，但近半政策制定者表示支持今年晚些时候加息。基准利率影响整个经济的借贷成本，而当前通胀回升是这一讨论的背景。

**「影响」** 如果通胀继续加速，美联储可能在后续会议加息，这将推高抵押贷款、车贷等消费借贷成本，影响家庭和企业借款人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door open to hike - CBS News</a></li>
<li><a href="https://www.detroitnews.com/story/business/2026/04/27/fed-likely-to-hold-rates-steady-as-powell-nears-possible-swan-song/89818844007/">Fed likely to hold rates steady as Powell nears possible swan song</a></li>
<li><a href="https://www.shortform.com/podcast/episode/money-rehab-with-nicole-lapin-2026-06-03-episode-summary-how-the-upcoming-fed-meeting-will-impact-your-wallet">How The Upcoming Fed Meeting Will Impact Your Wallet Podcast...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-4"></a>
### [美联储维持利率不变并倾向未来加息以遏制通胀](https://news.google.com/rss/articles/CBMiiAFBVV95cUxOWlo2eWRfMHQzRGk2MTdTdkR4R3FLWHlxWjdRekZCOWRhWk42ajJxamdDcmZlbER4TzVxZlFMa0F5d0wycHVMejh1Qk1vTGtWQW1qV05HdXp6ZFFOd3FEOXdaRmw5ZC1HdDd6WGl1Q3NnOS0xc3Y0YUdyQ3htLUlzTVJqRG9oalZM?oc=5) ⭐️ 9.0/10

美联储宣布维持利率不变，同时释放未来可能继续加息的信号，以对抗持续的通胀压力。这一决定反映其货币政策仍以控制通胀为优先目标。

google\_news · The New York Times · 6月17日 07:00

**「背景」** 美联储在 2026 年 7 月将基准利率维持在 3.50%–3.75%不变，此前这一年里利率一直未作调整。由于通胀仍明显高于美联储 2%的目标，市场已押注 2026 年晚些时候可能加息。

**「影响」** 如果美联储如信号所示在未来加息，抵押贷款、信用卡等消费信贷成本将上升，进一步加重家庭和企业的融资负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Federal Reserve Holds Rates at 3.50%-3.75% in July 2026 | U.S. Bank</a></li>
<li><a href="https://www.cnbc.com/2026/08/10/fed-rate-hike-prospects-higher-interest-rates.html">Fed rate hike prospects: What higher interest rates mean for your money</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>
<li><a href="https://www.cnbc.com/2026/08/10/fed-rate-hike-prospects-higher-interest-rates.html">Fed rate hike prospects: What higher interest rates mean for your money</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`

---

<a id="item-finance-news-5"></a>
### [伯克希尔增持谷歌母公司 Alphabet 至第三大持仓，加码达美航空和住房板块](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 8.0/10

伯克希尔哈撒韦第二季度监管文件显示，其将 Alphabet（谷歌母公司）持仓提高 83%，使该股以 379 亿美元市值成为第三大美股持仓；同时增持达美航空 44%，并转为近 200 亿美元的股票净买家。

rss · CNBC Finance · 8月14日 21:06

**「背景」** 大幅增持主要源于 6 月初 Alphabet 为人工智能基础设施建设融资而进行的 100 亿美元私募配售。此前伯克希尔已连续 14 个季度净卖出股票，当季现金从创纪录的 3974 亿美元降至 3655 亿美元。

**标签**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#homebuilders`, `#equity investing`

---

<a id="item-finance-news-6"></a>
### [高盛在 AI 基建融资热潮中扮演关键角色](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 8.0/10

高盛正通过为 AI 基础设施相关交易提供融资服务获取丰厚费用：英伟达宣布高盛等六家机构将共同筹资 5000 亿美元，英特尔股票发行规模从 150 亿美元提高至 200 亿美元，高盛担任联席账簿管理人。

rss · CNBC Finance · 8月14日 20:05

**「背景」** AI 基础设施建设需要巨额资金，大型银行凭借承销和融资能力成为重要中介；此前高盛还参与了 Alphabet 总额 850 亿美元的股票发行。

**「影响」** 这些交易可为高盛带来承销费、买卖价差和佣金收入，但英伟达计划仅为不具约束力的谅解备忘录，细节尚未公布，实际收益仍不确定。

**标签**: `#Goldman Sachs`, `#AI infrastructure`, `#Nvidia`, `#Intel`, `#equity offering`

---

<a id="item-finance-news-7"></a>
### [盘前：Reddit 大涨 12%将入标普 500，应用材料财报后下跌](https://www.cnbc.com/2026/08/14/stocks-making-the-biggest-moves-premarket-rddt-amat-sndk-w.html) ⭐️ 8.0/10

Reddit 盘前大涨 12%，因标普道琼斯指数公司宣布其将于 8 月 18 日加入标普 500 指数并取代 AvalonBay Communities。应用材料盘前跌超 5%，其第二财季调整后每股收益为 3.50 美元、营收为 91.2 亿美元，关键半导体系统部门营收 70.4 亿美元仅略高于分析师预期的 69.6 亿美元；Wayfair、福克斯、闪迪和 Workday 也走高，分别受到券商上调评级或收购传闻推动。

rss · CNBC Finance · 8月14日 10:46

**「背景」** 这些变动发生在 8 月 14 日美股盘前交易时段，即常规交易开始前的买卖阶段。

**标签**: `#S&amp;P 500`, `#Earnings`, `#M&amp;A`, `#Stock Upgrades`, `#Premarket`

---

<a id="item-finance-news-8"></a>
### [哈萨克斯坦指控卡沙甘项目大型油企涉 107 亿美元腐败](https://oilprice.com/Latest-Energy-News/World-News/Kazakhstan-Accuses-Big-Oil-of-107-Billion-Corruption-in-Kashagan-Oil-Project.html) ⭐️ 8.0/10

哈萨克斯坦在一桩保密仲裁案中指控，开发卡沙甘油田的国际大型油企通过不正当提价或贿赂，授予了价值 107 亿美元的合同。据调查新闻国际联盟（ICIJ）援引消息人士报道，这一腐败指控是其针对大型油企合计 160 亿美元索赔案的一部分，仲裁庭尚未作出裁定。

rss · OilPrice.com · 8月14日 14:30

**「背景」** 卡沙甘油田由 North Caspian Project 财团开发，股东包括 KazMunayGas、Eni、Shell、ExxonMobil、TotalEnergies、CNPC 和 INPEX。该指控已提交海牙常设仲裁法院，是哈萨克斯坦与财团多年争端中最严重的指控；纠纷还涉及成本超支、项目延误和环境损害。

**「影响」** 因多年争端，壳牌已暂停在哈萨克斯坦的新投资；其 CEO 称在政府与合资伙伴未能对齐之前，公司会观望。

**标签**: `#corruption`, `#oil industry`, `#Kazakhstan`, `#arbitration`, `#Big Oil`

---

<a id="item-finance-news-9"></a>
### [伊朗经济在战争与制裁压力下濒临崩溃](https://oilprice.com/Geopolitics/Middle-East/Irans-Economy-Is-Buckling-Under-the-Weight-of-War.html) ⭐️ 8.0/10

国际货币基金组织预测，伊朗今年整体通胀率将接近 69%，为 1979 年伊斯兰革命以来最高；连续五个月的战争、美国制裁和海上封锁正推高基本食品价格，伊朗家庭约 70%的收入用于购买食品。

rss · OilPrice.com · 8月14日 14:00

**「背景」** 多年国际制裁和政府管理不善已削弱伊朗经济；去年 12 月，高通胀和货币贬值已引发全国抗议。美国还通过海军封锁和制裁阻断伊朗石油出口这一主要收入来源。

**「影响」** 约 9000 万伊朗民众正面临购买力下降和必需品短缺；随着政府削减补贴，基本物资短缺可能进一步恶化。

**标签**: `#Iran economy`, `#inflation`, `#sanctions`, `#war`, `#oil blockade`

---

<a id="item-finance-news-10"></a>
### [霍尔木兹危机促使亚洲炼油商转向美国原油](https://oilprice.com/Latest-Energy-News/World-News/Hormuz-Crisis-Pushes-Asian-Refiners-Toward-US-Oil.html) ⭐️ 8.0/10

霍尔木兹海峡持续受阻之际，多家亚洲炼油商本周购入美国原油，以替代可能无法运出的中东原油。据路透社贸易消息人士，韩国 GS Caltex 以每桶较迪拜基准溢价 13-14 美元购入 200 万桶 Mars 原油，日本 Eneos 以每桶较 WTI 溢价逾 10 美元购入 200 万桶 WTI 原油；台湾 CPC 及日本 Cosmo 等也有采购。

rss · OilPrice.com · 8月14日 12:30

**「背景」** 霍尔木兹海峡是伊朗与阿曼之间的狭窄航道，全球约 20%的石油经此运输。2026 年 2 月 28 日美国与以色列对伊朗开战后，该海峡被封锁，导致中东原油出口受阻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Strait_of_Hormuz_crisis">2026 Strait of Hormuz crisis - Wikipedia</a></li>
<li><a href="https://research.cashugroup.com/research-reports/hormuz-chokepoint-oil-markets-crisis">Hormuz Chokepoint Crisis — Oil Supply Disruption Analysis ...</a></li>
<li><a href="https://www.dallasfed.org/research/economics/2026/0320">What the closure of the Strait of Hormuz means for the global ...</a></li>

</ul>
</details>

**标签**: `#Oil markets`, `#Strait of Hormuz`, `#Asian refiners`, `#US crude`, `#Geopolitics`

---

<a id="item-finance-news-11"></a>
### [美联储维持利率不变 主席沃什召开记者会](https://news.google.com/rss/articles/CBMivgFBVV95cUxNR1BZa2dPa1lOcjNBSmF2MHFHcTNBTV9mQzZOZ3BzR1ZrekhVWUhzLWszajBVWExhYWxJUWJDejh4SjBTdFdobFk1Y1NlMEpad0I4cUtrY0o1VzhMYmNOX2tuWjF3dXhGbkFVOWJncnZDdEt2dUEydkhhX2pwQXZlaF96QTZ3Z2l3OURfN2lLaVRRcEFLejhVTGZVSEl4XzJLWmE0RmxKRy16Mkh2ZGJvbm0wMUExTU83dHVJUlRn0gHDAUFVX3lxTE9kWHZBeUc3cjFTeGNrQk5QeGl2cHpycW5zR19kQl9vbEY3MzdUX0ZCa2pmV0RNT1VSUElKTEhhNmRmaVVnc1k5R0V2RkhTYkJROUZ3YXZmVjlPSWZ5MWVTWkxYS1B3ai1BZnRVeTE5bmR6Mm01eHlDYlpJblAta3hYSnN5Tnhzc19ZRjJwUWVTZzNRQXd0MUJGU29NRko2aVVuTTByMndYeWU3bTRXNWpEeFBlVDF5RTBUU1VaQUdlT1RlRQ?oc=5) ⭐️ 8.0/10

据 PBS 报道，美联储在最新会议上决定维持利率不变，美联储主席沃什随后举行新闻发布会说明这一决定。

google\_news · PBS · 7月29日 07:00

**「背景」** 美联储新任主席凯文·沃什主持了其第二次利率会议，会议决定维持基准利率不变，但有三名官员反对并主张加息，显示决策层在通胀压力下存在分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-warsh-holds-news-conference-after-latest-interest-rate-decision">WATCH: Fed chair Warsh holds news conference after ... - PBS</a></li>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-new-fed-chair-kevin-warsh-holds-first-news-conference-after-interest-rate-decision">WATCH: New Fed chair Kevin Warsh holds first news conference ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/kevin-warsh-fed-treasury-yields-inflation-credibility-interest-rates.html">Fed&#x27;s Warsh&#x27;s credibility in question after rate decision ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#news conference`, `#economy`

---

<a id="item-finance-news-12"></a>
### [美联储 7 月会议决定维持利率不变](https://news.google.com/rss/articles/CBMiiwFBVV95cUxNUVVUMW1Hb2g1N2cyQkJneFl4YXJ1aFVvOGQzX19Oc2IxZUFyVUcwOXI0VmlpaW04d0N0MWZxVFlhSkJLUTltY3VxOVVHVGFBZHc5eVRzUTRQN1FXSEQ1Qm16U1pJMC1rOHNSdFd6UTEyWTF4cUpjX3NJUGs1alI3VGtLSmdNZmpOdjM0?oc=5) ⭐️ 8.0/10

据《财富》报道，美联储在 7 月会议后决定维持利率不变。

google\_news · Fortune · 7月29日 07:00

**「背景」** 美联储在 7 月会议上决定维持利率不变，将联邦基金利率目标区间保持在 3.5%至 3.75%。这一决定并非一致通过，且声明未包含前瞻指引，令市场对 9 月会议缺乏明确预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady</a></li>
<li><a href="https://www.usatoday.com/story/money/economy/2026/07/29/fed-meeting-live-july-interest-rates--live/91061021007/">It wasn&#x27;t unanimous, but the Fed continued its pause on interest rates</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#economy`

---

<a id="item-finance-news-13"></a>
### [苹果提出 App Store 外部购买抽成方案，最高 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

苹果已向法院提交美国 App Store 外部购买抽成方案：标准应用抽成 15%，视频、新闻等合作项目及订阅续费抽成 10%，小型企业计划应用抽成 5%。这些数字是苹果的提案，仍需法院后续审理。

telegram · zaihuapd · 8月14日 02:33

**「背景」** 这是苹果与 Epic Games 诉讼的一部分；美国最高法院此前驳回了苹果暂停下级法院费率审理的请求。Epic 将有机会回应，苹果预计在 9 月 14 日前向最高法院提交书面意见。

**标签**: `#Apple`, `#App Store`, `#commission fees`, `#regulation`, `#Epic Games`

---