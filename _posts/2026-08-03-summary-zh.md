---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 98 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Qwen 3.8-Max 官宣：2.4 万亿参数，首次开源 Max 权重](#item-tech-news-1) ⭐️ 9.0/10
2. [开放权重模型监管之争：AI 行业公开信](#item-tech-news-2) ⭐️ 8.0/10
3. [Kakehashi：在 Linux ARM 上运行 macOS 二进制的实验项目](#item-tech-news-3) ⭐️ 7.0/10
4. [苹果限制漏洞提交应对 AI 低质报告](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [美联储连续第二次维持利率不变，三位官员持异议](#item-finance-news-1) ⭐️ 9.0/10
2. [高盛交易业务有望创下创纪录年度收入](#item-finance-news-2) ⭐️ 8.0/10
3. [公积金条例拟修订：灵活就业者可缴存，装修物业费可提取](#item-finance-news-3) ⭐️ 8.0/10
4. [日美据报联合干预汇市以阻止日元跌至近 40 年低点](#item-finance-news-4) ⭐️ 8.0/10
5. [本周财报看点：SpaceX、迪士尼、AMD、麦当劳](#item-finance-news-5) ⭐️ 7.0/10
6. [道指期货上涨、油价大跌：特朗普调整对伊政策，AMD 等财报在即](#item-finance-news-6) ⭐️ 7.0/10
7. [贝索斯支持的 AI 芯片材料初创公司估值 26 亿美元，携手英伟达和 Meta](#item-finance-news-7) ⭐️ 7.0/10
8. [分析：高通 Q3 业绩与指引或重塑其 AI 投资叙事](#item-finance-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen 3.8-Max 官宣：2.4 万亿参数，首次开源 Max 权重](https://qwen.ai/blog?id=qwen3.8) ⭐️ 9.0/10

据 Qwen 团队今日发布的消息，Qwen 3.8-Max 正式亮相，总参数规模达 2.4 万亿，活跃参数为 95B，并计划于下周开源模型权重，这将是 Qwen 首次开放 Max 级别模型权重。该模型基于 Qwen 3.5 架构，在编码、工作、研究和长周期任务上均有提升；据称在编码测试中可自主运行超过 10 天完成项目构建与自我进化，并在 WWW2025 多模态对话意图识别竞赛中以 458/526 的战绩击败对手。目前该模型已通过 QwenCloud 提供 API 服务，但上述具体性能数据来自 Telegram 渠道，尚需官方正式发布材料进一步核实。

telegram · zaihuapd · 8月3日 02:31

**「背景」** Qwen 是阿里巴巴通义千问团队推出的大语言模型系列。此前 Qwen 的 Max 级旗舰模型（如 Qwen 3.7-Max）均以闭源形式发布，权重不对外开放；而 Qwen 3.8-Max 于 2026 年 7 月 19 日以预览版亮相，采用 2.4 万亿参数的稀疏 MoE 架构，并承诺将开放权重。该模型还支持文本、图像、视频和文档等多模态输入，并拥有 100 万 token 的上下文窗口。

**「影响」** 如果下周如期开源，Qwen 3.8-Max 将成为开发者可直接获取权重的最强开源模型之一，显著降低顶级模型的自部署和研究门槛，并可能加剧开源与闭源模型在编码、智能体等场景的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/qwen38-max-review">Qwen 3 . 8 Max review: Alibaba&#x27;s 2 . 4 T flagship, tested (2026) | eesel AI</a></li>
<li><a href="https://saascity.io/blog/kimi-k3-vs-qwen38-max-china-trillion-parameter-open-models-2026">Kimi K3 vs Qwen 3 . 8 - Max : China Shipped Two Trillion - Parameter ...</a></li>
<li><a href="https://shaam.blog/articles/qwen-3-8-max-honest-review-2026">Qwen 3 . 8 Max : An Honest Review of Alibaba&#x27;s 2 . 4 T Parameter AI...</a></li>

</ul>
</details>

**标签**: `#qwen`, `#large language models`, `#open-source`, `#Mixture-of-Experts`, `#AI research`

---

<a id="item-tech-news-2"></a>
### [开放权重模型监管之争：AI 行业公开信](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

西蒙·威利森总结了近期围绕 AI 开发的多封公开信。7 月 24 日，微软主导发布题为《开放权重与美国 AI 领导力》的公开信，获英伟达、亚马逊、Y Combinator、Linux 基金会以及后来加入的 OpenAI 等 235 家 AI 相关公司联署，明确反对美国政府因“安全”担忧而禁止或限制开放权重模型的倾向，并公开支持蒸馏这一模型开发技术。Anthropic 缺席联署，并在三天后发表自身立场，CEO 达里奥·阿莫迪强调开放权重模型可能被专制政府或攻击者滥用，呼吁打击工业规模的蒸馏操作，但表示从未主张全面禁止开放权重模型。7 月 28 日，另一封由前沿 AI 公司 1324 名员工签署的公开信《Pacing the Frontier》发布，呼吁美国政府支持国际合作，为自动化 AI 研发节奏建立技术与治理工具。这些信件反映出行业内对开放权重监管和 AI 发展速度存在明显分歧。

rss · Simon Willison · 8月2日 04:16

**「背景」** 开放权重模型指公开模型权重，使研究者和开发者可以检查、修改和部署模型，但也可能被用于恶意目的；蒸馏则指用一个模型的输出来训练或改进另一个模型，是常见的模型开发技术。美国政府内部存在因安全风险限制开放权重模型的讨论，促使产业界通过公开信表达立场。

**「影响」** 这场公开信运动可能影响美国对开放权重模型的监管走向，同时凸显行业阵营分裂：微软、英伟达、OpenAI 等企业主张开放权重与合法蒸馏，而 Anthropic 则将安全风险放在更突出位置并呼吁打击蒸馏滥用。

**标签**: `#AI policy`, `#open source`, `#open-weight models`, `#industry letters`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [Kakehashi：在 Linux ARM 上运行 macOS 二进制的实验项目](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi 是一个实验性用户态项目，目标是在 Linux ARM 机器上原生运行 macOS 命令行二进制文件。目前已有可工作的原型，包括 7-Zip、curl 和 Xcode Tools Git。其中 7-Zip 在包含 8k 文件树的多线程压缩测试中通过，但当前比 Linux 原生执行慢约 5.2 倍，作者已制定优化计划以缩小差距；curl 有超过 200 条命令和选项通过自动化 Docker 测试脚本；Xcode Tools Git 的基础版本控制功能可用。该项目仍处于早期阶段，整体性能尚未达到原生水平，但展示了在不依赖完整 macOS 的情况下运行 macOS CLI 工具的可行性。

hackernews · vlad\_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**「背景」** macOS 二进制文件依赖 Apple 的系统调用接口和库（如 Foundation、CoreFoundation 等），要在 Linux 上运行通常需要兼容层或系统调用翻译。Kakehashi 采用用户态实现，类似于 WINE 对 Windows 应用或 Darling 对 macOS 应用的做法，但目前仅支持 ARM 架构的 Linux 主机。

**「影响」** 如果该项目继续发展，ARM Linux 用户未来或许能直接运行部分 macOS 命令行工具，而无需完整的 macOS 环境或虚拟化；不过目前仅有少量工具可用，且性能明显低于原生执行，实际使用价值仍有限。

**「社区讨论」** Hacker News 评论中，用户 13rac1 提到 Darling 项目及其 ARM64 支持 PR，建议考虑合作；作者回应了当前原型和性能数据。其他用户一方面表示长期关注，另一方面也指出项目仍处于早期阶段，并有一位评论者批评项目命名不佳。

**标签**: `#macOS compatibility`, `#Linux ARM`, `#userspace`, `#binary translation`, `#experimental`

---

<a id="item-tech-news-4"></a>
### [苹果限制漏洞提交应对 AI 低质报告](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

苹果承认已在今年 6 月限制研究人员可同时提交的漏洞报告数量，并设置 30 天冷却期，以应对借助 AI 模型生成的大量低质量安全报告。意大利安全初创公司 Bynario 表示，他们用 ChatGPT 在三周内于最新 macOS 中发现 50 多个漏洞，其中包括可让攻击者完全控制电脑的提权漏洞链，但因提交限额无法向苹果报告。苹果称已与 Bynario 取得联系并审核其提交，同时也在用 AI 加强自身防御；本周发布的系统安全更新修复数量约为以往的五倍，并致谢 Anthropic 和 OpenAI 的工具协助发现漏洞。

telegram · zaihuapd · 8月2日 05:50

**「背景」** 安全研究人员通常通过向厂商提交漏洞报告来换取奖励或修复承诺；苹果设有安全奖励计划，并依赖外部研究者的漏洞发现。随着生成式 AI 工具普及，大量借助 AI 生成的报告可能质量低下或重复，挤占人工审核资源，因此苹果开始限制提交数量；但 AI 也被用于真实漏洞挖掘，例如 Bynario 用 ChatGPT 发现大量 macOS 漏洞。

**「影响」** 对依赖漏洞奖励计划的安全研究员，提交限额可能延迟高价值漏洞（如 Bynario 发现的提权链）的上报，但苹果已主动联系并审核其提交，实际修复尚不确定。

**标签**: `#Apple`, `#AI security`, `#vulnerability reporting`, `#macOS`, `#ChatGPT`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储连续第二次维持利率不变，三位官员持异议](https://finance.yahoo.com/economy/policy/articles/fed-held-interest-rates-steady-015000677.html) ⭐️ 9.0/10

美联储在凯文·沃什领导下连续第二次会议维持利率不变，三位官员对此决定持异议，为投资者提供未来货币政策走向的信号。

openbb · NVDA · 8月3日 01:50

**「背景」** 美联储在 7 月 29 日结束的会议上将联邦基金利率维持在 3.5%至 3.75%不变，这是新任主席凯文·沃什（Kevin Warsh）领导下连续第二次按兵不动。克利夫兰联储行长 Beth Hammack、明尼阿波利斯联储行长 Neel Kashkari 和达拉斯联储行长 Lorie Logan 投了反对票，主张加息 25 个基点；沃什在记者会上重申美联储致力于实现 2%通胀目标。

**「影响」** 市场投资者目前普遍预期美联储可能在 9 月会议上加息 25 个基点，这将进一步推高企业和家庭的借贷成本，并影响债券市场表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/29/fed-meeting-today-live-updates.html">Fed meeting recap: Warsh says Fed won&#x27;t hesitate to stop inflation, but bond market has doubts</a></li>
<li><a href="https://www.cnn.com/2026/07/29/business/live-news/federal-reserve-interest-rate-07-29-26">Fed holds interest rates steady after cliffhanger meeting, but three officials dissent | CNN Business</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/kevin-warsh-fed-treasury-yields-inflation-credibility-interest-rates.html">Analysis: Fed Chairman Warsh&#x27;s credibility in question after leaving interest rates unchanged</a></li>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Kevin Warsh`, `#Dissents`

---

<a id="item-finance-news-2"></a>
### [高盛交易业务有望创下创纪录年度收入](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛交易员有望创下创纪录的年度交易收入；实际公布的第二季度股票交易收入同比增长 72%至 74.2 亿美元，创季度新高，投行收入增长 55%至 34 亿美元，主要受 SpaceX IPO 和 Alphabet 850 亿美元增发等交易推动。

rss · CNBC Finance · 8月2日 13:52

**「背景」** 股票交易属于高盛全球银行与市场部门，该部门上季度贡献 155 亿美元收入，占全行总收入逾 75%；高盛近年推动投行、财富管理客户交叉使用股票交易服务，以扩大客户基础。

**标签**: `#Goldman Sachs`, `#equities trading`, `#earnings`, `#investment banking`, `#market volatility`

---

<a id="item-finance-news-3"></a>
### [公积金条例拟修订：灵活就业者可缴存，装修物业费可提取](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 8.0/10

住建部就《住房公积金管理条例（修订征求意见稿）》公开征求意见，拟允许个体工商户、外卖员、快递员、网约车司机等灵活就业人员自愿缴存公积金，并将自住房装修、物业费纳入可提取范围。该规定仍属征求意见稿，尚未生效。

telegram · zaihuapd · 8月2日 06:32

**「背景」** 现行公积金主要用于购房或租房，灵活就业人员通常无法正常缴存，异地使用也不够便利。

**「影响」** 若条例正式通过，可能让灵活就业人员获得公积金缴存渠道，并让缴存者能用公积金支付装修和物业费，相关群体将直接受益。

**标签**: `#housing`, `#policy`, `#China`, `#provident fund`, `#flexible employment`

---

<a id="item-finance-news-4"></a>
### [日美据报联合干预汇市以阻止日元跌至近 40 年低点](https://www.zaobao.com.sg/news/world/story20260802-9457369) ⭐️ 8.0/10

据联合早报报道，日本财务大臣片山皋月预计 8 月 3 日宣布日美已联合干预外汇市场，以阻止日元继续逼近近 40 年低点；市场消息称美国财政部计划买入 50 亿至 100 亿美元日元。日元兑美元此前一度接近 164，为 1986 年以来最低。

telegram · zaihuapd · 8月3日 01:29

**「背景」** 此前日元兑美元一度逼近 164，创 1986 年以来新低；据日本财务省 8 月 3 日证实，日美已于上周五（8 月 1 日）实施协调买入日元的联合干预，这是约 30 年来两国首次联手支撑日元。联合干预意在阻止日元过度贬值、防范套息交易平仓引发全球波动，但市场普遍认为其难以扭转日元长期弱势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.japantimes.co.jp/business/2026/08/03/markets/japan-us-joint-yen-intervention/">Japan confirms joint yen intervention with U.S., signaling readiness for more action - The Japan Times</a></li>
<li><a href="https://www.cnbc.com/2026/08/03/yen-intervention-us-japan-trump-bessent-katayama.html">U.S., Japan confirm coordinated yen intervention, signal readiness for more</a></li>
<li><a href="https://www.chosun.com/english/market-money-en/2026/08/02/TDIKXF57NZEEBPPGI72QI7ALSQ/">U.S. and Japan Intervene to Buy Yen for First Time in 30 Years</a></li>

</ul>
</details>

**标签**: `#forex`, `#yen`, `#Japan`, `#US`, `#intervention`

---

<a id="item-finance-news-5"></a>
### [本周财报看点：SpaceX、迪士尼、AMD、麦当劳](https://finance.yahoo.com/video/earnings-watch-week-spacexs-first-180000072.html) ⭐️ 7.0/10

据 Yahoo Finance 视频预告，本周值得关注的企业财报包括 SpaceX 首次发布的财报，以及迪士尼、AMD 和麦当劳的业绩。目前仅为预告，尚无实际业绩数据。

openbb · NVDA · 8月2日 18:00

**「背景」** SpaceX 定于 8 月 4 日发布上市以来首份财报，此次发布将触发首次重大锁定期到期；该公司 2025 年净亏损约 50 亿美元、营收 187 亿美元，2026 年第一季度亏损约 42.8 亿美元，其中 Starlink 收入近 12 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/21/spacex-spcx-earnings-lock-up-expiration.html">SpaceX snaps 7-day losing streak, sets earnings date that triggers first big share unlock</a></li>
<li><a href="https://www.morningstar.com/stocks/5-charts-what-watch-spacex-earnings">5 Charts on What to Watch in SpaceX Earnings | Morningstar</a></li>

</ul>
</details>

**标签**: `#earnings`, `#SpaceX`, `#Disney`, `#AMD`, `#McDonald&\#x27;s`

---

<a id="item-finance-news-6"></a>
### [道指期货上涨、油价大跌：特朗普调整对伊政策，AMD 等财报在即](https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-spacex-amd-sandisk-eli-lilly-earnings-loom/?src=A00220&amp;yptr=yahoo) ⭐️ 7.0/10

道指期货上涨，油价大跌，因特朗普在伊朗问题上转变立场；AMD、SanDisk、Eli Lilly 等财报即将发布。

openbb · NVDA · 8月3日 01:59

**「背景」** 此前报道称，特朗普威胁伊朗曾推动油价单日大涨 7%；如今他在伊朗问题上的立场转变令油价承压。本周美股将迎来 AMD、SanDisk、Eli Lilly 和 SpaceX 等公司的财报，市场关注 AI 芯片、Starlink 和资本开支等焦点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oilprice.com/">Crude Oil Prices Today | OilPrice .com</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262068819-weekly-preview-us-july-non-farm-payrolls-data-market-focus-pltr-sandisk-amd-spacex-earnings-reports-tradingkey">The Week Ahead: US July Non-Farm Payrolls in Focus; PLTR, SanDisk, AMD, and SpaceX Earnings Ahead</a></li>

</ul>
</details>

**标签**: `#Oil Prices`, `#Iran Policy`, `#Earnings`, `#Stock Market`, `#Dow Jones`

---

<a id="item-finance-news-7"></a>
### [贝索斯支持的 AI 芯片材料初创公司估值 26 亿美元，携手英伟达和 Meta](https://finance.yahoo.com/technology/ai/articles/jeff-bezos-backed-2-6-233300700.html) ⭐️ 7.0/10

据报道，一家由杰夫·贝索斯支持的 AI 初创公司目前估值 26 亿美元，正与英伟达和 Meta 合作研发新的芯片材料。

openbb · NVDA · 8月2日 23:33

**「背景」** CuspAI 是一家获杰夫·贝索斯旗下 Bezos Expeditions 投资的 AI 初创公司，最近完成 4.5 亿美元融资，估值达 26 亿美元；它与 Nvidia 和 Meta 合作，用 AI 寻找下一代芯片材料。

**「影响」** 据合作方介绍，CuspAI 将与英伟达、Meta 等合作，把计算基础设施与科学专业知识结合，开发旨在降低识别下一代半导体材料时间和成本的软件；这直接影响芯片制造商和 AI 硬件供应链的材料研发环节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/02/jeff-bezos-backed-a-26-billion-ai-startup-thats-pa/">Jeff Bezos Backed a $2.6 Billion AI Startup That&#x27;s Partnering With Nvidia and Meta on New Chip Materials | The Motley Fool</a></li>
<li><a href="https://www.benzinga.com/markets/private-markets/26/07/60549441/jeff-bezos-backs-2-6-billion-ai-startup-teaming-up-with-nvidia-and-meta-to-tackle-one-of-the-chip-industrys-biggest-challenges">Jeff Bezos Backs $2.6 Billion AI Startup Teaming Up With Nvidia and Meta to Tackle One of the Chip Indust - Benzinga</a></li>
<li><a href="https://www.flowerclaw.tech/en/articles/meta-nvidia-ai-materials-semiconductor-discovery-en">Meta and Nvidia Back AI Materials Startup: How AI Is ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/nvidia-meta-join-bezos-backed-124650337.html?fr=sycsrp_catchall">Nvidia, Meta Join Bezos-Backed AI Startup Speed Next ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#semiconductors`, `#startups`, `#Nvidia`, `#Meta`

---

<a id="item-finance-news-8"></a>
### [分析：高通 Q3 业绩与指引或重塑其 AI 投资叙事](https://news.google.com/rss/articles/CBMi0gFBVV95cUxQcUZwUjdtX2tIN3NUbmFrSnEwRDFKZC1EMmpkVmxHd0JjVmxxM0k5QjNsU1JmeXBBN1VJaFBNdGJJTTVVQzA2SVhwYklzTXRTWVBfRFNEZ0MxVWNLR214X1M3cXY1c1lwcnRSQWxEM295TUwzbGp4eV95ZDUxRTZ2NkFzOS0xcDd6dUFRMXROZ0dzTi1EbjhoZ2tOOExMakNOZEdZOVpMX0hVaUMtOXFFZFMzRGRUY0puUU1fYnNDdjlTY0d6QjMyNHFabXNXTUZfUWfSAdIBQVVfeXFMUHFGcFI3bV9rSDdzVG5ha0pxMEQxSmQtRDJqZFZsR3dCY1ZscTNJOUIzbFNSZnlwQTdVSWhQTXRiSU01VUMwNklYcGJJc010U1lQX0RTRGdDMVVjS0dteF9TN3F2NXNZcHJ0UkFsRDNveU1MM2xqeHlfeWQ1MUU2djZBczktMXA3enVBUTF0TmdHc04tRG44aGdrTjhMTGpDTmRHWTlaTF9IVWlDLTlxRWRTM0RkVGNKblFNX2JzQ3Y5U2NHekIzMjRxWm1zV01GX1Fn?oc=5) ⭐️ 7.0/10

simplywall.st 的分析认为，高通（Qualcomm）第三季度业绩与指引的组合可能正在改写其“AI 优先”的投资叙事。该分析未提供具体的营收或盈利数字。

google\_news · simplywall.st · 8月2日 10:23

**「背景」** 高通于 2025 年 6 月 29 日发布 2025 财年第三季度业绩，并强调其在 AI 处理、高性能低功耗计算和先进连接方面的领导地位，称随着 AI 在边缘侧扩展，公司有望成为行业平台的首选。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qualcomm.com/news/releases/2025/07/qualcomm-announces-third-quarter-fiscal-2025-results">Qualcomm Announces Third Quarter Fiscal 2025 Results</a></li>

</ul>
</details>

**标签**: `#Qualcomm`, `#Q3 earnings`, `#guidance`, `#AI`, `#semiconductors`

---