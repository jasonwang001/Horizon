---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 247 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [Shopify 从 React Native 转向 Swift 与 Kotlin 原生开发](#item-tech-news-1) ⭐️ 8.0/10
2. [微软将 Rust 列为一级语言](#item-tech-news-2) ⭐️ 8.0/10
3. [Calif Research 称借 AI 九天造出 WeChat 零点击蠕虫](#item-tech-news-3) ⭐️ 8.0/10
4. [trynix.dev 让任意 Nix 包在浏览器中启动](#item-tech-news-4) ⭐️ 7.0/10
5. [果蝇连接组子图学 Pong 失败，审计更有价值](#item-tech-news-5) ⭐️ 7.0/10
6. [蚂蚁国际与 Visa、Mastercard 合作开发 AI 支付标准](#item-tech-news-6) ⭐️ 7.0/10
7. [腾讯混元开源音频编辑模型 AuK](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [IEA：霍尔木兹海峡 LNG 受阻推高气价，2026 年全球煤炭需求预计创 89.4 亿吨纪录](#item-finance-news-1) ⭐️ 8.0/10
2. [美联储以 9 比 3 投票维持利率不变](#item-finance-news-2) ⭐️ 8.0/10
3. [Kalshi 获 CFTC 批准推出黄金、白银永续期货](#item-finance-news-3) ⭐️ 7.0/10
4. [美国 30 亿美元扶持关键矿产，分析称仍难撼动中国主导地位](#item-finance-news-4) ⭐️ 7.0/10
5. [墨西哥计划将对 Pemex 的财政支持削减约 70%](#item-finance-news-5) ⭐️ 7.0/10
6. [EIA 预测美国天然气产量、消费和 LNG 出口到 2027 年连创纪录](#item-finance-news-6) ⭐️ 7.0/10
7. [二叠纪盆地天然气价格年内 118 天为负](#item-finance-news-7) ⭐️ 7.0/10
8. [印度严重欺诈调查局建议详查小米在印业务](#item-finance-news-8) ⭐️ 7.0/10
9. [HBM 短缺推高中国 AI 芯片价格，华为、寒武纪上调报价](#item-finance-news-9) ⭐️ 7.0/10
10. [TSMC Stock Slips Despite 53% August Revenue Growth](#item-finance-news-10) ⭐️ 7.0/10
11. [台积电 9 月营收据报道大增 53%，需求超出现有供应](#item-finance-news-11) ⭐️ 7.0/10
12. [OpenAI 选择博通开发其首款定制 AI 芯片](#item-finance-news-12) ⭐️ 7.0/10
13. [特朗普据报称对伊朗战争不后悔，油价突破 100 美元](#item-finance-news-13) ⭐️ 7.0/10
14. [美债抛售持续，10 年期国债收益率逼近 5%](#item-finance-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Shopify 从 React Native 转向 Swift 与 Kotlin 原生开发](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 工程团队介绍，公司将移动端从 React Native 迁移回原生 Swift 与 Kotlin，回退此前的跨平台路线。该动向被视为一家大型公司对跨平台与原生移动开发取舍的重要工程战略调整，并引发 Hacker News 上关于 React Native、原生工程师价值及 LLM 辅助迁移的广泛讨论。由于提供的来源正文缺失，迁移范围、时间表、性能数据和具体技术限制无法从现有材料中核实。来源作者 fnthawar2 在讨论中表示，LLM 改变了其 2020 年决策背后的一个核心假设，因此重新评估原路线；评论者则对 LLM 是否为该迁移的决定性因素存在分歧。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**「背景」** React Native 是 Meta 主导的跨平台移动开发框架，允许用共享的 JavaScript 代码库同时构建 iOS 与 Android 应用，Shopify 在 2020 年正是基于这一思路采用它，以减少分别维护两套原生代码的成本。据 Shopify 工程博客，编码智能体（coding agents）改变了构建移动应用的成本结构，使公司重新评估这一核心假设，并决定把所有移动应用迁回 Swift 与 Kotlin 原生开发。其中 Shop 应用已从概念验证到发布在 12 周内完成迁移。

**「影响」** 对正在评估跨平台策略的移动团队而言，这一案例可能推动其重新计算 React Native 与原生 Swift/Kotlin 的长期维护和招聘成本，但评论中的经验表明收益与可行性取决于应用规模和团队能力。

**「社区讨论」** 评论总体偏向认可离开 React Native，但围绕 LLM 是否让原本过于昂贵的迁移变得可行存在明显分歧：有评论者称用 Codex 在一夜之间为 15–20 个屏幕的小型应用生成 Android 与 iOS 版本，另有评论者表示其参与的中型 React Native 应用迁移到 Swift/Kotlin 的大部分工作发生在 2026 年 1 月前且未使用 LLM 代码辅助。也有观点认为 RN 原本的吸引力是用 Web 开发者兼顾移动端，适合初创阶段，但随着模型生成原生代码能力增强，其优势正在缩小，平台仍需要专门的 native 工程师。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://shopify.engineering/shop-app-migration">Migrating Shop app from React Native to native (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding Agents Made It Cheaper to Build Twice Than to Share One Codebase. - DEV Community</a></li>

</ul>
</details>

**标签**: `#React Native`, `#mobile development`, `#Swift/Kotlin`, `#engineering strategy`, `#LLM-assisted migration`

---

<a id="item-tech-news-2"></a>
### [微软将 Rust 列为一级语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Rust 基金会的一篇客座文章称，Rust 已成为微软的 Tier 1 语言。这一认定被视为 Rust 在系统编程与开源生态中获得重要行业采用的信号。该文章属于基金会客座内容，并非微软的工程深度说明或主要工程公告，因此具体支持范围、时间表和技术条件在现有材料中仍不明确。Hacker News 上该话题获得 590 分和 331 条评论，讨论集中在 Rust 的成熟度、迁移规模及与其他语言的比较。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**「背景」** Rust 于 2015 年 5 月发布首个稳定版 1.0，并自 2021 年 2 月起由 Rust Foundation 赞助，此后在 Web 服务和系统软件等领域被广泛采用。微软的相关文章指出，其原生平台会同时演进对 Rust 与 C++ 的支持；Rust 已成为微软的 Tier-1 语言，但经过数十年发展的 C++ 仍占据主导。围绕这一身份，社区也关注配套工具链，例如 Hacker News 上有人追问 Visual Studio 何时能提供 Tier-1 级别的调试支持。

**「影响」** 对微软内部开发者与依赖 Windows/MSVC 工具链的系统开发者而言，Rust 成为 tier-1 语言意味着它将获得贯穿获取、工具链、质量、安全、平台集成、生产部署和长期支持的持续投入，从而降低在大型代码库中采用与维护 Rust 的迁移风险。不过，该消息源自 Rust 基金会客座文章而非微软的工程公告，具体落地范围和节奏仍待官方细节确认。

**「社区讨论」** 评论整体上把这视为 Rust 成熟度和行业采用的重要验证：一位写了五年专业 Rust 的开发者称，在高层应用开发中已看不到其他语言的技术理由，但 WASM 与原生 UI 支持仍是限制其全栈使用的现实条件。讨论还提到微软到 2030 年转换 10 亿行代码的自动化目标、DARPA 的多团队 C 到 Rust 转换工作、MSVC 集成传闻、微软产品 CVE 中约 70% 与内存安全相关，以及与 Zig/Odin 的成熟度对比；这些评论中的数字、计划与集成消息未在原文中得到验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rust_%28programming_language%29">Rust (programming language ) - Wikipedia</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post : Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643546">Rust Is Tier - 1 Language at Microsoft | Hacker News</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#programming languages`, `#open source`, `#systems programming`

---

<a id="item-tech-news-3"></a>
### [Calif Research 称借 AI 九天造出 WeChat 零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 8.0/10

Simon Willison 在其博客中引用 Calif Research 的声明：该团队发布了 WeWorm 演示，称这是首个通过 WeChat 通话在 iOS 与 Android 之间传播的零点击蠕虫。按帖子描述，受害者无需接听电话，甚至完全不必操作手机；即便接听，听不到任何声音，利用仍然成功。Calif Research 表示，他们借助 AI 在大约两天内找到漏洞并写出首个远程代码执行（RCE）利用，随后又用一周时间构建出蠕虫。该团队还称，这种规模的蠕虫过去往往需要更大规模的团队耗时数月，而 AI 已经能完成其中大部分工作，人类团队主要负责选择目标以及安全测试方式的判断。所引内容仅为一段引文式帖子，未提供技术细节、方法论或独立验证，相关说法仍属未经证实。

rss · Simon Willison · 9月10日 00:56

**「背景说明」** 零点击漏洞指攻击者无需受害者接听、点击或进行任何操作即可完成入侵；蠕虫则指攻击得手后能自动从一台设备或账号传播到下一台。Calif Research 称，WeWorm 通过微信通话传播，可劫持账号并用受害者的身份呼叫其好友，若被利用可能波及超过十亿部手机或账号。据 Help Net Security 报道，Calif 已发现并武器化了这一严重漏洞，并私下报告给腾讯，同时公开了演示；相关说法目前尚无独立验证。

**「影响」** 若该说法成立，WeChat 用户可能在毫无交互的情况下被攻击，同时意味着在 LLM 辅助下，漏洞利用与蠕虫开发的耗时和人力门槛被大幅拉低。不过目前仅有演示与声明，缺乏技术细节和第三方验证，实际影响范围尚不明确。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://calif.io/research/weworm">WeWorm | Calif</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://blog.calif.io/p/weworm">WeWorm</a></li>

</ul>
</details>

**标签**: `#ai-security-research`, `#exploit-development`, `#zero-click-worm`, `#llm-assisted-coding`, `#wechat`

---

<a id="item-tech-news-4"></a>
### [trynix.dev 让任意 Nix 包在浏览器中启动](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 7.0/10

Farid Zakaria 发布了 trynix.dev，他称其为自己在 Nix 工作上的“magnum opus”。该站点通过 qemu-wasm 驱动的 x86\_64 Linux 虚拟机，完全在浏览器中借助 WebAssembly 运行，并可启动过去 13 年中的任意 Nix 包。这些环境可通过 URL 直接寻址，例如访问 https://trynix.dev/?pkg=python3%403.6.2 并点击 “Load”，即可获得一个运行 2017 年 Python 3.6.2 的交互式 shell。Zakaria 还在此基础上构建了新工具 trynix-preview：这是一个 GitHub Action，会在 pull request 中评论一个链接，让评审者用 trynix.dev 在浏览器里启动该 PR 的构建，其描述是“没有服务器，只有浏览器”。

rss · Simon Willison · 9月10日 23:44

**「背景」** Nix 及其软件包集合 nixpkgs 依靠可复现构建与内容寻址的二进制缓存，使历史上发布过的包版本都能被精确重建和取用，trynix.dev 正是借 nixpkgs-multiverse 索引来提供过去 13 年的包。运行侧依赖 ktock 的 qemu-wasm：该项目为 QEMU 增加了把中间表示（IR）翻译为 WebAssembly 的 TCG 后端，并借助浏览器的 WebAssembly.Module 与 WebAssembly.Instance API 在页面内启动 x86\_64 Linux 虚拟机。界面由终端模拟器 Ghostty 提供，Nix store 保存在内存中，包文件本身则通过普通 HTTP 从 Nix 二进制缓存下载。

**「影响」** 对 Nix 用户和代码评审者而言，历史版本的软件包环境与待合并 PR 的构建结果现在可以直接在浏览器中启动和交互，无需自行准备服务器或本地虚拟机，从而降低了复现与评审验证的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trynix.dev/">trynix</a></li>
<li><a href="https://fzakaria.com/2026/09/04/any-nix-package-live-in-your-browser">Any Nix package, live in your browser | Farid Zakaria’s Blog</a></li>
<li><a href="https://techaiwire.com/articles/trynix-nix-packages-in-browser-wasm/">TryNix runs Nix packages in your browser - techaiwire.com</a></li>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#QEMU`, `#reproducible builds`, `#browser VMs`

---

<a id="item-tech-news-5"></a>
### [果蝇连接组子图学 Pong 失败，审计更有价值](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

一位 Reddit 作者报告称，他把 MaleCNS v1.0 真实 EM 重构果蝇连接组（166k 神经元）的一小段真实子图接入 Pong，用类多巴胺可塑性训练，但最终没有学会，并认为逐突触审计这次失败比成功更有信息量。审计发现：他修复了 neuPrint 正则表达式 bug（全匹配与子串语义差异），该 bug 曾静默地把两个神经元群体清零；最初选出的神经元在光感受器到其他任何神经元之间没有任何通路，因为真实光感受器并不直接突触到运动检测器，中间还有一整层缺失。开启与关闭学习后，在多个随机种子下结果逐位相同，即使权重确实在变化；原因是一共 4 个可用运动神经元中有一半在模型里与任何感觉通路都没有突触，因数组索引巧合被分到“paddle down”组，永远不可能发放。之后他改用与求偶追逐视觉目标跟踪相关的通路重建电路，该假设被数据否定，但顺着线索找到另一个端到端连通的下降神经元，首次让学习开关产生差异；不过效果看起来是学习规则让整个系统安静下来，而不是技能提升，因为 miss 多于 hit，惩罚占主导并缩小运动响应。他还指出几个流行项目也未解决该问题：Doom 项目自己的仓库称六次迭代后未通过其验证门槛，Minecraft 模组的限制说明承认真实运动检测通路保持沉默、逃跑和觅食行为是手工注入或反射层回退，Beat Saber 作者回复承认只对一首曲目过拟合并把回放数据混入输入；这是一项单次自述、未经同行评审的业余实验，没有已验证结果。

reddit · r/MachineLearning · /u/oPeraza2007 · 9月10日 02:28

**「背景」** 连接组（connectome）是通过电子显微镜重建的神经元及其突触连接图谱；本次事件涉及的 MaleCNS v1.0 来自 Janelia FlyEM 项目对果蝇雄性中枢神经系统的完整重建，并提供突触级别的连接权重表，作者使用其中约 16.6 万个神经元的一个小子图作为实验对象。研究者通常借助 neuPrint 及其 Python 客户端查询这类数据集，该接口允许用正则表达式匹配神经元的类型与实例名，而不同匹配语义（完整匹配与子串匹配）的差异正是本次审计所发现问题的一个来源。所谓多巴胺式可塑性，指用类似奖赏或惩罚的信号来调节突触权重的学习规则，作者据此让真实连接组的子图尝试通过每帧的二元命中/未命中信号来玩 Pong。

**「影响」** 对尝试基于 MaleCNS v1.0（16.6 万神经元）复现此类演示的开发者与研究者而言，这项工作表明在宣称&quot;大脑学会了玩游戏&quot;之前必须先审计数据管道与电路连通性：neuPrint 查询的全匹配与子串语义差异会静默清零整个神经元群，而经媒体广泛报道的 Doom、Minecraft 等演示项目本身也承认存在大量近似处理、结果未经其自身验证门槛，或行为实为手工注入而非涌现。不过该分析属单个自述、未经同行评审的业余实验，其负面结论仍需独立复现验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://male-cns.janelia.org/">Male CNS Connectome - MaleCNS connectome</a></li>
<li><a href="https://male-cns.janelia.org/download/">Download - MaleCNS connectome</a></li>
<li><a href="https://connectome-neuprint.github.io/neuprint-python/docs/neuroncriteria.html">NeuronCriteria — neuprint-python 0.6.2 documentation</a></li>
<li><a href="https://hothardware.com/news/google-mapped-a-fruit-fly-brain-so-engineers-taught-it-to-play-doom">Google Mapped A Fruit Fly Brain, So Engineers Taught It To Play Doom</a></li>
<li><a href="https://www.msn.com/en-us/gaming/general/google-used-ai-to-reconstruct-a-fly-brain-so-people-made-it-play-doom/ar-AA2bTTZ8">Google used AI to reconstruct a fly brain, so people made it play Doom</a></li>
<li><a href="https://github.com/evnsnclr/neurocraft-fly-public">GitHub - evnsnclr/neurocraft- fly -public: NeuroCraft Fly by Evan Sinclair...</a></li>

</ul>
</details>

**标签**: `#connectomics`, `#computational neuroscience`, `#reinforcement learning`, `#reproducibility`, `#bio-inspired AI`

---

<a id="item-tech-news-6"></a>
### [蚂蚁国际与 Visa、Mastercard 合作开发 AI 支付标准](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 7.0/10

蚂蚁国际宣布与 Visa、Mastercard 合作，为 AI 代理支付制定通用标准。三方将建立“了解你的代理”（Know Your Agent）机制，把代理与有效实体关联，评估其行为并监测风险，以提升不同支付系统之间的互操作性和安全性。三方援引麦肯锡预测称，到 2030 年 AI 代理可能处理全球消费者商业交易中的 3 万亿至 5 万亿美元。目前该合作仍处于标准制定阶段，尚未公布具体技术规范或已落地实施的标准。

telegram · zaihuapd · 9月10日 03:00

**「背景」** AI 代理支付指让 AI 代理代表用户完成交易；要让这类支付在不同支付系统之间互操作，首先需要确认代理身份及其授权范围。中国金融科技公司蚂蚁国际与卡组织 Visa、Mastercard 提出的“了解你的代理”（KYA）机制，正是把传统 KYC 思路延伸到 AI 代理，通过关联代理与有效实体、评估行为并监测风险来建立信任。三方于 2026 年 9 月 10 日在圣保罗宣布了 KYA 互操作性框架，其背景是 AI 代理协议碎片化、跨系统执行存在摩擦。

**「影响」** 对 AI 代理开发者和商户而言，若这一通用标准落地，代理可能须先完成注册、与有效实体关联并取得限定权限的凭证，才能接入 Visa、Mastercard 等网络发起支付，从而抬高代理支付的准入门槛。目前三方仅宣布合作制定标准，尚无已实施标准的确认，具体合规要求与时间表仍不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html">Ant International, Visa and Mastercard team up on AI payment standard</a></li>
<li><a href="https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/">Ant International, Visa, and Mastercard Agree on Agent Identity Standard. Now Comes the Hard Part. – Forkast</a></li>
<li><a href="https://www.hokanews.com/2026/09/visa-and-mastercard-back-ant.html">Visa and Mastercard Back Ant International’s ‘Know Your Agent’ Standard for AI Payments - Hokanews</a></li>
<li><a href="https://www.linkedin.com/pulse/5-ai-protocols-every-commerce-practitioner-must-know-aditya-chaudhari-sgmee">5 AI Protocols Every Commerce Practitioner Must Know for Agentic ...</a></li>

</ul>
</details>

**标签**: `#AI payments`, `#AI agents`, `#payment standards`, `#fintech`, `#Visa/Mastercard`

---

<a id="item-tech-news-7"></a>
### [腾讯混元开源音频编辑模型 AuK](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

腾讯混元宣布正式发布开源音频编辑模型 AuK，并同步推出速度更快的 AuK-Flash 变体。AuK 可通过自然语言指令与参考音频统一完成语音生成和编辑，支持零样本文本转语音、音色/风格/情绪编辑、去口音及多人语音分离等功能。AuK-Flash 采用 4 步推理，在匹配条件下速度约提升 4.5 倍。代码、模型权重和演示已上线。

telegram · zaihuapd · 9月10日 11:56

**「背景」** AuK 属于“统一语音生成与编辑”这一类语音基础模型：传统方案中，文本转语音、音色转换、语音增强与声源分离等任务通常由各自独立的模型分别处理，而 AuK 试图通过统一的自然语言指令接口把生成与编辑合并到同一模型中，用户既可用文本指令，也可用参考音频来驱动。根据公开的模型仓库与报道，AuK 是一个参数量 15 亿的基础模型，训练数据达数百万小时，包含标准版与推理更快的 AuK-Flash 两个版本。

**「影响」** 对语音工程团队而言，AuK 以 1.5B 参数的开源权重把零样本 TTS、音色/风格/情绪编辑、去口音与多人语音分离收敛到同一套「自然语言指令 + 参考音频」接口，有望减少把合成、降噪、分离、变声等分散工具逐一拼装的集成成本；AuK-Flash 的 4 步推理（匹配条件下约 4.5 倍加速）则面向更贴近实时或批量处理的场景。不过其编辑质量、稳定性和实际加速幅度仍需第三方评测验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Tencent-Hunyuan/AuK">GitHub - Tencent-Hunyuan/AuK: AuK: An Open-Source ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/tencent-open-sources-1-5b-parameter-audio-model-auk-for-voice-editing-and-generation">Tencent open-sources the 1.5-billion-parameter audio model ...</a></li>
<li><a href="https://arxiv.org/html/2609.08936v1">AuK Technical Report: An Open-Source Foundational Model for ...</a></li>
<li><a href="https://github.com/davahiatak1/AuK-tss-voice">GitHub - davahiatak1/AuK-tss-voice: AuK: An Open-Source ...</a></li>
<li><a href="https://www.aimodeling.com/en/news/slug/tencent-hunyuan-auk-speech-editing">AuK: Tencent&#x27;s Open 1.5B Speech Generation and Editing Model</a></li>

</ul>
</details>

**标签**: `#audio-editing`, `#open-source`, `#text-to-speech`, `#speech-synthesis`, `#Tencent-Hunyuan`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [IEA：霍尔木兹海峡 LNG 受阻推高气价，2026 年全球煤炭需求预计创 89.4 亿吨纪录](https://oilprice.com/Latest-Energy-News/World-News/IEA-Global-Coal-Demand-Set-to-Hit-Record-High-as-Iran-War-Chokes-LNG-Supply.html) ⭐️ 8.0/10

国际能源署（IEA）在《2026 年煤炭中期更新》报告中表示，因伊朗战争导致霍尔木兹海峡液化天然气（LNG）运输大幅减少、天然气价格走高，全球煤炭需求 2026 年预计增长 1.2%至 89.4 亿吨，创历史新高；而在战前，该机构预计今年全球煤炭需求会小幅下降。IEA 称，中国煤炭需求预计增长 1%至 50 亿吨，印度增长 4.2%至 13.53 亿吨，扭转了去年印度需求小幅下降的局面。

rss · OilPrice.com · 9月10日 14:30

**「背景」** 霍尔木兹海峡是卡塔尔、阿联酋等国液化天然气（LNG，即冷却成液态以便海运的天然气）出口的主要通道，中东战事开始六个多月来该海峡的 LNG 运输大幅受阻，推高了天然气和 LNG 价格。中东并非煤炭出口大户，因此煤炭海运本身未受直接冲击，但发电企业因气价上涨而更多启用燃煤机组——IEA 原先预计今年全球煤炭需求会小幅下降，如今改为上升 1.2%。

**「影响」** 对亚洲和欧洲的电力用户与天然气进口商而言，霍尔木兹海峡液化天然气运输受阻推高了气价，公用事业公司因此更多启用燃煤机组发电，这一转变也波及亚洲市场的电价与能源安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dinardetectives.com/iea-global-coal-demand-record-high-iran-lng/">IEA: Global Coal Demand Set for Record High</a></li>
<li><a href="https://www.linkedin.com/pulse/strait-hormuz-lng-oil-new-energy-security-shock-md-nasiruddin-evohf">Strait of Hormuz , LNG &amp; Oil | The New Energy Security Shock</a></li>
<li><a href="https://eecc.energy/insights/blog-and-updates/asias-energy-chokepoint-how-the-hormuz-disruption-is-impacting-energy-markets">Asia&#x27;s energy chokepoint: How the Hormuz disruption is ...</a></li>

</ul>
</details>

**标签**: `#IEA`, `#coal demand`, `#LNG supply`, `#Strait of Hormuz`, `#energy markets`

---

<a id="item-finance-news-2"></a>
### [美联储以 9 比 3 投票维持利率不变](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 8.0/10

据 ABC7 Los Angeles 报道，美联储以 9 比 3 的投票结果决定维持利率不变。该报道未提供当前利率水平或投票分歧的具体原因。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储的利率决定由其利率制定机构——联邦公开市场委员会（FOMC）作出，本次会议以 9 票赞成、3 票反对的结果，将联邦基金利率目标区间维持在 3.5%至 3.75%不变，这已是该委员会连续第五次会议按兵不动。据 Spectrum News 报道，这一决定是在通胀持续高企、伊朗战争推高能源价格的背景下作出的；美联社报道称，市场普遍预计美联储可能在 9 月的下次会议上加息。

**「影响」** 政策利率维持在 3.50%-3.75%区间，意味着信用卡欠款、浮动利率贷款等与美联储基准利率挂钩的借贷成本短期内不会下降，相关家庭与企业仍需承担较高利息支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrumlocalnews.com/us/snplus/business/2026/07/29/federal-reserve-interest-rate-announcement">Federal Reserve leaves interest rate unchanged - Spectrum News</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-leaves-interest-rate-unchanged-180102302.html?fr=sycsrp_catchall">Federal Reserve leaves interest rate unchanged in 9-3 vote ...</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Federal Reserve Holds Rates at 3.50%-3.75% in July 2026 | U.S ...</a></li>
<li><a href="https://marketwise.com/investing/fed-policy-decision-market-impact/">Fed Leaves Interest Rates Unchanged: How Stocks, Bonds, and ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#US economy`

---

<a id="item-finance-news-3"></a>
### [Kalshi 获 CFTC 批准推出黄金、白银永续期货](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

Kalshi 本周获得美国商品期货交易委员会（CFTC）批准，并于周四上线黄金和白银的永续期货，这是美国首个获批的非加密货币类永续合约。据该平台网站数据，自 5 月底获批推出加密货币永续期货以来，这类合约已累计成交 440 亿美元名义金额。

rss · CNBC Finance · 9月10日 14:00

**「背景」** 永续期货是没有到期日的期货式合约，通过资金费机制使其价格贴近标的资产价格，投资者无需持有实物黄金或白银。Kalshi 于 5 月底成为首家在美国境内提供加密货币永续期货的平台，而 CME 集团已起诉 CFTC，认为该机构不当批准了这类合约。

**「影响」** Kalshi 还在寻求获批与美股、工业金属铜和外汇挂钩的合约，若范围扩大，投资者可能转向此类平台，分流 CME 等传统交易所的期货业务；CNBC 报道称，CBOE 与 CME 集团股价已因这一担忧下跌。

**标签**: `#Kalshi`, `#CFTC`, `#perpetual futures`, `#gold and silver`, `#CME`

---

<a id="item-finance-news-4"></a>
### [美国 30 亿美元扶持关键矿产，分析称仍难撼动中国主导地位](https://oilprice.com/Metals/Commodities/Why-The-United-States-Belated-Critical-Minerals-Gambit-Wont-Stop-China.html) ⭐️ 7.0/10

特朗普政府宣布向美国关键矿产项目投资 30 亿美元，其中最大一笔是五角大楼战略资本办公室向电池材料初创公司 Sila Nanotechnologies 提供的 14 亿美元有条件贷款。该报道分析认为，这些联邦投资仍不足以改变中国在关键矿产开采与加工环节的主导地位。

rss · OilPrice.com · 9月10日 23:00

**「背景」** 中国依靠数十年的国家补贴、以“一带一路”为代表的基建融资以及对采矿加工环境代价的承受，目前约占全球关键矿产开采量的 60%，并承担稀土、石墨、镓等材料 90%以上的精炼和加工；据国际能源署数据，中国还生产全球 80%的电池电芯、90%以上的负极活性材料和约 85%的正极活性材料。

**「影响」** 在联邦 7500 美元电动车税收抵免被取消后，美国电动车销量 2026 年第一季度同比下降 27%，本土市场萎缩可能反过来压制 Sila 等美国电池材料企业的需求。

**标签**: `#critical minerals`, `#rare earths`, `#US-China relations`, `#supply chain`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [墨西哥计划将对 Pemex 的财政支持削减约 70%](https://oilprice.com/Energy/Energy-General/Higher-Oil-Prices-Let-Mexico-Pull-Back-Billions-in-Pemex-Support.html) ⭐️ 7.0/10

据彭博报道，墨西哥政府计划在下一财年预算中把对国有能源公司 Pemex 的财政支持削减约 70%，降至 810 亿比索（约 48 亿美元），押注油价上涨能带来约 950 亿比索（约 56 亿美元）的罕见现金盈余。不过 Pemex 今年第一季度实际净亏损 459.9 亿比索（约 26 亿美元），为 2020 年以来最差的首季表现。

rss · OilPrice.com · 9月10日 22:00

**「背景」** 墨西哥石油公司（Pemex）是墨西哥国有石油企业，长期依赖政府注资维持偿债和运营；本届政府于 2025 年 8 月公布的 2025—2035 年战略计划，已明确提出最早在 2027 年让 Pemex 逐步摆脱政府财政支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mexicobusiness.news/oilandgas/news/mexico-unveils-10-year-plan-reform-revive-pemex">Mexico Unveils 10-Year Plan to Reform, Revive PEMEX</a></li>
<li><a href="https://momentsinmexico.substack.com/p/what-is-sheinbaums-pemex-strategic-plan">What is Sheinbaum&#x27;s Strategic Plan for Pemex?</a></li>

</ul>
</details>

**标签**: `#Pemex`, `#Mexico energy policy`, `#oil prices`, `#sovereign support`, `#corporate debt`

---

<a id="item-finance-news-6"></a>
### [EIA 预测美国天然气产量、消费和 LNG 出口到 2027 年连创纪录](https://oilprice.com/Energy/Natural-Gas/US-Natural-Gas-Market-Verging-on-Record-Growth.html) ⭐️ 7.0/10

美国能源信息署（EIA）在《短期能源展望》中预测，美国天然气产量将从 2025 年的 107.6 bcfd（十亿立方英尺/日）升至 2026 年创纪录的 111.7 bcfd、2027 年 115.9 bcfd，LNG 出口将从 2025 年创纪录的 15.1 bcfd 升至 2026 年 17.4 bcfd、2027 年 18.6 bcfd，并预计国内消费也将创纪录。EY 对 30 家最大上市勘探与生产公司的研究显示，资本支出同比下降 49%、并购支出下降 70%，石油储量新增未能完全替代产量（2021 年以来首次），而天然气产量、储量和发现分别增长 18%、14%和 21%。

rss · OilPrice.com · 9月10日 19:00

**「背景」** EIA《短期能源展望》为月度供需预测，此次对 2026 年的预测高于其 8 月预估（产量 111.2 bcfd、需求 92.0 bcfd）；美国天然气库存预计在 10 月 31 日较五年同期均值高约 5%。

**「影响」** 若这些预测实现，美国天然气生产商、LNG 出口设施开发商以及电力密集的 AI 数据中心将是主要受影响方，因为电力需求、LNG 出口和 AI 相关基础设施扩张被列为支撑长期天然气需求的因素。

**标签**: `#US natural gas`, `#EIA forecasts`, `#LNG exports`, `#oil &amp; gas M&amp;A`, `#reserve replacement`

---

<a id="item-finance-news-7"></a>
### [二叠纪盆地天然气价格年内 118 天为负](https://oilprice.com/Energy/Energy-General/Permian-Gas-Has-Been-Worth-Less-Than-Nothing-for-118-Days-This-Year.html) ⭐️ 7.0/10

由于管道外输能力不足、天然气产量创下纪录，得州二叠纪盆地的 Waha 枢纽气价在今年前 131 个交易日中有 118 天为负值，意味着生产商要倒贴钱请人把气拉走。雪佛龙子公司 Energy Forge One 已于 6 月与微软签署 20 年协议，将在 Pecos 建设最高约 2.67 吉瓦的自用燃气电厂为数据中心供电，最终投资决定预计今年年底前做出、2028 年供电。

rss · OilPrice.com · 9月10日 15:00

**「背景」** 二叠纪盆地以采油为主，但油田随开采年限增加，每桶油伴生的天然气越来越多：美国能源信息署预计该地区今年天然气日均产量将达 29.2 亿立方英尺（Bcf/d），同比增长 6%，创历史新高，而附近的管道和买家都消化不了，生产商宁可贴钱处理天然气，也不愿关停真正赚钱的油井。

**「影响」** 这类不接入公共电网的“表后”自建电厂是雪佛龙、微软等项目的关键设计，也因此不受得州州长阿博特 8 月 3 日暂停新数据中心审批、并审计电网并网排队项目（约 474 吉瓦申请，而历史峰值需求约 85 吉瓦）的影响。

**标签**: `#Permian Basin`, `#Natural Gas Prices`, `#Energy Infrastructure`, `#Data Centers`

---

<a id="item-finance-news-8"></a>
### [印度严重欺诈调查局建议详查小米在印业务](https://www.zaobao.com.sg/news/china/story20260909-9652945) ⭐️ 7.0/10

印度严重欺诈调查局建议对小米在印度的业务展开详细调查，涉及商业模式、资金流向及外资法规合规情况，印度政府正在审查相关备忘录。小米回应称尚未收到通知，并强调始终遵守当地法律。

telegram · zaihuapd · 9月10日 04:09

**「背景」** 小米此前已在印度面临税务与特许权使用费支付方面的争议。据印方媒体报道，此次拟议调查还将审查其受益所有权、电商交易安排，以及对 2020 年后出台的外资法规的遵守情况。

**「影响」** 若调查推进，小米在印度的业务及其当地供应商、渠道伙伴将面临更严格的合规审查，其他在印经营的中国手机厂商也可能被更密切关注；据 Counterpoint Research 数据，小米印度市场份额已从 19%降至 13%、退居第四，2025 年印度收入 25.2 亿美元、较三年前下降 40%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.gujaratsamachar.com/news/science-technology/serious-fraud-investigation-office-recommends-detailed-probe-into-xiaomis-india-business-over-foreign-investment-compliance-68723015972">Serious Fraud Investigation Office Recommends... | Gujarat Samachar</a></li>
<li><a href="https://economictimes.indiatimes.com/industry/cons-products/electronics/indias-serious-fraud-office-recommends-detailed-probe-into-xiaomis-business-in-country/articleshow/133963640.cms">India &#x27;s Serious Fraud Office recommends &#x27;detailed&#x27; probe into...</a></li>
<li><a href="https://www.businesstoday.in/latest/corporate/story/sfio-recommends-investigation-into-xiaomis-india-business-over-alleged-irregularities-report-554432-2026-09-10">SFIO recommends investigation into Xiaomi’s India business over alleged irregularities: Report - BusinessToday</a></li>
<li><a href="https://www.firstpost.com/tech/xiaomi-probe-report-china-urges-india-to-provide-fair-just-business-environment-14044680.html">Xiaomi probe report: China urges India to &#x27;provide fair, just business environment&#x27;</a></li>
<li><a href="https://www.chinamoneynetwork.com/2026/09/09/investigation-recommended-for-xiaomis-business-in-india-amid-alleged-irregularities">Investigation Recommended for Xiaomi’s Business in India Amid Alleged Irregularities</a></li>

</ul>
</details>

**标签**: `#Xiaomi`, `#India`, `#regulatory investigation`, `#foreign exchange compliance`, `#corporate governance`

---

<a id="item-finance-news-9"></a>
### [HBM 短缺推高中国 AI 芯片价格，华为、寒武纪上调报价](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

受全球高带宽存储器（HBM）供应紧张影响，华为、寒武纪等中国 AI 芯片厂商已上调产品价格：据路透报道，华为升腾 950DT 报价较两个月前上涨约 20%—50%，部分老款芯片涨约 30%，寒武纪新一代思元 690 预计涨价约 20%—30%。HBM 主要由 SK 海力士、三星和美光供应，美国的出口限制进一步加剧了中国市场的供应压力，使 HBM 短缺成为制约国产 AI 芯片扩张的重要瓶颈。

telegram · zaihuapd · 9月10日 09:29

**「背景」** AI 芯片需要与 HBM（高带宽存储器，一种专为 AI 计算配套的高速内存）配合使用，而先进 HBM 市场主要由韩国 SK 海力士、三星和美国美光三家供应（tool-1-1）。美国的出口管制限制了中国厂商获取这些产品的渠道，因此 HBM 供应紧张成为国产 AI 芯片扩大产能的关键制约。

**「影响」** 涨价将直接抬高中国企业搭建 AI 算力基础设施的成本，从而推高训练和运行 AI 模型的开支。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-09-10/exclusive-chinas-ai-chipmakers-raise-prices-as-high-bandwidth-memory-shortage-bites">Exclusive- China &#x27;s AI Chipmakers Raise Prices as High-Bandwidth...</a></li>
<li><a href="https://www.itp.net/ai-automation/chinas-ai-chipmakers-raise-prices-as-hbm-shortage-drives-up-costs">China’s AI Chipmakers Raise Prices as HBM Shortage Drives Up Costs - ITP.net</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#HBM`, `#semiconductor supply chain`, `#China tech`, `#export controls`

---

<a id="item-finance-news-10"></a>
### [TSMC Stock Slips Despite 53% August Revenue Growth](https://finance.yahoo.com/markets/stocks/articles/tsmc-stock-slips-despite-53-122227013.html) ⭐️ 7.0/10

TSMC stock slipped even as the company reported 53% August revenue growth, a notable indicator for the semiconductor industry.

openbb · NVDA · 9月10日 12:22

**标签**: `#TSMC`, `#semiconductor industry`, `#revenue growth`, `#stock market reaction`, `#monthly revenue`

---

<a id="item-finance-news-11"></a>
### [台积电 9 月营收据报道大增 53%，需求超出现有供应](https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductor-september-revenue-surges-151224109.html) ⭐️ 7.0/10

据报道，台积电（TSMC）9 月营收增长 53%，同时这家芯片代工商表示需求超出其供应能力、无法完全满足。该报道未给出具体营收金额，也未明确 53%增幅所对应的对比基期。

openbb · NVDA · 9月10日 15:12

**「背景」** 台积电成立于 1987 年，是全球首家专业芯片代工厂：它自己不设计芯片，而是替英伟达、苹果等客户生产芯片。由于处在 AI 芯片供应链的关键环节，其月度营收被市场视为观察全球 AI 基础设施需求的先行指标。

**「影响」** 台积电产能跟不上需求，直接承压的是依赖其代工先进芯片的下游设计企业——英伟达、AMD、苹果等客户的芯片供应可能因此受限，交货周期与排产节奏受制于代工厂产能，这也被视为全球最关键供应链之一的瓶颈所在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tsmc.com/english/aboutTSMC">About TSMC - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.tsmc.com/english">Taiwan Semiconductor Manufacturing Company Limited - TSMC</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-10/tsmc-revenue-rises-53-as-ai-chip-demand-outstrips-supply">TSMC Revenue Rises 53 % as AI Chip Demand Outstrips Supply</a></li>
<li><a href="https://theboard.world/articles/geopolitics/tsmc-semiconductor-supply-chain-risk-factors/">TSMC: Semiconductor Supply Chain Risk Factors | The Board</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductors`, `#revenue growth`, `#supply constraints`, `#Taiwan`

---

<a id="item-finance-news-12"></a>
### [OpenAI 选择博通开发其首款定制 AI 芯片](https://finance.yahoo.com/technology/ai/articles/openai-picked-broadcom-first-custom-164039569.html) ⭐️ 7.0/10

OpenAI 已选择博通（Broadcom）为其开发首款定制 AI 芯片；现有报道未提供交易条款、金额或时间表等细节。相关分析认为，这对博通而言可能是一次重要的战略胜利，并可能加剧 AI 芯片市场的竞争。

openbb · NVDA · 9月10日 16:40

**「背景」** OpenAI 与博通早在 2025 年 10 月就宣布合作，由博通为其生产首批自研 AI 芯片，当时公布的目标算力规模为 10 吉瓦；2026 年 6 月，双方公布首个合作成果——名为 Jalapeño 的定制芯片，属于“推理”芯片，即专门用于运行已训练好的 AI 模型、而不是训练模型本身。

**「影响」** 据外部报道，该定制芯片针对 AI 推理场景、规模约 100 亿美元并计划 2026 年投产，若属实，将为希望降低对英伟达依赖的大型 AI 客户提供替代选项，也会让英伟达在 AI 加速器市场面对来自自研推理芯片的竞争压力；但由于原始来源未确认交易条款、时间和采购规模，实际影响仍不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/24/openai-and-broadcom-reveal-jalapeno-first-ai-chip-in-partnership.html">OpenAI and Broadcom reveal Jalapeno, first AI chip in ... - CNBC</a></li>
<li><a href="https://cybernews.com/ai-news/openai-broadcom-build-first-ai-processor-chip-deal/">OpenAI, Broadcom join forces on AI chips | Cybernews</a></li>
<li><a href="https://intellectia.ai/blog/openai-broadcom-jalapeno-ai-chip-2026">OpenAI Broadcom Jalapeno Chip : AI Hardware Revolution 2026</a></li>
<li><a href="https://www.linkedin.com/posts/auria-asadsangabi-98b608143_openai-broadcom-make-10-billion-deal-for-activity-7369854557390147584-s5wn">Broadcom and OpenAI partner on custom AI chip deal | LinkedIn</a></li>
<li><a href="https://opentools.ai/news/broadcom-and-openai-announce-landmark-dollar10-billion-deal-for-custom-ai-chips">Broadcom and OpenAI Announce Landmark $10 Billion... | OpenTools</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#Broadcom`, `#OpenAI`, `#semiconductor competition`

---

<a id="item-finance-news-13"></a>
### [特朗普据报称对伊朗战争不后悔，油价突破 100 美元](https://finance.yahoo.com/energy/articles/trump-reportedly-says-no-regrets-233654584.html) ⭐️ 7.0/10

据雅虎财经的一则标题报道，特朗普表示对伊朗战争没有后悔之意，同时油价突破每桶 100 美元，能源 ETF——美国原油基金（USO）和两倍做多原油的 UCO——随之上涨，中期选举的政治风险上升。该报道仅有标题，未确认具体日期、油价所指的是布伦特还是 WTI、以及 USO 和 UCO 的涨幅等细节。

openbb · CL=F · 9月10日 23:36

**「背景」** 美国与伊朗的军事冲突近期升级：据 CNBC 报道，伊朗为报复美方摧毁五艘伊朗油轮，向美军驻约旦基地发射导弹，能源供应受扰，成为油价上行的直接背景。USO 是追踪西德克萨斯中质原油（WTI）价格的基金，UCO 则是带杠杆的原油产品，因此油价上涨时其波动被放大。

**「影响」** 据 CNBC 转述，特朗普称油价要到中期选举之后才会回落，这意味着美国普通家庭和依赖燃油的企业在 11 月选举前可能继续承受较高的能源成本；持有 USO、UCO 等原油期货 ETF 的投资者则直接承担油价的短期波动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.msn.com/en-in/money/general/trump-reportedly-says-he-has-no-regrets-over-iran-war-even-as-oil-tops-100-uso-and-uco-jump-while-midterm-stakes-get-higher/ar-AA2bYGJc">Trump reportedly says he has no regrets over Iran war even as ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/10/iran-us-oil-hormuz-supply-trump-military-brent-wti.html">U.S. crude oil tops $100 again as market braces for ... - CNBC Oil prices climb over $100 per barrel as US war in Iran ... Oil Hits $100 a Barrel for First Time Since July as U.S. and ... Oil Price Surges Toward $100 as Markets Fail to Share Trump’s ... US oil tops $100 a barrel as Iran war rages; Donald Trump ...</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/trump-reportedly-says-oil-prices-wont-tumble-until-after-midterms-while-iran-signals-more-intense-war-uso-uco-rise/cZt7k6WRJC2">Trump Reportedly Says Oil Prices Won’t Tumble Until After Midterms ...</a></li>

</ul>
</details>

**标签**: `#oil prices`, `#Iran conflict`, `#energy ETFs`, `#geopolitical risk`, `#midterm elections`

---

<a id="item-finance-news-14"></a>
### [美债抛售持续，10 年期国债收益率逼近 5%](https://www.wsj.com/finance/investing/the-unrelenting-bond-selloff-puts-the-10-year-yield-on-the-cusp-of-5-78bfb4db?siteid=yhoof2&amp;yptr=yahoo) ⭐️ 7.0/10

《华尔街日报》报道称，持续的债券抛售使美国 10 年期国债收益率逼近 5%这一受到广泛关注的市场关口。由于仅有标题信息，目前没有该收益率的具体数值、比较基准、抛售原因或市场反应细节可作说明。

openbb · CL=F · 9月10日 23:10

**「背景」** 10 年期美国国债收益率是全球借贷成本的重要基准，房贷和企业债利率常以其为参照。据市场数据，该收益率近期一度升至约 4.79%，自 3 月初以来上涨逾 80 个基点，为 2023 年 11 月以来最高水平；另有报道称其本周上行 18 个基点，逼近 5%这一心理关口。

**「影响」** 10 年期美国国债收益率是房贷和企业长期借款的定价基准，因此其持续上行（TradingView 数据显示过去一年累计上升 13.5%）会通过再融资和新增贷款推高家庭与企业的利息负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-11/global-bond-selloff-sends-10-year-treasury-yields-to-cusp-of-5">Global Bond Selloff Sends 10 - Year Treasury Yields to... - Bloomberg</a></li>
<li><a href="https://www.ibtimes.com/higher-bond-yields-havent-broken-stock-rally-yet-wall-street-sees-5-benchmark-big-test-3807057">Higher Bond Yields Haven&#x27;t Broken The Stock Rally Yet. Wall Street ...</a></li>
<li><a href="https://www.tradingview.com/symbols/TVC-US10Y/">10 Year Treasury Yield (US10Y) Price and Chart — TradingView</a></li>

</ul>
</details>

**标签**: `#Treasury yields`, `#bonds`, `#market selloff`, `#interest rates`, `#fixed income`

---