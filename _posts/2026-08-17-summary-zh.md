---
layout: default
title: "Horizon Summary: 2026-08-17 (ZH)"
date: 2026-08-17
lang: zh
---

> 从 150 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Claude 系统提示词现已公开](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B：本地表现优秀，但默认过度思考](#item-tech-news-2) ⭐️ 8.0/10
3. [SSOG-Attention：可分离高斯和实现亚二次注意力，可扩展替代 SDPA](#item-tech-news-3) ⭐️ 7.0/10

**财经新闻**
1. [美联储迎来多年来最难预测的会议](#item-finance-news-1) ⭐️ 9.0/10
2. [伊朗战争推动八大石油公司季度利润超 900 亿美元](#item-finance-news-2) ⭐️ 8.0/10
3. [Anthropic 第二季初步营收破 115 亿美元，同比增长逾 14 倍](#item-finance-news-3) ⭐️ 8.0/10
4. [英伟达 30 亿美元押注 AI 电力基础设施](#item-finance-news-4) ⭐️ 8.0/10
5. [格雷格·阿贝尔上季度投入近 350 亿美元](#item-finance-news-5) ⭐️ 8.0/10
6. [美联储 7 月会议决定维持利率不变](#item-finance-news-6) ⭐️ 8.0/10
7. [美联储主席凯文·沃什在众议院就通胀与货币政策作证](#item-finance-news-7) ⭐️ 8.0/10
8. [美国中东石油出口数据现分歧：官方称回升至 1500 万桶/日，追踪机构称仅约 1000 万桶/日](#item-finance-news-8) ⭐️ 7.0/10
9. [欧洲天然气库存降至 17 年最低](#item-finance-news-9) ⭐️ 7.0/10
10. [人工智能扩张或延长化石燃料主导地位](#item-finance-news-10) ⭐️ 7.0/10
11. [AMD 发行 47.5 亿美元债券，规模为上次三倍多](#item-finance-news-11) ⭐️ 7.0/10
12. [黄金触及每盎司 4,400 美元，矿企股开始跟进上涨](#item-finance-news-12) ⭐️ 7.0/10
13. [多家消费巨头 CEO 警告：美国消费者资金紧张](#item-finance-news-13) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude 系统提示词现已公开](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 公开了 Claude 模型的系统提示词，使研究者、提示工程师和开发者能够深入分析并比较不同版本之间的行为变化。这一透明度举措为理解模型在安全、同理心和任务执行上的取舍提供了直接依据。公开内容涵盖多个 Claude 模型版本，并释放出 Anthropic 对模型行为进行系统性塑造的信号。社区已经开始以版本化方式整理这些提示词，方便追踪具体差异。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**「背景」** Anthropic 会在官方发布说明中公开 Claude 系列模型（包括网页版和移动应用）所使用的系统提示词（system prompt）。这些提示词在每个对话开始时注入，用来为模型提供当前日期等最新信息，并引导语气、限制和输出格式等行为。社区开发者（如 Simon Willison）会追踪不同版本之间的差异，以分析模型行为的变化。

**「影响」** 对依赖 Claude 模型的开发者而言，公开的系统提示词可作为提示工程和回归测试的参考，减少对模型行为变化的盲区。

**「社区讨论」** 社区主要肯定这一透明做法，并已有人将提示词整理成 git 提交历史，便于查看 Opus 4.8 与 Opus 5 等版本间的具体差异。也有评论指出，系统提示词只是塑造行为的众多环节之一，并将危机干预等优先规则视为 Anthropic 对模型安全边界的明确指引。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs</a></li>
<li><a href="https://tactiq.io/learn/claude-system-prompt">Claude System Prompt Explained: What&#x27;s Inside and Why It Matters</a></li>
<li><a href="https://simonwillison.net/2025/May/25/claude-4-system-prompt/">Highlights from the Claude 4 system prompt</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#System Prompts`, `#Transparency`, `#Prompt Engineering`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B：本地表现优秀，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

Simon Willison 测试了阿里巴巴 Qwen 实验室发布的 Apache 2 许可、27B 参数、支持视觉的 Qwen 3.8 27B。官方自报基准显示它超过前代 Qwen 3.6 27B 以及闭源 Qwen 3.7-Plus（后者今年 5 月仍是 Qwen 最强模型之一），但独立基准尚未公布。他在 128GB M5 Max MacBook Pro 和 NVIDIA DGX Spark 上通过 LM Studio 的 17GB Q4\_K\_M 量化版运行，发现模型默认 reasoning\_effort 为 xhigh，导致即使简单请求也会疯狂思考：绘制“骑自行车的鹈鹕”SVG 花了 21 分钟、用掉 22,276 个推理 token 才输出 3,223 个 token，而关闭推理后同样任务约两分钟产出 3,715 个 token。他强烈建议先使用 low 或关闭推理，并指出默认 8,192 token 上下文不够用，需加载到 262,144 最大上下文。

rss · Simon Willison · 8月16日 22:00

**「背景」** Qwen 是阿里巴巴研究实验室发布的系列大语言模型；27B 参数级别适合在配置较好的笔记本上本地运行，前代 Qwen 3.6 27B 已表现出色。reasoning\_effort 是模型用于控制推理深度的官方参数，xhigh 追求细致分析，medium 平衡，low 偏向速度与成本。

**「影响」** 对希望在本地设备使用视觉模型的人而言，Qwen 3.8 27B 的默认 xhigh 设置会造成极端延迟和 token 浪费，按 Simon Willison 的建议改用 low 或关闭推理才能获得实用体验。

**标签**: `#Qwen`, `#LLM`, `#open source`, `#AI benchmarks`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [SSOG-Attention：可分离高斯和实现亚二次注意力，可扩展替代 SDPA](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 7.0/10

SSOG-Attention 提出一种基于可分离高斯和（Sum Of Separable Gaussians）的注意力机制，作为缩放点积注意力（SDPA）的亚二次复杂度替代方案。其通过为每个注意力头学习少量高斯原子，并依据查询词元仅进行几何引导，利用原子可分解为可分离高斯和的性质，将复杂度从 SDPA 的 O\(N²·d\) 降至 O\(N·√N·d\)。实验显示，在 CIFAR-100 小数据集上该方法明显优于 SDPA；在更大的 ImageNet（IN1k）数据集上达到相当性能且收敛更快，同时随规模增长保持更快的速度和更低的内存占用。作者公开了博客（https://pisoni.ai/posts/ssog）和代码仓库（https://github.com/4rtemis5/ssog），并说明部分代码和博客内容使用了 AI 协助但作者为内容负责。

reddit · r/MachineLearning · /u/4rtemi5 · 8月16日 10:06

**「背景信息」** SDPA 需要计算所有查询词元与所有键/图像词元之间的相似度得分，因此时间和内存复杂度随序列长度 N 呈二次增长，限制了长序列和高分辨率图像的处理。可分离高斯表示允许将多维高斯核分解为多个一维高斯滤波器的乘积或和，从而在保留局部注意力建模能力的同时减少计算与存储开销。

**「影响」** 对需要处理高分辨率图像或长序列的视觉模型开发者而言，该机制提供了比 SDPA 更可扩展的注意力实现，并在中小型数据集上显示竞争性能；但当前证据仅来自图像分类基准，尚需验证其在不同任务和更大模型上的泛化与稳定性。

**标签**: `#attention mechanism`, `#efficient attention`, `#machine learning`, `#computer vision`, `#Gaussian kernels`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储迎来多年来最难预测的会议](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 9.0/10

据《华尔街日报》报道，美联储即将召开的会议被认为是多年来最难预测的会议之一。

google\_news · WSJ · 7月23日 07:00

**「背景」** 美联储即将举行会议，近期通胀数据好坏参半：上月消费者价格出现 2020 年以来最大环比跌幅，但整体通胀率自 2021 年以来持续高于 2%的目标。

**「影响」** 美联储在 2025 年 9 月的议息会议后将银行准备金利率下调至 4.15%；有分析认为，这一决定会影响全球金融市场，包括黄金、白银和汇率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dailywire.com/news/fed-holds-rates-after-its-most-unpredictable-meeting-of-the-year">Fed Holds Rates After Its Most Unpredictable Meeting Of The Year</a></li>
<li><a href="https://www.federalreserve.gov/monetarypolicy/files/monetary20250917a1.pdf">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://www.markets.com/analysis/fed-rate-decision-september-2025-global-market-impact-1054-en">Fed Rate Decision September 2025: Impact of Rate Cuts on ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#economy`, `#markets`

---

<a id="item-finance-news-2"></a>
### [伊朗战争推动八大石油公司季度利润超 900 亿美元](https://oilprice.com/Energy/Energy-General/Oil-Majors-Reap-93-Billion-Windfall-From-the-Iran-War.html) ⭐️ 8.0/10

据 Oilprice.com 报道，美国、欧洲和中东的八大石油公司在 2025 年第二季度（4 月至 6 月）合计利润超过 900 亿美元，较上年同期略低于 500 亿美元的水平几乎翻倍。利润高企出现在伊朗战争导致霍尔木兹海峡几乎完全关闭之后。

rss · OilPrice.com · 8月16日 19:00

**「背景」** 霍尔木兹海峡位于阿曼与伊朗之间，是连接波斯湾与阿曼湾、阿拉伯海的关键航道；海峡关闭造成化石燃料供应严重短缺。布伦特原油价格 2 月底约为每桶 68 美元，5 月一度升至近 100 美元。

**「影响」** 高油价推高了全球消费者的能源账单，并重新引发多国政府对石油公司征收暴利税（即对超额利润征税）的讨论。

**标签**: `#oil prices`, `#Strait of Hormuz`, `#oil majors`, `#energy profits`, `#geopolitical risk`

---

<a id="item-finance-news-3"></a>
### [Anthropic 第二季初步营收破 115 亿美元，同比增长逾 14 倍](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

据彭博社援引的文件，Anthropic 第二季初步营收超过 115 亿美元，较去年同期的 7.87 亿美元增长逾 14 倍，也高于第一季的 47.3 亿美元；当季调整后营业利润转正。公司正筹备可能于今年秋季启动的大型 IPO，但初步数字仍可能调整。

telegram · zaihuapd · 8月16日 07:26

**「背景」** Anthropic 是一家人工智能安全与研究公司，以对话式 AI 助手 Claude 等产品著称，此前长期为获得风投支持的私营企业。

**「影响」** Anthropic 的初步营收数据正值其筹备大型 IPO 之际，可能为 AI 公司估值确立基准，并影响投资者对快速增长的 AI 行业的定价预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://forgeglobal.com/insights/how-to-invest-in-anthropic-pre-ipo/">Insights: How to Invest in Anthropic Pre-IPO - Forge</a></li>
<li><a href="https://listenlabs.ai/case-studies/anthropic">Anthropic &amp; Listen Labs | Customer Stories</a></li>
<li><a href="https://www.bnnbloomberg.ca/investing/investor-outlook/2026/06/03/investor-outlook-anthropic-ipo-filing-heats-up-ai-industry-race/">Anthropic filing puts spotlight on AI valuations</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#revenue growth`, `#AI industry`, `#IPO`, `#earnings`

---

<a id="item-finance-news-4"></a>
### [英伟达 30 亿美元押注 AI 电力基础设施](https://finance.yahoo.com/technology/ai/articles/nvidia-3-billion-bet-power-202314612.html) ⭐️ 8.0/10

NVIDIA 宣布投入 30 亿美元，目标是支撑人工智能（AI）的电力基础设施。

openbb · NVDA · 8月16日 20:23

**「背景」** 英伟达（Nvidia）据报道计划向总部位于得克萨斯州的电力与土地开发商 Lancium 投资至多 30 亿美元，以确保人工智能数据中心，尤其是耗电约 1.2 吉瓦（1 gigawatt = 10 亿瓦）的 Stargate 园区，获得足够的电力基础设施。相关消息最早由 The Information 报道。

**「影响」** 这项投资主要瞄准电力基础设施，可能影响数据中心运营商、电网企业和能源供应商，因为它旨在缓解 AI 算力扩张带来的电网瓶颈，并通过与能源企业的合作推动更灵活的供电方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/9020455/nvidia-to-invest-3-billion-in-lancium-for-ai-infrastructure-development-nvda">Nvidia to Invest $3 Billion in Lancium for AI Infrastructure Development (NVDA)</a></li>
<li><a href="https://datacenters.economictimes.indiatimes.com/news/ai-compute-infrastructure/nvidia-invests-3-billion-in-lancium-for-ai-power-access/133141093">Nvidia invests $3 billion in Lancium for AI power access, ETDatacenters</a></li>
<li><a href="https://truescho.com/en/blog/nvidia-stargate-lancium-3-billion-ai-infrastructure-2026">Nvidia $3B Stargate Investment 2026: AI Infrastructure | Truescho</a></li>
<li><a href="https://enkiai.com/data-center/nvidias-2026-power-play-how-ai-is-reshaping-the-grid/">NVIDIA&#x27;s 2026 Power Play: How AI Is Reshaping The Grid</a></li>
<li><a href="https://enkiai.com/nvidia/nvidia-power-strategy-2025-inside-the-ai-energy-pivot/">NVIDIA Power Strategy 2025: Inside the AI Energy Pivot - EnkiAI</a></li>
<li><a href="https://blogs.nvidia.com/blog/energy-efficiency-ai-factories-grid/">NVIDIA, Energy Leaders Accelerating Power‑Flexible AI ...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI`, `#investment`, `#energy`, `#data centers`

---

<a id="item-finance-news-5"></a>
### [格雷格·阿贝尔上季度投入近 350 亿美元](https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-successor-greg-abel-102200832.html) ⭐️ 8.0/10

据雅虎财经报道，伯克希尔·哈撒韦的沃伦·巴菲特继任者格雷格·阿贝尔上季度投入了近 350 亿美元资金。报道称该文说明了具体买入对象，但当前提供的摘要未包含这些细节。

openbb · BRK-B · 8月16日 10:22

**「背景」** 伯克希尔·哈撒韦由沃伦·巴菲特继任者格雷格·阿贝尔主导的资本部署近期明显加大；阿贝尔上一季度投入近 350 亿美元，涉及股票、收购和回购，其中买入谷歌母公司 Alphabet 约 4810 万股，并回购约 45 亿美元自家股票。据外媒报道，这打破了伯克希尔连续 14 个季度的净卖出趋势，使 Alphabet 成为其第三大持仓。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.msn.com/en-us/money/top-stocks/warren-buffett-s-successor-greg-abel-put-nearly-35-billion-of-cash-to-work-last-quarter-here-s-what-he-bought/ar-AA2adZZH">Warren Buffett&#x27;s successor, Greg Abel, put nearly $35 billion of ... - MSN</a></li>
<li><a href="https://apnews.com/article/berkshire-hathaway-warren-buffett-greg-abel-buybacks-e36ed92787eef9c9c67502501b345174">Berkshire Hathaway CEO Greg Abel spends cash on buybacks | AP News</a></li>
<li><a href="https://247wallst.com/investing/2026/08/15/alphabet-is-berkshire-hathaways-new-favorite-stock-after-buying-48-million-shares/">Alphabet Is Berkshire Hathaway&#x27;s New Favorite Stock After Buying 48 ...</a></li>

</ul>
</details>

**标签**: `#Berkshire Hathaway`, `#Greg Abel`, `#Capital Allocation`, `#Portfolio Management`, `#Investment Strategy`

---

<a id="item-finance-news-6"></a>
### [美联储 7 月会议决定维持利率不变](https://news.google.com/rss/articles/CBMiiwFBVV95cUxNUVVUMW1Hb2g1N2cyQkJneFl4YXJ1aFVvOGQzX19Oc2IxZUFyVUcwOXI0VmlpaW04d0N0MWZxVFlhSkJLUTltY3VxOVVHVGFBZHc5eVRzUTRQN1FXSEQ1Qm16U1pJMC1rOHNSdFd6UTEyWTF4cUpjX3NJUGs1alI3VGtLSmdNZmpOdjM0?oc=5) ⭐️ 8.0/10

美联储在 7 月会议上决定维持利率不变。

google\_news · Fortune · 7月29日 07:00

**「背景」** 美联储以 2%通胀率为长期目标，当前通胀仍高于该目标。本次会议维持利率不变，反映决策层在通胀压力与关税政策带来的经济不确定性之间权衡。

**「影响」** 利率维持不变意味着消费者的房贷、车贷和企业贷款等借贷成本暂时不会因央行加息而上升；但通胀仍偏高，且关税和地缘冲突构成压力，市场对后续是否加息仍有分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady | Fox Business</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-2025">Federal Reserve leaves key interest rate unchanged for fifth straight ...</a></li>
<li><a href="https://www.nbcnews.com/business/economy/fed-meeting-interest-rate-decision-kevin-warsh-rcna589536">Fed holds interest rates steady as Iran war and tariffs loom</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-7"></a>
### [美联储主席凯文·沃什在众议院就通胀与货币政策作证](https://news.google.com/rss/articles/CBMitwFBVV95cUxNNGoza1B1bFlYakZUZTlfMDZXQW5lak5PUUJmazNOUTZXdzZsb0ZfaUdNRmRZSmRHQmVLM1YweXBYaG5QWko3UE9pWk13MThsazJXZnAxZXQzdjFBNS1JQndtTU5WYzNjbExBWFVmaHRiUGlzNVB6WW9yTmdwQWdyWGNvWktMMWpQcXZrVWFtVGxwYW5WUEY1WEhJUWw2MTFfaFFBREMxQkVfUmx6WGVsNzZoU1AwYjjSAbwBQVVfeXFMTmJaLU9CcDhYZjVFbnJ1OEk5MFdNTzNNNlNQcjZTNnBndmtVMUFaaGVhYVZaR05MMnVKekp6NmlLdXZRbUwyUEdmLUZvT3h1bkVsVEZoR0k3MFN2QXIxTmY5bUtPdVVBODgwMHBiSDlqbl96VU9xSHppMGY4Q1M1VTVRVXl3VldVQ1dMTHoxNndVcDd5VEUySWZhSmU1RWtsSVpvUFVWWkI5T3Bfdy1FWHN2Zy1GT0R4UnhmN1M?oc=5) ⭐️ 8.0/10

PBS 报道称，美联储主席凯文·沃什在众议院听证会上就通胀和货币政策作证；该报道为直播提示，未包含作证内容的具体政策表态或数据。

google\_news · PBS · 7月13日 07:00

**「背景」** 这是美联储主席凯文·沃什首次以主席身份出席国会听证会，依据美联储每半年向国会提交的《货币政策报告》作证；他在事先准备的发言中表示，政策制定者对持续五年的高通胀“零容忍”，并将继续遏制物价上涨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/newsevents/testimony/warsh20260714a.htm">Testimony by Chairman Warsh on the semiannual Monetary Policy ...</a></li>
<li><a href="https://cryptobriefing.com/warsh-monetary-policy-report-house-committee/">Federal Reserve Chairman Warsh presents first Monetary Policy ...</a></li>
<li><a href="https://www.zerohedge.com/economics/warsh-tells-congress-fed-has-no-tolerance-elevated-inflation-watch-his-testimony-live">Warsh Tells Congress Fed Has &quot;No Tolerance For Elevated Inflation ...&quot;</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Congressional Hearing`

---

<a id="item-finance-news-8"></a>
### [美国中东石油出口数据现分歧：官方称回升至 1500 万桶/日，追踪机构称仅约 1000 万桶/日](https://oilprice.com/Energy/Crude-Oil/Have-Middle-East-Oil-Flows-Rebounded-to-15-Million-Bpd-as-US-Claims.html) ⭐️ 7.0/10

美国能源部长克里斯·赖特声称，中东石油出口已回升至每日 1500 万桶，周日单日流量甚至超过冲突前平均水平；但多家船舶追踪机构估计，中东所有出口渠道本月至今仅约每日 900 万至 1000 万桶。美国能源信息署也认为霍尔木兹海峡交通仍“严重受限”。

rss · OilPrice.com · 8月16日 23:00

**「背景」** 船舶追踪机构通过卫星和油轮装载数据估算出口量，而美方称其与美国军方协调拥有“最佳数据”，并称私营机构因船只关闭识别信号而漏数。美方没有说明数据如何编制；这些数字差异可能要等未来五六周各国进口数据公布后才能验证。

**标签**: `#Oil exports`, `#Middle East`, `#Energy policy`, `#Gasoline prices`, `#Tanker tracking`

---

<a id="item-finance-news-9"></a>
### [欧洲天然气库存降至 17 年最低](https://oilprice.com/Energy/Natural-Gas/Europes-Gas-Storage-Crunch-Deepens-Ahead-of-Heating-Season.html) ⭐️ 7.0/10

据行业媒体报道，欧洲天然气库存已降至 17 年最低，且临近供暖季仍需继续购气；欧盟还将于明年 1 月起禁止购买俄罗斯液化天然气，令供应更加紧张。

rss · OilPrice.com · 8月16日 21:00

**「背景」** 欧洲过去几年因制裁俄罗斯而转向美国液化天然气，今年夏季高温推高发电用气需求，导致库存未能在夏季淡季充分补充。

**「影响」** 若补库不及预期，冬季供暖和电力价格可能进一步上涨，令欧洲家庭和企业能源成本承压。

**标签**: `#natural gas`, `#Europe`, `#energy security`, `#LNG`, `#sanctions`

---

<a id="item-finance-news-10"></a>
### [人工智能扩张或延长化石燃料主导地位](https://oilprice.com/Energy/Energy-General/AI-Set-to-Extend-Fossil-Fuel-Dominance.html) ⭐️ 7.0/10

人工智能的快速扩张正推动大型科技公司碳排放以两位数增长：按官方公司数据，谷歌和微软在 2025 至 2026 年间的年度总排放同比各增 25%，亚马逊增 16%，三家公司在上一财年合计排放 1900 万吨二氧化碳当量，相当于法国排放总量的三分之一。发表于《自然》旗下期刊的研究警告，人工智能通过提升化石燃料行业收益，可能延长其主导地位，而非带来减排。

rss · OilPrice.com · 8月16日 17:00

**「背景」** 数据中心建设速度超过清洁能源供应，促使科技企业转向天然气等一切可用电源。上述研究测算，若化石燃料和可再生能源从人工智能获益幅度相同，全球二氧化碳年排放将增加 4.7 亿至 18 亿吨；只有可再生能源获益达到化石燃料的 4 至 5 倍，人工智能才能产生净减排。

**「影响」** 若缺乏政策干预，研究预计人工智能会提高全球经济碳强度并强化化石燃料的现有地位；亚马逊在得克萨斯州南部投建的天然气电厂若按计划建成，可能成为全美单点排放最大的电厂，获准年排放 3300 万吨二氧化碳。

**标签**: `#AI`, `#fossil fuels`, `#carbon emissions`, `#data centers`, `#energy policy`

---

<a id="item-finance-news-11"></a>
### [AMD 发行 47.5 亿美元债券，规模为上次三倍多](https://finance.yahoo.com/markets/stocks/articles/amd-just-borrowed-4-75-023900183.html) ⭐️ 7.0/10

AMD 通过债券发行借入 47.5 亿美元，实际融资规模是此前最近一次发债的三倍多。

openbb · NVDA · 8月16日 02:39

**「背景」** AMD 本周完成了公司史上最大规模的债券发行，通过四批 2029 年至 2036 年到期的优先票据筹集 47.5 亿美元；这类发债通常用于满足资本开支需求，本次也与人工智能需求相关。

**「影响」** 这笔 45.7 亿美元的债券发行是 AMD 历史上规模最大的债务融资，凸显其人工智能扩张所需的巨额现金。此前 AMD 在 2025 年 3 月仅借款 15 亿美元，此次规模超过三倍。债券需求强劲，最长年期债券定价较初步讨论收窄 0.25 个百分点，显示投资者对 AMD AI 增长计划的信心，同时也意味着公司债务负担增加。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/amd-plans-to-raise-as-much-as-5-billion-from-debt-offering">AMD Raises $4.75 Billion From Bond Sale as AI Demand Surges - Bloomberg</a></li>
<li><a href="https://www.fool.com/investing/2026/08/15/amd-just-borrowed-475-billion-more-than-triple-its/">AMD Just Borrowed $4.75 Billion, More Than Triple Its Last Bond Sale | The Motley Fool</a></li>
<li><a href="https://www.briefs.co/news/chipmaker-s-largest-debt-deal-yet-4-75-billion-for-ai-growth/">AMD&#x27;s $4.75 Billion Bond Sale Funds AI Growth - briefs.co</a></li>

</ul>
</details>

**标签**: `#AMD`, `#Debt Financing`, `#Semiconductor Industry`, `#Capital Markets`, `#Bond Sale`

---

<a id="item-finance-news-12"></a>
### [黄金触及每盎司 4,400 美元，矿企股开始跟进上涨](https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html) ⭐️ 7.0/10

据头条报道，黄金价格已触及每盎司 4,400 美元，矿业股也开始跟进上涨，但报道未提供具体数据基准或详细说明。

openbb · GLD · 8月16日 14:21

**「背景」** 金价近日突破每盎司 4,000 美元并逼近 4,400 美元的历史高位，而矿业股此前多年涨幅落后于金价；据相关市场分析，7 月以来这一差距开始快速收窄。

**「影响」** 金矿企业和矿业股投资者是直接受益者：金价创新高带动矿业股追涨，收窄了此前矿业股落后于金价的差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html">Gold Just Hit $4,400 and the Miners Are Finally Catching Up</a></li>
<li><a href="https://www.cnbc.com/2025/10/08/gold-zooms-past-4000-for-first-time-in-historic-flight-to-safety.html">Gold shatters $4,000 milestone, silver belts record high as ... - CNBC</a></li>
<li><a href="https://economictimes.indiatimes.com/news/international/us/gold-price-to-touch-highest-closing-price-ever-now-close-to-4400-why-is-gold-price-nearing-fresh-record-highs-heading-into-2026/articleshow/125935722.cms">Gold price to touch highest closing price ever, now close to $4,400 ...</a></li>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html?fr=sycsrp_catchall">Gold Just Hit $4,400 and the Miners Are Finally Catching Up</a></li>
<li><a href="https://www.usfunds.com/resource/these-mining-stocks-have-rallied-the-most-from-high-gold-prices/">These Mining Stocks Have Rallied the Most from High Gold ...</a></li>
<li><a href="https://thescjournal.com/business/gold-prices-surge-to-record-highs-surpassing-4400-an-ounce/">Gold Prices Surge to Record Highs, Surpassing $4,400 an Ounce</a></li>

</ul>
</details>

**标签**: `#gold`, `#commodity prices`, `#mining stocks`, `#precious metals`, `#market milestone`

---

<a id="item-finance-news-13"></a>
### [多家消费巨头 CEO 警告：美国消费者资金紧张](https://finance.yahoo.com/economy/articles/running-money-kraft-mcdonald-whirlpool-114500035.html) ⭐️ 7.0/10

卡夫、麦当劳和惠而浦的首席执行官均警告，美国消费者正“耗尽资金”，这是他们在近期财报电话会上发出的预测，可能预示消费者支出将减弱。该表态属于企业高管的判断，并非已公布的经济数据。

openbb · PG · 8月16日 11:45

**「背景」** 这些表态出自近期财报电话会议：卡夫亨氏 CEO 表示，低收入消费者面临的财务压力最明显，并称并非所有美国人都在耗尽资金；多家公司 CEO 还提到消费者储蓄减少、更多依赖信用卡支付日常开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/articles/running-money-kraft-mcdonald-whirlpool-114500035.html">‘ Running out of money ’: Kraft , McDonald ’ s , Whirlpool CEOs all flag...</a></li>
<li><a href="https://www.linkedin.com/posts/matthewsboyle_americans-are-running-out-of-money-the-ceos-activity-7458252875631276033-VFx8">CEOs Warn Americans Are Running Out of Money | LinkedIn</a></li>

</ul>
</details>

**标签**: `#Consumer Spending`, `#Economic Slowdown`, `#Corporate Earnings`, `#Retail`, `#US Economy`

---