---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---

> 从 234 条内容中筛选出 28 条重要资讯。

---

**科技新闻**
1. [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1](#item-tech-news-1) ⭐️ 8.0/10
2. [AI 怀疑论者 Zitron 的预测准确度评析](#item-tech-news-2) ⭐️ 8.0/10
3. [一个 1.5 小时训练的小型 Transformer 在 ARC 上击败众多 LLM](#item-tech-news-3) ⭐️ 8.0/10
4. [EvoUndo：为 LLM 智能体自演化提供可恢复性验证框架](#item-tech-news-4) ⭐️ 8.0/10
5. [Virtualizor 更新设施遭 BGP 劫持并植入 root 后门](#item-tech-news-5) ⭐️ 8.0/10
6. [Google Play 不再允许 AnkiDroid 使用 Open Collective 捐赠链接](#item-tech-news-6) ⭐️ 7.0/10
7. [Jujutsu 作者 Martin 加入 GitHub 竞品 ERSC](#item-tech-news-7) ⭐️ 7.0/10
8. [2026 年潜在推理格局：超越 Token 流的五种技术路线](#item-tech-news-8) ⭐️ 7.0/10
9. [TontaubeV1：面向长篇生成的开源字符级 TTS 模型](#item-tech-news-9) ⭐️ 7.0/10
10. [光伏装机超煤电成中国第一大电源](#item-tech-news-10) ⭐️ 7.0/10
11. [谷歌发布 Gemini 3.8 Flash，编码能力据称追赶 OpenAI 与 Anthropic](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [亚洲现货 LNG 价格升至五个月高位 霍尔木兹海峡受阻持续](#item-finance-news-1) ⭐️ 9.0/10
2. [美伊再度互袭推高油价](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储维持利率不变](#item-finance-news-3) ⭐️ 9.0/10
4. [美联储理事巴尔：若通胀未降温将支持加息](#item-finance-news-4) ⭐️ 8.0/10
5. [沙特计划到 2030 年替代逾 100 万桶/日石油消费](#item-finance-news-5) ⭐️ 8.0/10
6. [锂价大涨与美国大单：美国锂矿商迎来转机](#item-finance-news-6) ⭐️ 8.0/10
7. [坦桑尼亚矿业改革见效：黄金出口创纪录](#item-finance-news-7) ⭐️ 8.0/10
8. [英国 8 月商店价格通胀创两年多新高，食品通胀升至 2.8%](#item-finance-news-8) ⭐️ 8.0/10
9. [美国 2026 年第二季度储能装机量创纪录新高](#item-finance-news-9) ⭐️ 8.0/10
10. [日本放宽每月 45 小时加班上限](#item-finance-news-10) ⭐️ 8.0/10
11. [台积电 2690 亿美元扩张引关注，67.7%毛利率成焦点](#item-finance-news-11) ⭐️ 8.0/10
12. [通胀数据降温或使沃什领导的美联储维持利率不变](#item-finance-news-12) ⭐️ 8.0/10
13. [美联储维持利率不变，鲍威尔召开记者会](#item-finance-news-13) ⭐️ 8.0/10
14. [高通宣布 9 月 1 日后出货芯片涨价两位数](#item-finance-news-14) ⭐️ 7.0/10
15. [《微短剧发展管理办法》今日正式施行](#item-finance-news-15) ⭐️ 7.0/10
16. [三部门发布汽车行业境外竞争与合规指引](#item-finance-news-16) ⭐️ 7.0/10
17. [外籍个人股息红利个税税率明确为 20%](#item-finance-news-17) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1](https://www.anthropic.com/claude-fable-and-mythos-5-1) ⭐️ 8.0/10

Anthropic 发布了 Claude Fable 5.1 与 Claude Mythos 5.1 两个新 AI 模型，并公布了系统卡。新版本据称在写作风格和科学性能上有所提升，同时调整了定价策略。社区评论指出缓存读取价格下调、价格竞争和思维链可见性等问题。整体是增量更新，未出现范式转变。

hackernews · denysvitali · 9月1日 17:53 · [社区讨论](https://news.ycombinator.com/item?id=49525378)

**「背景」** Claude Fable 5.1 和 Claude Mythos 5.1 是 Anthropic 新发布的 AI 模型，两者实际上是同一个模型，但采用了不同级别的安全保护措施。Fable 5.1 已全面可用，而 Mythos 5.1 仅通过可信访问计划提供，其安全措施专门用于支持网络安全和生命科学领域的工作。此次发布延续了 Anthropic 的 Claude 模型系列，并带来了性能改进、价格调整以及系统卡等细节。

**「影响」** 对依赖缓存的 API 用户，缓存读取定价的大幅下调（据社区帖子为每百万 tokens 从 1 美元降至 0.25 美元）会直接降低推理成本，并可能加剧行业价格竞争。

**「社区讨论」** 社区反应两极：部分人称赞写作风格更自然、思考力度选项表现不错，也有人质疑除 Terminal-Bench-Science 外改进有限，并批评 Anthropic 削弱 Fable、以 Mythos 营销及移除思维轨迹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5.1 and Claude Mythos 5.1 \\ Anthropic</a></li>

</ul>
</details>

**标签**: `#anthropic`, `#claude`, `#ai-models`, `#machine-learning`, `#llm`

---

<a id="item-tech-news-2"></a>
### [AI 怀疑论者 Zitron 的预测准确度评析](https://danluu.com/zitron/) ⭐️ 8.0/10

Dan Luu 发布了对 Ed Zitron 一系列 AI 怀疑论预测准确性的评估，采用数据驱动的方式逐一检验其言论，并给出了一个细致的、非一边倒的结论。这项分析之所以受关注，是因为 Zitron 是 AI 行业知名的批评者，而 Luu 的评估为围绕 AI 泡沫与进展的争论提供了具体依据。评论区的讨论进一步指出，Zitron 与 AI 行业领袖一样经常夸大其词，且其怀疑论立场可能限制他承认错误。整体而言，该文并非重大突破，但对 AI 行业观察者具有较高参考价值。

hackernews · jatins · 9月1日 18:35 · [社区讨论](https://news.ycombinator.com/item?id=49526069)

**「背景」** Dan Luu 在《How accurate have Ed Zitron&\#x27;s AI skeptic predictions been?》一文中，逐一评估了 Ed Zitron 对 AI 行业的悲观预测的准确性，并指出 Zitron 喜欢构建英雄与反派式的叙事，而这种叙述往往无法准确识别技术发展中的真实因果机制。该文章在 Hacker News 和 X 上引发广泛讨论，部分评论者认可 Zitron 偶尔能披露独家数据，但也批评他将信息包裹在强烈偏见之中，还有人认为他已成为自己所嘲讽的 AI 鼓吹者的镜像。

**「社区讨论」** 评论认为 Zitron 与 AI 吹鼓手一样常夸大其词，并因 AI 怀疑论成为政治立场而拥有固定受众，导致他难以承认错误；也有人指出帖子未讨论超大规模厂商通过投资 Anthropic、OpenAI 等公司升值并计入“其他收入”，从而显著提升财报营收的现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://danluu.com/zitron/">How accurate have Ed Zitron&#x27;s AI skeptic predictions been?</a></li>
<li><a href="https://x.com/danluu/status/2094853413788127413">Dan Luu (@danluu) on X</a></li>
<li><a href="https://news.ycombinator.com/item?id=49526069">How accurate have Ed Zitron&#x27;s AI skeptic predictions been? | Hacker News</a></li>

</ul>
</details>

**标签**: `#AI skepticism`, `#Ed Zitron`, `#predictions`, `#AI industry`, `#analysis`

---

<a id="item-tech-news-3"></a>
### [一个 1.5 小时训练的小型 Transformer 在 ARC 上击败众多 LLM](https://mvakde.github.io/blog/44-on-arc-1/) ⭐️ 8.0/10

作者展示，一个从零训练的小型自回归 Transformer 仅用 1.5 小时，就在 ARC 基准上取得了优于许多大型语言模型的结果。它并非 LLM，而是一个小型自回归 Transformer，关键改进包括现代架构（如 SwiGlu、RMSNorm）和更丰富的训练数据多样性。该结果挑战了“复杂问题必须依赖大规模 LLM”的普遍假设，凸显了样本效率和架构设计的重要性。不过，这一结果尚未被全面独立验证，仍需要更多复现和外部评估。

hackernews · porridgeraisin · 9月1日 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49519939)

**「背景」** ARC-AGI（ARC-1）是一个抽象推理基准，要求模型从少量示例中归纳规则并完成视觉网格变换任务；该基准长期被认为难以靠小模型突破，通常只有大语言模型或大量微调才能取得较高分数。本文作者训练了一个从零开始的小型 Transformer，仅在单张 RTX 5090 上用 1.5 小时完成训练，成本约 67 美分，就在 ARC-1 公开评测上达到 44%，与使用更多算力的 TRM/HRM 成绩相当；关键改进包括使用测试时训练、3D RoPE 嵌入和每任务可学习嵌入，且这些设计被消融实验证明至关重要。该模型并非 LLM，同时也在 ARC-2 上取得 7%的成绩。

**「影响」** 对于计算资源有限的研究者，该结果表明在 ARC 等特定基准上，小模型配合现代架构与数据策略也能达到强竞争力，可能降低 AI 研究的入门门槛；但独立复现与更广泛基准上的验证仍然必要。

**「社区讨论」** 作者在评论中澄清这不是 LLM，而是从零训练的小型自回归 Transformer，并指出 ARC 是元学习基准，因此基于评估谜题训练并不算测试集作弊，因为测试标签未被使用。另一位评论者肯定了作者提出样本效率问题的价值，但认为架构改进（如 SwiGlu、RMSNorm）和增加层数属于常见的“挤柠檬”式优化，而非从根本上解决样本效率的新方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mangodeveloper.com/articles/a-15-hour-transformer-beats-llms-on-arc-agi-and-it-costs-pocket-change">A 1.5-Hour Transformer Beats LLMs on ARC-AGI, And It Costs ...</a></li>
<li><a href="https://mvakde.github.io/blog/44-on-arc-1/">44% on ARC-AGI-1 in 67 cents - Mithil Vakde’s Homepage</a></li>
<li><a href="https://www.youtube.com/watch?v=tEfBCnyg5BQ">Small Transformer Model Beats LLMs on ARC-1 Benchmark Researcher trains small transformer from scratch in 1.5 hours ... A 67-cent transformer beats many LLMs on ARC-AGI-1 I trained a small transformer in 1.5hrs and it beats many ... 44% on ARC-AGI-1 in 67 cents</a></li>

</ul>
</details>

**标签**: `#transformer`, `#ARC`, `#efficiency`, `#training`, `#AI`

---

<a id="item-tech-news-4"></a>
### [EvoUndo：为 LLM 智能体自演化提供可恢复性验证框架](https://www.reddit.com/r/MachineLearning/comments/1w4m0hq/evoundo_recoverabilityconstrained_selfevolution/) ⭐️ 8.0/10

EvoUndo 是一个为 LLM 智能体自演化设计的可恢复性验证框架，能够表示、综合、诊断并独立验证模型生成的自我修改在反事实状态下的可恢复性。在 600 个未见的一次性自演化任务中，框架识别出 197 个通过能力提升但未通过可恢复性验证的突变；在原始恢复表示下，常规修复策略无法恢复其中任何一个，而扩展的恢复演算将确定性 oracle 恢复数量提升至 191/197。进一步协议锁定实验表明，精确状态地址接地在原始语言足够时将恢复率从 0/48 提升至 38/48（79.2%），扩展恢复语言则在 oracle 定义的 S1 层恢复 142/143（99.3%）；但在 gpt-oss-120b 主干上加入精确地址诊断后恢复降为 133/143（93.0%），而 Qwen3.8-27B 复制实验未发现这一负交互，说明该现象具有模型依赖性。研究指出，可靠的智能体自演化需要协同设计验证、状态接地、见证语义和恢复语言表达力，而不能仅依赖迭代提示。

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · 9月1日 19:17

**「背景」** 大型语言模型（LLM）代理可在运行时修改自身的提示、工具、中间件和资源，这种自进化能力可能带来无法在反事实状态下安全逆转的持久影响。EvoUndo 是一个框架，用于表示、合成、诊断并独立验证模型生成的自修改的可恢复性，通过扩展恢复演算在 600 个未见任务中识别并修复了 197 个自然失败。该工作表明，可靠的代理自进化需要协同设计验证、状态接地、见证语义和恢复语言表达力，而不仅仅依赖迭代提示，相关论文见 arXiv:2608.28363。

**「影响」** 该框架为自演化 LLM 智能体的开发者提供了可验证的故障恢复与回滚机制，帮助避免不可逆突变造成的持久错误；但恢复效果的模型依赖性意味着在实际部署前仍需针对具体模型验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.28363">[2608.28363] EvoUndo: Recoverability-Constrained Self-Evolution for LLM Agent Harnesses</a></li>
<li><a href="https://arxiv.org/html/2608.28363">EvoUndo: Recoverability-ConstrainedSelf-Evolution for LLM Agent Harnesses</a></li>

</ul>
</details>

**标签**: `#LLM agents`, `#AI safety`, `#self-evolution`, `#recoverability`, `#software engineering`

---

<a id="item-tech-news-5"></a>
### [Virtualizor 更新设施遭 BGP 劫持并植入 root 后门](https://www.virtualizor.com/blog/security-incident-bgp-hijacking/) ⭐️ 8.0/10

Virtualizor 的更新基础设施在 2026 年 8 月 28 日至 30 日遭到 BGP 路由劫持，攻击者使用有效 TLS 证书投递恶意更新包，官方确认仅有在更新窗口内完成安装的少量服务器受影响，并强调问题出在分发链路而非软件漏洞。独立取证显示，恶意包会写入 root SSH 密钥、安装 Java 载荷并建立持久化服务；AlbaHost 在 34 台 hypervisor 中发现 5 台存在感染指标。Softaculous 表示目前没有证据表明其他产品受到影响。管理员应优先审查该窗口期内的更新记录和相关主机。

telegram · zaihuapd · 9月1日 06:05

**「背景」** BGP 劫持是指攻击者通过伪造或劫持边界网关协议路由，将原本应到达合法服务器的网络流量重定向到攻击者控制的服务器。Virtualizor 的更新请求因此在攻击窗口内被引导至恶意端点；由于攻击者持有与被劫持域名匹配的有效 TLS 证书，客户端无法仅通过证书验证识别出更新包已被替换。

**「影响」** 在受影响窗口内更新过 Virtualizor 的服务器管理员应立即检查 root SSH 授权密钥、Java 进程与持久化服务，并对确认感染的 hypervisor 进行重装或彻底清理。官方称这不是软件自身漏洞，但任何运行受影响版本的节点都应视为可能已被完全控制。

**标签**: `#security`, `#supply-chain attack`, `#BGP hijacking`, `#rootkit`, `#Virtualizor`

---

<a id="item-tech-news-6"></a>
### [Google Play 不再允许 AnkiDroid 使用 Open Collective 捐赠链接](https://github.com/ankidroid/Anki-Android/issues/21656) ⭐️ 7.0/10

AnkiDroid 在 GitHub 议题中报告，Google Play 已不再允许其应用内包含 Open Collective 捐赠链接，这项政策变化直接影响了开源项目通过应用商店页面获得捐赠的途径。由于 AnkiDroid 是一个广泛使用的开源应用，该变化引发开发者对应用商店垄断控制以及开源项目可持续资金模式的讨论。目前具体的政策细节和替代方案尚不明确，受影响的用户和开发者可查阅相关议题了解后续发展。

hackernews · hexa555 · 9月1日 10:11 · [社区讨论](https://news.ycombinator.com/item?id=49520022)

**「背景」** AnkiDroid 是一款开源闪卡应用，通过 Open Collective 平台接受捐赠以维持开发。Google Play 对应用内捐赠有严格政策，通常只允许面向美国 501\(c\)\(3\) 慈善机构的捐赠，而 AnkiDroid 所依托的 Open Collective 属于 501\(c\)\(6\) 身份，捐赠对捐赠者不可抵税，因此被 Play 商店判定不符合政策，导致其捐赠链接被移除。社区讨论指出，Google 在 2019 年也曾以类似方式将 WireGuard 等项目从 Play 商店下架，这反映了应用商店对开源项目资金渠道的高度控制。

**「影响」** Google Play 不再允许 AnkiDroid 在应用商店页面放置 Open Collective 捐赠链接，切断了该项目通过该商店页面直接引导用户捐款的渠道。

**「社区讨论」** 评论中多数人将此视为 Google 对该类链接的既定做法，并拿 2019 年 WireGuard 被 Google Play 下架一事作类比，认为应用商店的绝对控制对开源项目不利。另一些评论则辨析了 501\(c\)\(6\) 组织下的捐赠并非税务意义可抵扣的捐赠，并有一位用户表示会借此机会向 AnkiDroid 捐款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49520022">AnkiDroid : Google Play no longer allowing Open Collective ...</a></li>
<li><a href="https://github.com/ankidroid/Anki-Android/issues/21656">[Community Help Needed] Google Play : no longer allowing our Open ...</a></li>
<li><a href="https://www.drweb.de/google-play-ankidroid-spendenlink/">Warum blockiert Google Play den Spendenlink von AnkiDroid ?</a></li>

</ul>
</details>

**标签**: `#open source`, `#Google Play`, `#app stores`, `#software funding`, `#policy`

---

<a id="item-tech-news-7"></a>
### [Jujutsu 作者 Martin 加入 GitHub 竞品 ERSC](https://ersc.io/blog/martin-joins-ersc) ⭐️ 7.0/10

Jujutsu 版本控制系统作者 Martin 已加入 ERSC，一家旨在与 GitHub 竞争的初创公司，相关消息发布于 ERSC 博客，并引发 Hacker News 社区的热烈讨论（138 条评论）。Jujutsu 是一款兼容 Git 的版本控制工具，以可撤销操作和更简洁的工作流等特性著称；Martin 加入后，ERSC 希望借此在开发者工具市场建立差异化优势。目前 ERSC 是否以及如何解决 GitHub 的不足尚不明确，其后续产品方向仍待观察。

hackernews · steveklabnik · 9月1日 17:46 · [社区讨论](https://news.ycombinator.com/item?id=49525297)

**「背景」** Jujutsu（常简写为 jj）是一个与 Git 兼容的开源版本控制系统，由 Martin von Zweigbergk 于 2019 年末作为个人项目启动，之后在 Google 将其发展为全职工作。ERSC（East River Source Control）是一家旨在与 GitHub 竞争的初创公司，其目标是解决基于 Git 的远程仓库在可扩展性上的限制。近期 ERSC 宣布 Martin von Zweigbergk 加入并担任首席技术官，负责领导其下一代版本控制平台的工程开发。

**「影响」** 对 Jujutsu 用户和关注 Git 生态的开发者而言，Martin 加入 ERSC 可能加速 jj 与协作平台的集成，并加剧开发者工具领域的竞争；但由于项目路线图尚未公布，实际影响存在不确定性。

**「社区讨论」** 评论者看法不一：有人称赞 jj 的“可撤销”UX 和更聪明的 Git 体验，也有人认为 jj 本质上是 Git 之上的新“方向盘”，需要 ERSC 解释其相对 GitHub 的额外价值。steveklabnik 表示与 Martin 合作愉快，后续会有更多消息；社区整体保持好奇，但在价值主张上存在分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ersc.io/blog/martin-joins-ersc">East River Source Control Names Jujutsu Creator Martin von ...</a></li>
<li><a href="https://zeli.app/story/49525297">Jujutsu Creator Martin von Zweigbergk Joins ERSC as CTO</a></li>

</ul>
</details>

**标签**: `#jujutsu`, `#version-control`, `#ersc`, `#open-source`, `#developer-tools`

---

<a id="item-tech-news-8"></a>
### [2026 年潜在推理格局：超越 Token 流的五种技术路线](https://www.reddit.com/r/MachineLearning/comments/1w4evwo/latent_reasoning_landscape_in_2026_mapping_bdhcq/) ⭐️ 7.0/10

该 Reddit 分析梳理了 2026 年潜在推理（latent reasoning）研究格局，认为通往更强 AI 的路径可能更依赖超越 token 流的架构，而非更长的思维链（CoT）。作者将方法分为五类：自回归 LM 中的连续思维（Coconut、Soft Thinking）、压缩的非语言离散 token（Abstract-CoT）、循环深度/回环模型、任务训练的递归求解器（HRM/TRM），以及上下文内循环潜在求解器（BDH-CQ）。其中 BDH-CQ 基于 Dragon hatchling 架构，报告在 ARC-AGI-1 上超越先前成本-准确率帕累托前沿，并展示了高达 600B 参数的 Transformer 类似缩放规律。文章同时提出了若潜在推理胜出，可读的 CoT 轨迹（支撑行业可解释性与评估）将何去何从的问题。

reddit · r/MachineLearning · /u/Typical-Scene-5794 · 9月1日 15:14

**「背景」** 潜在推理的核心观点是，语言模型虽然能生成看似合理的中间步骤，但研究表明（如 Kambhampati，2025）推理轨迹并不等同于计算本身。因此，一些研究者转向让模型在连续的隐藏状态中反复变换并直接解码答案，而非将每一步都转成文字。这是理解五类方法为何出现、以及它们如何区别于传统 CoT 的背景。

**「影响」** 对 AI/ML 从业者而言，这套分类有助于比较不同潜在推理路线；若 BDH-CQ 等方法的效率优势得到验证，可能改变推理模型的设计取舍，但也会牺牲当前依赖可读 CoT 的可解释性与评测方式。

**标签**: `#latent reasoning`, `#machine learning`, `#continual learning`, `#chain-of-thought`, `#arXiv`

---

<a id="item-tech-news-9"></a>
### [TontaubeV1：面向长篇生成的开源字符级 TTS 模型](https://www.reddit.com/r/MachineLearning/comments/1w4afjn/we_released_tontaubev1_a_characterlevel_tts_model/) ⭐️ 7.0/10

开发者发布了 TontaubeV1，一个约 29 亿参数的开源权重 TTS 模型，重点支持英语和德语的长篇叙事、富有表现力的语音，并可从最多一分钟参考音频进行零样本声音克隆。该模型基于 DualCodec 多码本音频编解码器，在 7 种语言、约 20 万小时音频上训练；其语义码本模型从 Qwen3-1.7B 初始化，并采用字符级分词和跨文本/音频的块式位置编码，以降低长文本生成中的越界与罕见 token 问题。当前版本需要至少 24GB 显存（低显存/均衡配置）或 32GB（高吞吐配置），作者计划发布量化版本和微调支持。作者还报告了 400 段有声书基准测试，在韵律方面对 ElevenLabs Flash v2.5 取得 50.1%的偏好率，但强调仍需人工听测验证。

reddit · r/MachineLearning · /u/EAVDR · 9月1日 12:23

**「背景」** 基于大语言模型的 TTS 通常复用骨干模型的 BPE 分词器，并向其中加入音频 token，让模型预测下一个音频 token；字符级分词则把文本拆成单个字符，简化字符到声音的映射，但很少被采用。TontaubeV1 采用多码本离散音频编解码器 DualCodec，并设计了跨块的位置编码，使文本与音频共享同一时间轴，以支持长文本生成和流式输出。

**「影响」** 对于需要在英语或德语上做零样本声音克隆和长篇音频生成的开发者和研究团队，TontaubeV1 提供了一个可本地部署的开源基线；其 24GB 显存门槛和基于 LLM 评判而非人工听测的韵律胜率意味着，实际听感优势和部署成本仍需独立验证。

**标签**: `#text-to-speech`, `#open-source`, `#machine-learning`, `#audio`, `#LLM`

---

<a id="item-tech-news-10"></a>
### [光伏装机超煤电成中国第一大电源](https://content-static.cctvnews.cctv.com/) ⭐️ 7.0/10

央视新闻报道称，截至 2026 年 7 月底，全国光伏发电装机达 12.86 亿千瓦，首次超越煤电，占总装机 31.5%，成为中国第一大电源。2026 年 1 至 7 月，全国光伏发电量突破 8024 亿千瓦时，同比增长 15.5%，相当于每 8 度电中就有 1 度来自光伏；全球每 10 块光伏组件有 8 块为中国制造，未来五年产业投资预计超 2 万亿元。值得注意的是，这些数据来自媒体报道，且日期晚于当前时间，尚未获得独立核实。

telegram · zaihuapd · 9月1日 02:42

**「背景」** 中国长期以来以煤电为第一大电源，装机容量指发电设备的总规模，而发电量还取决于光照条件、利用小时数等因素。此次国家能源局宣布，截至 2026 年 7 月底光伏装机达 12.86 亿千瓦，首次超过煤电，标志着可再生能源里程碑；不过“装机第一大”并不等于“发电量第一大”。

**「影响」** 如果该数据得到官方统计确认，将标志着中国电力装机结构出现历史性转折，可能加速能源行业对光伏投资和电网消纳能力的重新评估。不过，装机容量超过煤电并不等于发电量超过煤电，实际发电贡献仍受光照条件和电网调度等因素限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.dbw.cn/system/2026/09/01/001566414.shtml">China &#x27;s photovoltaic power capacity overtakes coal -fired power for...</a></li>
<li><a href="https://www.globaltimes.cn/page/202609/1369526.shtml">China ’s installed solar power generating capacity surpasses coal ...</a></li>
<li><a href="https://english.aawsat.com/business/5313306-china-says-solar-power-capacity-surpasses-coal-first-time">China Says Solar Power Capacity Surpasses Coal for First Time</a></li>

</ul>
</details>

**标签**: `#solar energy`, `#China`, `#energy transition`, `#photovoltaics`, `#technology industry`

---

<a id="item-tech-news-11"></a>
### [谷歌发布 Gemini 3.8 Flash，编码能力据称追赶 OpenAI 与 Anthropic](https://www.wsj.com/tech/ai/new-google-ai-model-said-to-narrow-gap-on-coding-ability-264c6052) ⭐️ 7.0/10

据《华尔街日报》援引知情人士报道，谷歌 DeepMind 计划最早于本周三发布新模型 Gemini 3.8 Flash（内部代号 Skimaki），其编码能力大幅升级。在内部编程工具 Jetski 的对比测试中，工程师据称更偏好该模型而非 Anthropic 的 Opus 模型。此次发布可能弥补谷歌在编码领域落后于 OpenAI 和 Anthropic 的短板。报道基于内部信息，尚未提供详细技术基准或官方确认。

telegram · zaihuapd · 9月2日 00:35

**「背景」** Gemini 是谷歌 DeepMind 开发的大语言模型系列，主要与 OpenAI 的 GPT 系列和 Anthropic 的 Claude 系列竞争。在编程（代码生成与理解）能力上，OpenAI 与 Anthropic 目前保持领先，而谷歌的 Gemini 系列此前被认为存在一定差距。本次传闻中的 3.8 Flash 是一个轻量级快速版本，定位可能与低延迟编码场景有关。

**「影响」** 如果报道属实，Gemini 3.8 Flash 的发布将使谷歌在 AI 编程助手领域获得更有竞争力的模型，可能影响开发者对编码助手的选择。不过目前该消息仍属内部传闻，模型实际性能与正式发布时间需待官方确认。

**标签**: `#artificial intelligence`, `#Google`, `#Gemini`, `#coding`, `#machine learning`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [亚洲现货 LNG 价格升至五个月高位 霍尔木兹海峡受阻持续](https://oilprice.com/Latest-Energy-News/World-News/Asia-Spot-LNG-Prices-Hit-5-Month-High-as-Hormuz-Blockage-Drags-On.html) ⭐️ 9.0/10

亚洲现货 LNG 价格周二升至约每百万英热单位 24.614 美元，为五个月来最高，高于上周五的 23.388 美元。原因是霍尔木兹海峡通行受阻、卡塔尔 LNG 交货的不可抗力延长，以及美伊在一个多月来首次恢复交火。

rss · OilPrice.com · 9月1日 15:30

**「背景」** 霍尔木兹海峡是中东 LNG 和石油外运的关键通道。卡塔尔国营的卡塔尔能源公司已将 LNG 交货的不可抗力（即因不可控事件无法履约）延长至 11 月，美伊交火加剧了市场对中东供应中断的担忧。

**「影响」** 巴基斯坦、孟加拉国以及韩国、印度、台湾等正在采购现货的买家可能面临更高的天然气进口成本；欧洲 TTF 基准天然气价格也升至三年多新高，周一涨 5%至约 70 欧元/兆瓦时，周二进一步升至 71.20 欧元/兆瓦时。

**标签**: `#LNG`, `#Energy Prices`, `#Strait of Hormuz`, `#Geopolitics`, `#Natural Gas`

---

<a id="item-finance-news-2"></a>
### [美伊再度互袭推高油价](https://finance.yahoo.com/video/us-iran-exchange-strikes-renewing-194217817.html) ⭐️ 9.0/10

美国和伊朗在一个月内首次直接互相攻击，重燃中东冲突可能延续至 2027 年的担忧，推动油价上涨。目前 ICE 布伦特原油报每桶 92 美元，而中东基准油价已再次突破每桶 100 美元。

openbb · CL=F · 9月1日 19:42

**「背景」** 此前约一个月双方未再直接交火，美国对伊朗的制裁本就令霍尔木兹海峡油轮通行困难；这次袭击中，两艘载有沙特原油的油轮在驶出海峡时遭导弹击中。

**「影响」** 油价上涨加剧通胀担忧，已推高全球债券收益率并提高家庭和企业借贷成本，可能抑制后续石油需求。

**标签**: `#oil prices`, `#geopolitics`, `#Iran`, `#US foreign policy`, `#energy markets`

---

<a id="item-finance-news-3"></a>
### [美联储维持利率不变](https://news.google.com/rss/articles/CBMipAFBVV95cUxOY1hWQlVSY2RxeHd1dGdaVHQ0RWFHWXVOWWdNTmhuNktNVVc2bGE1S29PbW95dHd6Ml9Da05XTEpzNW92aVFEdlY1MUVPaTBtaV9ENDhxNjFYU0FQcFRXZ0Y4TllqYXdOckd3VjhrM0hjWGJjWEJUcy1fOWFibENaNVdHcnNKaDhERE9lTTYyNTExczZWcXFkbjFURUpmMEFldzRMbA?oc=5) ⭐️ 9.0/10

美国联邦储备委员会（美联储）决定维持基准利率不变，未进行加息或降息。

google\_news · Spectrum News · 7月29日 07:00

**「背景」** 美联储在 6 月 16 日至 17 日会议后决定将联邦基金利率维持在 3.5%至 3.75%不变，这是新任主席凯文·沃什上任后的首次政策决定。此前美国经济面临通胀压力上升，本次按兵不动显示美联储暂缓调整利率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-holds-interest-rates-steady-220059911.html?fr=sycsrp_catchall">Federal Reserve Holds Interest Rates Steady At 3.5%-3.75% In ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`

---

<a id="item-finance-news-4"></a>
### [美联储理事巴尔：若通胀未降温将支持加息](https://www.cnbc.com/2026/09/01/fed-governor-barr-says-hell-support-rate-hike-if-inflation-doesnt-ease.html) ⭐️ 8.0/10

美联储理事迈克尔·巴尔表示，如果通胀没有缓解，他将支持上调利率。最新数据显示整体通胀同比上涨 3.7%，市场目前预计本月加息概率约 66%。

rss · CNBC Finance · 9月1日 14:01

**「背景」** 美联储自 7 月以来将基准利率维持在 3.5%-3.75%不变，但通胀已连续近五年半高于 2%的目标。美联储主席凯文·沃什上周的讲话也被市场解读为偏向加息。

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Monetary Policy`, `#Michael Barr`

---

<a id="item-finance-news-5"></a>
### [沙特计划到 2030 年替代逾 100 万桶/日石油消费](https://oilprice.com/Alternative-Energy/Nuclear-Power/Saudi-Arabia-Plans-To-Free-1-Mbd-As-it-Invests-in-Nuclear-Power.html) ⭐️ 8.0/10

沙特阿拉伯计划到 2030 年以天然气和可再生能源替代国内逾 100 万桶/日的石油消费，并押注核电在 2030 年后进一步降低用油量；美国与沙特已于 7 月 22 日签署 30 年民用核合作协议，但核电对 2030 年目标贡献预计有限。

rss · OilPrice.com · 9月2日 00:00

**「背景」** 该计划旨在削减发电厂、海水淡化厂、工厂和农场的用油；EIA 数据显示，2024 年 6 月沙特夏季用电高峰期间发电用原油和燃料油合计达 142 万桶/日。美国核协议 8 月 24 日已提交国会审议，特朗普称协议取决于沙特与以色列建交，但这一条件是否写入协议尚不明确。

**「影响」** 若计划落实，沙特可将原本国内烧掉的石油转为出口，影响全球石油供应；按文中估算，拟建核电站若满负荷并全部替代燃油发电，最多等效约 10.5 万桶/日原油，低于 100 万桶/日的总目标。

**标签**: `#Saudi Arabia`, `#Nuclear Power`, `#Oil Displacement`, `#Energy Policy`, `#US-Saudi Agreement`

---

<a id="item-finance-news-6"></a>
### [锂价大涨与美国大单：美国锂矿商迎来转机](https://oilprice.com/Energy/Energy-General/US-Lithium-Miners-Finally-Have-a-Shot-at-Cashing-In.html) ⭐️ 8.0/10

据彭博报道，中国广受关注的锂现货价格在 2026 年上半年大涨 22%；同时，LG 新能源与 Smackover Lithium 签订十年期协议，从 2029 年起每年采购 8000 吨电池级碳酸锂，美国锂矿商有望借此扩大全球供应份额。

rss · OilPrice.com · 9月1日 20:00

**「背景」** 全球锂供应高度集中，85%的精炼产能来自中国、智利和阿根廷，过去几年因产能扩张快于需求，导致锂价持续波动并抑制了新项目投资。

**「影响」** 这笔长期订单为美国锂矿项目提供了一个稳定的需求基础，但分析师提醒 2027 年后供应增速可能超过需求，长期价格仍存在波动风险。

**标签**: `#lithium`, `#energy storage`, `#supply chain`, `#mining`, `#battery materials`

---

<a id="item-finance-news-7"></a>
### [坦桑尼亚矿业改革见效：黄金出口创纪录](https://oilprice.com/Energy/Energy-General/Tanzanias-Mining-Model-Is-Starting-to-Pay-Off.html) ⭐️ 8.0/10

据 Oilprice.com 报道，坦桑尼亚矿业改革正在见效：2021 年以来矿业相关税收和特许权使用费收入增加一倍以上，去年黄金出口同比增长 38.2%至 47 亿美元，创纪录，矿业对 GDP 的贡献首次超过 10%。

rss · OilPrice.com · 9月1日 17:00

**「背景」** 2017 年以来，坦桑尼亚修订《矿业法》，规定政府在大规模采矿许可中持有 16%的不稀释干股（无需出资即可享有的权益），并要求本地企业在采矿和服务链中持有最低股权，以扭转过去矿产收益大量外流的局面。

**「影响」** 过去四年，该国矿业吸引约 33 亿美元私人投资，表明改革在提高政府收入的同时仍能吸引国际资本。

**标签**: `#Tanzania`, `#mining`, `#critical minerals`, `#gold exports`, `#mining policy`

---

<a id="item-finance-news-8"></a>
### [英国 8 月商店价格通胀创两年多新高，食品通胀升至 2.8%](https://oilprice.com/Energy/Energy-General/Food-Inflation-Jumps-as-Higher-Energy-Costs-Hit-UK-Retailers.html) ⭐️ 8.0/10

英国零售商协会（BRC）数据显示，英国商店价格通胀在截至 8 月的一年里升至 1.5%，高于 7 月的 0.9%，创两年多新高；食品价格通胀从 7 月的 2.2%升至 2.8%。

rss · OilPrice.com · 9月1日 16:00

**「背景」** BRC 表示，能源和大宗商品成本上升正开始传导至零售价格；食品通胀在 2026 年大部分时间呈下降趋势后出现反弹。

**「影响」** BRC 警告，未来几个月家庭预算将因账单上涨承压；若中东局势导致霍尔木兹海峡持续关闭，英国央行预测通胀可能超过 4%，并可能加息，推高借贷成本。

**标签**: `#UK inflation`, `#food prices`, `#energy costs`, `#retail`, `#Bank of England`

---

<a id="item-finance-news-9"></a>
### [美国 2026 年第二季度储能装机量创纪录新高](https://oilprice.com/Latest-Energy-News/World-News/US-Energy-Storage-Capacity-Installations-Hit-Record-High-in-Q2.html) ⭐️ 8.0/10

2026 年第二季度美国储能装机创纪录，新增 20.2 吉瓦时（GWh），上半年累计 30.8 吉瓦时。美国太阳能行业协会（SEIA）与基准矿业情报公司（Benchmark Mineral Intelligence）据此将到 2030 年的装机预测上调 11.5%，预计年装机量将超过 110 吉瓦时。

rss · OilPrice.com · 9月1日 14:30

**「背景」** 电网运营商和公用事业公司正用储能提升电网可靠性并满足增长的电力和数据中心需求；增长主要由电网级项目推动，安装范围也从加利福尼亚、得克萨斯扩展到亚利桑那、内华达等州。

**「影响」** 2026 年前八个月，电池储能向电网输送的电量已超过 2025 年全年，显示储能对电力系统的实际支撑作用正在快速上升。

**标签**: `#energy storage`, `#grid reliability`, `#utility-scale`, `#U.S. market`, `#renewable energy`

---

<a id="item-finance-news-10"></a>
### [日本放宽每月 45 小时加班上限](https://www.orientaldaily.com.my/news/international/2026/09/01/844683) ⭐️ 8.0/10

日本自 9 月 1 日起放宽加班规定，劳动标准监察机构不再强制企业遵守每月 45 小时加班上限，此举旨在刺激经济，但被批评为“工作狂”文化回归。约 40%日本企业目前允许每月最多加班 100 小时。

telegram · zaihuapd · 9月1日 12:56

**「背景」** 新规源于首相高市早苗政府 7 月通过的成长策略，此前日本一直在推动缩短工时的改革。

**「影响」** 对日本劳动者而言，新规可能使部分企业增加加班安排；官员提醒，超过 45 小时加班会增加过劳死风险。

**标签**: `#Japan labor policy`, `#overtime regulation`, `#economic stimulus`, `#workplace reform`, `#labor market`

---

<a id="item-finance-news-11"></a>
### [台积电 2690 亿美元扩张引关注，67.7%毛利率成焦点](https://finance.yahoo.com/markets/stocks/articles/tsmcs-269-billion-expansion-puts-170918317.html) ⭐️ 8.0/10

报道称，台积电正在推进一项 2690 亿美元的扩张计划，其 67.7%的毛利率因此成为关注焦点。

openbb · NVDA · 9月1日 17:09

**「背景」** 台积电（TSMC）正推进在美国亚利桑那州和德国等地的大规模扩产，并因 AI 相关需求强劲，把 2026 年资本支出指引上调至最高 640 亿美元。其 2026 年第二季度毛利率为 67.7%，高于公司自身 65.5%-67.5%的指引区间，净利润同比大增 77.4%。

**「影响」** 业内分析认为，台积电在美国追加约 1000 亿美元扩产可能重塑全球半导体供应链布局和先进制程竞争格局，进而影响芯片制造商及下游电子设备厂商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/9062197/tsmcs-269-billion-expansion-puts-its-677-margin-in-focus">TSMC&#x27;s $269 Billion Expansion Puts Its 67.7% Margin in Focus</a></li>
<li><a href="https://xenospectrum.com/en/tsmc-q2-2026-record-margin-capex/">TSMC Posts 77% Profit Growth with 67.7% Gross Margin: Capex ...</a></li>
<li><a href="https://aitoolsrecap.com/Blog/tsmc-q2-2026-full-earnings-record-profit-arizona-2026">TSMC Q2 2026 Full Earnings: Record Profit +77%, Gross Margin ...</a></li>
<li><a href="https://www.semiconreport.org/en/articles/tsmc-100-billion-us-chipmaking-expansion">TSMC&#x27;s $100 Billion US Expansion: In-depth Analysis of ...</a></li>
<li><a href="https://www.ftcelectronics.com/news/semiconductor-industry-news-july-2026-ai-tsmc-supply-chain">Semiconductor News July 2026: TSMC Investment, AI Chips ...</a></li>
<li><a href="https://www.semiconreport.org/en/articles/tsmc-100-billion-usa-chipmaking-expansion">TSMC invests another $100 billion to expand production in the ...</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductors`, `#capital expenditure`, `#margins`, `#expansion`

---

<a id="item-finance-news-12"></a>
### [通胀数据降温或使沃什领导的美联储维持利率不变](https://news.google.com/rss/articles/CBMisAFBVV95cUxQbDJaOWp0UVZZRVd3MUp5UGNUVk1EOXNybWFfeXRKR2FQYzJsUnJCN3VEU1I2bldJWHFodHlUWXQxcUdzXzVtaTN4RmEyaHlwREhvdVpialZycTYyaFozME5kWWV3MGFqT1hGS00zTnMyQmVDZkZXZTFvT0VGR0RSMU1FMnBiT3dyZFlSQmx5RDRXX0JsZ1dPMy1KOTNteGVOaVJRemdUaDhtWkpmRndEeQ?oc=5) ⭐️ 8.0/10

据路透社报道，通胀数据降温可能让由沃什（Warsh）领导、内部存在分歧的美联储维持现有利率不变。

google\_news · Reuters · 8月14日 07:00

**「背景」** 凯文·沃什（Kevin Warsh）自 2026 年起担任美联储主席。在 2026 年 8 月的杰克逊霍尔会议上，他警告通胀仍然过高，并暗示如果物价压力未缓解，利率可能需要上调。

**「影响」** 若美联储维持利率不变，依赖贷款的家庭和企业将继续面对当前的借贷成本；股市投资者则会密切关注这一决定是否印证市场对利率和经济前景的预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kevin_Warsh">Kevin Warsh - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/08/28/kevin-warsh-jackson-hole-federal-reserve-inflation.html">Fed Chairman Warsh warns on inflation at Jackson Hole - CNBC</a></li>
<li><a href="https://www.npr.org/2026/08/28/nx-s1-5947903/federal-reserve-inflation-jackson-hole-interest-rates">Fed Chair Kevin Warsh warns inflation is still too high : NPR</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/how-do-rising-interest-rates-affect-the-stock-market.html">How Do Changing Interest Rates Affect the Stock Market? | U.S. Bank</a></li>
<li><a href="https://finance.yahoo.com/personal-finance/investing/article/how-are-stocks-impacted-when-the-fed-doesnt-change-interest-rates-154436785.html">How are stocks impacted when the Fed doesn’t change interest rates?</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Monetary Policy`, `#Economy`

---

<a id="item-finance-news-13"></a>
### [美联储维持利率不变，鲍威尔召开记者会](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 8.0/10

据 PBS 报道，美联储在最近一次会议后决定维持利率不变，主席鲍威尔随后举行新闻发布会，说明货币政策立场。

google\_news · pbs.org · 3月18日 07:00

**「背景」** 美联储在最近一次会议决定将短期基准利率维持在约 3.6%不变，这是连续第二次按兵不动；此前该行在去年已三次降息。美联储在声明中还提到，需要关注中东局势发展对美国经济的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-powell-holds-news-briefing-after-latest-interest-rate-decision">WATCH: Fed Chair Powell holds news briefing after interest rate left unchanged | PBS News</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Jerome Powell`, `#Press Conference`

---

<a id="item-finance-news-14"></a>
### [高通宣布 9 月 1 日后出货芯片涨价两位数](https://www.macrumors.com/2026/08/31/qualcomm-chip-price-increase/) ⭐️ 7.0/10

高通将对 2026 年 9 月 1 日后出货的全系列芯片提价，涨幅为两位数，并称原因是供应商成本持续上升；具体涨幅将与客户逐一协商。

telegram · zaihuapd · 9月1日 04:10

**「背景」** 高通 CEO Cristiano Amon 表示，公司无法继续自行承担上涨的供应商成本。苹果仍为 iPhone 17 系列机型采购高通调制解调器芯片。

**「影响」** 采购高通芯片的手机及设备厂商将直接面对芯片采购成本上升；高通称将与客户逐一协商实际涨幅。

**标签**: `#Qualcomm`, `#semiconductor pricing`, `#supply chain`, `#Apple`, `#chip costs`

---

<a id="item-finance-news-15"></a>
### [《微短剧发展管理办法》今日正式施行](https://content-static.cctvnews.cctv.com/snow-book/index.html?item_id=13099489542770738243) ⭐️ 7.0/10

《微短剧发展管理办法》今天起正式施行，这是中国首部专门规范微短剧的部门规章，法律效力高于此前行业指引类文件。该办法按投资额度和题材将微短剧分为三类并设置不同备案审核要求，同时要求制作和播出单位为使用人工智能技术生成的微短剧在每集明显位置添加提示标识。

telegram · zaihuapd · 9月1日 05:19

**「背景」** 此前微短剧行业主要依靠通知、管理提示和专项整治等临时性文件监管；本次《办法》是首部专门针对微短剧的部门规章，经国家广播电视总局 2026 年 7 月 27 日局务会审议通过，自 2026 年 9 月 1 日起施行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nrta.gov.cn/art/2026/7/31/art_113_73785.html">国家广播电视总局 公告公示 国家广播电视总局令第16号：《微短剧发展管理办法》</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33691660">广电总局重磅发布!《微短剧发展管理办法》来了!AI剧纳入监管!9月实施!_澎湃号·湃客_澎湃新闻-The Paper</a></li>
<li><a href="https://www.news.cn/legal/20260731/4b8eea40226644d0a347c72ea1b21b75/c.html">9月1日起，《微短剧发展管理办法》正式施行 - 新华网</a></li>

</ul>
</details>

**标签**: `#regulation`, `#micro-short-dramas`, `#China`, `#AI-content-labeling`, `#media-industry`

---

<a id="item-finance-news-16"></a>
### [三部门发布汽车行业境外竞争与合规指引](https://weibo.com/1664176597/Rg5PKzXXE) ⭐️ 7.0/10

商务部、工业和信息化部、市场监管总局联合发布《汽车行业境外竞争行为与合规建设指引》，要求中国车企在海外依法合规定价，不得通过低价倾销等不正当方式扰乱市场秩序，并鼓励与当地产业链合作、履行社会责任。

telegram · zaihuapd · 9月1日 08:15

**「背景」** 该指引由商务部、工业和信息化部、市场监管总局联合印发，属于供企业参考的指导性文件，旨在引导车企在境外依法依规定价、避免低价倾销，并与当地产业链合作。

**「影响」** 该指引将影响计划或正在出海的中国汽车企业，要求其在海外定价和竞争行为中加强合规管理，避免低价倾销，并注重与当地产业链合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stcn.com/article/detail/4167297.html">三部门发布《汽车行业境外竞争行为与合规建设指引》</a></li>
<li><a href="https://www.ithome.com/0/996/965.htm">ithome.com/0/996/965.htm</a></li>
<li><a href="https://news.smm.cn/news/104091526">news.smm.cn/news/104091526</a></li>
<li><a href="https://www.news.cn/fortune/20260901/b55704c5d68c4a72af88fb675de2efcb/c.html">三部门发布《 汽 车 行 业 境 外 竞 争 行 为 与 合 规 建设 指 引 》-新华网</a></li>

</ul>
</details>

**标签**: `#汽车行业`, `#境外合规`, `#产业政策`, `#反倾销`, `#商务部`

---

<a id="item-finance-news-17"></a>
### [外籍个人股息红利个税税率明确为 20%](https://m.cnfin.com/wx/share?url=//m.cnfin.com/yw-lb//zixun/20260901/4463424_1.html) ⭐️ 7.0/10

财政部和税务总局公告，外籍个人从外商投资企业取得的股息红利所得，自 2026 年 9 月 1 日起按“利息、股息、红利所得”缴纳 20%个人所得税。该政策取代了此前相关免税规定，外商投资企业向外籍个人支付股息红利时应代扣代缴。

telegram · zaihuapd · 9月1日 09:33

**「背景」** 此前，根据财税字〔1994〕20 号文件，外籍个人从外商投资企业取得的股息、红利所得暂免征收个人所得税；此次公告废止了相关条款，并自 2026 年 9 月 1 日起改为按 20%税率征税。

**「影响」** 受影响的是在华外商投资企业及其外籍个人股东：企业需在支付时代扣代缴税款，并在支付所得次月 15 日内申报纳税。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tg.okhk.net/posts/11131">tg.okhk.net/posts/11131</a></li>

</ul>
</details>

**标签**: `#China tax policy`, `#dividend tax`, `#foreign individuals`, `#personal income tax`, `#foreign-invested enterprises`

---