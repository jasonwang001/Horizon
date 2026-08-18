---
layout: default
title: "Horizon Summary: 2026-08-19 (ZH)"
date: 2026-08-19
lang: zh
---

> 从 244 条内容中筛选出 24 条重要资讯。

---

**科技新闻**
1. [Mojo 编程语言正式开源，采用 Apache 2 许可](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B 以 52 分追平 GPT-5.6 Luna 基准](#item-tech-news-2) ⭐️ 8.0/10
3. [Turbovec：Rust 实现的 Google TurboQuant 向量搜索](#item-tech-news-3) ⭐️ 7.0/10
4. [用 20 美元工具修复被 BIOS 更新变砖的 Framework 笔记本](#item-tech-news-4) ⭐️ 7.0/10
5. [Linux 7.3 优化显存超量分配性能](#item-tech-news-5) ⭐️ 7.0/10
6. [数据中心废热实测：下风侧街区平均升温约 0.8°C](#item-tech-news-6) ⭐️ 7.0/10
7. [相机版 AirPods 传闻，macOS Tahoe 演示视觉智能](#item-tech-news-7) ⭐️ 7.0/10
8. [macOS 26.7 代码揭示中国大陆 Apple 智能审查机制](#item-tech-news-8) ⭐️ 7.0/10
9. [中国要求部分政府机构提前卸载定制版 Windows 10](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [海湾石油绕行霍尔木兹海峡，运费创纪录](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储维持利率不变 投票结果为 9 比 3](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储维持利率不变，鲍威尔举行记者会](#item-finance-news-3) ⭐️ 9.0/10
4. [债券市场抛售推高美债收益率，美国家庭承压](#item-finance-news-4) ⭐️ 8.0/10
5. [霍尔木兹海峡“影子”石油运输网络每日转运逾 400 万桶](#item-finance-news-5) ⭐️ 8.0/10
6. [沙特阿美恢复经霍尔木兹海峡装运 VLCC 原油](#item-finance-news-6) ⭐️ 8.0/10
7. [多瑙河低水位迫使罗马尼亚核电站停运，燃煤电厂重启](#item-finance-news-7) ⭐️ 8.0/10
8. [“先买后付”贷款覆盖水电和房租，2025 年美国借贷额达 1600 亿美元](#item-finance-news-8) ⭐️ 8.0/10
9. [美联储利率决定与关税动态主导繁忙经济周](#item-finance-news-9) ⭐️ 8.0/10
10. [美联储或将迎来多年来最难预测的会议](#item-finance-news-10) ⭐️ 8.0/10
11. [盘后多只个股因财报与指引大幅波动](#item-finance-news-11) ⭐️ 7.0/10
12. [珍妮·巴斯反对兄弟姐妹出售湖人股份](#item-finance-news-12) ⭐️ 7.0/10
13. [美国企业将在伊拉克建设首个液化天然气进口终端](#item-finance-news-13) ⭐️ 7.0/10
14. [苹果美国 App Store 佣金收入下降 18%，二季度用户消费额同比降 6%](#item-finance-news-14) ⭐️ 7.0/10
15. [TrendForce：2026 年中国本土 AI 芯片市占率或达 90%](#item-finance-news-15) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Mojo 编程语言正式开源，采用 Apache 2 许可](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Mojo 编程语言现已正式开源，Modular 公司按照 Apache 2 许可证发布了编译器与工具链，兑现了自 2023 年 5 月以来的承诺。此前一周，Mojo 刚刚发布了 1.0 版本。Mojo 最初计划成为 Python 的超集，但 2025 年 8 月左右调整了愿景，表示可能不会完全兼容 Python。如今 Mojo 已发展为一门独立的语言，专注于让 GPU 编程尽可能简单，使用受 Python 启发的语法。

rss · Simon Willison · 8月18日 21:39

**「背景」** Mojo 是由 Modular 推出的面向 AI 和高性能计算的语言，设计目标是通过类 Python 语法简化 GPU 等加速器的编程。2023 年其团队承诺将开源，但路线图经历了调整，放弃了必须成为 Python 完整超集的目标。

**「影响」** 开发者和组织现在可以自由查看、修改和分发 Mojo 的编译器与工具链，并可在商业项目中基于 Apache 2 许可使用，降低了对闭源工具的依赖。

**标签**: `#mojo`, `#open-source`, `#programming-language`, `#ai`, `#modular`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B 以 52 分追平 GPT-5.6 Luna 基准](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，与 GPT-5.6 Luna（最高配置）得分相同，仅比 GLM-5.2（最高配置）和 DeepSeek V4 Pro 0813（最高配置）低 1 分。根据引用的模型页面，GLM-5.2 为 753B 参数，DeepSeek V4 Pro 0813 为 1.7T 参数，而 Luna 的参数量未知，但很可能远大于 27B。Simon Willison 于 2026 年 8 月 17 日报道了这一消息，并在前一天撰文称该模型“真正令人惊叹”。一个 27B 参数模型达到与超大前沿模型相近的基准分数，被视为 AI 模型效率上的显著突破。

rss · Simon Willison · 8月17日 23:58

**「背景」** Artificial Analysis Intelligence Index 是 Artificial Analysis 发布的模型智能评测指标，用于横向比较不同大语言模型的综合能力。Qwen 3.8 27B 是一款开源模型，支持文本和图像输入、文本输出，上下文窗口为 256k tokens。该指数将 27B 参数的小模型与 GPT-5.6 Luna、GLM-5.2、DeepSeek V4 Pro 等超大模型放在同一把尺子上衡量，因此其 52 分成绩被视为效率上的显著突破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B Intelligence, Performance &amp; Price Analysis</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLMs`, `#Qwen`, `#benchmark`, `#model-efficiency`

---

<a id="item-tech-news-3"></a>
### [Turbovec：Rust 实现的 Google TurboQuant 向量搜索](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec 是一个用 Rust 实现 Google TurboQuant 向量搜索技术的开源库，项目托管在 GitHub，主打紧凑的内存占用和实用的检索效率。根据项目介绍，它可以用约 4GB 内存处理 1000 万文档的索引，这对本地/隐私优先搜索、AI 基础设施以及调试和性能测试等开发场景很有吸引力。社区讨论已延伸到 SQLite 绑定、WASM 编译运行在浏览器扩展等方向，同时也有评论提醒，Qdrant 等既有方案已经在集成 TurboQuant，因此 Turbovec 的相对优势仍需结合基准测试和实际使用情况验证。

hackernews · fittingopposite · 8月18日 18:07 · [社区讨论](https://news.ycombinator.com/item?id=49349898)

**「背景」** TurboQuant 是 2025 年由 Google Research 等机构提出的在线向量量化方法，旨在以极低的比特率实现接近最优的失真率，并宣称在显著压缩模型大小的同时保持零准确率损失，因此被用于大语言模型推理中的 KV 缓存压缩、向量数据库和最近邻搜索等场景。Turbovec 是该项目对 TurboQuant 的 Rust 实现，利用该方法的特性（无需学习数据集特定的码本）来执行量化；针对真实世界嵌入不完美的情况，它还引入了 TQ+ 校准机制。

**「影响」** Rust 开发者与本地搜索用户可以用约 4GB 内存构建 1000 万文档的向量索引，从而以更低的资源成本开展本地/隐私优先搜索，并可能加快索引重建、调试和性能测试流程；实际效果仍需与已集成 TurboQuant 的 Qdrant 等方案对比确认。

**「社区讨论」** 评论者普遍对 4GB/1000 万文档的内存表现感到兴奋，期待 SQLite 绑定，并询问将 Rust 实现编译为 WASM 以在浏览器扩展中运行的可能性；也有人建议 README 写得更有人情味，同时指出 Qdrant 已集成 TurboQuant 数月，质疑为何不直接使用成熟方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TurboQuant">TurboQuant - Wikipedia</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google’s TurboQuant Makes Vector Search Smaller, Faster, and Simpler | by Mehul Gupta | Data Science in Your Pocket | Medium</a></li>

</ul>
</details>

**标签**: `#vector-search`, `#rust`, `#quantization`, `#ai-infrastructure`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [用 20 美元工具修复被 BIOS 更新变砖的 Framework 笔记本](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 7.0/10

一位开发者记录了自己用约 20 美元工具，修复一台因 BIOS 更新失败而变砖的 Framework 13（AMD 7040 系列）笔记本电脑的过程。该指南展示了在缺少官方刷写连接器的情况下，借助低成本硬件完成固件恢复的具体做法。这一案例引发了关于官方固件更新导致设备损坏时的责任归属、保修政策以及维修权问题的讨论。社区评论指出，BIOS 更新导致变砖的情况仍然常见，并有人呼吁制造商承担更多法律责任。

hackernews · jp\_sc · 8月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49345220)

**「背景信息」** Framework 13 英寸 AMD 7040 系列笔记本电脑在通过官方 BIOS 更新（如从 3.05 升级到 3.07）时，可能因更新失败而“变砖”，导致无法开机。这类问题通常需要硬件级刷写 SPI 闪存芯片才能恢复，但 Framework 官方并未提供简易的 BIOS 刷写接口，用户往往只能更换主板。该作者使用约 20 美元的简易工具（如 pogo pin 等）自行恢复了电脑，而社区中也有其他用户分享过类似成功的恢复案例。

**「影响」** 对于遭遇同类固件变砖的 Framework 用户，这篇指南提供了一条约 20 美元工具即可尝试的恢复路径；但 Framework 未提供官方刷写接口意味着普通用户仍可能面临较高的维修门槛。

**「社区讨论」** 评论中多数人认同作者对厂商责任的批评：有人主张应将此类问题诉诸小额法庭，也有人以 ThinkPad Nano 的经历说明 BIOS 更新变砖仍常见且厂商往往不关心。另有评论指出 Framework 曾提供调试器 JSPI 方案，只是连接器未预装以节省成本；还有人表示因此后悔购买 Framework 笔记本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/">Fixing a bricked AMD 7040 series Framework 13” laptop with $20 tools | Quantum</a></li>
<li><a href="https://community.frame.work/t/success-in-recovering-from-bad-bios-upgrade-framework-13-amd-7040/66598">Success in recovering from bad BIOS upgrade - Framework 13 AMD 7040 - Community Support - Framework Community</a></li>
<li><a href="https://resources.frame.work/downloads/laptop-13/amd-ryzen-7040-series/">Framework Laptop 13 AMD Ryzen™ 7040 Series — BIOS &amp; Drivers | Resources</a></li>

</ul>
</details>

**标签**: `#hardware repair`, `#BIOS update`, `#Framework laptop`, `#embedded systems`, `#electronics repair`

---

<a id="item-tech-news-5"></a>
### [Linux 7.3 优化显存超量分配性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 7.0/10

Linux 内核 7.3 版本带来一项旨在改进显存（VRAM）超量分配处理的变更，目标是在 GPU 显存耗尽时减少性能问题。这项改进针对 GPU 工作负载的真实性能瓶颈，具有技术细节，并被视为对 Linux 系统和开源软件工程的及时且有价值的进展。文章分析认为，该改动能够缓解显存不足时的性能下降，但未提供具体的基准测试数据或实现细节。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**「背景」** VRAM 超量使用（VRAM overcommit）指的是应用程序请求的 GPU 显存超过物理可用容量，导致性能严重下降。Linux 内核此前的显存管理方式在这方面处理不够理想。Valve Linux 图形团队的 Natalie Vock 提出了相关补丁，旨在改善游戏等负载在有限显存下的显存管理，这些补丁已被合并并计划进入 Linux 7.3 内核。

**「影响」** Linux 7.3 的 VRAM 超额分配改进主要惠及 AMD GPU 且显存有限、会频繁超出显存容量的用户，Natalie Vock 的补丁集此前已大幅提升了低显存 AMD GPU 的性能；这些改进能否生效取决于驱动是否支持显存分页/换出，因此并非所有 GPU 都能同等受益。

**「社区讨论」** 评论区整体持积极态度：有人称赞文章并期待改动上游化，也有人（尤其是 Nvidia 用户）指出当前驱动仍缺少显存分页能力，并希望系统在系统内存耗尽时也能避免卡死。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://www.osnews.com/story/145846/beyond-the-limits-of-physical-vram/">Beyond the limits of physical VRAM – OSnews</a></li>

</ul>
</details>

**标签**: `#linux`, `#kernel`, `#vram`, `#performance`, `#gpu`

---

<a id="item-tech-news-6"></a>
### [数据中心废热实测：下风侧街区平均升温约 0.8°C](https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban) ⭐️ 7.0/10

一项发表在 ASME《可持续建筑》期刊的实地测量研究，以美国凤凰城某数据中心园区为对象，量化了数据中心废热对街区尺度气温的影响。测量显示，设施上风侧平均气温约为 42.7°C，而下风侧园区东侧邻近街区升至约 43.5°C，平均增温约 0.8°C，影响范围约向下风方向延伸 500 米。该研究为数据中心废热作为新兴城市热源提供了经验证据，表明其局部热效应真实存在，但平均幅度相对有限。这一结果将此前多停留在估算层面的数据中心热岛影响转化为可实测的数据，同时也在社区讨论中引发对是否夸大风险的争议。

hackernews · cwwc · 8月18日 17:24 · [社区讨论](https://news.ycombinator.com/item?id=49349147)

**「背景」** 数据中心消耗大量电力，因而会排放大量废热，但其对周边居民区气温的直接影响此前长期缺乏实地测量。这项研究据称首次提供运营中的数据中心使相邻居民区空气温度出现可测量升高的现场证据。在美国数据中心容量预计到 2030 年翻倍以上的背景下，研究者将数据中心废热定性为先前未获记录的都市热害，并呼吁数据中心和城市规则界予以重视。

**「影响」** 这一实测数据使数据中心废热对周边社区的局部热影响从估算变为可量化证据，可能影响数据中心选址、社区环境评估和“邻近升温”类争议的讨论方式；但 0.8°C 的平均增温也提示不宜将此简单等同于更大范围或更严重的气候影响。

**「社区讨论」** Hacker News 评论中，有用户质疑数据中心“热恐慌”是否被人为放大，认为数据中心相对地球规模很小；也有用户引用测量数据指出平均温差远小于标题暗示，同时感叹相关讨论充满极端化、情绪化甚至疑似不实账号的言论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban">Data Center Waste Heat as an Emerging Urban Thermal Hazard ...</a></li>
<li><a href="https://asu.elsevierpure.com/en/publications/data-center-waste-heat-as-an-emerging-urban-thermal-hazard-first-/">Data Center Waste Heat as an Emerging Urban Thermal Hazard ...</a></li>

</ul>
</details>

**标签**: `#data centers`, `#waste heat`, `#urban heat island`, `#environmental impact`, `#field measurements`

---

<a id="item-tech-news-7"></a>
### [相机版 AirPods 传闻，macOS Tahoe 演示视觉智能](https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/) ⭐️ 7.0/10

苹果正开发配备摄像头的 AirPods，产品代号为 B790。macOS Tahoe 26.7 RC 中的演示显示，摄像头可识别书名并通过视觉智能保存信息，Siri 能回答佩戴者周边问题并记录信息。Mark Gurman 称该产品最快可能于 9 月发布。目前为未经证实的传闻，具体技术规格和兼容性尚未公布。

telegram · zaihuapd · 8月18日 02:00

**「背景」** 苹果的相机版 AirPods（内部代号 B790）此前只是传闻，但 MacRumors 在 macOS Tahoe 26.7 候选版本的代码和演示视频中发现了相关证据。视频显示 AirPods 内置摄像头可识别图书封面等物体，并与苹果的视觉智能（Visual Intelligence）和 Siri 联动，回答佩戴者周围环境的问题并保存信息。这款设备尚未正式发布，外界预期它可能在 9 月与 iPhone 18 Pro 一同亮相，不过苹果未予确认。

**「影响」** 若消息属实，这款产品将把视觉智能带到耳机形态的可穿戴设备上，可能影响苹果生态系统内的 AI 交互方式，但发布计划仍存在不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techspot.com/news/113519-leak-suggests-next-apple-airpods-have-cameras-visual.html">Leaked video shows Apple&#x27;s camera-equipped AirPods ... - TechSpot</a></li>
<li><a href="https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/">Apple&#x27;s Camera-Equipped AirPods Confirmed: See Them in Action</a></li>
<li><a href="https://techgenyz.com/apple-camera-equipped-airpods-leak/">Apple Camera-Equipped AirPods Just Leaked: 5 Details Revealed</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AirPods`, `#Visual Intelligence`, `#AI Hardware`, `#macOS`

---

<a id="item-tech-news-8"></a>
### [macOS 26.7 代码揭示中国大陆 Apple 智能审查机制](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

据 MacRumors 报道，macOS 26.7 等代码显示 Apple 智能的“写作工具”将登陆中国大陆，并配有独立的内容安全过滤、拦截和处罚机制。代码中出现多条面向用户的提示：需先完成内容安全更新才能使用工具；对无法编辑的文本会提示可发送给指定 App 处理；多次触发安全警报后“写作工具”将暂时受限。相关安全审查规则可通过云端远程下发，意味着系统可在本地或服务端动态调整限制策略。该发现有助于了解 Apple 如何在区域法规下部署 AI 编辑功能。

telegram · zaihuapd · 8月18日 02:16

**「背景」** Apple Intelligence 是苹果于 2024 年 WWDC 公布的 AI 功能集合，结合设备端与服务器端处理，写作工具是其一项功能。macOS Tahoe 26.7 的代码显示，写作工具将在中国大陆推出，并包含因多次触发安全警报而暂时限制、以及系统提示部分内容无法使用 Apple 智能编辑等机制。相关安全审查规则可经由云端远程下发，这与苹果为符合中国大陆地区监管要求所做的调整有关。

**「影响」** 开发者若在中国大陆版系统中集成或调用“写作工具”，需要处理安全更新未完成、文本无法编辑以及多次警报后工具受限等状态，并向用户提供相应提示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>
<li><a href="https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/">macOS Tahoe 26.7 is Full of References to Unreleased Apple Products - MacRumors</a></li>
<li><a href="https://www.gadgets360.com/laptops/news/apple-macos-tahoe-26-7-code-new-product-codenames-report-11924169">Apple’s macOS Tahoe 26.7 Reportedly Includes References to iPhone 18, New Macs and More | Technology News</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI censorship`, `#China`, `#macOS`, `#content moderation`

---

<a id="item-tech-news-9"></a>
### [中国要求部分政府机构提前卸载定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

中国国家安全部已要求部分政府相关机构卸载定制版 Windows 10，使原定 2027 年 2 月的停用计划提前数月。知情人士称，这一指令源于数据安全担忧，但未说明具体漏洞。微软回应称，未发现影响该产品的安全事件，该产品仍定期获得安全更新。此举反映中国对政府系统软件供应链的安全审查趋严，对微软在华政府市场及定制系统部署构成影响。

telegram · zaihuapd · 8月18日 06:22

**「背景」** 中国为政府机构定制的 Windows 10 版本（通常称为政府版）此前计划在 2027 年 2 月停用，而微软通用的 Windows 10 主流支持已于 2024 年 10 月 14 日结束。此次中国国家安全部要求部分政府相关机构提前卸载该定制版，主要源于数据安全担忧，同时中国正推动采用国产操作系统替代。

**「影响」** 提前停用将使微软政府版 Windows 相关收入归零，但由于微软整体业绩更依赖 Azure 云与 AI 商业化，财务影响相对可控；同时该指令已推动国产操作系统概念股大涨（麒麟信安、Archermind 触及 20% 涨停，中国软件涨 10%），加速国产替代进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/china-state-agencies-uninstall-windows-10-cmit-government-edition/">China’s State-Linked Firms Are Moving Away From Windows 10 ...</a></li>
<li><a href="https://tech.yahoo.com/computing/articles/china-finally-pulling-windows-10-112000903.html">China is finally pulling Windows 10 from government machines ...</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its ...</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262114664-win10-government-removal-microsoft-china-headwinds-tradingkey">Win10 Government Edition Phased Out Early as Microsoft&#x27;s China Business Faces New Headwinds</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>

</ul>
</details>

**标签**: `#Windows 10`, `#China`, `#government`, `#data security`, `#Microsoft`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [海湾石油绕行霍尔木兹海峡，运费创纪录](https://oilprice.com/Energy/Crude-Oil/How-Gulf-Oil-Is-Escaping-the-Strait-of-Hormuz.html) ⭐️ 9.0/10

海湾产油国正通过船对船转运绕开霍尔木兹海峡，中东至中国航线的超大型油轮（VLCC）评估日收益已超过 50 万美元，单程包船成本达 3100 万美元，而布伦特原油价格约为每桶 91 美元。

rss · OilPrice.com · 8月18日 15:00

**「背景」** 霍尔木兹海峡是全球最重要石油咽喉，因美伊紧张和 60 天休战备忘录到期，大型油轮通行几近停滞；沙特阿美等油企转向在阿联酋富查伊拉港外进行船对船转运，以继续向亚洲买家交付船货。

**「影响」** 绕过海峡的运输成本大幅上升，可能推高亚洲炼油商的进口成本，并加剧全球石油供应紧张。

**标签**: `#crude-oil`, `#strait-of-hormuz`, `#shipping-rates`, `#geopolitics`, `#oil-prices`

---

<a id="item-finance-news-2"></a>
### [美联储维持利率不变 投票结果为 9 比 3](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

美联储在 9 比 3 的投票中决定维持利率不变，其中 9 名官员赞成，3 名官员反对。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储是美国的中央银行，其利率决定会影响整体借贷成本。此次它以 9 票赞成、3 票反对维持基准利率不变，意味着多数官员同意暂不调整利率；报道显示，三名持反对意见的官员希望加息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-leaves-interest-rate-unchanged-180102302.html">Federal Reserve leaves interest rate unchanged in 9 - 3 vote , but...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-3"></a>
### [美联储维持利率不变，鲍威尔举行记者会](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 9.0/10

美联储将利率维持不变，主席鲍威尔随后举行新闻发布会，说明最新政策决定。

google\_news · PBS · 3月18日 07:00

**「背景」** 美联储在连续三次降息后决定维持利率不变，尽管特朗普总统多次要求降息，且委员会内部存在分歧。

**「影响」** 美联储将联邦基金利率维持在 3.50%–3.75%不变，并暂停了此前连续三次降息的步伐，这意味着依赖浮动利率贷款的家庭和企业将继续承担当前的借贷成本，而通胀不确定性也使未来降息的时点更加不明朗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thehindu.com/news/international/us-federal-reserve-leaves-interest-rates-unchanged-even-as-trump-demands-cuts/article69875802.ece">FOMC keeps interest rates unchanged despite... - The Hindu</a></li>
<li><a href="https://au.finance.yahoo.com/news/federal-reserve-leaves-interest-rates-unchanged-after-three-straight-cuts-as-two-officials-vote-against-decision-140019034.html">Federal Reserve leaves interest rates unchanged after three straight...</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>
<li><a href="https://www.tiktok.com/discover/the-latest-federal-reserve-meeting">The Latest Federal Reserve Meeting | TikTok</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Powell`, `#FOMC`

---

<a id="item-finance-news-4"></a>
### [债券市场抛售推高美债收益率，美国家庭承压](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 8.0/10

债券市场近期抛售推高长期美债收益率：10 年期收益率已超过 4.7%，并带动 30 年期房贷利率升至 6.75%、柴油价格同比上涨 48%，挤压美国家庭；市场正关注新任美联储主席沃什的下一步表态。

rss · CNBC Finance · 8月18日 16:48

**「背景」** 背景是长期收益率受美国财政赤字、伊朗战争和科技公司 AI 投资带来的发债需求等共同因素推高；2 年期与 10 年期国债利差自 6 月 24 日以来扩大近 29 个基点，反映市场对长期增长和通胀的预期变得不明朗。

**「影响」** 受影响最大的是房贷借款人和依赖柴油运输的家庭与企业，融资和能源成本上升；而近年股市上涨的财富收益主要落在最富有的美国人群体。

**标签**: `#bond market`, `#Treasury yields`, `#monetary policy`, `#consumer impact`, `#fiscal policy`

---

<a id="item-finance-news-5"></a>
### [霍尔木兹海峡“影子”石油运输网络每日转运逾 400 万桶](https://oilprice.com/Energy/Crude-Oil/A-4-Million-Bpd-Shadow-Oil-Highway-Is-Running-Through-Hormuz.html) ⭐️ 8.0/10

在伊朗战争持续之际，一个经霍尔木兹海峡的影子石油运输网络正以每日超过 400 万桶的规模运转，以绕过基本关闭的商业航道。据彭博社报道，约 150 艘油轮集结在阿曼附近，通过关闭应答器的穿梭船将货物转运到海峡外的大型油轮上，而战前该海峡每日通行近 2000 万桶。

rss · OilPrice.com · 8月18日 19:00

**「背景」** 这一网络自 5 月初在美国军方监督下成形，并在沙特东-西管道及红海航线受到胡塞武装袭击后进一步扩大。

**「影响」** 该机制暂时缓解了全球油市对供应短缺的担忧，但伊拉克、科威特和卡塔尔的出口仍高度依赖霍尔木兹海峡。

**标签**: `#oil supply`, `#Strait of Hormuz`, `#tankers`, `#geopolitics`, `#energy markets`

---

<a id="item-finance-news-6"></a>
### [沙特阿美恢复经霍尔木兹海峡装运 VLCC 原油](https://oilprice.com/Latest-Energy-News/World-News/Aramco-Puts-VLCCs-Back-Into-Hormuz-After-Three-Week-Pause.html) ⭐️ 8.0/10

沙特阿美已恢复从霍尔木兹海峡内的拉斯坦努拉和朱阿马码头装载 VLCC 原油；据 Kpler 和 Vortexa 数据，8 月 12 日至 16 日已有 3 艘 VLCC 各装载约 200 万桶，预计本月晚些时候还有 6 艘 VLCC 可能装载。

rss · OilPrice.com · 8月18日 18:18

**「背景」** 此前在美国与伊朗冲突升级期间，阿美的油轮遭袭，公司暂停从海峡内发货约三周，并尝试经富查伊拉船对船转运或红海延布等替代路线，但延布受到胡塞武装封锁，替代路线成本更高。

**「影响」** 对亚洲炼油厂而言，恢复直航可减少绕行，但出口尚未恢复常态；阿美仍通过富查伊拉转运、埃及 Sidi Kerir 发货，预期本月经该终端向亚洲装载约 67 万桶/日，远低于此前经延布的约 400 万桶/日。

**标签**: `#Oil Markets`, `#Saudi Aramco`, `#Strait of Hormuz`, `#Shipping`, `#Geopolitics`

---

<a id="item-finance-news-7"></a>
### [多瑙河低水位迫使罗马尼亚核电站停运，燃煤电厂重启](https://oilprice.com/Latest-Energy-News/World-News/Romania-Restarts-Coal-Plant-as-Danube-Drought-Forces-Nuclear-Shutdown.html) ⭐️ 8.0/10

为部分弥补多瑙河低水位导致的切尔纳沃德核电站两座反应堆停运，罗马尼亚本周重启了罗维纳里 4 号燃煤机组，新增近 300 兆瓦发电能力。罗马尼亚能源部国务秘书称，核电站停运使该国损失约 20%的发电量。

rss · OilPrice.com · 8月18日 14:30

**「背景」** 切尔纳沃德核电站两座反应堆各拥有 680 兆瓦装机容量，通常提供罗马尼亚约 20%的电力；由于今夏高温干旱使多瑙河水位降至 90 年来最低，冷却水不足导致反应堆自 7 月底以来陆续关停。低水位同样影响匈牙利保克什核电站，匈方通过向河中下沉驳船维持其运行。

**标签**: `#energy security`, `#nuclear power`, `#drought`, `#coal power`, `#Romania`

---

<a id="item-finance-news-8"></a>
### [“先买后付”贷款覆盖水电和房租，2025 年美国借贷额达 1600 亿美元](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 8.0/10

U.S. buy-now-pay-later borrowing hit $160 billion in 2025, nearly doubling since 2023, as lenders expand into essential bills like rent and utilities, raising debt-trap concerns.

telegram · zaihuapd · 8月18日 01:41

**标签**: `#consumer credit`, `#buy now pay later`, `#household debt`, `#financial regulation`, `#US economy`

---

<a id="item-finance-news-9"></a>
### [美联储利率决定与关税动态主导繁忙经济周](https://news.google.com/rss/articles/CBMixAFBVV95cUxQY3BZcHU3LV9UTzlXZUxGb2FuM0hyQ25FaE55bHVEbG1LZFV1ZS1HejlvbEhjcU51NDdXVlJPZGIwRzdLa1dhNG9ZT3BVZXNVUVlqcm9lbmI0Q192ZHJKX3UteGd5Rmk0cTZaT1daS0I4NlFCZW1xbmU1bS1oZV9JenB0WVkwT3N2Ym1rRmRjbjFfZVRGaWhzeEVSZlg0SThxdW5oMkpRbFdnNVRnWlVwQ25EZUtoOTNxOVBYMnZITHJhTmF1?oc=5) ⭐️ 8.0/10

据美国新闻媒体报道，本周美国经济日程密集，焦点包括美联储的利率决定、关税进展以及伊朗相关的“暂停”事态。

google\_news · usnews.com · 7月27日 07:00

**「背景」** 本周的美联储利率决定将是新任主席凯文·沃什的首次会议，他曾表示致力于降低通胀；同时，美国最高法院近期裁定特朗普政府的关税政策大部分无效；此外，伊朗“暂停”成为市场关注的进展。

**「影响」** 新一轮关税可能提高进口商品成本，给依赖进口的企业和消费者带来压力；美联储的利率决定则会影响借贷成本，投资者将关注其政策信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.usnews.com/news/national-news/articles/2026-07-27/fed-rate-decision-tariffs-iran-pause-make-for-busy-economic-week">Fed Rate Decision , Tariffs , Iran ‘ Pause ’ Make for Busy Economic ...</a></li>
<li><a href="https://www.semafor.com/article/02/24/2026/us-tariffs-decision-wont-heavily-impact-clean-tech-firms">US tariffs decision won’t heavily impact clean tech firms | Semafor</a></li>
<li><a href="https://www.usnews.com/news/national-news/articles/2026-07-27/fed-rate-decision-tariffs-iran-pause-make-for-busy-economic-week">Fed Rate Decision, Tariffs, Iran ‘Pause’ Make for Busy ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#tariffs`, `#Iran`, `#economic calendar`

---

<a id="item-finance-news-10"></a>
### [美联储或将迎来多年来最难预测的会议](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 8.0/10

据《华尔街日报》报道，美联储下一次会议预计将是多年来最难以预测的会议之一，政策走向存在高度不确定性。

google\_news · WSJ · 7月23日 07:00

**「背景」** 此前，美联储在 2026 年 7 月 29 日结束的一次会议上维持基准利率不变，但有三名官员投了反对票。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnn.com/2026/07/29/business/live-news/federal-reserve-interest-rate-07-29-26">Fed holds interest rates steady after cliffhanger meeting, but three officials dissent | CNN Business</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Monetary Policy`, `#Interest Rates`, `#Central Bank`, `#Economy`

---

<a id="item-finance-news-11"></a>
### [盘后多只个股因财报与指引大幅波动](https://www.cnbc.com/2026/08/18/stocks-making-the-biggest-moves-after-hours-tol-keys-lzb.html) ⭐️ 7.0/10

业绩指引分化引发盘后股价异动：La-Z-Boy 因当前季度收入指引（5 亿至 5.2 亿美元）远低于分析师共识（5.368 亿美元）而暴跌 17%，Keysight Technologies 因第三财季经调整每股收益 3.07 美元超过预期的 2.48 美元而上涨 2%。其他公司中，Toll Brothers 第四季交付量指引基本符合预期、股价微跌 0.3%，Mercury Systems 因财年收入指引高于预期但每股盈利不及预期而跌逾 10%，Jack Henry &amp; Associates 因盈利超预期上涨 3%。

rss · CNBC Finance · 8月18日 20:55

**「背景」** 这些波动发生在 8 月 18 日美股收盘后，企业发布季度财报和未来指引后，投资者在盘后交易时段重新定价，相关影响通常会延续到下一个交易日开盘。

**标签**: `#earnings`, `#after-hours`, `#guidance`, `#stocks`, `#company results`

---

<a id="item-finance-news-12"></a>
### [珍妮·巴斯反对兄弟姐妹出售湖人股份](https://www.cnbc.com/2026/08/17/jeanie-buss-opposes-sale-family-stake.html) ⭐️ 7.0/10

洛杉矶湖人队控股老板珍妮·巴斯反对兄弟姐妹将家族所持球队股份出售给鲍勃·伊格尔和乔舒亚·库什纳，称根据法院命令，未经她同意任何出售投票都“无效”；争议涉及家族信托持有的 17.8%球队股份。

rss · CNBC Finance · 8月18日 21:29

**「背景」** 珍妮·巴斯的五个兄弟姐妹此前发表声明，称已决定出售家族剩余股份；上周伊格尔和库什纳同意收购马克·沃尔特的多数股权，该交易对球队的估值为 125 亿美元。

**标签**: `#Los Angeles Lakers`, `#Buss family`, `#NBA`, `#ownership dispute`, `#mergers and acquisitions`

---

<a id="item-finance-news-13"></a>
### [美国企业将在伊拉克建设首个液化天然气进口终端](https://oilprice.com/Energy/Natural-Gas/The-US-Is-Quietly-Building-a-New-Energy-Foothold-in-Iraq.html) ⭐️ 7.0/10

美国企业 Excelerate Energy 将开发伊拉克首个液化天然气（LNG）进口终端，该公司宣布项目预计于 2027 年第二季度投运。项目初步预算为 4.5 亿美元，设计日处理能力为 5 亿立方英尺，伊拉克承诺每日最低采购 2.5 亿立方英尺。

rss · OilPrice.com · 8月18日 23:00

**「背景」** 项目位于 Khor Al Zubair 港，Excelerate 将同时作为主要 LNG 供应商；报道称，伊拉克政府收入超过 90%来自石油和天然气，美方希望借此削弱伊朗和中国对伊拉克的影响力。

**「影响」** 项目投运后，伊拉克将首次拥有 LNG 进口能力，为其电力部门提供新的天然气供应来源。

**标签**: `#LNG`, `#Iraq`, `#energy infrastructure`, `#Excelerate Energy`, `#U.S. energy policy`

---

<a id="item-finance-news-14"></a>
### [苹果美国 App Store 佣金收入下降 18%，二季度用户消费额同比降 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

第三方数据（Appfigures、Sensor Tower）显示，受监管变化影响，苹果美国 App Store 佣金收入自 2026 年初下降 18%，第二季度用户消费额同比下降 6%，而去年同期为增长 9%；苹果表示监管变化已拖累服务业务增长。

telegram · zaihuapd · 8月18日 12:17

**「背景」** App Store 佣金收入是苹果对应用内数字商品或服务销售抽取的分成；数据显示，自 2026 年初以来，由于美国、巴西和日本等地实施新规，苹果在美国的这项收入下降了 18%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/">Apple&#x27;s US App Store Commission Revenue Down 18% This Year - MacRumors</a></li>
<li><a href="https://appleinsider.com/articles/26/08/18/apples-app-store-revenue-in-danger-of-being-regulated-away">Apple&#x27;s App Store revenue in danger of being regulated away</a></li>

</ul>
</details>

**标签**: `#Apple`, `#App Store`, `#Regulatory Impact`, `#Services Revenue`, `#Antitrust`

---

<a id="item-finance-news-15"></a>
### [TrendForce：2026 年中国本土 AI 芯片市占率或达 90%](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 7.0/10

市场研究机构 TrendForce 预计，2026 年中国本土 AI 加速器占国内市场的份额将从 2025 年的约 45% 升至近 90%，寒武纪与华为被视为最大赢家。

telegram · zaihuapd · 8月18日 13:03

**「背景」** 据同一份 TrendForce 数据，2025 年英伟达出货 220 万颗、市占 55%，华为出货 81.2 万颗、市占 20.3%。TrendForce 称，中国需要一年内把高端 AI 芯片产量提高约 2.2 倍至 196 万颗，产能能否跟上仍存疑。

**标签**: `#AI accelerators`, `#China`, `#semiconductor`, `#Huawei`, `#market forecast`

---