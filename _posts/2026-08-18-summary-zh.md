---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 238 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [DuckDB v2.0 预览发布与社区反响](#item-tech-news-1) ⭐️ 9.0/10
2. [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越更大规模模型](#item-tech-news-2) ⭐️ 9.0/10
3. [Copilot 自动修复在 Snowflake Jira 工作流中引入命令注入漏洞](#item-tech-news-3) ⭐️ 8.0/10
4. [追踪稀有书籍发现亚马逊 AI 训练设施](#item-tech-news-4) ⭐️ 8.0/10
5. [AI;DR：开发者对 AI 生成内容的反感正在蔓延](#item-tech-news-5) ⭐️ 7.0/10
6. [如何让任意稀疏注意力/KV 压缩看起来效果很好？](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [战争与干旱冲击全球关键航运通道](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储维持利率不变，三名决策者反对加息](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储维持利率不变，为伊朗战争推高油价后首次决定](#item-finance-news-3) ⭐️ 9.0/10
4. [美联储维持利率不变，鲍威尔举行记者会](#item-finance-news-4) ⭐️ 9.0/10
5. [中国上半年弃风弃光电量创纪录](#item-finance-news-5) ⭐️ 8.0/10
6. [苹果调整 App 广告数据授权规则以回应德国反垄断裁定](#item-finance-news-6) ⭐️ 8.0/10
7. [布伦特原油逼近 89 美元，霍尔木兹海峡持续中断](#item-finance-news-7) ⭐️ 8.0/10
8. [特朗普威胁轰炸阿曼后美股下跌、油价上涨、30 年期美债收益率创 19 年新高](#item-finance-news-8) ⭐️ 8.0/10
9. [30 年期美债收益率升至 2007 年以来最高](#item-finance-news-9) ⭐️ 8.0/10
10. [美联储主席沃什在维持利率不变后举行记者会](#item-finance-news-10) ⭐️ 8.0/10
11. [美联储维持利率不变，9 票赞成 3 票反对](#item-finance-news-11) ⭐️ 8.0/10
12. [美联储即将召开多年来最难预测的会议](#item-finance-news-12) ⭐️ 8.0/10
13. [美联储维持利率不变 暗示未来仍可能加息](#item-finance-news-13) ⭐️ 8.0/10
14. [Stripe 据称以超 70 亿美元收购 AI 模型聚合商 OpenRouter](#item-finance-news-14) ⭐️ 7.0/10
15. [宇树科技 8 月 19 日科创板上市，发行价 150.8 元](#item-finance-news-15) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DuckDB v2.0 预览发布与社区反响](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

DuckDB 官方博客发布了 v2.0 预览，页面时间标注为 2026 年 8 月 17 日。作为广泛使用的嵌入式分析数据库，这一主要版本预览在 Hacker News 引发大量关注。社区用户对 Quack 等新内容感到兴奋，并肯定 DuckDB 在分析处理、空间支持、dbt 集成以及消费级硬件上超内存数据处理方面的表现。也有评论指出项目在不到 6 个月内约有 1 万次提交，引发了关于 AI 辅助开发程度的讨论。当前仍是预览版，具体特性与性能变化需要等待官方正式发布说明。

hackernews · ibotty · 8月17日 13:46 · [社区讨论](https://news.ycombinator.com/item?id=49330781)

**「背景」** DuckDB 是一个进程内分析型数据库，以嵌入式、高性能和易于使用著称。此次预览的 v2.0 是其主要版本更新，官方计划于今年秋季发布。该版本将引入服务器模式、触发器、VARIANT 类型、异步 I/O、新的 SQL 解析器和新的存储格式等多项重大变化。

**「影响」** 对已在使用 DuckDB 进行分析、dbt 管线或运行时数据处理的数据工程团队，v2.0 预览显示该项目正继续朝更低资源占用和更大数据处理能力演进，可能进一步降低生产环境的硬件与成本需求；但最终影响取决于正式版的发布内容和稳定性。

**「社区讨论」** 社区整体对 DuckDB 高度认可，多名开发者表示自 2023 年起在多家公司引入后显著降低了资源需求，并能在低端消费级硬件上处理超出内存的数据。与此同时，部分用户希望增加增量物化视图，也有人质疑近 6 个月约 1 万次提交中 AI 的参与程度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://duckdb.org/2026/08/17/duckdb-20-highlights">A Preview of DuckDB v2.0 – DuckDB</a></li>
<li><a href="https://duckdblab.org/en/post/duckdb-upcoming-v2-roadmap-preview/">DuckDB 1.5.4 Released: Stability Enhancements and v2.0.0 Preview</a></li>

</ul>
</details>

**标签**: `#duckdb`, `#database`, `#analytics`, `#data-engineering`, `#release`

---

<a id="item-tech-news-2"></a>
### [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越更大规模模型](https://artificialanalysis.ai/models/qwen3-8-27b) ⭐️ 9.0/10

根据 Artificial Analysis 的评测，Qwen3.8 27B 获得 52 分，超越了 Opus 4.6 等远大于它的模型，并与 DeepSeek V4 Flash 0731 得分相同；该 27B 小模型同时超过中档（40B–150B）模型，社区认为这对 AI 效率和部署经济性有重要意义。评论者提到前代 Qwen3.6 27B 为 38 分，曾是 4B–40B 类别最高，而新版本直接跨越多个规模类别。用户实测称其在高推理等级下表现出强烈的 agentic 行为、目标跟踪和工具调用，甚至接近 GPT-5.6-Sol-max 的执著风格。由于来源缺乏官方发布说明，具体参数量、训练数据和评测协议等细节仍需进一步确认。

hackernews · anana\_ · 8月17日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=49334544)

**「背景」** Artificial Analysis 智能指数（Intelligence Index）是一个综合基准，衡量大语言模型的推理与综合能力，分数越高代表模型能力越强；据该网站数据，Qwen 3.8 27B 在该指数上得到 52 分，显著高于同类模型的中位数 9 分。Qwen 系列是阿里巴巴开源的高效模型系列，前代 Qwen 3.6 27B 在 40 亿至 400 亿参数的小模型类别中已是最高分之一（38 分），而 3.8 版本以 27B 参数量在第 3 方测试中拿到了与 DeepSeek V4 Flash 0731 相同的 52 分，并超过了参数量远大于它的前沿模型，这体现了模型缩放和训练效率方面的显著进展。

**「影响」** 由于 27B 模型可在消费级游戏 PC 上运行，这一成绩可能降低企业本地部署前沿级模型的硬件门槛，并加剧关于大型数据中心投资必要性的讨论。

**「社区讨论」** 评论者普遍震惊于小模型超过 6 个月前的 SOTA Opus 4.6，并认为这是一次“离谱”的发布；同时也有用户表示将进行更广泛测试，因为仅凭基准分数还不足以判断实际编码能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen 3 . 8 27 B - Intelligence, Performance &amp; Price Analysis</a></li>
<li><a href="https://www.orcarouter.ai/blog/qwen-3-8-27b-benchmarks">Qwen 3 . 8 - 27 B Benchmarks: Full Table, Sourced &amp; Ranked</a></li>

</ul>
</details>

**标签**: `#AI benchmarks`, `#Qwen`, `#model efficiency`, `#open source`, `#scaling`

---

<a id="item-tech-news-3"></a>
### [Copilot 自动修复在 Snowflake Jira 工作流中引入命令注入漏洞](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

Wiz 发布的一篇博客披露，GitHub Copilot 的 AI 自动修复功能在 Snowflake 的 Jira 工作流中引入了一个命令注入漏洞。具体问题出现在 .github/workflows/jira\_issue.yml 中，静态分析工具报告了通过模板展开产生的代码注入（template-injection）。该案例表明，未经安全审查的 AI 生成代码可能给 CI/CD 管道带来严重风险。分析强调，开发者需要像对待普通代码一样对 AI 生成代码进行静态分析、SAST 和 SCA 扫描，而不能直接信任自动修复结果。

hackernews · galnagli · 8月17日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=49331423)

**「背景」** Wiz 的 Red Agent 团队独立发现并利用了一个由 GitHub Copilot Autofix 自动修复引入的 GitHub Actions 注入漏洞，该漏洞存在于 Snowflake 的内部 Jira 工作流中。攻击者仅需在 GitHub issue 标题中精心构造内容，即可触发命令注入，因为工作流将未经充分转义的用户输入直接拼接到 shell 命令中。这一事件凸显了 AI 生成的代码同样需要经过静态分析和安全审查，不能仅依赖 AI 的自动修复建议。

**「影响」** 该事件为所有使用 AI 辅助编码并依赖 Copilot 自动修复 CI/CD 工作流的组织敲响警钟：如果不对 AI 生成代码进行自动化和人工安全审查，就可能将命令注入等漏洞直接引入生产管道。Snowflake 的具体 Jira 工作流已被发现存在该问题，但尚不清楚是否已被实际利用。

**「社区讨论」** 评论区多数观点认为这是人为疏忽，而不是 AI 本身的问题，强调 AI 生成的代码必须经过与开发者代码同等的质量与安全检查，并建议在 CI 中使用 zizmor 等静态分析工具。也有用户指出 Copilot 自动修复试图简化已弃用的 Atlassian Jira Actions，但修改过程中引入了漏洞；另有用户质疑漏洞与所引用 PR 的实际关联，因为 PR 中与 Copilot 相关的提交并不涉及该漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug">Red Agent Exploits Snowflake Vuln Missed by Github Copilot ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#GitHub Copilot`, `#CI/CD`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [追踪稀有书籍发现亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

404 Media 的一项调查通过在稀有书籍订单中放置 Apple AirTag，追踪到该批约 1000 本书最终被送往拉斯维加斯东北部的亚马逊 LAS8 设施 VGT3 区域，该设施入口标有恐龙啃书的标志。亚马逊员工在论坛中确认 VGT3 会破坏性地扫描大量书籍，证实了图书经销商长期怀疑的匿名大额订单用于 AI 训练数据采集。此事与 2025 年 6 月 Anthropic 书籍扫描事件相呼应，进一步凸显 AI 公司从实体书扫描获取训练数据引发的版权争议。

rss · Simon Willison · 8月17日 15:21

**「背景」** 404 Media 调查人员在 Biblio 平台上一笔约 1000 本罕见书籍的订单中放入了一枚 AirTag，追踪后发现这本书最终被送到拉斯维加斯东北部亚马逊 LAS8 设施的 VGT3 区域，那里据称有团队会将书籍拆下书脊并进行破坏性扫描，用于 AI 训练。此前书商长期怀疑有匿名大客户批量购书是为了扫描成训练数据，例如 2025 年 6 月就有关于 Anthropic 扫描书籍的报道；这次调查为这些猜测提供了具体的实物证据。

**「影响」** 此次调查证实，亚马逊在拉斯维加斯 LAS8 设施的 VGT3 区域会破坏性地扫描大批量采购的稀有图书用于 AI 训练，这对图书经销商、藏书者以及 AI 训练数据合法性的争议都有直接影响，因为此类订单通常来自不关心价格的匿名买家，且图书在扫描后被销毁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-training-facility/">We Tracked a Shipment of Rare Books. It Ended at an Amazon AI ...</a></li>
<li><a href="https://techcrunch.com/2026/08/17/amazon-once-an-online-bookseller-is-destroying-rare-books-to-train-ai-models/">Amazon, which started off selling books, is destroying rare ...</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/08/hidden-airtag-reveals-amazon-is-trashing-rare-books-to-train-ai/">Hidden Airtag reveals Amazon is trashing rare books to train AI</a></li>
<li><a href="https://techcrunch.com/2026/08/17/amazon-once-an-online-bookseller-is-destroying-rare-books-to-train-ai-models/">Amazon, which started off selling books, is destroying rare ...</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/08/hidden-airtag-reveals-amazon-is-trashing-rare-books-to-train-ai/">Hidden Airtag reveals Amazon is trashing rare books to train AI</a></li>
<li><a href="https://lithub.com/now-amazon-is-destroying-rare-books-to-train-its-ai/">Now Amazon is destroying rare books to train its AI.</a></li>

</ul>
</details>

**标签**: `#AI`, `#data`, `#Amazon`, `#books`, `#investigation`

---

<a id="item-tech-news-5"></a>
### [AI;DR：开发者对 AI 生成内容的反感正在蔓延](https://www.rickmanelius.com/p/aidr-ai-didnt-read) ⭐️ 7.0/10

这篇在 Hacker News 上引起讨论的观点文章以“AI;DR（AI；没读）”为题，讨论了人们对 AI 生成内容日益强烈的反感，以及这种反感在代码审查和在线交流中的体现。文章并非孤立的技术批评，而是围绕一个真实工作场景的共鸣：越来越多开发者发现，AI 编写的文档和逐行注释让代码库变得冗长、空洞且难以阅读。评论中提出的具体问题包括过度自信、术语滥用、缺乏 nuance，以及读者怀疑这些内容来自“智力懒惰”。有评论者建议，与其把 AI 生成的输出发给别人，不如告诉对方你当初使用的 prompt，因为只有 prompt 才包含你真正想传达的信息。整体上，社区正在从“可以使用 AI”转向“请别用 AI 来填满我的阅读时间”。

hackernews · mooreds · 8月17日 19:47 · [社区讨论](https://news.ycombinator.com/item?id=49336573)

**「背景」** “AI;DR”（AI；没读）是一个新兴的网络简写，用来表达读者因为怀疑内容是 AI 生成的而选择不阅读。支持这种做法的人常认为，AI 生成内容来自“智力懒惰”，且往往冗长、充满行话、过度自信，缺乏人类写作中的细微差别；在代码评审和工作沟通中，这种内容会损害可读性与信任。这一趋势反映出现有 AI 工具在专业场景中的局限，也推动了关于如何在写作中保留“人格”和真实表达的讨论。

**「影响」** 对于软件工程师和依赖代码审查的团队，最直接的后果是 AI 生成注释和文档可能显著破坏代码库可读性，甚至有开发者形容自己的代码库已经进入“后可读性”状态；因此，分享真实意图（例如原始 prompt）而不是成品 AI 文本，正成为一种被推荐的沟通方式。

**「社区讨论」** 评论者大多认同 AI 内容令人反感：gortok 认为在 2026 年把 AI 回复贴给别人“不可接受且令人厌恶”，afr0ck 则将反感归因于智力懒惰感、冗长、过度自信和缺少 nuance。LPisGood 报告了实际工作后果——每个 PR 里都有大量 AI 文档和注释，代码库基本失去可读性；cortesoft 提出“直接发 prompt，而不是 AI 输出”，因为它才包含真正想传达的信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49336573">AI ; DR ( AI ; Didn &#x27; t Read ) | Hacker News</a></li>
<li><a href="https://www.theframeworks.com/frame-of-mind/the-prompt-ai-didnt-read-why-audiences-are-craving-personality">The Prompt: AI ; didn ’ t read . Why audiences are craving personality</a></li>

</ul>
</details>

**标签**: `#AI-generated content`, `#code review`, `#documentation`, `#software engineering`, `#Hacker News`

---

<a id="item-tech-news-6"></a>
### [如何让任意稀疏注意力/KV 压缩看起来效果很好？](https://www.reddit.com/r/MachineLearning/comments/1vqqqcs/how_to_make_any_sparse_attention_kv_compression/) ⭐️ 7.0/10

一位机器学习从业者在 Reddit 发文，根据多年研究注意力与 KV Cache 压缩的经验，总结了让稀疏注意力或 KV 压缩方法在论文中显得有效的常见评估技巧，并承认自己也犯过这些错误。他指出最配合的三类场景是：单跳检索时没有干扰项且上下文无用的“大海捞针”式合成任务、模型已不再查看上下文的多年旧基准、以及额外示例不会改进结果的少样本上下文学习。他还建议不要隔离自己的贡献：沿用基线作者的“推荐超参数”，只优化自己的方法；用 LLM 写 Triton kernel 而保留基线旧实现；把问题放到上下文之前再宣称无损压缩。在指标上，只报告 RULER 等基准的聚合分数，而不强调在 NIAH-MK3 这类真正压力测试上的退化；在已饱和的任务上，较小的模型即使不经压缩也得分很低，较大模型却可以通过更强的参数容量“吸收”压缩带来的损失。文中还提醒，AIME 只有 30 个样本，4 个种子下 1 分差距不应被视为超越基线。

reddit · r/MachineLearning · /u/korec1234 · 8月17日 12:18

**「背景」** 稀疏注意力（sparse attention）和 KV Cache 压缩是减少大语言模型推理时内存与带宽开销的技术，理想情况下希望在显著压缩或稀疏化后仍保持接近稠密注意力的输出质量。然而，评测设计会严重影响这类方法的表现：模型可以利用局部窗口、attention sinks 和与问题高度字面匹配的答案句来恢复大部分性能，而不需要真正做完整的全局检索。

**「影响」** 对于研究者与工程团队而言，本文提醒：若依赖作者在合成或过时基准上的聚合分数、未隔离超参数与实现优化，则稀疏注意力/KV 压缩方法的报告效果可能无法迁移到真实长上下文或强干扰场景；评估时应加入 NIAH-MK3 等压力测试、做充分的基线和实现公平比较。不过这是个别从业者的经验性视角，并非系统性调研结果。

**标签**: `#sparse attention`, `#KV cache compression`, `#evaluation methodology`, `#machine learning research`, `#LLM inference`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [战争与干旱冲击全球关键航运通道](https://oilprice.com/Energy/Energy-General/War-and-Drought-Are-Choking-the-Worlds-Most-Vital-Trade-Routes.html) ⭐️ 9.0/10

报道称，自今年 3 月初伊朗关闭霍尔木兹海峡以来，这条通常承载全球约 20%石油运输量的水道已对大多数船只关闭；胡塞武装还对沙特船只关闭了曼德海峡，而巴拿马运河和莱茵河也因干旱面临通行限制。

rss · OilPrice.com · 8月17日 18:00

**「背景」** 位于伊朗与阿曼之间的霍尔木兹海峡是中东油气出口的咽喉要道，曼德海峡则连接红海与亚洲航线；巴拿马运河依赖降雨补充船闸用水，莱茵河低水位迫使船只减载以防搁浅。

**「影响」** 依赖这些航线的能源和大宗商品贸易将面临更长的绕行与等待成本：沙特油轮需绕行非洲才能抵达亚洲，欧洲部分原本走莱茵河的货物已改用卡车和铁路。

**标签**: `#trade routes`, `#geopolitics`, `#climate change`, `#supply chains`, `#energy`

---

<a id="item-finance-news-2"></a>
### [美联储维持利率不变，三名决策者反对加息](https://news.google.com/rss/articles/CBMipwFBVV95cUxPcTZRdS1qU1NyM2NYeEoyTVBCdUFERzRDa3ZmelhwYkstWUNlMkc3S2tsUXRHcnhOUnAzMDdHXzY3TXdWa3JFbTE4TWZBeEJBSlRWSWFzSnZxX1VBVTE4ZklGV1JJSlJVTXNyN2VJMV9WWWJ0alNfeFZMZWNYTnJrVUk1SG5rczF0ekk1NXhRZFZQSE40RGx2UGROWlE1YVR3aWZUaVRxbw?oc=5) ⭐️ 9.0/10

据路透社报道，美联储决定维持利率不变，但有三位政策制定者对此表示反对，主张加息。

google\_news · Reuters · 7月29日 07:00

**「背景」** 美联储主席凯文·沃什（Kevin Warsh）曾承诺降低通胀，此次维持利率不变使外界更加关注他将如何兑现这一承诺，而三名政策制定者投票支持加息则凸显委员会内部分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/business/view-fed-holds-rates-steady-three-policymakers-dissent-hike-2026-07-29/">VIEW Fed holds rates steady as three policymakers dissent for ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`

---

<a id="item-finance-news-3"></a>
### [美联储维持利率不变，为伊朗战争推高油价后首次决定](https://news.google.com/rss/articles/CBMilAFBVV95cUxOWVgwU0l2bjYwREJ2NE9WVC1ObnpJa3Qxa2syS0lmUXphVm8zTWpnYVJ5NXpFZmxWYUZlVXpmc3ZFQzk2ZnZlYjNSUHRPb3F1emZhVDdPNEMxak1mM2wzOEZtYnA5dklfUFlfOUdVRU5lSXNmTlhqMy1pUElaMjNBTEFJbV9IRHNkRGt1NHJKVDVFd1Za0gGaAUFVX3lxTE9IOWFDX2MzMVhjUXl2VE1oTGNTTlowMmxkMUZnNEQ1TzhKemJ3TmlSTElmdzVPQ3VmR2E3OGdNLXN2dVBHQ2xiLXl0WWJfdjBUQktuSnNwbTNQV3puQzBJTUVZS295S2lHYU9iQVpFd05FQkw4WmhmZ2EyU3dCUWt0bHNCUy1xX0pHME5ZbVBlZ1RXSkxnSVZ1TWc?oc=5) ⭐️ 9.0/10

美联储决定维持利率不变，这是自伊朗战争推高油价以来的首次利率决定。

google\_news · abcnews.com · 3月18日 07:00

**「背景」** 美联储在伊朗战争推高汽油价格、加大通胀风险后举行了首次议息会议，并决定维持利率不变；这场战争还曾导致油价飙升、股市下跌。

**「影响」** 伊朗战争导致的油价飙升与供应链中断，正加大通胀和衰退风险：高盛估计油价月底或达每桶 150 美元，里士满联储主席也提到历史上油价冲击常与经济衰退同步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://abcnews.com/Business/fed-set-adjust-interest-rates-1st-time-war/story?id=131155455">Fed holds interest rates steady in 1st move since Iran war spiked oil prices - ABC News</a></li>
<li><a href="https://abcnews.com/Business/fed-issue-interest-rate-decision-gas-prices-rise/story?id=135130446">Fed holds interest rates steady as economy weathers resurgent inflation - ABC News</a></li>
<li><a href="https://www.richmondfed.org/press_room/speeches/thomas_i_barkin/2026/barkin_speech_20260327">Driving Through Economic Fog (Still) | Tom Barkin | Richmond Fed</a></li>
<li><a href="https://ca.news.yahoo.com/trump-says-oil-spike-small-003855112.html">Trump says oil price spike is ‘very small price ... - Yahoo News Canada</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#oil prices`, `#Iran`

---

<a id="item-finance-news-4"></a>
### [美联储维持利率不变，鲍威尔举行记者会](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 9.0/10

美联储在最新会议上决定维持利率不变，主席鲍威尔随后举行新闻发布会，就货币政策与经济增长前景回答提问。

google\_news · PBS · 3月18日 07:00

**「背景」** 联邦公开市场委员会（FOMC）是美联储内负责设定基准利率的机构；在 2026 年 4 月 29 日结束的会议上，美联储决定将基准利率维持在原有水平。鲍威尔在会后的记者会上表示，担心外部攻击正在损害美联储这一机构，并称这些攻击可能危及公众真正看重的东西。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.usnews.com/news/business/articles/2026-04-29/fed-likely-to-leave-rates-unchanged-at-what-may-be-powells-last-meeting-as-warsh-to-advance">Powell Plans to Remain on Fed Board, Cites Legal Actions by Trump...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#Jerome Powell`, `#economic outlook`

---

<a id="item-finance-news-5"></a>
### [中国上半年弃风弃光电量创纪录](https://oilprice.com/Latest-Energy-News/World-News/Chinas-Renewables-Boom-Faces-Record-Clean-Power-Curtailments.html) ⭐️ 8.0/10

能源与清洁空气研究中心（CREA）和全球能源监测组织（GEM）发布的报告显示，今年上半年中国弃风弃光电量达 360 太瓦时（TWh），同比上升 49%，创下纪录。报告称，被浪费的清洁电力已超过同期全国电力需求增量。

rss · OilPrice.com · 8月17日 15:30

**「背景」** 中国风电和光伏装机激增，当发电量超出电网可消纳能力时便需要限制出力；同时煤电产能快速扩张，加深了电力系统供应过剩。

**「影响」** 伍德麦肯兹（Wood Mackenzie）分析称，弃电率高企和电价波动对可再生能源项目收入稳定性构成主要风险，高弃电率省份在吸引投资时将面临挑战。

**标签**: `#China`, `#renewable energy`, `#power curtailment`, `#solar`, `#wind`

---

<a id="item-finance-news-6"></a>
### [苹果调整 App 广告数据授权规则以回应德国反垄断裁定](https://www.reuters.com/business/retail-consumer/apple-change-app-data-consent-rules-german-regulator-says-2026-08-17/) ⭐️ 8.0/10

苹果将调整 iPhone 和 iPad 上 App 使用个人数据投放定向广告的授权规则，以回应德国监管机构对其追踪透明度框架（ATT）偏袒自家应用、涉嫌违反竞争规则的裁定；苹果须在裁决送达后四个月内落实，承诺有效期七年，并确保第三方授权弹窗去除劝阻性措辞和符号。

telegram · zaihuapd · 8月17日 12:50

**「背景」** 此前法国和意大利已分别因类似问题对苹果处以 1.5 亿欧元和 9860 万欧元的罚款，德国监管机构此次则直接要求修改授权规则。

**标签**: `#Apple`, `#antitrust`, `#data privacy`, `#digital advertising`, `#regulation`

---

<a id="item-finance-news-7"></a>
### [布伦特原油逼近 89 美元，霍尔木兹海峡持续中断](https://finance.yahoo.com/energy/articles/brent-crude-nears-89-hormuz-065225266.html) ⭐️ 8.0/10

布伦特原油价格接近每桶 89 美元，原因是霍尔木兹海峡的持续中断；同时，埃克森美孚、雪佛龙和壳牌报告了创纪录的现金流。

openbb · BRK-B · 8月17日 06:52

**「背景」** 霍尔木兹海峡是全球最重要的石油运输通道之一，如果出现持续中断，会直接影响全球原油供应和价格。布伦特原油当前约为每桶 87.66 美元，已接近 89 美元；此前在断供担忧最严重时曾单日大涨 5.6%至 95.48 美元。

**「影响」** 这次霍尔木兹海峡中断正在把创纪录的利润带给大型石油公司——根据 The Kobeissi Letter 的数据，包括埃克森美孚、雪佛龙、壳牌、道达尔能源和 BP 在内的前五大国际石油公司在 2026 年第二季度产生了近 700 亿美元的自由现金流，创下历史新高，其中埃克森美孚一家就向股东返还了 94 亿美元；与此同时，依赖石油进口的家庭和企业则面临更高的燃料成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/brendan-hughes-85a347187_breaking-oil-prices-could-spike-to-120-activity-7445692814434217985-RIdh">Oil prices may spike to $120-$130 per barrel due to Strait of Hormuz ...</a></li>
<li><a href="https://oilprice.com/futures/brent/">Brent Crude Oil Futures Contracts | Oilprice.com</a></li>
<li><a href="https://stocktwits.com/news-articles/markets/equity/brent-crude-nears-89-strait-hormuz-xom-cvx-uso-record-cash-flow/cZo6uIKRJKY">Brent Crude Nears $89 As Hormuz Stays Disrupted – Exxon , Chevron ...</a></li>
<li><a href="https://247wallst.com/investing/2026/08/17/oil-profits-have-more-than-doubled-heres-what-trump-escalating-the-iran-war-could-mean-for-xom-and-cvx/">Oil Profits Have More Than Doubled. Here’s What... - 24/7 Wall St.</a></li>

</ul>
</details>

**标签**: `#Brent crude`, `#Strait of Hormuz`, `#oil prices`, `#energy earnings`, `#geopolitical risk`

---

<a id="item-finance-news-8"></a>
### [特朗普威胁轰炸阿曼后美股下跌、油价上涨、30 年期美债收益率创 19 年新高](https://finance.yahoo.com/markets/stocks/articles/us-equity-indexes-slide-trump-211106690.html) ⭐️ 8.0/10

特朗普威胁轰炸阿曼后，美国股市主要指数下跌，原油价格上涨，30 年期美债收益率触及 19 年高点。

openbb · CL=F · 8月17日 21:11

**「背景」** 据报道，特朗普威胁称，如果阿曼妨碍美国与伊朗的谈判，将“炸毁”阿曼；阿曼传统上是美伊之间的重要沟通渠道，并据报正与伊朗讨论霍尔木兹海峡通行问题。该海峡承担全球超过 20%的石油运输，相关威胁加剧了市场对供应中断的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy5dzk0ryzdo">Trump threatens to bomb US ally Oman if it &#x27;gets in the way&#x27; over...</a></li>
<li><a href="https://www.aljazeera.com/news/2026/5/28/why-has-trump-threatened-to-bomb-oman-amid-iran-war-escalation">Why has Trump threatened to bomb Oman , amid Iran... | Al Jazeera</a></li>
<li><a href="https://www.theguardian.com/world/2026/aug/17/donald-trump-threatens-bomb-oman">Donald Trump threatens to bomb Oman if it ‘gets in... | The Guardian</a></li>

</ul>
</details>

**标签**: `#US equities`, `#crude oil`, `#Treasury yields`, `#geopolitical risk`, `#market reaction`

---

<a id="item-finance-news-9"></a>
### [30 年期美债收益率升至 2007 年以来最高](https://www.barrons.com/articles/30-year-yield-level-oil-d97d62f8?siteid=yhoof2&amp;yptr=yahoo) ⭐️ 8.0/10

据巴伦周刊，30 年期美国国债收益率升至 2007 年以来最高水平，主要受油价上涨和美国国债供应增加影响。

openbb · CL=F · 8月17日 21:04

**「背景」** 30 年期美国国债收益率是长期借贷成本的重要参考，上升意味着债券价格下跌，并会传导至房贷等长期利率。据市场数据，8 月 17 日该收益率一度升至 5.311%，为 2007 年 6 月以来最高，近期上行主要受油价带来的通胀压力和国债供应增加影响。

**「影响」** 30 年期美债收益率攀升可能推高房贷、企业贷款和汽车贷款等各类借贷成本，因为这些利率在一定程度上参考国债收益率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/17/treasury-yields-federal-reserve-fomc-minutes.html">30-year Treasury yield tops 5.31%, the highest in 19 years</a></li>
<li><a href="https://www.axios.com/2026/08/17/treasury-yields-warsh-bonds">What rising Treasury yields are telling us - Axios</a></li>

</ul>
</details>

**标签**: `#Treasury yields`, `#30-year bond`, `#interest rates`, `#bond market`, `#oil prices`

---

<a id="item-finance-news-10"></a>
### [美联储主席沃什在维持利率不变后举行记者会](https://news.google.com/rss/articles/CBMivgFBVV95cUxNR1BZa2dPa1lOcjNBSmF2MHFHcTNBTV9mQzZOZ3BzR1ZrekhVWUhzLWszajBVWExhYWxJUWJDejh4SjBTdFdobFk1Y1NlMEpad0I4cUtrY0o1VzhMYmNOX2tuWjF3dXhGbkFVOWJncnZDdEt2dUEydkhhX2pwQXZlaF96QTZ3Z2l3OURfN2lLaVRRcEFLejhVTGZVSEl4XzJLWmE0RmxKRy16Mkh2ZGJvbm0wMUExTU83dHVJUlRn0gHDAUFVX3lxTE9kWHZBeUc3cjFTeGNrQk5QeGl2cHpycW5zR19kQl9vbEY3MzdUX0ZCa2pmV0RNT1VSUElKTEhhNmRmaVVnc1k5R0V2RkhTYkJROUZ3YXZmVjlPSWZ5MWVTWkxYS1B3ai1BZnRVeTE5bmR6Mm01eHlDYlpJblAta3hYSnN5Tnhzc19ZRjJwUWVTZzNRQXd0MUJGU29NRko2aVVuTTByMndYeWU3bTRXNWpEeFBlVDF5RTBUU1VaQUdlT1RlRQ?oc=5) ⭐️ 8.0/10

据 PBS 报道，美联储主席沃什在央行决定将利率维持不变后举行了记者会。报道未提供利率目标区间的具体数字或进一步政策细节。

google\_news · PBS · 7月29日 07:00

**「背景」** 美联储在为期两天的议息会议后决定维持基准利率不变，利率保持在 3.5%至 3.75%区间（约 3.6%），这是连续第五次会议和连续第七个月按兵不动；主席沃什随后举行新闻发布会解释这一决定。

**「市场影响」** 新闻发布会后，债券投资者下调了近期加息的可能性，但推高了长期美国国债收益率，因为沃什拒绝说明触发加息的具体条件，令市场对其抗通胀可信度产生疑虑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/economy/watch-live-fed-chair-warsh-holds-news-conference-after-latest-interest-rate-decision">WATCH: Fed chair Warsh holds news conference after leaving interest rate unchanged | PBS News</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-meeting-today-live-updates.html">Fed meeting recap: Warsh says Fed won&#x27;t hesitate to stop inflation, but bond market has doubts</a></li>
<li><a href="https://www.cnn.com/2026/07/29/business/live-news/federal-reserve-interest-rate-07-29-26">Fed holds interest rates steady after cliffhanger meeting, but three officials dissent | CNN Business</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/kevin-warsh-fed-treasury-yields-inflation-credibility-interest-rates.html">Analysis: Fed Chairman Warsh&#x27;s credibility in question after leaving interest rates unchanged</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-meeting-today-live-updates.html">Fed meeting recap: Warsh says Fed won&#x27;t hesitate to stop inflation, but bond market has doubts</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Press Conference`, `#Central Bank`

---

<a id="item-finance-news-11"></a>
### [美联储维持利率不变，9 票赞成 3 票反对](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 8.0/10

美联储在 9 比 3 的投票中决定维持利率不变，没有调整当前利率水平。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储在 7 月 29 日会议上以 9 比 3 的投票结果决定维持利率不变，将联邦基金利率目标区间保持在 3.5%至 3.75%，这一水平自 1 月以来一直未变；三位委员投票支持加息，据 ABC7 报道，9 月会议加息已被普遍预期。

**「影响」** 美联储维持利率不变，使美国消费者和企业中与联邦基金利率挂钩的可变利率贷款借款成本继续保持在 3.50%至 3.75%的水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>
<li><a href="https://abc7chicago.com/post/federal-reserve-is-expected-keep-rates-unchanged-now-despite-high-prices/19595693/">Federal Reserve leaves interest rate unchanged in 9-3 vote - ABC7 Chicago</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Divided Fed holds interest rates steady, but three members voted to hike</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-12"></a>
### [美联储即将召开多年来最难预测的会议](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 8.0/10

据《华尔街日报》报道，美联储即将召开的会议是近年来最不可预测的一次，会议结果可能意味着重大政策调整，但具体决定尚不确定。

google\_news · WSJ · 7月23日 07:00

**「背景」** 美联储即将召开会议，外界对维持利率不变还是加息存在多年未有的不确定性。此前美联储已将联邦基金利率目标区间维持在 3.5%–3.75%，若此次按预期按兵不动，将是连续第五次会议不加息。

**「影响」** 如果美联储调整基准利率，这一变动可能通过影响其他短期利率、长期利率和汇率，进而波及家庭和企业的借贷成本以及整体价格水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/article/fed-expected-to-hold-rates-steady--but-an-interest-rate-hike-isnt-off-the-table-090000519.html">Fed expected to hold rates steady — but an interest rate hike isn&#x27;t off...</a></li>
<li><a href="https://www.linkedin.com/posts/fi-plan-partners-llc_fed-on-the-case-activity-7488979318728065024-fAYr">Fed Holds Rates Steady, Market Expectations Shift | Fi Plan... | LinkedIn</a></li>
<li><a href="https://www.federalreserve.gov/monetarypolicy/fomc.htm">The Fed - Federal Open Market Committee - Federal Reserve Board</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Monetary Policy`, `#Interest Rates`, `#Central Bank`, `#Markets`

---

<a id="item-finance-news-13"></a>
### [美联储维持利率不变 暗示未来仍可能加息](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

美联储宣布维持基准利率不变，同时表示未来仍可能加息。

google\_news · cbsnews.com · 6月17日 07:00

**「背景」** 美联储在 7 月 29 日结束的会议上将联邦基金利率（银行间隔夜贷款基准利率）维持在 3.5%至 3.75%区间，但投票结果为 9 比 3，三名政策制定者希望加息。此前 6 月会议显示，近半数美联储官员支持今年晚些时候加息；美联储主席凯文·沃什曾承诺抑制通胀。

**「影响」** 由于美联储将利率维持在 3.50%–3.75%的目标区间（连续第五次保持不变），家庭和企业的贷款与按揭成本短期内保持稳定，但政策制定者仍保留未来加息空间，借贷成本之后仍可能上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Fed rate decision July 2026: Divided Fed holds interest rates ...</a></li>
<li><a href="https://www.reuters.com/business/view-fed-holds-rates-steady-three-policymakers-dissent-hike-2026-07-29/">VIEW Fed holds rates steady as three policymakers dissent for ...</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Economy`

---

<a id="item-finance-news-14"></a>
### [Stripe 据称以超 70 亿美元收购 AI 模型聚合商 OpenRouter](https://www.bloomberg.com/news/articles/2026-08-16/stripe-nears-deal-to-buy-ai-firm-openrouter-for-over-7-billion) ⭐️ 7.0/10

据知情人士透露，Stripe 已与 AI 模型聚合商 OpenRouter 达成收购协议，金额超过 70 亿美元，但最终价格仍可能变动。Stripe 发言人称不评论传闻或猜测，OpenRouter 未回应置评请求。

telegram · zaihuapd · 8月17日 01:19

**「背景」** OpenRouter 成立于 2023 年，是一个让开发者通过统一接口访问 400 多个 AI 模型的平台，据其称已服务 800 万名开发者；Stripe 则是支付基础设施公司，收购后可将模型调用与计费、路由结合。此前已有双方谈判的报道，最终价格仍可能变动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/stripe-acquires-openrouter-7b-turning-091812340.html?fr=sycsrp_catchall">Stripe Acquires OpenRouter for $7B+, Turning Model Routing ...</a></li>
<li><a href="https://www.techtimes.com/articles/324688/20260817/stripe-closes-7-billion-openrouter-deal-payment-giant-now-bills-routes-ai-traffic.htm">Stripe Closes $7 Billion OpenRouter Deal: Payment Giant Now ...</a></li>
<li><a href="https://fortune.com/2026/08/16/stripe-7-billion-deal-ai-firm-openrouter-acquisition/">Stripe clinches over $7 billion deal to buy AI firm OpenRouter</a></li>

</ul>
</details>

**标签**: `#M&amp;A`, `#Stripe`, `#OpenRouter`, `#AI`, `#payments`

---

<a id="item-finance-news-15"></a>
### [宇树科技 8 月 19 日科创板上市，发行价 150.8 元](https://wap.eastmoney.com/a/202608173843415437.html) ⭐️ 7.0/10

据公司公告，宇树科技（688836.SH）将于 2026 年 8 月 19 日在科创板上市，发行价为 150.80 元/股；按 2025 年摊薄后静态数据计算，发行价对应市销率 35.89 倍，高于可比公司平均水平。

telegram · zaihuapd · 8月17日 13:20

**「背景」** 宇树科技是一家 2016 年创立的中国民用机器人公司，总部位于浙江杭州，主要研发和生产四足机器人等产品。

**「影响」** 发行价格对应 2025 年摊薄后静态市销率 35.89 倍，高于可比公司平均水平，相当于抬高机器人板块的估值对标，可能促使投资者重新评估科创板及港股同类机器人公司的定价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/%E5%AE%87%E6%A0%91%E7%A7%91%E6%8A%80">宇树科技 - 维基百科，自由的百科全书</a></li>
<li><a href="https://baike.baidu.com/item/%E5%AE%87%E6%A0%91%E7%A7%91%E6%8A%80%E8%82%A1%E4%BB%BD%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8/66925085">宇树科技股份有限公司 - 百度百科</a></li>

</ul>
</details>

**标签**: `#IPO`, `#Unitree`, `#Robotics`, `#STAR Market`, `#Valuation`

---