---
layout: default
title: "Horizon Summary: 2026-09-04 (ZH)"
date: 2026-09-04
lang: zh
---

> 从 234 条内容中筛选出 18 条重要资讯。

---

**科技新闻**
1. [GPT-6 Astra 发布：ARC-AGI-3 表现引热议](#item-tech-news-1) ⭐️ 9.0/10
2. [Audacity 4.0 发布：Qt6 界面重构与社区争论](#item-tech-news-2) ⭐️ 9.0/10
3. [美政府支持 OpenAI：AI 训练属合理使用](#item-tech-news-3) ⭐️ 8.0/10
4. [用 LLM 把 1993 年 Amiga 汇编游戏移植到 Godot](#item-tech-news-4) ⭐️ 7.0/10
5. [GPT-6 Astra 的 ARC-AGI-3 评测](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [美国与委内瑞拉油田协议威胁中国石油偿贷](#item-finance-news-1) ⭐️ 8.0/10
2. [美国柴油价格逼近历史最高纪录](#item-finance-news-2) ⭐️ 8.0/10
3. [欧盟在莱比锡无人机事件后拟对俄罗斯实施更严制裁](#item-finance-news-3) ⭐️ 8.0/10
4. [美国考虑对进口芯片加征新一轮关税以推动制造回流](#item-finance-news-4) ⭐️ 8.0/10
5. [英伟达拟以 140 亿美元收购一家免费开放核心成果的公司](#item-finance-news-5) ⭐️ 8.0/10
6. [美联储 9 比 3 投票维持利率不变](#item-finance-news-6) ⭐️ 8.0/10
7. [美联储偏好的通胀指标创三年最快涨幅](#item-finance-news-7) ⭐️ 8.0/10
8. [财报与指引引发盘前个股大幅波动](#item-finance-news-8) ⭐️ 7.0/10
9. [AI 数据中心热潮令美国电力设备供应承压](#item-finance-news-9) ⭐️ 7.0/10
10. [2025 年全球零排放中重型卡车及客车销量增 86%，电动卡车进入规模化阶段](#item-finance-news-10) ⭐️ 7.0/10
11. [高油价推动中国加速减少石油消费](#item-finance-news-11) ⭐️ 7.0/10
12. [巴西国会通过法案，授权政府干预矿业并购](#item-finance-news-12) ⭐️ 7.0/10
13. [马查多支持美国参与委内瑞拉石油合作，但质疑协议授权](#item-finance-news-13) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GPT-6 Astra 发布：ARC-AGI-3 表现引热议](https://openai.com/index/gpt-6-astra/) ⭐️ 9.0/10

OpenAI 发布了旗舰模型 GPT-6 Astra，官方页面提供了部署安全系统卡，并将其定位为与 GPT-4、GPT-5 同级的新一代旗舰版本。该模型开始推送引发社区高度关注，讨论集中在其 ARC-AGI-3 得分，有评论称达到 99.9%，但批评者认为官方成绩单存在对比方法争议，例如在相同响应 API 测试条件下对 GPT-5.6 Sol 的估算约为 30%，而表格中仍显示 7.8%。社区同时指出，除 ARC-AGI-3 外，多数其他基准的提升相对温和，更像渐进式改进，并提醒需等待 OpenAI 公布更多关于测试流程、推理保留与压缩等细节。

hackernews · kibae · 9月3日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49554643)

**「背景」** GPT-6 Astra 是 OpenAI 本次发布的下一代旗舰模型。相关讨论主要围绕 ARC-AGI-3 基准展开：OpenAI 宣称 Astra 在该基准上得分约为 98.6%，而 ARC Prize 使用标准 harness（允许模型在环境中保留笔记）测得 Astra（max）在 ARC-AGI-3 Semi-Private 上得分 62.7%，成本约 2.6 万美元。第三方评论指出，未披露的测试设置使该分数需要谨慎解读。需要理解的是，ARC-AGI-3 是用于测试抽象推理和泛化能力的高难度基准，而厂商自定义的评测 harness 可能改变模型的推理保留与信息压缩方式，这使得同一模型在不同评测设定下可能出现明显分数差异。

**「影响」** 若由独立第三方验证其 ARC-AGI-3 高分属实，GPT-6 Astra 可能成为衡量推理能力的新标杆，推动研究者和开发者重新审视现有基准的测试条件与公平性；当前结论仍需依赖 OpenAI 后续公布的详细方法。

**「社区讨论」** 社区反应两极：一部分人认为 ARC-AGI-3 的 99.9% 得分令人瞩目，另一部分人质疑基准展示有失公允，并认为其他 benchmarks 提升有限，更像技能获取而非通用智能突破。也有评论顺带批评演示偏爱“AI 自主购物”场景，认为这并不贴近用户真实决策需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/blog/astra">OpenAI&#x27;s GPT-6 Astra on ARC-AGI-3 | ARC Prize</a></li>
<li><a href="https://thenewstack.io/astra-arc-agi-benchmark/">GPT-6 Astra aced the hardest AI benchmark. The asterisk matters more than the score. - The New Stack</a></li>
<li><a href="https://venturebeat.com/technology/welcome-to-the-agi-era-openai-launches-gpt-6-astra">&#x27;Welcome to the AGI era&#x27;: OpenAI launches GPT-6 Astra | VentureBeat</a></li>

</ul>
</details>

**标签**: `#GPT-6`, `#OpenAI`, `#AI`, `#benchmarks`, `#language models`

---

<a id="item-tech-news-2"></a>
### [Audacity 4.0 发布：Qt6 界面重构与社区争论](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 9.0/10

Audacity 4.0（发布标签 Audacity-4.0.0）是开源音频编辑器的一次主要版本发布，引入了基于 Qt6 的界面以及一系列值得注意的改进。该版本通过项目的官方 GitHub Releases 页面分发。作为广泛使用的免费音频工具，Qt6 界面重构标志着一次重要的现代化升级。此次发布在 Hacker News 上引发了大量关注与讨论，社区聚焦于新界面以及音频后端支持尚未解决的问题。

hackernews · ClydeN · 9月3日 10:53 · [社区讨论](https://news.ycombinator.com/item?id=49548395)

**「背景」** Audacity 是一款开源音频编辑软件，长期以 3.x 版本提供录音、剪辑和导出等功能。4.0.0 是官方发布的主要版本更新，将应用程序界面重构到 Qt 之上，并引入了新的片段（clip）编辑模型、更灵活的录音流程以及新的项目文件格式。由于这些改动改变了旧版 3.x 系列的操作方式和文件兼容性，因此了解版本演进有助于判断升级和迁移的影响。

**「社区讨论」** 有评论者推荐了介绍新 Qt6 界面和开发过程的官方视频；一位已经放弃 Audacity 的用户表示，4.0 的更新日志并没有解决它在 Linux 家庭录音系统中 JACK/Pipewire 集成方面的烦人问题。另一位长期使用 v3 制作音乐的用户觉得 v4 测试版更干净，并修复了工程保存和片段“咔哒”声等问题，但担忧不断增强的 audio.com 集成；还有人问起 Tenacity、Sneedacity 等去遥测分支的现状。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0">Release Audacity - 4 . 0 . 0 · audacity / audacity · GitHub</a></li>
<li><a href="https://www.audacityteam.org/changelog/">What changed in each release of Audacity , from 3. 0 . 0 onwards.</a></li>
<li><a href="https://www.omgubuntu.co.uk/2026/09/audacity-4-released">Audacity 4 . 0 released with brand-new look, clip... - OMG! Ubuntu</a></li>

</ul>
</details>

**标签**: `#audacity`, `#open-source`, `#audio-editing`, `#qt6`, `#release`

---

<a id="item-tech-news-3"></a>
### [美政府支持 OpenAI：AI 训练属合理使用](https://www.reuters.com/legal/litigation/us-government-backs-openai-new-york-times-copyright-case-2026-09-02/) ⭐️ 8.0/10

美国政府向曼哈顿联邦法院提交意见书，支持 OpenAI 在与《纽约时报》等媒体的版权纠纷中胜诉，主张使用受版权保护的内容训练大语言模型通常属于合理使用。这是美国政府首次就 AI 训练版权问题正式表态；意见书虽不具法律约束力，但可能增强科技公司在类似诉讼中的应诉底气。《纽约时报》则批评政府站在“少数万亿美元级 AI 公司”一边，牺牲创作者权益。该报于 2023 年起诉 OpenAI 及微软，指控其未经许可使用其数百万篇文章训练 ChatGPT。

telegram · zaihuapd · 9月3日 05:45

**「背景」** 合理使用是美国版权法中的一项限制与例外，允许在评论、教学、新闻报道等目的下未经权利人许可使用受版权保护的作品，判断时通常考虑使用目的与性质、原作品性质、使用比例以及对原作品市场的影响。《纽约时报》于 2023 年起诉 OpenAI 及其主要投资方微软，指控其擅自使用该报数百万篇文章训练 ChatGPT。美国政府于 2026 年 9 月 2 日在曼哈顿联邦法院提交法庭之友意见书，首次正式表明支持“用受版权保护内容训练 AI 一般属于合理使用”的立场，并称生成式 AI 训练具有高度变革性，但该意见书不具法律约束力。

**「影响」** 美国政府提交的非约束性意见书主张 AI 训练通常构成合理使用，可能增强 OpenAI 及其他 AI 公司在版权诉讼中的抗辩立场，影响纽约时报案以及类似案件的走向；但意见书不具法律约束力，最终裁判仍由法院作出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.indiavision.com/business/trump-administration-sides-with-openai-in-new-york-times-copyright-lawsuit/606575/">Trump Administration Sides With OpenAI in New York Times Copyright Lawsuit - IndiaVision India News &amp; Information</a></li>
<li><a href="https://appleinsider.com/articles/26/09/02/us-government-worried-that-ai-companies-cant-innovate-without-legal-theft">US government worried that AI companies can&#x27;t innovate without legal theft</a></li>
<li><a href="https://www.datastudios.org/post/us-government-backs-openai-new-york-times-copyright-fair-use-ai-training">US Government Backs OpenAI in New York Times Copyright Case: Fair Use and AI Training</a></li>
<li><a href="https://www.datastudios.org/post/us-government-backs-openai-new-york-times-copyright-fair-use-ai-training">US Government Backs OpenAI in New York Times Copyright Case: Fair Use and AI Training</a></li>
<li><a href="https://tradersunion.com/news/financial-news/show/3198058-openai-us-support-nyt-copyright-case/">OpenAI gains U.S. government backing in New York Times copyright training case</a></li>
<li><a href="https://sjvsun.com/u-s/government-sides-with-openai-in-new-york-times-copyright-battle/">Government sides with OpenAI in New York Times copyright battle</a></li>

</ul>
</details>

**标签**: `#AI`, `#copyright`, `#legal`, `#OpenAI`, `#policy`

---

<a id="item-tech-news-4"></a>
### [用 LLM 把 1993 年 Amiga 汇编游戏移植到 Godot](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 7.0/10

作者用大语言模型（文中称 Claude Fable 5）把自己 1993 年在巴格达用 MC68000 汇编为 Amiga 编写的游戏移植到 Godot；核心流程是先让模型在 Mac 上用 vasm 反复汇编，直到生成与原二进制逐字节相同的目标文件，再据此重写游戏。首个可用版本只花了一个晚上，但调整手感并正式发布又用了几周和几个晚上；作者还把原始素材、笔记和 33 年记忆作为提示资料，并让模型起草本文后逐行编辑。文章披露了一处未完全查证的细节：原游戏用 AsmOne 汇编到内存后把运行中的内存快照保存为发行文件，因此与干净汇编输出存在约 108 字节差异，模型直到命中这个差异才停止。作者同时免费发布了原版游戏，为 AI 辅助逆向与老旧游戏移植提供了一个具体、可复制的案例。

hackernews · rabahs · 9月3日 14:28 · [社区讨论](https://news.ycombinator.com/item?id=49550375)

**「背景」** Amiga 是 1980 至 1990 年代流行的个人电脑，MC68000 汇编接近机器码，游戏直接操作内存和定制芯片，这类源码很难在现代平台直接维护。Godot 是开源游戏引擎，支持用高级语言和脚本重写游戏逻辑，因此把汇编逻辑翻译成 Godot 项目是复原老游戏的一条现实路径。文章中的 108 字节差异源于 AsmOne 会先在内存中运行程序再保存内存快照，而不是输出全新汇编二进制。

**「影响」** 作者把原版游戏免费发布，并公开了详细移植笔记，为其他想用 LLM 复活或移植老汇编游戏的开发者提供了一个端到端范例。另一个具体结果是，模型生成的二进制必须与原始快照逐字节一致才继续，说明个人项目上的 AI 辅助“代码考古”已经可以落地。

**「社区讨论」** 评论者普遍表示赞赏，并分享了自己的类似经历：mattjoyce 让 Claude 把一个 ZX81 游戏的内存转储转成 Go 并成功运行；dannyobrien 感慨 1993 年手工汇编开发不易并询问调试故事；hedgehog 希望作者让 Claude 导出一份通用移植工程指南；glimshe 则计划用同样方法移植另一款被遗忘的游戏。还有评论猜测游戏灵感是否来自《Gods: Into the Wonderful》，作者尚未在摘录中回应。

**标签**: `#LLM-assisted development`, `#reverse engineering`, `#retro game porting`, `#Godot`, `#assembly`

---

<a id="item-tech-news-5"></a>
### [GPT-6 Astra 的 ARC-AGI-3 评测](https://arcprize.org/blog/astra) ⭐️ 7.0/10

ARC Prize 发布了 OpenAI GPT-6 Astra 在 ARC-AGI-3 基准上的评测，相关讨论聚焦于性能、成本与智能定义，并未将其视为明确突破。评论者引用 Epoch 的 FrontierMath Erdős 数据显示，在参与测试的模型中只有 GPT-6 Astra 有解出题目：68 题中解出 2 题，包括用 15 小时和 218 美元以反例否定第 74 题、用 16 小时和 247 美元证明第 126 题；如果把多次尝试都计入，则合计解出 5 题。评论估算每道题成本约 360 美元，并对比人类测试者约 10 分钟完成一道题的速度，显示当前经济性仍较差。另有评论质疑最小步数式解谜任务是否真正衡量智能，以及 OpenAI 是否可能提前接触测试题并针对 ARC-AGI-3 构建定制提示或强化学习流程。

hackernews · vignesh\_warar · 9月3日 19:45 · [社区讨论](https://news.ycombinator.com/item?id=49555691)

**「背景」** ARC-AGI-3 是一个用于研究代理型智能的基准测试，要求智能体在全新、抽象的回合制环境中探索、推断目标并构建环境的内部模型，以便在没有明确指令的情况下有效地规划行动。OpenAI 的 GPT-6 Astra 在该基准上取得了经过 ARC Prize 验证的结果（2026 年 9 月 2 日），而此前 Anthropic 的 Claude Opus 5 以约 30.2% 的表现位列前茅，OpenAI 自己的 GPT-5.6 Sol 在官方测试条件下仅为 7.78%。这些结果反映了当前模型在抽象推理与自主探索类任务上的进展水平。

**「社区讨论」** 许多评论者认为若价格与性能按既有速度继续改善，两三年内 AI 解题成本可能低于美国最低工资的人工测试；另一些人则质疑用最少步数解谜题是否等于衡量智能。还有评论担心 OpenAI 会不会预先知道 ARC-AGI-3 的具体题目，并针对该测试集使用监督强化学习或定制提示来优化结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/blog/astra">OpenAI &#x27;s GPT - 6 Astra on ARC - AGI - 3 | ARC Prize</a></li>
<li><a href="https://arcprize.org/results/openai-gpt-6-astra">GPT - 6 Astra - ARC - AGI Results</a></li>
<li><a href="https://cryptobriefing.com/gpt-6-astra-arc-agi-3-claims-unverified/">Claims of GPT - 6 Astra scoring 98.6% on ARC - AGI - 3 don&#x27;t hold up to...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6 Astra`, `#ARC-AGI`, `#AI benchmarking`, `#artificial intelligence`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美国与委内瑞拉油田协议威胁中国石油偿贷](https://oilprice.com/Energy/Crude-Oil/US-Venezuela-Oil-Deal-Threatens-Chinas-Oil-Backed-Loans.html) ⭐️ 8.0/10

美国与委内瑞拉的新协议将 17 个含约 65 亿桶探明储量的油田 100 年期开发权授予美方关联企业 NABEP，美国政府可取得其母公司 35%股份并以成本价购买两成产量；分析师估计，委内瑞拉对中国贷款人至少还有 100 亿美元以石油偿还的债务，清收前景因此更难。

rss · OilPrice.com · 9月4日 00:00

**「背景」** 长期以来，中国政策性银行以石油交付作为偿还方式向委内瑞拉提供融资，截至 2015 年至少放贷 600 亿美元；本次纳入 NABEP 的部分油田此前由中石油、中石化等中国企业运营或推进开发。

**「影响」** 对中国而言，损失可能包括贷款回收周期拉长、独立炼厂失去折扣重质原油供应，以及油企被排除在已投入多年的油田之外；美国则增加了对委内瑞拉石油流向的影响力。

**标签**: `#Venezuela`, `#China`, `#oil`, `#geopolitics`, `#debt`

---

<a id="item-finance-news-2"></a>
### [美国柴油价格逼近历史最高纪录](https://oilprice.com/Energy/Gas-Prices/US-Diesel-Prices-Surge-Toward-All-Time-High.html) ⭐️ 8.0/10

美国汽车协会（AAA）数据显示，美国柴油平均价格周四升至每加仑 5.7832 美元，仅比 2022 年 6 月创下的历史纪录 5.8159 美元低约 3 美分。汽油价格也处于同期高位，供应中断和季节性需求推动全美油价上行。

rss · OilPrice.com · 9月3日 15:00

**「背景」** 柴油是货运、农业和商品生产的核心燃料，其价格上涨会推高物流和消费品成本，因此也是美国经济和美联储利率政策关注的重要变量。

**「影响」** 若柴油价格继续走高，运输企业和农户的成本将承压，并可能进一步传导至商品价格，增加通胀压力，从而影响美联储的利率决策。

**标签**: `#diesel prices`, `#U.S. economy`, `#inflation`, `#energy supply`, `#Federal Reserve`

---

<a id="item-finance-news-3"></a>
### [欧盟在莱比锡无人机事件后拟对俄罗斯实施更严制裁](https://oilprice.com/Geopolitics/Europe/EU-Vows-Tougher-Russia-Measures-After-Leipzig-Drone-Attack.html) ⭐️ 8.0/10

欧盟委员会主席冯德莱恩 9 月 2 日表示，莱比锡机场遭携带爆炸物无人机袭击是“新常态”，欧盟将采取更严格对俄措施。欧盟外交政策机构已提议对约 1600 个俄罗斯国防相关个人和企业实施签证禁令和资产冻结，计划下月通过。

rss · OilPrice.com · 9月3日 14:00

**「背景」** 德国 8 月 4 日至 5 日莱比锡机场发生携带爆炸物无人机袭击、导致航班中断；德国官方 9 月 1 日将事件归咎于俄罗斯，欧盟及法国、比利时、葡萄牙、荷兰等为此召见俄罗斯大使。此外，欧盟外长讨论限制俄罗斯公民使用申根旅游签证，因涉嫌肇事者据德媒报道持意大利签发的申根旅游签证入境，但部分南欧国家表示反对。

**标签**: `#EU`, `#Russia`, `#sanctions`, `#defense`, `#geopolitics`

---

<a id="item-finance-news-4"></a>
### [美国考虑对进口芯片加征新一轮关税以推动制造回流](https://www.bloomberg.com/news/videos/2026-09-03/trump-to-levy-more-chip-tariffs-to-boost-manufacturing-video) ⭐️ 8.0/10

美国商务部长霍华德·卢特尼克表示，特朗普政府正考虑对进口半导体以及数据中心服务器、消费电子等含芯片产品加征新一轮关税，以推动更多芯片制造回流美国。据报道，政府倾向对在美建设生产能力的企业提供关税减免，但这项计划仍在考虑中，尚未最终决定。

telegram · zaihuapd · 9月3日 07:00

**「背景」** 该政策构想的核心机制，是通过抬高进口成本并配套本土投资关税优惠来刺激芯片制造回流。在台湾 Semicon 展会现场，芯片供应链企业仍对强劲的美国 AI 芯片需求持乐观态度。

**标签**: `#tariffs`, `#semiconductors`, `#trade policy`, `#manufacturing`, `#AI chips`

---

<a id="item-finance-news-5"></a>
### [英伟达拟以 140 亿美元收购一家免费开放核心成果的公司](https://finance.yahoo.com/technology/ai/articles/nvidia-paying-14-billion-company-170037102.html) ⭐️ 8.0/10

据相关报道，英伟达正以 140 亿美元收购一家将其最优秀成果免费开放的公司。此举被分析视为英伟达对开源人工智能技术的一项战略押注。

openbb · NVDA · 9月3日 17:00

**「背景」** Hugging Face 是一个开发者分享和展示 AI 模型（包括开源模型）的主要平台。据彭博社报道，Nvidia 正洽谈以 140 亿美元收购该公司，若完成将成为今年 AI 行业最大并购交易。Nvidia 首席执行官黄仁勋曾表示支持开源模型，以避免 AI 技术被少数大公司垄断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=g-YDNJcyuck">Nvidia Nears $ 14 Billion Hugging Face Deal | Bloomberg... - YouTube</a></li>
<li><a href="https://eu.36kr.com/en/p/3966094074600965">NVIDIA $ 14 B Hugging Face Acquisition Set to Become...</a></li>
<li><a href="https://www.arcamax.com/business/businessnews/s-4289228">Nvidia nears $ 14 billion Hugging Face deal this... | ArcaMax Publishing</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Acquisition`, `#AI`, `#Open Source`, `#M&amp;A`

---

<a id="item-finance-news-6"></a>
### [美联储 9 比 3 投票维持利率不变](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 8.0/10

美国联邦储备委员会（美联储）在 9 比 3 的投票中决定维持利率不变。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 本次会议是美联储主席凯文·沃什（Kevin Warsh）上任后的首次利率决策会议。美联储在 2026 年 6 月 16 日至 17 日的会议上决定将联邦基金利率目标区间维持在 3.5%至 3.75%不变，以应对美国经济面临的通胀压力。

**「影响」** 利率维持不变意味着消费者和企业的借贷成本将继续保持在当前水平，较高的借贷成本会抑制支出和投资，从而有助于缓解通胀压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-holds-interest-rates-steady-220059911.html?fr=sycsrp_catchall">Federal Reserve Holds Interest Rates Steady At 3.5%-3.75% In ...</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-tapering-asset-purchases.html">What Federal Reserve monetary policy means for investors</a></li>
<li><a href="https://www.federalreserve.gov/faqs/money_12856.htm">The Fed - How does the Federal Reserve affect inflation and employment?</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#central bank`

---

<a id="item-finance-news-7"></a>
### [美联储偏好的通胀指标创三年最快涨幅](https://news.google.com/rss/articles/CBMiigFBVV95cUxNODJpSG0zUXZ3T3JiemstZEM0ek55U3NHQVh2YlVSdG1WZnBwdEFMQUhmemQ5NnlmVk0teWFqV2lsRXJ2XzB0ZjJ5YW91ejZWUjRzZ2RkdzdCekdGNjAya2VIRnVPbmdSODE4WlEyR1BVY3hBeXhyTDV4NmZBVE9ybkpkbERKTnh2cFE?oc=5) ⭐️ 8.0/10

CBS 新闻援引最新数据报道，美联储偏好的通胀指标显示物价正以三年来最快速度上涨，反映价格压力有所加大。报道未给出具体的通胀数字。

google\_news · CBS News · 6月25日 07:00

**「背景」** 美国商务部数据显示，美联储主要追踪的通胀指标——个人消费支出（PCE）价格指数在截至 2026 年 5 月的一年里上涨 4.1%，高于 4 月的 3.8%，为 2023 年 4 月以来最快增速。美联储以 PCE 作为判断通胀压力的核心指标，能源价格尤其是汽油价格上涨是推高通胀的重要因素。

**「影响」** 据市场报道，美联储官员已暗示可能再次加息，因为 3 月个人消费支出价格指数（PCE）通胀率仍高于 2%的目标；若实施，家庭和企业的信贷成本将增加。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://piptheory.com/research/pce-inflation-3-year-high-dollar">The Fed&#x27;s Preferred Inflation Gauge Just Hit a 3 - Year ... — Pip Theory</a></li>
<li><a href="https://www.theguardian.com/business/2026/jun/25/us-may-inflation-gauge-three-year-high">Key Fed inflation gauge rises to three - year high in... | The Guardian</a></li>
<li><a href="https://market-pulse.co/article/19397/fed-officials-signal-potential-rate-hikes-as-inflation-persists-above-target">Fed Officials Signal Potential Rate Hikes as Inflation ... | MarketPulse</a></li>

</ul>
</details>

**标签**: `#inflation`, `#Federal Reserve`, `#PCE price index`, `#economic data`, `#monetary policy`

---

<a id="item-finance-news-8"></a>
### [财报与指引引发盘前个股大幅波动](https://www.cnbc.com/2026/09/03/stocks-making-the-biggest-moves-premarket-snow-mrna-avgo.html) ⭐️ 7.0/10

盘前个股行情主要受财报与业绩指引影响：Snowflake 第二季度调整后每股收益 62 美分、营收 15.5 亿美元，高于分析师预期的 45 美分和 14.8 亿美元，并上调全年产品收入指引，股价大涨 24%；Ultragenyx 因治疗 Angelman 综合征的药物三期试验未达主要终点，股价大跌逾 46%。

rss · CNBC Finance · 9月3日 11:35

**「背景」** 这类波动属于公司层面的消息反应，不一定代表大盘走向；Snowflake 的强势上涨也带动部分软件同行走高，例如 Datadog 涨逾 5%、ServiceNow 涨 3%，而 Broadcom 因第四财季收入指引低于预期下跌 2.5%。

**标签**: `#Earnings`, `#Premarket Movers`, `#Guidance`, `#Software`, `#Biotech`

---

<a id="item-finance-news-9"></a>
### [AI 数据中心热潮令美国电力设备供应承压](https://oilprice.com/Energy/Energy-General/AI-Data-Center-Boom-Pushes-US-Power-Equipment-to-the-Breaking-Point.html) ⭐️ 7.0/10

AI 数据中心建设热潮正在加剧美国电力设备短缺。据伍德麦肯兹估计，今年变压器供应缺口为 15%，变电站缺口为 8%；韩国现代电气表示其积压订单已增至 85 亿美元，较上半年增长 23%。

rss · OilPrice.com · 9月3日 22:00

**「背景」** 变压器是把高压电转为用户可用低压电的关键电网设备。美国近年因数据中心用电激增已出现变压器供应紧张，特朗普政府又下令禁止进口中国产大容量电力设备，使本就吃紧的设备供应更难缓解。

**「影响」** 美国电网设备短缺可能直接影响 AI 数据中心建设进度：大型科技公司和公用事业公司面临变压器（今年短缺约 15%）、变电站（缺口约 8%）以及多至数年的订单积压，新建或扩容数据中心可能需要等待更长时间才能接入电网。外部研究也预计，AI 基础设施扩张将推高电力设备需求，但设备短缺和交货期延长可能威胁后续建设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://solmarcapital.co/bulk-power-import-ban-transformer-shortage/">Bulk-power import ban heightens U.S. transformer shortfall</a></li>
<li><a href="https://collapse.news/2026-05-02-ai-data-center-boom-drives-65b-equipment-demand.html">AI Data Center Boom Drives $65 Billion Power Equipment Demand...</a></li>

</ul>
</details>

**标签**: `#power equipment`, `#data centers`, `#electricity demand`, `#supply chain`, `#AI infrastructure`

---

<a id="item-finance-news-10"></a>
### [2025 年全球零排放中重型卡车及客车销量增 86%，电动卡车进入规模化阶段](https://oilprice.com/Energy/Energy-General/Electric-Trucks-Have-Moved-From-Impossible-to-Inevitable.html) ⭐️ 7.0/10

国际清洁交通委员会（ICCT）数据显示，2025 年全球零排放中重型卡车及客车销量同比增长 86%、超过 52 万辆，其中中国占近 90%；欧洲零排放卡车在新车销量中的占比也从约 2.5%升至 4.5%。文章认为，这表明电动卡车已从“技术上不可能”进入商业规模化。

rss · OilPrice.com · 9月3日 19:00

**「背景」** 此前，电动重卡的主要质疑是电池太重、充电太慢，难以胜任长距离运输；报道援引国际能源署（IEA）称，电池价格下降和磷酸铁锂电池技术改善后，中国电动卡车已在部分应用场景与柴油车实现总拥有成本持平，欧洲预计要到 2030 年前后才广泛达到这一水平。

**「影响」** 对考虑购买电动卡车的物流企业来说，主要制约已从车辆本身转向充电设施和电网接入；欧洲目前只有 1000 多个卡车专用充电点，远低于大规模推广所需，审批和建设周期可能限制电动卡车的普及速度。

**标签**: `#electric trucks`, `#zero-emission vehicles`, `#China EV market`, `#battery technology`, `#hydrogen fuel cells`

---

<a id="item-finance-news-11"></a>
### [高油价推动中国加速减少石油消费](https://oilprice.com/Latest-Energy-News/World-News/High-Oil-Prices-Speed-Up-Chinas-Shift-Away-From-Crude.html) ⭐️ 7.0/10

据能源与清洁空气研究中心（CREA）分析，2026 年第二季度中国石油消费量同比下降 9%，同期碳排放量下降约 1%；高油价正在加速电动汽车、电动卡车、铁路及工业设备对燃油的替代，这是中国首次主要由石油消费下降带动的季度减排。

rss · OilPrice.com · 9月3日 17:30

**「背景」** 伊朗战争干扰了波斯湾供应和霍尔木兹海峡通行后，油价走高；中国为减少对高价原油的依赖，削减进口并更多动用库存，同时电动车辆持续替代汽油和柴油消费。

**「影响」** 中国是全球最大原油进口国，其石油需求下滑不仅降低自身排放，也会通过减少进口影响依赖对华出口的石油生产国和全球油市需求格局。

**标签**: `#China oil demand`, `#electric vehicles`, `#oil prices`, `#energy transition`, `#emissions`

---

<a id="item-finance-news-12"></a>
### [巴西国会通过法案，授权政府干预矿业并购](https://oilprice.com/Metals/Commodities/Brazil-Hands-Government-Control-Over-Mining-Deals.html) ⭐️ 7.0/10

巴西国会通过一项法案，授权政府审查并可能阻止外国收购矿业公司及长期矿产供应合同，同时设立 20 亿雷亚尔（约 3.93 亿美元）担保基金，并在五年内提供约 50 亿雷亚尔（约 9.8 亿美元）税收抵免，鼓励企业在巴西境内加工矿产。该法案已送交总统卢拉签署。

rss · OilPrice.com · 9月3日 17:00

**「背景」** 巴西拥有全球第二大稀土储量，但几乎没有矿石精炼或磁铁生产能力；法案中设立的总统府下属审查委员会，是政府拒绝左翼议员国有化提议后的折中安排。

**「影响」** 巴西矿业协会首席执行官警告，新规赋予行政部门过多自由裁量权，可能吓跑外国投资者；而巴西目前仍主要依靠中国完成稀土加工。

**标签**: `#Brazil`, `#mining policy`, `#rare earths`, `#foreign investment`, `#regulation`

---

<a id="item-finance-news-13"></a>
### [马查多支持美国参与委内瑞拉石油合作，但质疑协议授权](https://oilprice.com/Latest-Energy-News/World-News/Machado-Backs-US-Oil-Partnership-but-Questions-Venezuela-Deal.html) ⭐️ 7.0/10

委内瑞拉反对派领导人玛丽亚·科里纳·马查多表示支持美国长期参与开发本国石油储备，但质疑代总统德尔西·罗德里格斯所宣布协议的签署权与条款。该协议拟覆盖约 650 亿桶原油，期限 25 年、涉及 17 个油田，产量目标为日产 150 万桶；委内瑞拉目前日产量约 125 万桶。

rss · OilPrice.com · 9月3日 16:30

**「背景」** 这份协议由美国政府与加拉加斯方面上周宣布，但完整合同尚未公开。委内瑞拉虽拥有全球最大已探明原油储量，但多年投资不足使管道、电力和生产设施状况不佳；埃克森美孚和康菲石油仍持有 2007 年国有化相关的数十亿美元索赔，因此新投资方在一长串债权人中的清偿顺序成为关键问题。

**「影响」** 对于考虑投入数十亿美元的外国石油企业，核心风险在于合同能否在政府更迭后继续有效，以及它们相对既有债务和索赔的受偿位置。

**标签**: `#Venezuela`, `#oil`, `#U.S.-Venezuela relations`, `#energy policy`, `#oil reserves`

---