---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 225 条内容中筛选出 24 条重要资讯。

---

**科技新闻**
1. [DRAM 攻击可在部分 AMD 芯片上获取 ring-0 权限](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI 与 Cerebras 推出 GPT-5.6 Sol Ultrafast：7 倍加速推理](#item-tech-news-2) ⭐️ 8.0/10
3. [DeepSeek 开源 Harness 开发者预览版：AI 智能体可观测框架](#item-tech-news-3) ⭐️ 8.0/10
4. [选择无聊技术：创新令牌与务实技术选型](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepSeek V4 Pro 0813 发布：1.7T 参数开放权重上线](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepMind SL2T 手语转文字模型落地 Pixel 11](#item-tech-news-6) ⭐️ 8.0/10
7. [Google 推出 Gemini 3.7 Flash，社区争论定价与性能](#item-tech-news-7) ⭐️ 7.0/10
8. [Gloomberb：类彭博的开源终端金融仪表盘](#item-tech-news-8) ⭐️ 7.0/10
9. [City2Graph：将城市地理空间数据转化为异构图的 Python 库](#item-tech-news-9) ⭐️ 7.0/10
10. [worldproof：诊断世界模型预测失效并测量像素指标失去排序能力的区间](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [霍尔木兹海峡僵局加大油价飙升至 120 美元的风险](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储以 9 比 3 投票维持利率不变](#item-finance-news-2) ⭐️ 9.0/10
3. [英国央行发布 2026 年 7 月《货币政策报告》](#item-finance-news-3) ⭐️ 9.0/10
4. [标普 500 净利润率创历史新高，持续支撑股市上涨](#item-finance-news-4) ⭐️ 8.0/10
5. [长江存储在 NAND 芯片出货量升至全球第三](#item-finance-news-5) ⭐️ 8.0/10
6. [太阳能发电量首次超过风电：2025 年全球可再生能源占电力 33.4%](#item-finance-news-6) ⭐️ 8.0/10
7. [美国为 X-energy 与 Dow 的先进核反应堆项目提供最高 21.5 亿美元支持](#item-finance-news-7) ⭐️ 8.0/10
8. [俄罗斯柴油出口降至多年低点，全球燃料市场趋紧](#item-finance-news-8) ⭐️ 8.0/10
9. [IEA：本季度全球石油供应缺口将达每日 180 万桶](#item-finance-news-9) ⭐️ 8.0/10
10. [乌克兰袭击俄萨拉瓦特炼油厂，俄燃料出口受抑](#item-finance-news-10) ⭐️ 8.0/10
11. [长鑫存储市值超越腾讯，成为中国市值最高公司](#item-finance-news-11) ⭐️ 8.0/10
12. [Aboitiz Equity Ventures 第二季度净利润增长 65%](#item-finance-news-12) ⭐️ 8.0/10
13. [通胀降温推动美股上涨，Workday 大涨 18%](#item-finance-news-13) ⭐️ 8.0/10
14. [中国经济放缓挤压就业 零工岗位增至超 5300 万仍供过于求](#item-finance-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DRAM 攻击可在部分 AMD 芯片上获取 ring-0 权限](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

GitHub 上发布的“Spaghettifying DRAM”展示了一种利用 DRAM 操纵在特定 AMD 处理器上实现 ring-0 特权提升的新技术，研究者为 Christopher Domas。该攻击针对内存寻址与内存控制器寄存器机制，属于硬件层面的安全绕过。根据 README，AMD Jaguar（约 2013 年的 AMD16h 低功耗家族）可被利用，而 Zen 3 的控制器基地址不同，因此攻击在其他新架构上的适用范围尚不清楚。相关工作预计将在 Black Hat 大会上进行讲解。

hackernews · matt\_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**「背景」** 该研究针对 AMD 处理器内存控制器中的 DRAM 地址加扰机制。现代 DRAM 控制器会对物理地址进行加扰或翻译，以分散访问模式；这项名为 skitter-creek-bath-salts 的概念验证工具通过篡改这些地址翻译寄存器，可重新映射物理地址并绕过硬件安全边界，从而获得 ring-0 权限。项目由安全研究员 Christopher Domas 发布，主要验证平台为 AMD Jaguar 等较老的 AMD16h 架构。

**「影响」** 对于使用 AMD Jaguar 等受影响旧平台的用户，攻击者可借助 DRAM 访问获得 CPU 最高特权级，从而控制整个系统；由于目前确认范围限于较老的 AMD16h 家族，新 CPU 用户受影响程度尚不明确。

**「社区讨论」** 评论者普遍期待 Christopher Domas 在 Black Hat 的演讲，并推荐他过去关于逆向工程、混淆和硬件后门的 talks；也有评论指出 DRAM 复杂度增加导致攻击面扩大，同时质疑该攻击是否适用于 Zen 3 等更新处理器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/amd-hardware-vulnerability-exposed-by-dram-address-scrambling-research">AMD DRAM Scrambling Exploit Bypasses Security Fences | Linxi News</a></li>

</ul>
</details>

**标签**: `#hardware security`, `#DRAM`, `#privilege escalation`, `#AMD`, `#exploit`

---

<a id="item-tech-news-2"></a>
### [OpenAI 与 Cerebras 推出 GPT-5.6 Sol Ultrafast：7 倍加速推理](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

OpenAI 与 Cerebras 宣布推出 GPT-5.6 Sol Ultrafast，宣称在不损失准确率的情况下将推理速度提升约 7 倍。据评估，Ultrafast 模式用 11 小时 11 分钟完成全部 2500 道 HLE 问题，而 Claude Fable 5 需要 78 小时 27 分钟，二者达到相近准确率。社区评论指出，Cerebras 与 OpenAI 并未明确表示该模式与普通版 GPT-5.6 Sol 在性能上完全一致，也未公布定价，因此“只是更快”的说法尚待证实。另有第三方数据称，按 Artificial Analysis 报告的输出速度，Ultrafast 比 Fable 5 快 11 倍，比 Opus 4.8 Fast 模式快 5 倍。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**「背景」** OpenAI 与 Cerebras 合作推出了名为 Ultrafast 的新服务层级，首先在 OpenAI API 中提供 GPT-5.6 Sol 模型，据称可比标准处理快最高 14 倍，每秒生成最多 750 个输出 token。Cerebras 表示，其硬件为 Ultrafast 模式提供算力，并宣称在加速的同时不牺牲质量。该功能最初仅面向部分客户开放，后续将逐步扩大使用范围。

**「影响」** 若 Ultrafast 真的保持相同质量，它将让前沿模型用户把一个完整推理工作负载压缩到一个工作日以内，并可能显著改变依赖大量迭代推理的 AI 应用成本与响应时间；但目前缺少 OpenAI 对质量等同的明确确认和价格信息，实际影响仍有不确定性。

**「社区讨论」** 社区讨论多肯定速度对思考质量的价值，认为快速迭代与反复修改能显著提升结果质量，但也有评论质疑厂商并未在官方文章中明确声明 Ultrafast 与普通 5.6 Sol 的表现完全相同，并指出缺少定价信息可能意味着价格不菲或厂商仍在试探需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT‑5.6 Sol at up to ... - OpenAI</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI - cerebras.ai</a></li>
<li><a href="https://investors.cerebras.ai/news-releases/news-release-details/cerebras-powers-ultrafast-mode-openais-gpt-56-sol">Cerebras Powers Ultrafast Mode for OpenAI’s GPT-5.6 Sol ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#inference speed`, `#OpenAI`, `#Cerebras`, `#large language models`

---

<a id="item-tech-news-3"></a>
### [DeepSeek 开源 Harness 开发者预览版：AI 智能体可观测框架](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 发布了 Harness 的开发者预览版，基于 MIT 许可证开源，这是一个用于构建和观测 AI 智能体的框架。Harness 实现了完整的会话可追溯性：模型看到的一切（系统提示、推理、工具调用与结果、子智能体调度、上下文注入）都记录在只追加的会话日志中，并可通过轨迹视图按来源检查、恢复、分叉、搜索和重放。该框架采用“一切皆插件”的架构，底层使用 Cordis v4，支持插件的热加载与动态启用/禁用，并能回滚插件产生的状态和副作用。官方明确表示这是早期预览版，存在粗糙之处并可能出现破坏性变更。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**「背景」** AI 智能体的调试与审计一直比较困难，因为模型内部推理和工具调用过程往往难以观察。Harness 试图通过事件流式记录和可视化轨迹来解决这一问题，其插件体系则让开发者无需重启进程即可扩展或调整智能体功能。

**「影响」** 对于构建 AI 智能体的开发者，Harness 提供了一套开源且可完整回溯会话的观测方案，在调试、审计和复现方面可能优于许多将轨迹加密或混淆的商业模型。由于目前只是预览版，API 和功能仍可能大幅变化，生产环境采用需谨慎。

**「社区讨论」** 作者在评论中说明这只是早期预览版，欢迎反馈和建议，并提醒会有破坏性变更。社区中，有的用户认为完整轨迹记录是“杀手级功能”，并指出美国商业模型通常不开放这种透明访问；另一些评论则认为该框架“有用但没那么有用”，并对“一切皆插件”的架构表达了插件疲劳。

**标签**: `#AI`, `#open-source`, `#agent-tooling`, `#observability`, `#DeepSeek`

---

<a id="item-tech-news-4"></a>
### [选择无聊技术：创新令牌与务实技术选型](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

2015 年发表的经典文章《Choose Boring Technology》主张，技术选型应刻意选择无聊、被充分理解的技术，因为每家公司大约只有三个“创新令牌”（innovation tokens），这些有限预算只应花在能带来明显差异化优势的地方。这篇文章因提出“创新令牌”这一可操作框架而成为工程文化讨论中常被引用的作品，也持续影响着后续关于微服务、数据库选型等话题的讨论。它强调稳定、熟悉的技术能降低长期维护和认知成本，而创新应集中在真正让产品与众不同的部分。在当下围绕 AI agent 的工程讨论中，该框架仍被用来建议通过“把创新令牌集中到 agent，底层工具保持无聊”来降低不确定性。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**「背景」** 《选择无聊的技术》是 Dan McKinley 于 2015 年发表的文章，提出了“创新代币”这一概念：每个公司在一段时间内只能承担少量高风险的技术试验，其余部分应使用成熟、可预期、社区经验丰富的“无聊”技术。该文后来成为工程文化中关于技术选型的经典框架，常被用来反对盲目追逐新技术栈。

**「社区讨论」** 评论区高度认可这篇文章，认为“创新令牌”是帮助管理者向各层级同事解释技术取舍的实用概念；也有读者补充例外情况，例如内部已有 Cassandra 专家时，即使它不是最理想方案也可能成为“无聊选择”。另有观点认为，在 AI agent 时代应把创新令牌集中投入到 agent 本身，而让 agent 所依赖的技术栈保持无聊、接近训练分布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Choose Boring Technology - Dan McKinley</a></li>
<li><a href="https://www.laws-of-software.com/laws/choose-boring-technology/">Choose Boring Technology - Laws of Software</a></li>

</ul>
</details>

**标签**: `#boring-technology`, `#engineering-culture`, `#technology-choice`, `#innovation-tokens`, `#software-architecture`

---

<a id="item-tech-news-5"></a>
### [DeepSeek V4 Pro 0813 发布：1.7T 参数开放权重上线](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 已通过 API 在 OpenRouter 上线，更新后的开放权重也已发布到 Hugging Face，参数规模达 1.7T，权重文件约 893GB。截至报道时，DeepSeek 官方没有明显的公告页面，因此 Simon Willison 以 OpenRouter 链接作为入口。评测数据据称先发布在官方微信群，后被复制到 Reddit 但因被认为“低效”而被删除，又以 ASCII 表格形式出现在 Hacker News。作者测试发现，该模型在 low、medium、high 三种推理等级下生成的鹈鹕骑自行车图像风格差异非常明显，这是他此前未在其他模型上观察到的现象。

rss · Simon Willison · 8月12日 23:59

**「背景」** DeepSeek V4 Pro 系列是深度求索的开源权重模型，此前已发布 4 月的 DeepSeek-V4-Pro 和 7 月的 DeepSeek-V4-Flash-0731 权重。这次 0813 版本延续了开放权重做法，但模型体积庞大，1.7T 参数和 893GB 权重意味着本地部署需要多卡环境或进行量化。

**「影响」** 对于希望本地部署或微调的研究者与开发者，该模型需要庞大的硬件资源才能运行，而通过 OpenRouter 可以立即以 API 形式试用。由于官方缺少正式公告，基准测试数据目前仅能在社区转载中看到，评估时需要注意信息来源的非官方性。

**标签**: `#deepseek`, `#llm`, `#open-weights`, `#huggingface`, `#api`

---

<a id="item-tech-news-6"></a>
### [DeepMind SL2T 手语转文字模型落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

谷歌 DeepMind 发布大规模多语言手语转文字模型 SL2T，并首次将其带入消费产品：率先支持美国手语转英语，已在 Pixel 11 的 Gboard 和 Live Transcribe 中上线。该模型使用超过 10 万小时、50 多种手语数据训练，在 FLEURS-ASL 基准上零样本得分为 70 BLEURT，远高于此前纪录。为保护隐私，SL2T 只处理手部与身体姿态关键点，不读取原始视频。后续 DeepMind 计划将 SL2T 扩展到更多设备和语言。

telegram · zaihuapd · 8月13日 08:55

**「背景」** 传统手语识别通常依赖完整视频帧，运算量大且存在隐私顾虑。SL2T 改用仅提取手部与身体姿态关键点的方式，在减少数据处理的同时进行翻译，并借助大规模多语言训练提升对不同手语的泛化能力。

**「影响」** 对使用美国手语的 Pixel 11 用户，SL2T 在 Gboard 和 Live Transcribe 中提供了实时的 ASL 转英语能力，这是手语 AI 首次进入主流消费产品。不过该功能目前仅限特定设备和语言组合，其他用户仍需等待后续扩展。

**标签**: `#DeepMind`, `#sign language AI`, `#accessibility`, `#machine learning`, `#Pixel 11`

---

<a id="item-tech-news-7"></a>
### [Google 推出 Gemini 3.7 Flash，社区争论定价与性能](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google 推出 Gemini 3.7 Flash，这是 Flash 系列的新模型，发布后社区迅速围绕定价、视觉转 HTML 能力和基准表现展开讨论。该模型的限时优惠价预计在 2026 年 12 月 31 日翻倍，2027 年 1 月 1 日起输入/输出价格将分别为每百万 token 1.50 美元和 7.50 美元（评论引述）。开发者 @jjcm 的图片转 HTML 测试显示，Gemini 3.7 Flash 表现出色，但 Anthropic 的 Opus 5 仍是同类最佳；同时多位用户指出，Luna 模型更便宜且在 DeepSWE 1.1 上性能更强，削弱了 Flash 的性价比优势。官方基准更偏向与 Terra 对比，而非 Luna。整体上，新 Flash 模型在低成本高吞吐文本场景中的定位受到质疑，尤其是 3.6 Flash 仅三周前刚发布。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**「背景」** Gemini Flash 系列是 Google 面向低成本、高吞吐量文本任务推出的轻量级模型。此次发布的 Gemini 3.7 Flash 采用限时促销定价：2026 年 12 月 31 日前输入每百万 token 为 0.75 美元、输出每百万 token 为 3.75 美元，自 2027 年 1 月 1 日起恢复为输入 1.50 美元、输出 7.50 美元，这与 Gemini 3.6 Flash 的标准 API 价格一致。社区讨论主要关注其视觉转 HTML 能力、基准测试表现以及与 GPT-5.6 Luna 等竞品的价格和性能对比。

**「影响」** 对于使用 Gemini API 处理视觉转 HTML 或高吞吐文本任务的开发者，Gemini 3.7 Flash 提供了比 Opus 5 更便宜但稍逊的替代选项，同时需要评估 2027 年价格翻倍及与 Luna 相比的成本/性能权衡。

**「社区讨论」** 社区评论呈现共识：Gemini 3.7 Flash 的视觉能力在同类价位中突出，但多数讨论集中于其定价策略和与 Luna/Terra 的竞争关系；有开发者质疑为何选择该模型，并认为 Luna 更便宜、性能更强，还有人认为官方基准应直接与 Luna 对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://venturebeat.com/technology/googles-gemini-3-7-flash-targets-coding-and-agents-with-a-50-introductory-price-cut">Google’s Gemini 3.7 Flash targets coding and agents with a 50% introductory price cut | VentureBeat</a></li>
<li><a href="https://www.techtimes.com/articles/324387/20260813/google-cuts-gemini-37-flash-price-half-it-claims-top-claude-business-workflows.htm">Google Cuts Gemini 3.7 Flash Price in Half as It Claims to Top Claude on Business Workflows</a></li>
<li><a href="https://officechai.com/ai/gemini-3-7-flash-benchmarks/">Google Releases Gemini 3.7 Flash, Competes With GPT 5.6 Terra &amp; Muse Spark 1.2 On Benchmarks</a></li>

</ul>
</details>

**标签**: `#gemini`, `#google`, `#ai-models`, `#machine-learning`, `#release`

---

<a id="item-tech-news-8"></a>
### [Gloomberb：类彭博的开源终端金融仪表盘](https://gloom.sh/) ⭐️ 7.0/10

Gloomberb 是一个开源、类 Bloomberg 的终端金融数据仪表盘，采用平铺式用户界面，目标是提供类似彭博终端的操作体验。该项目在 Hacker News 上引发讨论，主要集中在安装脚本的依赖解析方式、技术栈选择，以及它与彭博真实数据服务的差距。评论者指出彭博每年约 31,980 美元的费用主要买的是数据源，而 Gloomberb 并不具备彭博的连接能力。总体上，它被认为本身有实用价值，适合对 TUI 和金融数据界面感兴趣的开发者尝鲜。

hackernews · rbanffy · 8月13日 13:52 · [社区讨论](https://news.ycombinator.com/item?id=49285982)

**「背景」** Gloomberb 是一款致敬彭博终端（Bloomberg Terminal）的开源终端界面（TUI）金融数据仪表盘。彭博终端是 Bloomberg L.P. 提供的专业软件系统，用于实时金融行情、分析与电子交易，但其数据服务价格高昂且不开放，因此这类克隆项目通常只复刻界面交互，无法获得彭博同等级的数据连接。该项目采用平铺多面板设计，用户可通过键盘快速切换行情、研究等面板，但安装方式采用 curl 脚本、以及依赖解析方式，成为社区讨论的焦点。

**「社区讨论」** 评论中，有用户希望项目明确说明安装脚本背后的技术栈与依赖解析方式，而非默认执行 curl 安装；也有用户肯定平铺界面易用，但困惑如何让新窗格跟随另一窗格联动切换代码。还有评论列举了 Godel Terminal 等闭源竞品，强调彭博的价值在于数据源而非界面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bloomberg_Terminal">Bloomberg Terminal - Wikipedia</a></li>

</ul>
</details>

**标签**: `#terminal`, `#open source`, `#finance`, `#TUI`, `#developer tools`

---

<a id="item-tech-news-9"></a>
### [City2Graph：将城市地理空间数据转化为异构图的 Python 库](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph 是一个新发布的开源 Python 库，用于把城市地理空间数据转换为适合空间分析、网络分析和图神经网络（GeoAI）的异构图。该库支持从 OpenStreetMap 和 Overture Maps 构建建筑、街道和城市肌理的形态图，通过 DuckDB 加载 GTFS 和 GBFS 交通数据并聚合为站点间公交图，还能处理 OD 矩阵、迁移、共享单车和行人流量等加权空间图。它提供 KNN、Delaunay、Gilbert、Waxman 以及皇后/车相邻性等邻近与连通性构建方法，支持异构图和元路径，并可在 GeoDataFrame、NetworkX、rustworkx 与 PyTorch Geometric 的 Data/HeteroData 之间往返转换，同时保留几何和属性信息。相关论文由 Sato、Pietrostefani、Mahabir 和 Arribas-Bel 撰写，发表于《Computers, Environment and Urban Systems》第 130 卷，文章编号 102492。

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · 8月13日 11:59

**「背景信息」** 城市数据通常包含建筑、街道、交通站点等多种实体，以及邻近、连通、通勤等复杂空间关系，传统平铺特征表难以自然表达这些结构。异构图将多种节点类型和多种边类型统一到一个图结构中，能够更完整地刻画城市系统，因此更适合用图神经网络进行建模和空间分析。City2Graph 的目标就是自动完成从原始地理数据到这种异构图的转换。

**「影响」** 对从事 GeoAI、城市计算和空间分析的研究者与开发者而言，City2Graph 提供了一条直接从 OSM/Overture、GTFS/GBFS 等数据源生成 PyTorch Geometric 异构图的现成路径，可显著降低构建城市级图数据管线的成本，并提供了正式论文（CEUS 130 卷，102492）作为研究引用依据。

**标签**: `#graph-neural-networks`, `#geospatial`, `#urban-computing`, `#python-library`, `#GeoAI`

---

<a id="item-tech-news-10"></a>
### [worldproof：诊断世界模型预测失效并测量像素指标失去排序能力的区间](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 7.0/10

Reddit 用户发布了一个开源工具 worldproof（Apache-2.0，pip install worldproof），用于诊断会预测未来帧的世界模型。通过在真实机器人视频上对比 rollout 与真值和物理不变量，作者发现以最后一帧为基线时，SO-101 机械臂 30fps 三摄像头、64 次 rollout、6 步视界上的动态区域 SSIM 为 0.983、PSNR 为 53.9 dB，且误差不随视界增长；在 DROID 15fps 数据上延伸至 48 步后，SSIM 在前 3 步接近满分、第 4 至 24 步单调下降，约 28 步后触底于 0.20 SSIM 和 10.3 dB，因此这段真实 footage 的可用评测窗口约为 8 至 24 步。作者认为两端都会让模型打平，像素指标本身在精选数据上通过排序测试，但评测设置缺乏区分力；另外把 step 0 计入会把 30fps 录制的标量从约 32 dB 拉到 53.9 dB，扭曲结果。工具读取 LeRobotDataset v3.0 的 parquet/mp4，核心依赖 numpy、torch 和 pillow，无需 GPU，支持 Python 3.10；LPIPS 无法分离两个数据集且 masked 变体方向相反，作者称尚无解释。

reddit · r/MachineLearning · /u/georgia\_bucea · 8月13日 19:58

**「背景」** 世界模型（world model）是一类根据初始上下文和动作序列预测未来帧的模型，评测时通常用 SSIM、PSNR、LPIPS 等像素级指标与真实视频对比。帖子中提到的“最后帧复制基线”（copy last frame baseline）假设场景不变，是最朴素的预测；若这类基线在某个时间范围上已经与真实视频高度接近，则更复杂的模型在该范围内几乎没有可区分的提升空间。Agarwal 等人提出的 rliable 工具为这种评测提供分层自助置信区间和四分位均值（IQM）等统计方法，用于避免少量 rollout 带来的误导性比较，帖子的作者说明其 64 次 rollout 和区间统计正是沿用这一方法。

**「影响」** 对使用像素指标评估真实机器人视频世界模型的研究者，默认评测视界可能落在无法区分模型的死区；需要在自己的帧率×任务速度组合上测量可用窗口（该数据中约为 8 至 24 步），并优先报告按步骤的曲线而不是单一标量，否则模型排序可能不可靠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/google-research/rliable">GitHub - google-research/rliable: [NeurIPS&#x27;21 Outstanding ...</a></li>
<li><a href="https://research.google/blog/rliable-towards-reliable-evaluation-reporting-in-reinforcement-learning/">RLiable: Towards Reliable Evaluation &amp; Reporting in ...</a></li>

</ul>
</details>

**标签**: `#world models`, `#evaluation metrics`, `#video prediction`, `#robotics`, `#open source`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [霍尔木兹海峡僵局加大油价飙升至 120 美元的风险](https://oilprice.com/Energy/Oil-Prices/Hormuz-Stalemate-Raises-Risk-of-120-Oil.html) ⭐️ 9.0/10

霍尔木兹海峡局势陷入僵持，航运量处于两个月低位；分析人士称，若供应中断持续，油价可能升至每桶 120 至 140 美元。本周布伦特原油价格一度涨至每桶 89 美元以上。

rss · OilPrice.com · 8月13日 15:00

**「背景」** 自 2 月 28 日战争爆发以来，美伊双方围绕海峡控制权反复威胁，海峡大部分时间接近关闭。此前中国进口低迷、战略储备释放和海上库存缓冲使原油期货未创新高，但炼油利润率已升至大西洋盆地纪录高位。

**「影响」** 若僵局持续至三季度末、四季度初，经合组织国家石油库存可能快速消耗并达到“临界点”，柴油、航空燃油等中间馏分油供应将更紧张，推高全球燃料成本。

**标签**: `#Oil prices`, `#Strait of Hormuz`, `#Geopolitical risk`, `#Supply disruption`, `#Energy markets`

---

<a id="item-finance-news-2"></a>
### [美联储以 9 比 3 投票维持利率不变](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

据 ABC7 洛杉矶报道，美国联邦储备委员会（美联储）在 9 比 3 的投票中决定维持利率不变。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储在 7 月会议上以 9 比 3 的投票结果决定将联邦基金利率目标区间维持在 3.5%—3.75%不变，三名官员投反对票并倾向于加息；相关报道显示，市场普遍预期下次 9 月会议可能加息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/federal-leaves-interest-rate-unchanged-180102302.html">Federal Reserve leaves interest rate unchanged in 9 - 3 vote , but...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pJbTlyVkVSSHUzb3dpdmpXX2dpZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Fed&#x27;s interest rate meeting - Overview</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#economy`

---

<a id="item-finance-news-3"></a>
### [英国央行发布 2026 年 7 月《货币政策报告》](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

英国央行发布 2026 年 7 月《货币政策报告》，阐述其货币政策决定和经济展望。

google\_news · Bank of England · 7月30日 07:00

**「背景」** 英国央行每季度发布《货币政策报告》，其中包含货币政策委员会（MPC，即负责制定利率的委员会）在作出利率决策时所依据的经济分析和通胀预测；本报告是 2026 年 7 月版。

**「影响」** 英国央行将基准利率（Bank Rate，即银行利率）维持在 3.75%，货币政策委员会以 6 比 3 的投票结果决定不加息。由于该利率是许多贷款产品的定价基准，持有与基准利率挂钩的按揭或贷款的英国家庭和企业，近期还款成本不会立即变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/monetary-policy-report">Monetary Policy Reports | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/">Home | Bank of England</a></li>
<li><a href="https://www.forexfactory.com/news/1410968-bank-of-england-holds-uk-interest-rate-steady">Bank of England holds UK interest rate steady at 3.75... | Forex Factory</a></li>

</ul>
</details>

**标签**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#economic outlook`, `#UK`

---

<a id="item-finance-news-4"></a>
### [标普 500 净利润率创历史新高，持续支撑股市上涨](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 8.0/10

标普 500 指数第二季度综合净利润率目前为 16.9%，高于第一季度的 14.8%和去年同期的 12.9%，也高于五年平均值 12.4%；若最终确认，这将是 FactSet 自 2009 年开始跟踪该指标以来的最高纪录，主要由 Alphabet 和亚马逊贡献。

rss · CNBC Finance · 8月13日 20:21

**「背景」** 净利润率是企业扣除所有费用后从收入中保留的利润占比；即便剔除 Alphabet 和亚马逊，标普 500 净利润率仍达 15%，同为历史纪录，且 11 个行业中有 8 个的利润率高于一年前。

**「影响」** 企业盈利能力提升正在为股市上涨提供支撑，但科技行业竞争加剧可能给未来的利润率带来压力。

**标签**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#stock market`, `#FactSet`

---

<a id="item-finance-news-5"></a>
### [长江存储在 NAND 芯片出货量升至全球第三](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 8.0/10

市场研究机构 Counterpoint 数据显示，长江存储（YMTC）今年第二季度在全球 NAND 闪存芯片出货量中升至第三位，市占率约 14%，超过美光和铠侠，仅次于三星和 SK 海力士。

rss · CNBC Finance · 8月13日 02:59

**「背景」** NAND 芯片是断电后仍能保留数据的存储芯片；YMTC 正准备在中国大陆上市，此前专注于 DRAM 的长鑫存储上月刚上市。

**「影响」** 报告同时指出，YMTC 在出货量上领先，但 NAND 收入仍落后于美光和铠侠，主要销售集中于消费应用；数据中心预计到 2026 年底占 NAND 需求的一半，是后续竞争的重要领域。

**标签**: `#NAND memory`, `#semiconductors`, `#YMTC`, `#market share`, `#competition`

---

<a id="item-finance-news-6"></a>
### [太阳能发电量首次超过风电：2025 年全球可再生能源占电力 33.4%](https://oilprice.com/Alternative-Energy/Solar-Energy/Solar-Surpasses-Wind-In-Global-Electricity-Generation-For-The-First-Time.html) ⭐️ 8.0/10

根据能源研究所《世界能源统计评论》，2025 年全球太阳能发电量首次超过风电：太阳能发电达 2,811 太瓦时，占全球电力的 8.7%；风电为 2,714 太瓦时，占 8.4%。可再生能源合计约占全球电力的 33.4%，其中太阳能贡献了当年可再生电力增量的近四分之三。

rss · OilPrice.com · 8月13日 20:00

**「背景」** 数据来自英国能源协会（Energy Institute）发布的《世界能源统计评论》（Statistical Review of World Energy），该报告自 1952 年起发布，过去 70 余年由 bp 编制，2023 年起改由能源协会主办并与 Ember 等机构合作。该评论是能源行业常用的年度全球能源数据来源，本文引用的是 2026 年发布的第 75 版。

**「影响」** 由于 2025 年全球能源需求增量（约 8.1 艾焦耳）仍明显高于可再生能源供应增量（约 3.2 艾焦耳），可再生能源的快速扩张目前主要满足新增需求，尚未直接取代化石燃料消费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.energyinst.org/__data/assets/pdf_file/0004/1822009/Statistical-Review-of-World-Energy-2026-Summary-version.pdf">2026 | th edition Statistical Review of World Energy</a></li>
<li><a href="https://www.energyinst.org/statistical-review">Home | Statistical Review of World Energy</a></li>
<li><a href="https://ember-energy.org/latest-insights/energy-institute-statistical-review-of-world-energy/">Energy Institute Statistical Review of World Energy - Ember</a></li>

</ul>
</details>

**标签**: `#solar energy`, `#wind energy`, `#global electricity`, `#renewable energy`, `#energy transition`

---

<a id="item-finance-news-7"></a>
### [美国为 X-energy 与 Dow 的先进核反应堆项目提供最高 21.5 亿美元支持](https://oilprice.com/Latest-Energy-News/World-News/US-Backs-X-Energy-Reactor-With-Up-to-215-Billion.html) ⭐️ 8.0/10

美国能源部已通知 X-energy，将为该公司与 Dow 在得州 Seadrift 工业厂址的先进核反应堆项目追加最高 10 亿美元联邦资金，使该项目自 2021 年以来可获得的联邦资金总额最高达 21.5 亿美元；资金采用 50/50 成本分摊，项目目标在 2030 年代初投入商业运行。

rss · OilPrice.com · 8月13日 19:30

**「背景」** 该资金来自美国能源部的先进反应堆示范计划（Advanced Reactor Demonstration Program），旨在推动下一代核反应堆走向商业部署；X-energy 与 Dow 已于去年向美国核监管委员会提交建造许可申请。

**「影响」** 若按计划实现，这座反应堆将成为北美首个为工业厂区提供电力和工业蒸汽的并网级先进核反应堆，成为检验联邦成本分摊能否让新技术完成许可、建设并投入商用的案例。

**标签**: `#Nuclear Energy`, `#Government Funding`, `#Energy Policy`, `#X-energy`, `#Dow`

---

<a id="item-finance-news-8"></a>
### [俄罗斯柴油出口降至多年低点，全球燃料市场趋紧](https://oilprice.com/Energy/Energy-General/Russias-Diesel-Exports-Crash-to-Multiyear-Low-amid-Tight-Global-Market.html) ⭐️ 8.0/10

据彭博汇编数据估计，俄罗斯柴油和柴油类产品出口在 8 月 1 日至 7 日降至每日 8 万桶，为多年最低，而去年同期约为每日 100 万桶；原因是乌克兰无人机袭击炼油设施和俄方延长出口限制，全球中间馏分油市场更趋紧张。

rss · OilPrice.com · 8月13日 19:00

**「背景」** 乌克兰近几个月持续用无人机袭击俄炼油设施，迫使多座大型炼厂在春夏停产，俄国内汽油和柴油短缺已持续三个多月；莫斯科因此延长柴油出口限制。

**「影响」** 国际能源署称，7 月全球炼油加工量同比减少近 500 万桶/日，大西洋盆地中间馏分油利润率创纪录新高；全球海运成品油贸易减少 380 万桶/日，显示燃料供应收紧已超过原油市场。

**标签**: `#Russia`, `#diesel exports`, `#Ukraine drone attacks`, `#global oil market`, `#IEA`

---

<a id="item-finance-news-9"></a>
### [IEA：本季度全球石油供应缺口将达每日 180 万桶](https://oilprice.com/Energy/Crude-Oil/Jefferies-Diesel-Cracks-Reveal-the-Real-Oil-Market-Squeeze.html) ⭐️ 8.0/10

国际能源署\(IEA\)最新报告预测，本季度全球石油供应将出现每日 180 万桶的缺口，是此前预测的两倍多；布伦特原油在接近每桶 90 美元后回落至约 87 美元，柴油裂解价差创历史新高，反映市场供应紧张。

rss · OilPrice.com · 8月13日 17:00

**「背景」** 此次预警的背景是美伊谈判停滞、霍尔木兹海峡航运受阻，以及俄乌双方对能源基础设施的袭击，导致柴油等成品油市场吃紧。

**「影响」** 美国银行警告，柴油市场可能持续紧张、波动并保持高价至明年，这将推高运输和制造等依赖柴油的行业成本。

**标签**: `#oil`, `#diesel`, `#geopolitics`, `#IEA`, `#supply`

---

<a id="item-finance-news-10"></a>
### [乌克兰袭击俄萨拉瓦特炼油厂，俄燃料出口受抑](https://oilprice.com/Latest-Energy-News/World-News/Ukraine-Strikes-Gazproms-200000-Bpd-Salavat-Refinery-in-the-Urals.html) ⭐️ 8.0/10

乌克兰周四再次袭击俄罗斯炼油设施，击中俄气（Gazprom）旗下日产 20 万桶的萨拉瓦特炼油厂并引发火灾；由于炼油产能受损，俄罗斯已限制汽油、柴油和航空燃油出口，并开始进口汽油。

rss · OilPrice.com · 8月13日 15:30

**「背景」** 乌克兰近几个月几乎每天打击俄罗斯炼油与出口设施，旨在压缩莫斯科的石油收入；7 月俄罗斯炼油厂开工率约 360 万桶/日，比季节性正常水平低逾 30%。

**「影响」** 这已导致俄罗斯国内汽油短缺，并促使俄罗斯从印度进口汽油；同时还使 7 月俄罗斯海运成品油出口环比下降 33%、同比下降近 55%，进一步收紧全球成品油供应。

**标签**: `#Ukraine conflict`, `#Russian oil`, `#refinery attack`, `#energy markets`, `#fuel exports`

---

<a id="item-finance-news-11"></a>
### [长鑫存储市值超越腾讯，成为中国市值最高公司](https://www.bloomberg.com/news/articles/2026-08-13/cxmt-overtakes-tencent-to-become-most-valuable-chinese-company) ⭐️ 8.0/10

据彭博社报道，长鑫存储（CXMT）周四市值达 5240 亿美元，超越腾讯的 5100 亿美元，成为中国市值最高的公司。

telegram · zaihuapd · 8月13日 10:10

**「背景」** 长鑫存储（CXMT）是一家 2016 年成立、总部位于安徽合肥的 DRAM（动态随机存取存储器）芯片制造商，产品用于手机、电脑、服务器和 AI 系统等。腾讯股价下跌与其加大 AI 投入有关，公司计划 2026 年将 AI 投资至少翻倍至超过 360 亿元人民币，并可能相应减少股票回购。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cxmt.com/en/">ABOUT CXMT - CXMT</a></li>
<li><a href="https://finance.biggo.com/news/67HZBZ0BvbjfYyet0h4T">Tencent Shares Plunge Over 6% Post-Earnings as Doubled AI ...</a></li>

</ul>
</details>

**标签**: `#CXMT`, `#Tencent`, `#market cap`, `#semiconductor`, `#Chinese tech`

---

<a id="item-finance-news-12"></a>
### [Aboitiz Equity Ventures 第二季度净利润增长 65%](https://finance.yahoo.com/markets/stocks/articles/aboitiz-equity-ventures-inc-aboif-010543098.html) ⭐️ 8.0/10

据财报电话会议要点，Aboitiz Equity Ventures 2026 年第二季度净利润跃升 65%。

openbb · PG · 8月13日 01:05

**「背景」** Aboitiz Equity Ventures（AEV）是菲律宾上市控股公司，主要投资于电力、银行与金融服务、食品、基础设施和房地产等领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Aboitiz_Equity_Ventures">Aboitiz Equity Ventures - Wikipedia</a></li>
<li><a href="https://aboitiz.com/about-us">About the Aboitiz Techglomerate</a></li>

</ul>
</details>

**标签**: `#earnings`, `#net income`, `#Aboitiz Equity Ventures`, `#Philippines`, `#earnings call`

---

<a id="item-finance-news-13"></a>
### [通胀降温推动美股上涨，Workday 大涨 18%](https://finance.yahoo.com/markets/stocks/articles/stock-market-today-aug-13-213637440.html) ⭐️ 8.0/10

据市场报道，8 月 13 日美股因通胀数据降温而上扬，其中 Workday 股价大涨 18%。

openbb · GC=F · 8月13日 21:36

**「背景」** 此前公布的批发和消费者通胀数据低于预期，缓解了美联储的加息压力，市场因而预期美联储下月不会加息。

**「市场影响」** 美国 7 月通胀数据强化了投资者对美联储 9 月降息的预期，这一预期变化有助于降低消费者和企业的借贷成本，并推动标普 500 指数当日上涨 1.1%至创纪录收盘点位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fool.com/coverage/stock-market-today/2026/08/13/stock-market-today-aug-13-stocks-rise-as-inflation-cools-workday-soars-18/">Stock Market Today , Aug . 13 : Stocks Rise as Inflation Cools ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-12/stock-market-today-dow-s-p-live-updates">Stock Market Today : Dow, S&amp;P Live Updates for August 13</a></li>
<li><a href="https://www.mpcmarkets.com.au/mpc-morning-call-13th-august-stock-reach-new-record-as-benign-inflation-opens-the-door-for-rate-cuts/">MPC Morning Call 13 th August – Stock reach new... - MPC Markets</a></li>

</ul>
</details>

**标签**: `#inflation`, `#stock market`, `#Federal Reserve`, `#Workday`, `#economic data`

---

<a id="item-finance-news-14"></a>
### [中国经济放缓挤压就业 零工岗位增至超 5300 万仍供过于求](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 7.0/10

中国经济放缓正加剧就业挤压：截至 2025 年，外卖和网约车司机超过 5300 万人，两年增加 1000 万人，但供过于求正推低收入、拉长工时。

telegram · zaihuapd · 8月13日 06:40

**「背景」** 房地产低迷、消费疲弱、建设制造业收缩及自动化，令零工经济成为过剩劳动力出口；深圳今年 6 月已宣布网约车市场饱和。

**「影响」** 受影响的外卖及网约车司机等零工从业者接单等待时间延长、收入承压，例如机场出租车司机在上海浦东、北京大兴和成都天府机场排队等客最长分别达 7 小时、8 小时和 10 小时。

**标签**: `#China economy`, `#employment`, `#gig economy`, `#labor market`, `#ride-hailing`

---