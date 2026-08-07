---
layout: default
title: "Horizon Summary: 2026-08-07 (ZH)"
date: 2026-08-07
lang: zh
---

> 从 187 条内容中筛选出 26 条重要资讯。

---

**科技新闻**
1. [DeepSeek V4 Flash 0731：低成本高吞吐，稳定性存疑](#item-tech-news-1) ⭐️ 8.0/10
2. [批处理、算子融合与 SIMD 让 Postgres 分析查询提速数百倍](#item-tech-news-2) ⭐️ 8.0/10
3. [Kitesurf：在 V8 隔离中运行的代理优先浏览器](#item-tech-news-3) ⭐️ 8.0/10
4. [2027 年内存产能据报已售罄，AI 与 HBM 需求成主因](#item-tech-news-4) ⭐️ 8.0/10
5. [150 万页站点的爬虫对抗一年](#item-tech-news-5) ⭐️ 8.0/10
6. [SpaceX 2027 年 10GW 目标：3000 亿美元 ARR 与微软最大买家前景](#item-tech-news-6) ⭐️ 8.0/10
7. [OpenAI 警告 Astra 或达关键网络攻击能力，发布可能推迟](#item-tech-news-7) ⭐️ 8.0/10
8. [Oracle 禁止 OpenJDK 贡献使用 AI 生成代码](#item-tech-news-8) ⭐️ 7.0/10
9. [新墨西哥州法院判 Meta 付 5.67 亿美元儿童心理健康赔偿](#item-tech-news-9) ⭐️ 7.0/10
10. [Codex 与 GPT-5.6 Sol 生成更佳浣熊抢匪游戏](#item-tech-news-10) ⭐️ 7.0/10
11. [Token 末日来临：企业忙着降低 AI 花费](#item-tech-news-11) ⭐️ 7.0/10
12. [美国审查中国 AI 企业海外获取英伟达芯片渠道](#item-tech-news-12) ⭐️ 7.0/10
13. [SK 海力士确认 V10 NAND 为 375 层堆叠并首次导入晶圆键合](#item-tech-news-13) ⭐️ 7.0/10
14. [sub2api 高危 OAuth 漏洞可仅凭邮箱接管账户](#item-tech-news-14) ⭐️ 7.0/10
15. [亚马逊严查内部 CPU 浪费](#item-tech-news-15) ⭐️ 7.0/10

**财经新闻**
1. [美国海关已支付 1000 亿美元 IEEPA 关税退款](#item-finance-news-1) ⭐️ 9.0/10
2. [7 月就业数据疲软，美联储 9 月加息概率大降](#item-finance-news-2) ⭐️ 8.0/10
3. [纳斯达克 23 小时交易制获 SEC 批准，将于 2026 年 12 月 6 日上线](#item-finance-news-3) ⭐️ 8.0/10
4. [上汽通用宣布雪佛兰退出在华新车零售，750 万车主售后转别克渠道](#item-finance-news-4) ⭐️ 8.0/10
5. [北京下调非京籍购房社保年限至 1 年，提高公积金贷款额度](#item-finance-news-5) ⭐️ 8.0/10
6. [强生公司就滑石粉诉讼达成 55 亿美元和解](#item-finance-news-6) ⭐️ 8.0/10
7. [财报和指引引发美股盘前个股大幅波动](#item-finance-news-7) ⭐️ 7.0/10
8. [澳大利亚拟为外卖骑手设每小时 31.30 澳元最低收入保障](#item-finance-news-8) ⭐️ 7.0/10
9. [莫尔森库尔斯第二季度盈利超预期](#item-finance-news-9) ⭐️ 7.0/10
10. [帝亚吉欧初步财报显示北美市场疲软，烈酒行业或承压](#item-finance-news-10) ⭐️ 7.0/10
11. [Constellation Energy 签署 920 兆瓦新购电协议，含沃尔玛合同](#item-finance-news-11) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DeepSeek V4 Flash 0731：低成本高吞吐，稳定性存疑](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek V4 Flash 0731 是 DeepSeek V4 Flash 的新版本（并非数月前发布的 preview）。社区实测称它比 preview 整体提升了一档，适合调试、文档/数据分析，且成本很低；例如在 Oh My Pi 中同时开 5–6 个会话（约 12 个流）每天花费仍难超过 5 美元，OpenCode Go 临时双倍额度让 10 美元约等于 140 美元的 token。本地推理方面，在 2× RTX Pro 6000 Blackwell 上预填充约 8k tok/s、单流约 250 tok/s。不过也有用户反馈新版在 agent 场景下易陷入无限循环、不执行工具调用并浪费 token，与 preview 相比稳定性存疑。该版本出现在 ARC Prize 结果页，说明其作为高性价比强模型受到社区关注。

hackernews · tosh · 8月7日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49214008)

**「背景」** DeepSeek V4 Flash 0731 是 DeepSeek 于 2026 年 7 月 31 日发布的 Flash 系列效率版模型的正式公开版本，而非此前几个月推出的预览版。根据其模型卡，该模型在激活参数规模远小于 V4-Pro 预览版的情况下，在多项基准测试中表现更优，并与最强的专有模型大致相当；同时支持 1M 上下文窗口，并在 GPQA 等基准上取得高分。

**「影响」** 对在 agent/编码工具中依赖 DeepSeek 的开发者而言，这个版本最具体的收益是极低的使用成本和很高的本地/API 吞吐，使全天候多会话推理变得现实；但工具调用循环等稳定性问题意味着不能无监督地直接用于复杂 agent 流程。

**「社区讨论」** 社区态度分成两派：多数人认可其性能、速度和性价比，甚至称可“几乎什么都用”；但有人报告与上一版相比出现无限循环、不与工具交互、话题跳转等倒退，要求先观察稳定性的声音也存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek -ai/ DeepSeek - V 4 - Flash - 0731 · Hugging Face</a></li>
<li><a href="https://hokai.io/hub/models/deepseek-v4-flash-0731">DeepSeek - V 4 - Flash - 0731 : 1M Context &amp; GPQA 88.1 (2026) | HokAI</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#large-language-models`, `#arc-agi`, `#model-release`, `#ai-inference`

---

<a id="item-tech-news-2"></a>
### [批处理、算子融合与 SIMD 让 Postgres 分析查询提速数百倍](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

这篇文章介绍了一个面向 Postgres 的新查询引擎，通过批处理（batching）、算子融合（operator fusion）和 SIMD 指令，将分析查询速度提升数百倍。该引擎采用不同于原生 Postgres 的执行模型，主要面向分析型工作负载，并以形式化验证和差分模糊测试作为正确性保障。文章认为，这种设计能够在兼容 Postgres 语义的同时大幅改善分析性能，对现有依赖 Postgres 分析能力的用户具有潜在价值。当前这些结论主要来自引擎作者的技术说明，尚需更多独立验证与生产环境检验。

hackernews · poly2it · 8月7日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49208535)

**「背景」** pgrust 是一个用 Rust 重写 PostgreSQL 的实验性项目，旨在通过现代语言特性和底层优化来提升数据库性能。传统 PostgreSQL 查询引擎以行为单位逐行处理数据，而现代分析型引擎（如 ClickHouse）采用批量处理（batching）和向量化执行（如 SIMD）以大幅提升吞吐量。pgrust v0.2 在查询引擎中引入了批处理、算子融合和 SIMD 指令，并结合形式化验证与差分模糊测试来保证与 PostgreSQL 的逻辑一致性。

**「社区讨论」** 作者在讨论中表示，正确性是当前最高优先级，团队已通过形式化验证和差分模糊测试证明超过 1000 个面向用户的函数与 PostgreSQL 的逻辑一致。社区反应总体积极，但也存在明显分歧：部分用户期待自适应规划等能力得到验证并落地，另一部分则担心它不是官方 Postgres 团队维护的，信任和长期延续性会成为采用的主要障碍；也有人询问 IO 调度和线程调度如何处理“noisy neighbor”问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching, operator fusion, and SIMD - malisper.me</a></li>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now faster than Postgres and Clickhouse · GitHub</a></li>

</ul>
</details>

**标签**: `#postgres`, `#query-engine`, `#SIMD`, `#analytics`, `#rust`

---

<a id="item-tech-news-3"></a>
### [Kitesurf：在 V8 隔离中运行的代理优先浏览器](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare 宣布推出 Kitesurf，这是一款面向 AI 代理和浏览器自动化的“代理优先”浏览器，运行在 V8 隔离环境中，并构建于开源 Blitz 引擎之上。Kitesurf 将浏览器自动化带到 Cloudflare 边缘网络，为网页代理、内容抓取、测试等任务提供更接近数据源或用户的执行位置。该项目基于模块化浏览器引擎 Blitz，而 Blitz 作者表示 Cloudflare 计划开源并向上游合并其补丁。目前关于正式发布日期、可用地区和具体限制尚未公布。

hackernews · m3h · 8月7日 10:42 · [社区讨论](https://news.ycombinator.com/item?id=49208393)

**「背景」** Kitesurf 是 Cloudflare 在 Workers 平台上构建的“代理优先”浏览器，核心特点是利用 V8 隔离（V8 isolates）来运行浏览器的各个组件，从而提供无状态、可扩展且成本较低的无头浏览器能力。它基于开源模块化浏览器引擎 Blitz 构建，Blitz 由 Dioxus Labs 的团队开发，内部使用 Parley 进行文本整形和排版，并通过 blitz-paint 将网页栅格化为图像缓冲区。Kitesurf 将浏览器拆分为多个独立的 Workers 组件，只有一个面向外部的 Engine 组件通过 Chrome DevTools Protocol（CDP）和 HTTP REST 暴露接口，并存储每个会话的状态，这使其适用于浏览器自动化、网页抓取、测试和 AI 代理等场景。

**「影响」** 对希望在 Cloudflare 边缘运行 AI 代理或浏览器自动化任务的开发者而言，Kitesurf 提供了一个基于 V8 隔离的新执行选项；不过，它是否会与 Cloudflare 自己的 CDN 反机器人机制冲突，仍是社区关注且尚未明确的关键问题。

**「社区讨论」** 社区中，Blitz 作者确认 Kitesurf 基于 Blitz 构建，并表示 Cloudflare 打算开源并向上游合并修改；但多位长期用户对 Cloudflare 同时经营 CDN/反机器人安全业务与代理浏览器业务表示疑虑，质疑这些浏览器实例是否会被自己的反机器人系统拦截，也有人对“代理帮用户购物”等实际用例持保留态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf/">Introducing Kitesurf: The agent-first browser that runs in V8 isolates on Cloudflare Workers | Cloudflare Blog</a></li>
<li><a href="https://www.reddit.com/r/rust/comments/1vhetlq/introducing_kitesurf_cloudflares_new_headless_web/">r/rust on Reddit: Introducing Kitesurf: Cloudflare&#x27;s new headless web browser that runs in V8 Isolates, powered by Dioxus Blitz</a></li>
<li><a href="https://www.marktechpost.com/2026/08/06/cloudflare-introduces-kitesurf-an-agent-first-web-browser-that-runs-entirely-in-v8-isolates-on-cloudflare-workers/">Cloudflare Introduces Kitesurf: An Agent-First Web Browser That Runs Entirely in V8 Isolates on Cloudflare Workers - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#browser automation`, `#AI agents`, `#Cloudflare`, `#V8 isolates`, `#edge computing`

---

<a id="item-tech-news-4"></a>
### [2027 年内存产能据报已售罄，AI 与 HBM 需求成主因](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

据报道，2027 年的内存产能已被预订一空，主要驱动因素是 AI 对高带宽内存（HBM）的强劲需求。由于 HBM die 的封装方式使其体积大于普通 DRAM，同一技术节点下生产等量比特的 HBM3E 约占用三倍于 DDR5 的晶圆供应，因此 HBM 产能爬坡会限制非 HBM 产品（如 DDR5）的供应增长。这一供需紧张预计将持续影响内存价格和 AI 基础设施成本，并可能波及普通 PC 内存市场。

hackernews · inigyou · 8月7日 07:58 · [社区讨论](https://news.ycombinator.com/item?id=49207236)

**「背景」** 根据报道，三星、SK 海力士和美光 2027 年的 DRAM 与 HBM 产能已全部被预订，AI 数据中心是主要买家，既采购 HBM 用于加速器，也采购传统 DRAM 用于主机服务器。HBM 产能扩张会挤压非 HBM 产品供应，例如 HBM3E 在同一技术节点下生产给定比特数所消耗的晶圆供应量约为 DDR5 的三倍。美光预计 HBM 4E 将于 2027 年投产，这是为未来 AI 加速器设计的第四代高带宽内存增强版。

**「影响」** 对普通消费者和 PC 用户而言，DDR4/DDR5 内存价格可能继续上涨，新装机和升级成本增加；对依赖内存的 AI 和服务器厂商，则面临持续的供应与成本压力。

**「社区讨论」** 评论中既有对涨价的切身感受（如 DDR4 购买价偏高、订单被取消），也有技术背景说明 HBM 比 DDR5 更耗晶圆；还有人因此倾向减少使用 AI，并对个人硬件库存感到焦虑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tweaktown.com/news/113004/memory-capacity-for-all-of-2027-has-reportedly-been-booked-and-sold-with-no-more-dram-or-hbm-available/index.html">Memory capacity for all of 2027 has reportedly been booked and sold ...</a></li>
<li><a href="https://www.remio.ai/post/samsung-sk-hynix-and-micron-reportedly-sell-out-2027-memory-supply">Samsung, SK Hynix, and Micron Reportedly Sell Out 2027 Memory ...</a></li>
<li><a href="https://spilled.gg/memory-makers-production-capacity/">Memory makers have reportedly sold out their entire 2027 production...</a></li>

</ul>
</details>

**标签**: `#memory`, `#HBM`, `#AI infrastructure`, `#hardware`, `#supply chain`

---

<a id="item-tech-news-5"></a>
### [150 万页站点的爬虫对抗一年](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

一位运营约 150 万页网站的站长撰文回顾了与爬虫持续对抗一年的经历，文中称该站约 99%的流量来自机器人。这一现象凸显了 AI/LLM 爬虫和垃圾爬虫对网站带宽、成本及站长精力的显著冲击，也反映出反爬措施在误伤真实用户、搜索引擎抓取与维护成本之间的复杂权衡。作者的文章引发了关于集中式防护服务（如 Cloudflare）对开放网络影响的广泛讨论。

hackernews · petercooper · 8月7日 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49211386)

**「背景」** 网络爬虫或机器人会以自动化方式大量抓取网页，挤占带宽和计算资源；近年 AI/LLM 爬虫更让这类流量显著增加。许多站点依赖 Cloudflare 这类边缘平台来抵御或过滤机器人流量，因此在边缘平台上即使超过 99% 的请求来自机器人，运营者可能只感到“麻烦”而非生存危机；但若改用按 CPU 和带宽计费的传统 VPS，成本会迅速失控。文章作者指出，爬虫方的抓取成本下降速度远快于防御手段的改进，这正是机器人问题持续恶化的原因之一。

**「影响」** 面对 AI 爬虫带来的带宽与费用压力，Cloudflare 已于 2025 年 7 月 1 日推出“按爬取付费”（pay per crawl）市场机制，允许内容所有者向 AI 抓取方收费，并对无效请求返回 HTTP 402 Payment Required。这一措施直接回应了类似该网站这样遭遇海量爬虫请求的运营者，为他们提供了将机器人流量转化为收入的可能；但同时也强化了 Cloudflare 在网络访问中的守门人角色，使更多网站依赖其基础设施与政策来决定谁可以抓取内容。

**「社区讨论」** 社区对机器人流量问题的严峻性基本认同，并以实际数据佐证（例如有站长称 Claude-searchbot 在 72 小时内抓取了约 20.5 万页面，却只带来 1 次推荐访问）。不过在应对方式上存在分歧：一部分人担忧把访问控制权集中在 Cloudflare 等公司手中会损害开放网络；另一些实践者则推荐使用 Anubis 这类工作量证明方案，或建议改为静态托管以降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/">99% of My Website Traffic Is Bots | PatronView</a></li>
<li><a href="https://blog.cloudflare.com/introducing-pay-per-crawl/">Introducing pay per crawl: Enabling content owners to charge AI crawlers for access | Cloudflare Blog</a></li>
<li><a href="https://www.remio.ai/post/cloudflare-reveals-the-true-cost-of-ai-scrapers-on-the-open-web">Cloudflare Reveals the True Cost of AI Scrapers on the Open Web</a></li>
<li><a href="https://techcrunch.com/2025/07/01/cloudflare-launches-a-marketplace-that-lets-websites-charge-ai-bots-for-scraping/">Cloudflare launches a marketplace that lets websites charge AI bots for scraping | TechCrunch</a></li>

</ul>
</details>

**标签**: `#scraping`, `#bots`, `#web operations`, `#Cloudflare`, `#AI crawlers`

---

<a id="item-tech-news-6"></a>
### [SpaceX 2027 年 10GW 目标：3000 亿美元 ARR 与微软最大买家前景](https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real) ⭐️ 8.0/10

SemiAnalysis 的 Jeremie Eliahou Ontiveros 发文称，SpaceX 的星链（Starlink）可能在 2027 年达到 10GW 容量，以每 GW 每年 1000 亿美元的 AI 推理收入计算，这将推动 SpaceX 年经常性收入（ARR）达到 3000 亿美元。文章认为微软将成为这一太空推理容量的最大承购方，并指出微软 2026 年将迎来“10GW 觉醒”，Azure 可能出现三位数增长。该分析基于 SpaceX 的部署速度和 AI 推理需求增长，但属于前瞻性推测，依赖多项假设条件。

rss · Semianalysis · 8月7日 20:08

**「背景」** Starlink 是 SpaceX 的卫星互联网服务，目前正计划大幅扩张容量，有报道称其目标是在 2027 年前将容量扩大 100 倍，并可能接收大量 NVIDIA GPU 用于 AI 推理和训练。SpaceX 还与微软合作，通过 Azure 提供 Starlink 连接，这为它可能成为微软 AI 推理算力供应商的猜测提供了背景。

**「影响」** 若 SpaceX 在 2027 年实现 10GW 容量和 3000 亿美元年收入，微软可能成为太空 AI 推理服务的最大客户。不过，Runware 等公司提供的模块化地面推理舱以约 10 倍低价部署，可能对这类需求构成竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://convergedigest.com/spacex-starlink-v3-ai-infrastructure-expansion/">SpaceX Maps 100-Fold Starlink Capacity Expansion and Rapid AI Infrastructure Buildout - Converge Digest</a></li>
<li><a href="https://www.juniorstocks.com/spacex-announces-strong-partnership-microsoft">Juniorstocks | SpaceX announces strong partnership with Microsoft</a></li>
<li><a href="https://runware.ai/sonic-inference-pod">Sonic Inference Pods: Dramatically Cheaper AI Inference | Runware</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Starlink`, `#AI inference`, `#Microsoft Azure`, `#satellite internet`

---

<a id="item-tech-news-7"></a>
### [OpenAI 警告 Astra 或达关键网络攻击能力，发布可能推迟](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 8.0/10

OpenAI 于 2026 年 8 月 7 日披露，其即将推出的模型 Astra 在内部评估中展现出代理编码与网络安全方面的重大进展，初步结果强到无法排除达到“关键”网络能力阈值的可能性；此前 GPT-5.6-Sol 等模型在同一评估中仅被评为“高”。根据 OpenAI 的预备框架，达到关键阈值意味着模型可在无需人工干预的情况下自主发现并利用加固真实系统的零日漏洞，或仅凭高层目标策划和执行端到端的新型网络攻击。公司已暂停不符合强化安全要求的 Astra 相关内部活动，实施隔离测试环境、加密增强、通用监控等措施，并将与政府机构和 AI 安全组织合作开展第三方测试。这些扩大后的安全测试可能推迟 Astra 的发布，目前相关审查仍在进行，结果尚不确定。

telegram · zaihuapd · 8月7日 16:44

**「背景」** OpenAI 的预备框架（Preparedness Framework）是其评估和管控前沿模型风险的分级体系，通常将模型能力评为低、中、高或关键等级。达到“关键”等级意味着模型具备极高自主性的网络攻击能力，超出常规部署的安全保障范围，因此会触发更严格的安全测试和部署限制。此前 GPT-5.6-Sol 等模型仅被评为“高”，而 Astra 的初评结果第一次让 OpenAI 需要认真对待关键门槛的可能性。

**「影响」** 若 Astra 最终被确认达到关键阈值，与政府和第三方安全机构的联合测试及强化部署限制可能显著推迟其公开发布，并因此影响依赖 OpenAI 模型 API 的开发者和企业。

**标签**: `#AI safety`, `#OpenAI`, `#cybersecurity`, `#large language models`, `#preparedness framework`

---

<a id="item-tech-news-8"></a>
### [Oracle 禁止 OpenJDK 贡献使用 AI 生成代码](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 7.0/10

OpenJDK 发布了一项《生成式 AI 临时政策》，禁止向 OpenJDK 提交由 AI 生成的代码，并称最终版本正由律师起草。该政策主要出于版权溯源和代码质量担忧，因为 AI 生成内容可能带来知识产权风险，也会占用本来就有限的人工评审时间。此举对主要开源项目具有治理示范意义，也与 Oracle 自身积极拥抱 AI 的立场形成反差；有评论者指出，OpenJDK 的发布说明可能早已由模型撰写。

hackernews · delduca · 8月7日 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49213754)

**「背景」** OpenJDK 社区于 2026 年发布了一份关于生成式 AI 的临时政策，允许贡献者私下使用 AI 工具帮助理解、调试和审查代码，但明确禁止将 AI 生成的内容直接贡献给项目。这一政策由 Oracle 的法律团队主导制定，反映了公司对 AI 生成代码版权归属的谨慎态度。与此同时，Oracle 首席执行官 Larry Ellison 曾公开表示 Oracle 自身大量代码已由 AI 编写，这与 OpenJDK 的禁令形成鲜明对比，也凸显了大型科技企业在 AI 代码治理上的矛盾立场。

**「影响」** 该临时政策将直接影响所有 OpenJDK 贡献者：他们在最终政策出台前不得提交 AI 生成的代码，否则可能因版权或溯源问题被拒绝，并给项目的法律风险留下不确定性。

**「社区讨论」** 社区评论普遍认为这是为规避 AI 版权溯源问题而采取的谨慎措施，但也有人讽刺 Oracle 一边宣传 AI 一边禁止 AI 代码，并猜测发布说明早已由模型撰写。另有评论指出，最终成文政策由律师主导，可能不会比临时版本更宽松。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://www.tiktok.com/discover/oracle-ai-explained">Oracle Ai Explained | TikTok</a></li>

</ul>
</details>

**标签**: `#OpenJDK`, `#Oracle`, `#AI-generated code`, `#open-source policy`, `#software licensing`

---

<a id="item-tech-news-9"></a>
### [新墨西哥州法院判 Meta 付 5.67 亿美元儿童心理健康赔偿](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 7.0/10

美国新墨西哥州法院裁定 Meta 因损害儿童心理健康支付 5.67 亿美元（另有报道称为 9.42 亿美元），并须针对未成年用户做出产品与运营变更。该案依据新墨西哥州公共妨害法（NMSA 1978 § 30-8-1），认定 Meta 明知其平台对青少年心理健康构成危害仍维持相关功能。判决金额在多家媒体报道中存在差异：《卫报》与路透社报道为 5.67 亿美元，而《华尔街日报》报道为 9.42 亿美元。此案体现美国州级司法与监管对大型社交平台未成年人保护问题的持续追责，或会影响平台算法设计和内容审核策略。

hackernews · boplicity · 8月7日 00:06 · [社区讨论](https://news.ycombinator.com/item?id=49204352)

**「背景」** Meta 是 Facebook、Instagram 和 WhatsApp 的母公司。此前，美国多个州对社交媒体平台提起诉讼，认为其算法和产品设计对未成年人心理健康造成损害，并构成公共妨害。新墨西哥州法院此次裁定 Meta 支付 5.67 亿美元，用于弥补其平台对青少年心理健康造成的负面影响，并要求其为未成年用户作出相应改变。

**「影响」** 该裁决要求 Meta 向新墨西哥州支付 5.67 亿美元心理健康基金，并改变其平台在该州为年轻用户运作的方式，直接影响 Meta 在新墨西哥州的合规义务及产品政策。

**「社区讨论」** 评论者一方面认为罚款仅占 Meta 全球收入很小比例，是“象征性”处罚；另一方面指出对仅有约 200 万人口的新墨西哥州而言，9.42 亿美元按人口分摊十分可观，还有人援引该州公共妨害法 NMSA § 30-8-1，并担忧短视频算法对青少年的成瘾性影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pCN29EaUVSRXZkYkxJR1RjNjJDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Meta ordered to pay $ 567 million in New Mexico child safety case...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta">New Mexico court orders Meta to pay $ 567 m over... | The Guardian</a></li>
<li><a href="https://english.news.cn/20260807/a5e12666e9b444df8c546248735d0934/c.html">Meta ordered to pay 567 mln USD to address children &#x27;s mental health</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta">New Mexico court orders Meta to pay $567m over... | The Guardian</a></li>
<li><a href="https://www.aljazeera.com/news/2026/8/7/new-mexico-court-orders-meta-to-pay-567m-over-harm-to-youths">New Mexico court orders Meta to pay $567m over harm to... | Al Jazeera</a></li>
<li><a href="https://www.lbc.co.uk/article/meta-ordered-to-pay-567m-over-children-mental-harm-5Hjdfjz_2/">Meta ordered to pay $567m over harms to children ’s mental health as...</a></li>

</ul>
</details>

**标签**: `#legal`, `#regulation`, `#Meta`, `#social media`, `#technology policy`

---

<a id="item-tech-news-10"></a>
### [Codex 与 GPT-5.6 Sol 生成更佳浣熊抢匪游戏](https://simonwillison.net/2026/Aug/7/moonlight-mayhem/#atom-everything) ⭐️ 7.0/10

西蒙·威利森将完全相同的“Raccoon Heist”提示分别交给 Claude Fable 5 和运行 GPT-5.6 Sol Ultra 的 Codex Desktop，结果 Codex 生成了一款更好的游戏《Moonlight &amp; Mayhem》。这款游戏设定在博物馆中，玩家需要营救两只浣熊同伴并叠罗汉取出金色沙丁鱼，更贴合“抢匪”主题；Codex 还通过 gpt-image-2 生成了纹理与提示词。不过，一次性提示生成的版本存在一个 bug：每只浣熊的眼睛变成漂浮在头顶的巨大黑球，Codex 在开发过程中未能自行发现，威利森通过“为什么浣熊身上有巨大的黑色球体？”和“修复它”两条提示修复了该问题。整个 Codex 会话耗时 52 分钟，根据 AgentsView 的估算，如果按完整 API 价格而非订阅计费，成本约为 23.28 美元，涉及 700,700 个输入词元、3240 万个缓存词元和 148,000 个输出词元。这次对比为开发者提供了两大主流 AI 编程代理在实际游戏生成任务中的直观性能证据。

rss · Simon Willison · 8月7日 19:18

**「背景」** 西蒙·威利森几天前曾用 Claude Fable 5 根据一个四年前由 GPT-3 和 DALL-E 生成的游戏概念，一次性生成了一个完整的“Raccoon Heist”游戏。Codex 是 OpenAI 推出的编程代理，而 GPT-5.6 Sol Ultra 是其一个模式，会大量使用子代理来完成任务。该对比旨在测试同一提示在不同代理与模型下的生成质量与稳定性。

**「影响」** 对于关注 AI 辅助编程的开发者而言，这次对比表明 Codex 搭配 GPT-5.6 Sol Ultra 在一次性游戏生成任务中能产生比 Claude Fable 5 更令人满意的结果，但仍需人工审查和修复视觉缺陷；同时，使用每月订阅服务可能比按 API 总量付费更划算。

**标签**: `#AI coding agents`, `#Codex`, `#GPT-5.6`, `#game generation`, `#Simon Willison`

---

<a id="item-tech-news-11"></a>
### [Token 末日来临：企业忙着降低 AI 花费](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 7.0/10

404 Media 的一篇报道援引从 Accenture 泄露的会议音频指出，推动企业 AI token 消耗激增的主要并非工程师，而是大量非工程师用户；Accenture 的 agentic AI 战略负责人 Justice Kwak 证实，PDF 转成图片再转成 Markdown 是最大的 token 消耗来源之一。该现象反映出生成式 AI 在大型企业中落地后，成本正因低效率的工作流快速膨胀，促使企业开始重新审视 AI 使用方式。Simon Willison 在转载中评论道，如果 Accenture 能意识到 PDF 本身是糟糕的信息传递媒介，或许也能推动企业界改善这一习惯。

rss · Simon Willison · 8月7日 16:18

**「背景」** 大型语言模型通常按 token（文本处理的基本单位）计费，因此任何让输入或输出变长的操作都会直接推高成本，例如将 PDF 转换为 markdown 会产生大量额外 token。据报道，埃森哲内部数据显示其 token 支出“飙升”，且主要来自非工程师员工的使用行为；这标志着企业 AI 从无节制扩张逐渐转向严格控制成本。

**「影响」** 对正在优化生成式 AI 成本的企业而言，非工程师驱动的 token 消耗与 PDF 转 Markdown 这类高成本转换流程已成为明确的费用治理重点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/the-tokenpocalypse-is-here-companies-are-scrambling-to-stop-spending-so-much-on-ai/">The Tokenpocalypse Is Here : Companies Are Scrambling To Stop ...</a></li>

</ul>
</details>

**标签**: `#AI costs`, `#token consumption`, `#enterprise AI`, `#PDF processing`, `#AI economics`

---

<a id="item-tech-news-12"></a>
### [美国审查中国 AI 企业海外获取英伟达芯片渠道](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 7.0/10

美国商务部工业与安全局（BIS）正系统性审查中国人工智能企业如何在海外获取和使用英伟达芯片，重点包括通过租用他国算力进行远程访问的方式，并整理两份国家名单：涉嫌将受限芯片走私入境中国的黑市所在地，以及中国企业远程租用芯片的国家。此次审查是在月之暗面发布 Kimi K3 模型后启动的，一名白宫高官曾公开指控其非法获取英伟达芯片并经泰国远程访问，随后 BIS 执法团队展开调查。由于远程访问本身不违法，BIS 是否有权限制此类云计算协议仍存疑；美国众议院已通过两党法案拟明确授予该权力，但预计会遭到英伟达等科技公司反对。报道还指出，阿里巴巴通过开曼实体控制的新加坡壳公司，经正被美方调查的 Megaspeed 使用位于马来西亚的英伟达芯片。

telegram · zaihuapd · 8月7日 11:18

**「背景」** 美国对华先进半导体出口管制已把英伟达 H100、A100 等顶级芯片列入禁售范围，中国企业因此长期依赖海外云算力、二手市场和走私等灰色渠道获取算力。月之暗面约 7 月中旬发布的 Kimi K3 拥有 2.8 万亿参数和百万级上下文窗口，据称训练与推理使用了约 2 万片来自阿里的英伟达芯片，其性能与定价引发美方关注。BIS 此次审查正是针对这类“海外获取”路径是否绕过出口管制。

**「影响」** 若美国国会已通过的《远程访问安全法案》正式生效，BIS 将获得明确监管云计算远程访问的权限，从而可能切断中国 AI 企业通过海外云服务使用英伟达芯片的途径，直接影响阿里巴巴、Megaspeed 等公司；但由于 BIS 目前对远程访问的监管工具有限，且英伟达等科技公司预计反对，实际限制范围仍不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://carussignal.com/kimi-k3-2-8-trillion-parameters-compute-wall/">Kimi K 3 in Three Numbers: 2.8 Trillion Parameters, $15 Tokens, and...</a></li>
<li><a href="https://temperature2.com/p/2026-07-31-moonshot-kimi-alibaba-nvidia-chips/">Moonshot&#x27;s Kimi K 3 runs on 20,000 Alibaba Nvidia chips</a></li>
<li><a href="https://carnegieendowment.org/research/2026/05/the-geopolitical-debates-over-controlling-cloud-compute">The Geopolitical Debates Over Controlling Cloud Compute</a></li>
<li><a href="https://www.iaps.ai/research/remote-access-security-act">Remote Access Security Act (RASA) — Institute for AI Policy and...</a></li>

</ul>
</details>

**标签**: `#AI`, `#semiconductors`, `#export-controls`, `#Nvidia`, `#China`

---

<a id="item-tech-news-13"></a>
### [SK 海力士确认 V10 NAND 为 375 层堆叠并首次导入晶圆键合](https://www.gelonghui.com/live/2599953) ⭐️ 7.0/10

SK 海力士在 FMS 2026 峰会新闻稿中确认，继 321 层 V9“4D NAND”之后的新一代闪存 V10 采用 375 层堆叠设计，成为该公司首款采用晶圆键合技术的 NAND 产品。官方宣称 V10 实现了较上代产品 2.5 倍的每瓦性能，专为兼顾能效与性能的 AI 基础设施环境优化。该消息来自格隆汇转载的花频道 Telegram 内容，目前缺少更深入的技术细节或验证。此举表明 SK 海力士正通过层数提升和新型键合工艺，继续在高密度、高能效 NAND 领域推进。

telegram · zaihuapd · 8月7日 12:19

**「背景」** NAND 闪存通过垂直堆叠存储单元提升容量，层数越多单位面积密度越高。晶圆键合是一种将两片晶圆面对面结合的工艺，可替代传统穿透硅通孔等方式，有助于改善信号传输和散热，SK 海力士首次在 NAND 中采用该技术。V9 为 321 层 4D NAND，V10 为 375 层，性能功耗比提升 2.5 倍。

**「影响」** 对依赖高能效高密度存储的 AI 基础设施运营商而言，V10 NAND 有望提供更高效的大容量存储方案，同时推动晶圆键合技术在 NAND 制造中的进一步普及。

**标签**: `#NAND`, `#SK Hynix`, `#semiconductors`, `#AI infrastructure`, `#memory`

---

<a id="item-tech-news-14"></a>
### [sub2api 高危 OAuth 漏洞可仅凭邮箱接管账户](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 7.0/10

sub2api v0.1.171 及之前版本存在 CVSS 8.8 的高危 OAuth 账户接管漏洞。攻击者只需知道受害者的注册邮箱，无需密码、验证码或用户交互，即可通过接口将自身 OAuth 身份绑定到受害者账户，进而完全控制其 API 密钥、账单余额与订阅配额。漏洞根源是 pending session 流程中的 existingUser 分支未校验密码和验证码，攻击者将目标用户 ID 设为受害者后完成 OAuth 身份绑定。此后攻击者每次使用该 OAuth 身份登录，都会解析为受害者账户。

telegram · zaihuapd · 8月7日 14:59

**「背景信息」** sub2api 是一个开源 AI API 网关平台，用于把 AI 产品订阅的配额统一管理和分发，通常以 OAuth 方式让用户绑定订阅账户。OAuth 的 pending session（待处理会话）流程用于登录时建立会话，但受影响版本在 existingUser 分支缺少对密码和验证码的强校验，导致攻击者可借该流程将 OAuth 身份与受害者账户绑定。

**「影响」** 使用 sub2api v0.1.171 及更早版本的用户账户存在被完全接管的风险；由于攻击无需用户交互，已暴露邮箱的账户会面临 API 密钥、账单余额和订阅配额被完全控制的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github--com.proxy.hfzk.net.cn/Wei-Shaw/sub2api">GitHub - Wei-Shaw/ sub 2 api : Sub 2 API ...</a></li>

</ul>
</details>

**标签**: `#security`, `#oauth`, `#vulnerability`, `#open-source`, `#account-takeover`

---

<a id="item-tech-news-15"></a>
### [亚马逊严查内部 CPU 浪费](https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity) ⭐️ 7.0/10

Tom&\#x27;s Hardware 报道，亚马逊 AWS 今年 5 月起严查工程师对 EC2 实例的 CPU 浪费，以确保客户容量，内部申请实例的等待时间随之从数小时延长到数天。压力来自智能体 AI 工作负载的兴起：这类任务涉及大量运行在 CPU 上的工具调用和更复杂的 GPU 编排，使数据中心 GPU 与 CPU 配比从过去的 8:1 或 4:1 逐步逼近 1:1。AMD 和英伟达均已加大数据中心 CPU 布局，以争夺这一增长市场。

telegram · zaihuapd · 8月7日 16:31

**「背景」** 智能体 AI（agentic AI）指的是能够自主规划、调用工具并执行多步骤任务的人工智能工作流，其推理过程大量依赖 CPU 进行工具调用与 GPU 编排。传统 AI 推理通常以 GPU 为主，CPU 与 GPU 的配比曾为 8:1 或 4:1，而智能体 AI 的普及使这一比例逐渐逼近 1:1，大幅增加了数据中心对 CPU 的需求。AMD 的 EPYC 系列和英伟达等厂商的数据中心 CPU 产品正是为这类工作负载设计的。

**「影响」** 对 AWS 内部工程师最直接的影响是 EC2 实例申请等待时间从数小时拉长到数天，可能拖慢依赖算力的开发和测试进度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity">Amazon cracks down on &#x27; CPU waste&#x27; among engineers as agentic AI ...</a></li>
<li><a href="https://artvoice.com/2026/05/26/amd-stock-is-rising-because-of-something-nvidias-ceo-just-said/">AMD Stock Is Rising Because Of Something Nvidia &#x27;s CEO Just Said</a></li>
<li><a href="https://www.linkedin.com/posts/tamil-velan-jayakumar-b591b43_agentic-ai-brings-new-attention-to-cpus-in-activity-7455377503290019840-0XCR">Agentic AI boosts CPU demand in data centers | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AWS`, `#EC2`, `#Agentic AI`, `#CPU`, `#Cloud Computing`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美国海关已支付 1000 亿美元 IEEPA 关税退款](https://finance.yahoo.com/economy/policy/articles/cbp-paid-100-billion-ieepa-101617141.html) ⭐️ 9.0/10

美国海关与边境保护局（CBP）已根据《国际紧急经济权力法》（IEEPA）发放 1000 亿美元关税退款，这是已发生的财政与贸易事件。

openbb · PG · 8月7日 10:16

**「背景」** 此前，美国最高法院裁定政府依据《国际紧急经济权力法》（IEEPA）加征关税的行为无效，相关关税因此被退还。据美国海关与边境保护局（CBP）官员布兰登·洛德在提交给国际贸易法院的文件中所述，截至 7 月 31 日，已退还约 1000 亿美元的关税及利息。

**「影响」** 这 1000 亿美元退税已减少联邦收入，但目前美国消费者和部分企业正起诉美国公司，称这些公司收到了退税却未将相关款项返还给消费者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/cbp-paid-100-billion-ieepa-101617141.html">CBP has paid $ 100 billion in IEEPA tariff refunds</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/8/6/trump-administration-refunds-100bn-in-tariffs-struck-down-by-supreme-court">Trump administration refunds $ 100 bn in tariffs struck... | Al Jazeera</a></li>
<li><a href="https://fortune.com/2026/08/05/what-happened-trump-tariff-refunds-from-companies-consumers-class-action/">U.S. companies got $100 billion in tariff refunds , but... | Fortune</a></li>

</ul>
</details>

**标签**: `#tariffs`, `#IEEPA`, `#trade policy`, `#fiscal policy`, `#CBP`

---

<a id="item-finance-news-2"></a>
### [7 月就业数据疲软，美联储 9 月加息概率大降](https://www.cnbc.com/2026/08/07/odds-the-fed-hikes-in-september-tumble-following-big-july-jobs-miss.html) ⭐️ 8.0/10

7 月就业报告意外减少岗位，令市场对美联储 9 月加息的预期大跌。预测市场 Kalshi 显示，美联储下月维持利率不变的概率升至 65%，而报告公布前约为 50%。

rss · CNBC Finance · 8月7日 13:34

**「背景」** 美联储在 7 月会议上维持利率不变，但有三位联邦公开市场委员会委员反对这一决定，认为应加息以应对能源价格上涨。

**「影响」** 报告公布后，投资者重新定价利率路径，美债收益率走低、股市走高；利率期货仍显示 10 月有 55%和 12 月近 75%的加息概率。

**标签**: `#Federal Reserve`, `#interest rates`, `#jobs report`, `#monetary policy`, `#market expectations`

---

<a id="item-finance-news-3"></a>
### [纳斯达克 23 小时交易制获 SEC 批准，将于 2026 年 12 月 6 日上线](https://finance.sina.com.cn/stock/bxjj/2026-08-07/doc-inimnkup0012339.shtml) ⭐️ 8.0/10

美国证券交易委员会（SEC）已批准纳斯达克实行每周 5 天、每天 23 小时交易制度，计划于 2026 年 12 月 6 日上线；届时美股仅在美东时间 20:00 至 21:00 休市 1 小时用于系统清算。

telegram · zaihuapd · 8月7日 10:03

**「背景」** 此前 NYSE Arca 已获 SEC 加速批准将交易延长至每日 22 小时，Cboe 也提交了近 24×5 提案，均瞄准 2026 年 12 月。SEC 将于 9 月 17 日举办圆桌会议讨论隔夜交易的投资者保护等议题。

**「影响」** 在交易所正式延长时段前，散户已通过 Blue Ocean ATS 等另类交易系统进行隔夜交易，但隔夜交易流动性较薄、价差较大。

**标签**: `#nasdaq`, `#SEC`, `#trading-hours`, `#market-structure`, `#regulation`

---

<a id="item-finance-news-4"></a>
### [上汽通用宣布雪佛兰退出在华新车零售，750 万车主售后转别克渠道](https://m.mydrivers.com/newsview/1142126.html) ⭐️ 8.0/10

上汽通用宣布，雪佛兰正式终止在华新车零售业务并退出中国市场；品牌累计在华拥有 750 万车主，售后将由别克授权渠道承接。

telegram · zaihuapd · 8月7日 11:12

**「背景」** 过去 21 年，雪佛兰曾靠科鲁兹、迈锐宝等车型实现年销量最高突破 60 万辆；近年受国产新能源挤压，2025 年全年销量仅 5.2 万辆，多个月份终端销量跌至个位数。

**「影响」** 现有雪佛兰车主可转至别克授权渠道获得售后服务；国内工厂将继续生产并转为出口制造枢纽，上汽通用称车主权益不受影响。

**标签**: `#雪佛兰`, `#上汽通用`, `#中国汽车市场`, `#合资品牌`, `#通用汽车`

---

<a id="item-finance-news-5"></a>
### [北京下调非京籍购房社保年限至 1 年，提高公积金贷款额度](https://www.peopleapp.com/column/30052875352-500007640471) ⭐️ 8.0/10

北京市住建委等部门宣布进一步优化房地产政策：非京籍居民家庭购买五环内商品住房，社保或个税连续缴纳年限下调至 1 年及以上；夫妻双方均为缴存人时，首套住房公积金贷款最高额度提升至 240 万元，符合绿色建筑、多子女家庭等条件最高可再上浮 100 万元。

telegram · zaihuapd · 8月7日 13:57

**「背景」** 此前，北京对非京籍家庭购买五环内商品住房要求连续缴纳社保或个税满 2 年；本次由北京市住建委等部门联合印发的通知将其下调为满 1 年。限购指对购房资格设置社保或个税缴纳年限等门槛。

**「影响」** 这项调整将降低非京籍家庭在北京购房的资金和时间门槛，并提升公积金贷款支持力度，直接惠及有购房需求的非京籍居民家庭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.163.com/dy/article/L3OQOHEI0534A4SC.html">m.163.com/dy/article/L3OQOHEI0534A4SC.html</a></li>

</ul>
</details>

**标签**: `#Beijing real estate`, `#property policy`, `#housing provident fund`, `#China economy`, `#home purchase restriction`

---

<a id="item-finance-news-6"></a>
### [强生公司就滑石粉诉讼达成 55 亿美元和解](https://finance.yahoo.com/healthcare/articles/johnson-johnson-jnj-reaches-5-191035095.html) ⭐️ 8.0/10

强生公司同意支付 55 亿美元，以了结数千起指控其滑石粉产品导致癌症的诉讼。

openbb · BRK-B · 8月7日 19:10

**「背景」** 强生公司长期以来面临数千起滑石粉产品相关诉讼，原告指控其婴儿爽身粉等产品曾受石棉污染，可能导致卵巢癌和间皮瘤。此次拟议的 55 亿美元和解旨在解决约 7.6 万起相关案件，且公司已表示其中最多 30 亿美元将在明年支付，2028 年前不会再有额外付款。

**「影响」** 这项和解仍需足够多的原告参与才能生效；若大量原告拒绝，强生可能继续面对诉讼并承担额外法律费用，或需重新协商和解条件，从而影响公司及股东。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sokolovelaw.com/product-liability/talcum-powder/johnson-and-johnson/">Johnson &amp; Johnson Talcum Powder Lawsuit | Updated 2026</a></li>
<li><a href="https://www.bbc.com/news/articles/clyqnz52rp6o">Johnson &amp; Johnson offers to pay $5.5bn to settle baby powder lawsuits</a></li>
<li><a href="https://www.whalesbook.com/news/English/healthcarebiotech/Johnson-and-Johnson-Offers-dollar55-Billion-to-Resolve-Talc-Lawsuits/6a6964cb288da18bdd3ac212">Johnson &amp; Johnson Offers $5.5 Billion to Resolve Talc Lawsuits | Whalesbook</a></li>

</ul>
</details>

**标签**: `#Johnson &amp; Johnson`, `#talc settlement`, `#litigation`, `#consumer health`, `#corporate legal`

---

<a id="item-finance-news-7"></a>
### [财报和指引引发美股盘前个股大幅波动](https://www.cnbc.com/2026/08/07/stocks-making-the-biggest-moves-premarket-atlassian-corporation-wendys-vista-corp-first-solar-airbnb-more.html) ⭐️ 7.0/10

受财报和业绩指引影响，美股盘前个股大幅波动：Atlassian 第四财季营收和利润超 FactSet 预期，股价涨逾 29%；Twilio 将全年营收增长预期上调至 18%-18.5%，股价涨逾 17%；Trade Desk 二季度盈利和营收低于 LSEG 预期，股价跌 27%。另有 Doximity 因首席执行官称其 AI 搜索产品每次搜索收入超过运行成本 10 倍而一度涨逾一倍；太阳能股因美国对进口太阳能板制造材料加征关税上涨，First Solar 涨逾 5%。

rss · CNBC Finance · 8月7日 13:23

**「背景」** 盘前交易指美股常规开盘前的交易时段；财报季中，公司发布季度业绩和未来指引会直接影响其股价。

**标签**: `#earnings`, `#premarket`, `#guidance`, `#tech stocks`, `#stock movers`

---

<a id="item-finance-news-8"></a>
### [澳大利亚拟为外卖骑手设每小时 31.30 澳元最低收入保障](https://www.twu.com.au/press/food-delivery-workers-to-get-world-first-minimum-standards-on-pay-and-conditions-from-august/) ⭐️ 7.0/10

澳大利亚公平工作委员会公布一项拟议最低标准令，拟为优步外卖、DoorDash 等平台的外卖骑手设立每小时至少 31.30 澳元的最低收入保障；若最终通过，最早将于 2026 年 8 月 17 日生效，平台须在结算周期内补足收入差额。

telegram · zaihuapd · 8月7日 15:44

**「背景」** 该标准最初由澳大利亚运输工人工会（TWU）申请提出，后由工会与两大平台共同提交协商方案。工会称其为“全球首创”，但纽约、西雅图和加拿大不列颠哥伦比亚省已有类似的外卖平台最低支付制度；TWU 数据还显示，自 2017 年以来已有 25 名零工工人在道路上丧生。

**标签**: `#Australia`, `#gig economy`, `#minimum wage`, `#food delivery`, `#labor regulation`

---

<a id="item-finance-news-9"></a>
### [莫尔森库尔斯第二季度盈利超预期](https://finance.yahoo.com/markets/stocks/articles/molson-coors-q2-earnings-beat-164500953.html) ⭐️ 7.0/10

莫尔森库尔斯（Molson Coors）第二季度盈利超出分析师预期，主要得益于产品定价和成本节约。

openbb · PG · 8月7日 16:45

**「背景」** Molson Coors 第二季度盈利和销售额均同比下降，但仍高于分析师预期，主因是更高的定价、有利的产品组合和成本管控部分抵消了销量下滑的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zacks.com/stock/news/2971371/molson-coors-q2-earnings-beat-estimates-on-pricing-and-cost-savings">Molson Coors Q 2 Earnings Beat Estimates on Pricing and Cost ...</a></li>

</ul>
</details>

**标签**: `#earnings`, `#Molson Coors`, `#beverage`, `#pricing`, `#cost savings`

---

<a id="item-finance-news-10"></a>
### [帝亚吉欧初步财报显示北美市场疲软，烈酒行业或承压](https://finance.yahoo.com/markets/stocks/articles/deo-fy26-preliminary-earnings-show-154700605.html) ⭐️ 7.0/10

一项分析显示，全球烈酒巨头帝亚吉欧（Diageo）2026 财年初步业绩表明北美市场出现疲软，这可能为整个烈酒行业带来压力。

openbb · PG · 8月7日 15:47

**「背景」** 帝亚吉欧（Diageo）公布截至 2026 年 6 月 30 日的 2026 财年初步业绩，显示欧洲、拉美和非洲增长被北美和亚太的疲软抵消，导致全年净销售额同比下滑。公司预计北美市场在 2026 财年将下滑 3%，同时努力改善其在该地区的市场份额表现。

**「影响」** 对于投资者，帝亚吉欧 2026 财年初步业绩显示，北美和亚太地区疲软被欧洲、拉美和非洲的增长所抵消，同时管理层预计 2026 财年有机销售额增长将与 2025 财年相近，有机营业利润增长为个位数中段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/deo-fy26-preliminary-earnings-show-154700605.html">DEO FY 26 Preliminary Earnings Show Pressure on North America ...</a></li>
<li><a href="https://www.diageo.com/en/investors/results-reports-and-events/2026-preliminary-results">Fiscal 26 Preliminary Results | Diageo</a></li>
<li><a href="https://www.zacks.com/stock/news/2971291/deo-fy26-preliminary-earnings-show-pressure-on-north-america-weakness">DEO FY 26 Preliminary Earnings Show Pressure on North America ...</a></li>
<li><a href="https://www.diageo.com/en/investors/results-reports-and-events/2026-preliminary-results">Fiscal 26 Preliminary Results | Diageo</a></li>
<li><a href="https://markets.ft.com/data/announce/full?dockey=1323-17167819-5GGLDB98493503CA6H8LP0I25H">Diageo Preliminary Results 2025 – Company Announcement - FT.com</a></li>

</ul>
</details>

**标签**: `#Diageo`, `#Earnings`, `#North America`, `#Spirits`, `#FY26`

---

<a id="item-finance-news-11"></a>
### [Constellation Energy 签署 920 兆瓦新购电协议，含沃尔玛合同](https://finance.yahoo.com/energy/articles/constellation-signed-920-megawatts-power-164558421.html) ⭐️ 7.0/10

据文章报道，Constellation Energy 签署了总计 920 兆瓦的新购电协议，其中一项是与沃尔玛达成的。这显示出该公司在清洁能源领域的商业进展，但未披露具体财务条款。

openbb · PG · 8月7日 16:45

**「背景」** 星座能源在 2026 年第二季度签署了 920 兆瓦的长期核电购电协议，客户包括沃尔玛等投资级企业，协议期限为 15 至 20 年，预计在 2029 年至 2032 年间开始供电。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/07/constellation-signed-920-megawatts-of-new-power-deals-including-a-walmart-ppa-heres-what-it-means-for-ceg-stock/">Constellation Signed 920 Megawatts of New Power ... | The Motley Fool</a></li>
<li><a href="https://energynews.pro/en/constellation-energy-raises-2026-guidance-to-1150-1250-per-share">Constellation Energy Raises 2026 Guidance to... | energynews.pro</a></li>

</ul>
</details>

**标签**: `#Constellation Energy`, `#Power Purchase Agreement`, `#Walmart`, `#Clean Energy`, `#Utility Sector`

---