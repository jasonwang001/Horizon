---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 206 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [Mistral 发布 3B 开源多模态审核模型 Shieldstral](#item-tech-news-1) ⭐️ 8.0/10
2. [Keyv 及关联 npm 包遭遇活跃 Shai-Hulud 供应链攻击](#item-tech-news-2) ⭐️ 8.0/10
3. [MiniMax-H3 MLX 移植：Apple Silicon 本地视频生成](#item-tech-news-3) ⭐️ 8.0/10
4. [特朗普拟禁中国光模块进口](#item-tech-news-4) ⭐️ 8.0/10
5. [我国首部 L3/L4 自动驾驶强制性国标发布，2027 年 7 月实施](#item-tech-news-5) ⭐️ 8.0/10
6. [展示：简单算法与色彩空间，生成多样化肤色](#item-tech-news-6) ⭐️ 7.0/10
7. [Waymo 在达拉斯向所有用户开放自动驾驶服务](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek V4 Flash 在单块 AMD MI300X 上运行：速度超 150 tokens/秒](#item-tech-news-8) ⭐️ 7.0/10
9. [Oxide Computer 完成 4.45 亿美元新融资](#item-tech-news-9) ⭐️ 7.0/10
10. [华为首席科学家：芯片扩展将触及物理极限](#item-tech-news-10) ⭐️ 7.0/10
11. [Cloudflare 每月 58 美元 AI 自动化漏洞赏金，弃用第三方安全工具](#item-tech-news-11) ⭐️ 7.0/10
12. [白宫开源 AI 监管急转弯，硅谷分歧加剧](#item-tech-news-12) ⭐️ 7.0/10

**财经新闻**
1. [财报引发盘前波动：卡特彼勒与 Palantir 领涨](#item-finance-news-1) ⭐️ 8.0/10
2. [谷歌被曝为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](#item-finance-news-2) ⭐️ 8.0/10
3. [宝洁同意以 38 亿美元收购 Thorne](#item-finance-news-3) ⭐️ 8.0/10
4. [中东冲突推高油价，BP 利润增长逾一倍](#item-finance-news-4) ⭐️ 8.0/10
5. [高盛交易业务有望创纪录：上季股票交易收入大增 72%](#item-finance-news-5) ⭐️ 7.0/10
6. [国家邮政局对申通快递有限公司立案调查](#item-finance-news-6) ⭐️ 7.0/10
7. [NVIDIA 宣布重大投资神秘 AI 实验室，押注超级智能](#item-finance-news-7) ⭐️ 7.0/10
8. [AMD 第二季度业绩超预期，同时披露巨额资本支出](#item-finance-news-8) ⭐️ 7.0/10
9. [利润再高也难让芯片投资者满意](#item-finance-news-9) ⭐️ 7.0/10
10. [麦当劳财报超预期但警示未来业绩](#item-finance-news-10) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Mistral 发布 3B 开源多模态审核模型 Shieldstral](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral 发布了 Shieldstral-1.0-3B，一个 3B 参数的开源权重多模态内容审核模型。该模型针对图像和文本等内容的审核设计，宣称以低成本方式实现内容审核任务，可作为第一道防线并由人工复核。它是 Mistral 近期聚焦小型、精调模型策略的一部分。模型已可在 Hugging Face 上获取，社区讨论关注其能否支持任意规则集、与 OpenAI 的 omni-moderation 对比，以及实际应用中的可靠性问题。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**「背景」** Mistral 发布了 Shieldstral，一个 3B 参数、开放权重（Apache 2.0）的多模态安全分类器。它不像传统审核模型那样记忆固定的危害类别，而是将审核政策作为输入，因此无需重新训练即可适配不同规则集。据 Mistral 称，其在文本安全基准上可与 GPT-OSS-Safeguard-20B 媲美，性能优于体积最多 7 倍的模型，并在不同政策体系的适应性评估中达到 91.3% 的 F1 分数。

**「影响」** Shieldstral 的发布为构建社交或图片分享平台的开发者提供了一个开放权重、成本较低的 3B 多模态审核方案；该模型将内容审核转化为二元问答任务，能够按不同政策进行适配，作为人工复核前的第一道防线。

**「社区讨论」** 社区评测者对模型能否在不重新训练的情况下调整审核规则范围表示好奇，担心其只是复刻大平台现有的审核风格；也有人喜欢 Mistral 转向小型精调模型的策略，认为这类模型适合做内容审核的第一道防线，但需注意非确定性能力不能完全依赖，之后仍需人工复核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://aiweekly.co/alerts/mistral-open-sources-shieldstral-a-3b-multimodal-safety-guard">Mistral open-sources Shieldstral, a 3B multimodal safety ...</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral’s Shieldstral Packs Policy-Adaptive Safety Screening ...</a></li>
<li><a href="https://cctest.ai/en/articles/shieldstral-turns-content-moderation-into-a-yes-or-no-multimodal-safety-task">Shieldstral : A 3B Adaptive Multimodal Safety Classifier - CCTest</a></li>

</ul>
</details>

**标签**: `#Mistral`, `#content moderation`, `#open-weights`, `#multimodal`, `#AI safety`

---

<a id="item-tech-news-2"></a>
### [Keyv 及关联 npm 包遭遇活跃 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

近期，一个名为“Shai-Hulud”的活跃供应链攻击攻陷了广泛使用的 npm 包 Keyv 及其关联软件包，引发依赖安全紧急关注。该攻击利用安装钩子（如 pre-install 或 post-install）注入恶意行为，并具有蠕虫式传播能力，可能窃取凭据或创建外部数据渗出仓库。由于 Keyv 被大量项目依赖，受影响的开发者应立即审查依赖树、撤回到未受影响版本，并警惕新增安装钩子的任何包。目前尚无完整修复方案，安全团队正在紧急响应，但攻击仍在进行中，清理工作可能面临持久挑战。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**「背景」** Keyv 是一个在 npm 上每周下载量约 1.27 亿次的键值存储库。这次代号为 Shai-Hulud 的供应链攻击始于攻击者劫持其维护者的 GitHub 账户，并借此发布携带凭据窃取恶意软件的更新；受影响的相关包已超过 1280 个，合计每月安装量超过 20 亿次。攻击大约发生在 2023 年 8 月 4 日，恶意代码会在 npm install 期间静默执行，窃取 GitHub、npm、AWS、Kubernetes、Vault、Slack、Stripe、SSH、VPN 等凭据。

**「影响」** 所有在 npm 项目中使用 Keyv 及相关包并安装到受影响版本的开发者都可能面临恶意代码执行、数据泄露和凭据窃取的风险，应立即核查并替换受污染版本。

**「社区讨论」** 评论者普遍认为应彻底取消或暂停安装钩子机制，并有开发者推广使用 devcontainer 以隔离依赖风险；还有人指出此类攻击会造成难以清理的多级连带破坏，同时有 OSS 检测工具可用于识别供应链攻击指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package with 127M Weekly Downloads Compromised in ...</a></li>
<li><a href="https://devops.com/fast-moving-shai-hulud-attack-infects-npm-packages-with-2-billion-monthly-downloads/">Fast-Moving Shai-Hulud Attack Infects npm Packages with 2 ...</a></li>
<li><a href="https://gbhackers.com/shai-hulud-supply-chain-attack-compromises-keyv/">Shai-Hulud Supply Chain Attack Compromises Keyv and Hundreds ...</a></li>

</ul>
</details>

**标签**: `#supply-chain-attack`, `#npm`, `#security`, `#open-source`, `#dependency-management`

---

<a id="item-tech-news-3"></a>
### [MiniMax-H3 MLX 移植：Apple Silicon 本地视频生成](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax 于两天前发布 MiniMax-H3，这是一个通用全模态生成系统，可接受文本、图像、音频和视频输入，并生成最长 15 秒、包含音频的视频片段。PipeNetwork/minimax-h3-mlx 是一个 Python 包，将该模型移植到 MLX，用于在 Apple Silicon 上运行。Simon Willison 在 M5 Max MacBook Pro 上成功运行，下载约 115 GB 的模型文件后，视频生成耗时不到 45 分钟。他得到的视频效果令人印象深刻，但由于未按提示词指南提供音频引导，生成的音频听起来像是奇怪的类似语音的噪音。该项目的运行命令和模型下载方式已在文中给出，官方提示词指南则提供了改善音频效果的建议。

rss · Simon Willison · 8月4日 19:10

**「背景」** MiniMax-H3 是 MiniMax 于近日发布的全模态生成系统，能够同时理解文本、图像、视频和音频，并根据统一输入生成最长 15 秒、带原生立体声的 2K 视频片段。PipeNetwork 的 minimax-h3-mlx 项目将其移植到 MLX 框架，使该模型可以在 Apple Silicon（如 M5 Max MacBook Pro）上本地运行。运行时需要下载约 115 GB 的模型文件，且视频生成耗时较长，作者实测接近 45 分钟。

**「影响」** Apple Silicon 用户现在可以在本地运行这一全模态视频生成模型，但需要约 115 GB 存储空间且单次生成耗时较长；要获得满意的音频效果，需严格遵循官方提示词指南。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://www.marktechpost.com/2026/08/01/minimax-releases-minimax-h3-an-omni-modal-video-model-that-generates-15-second-2k-clips-with-native-stereo-audio/">MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#omni-modal`, `#MLX`, `#MiniMax`, `#video generation`, `#Apple Silicon`

---

<a id="item-tech-news-4"></a>
### [特朗普拟禁中国光模块进口](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

据路透社援引四名知情人士消息，特朗普政府正在起草一项禁令，拟禁止进口新型中国数据中心组件，重点是光模块。美国联邦通信委员会（FCC）正推进该措施，官员希望今年内发布并生效，以保护支撑人工智能热潮的关键基础设施，防止数据窃取、恶意软件植入或服务中断。知情人士强调禁令仍可能修改或搁置；中国驻美使馆表示将对损害中国利益的行为采取一切必要措施。若禁令实施，将冲击全球光模块龙头中际旭创，其市场份额约为 27%。此前 FCC 已对中国无人机、路由器、机器人和逆变器实施类似进口限制。

telegram · zaihuapd · 8月4日 11:29

**「背景」** 光模块是数据中心内部及数据中心之间高速数据传输的关键部件，也是支撑 AI 模型训练和推理所需算力集群的重要硬件。美国联邦通信委员会（FCC）此前已对中国制造的无人机、路由器、机器人和逆变器等产品实施类似进口限制，因此本次拟议中的光模块禁令延续了美方以“国家安全”为由限制中国技术产品进入美国关键基础设施的监管路径。

**「影响」** 若禁令最终落地，全球光模块龙头中际旭创将首当其冲：该公司约占全球市场 27%的份额，且超过 90%的营收来自中国以外，对美出口受限可能带来显著收入风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/the-fcc-mulls-banning-china-sourced-optical-transceivers-threatening-innolights-27-global-market-share-as-coherent-and-lumentum-prepare-to-pounce/">The FCC Mulls Banning China-Sourced Optical Transceivers ...</a></li>
<li><a href="https://aiweekly.co/alerts/fcc-drafts-import-ban-on-chinese-data-center-transceivers">FCC Drafts Import Ban on Chinese Data-Center Transceivers</a></li>

</ul>
</details>

**标签**: `#US-China tech policy`, `#optical modules`, `#AI infrastructure`, `#hardware supply chain`, `#data centers`

---

<a id="item-tech-news-5"></a>
### [我国首部 L3/L4 自动驾驶强制性国标发布，2027 年 7 月实施](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

工业和信息化部组织制定的《智能网联汽车 自动驾驶系统安全要求》（GB 44721—2026）强制性国家标准正式发布，拟于 2027 年 7 月 1 日起实施。这是我国首部针对 L3 级有条件自动驾驶和 L4 级高度自动驾驶系统的强制性国标，适用于搭载 L3、L4 系统的 M 类（载客）和 N 类（载货）车辆，不适用于自动泊车系统。该标准是对 2024 年推荐性国标的系统性升级，从企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、多维度检验检测四个维度构建安全要求体系，要求自动驾驶系统安全水平至少达到合格且专注驾驶人的水平。这一转变意味着相关安全要求从推荐性转为强制性，为 L3/L4 级自动驾驶的产品准入与上路提供统一底线。

telegram · zaihuapd · 8月4日 13:06

**「背景」** L3 级为有条件自动驾驶，车辆在特定条件下可自主驾驶但驾驶人需随时接管；L4 级为高度自动驾驶，系统在限定场景内可独立完成驾驶任务，无需人为干预。此前我国相关安全要求仅为 2024 年发布的推荐性国标，不具有强制约束力，本次将其升级为强制性国标，为行业提供统一的最低安全门槛。

**「影响」** 对于计划量产和交付 L3/L4 级车辆的企业及自动驾驶系统供应商，该标准将从 2027 年 7 月 1 日起强制生效，相关产品必须在实施日期前达到“至少等效于合格且专注驾驶人”的安全水平，并满足四个维度的安全要求，否则可能面临准入和上路障碍。

**标签**: `#autonomous-driving`, `#regulations`, `#China`, `#standards`, `#L3-L4`

---

<a id="item-tech-news-6"></a>
### [展示：简单算法与色彩空间，生成多样化肤色](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

作者 toneyalexander 在 Hacker News 上展示了一个基于自定义色彩空间的颜色选择器和程序化生成算法，旨在为数字艺术和游戏开发项目生成多样化且合理的肤色。该算法通过函数拟合等方式构建了一个易于使用的二维色彩空间，并配有交互式演示和详细的构建原理说明。作者表示该方法可能不够严谨，但已在实际项目中证明有用，并指出了未来改进空间。项目页面提供了大量 JavaScript 实现的方程和示例。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**「背景」** 该项目旨在定义一个更便于创建包容性色彩工具的肤色色彩空间，用于角色创建器或数字艺术等场景。传统 RGB 等色彩空间难以直观生成自然且多样的肤色，作者通过分析真实皮肤颜色的分布，设计了一个自定义色彩空间及采样算法。页面还提供了颜色选择器、程序化生成算法及交互演示，以展示该空间的特性。

**「影响」** 对于数字艺术家和游戏开发者，该工具提供了一种直接可用的方法来生成肤色调色板，避免了手动挑选时容易出现的失真或单一化问题。

**「社区讨论」** 社区普遍给予好评，称赞其呈现方式巧妙，并对比了 PCA、Oklab 色彩空间以及 Pantone 肤色参考等替代方案，也有用户指出生成结果中偶尔会出现绿、蓝、紫等不自然颜色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>

</ul>
</details>

**标签**: `#color-science`, `#procedural-generation`, `#digital-art`, `#game-development`, `#javascript`

---

<a id="item-tech-news-7"></a>
### [Waymo 在达拉斯向所有用户开放自动驾驶服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo 已将其自动驾驶打车服务向达拉斯所有用户开放，扩大了无人驾驶运营范围。这一举措被视为自动驾驶汽车部署中的一个重要里程碑，尽管本质上是常规服务公告，但涉及交通运输、城市政策和人工智能系统的广泛影响。达拉斯作为美国低密度、高扩张且汽车文化浓厚的都市区，该服务的开放具有标志性意义。目前尚不清楚具体的服务区域、车队规模或运营条件，但此举表明 Waymo 正在持续推进其商业化落地。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**「背景」** Waymo 是 Alphabet 旗下的自动驾驶公司，脱胎于谷歌的自动驾驶汽车项目，目前已在美国凤凰城、旧金山湾区、洛杉矶、亚特兰大、奥斯汀和迈阿密等地向公众提供商业机器人出租车服务，截至 2025 年 12 月每周完成超过 45 万次行程。达拉斯所在的达拉斯-沃斯堡都会区是美国前五大都市区之一，但人口密度低、城市蔓延严重、公共交通稀少且高度依赖汽车；Waymo 此前在达拉斯仅提供等待名单制服务，如今已向所有人开放。此次开放是 Waymo 在美国、英国和欧洲扩大自动驾驶技术部署的最新一步。

**「影响」** 对达拉斯及周边地区的居民和游客而言，他们现在可以直接使用 Waymo 的无人驾驶打车服务，这可能改变当地的出行选择，并引发关于自动驾驶对本地经济和劳动力影响的讨论。

**「社区讨论」** 社区评论中，有用户肯定 Waymo 车辆比人类司机更安全、可预测；也有人担心收入外流，认为乘客支付的费用可能不再留在本地经济中；还有从事商业地产的用户提出，自动驾驶汽车可被视作有效的经济适用房政策工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Self-Driving_Car_Project">Waymo - Wikipedia</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#Waymo`, `#Dallas`, `#transportation`, `#AI-deployment`

---

<a id="item-tech-news-8"></a>
### [DeepSeek V4 Flash 在单块 AMD MI300X 上运行：速度超 150 tokens/秒](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

GitHub 项目展示了如何在一张 AMD MI300X 上运行 DeepSeek V4 Flash，通过原生 MXFP4 量化实现了超过 150 tokens/秒的推理速度。该项目将上下文窗口从 1M 压缩到 256k，以换取在单卡上的实用性。MI300X 的高 HBM 容量（192GB）是能够容纳模型的关键。由于 MI300X 是 OAM 模块，通常无法单独购买，实际部署可能需要整机（约 250K 欧元，含 8 卡）。该项目还引用了先前在 2x MI300X 上的相关工作，并可能未列出 DwarfStar 等更早的实现。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**「背景」** DeepSeek-V4-Flash 是一个基于 MoE 架构的模型，其官方检查点中约 96% 的路由专家已原生采用 MXFP4 量化，其余部分使用 FP8 或 BF16，因此无需额外量化即可在本地硬件上运行。AMD MI300X 以高 HBM 容量著称，但通常以 OAM 模块形式出货（例如整机含 8 颗，价格约 25 万欧元），并非普通 PCIe 单卡。相关社区工作表明，MI300X 的高 HBM 对这类模型的本地推理很有价值，也已有在双路 MI300X 上运行该模型的先例，并提供了可用的实验环境。

**「影响」** 对于希望在 AMD 平台进行本地大模型推理的开发者，这一方案提供了已验证的高性能路径，但同时受限于硬件获取方式——单块 MI300X 不可直接购买，需使用整机或云服务。

**「社区讨论」** 社区评论指出了关键的可购买性和内存限制：MI300X 是 OAM 模块，难以单独采购，而 MI350P 作为 PCIe 卡且拥有 144GB 内存，也可能运行该模型（因为其 256 个 MoE 导出均为原生 MXFP4）。一些评论者认为，以 256k 上下文替代原始 1M 上下文是实际可行的折衷，但同时也质疑项目在对比先前工作时未提及 DwarfStar 等实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/deepseek-v4-flash-mi300x · GitHub</a></li>
<li><a href="https://fergusfinn.com/blog/deepseek-v4-flash-mi300x/">Bringing up DeepSeek-V4-Flash on AMD MI300X - Fergus Finn</a></li>
<li><a href="https://unsloth.ai/docs/models/deepseek-v4">DeepSeek-V4: How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#amd-mi300x`, `#llm-inference`, `#quantization`, `#moE`

---

<a id="item-tech-news-9"></a>
### [Oxide Computer 完成 4.45 亿美元新融资](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 7.0/10

Oxide Computer 通过美国证券交易委员会（SEC）的 Form D 文件披露，已完成一笔 4.45 亿美元的新一轮融资，这被视为该硬件与云基础设施初创公司迄今规模最大的一次募资。社区评论显示，此轮应为 Series D，此前的融资包括 2023 年的 4400 万美元 A 轮、2025 年的 1 亿美元 B 轮，以及 2026 年的 2 亿美元 C 轮。该公司是一家专注于云基础设施硬件的初创公司，本轮融资反映出投资者对其路线的强烈信心。目前官方尚未正式公布本轮融资的完整细节。

hackernews · depr · 8月4日 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**「背景」** Oxide Computer 是一家销售机架级云基础设施的初创公司，产品把计算、存储和网络整合进单台机架，并配有一整套云控制平面。据数据中心动态报道，该公司在不到一年前刚完成 1 亿美元 B 轮融资，随后又获得 2 亿美元融资；本次 4.45 亿美元同样通过 SEC Form D 披露，属于非公开发行的豁免备案。

**「影响」** 一位自称每年在 AWS 花费 90 万美元的潜在客户表示，Oxide 未回应其销售询问；本轮融资是否补齐这一短板，将直接影响此类客户对平台的采用决定。

**「社区讨论」** 社区普遍对 Oxide 的产品愿景和团队表示认可，尤其提到对 Jessie Frazelle 工作的信任，并期待 Oxide and Friends 节目继续更新。与此同时，也有用户质疑公司是否真正在批量交付硬件，另有一位自称是工程副总裁的评论者抱怨，自己去年提交销售表单后从未收到回复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacenterdynamics.com/en/news/oxide-computer-company-secures-200m-in-funding/">Oxide Computer Company secures $200m in funding - DCD</a></li>

</ul>
</details>

**标签**: `#funding`, `#hardware`, `#cloud computing`, `#tech industry`

---

<a id="item-tech-news-10"></a>
### [华为首席科学家：芯片扩展将触及物理极限](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 7.0/10

华为首席半导体科学家廖恒在 7 月底一场罕见的四小时公开采访中警告，英伟达等芯片巨头依靠持续增加计算芯片和高带宽内存来扩展规模的做法将触及物理极限，越过极限后可能出现“雪崩”。他提出“韬定律”作为替代路径，并透露首款采用 LogicFolding 技术框架的手机芯片将于今年晚些时候亮相。廖恒还指出，中美半导体产业正分化为两个独立生态系统，各方必须建立完整的制造与供应能力才能生存。由于这是前瞻性警告而非已发生事实，实际影响仍有待验证。

telegram · zaihuapd · 8月4日 08:04

**「背景」** 传统芯片性能提升主要依靠不断缩小晶体管尺寸并增加计算芯片与高带宽内存，但这一路径越来越接近物理极限。华为提出的“韬（τ）定律”是以“逻辑折叠”（LogicFolding）为核心的三维芯片架构理念，主张从“缩小芯片”转向“重新设计空间”，以突破制程约束并提升晶体管密度。廖恒正是在这一背景下警告英伟达等厂商的扩展方式将面临瓶颈，并预告首款采用该框架的手机芯片即将推出。

**「影响」** 若廖恒的判断成立，依赖持续堆叠计算芯片与高带宽内存的 AI 算力扩张模式将面临放缓，华为则计划以 LogicFolding 框架在手机芯片上尝试替代路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://csdnnews.blog.csdn.net/article/details/162423752">超越炒作：科普 华 为 LogicFolding 芯 片 背后残酷的数学与 物 理 -CSDN...</a></li>
<li><a href="https://www.pcpop.com/article/6938810.shtml">晶体管密度暴涨55%！ 华 为 LogicFolding 架构突破制程枷锁-泡泡网</a></li>
<li><a href="https://laoyaoba.com/n/1076242">华 为 首席科学家警告：英伟达等巨头即将面临 芯 片 性能瓶颈</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#chip scaling`, `#Huawei`, `#NVIDIA`, `#AI hardware`

---

<a id="item-tech-news-11"></a>
### [Cloudflare 每月 58 美元 AI 自动化漏洞赏金，弃用第三方安全工具](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare 首席安全官 Grant Bourzikas 在悉尼表示，公司已用 Anthropic 的 Claude Sonnet 自动化处理漏洞赏金报告，每月成本约 58 美元，用于去重和评估报告价值；若改用安全专用模型 Mythos，同类工作每月约需 20 万美元。Cloudflare 还构建了 200 多个自主安全代理，几乎弃用全部第三方安全工具，改用部分由 AI 辅助编写的自研应用，但 Bourzikas 建议其他企业不要直接效仿。首席战略官 Stephanie Cohen 称 AI 将根本改变厂商与客户合作模式，并把此前裁员 1100 人归因于 AI 自动化；她还透露 Cloudflare 计划充当 AI 公司与出版商之间的中介，通过微支付让 AI 公司为内容付费。

telegram · zaihuapd · 8月4日 09:24

**「背景」** Anthropic 的 Claude Sonnet 是通用大语言模型，而 Claude Mythos 则是专为修复软件漏洞设计的模型；据公开资料，Mythos 基于下一代 GPU 训练，英国 AI 安全研究院已对其做过测试，Anthropic 还推出了带更强网络安全防护的 Claude Fable 5 作为其安全变体。这解释了 Cloudflare 使用每月 58 美元的通用 Claude Sonnet 做漏洞报告去重和价值评估，与每月约 20 万美元的安全专用模型 Mythos 之间的巨大成本差距。

**「影响」** Cloudflare 的公开成本对比（Claude Sonnet 每月 58 美元 vs. 安全专用模型 20 万美元）以及其 200 多个自主安全代理实践，正在通过 Cloudflare One 的 AI 安全工具、AI Cloud 和代理工具链产品化（tool-2-1、tool-2-2、tool-2-3），可能促使企业安全团队重新评估第三方安全工具的价值；但 CISO 公开警告“不要效仿”也说明，这种自动化收益高度依赖自研安全工程能力，多数组织不能直接复制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>
<li><a href="https://www.scientificamerican.com/article/what-is-mythos-and-why-are-experts-worried-about-anthropics-ai-model/">What is Mythos, Anthropic’s unreleased AI model, and how ...</a></li>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos \ Anthropic</a></li>
<li><a href="https://www.cloudflare.com/solutions/ai/">Cloudflare AI Cloud</a></li>
<li><a href="https://www.techrepublic.com/article/cloudflare-one-new-ai-security-tools/">Cloudflare releases new AI security tools with Cloudflare One</a></li>
<li><a href="https://cloudflare-docs.cloudflare-docs.workers.dev/">Cloudflare Developer Docs | Cloudflare Docs</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#AI security`, `#security automation`, `#Anthropic Claude`, `#vulnerability management`

---

<a id="item-tech-news-12"></a>
### [白宫开源 AI 监管急转弯，硅谷分歧加剧](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

特朗普政府据《纽约时报》报道，在是否限制中国开源 AI 模型问题上出现急转弯：白宫幕僚长 Susie Wiles、财长 Scott Bessent 等人一度考虑动用制裁、贸易黑名单乃至禁止美企与中国公司合作，但在硅谷强烈反对后，转而聚焦提升美国 AI 竞争力。8 月 4 日，白宫邀请科技公司商议新框架，拟在模型发布前进行网络安全审查。导火索是中国开源模型 Kimi 部分性能比肩 OpenAI 顶级模型；OpenAI 与 Anthropic 以国家安全为由推动限制对手，Nvidia、Meta 等则力挺开放生态。黄仁勋上月首次在 X 发帖为开源辩护，并组建了逾 230 家成员的安全联盟。

telegram · zaihuapd · 8月4日 15:22

**「背景」** 开源 AI 模型允许外部开发者获取权重、修改和再分发，中国公司近年发布性能接近美国闭源旗舰的模型，引发美国国家安全担忧。白宫内部围绕“限制中国开源模型”与“扶持本国竞争力”的路线之争，在硅谷大型科技公司之间也对应形成对立阵营。

**「影响」** 若新框架落地，美国 AI 公司可能需在发布前沿模型前接受网络安全审查，从而改变开源权重公开节奏，并影响中美企业在 AI 领域的合作空间；不过政策尚未正式确定，具体约束范围和执行方式仍存在不确定性。

**标签**: `#AI policy`, `#open-source AI`, `#regulation`, `#Silicon Valley`, `#national security`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [财报引发盘前波动：卡特彼勒与 Palantir 领涨](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-premarket-mcd-cat-pltr-mrk.html) ⭐️ 8.0/10

在最新一批季度财报引发的盘前交易中，卡特彼勒和 Palantir 涨幅居前：卡特彼勒第二季度调整后每股收益 8.17 美元，高于 LSEG 分析师预期的 6.20 美元，股价上涨 8%；Palantir 因第二季度美国商业收入同比大增近 150%等强劲业绩上涨 15%。

rss · CNBC Finance · 8月4日 11:42

**「背景」** 上述股价变化发生在各公司公布季度财报后的盘前交易时段；“调整后”指剔除一次性项目后的盈利口径，LSEG 为汇总分析师一致预期的数据机构。

**标签**: `#Earnings`, `#Stock Market`, `#Premarket Trading`, `#Corporate Results`, `#Technology Stocks`

---

<a id="item-finance-news-2"></a>
### [谷歌被曝为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

据《金融时报》调查，谷歌为向 AI 公司 Anthropic 交付超 1500 亿美元 AI 芯片，搭建了合同总额约 2000 亿美元的华尔街融资架构，其中约八成与芯片直接相关；Anthropic 没有信用评级，各方分担风险，谷歌担保数据中心、博通购买并协助融资芯片、阿波罗和黑石出资购买硬件后回租给 Anthropic。今年 6 月，特殊目的载体 Compute SPV 完成首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力、100 万颗 TPU。

telegram · zaihuapd · 8月4日 10:52

**「背景」** Anthropic 是一家 AI 初创公司，谷歌是其长期合作伙伴和重要投资方。2026 年 4 月，两家公司曾宣布谷歌计划向 Anthropic 至多投资 400 亿美元，延续双方合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/04/24/google-to-invest-up-to-40-billion-in-anthropic-as-search-giant-spreads-its-ai-bets.html">Google to invest up to $40 billion in Anthropic as search ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#corporate finance`, `#Wall Street`

---

<a id="item-finance-news-3"></a>
### [宝洁同意以 38 亿美元收购 Thorne](https://finance.yahoo.com/healthcare/articles/procter-gamble-pg-agrees-buy-221007357.html) ⭐️ 8.0/10

宝洁（Procter &amp; Gamble）已同意以 38 亿美元收购健康与保健公司 Thorne。

openbb · PG · 8月4日 22:10

**「背景」** 宝洁是美国跨国消费品公司，Thorne 是膳食补充剂品牌；这笔交易预计于今年晚些时候完成，卖方是私募股权公司 L Catterton，交易将并入宝洁现有的补充剂产品线（如 Metamucil、Align 益生菌和 New Chapter）。

**「影响」** 该交易将扩大宝洁在高端健康与保健领域的产品组合，依托 Thorne 的科学健康解决方案增强其个人保健业务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qz.com/procter-gamble-acquiring-thorne-supplements-3-8-billion-080426">P&amp;G to acquire supplement brand Thorne for $ 3 . 8 billion</a></li>
<li><a href="https://www.axios.com/pro/merger-deals/2026/08/04/procter-gamble-thorne-3b">Procter &amp; Gamble buying Thorne for $ 3 . 8 billion</a></li>
<li><a href="https://www.thorne.com/press-releases/thorne-enters-definitive-agreement-to-be-acquired-by-procter-gamble">Thorne Enters into Definitive Agreement to Be Acquired by ...</a></li>
<li><a href="https://wwd.com/beauty-industry-news/wellness/procter-gamble-acquire-thorne-personal-health-care-1239093305/">Procter &amp; Gamble Acquires Thorne for $3.8 Billion - WWD</a></li>

</ul>
</details>

**标签**: `#M&amp;A`, `#Consumer Goods`, `#Healthcare`, `#Procter &amp; Gamble`, `#Thorne`

---

<a id="item-finance-news-4"></a>
### [中东冲突推高油价，BP 利润增长逾一倍](https://finance.yahoo.com/energy/articles/bp-profit-more-doubles-middle-093317262.html) ⭐️ 8.0/10

BP 公布的利润增长超过一倍，主要受中东冲突推动油价上涨影响。

openbb · BRK-B · 8月4日 17:18

**「背景」** 英国能源巨头 BP 公布，第二季度净利润较上年同期增加一倍以上。该公司称，中东战争扰乱了石油和天然气市场并推高油价，是利润大增的主要原因。

**「影响」** 这一利润跳升背后是地缘政治推动的油价上涨，而油价上涨会通过成本传导冲击依赖能源进口的经济体和下游行业：世界银行估算，地缘政治供应冲击使油价上涨 10%时，天然气价格峰值涨幅约 7%、化肥价格峰值涨幅超过 5%；若冲突长期持续，进口依赖度高的国家将持续承压。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://uk.finance.yahoo.com/video/bp-profit-more-doubles-middle-165837162.html">BP profit more than doubles as Middle East conflict boosts oil prices</a></li>
<li><a href="https://www.worldbank.org/en/news/press-release/2026/04/28/commodity-markets-outlook-april-2026-press-release">Middle East War to Spark Biggest Energy Price Surge in Four Years</a></li>
<li><a href="https://www.imf.org/en/blogs/articles/2026/03/30/how-the-war-in-the-middle-east-is-affecting-energy-trade-and-finance">How the War in the Middle East Is Affecting Energy, Trade ...</a></li>

</ul>
</details>

**标签**: `#BP`, `#earnings`, `#oil prices`, `#Middle East conflict`, `#energy sector`

---

<a id="item-finance-news-5"></a>
### [高盛交易业务有望创纪录：上季股票交易收入大增 72%](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 7.0/10

高盛交易业务正走向创纪录的一年：第二季度股票交易收入增长 72%至 74.2 亿美元，创下纪录并高于预期；投行收入也增长 55%至 34 亿美元，其中包含 SpaceX 首次公开募股、25 亿美元债券发行及 Alphabet 850 亿美元股权融资的相关费用。

rss · CNBC Finance · 8月4日 19:38

**「背景」** 高盛近年加大对股票交易业务的投入，并在全球银行与市场部门内推动投行、股票、固定收益等业务交叉销售，为此次交易收入大增提供支撑。

**标签**: `#Goldman Sachs`, `#equities trading`, `#investment banking`, `#earnings`, `#trading revenue`

---

<a id="item-finance-news-6"></a>
### [国家邮政局对申通快递有限公司立案调查](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 7.0/10

国家邮政局 8 月 4 日宣布，依法对申通快递有限公司立案调查。原因是 2026 年以来，使用“申通快递”商标、字号和快递运单经营的多家企业多次发生生产安全事故，并在场所内多次被发现事故隐患，而申通快递有限公司被指对相关企业安全生产管理缺位，未按规定实行安全保障统一管理。

telegram · zaihuapd · 8月4日 12:07

**「背景」** 国家邮政局 8 月 4 日宣布，因使用“申通快递”品牌的多家企业今年以来多次发生生产安全事故并被发现安全隐患，而申通快递有限公司未按规定对相关企业实行安全保障统一管理，依法对该公司立案调查。

**「影响」** 申通快递已回应称将立行立改、全力配合调查；这一立案调查显示监管重点从处罚网点转向追责总部，使用“申通快递”品牌的加盟网点和同行业公司可能面临更严格的安全管理合规检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.cctv.com/2026/08/04/ARTIxQDXIvTHcdHsMaU2kzU0260804.shtml">国家邮政局依法对申通快递有限公司立案调查_新闻频道_央视网 (cctv.co...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2068108283840402775">如何评价国家邮政局依法对申通快递立案调查？这释放了什么行业信号？ ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260804A0DLI600">国家邮政局依法对申通快递立案调查 申通回应：立行立改、全力配合各项...</a></li>
<li><a href="https://finance.sina.com.cn/stock/s/2026-08-04/doc-inimeknx4006837.shtml">申通快递被立案调查，加盟制度弊病集中爆发，被指总部收钱、网点担责...</a></li>

</ul>
</details>

**标签**: `#regulatory investigation`, `#STO Express`, `#logistics industry`, `#safety management`, `#China postal regulator`

---

<a id="item-finance-news-7"></a>
### [NVIDIA 宣布重大投资神秘 AI 实验室，押注超级智能](https://finance.yahoo.com/technology/ai/articles/secretive-ai-lab-chasing-superintelligence-180821241.html) ⭐️ 7.0/10

NVIDIA 宣布对一家致力于“超级智能”的神秘 AI 实验室进行重大投资，但未披露具体金额。此举凸显了 NVIDIA 对前沿 AI 领域的战略布局。

openbb · NVDA · 8月4日 18:08

**「背景」** Safe Superintelligence 是一家由前 OpenAI 首席科学家 Ilya Sutskever 联合创办的 AI 实验室，专注开发“超级智能”，目前尚无产品。据多家媒体报道，英伟达将通过约 50 亿美元的投资和芯片供应合作，与该实验室建立长期合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.resultsense.com/news/2026-07-28-nvidia-safe-superintelligence-investment/">Nvidia to put £3.8bn into Sutskever&#x27;s Safe Superintelligence</a></li>
<li><a href="https://www.linkedin.com/posts/guillermoflor_breaking-nvidia-is-betting-billions-on-the-activity-7487567502332461056-sMsa">Nvidia Funds Safe Superintelligence AI Lab | Guillermo... | LinkedIn</a></li>
<li><a href="https://www.tipranks.com/news/nvidia-nvda-bets-5b-on-ilya-sutskevers-safe-superintelligence-ai-lab-despite-capex-concerns">Nvidia (NVDA) Bets $5B on Ilya Sutskever’s Safe Superintelligence ...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Artificial Intelligence`, `#Investment`, `#Superintelligence`, `#AI Lab`

---

<a id="item-finance-news-8"></a>
### [AMD 第二季度业绩超预期，同时披露巨额资本支出](https://finance.yahoo.com/video/amd-beats-q2-earnings-estimates-202804476.html) ⭐️ 7.0/10

AMD 公布的第二季度业绩好于分析师预期，同时披露了大规模资本支出计划。

openbb · NVDA · 8月4日 20:28

**「背景」** AMD 于 2025 年 8 月 5 日发布 2025 年第二季度财报，营收为 115 亿美元，资本支出为 8.08 亿美元，环比增长约 108%，远高于分析师预期的 2.98 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ir.amd.com/news-events/press-releases/detail/1257/amd-reports-second-quarter-2025-financial-results">AMD Reports Second Quarter 2025 Financial Results :: Advanced Micro Devices, Inc. (AMD)</a></li>
<li><a href="https://finance.yahoo.com/technology/article/amd-tops-q2-earnings-estimates-and-provides-strong-outlook-but-leaves-investors-unimpressed-110000620.html">AMD tops Q2 earnings estimates and provides strong outlook, but leaves investors unimpressed</a></li>
<li><a href="https://breakingthenews.net/Article/AMD-posts-Q2-revenue-of-dollar11.5B-up-50/66850343">AMD posts Q2 revenue of $11.5B, but capex soars</a></li>

</ul>
</details>

**标签**: `#AMD`, `#Earnings`, `#Capital Expenditure`, `#Semiconductors`, `#Q2`

---

<a id="item-finance-news-9"></a>
### [利润再高也难让芯片投资者满意](https://www.wsj.com/finance/stocks/even-big-profits-arent-enough-to-keep-chip-investors-happy-36acfc66?siteid=yhoof2&amp;yptr=yahoo) ⭐️ 7.0/10

《华尔街日报》报道，半导体行业即使企业公布丰厚利润，投资者仍不满意；报道认为这反映出市场预期异常之高，并可能预示投资者情绪转变。

openbb · NVDA · 8月4日 21:23

**「背景」** Nvidia 是 AI 股票热潮的关键驱动者，其股价今年已上涨超过 200%，随后因中国 AI 初创公司 DeepSeek 引发市场恐慌而出现大幅下跌。此前的大幅上涨可能让投资者对芯片公司财报的期望变得异常高，使得即使利润强劲也不足以令他们满意。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cityam.com/nvidia-sinks-as-chinese-ai-startup-deepseek-spooks-global-markets/">Nvidia tanks as Chinese AI startup Deepseek spooks global markets</a></li>
<li><a href="https://www.tastylive.com/news-insights/nvidia-earnings-preview-up-over-200-this-year">Nvidia (NVDA) Q3 Earnings Preview: 8% Stock Move... | tastylive</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#Nvidia`, `#earnings`, `#investor sentiment`, `#stock market`

---

<a id="item-finance-news-10"></a>
### [麦当劳财报超预期但警示未来业绩](https://finance.yahoo.com/markets/stocks/articles/mcdonalds-earnings-win-comes-warning-200519881.html) ⭐️ 7.0/10

据报道，麦当劳最新财报盈利超出预期，但公司对未来业绩发出警示信号。

openbb · PG · 8月4日 20:05

**「背景」** 据美联社报道，麦当劳近期公布的第二季度财报显示盈利强劲，但美国市场销售仍受到消费者谨慎支出的影响，这可能是标题中“警示信号”所指。

**「影响」** 低收入消费者因通胀和谨慎支出而减少外出就餐，正在拖累麦当劳在美国的客流量和销售；公司已警告此类消费疲软已持续超过一年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/mcdonalds-profit-economy-9b9ef2da69dc72451928176f17051126">McDonald&#x27;s reports strong profit and names new head for US ...</a></li>
<li><a href="https://www.nytimes.com/2026/08/04/business/mcdonalds-earnings-consumers-inflation.html">McDonald’s U.S. Sales Slow as Diners Spend More Cautiously</a></li>
<li><a href="https://www.cnbc.com/2026/02/11/mcdonalds-mcd-q4-2025-earnings.html">McDonald&#x27;s (MCD) Q4 2025 earnings - CNBC</a></li>

</ul>
</details>

**标签**: `#McDonald&\#x27;s`, `#earnings`, `#consumer spending`, `#outlook`, `#fast food`

---