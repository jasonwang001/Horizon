---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 237 条内容中筛选出 27 条重要资讯。

---

**科技新闻**
1. [Qwen 开源 2.4T 参数 MoE 模型 Qwen3.8-2.4T-A95B](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813：低成本代码模型实测](#item-tech-news-2) ⭐️ 8.0/10
3. [Tailscale 定位 16 年历史的 SQLite WAL 重置竞态 bug](#item-tech-news-3) ⭐️ 8.0/10
4. [xAI 发布 Grok 4.6，引发 API 与基准测试讨论](#item-tech-news-4) ⭐️ 8.0/10
5. [高尔斯论 LLM 擅长的数学与测试时扩展](#item-tech-news-5) ⭐️ 8.0/10
6. [损失不感知基，Adam 感知](#item-tech-news-6) ⭐️ 8.0/10
7. [微信发布资源高效的 WeLM 大语言模型家族](#item-tech-news-7) ⭐️ 8.0/10
8. [Zed 推出 Delta：协作与 AI 编辑功能引争议](#item-tech-news-8) ⭐️ 7.0/10
9. [微小 JPEG 在 Chrome 与 Firefox 中的缩放差异解析](#item-tech-news-9) ⭐️ 7.0/10
10. [uBlock Origin 放弃屏蔽 Facebook 广告](#item-tech-news-10) ⭐️ 7.0/10
11. [Grok 4.6 获 61 分：编码性能与定价引关注](#item-tech-news-11) ⭐️ 7.0/10
12. [LTX-2.5 开源视频模型 单张 RTX 5090 可本地运行](#item-tech-news-12) ⭐️ 7.0/10
13. [企业级 SSD 占 NAND 出货 48%，长江存储首进前三](#item-tech-news-13) ⭐️ 7.0/10

**财经新闻**
1. [美联储 9 比 3 投票维持利率不变](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储主席沃什在众议院就通胀与货币政策作证](#item-finance-news-2) ⭐️ 9.0/10
3. [英国央行发布 2026 年 7 月货币政策报告](#item-finance-news-3) ⭐️ 9.0/10
4. [CME 计划推出 AI 算力期货合约，算力有望成为可交易资产类别](#item-finance-news-4) ⭐️ 8.0/10
5. [乌克兰袭击导致俄黑海主要谷物码头停运](#item-finance-news-5) ⭐️ 8.0/10
6. [EIA：到 2027 年底中东仍有约 60 万桶/日原油停产](#item-finance-news-6) ⭐️ 8.0/10
7. [炼油设施遇袭加剧全球柴油供应紧张](#item-finance-news-7) ⭐️ 8.0/10
8. [普京威胁扣押欧盟船只，回应欧盟对俄影子船队制裁](#item-finance-news-8) ⭐️ 8.0/10
9. [乌克兰据报应美方请求暂停攻击油轮和 CPC 管道](#item-finance-news-9) ⭐️ 8.0/10
10. [LME 铝库存降至 1990 年以来最低](#item-finance-news-10) ⭐️ 8.0/10
11. [腾讯第二季度营收超预期，资本开支激增至 528 亿元致自由现金流转负](#item-finance-news-11) ⭐️ 8.0/10
12. [台积电与索尼在日本成立合资企业，开发智能手机图像传感器](#item-finance-news-12) ⭐️ 8.0/10
13. [台积电 7 月营收同比增 45%，股价较历史高点低 13%](#item-finance-news-13) ⭐️ 8.0/10
14. [微软被曝将上调 Windows OEM 授权费 7%至 10%](#item-finance-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen 开源 2.4T 参数 MoE 模型 Qwen3.8-2.4T-A95B](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen 发布了 Qwen3.8-2.4T-A95B，一个总参数量为 2.4T、激活参数为 95B 的混合专家（MoE）模型，首发提供 BF16 与 FP8 权重；原生上下文长度为 262,144 tokens，可扩展至 1,010,000 tokens。社区转述模型卡称其性能介于 Opus 4.8 与 Fable 5 之间，并将其视为 Kimi k3 的竞品。1-bit 量化版本约 397GB，可在消费级硬件上运行，而完整无损 BF16 权重约 4.9TB。开源权重没有 Qwen3.8-Max 的视觉输入、非思考模式和默认 1M 上下文等能力，授权上内部使用或年收入低于 5000 万美元时可免费使用。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**「背景」** Qwen3.8 是 Qwen 团队发布的新一代大模型系列，其中包括总参数量 2.4T、激活参数 95B 的混合专家（MoE）模型 Qwen3.8-2.4T-A95B。该模型已在 Hugging Face 和 ModelScope 上开放权重，官方称其具备视觉与思考能力，原生上下文长度为 256K tokens，最高可扩展至约 1M tokens。

**「影响」** 对本地部署者而言，397GB 的 1-bit 量化版大幅降低了运行门槛，但 BF16 的 4.9TB 需求以及年收入超过 5000 万美元的商用授权限制，仍会让许多团队难以正式采用。

**「社区讨论」** 社区普遍关注量化后在消费级硬件上的可用性，并称赞其性能与体积比；也有评论遗憾开源版缺少视觉输入和默认 1M 上下文，认为与 Qwen3.8-Max 仍有差距。另有用户提到 DeepSeek V4-Pro-0813 的基准分数接近 Fable 5，形成同期竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B">Qwen / Qwen 3 . 8 - 2 . 4 T - A 95 B · Hugging Face</a></li>
<li><a href="https://modelscope.ai/models/Qwen/Qwen3.8-2.4T-A95B">Qwen 3 . 8 - 2 . 4 T - A 95 B</a></li>
<li><a href="https://unsloth.ai/docs/models/qwen3.8">Qwen 3 . 8 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**标签**: `#qwen`, `#llm`, `#mixture-of-experts`, `#model-release`, `#artificial-intelligence`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813：低成本代码模型实测](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 是一个新公布的模型版本，Hacker News 的提交只链接到 OpenRouter 页面而缺乏自身说明，但评论区给出了实测数据。一位用户在 Codex CLI 上对同一新功能分别使用 DeepSeek V4 Pro 0813 与 Grok 4.6：DeepSeek 运行 12 分 02 秒、花费 0.12 美元但存在一个 bug；Grok 4.6 运行 3 分 18 秒、花费 1.41 美元且无 bug。该测试显示 DeepSeek 在单次任务成本上显著更低（约为 Grok 的 1/12），但耗时更长并引入了缺陷。另有评论称 DeepSeek Flash 的上一更新已经能以很低成本完成较重的开发任务，并期待试用这一新版本。整体而言，发布缺乏官方基准链接，社区证据表明它适合成本敏感、可接受后续修复的开发场景。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**「背景」** DeepSeek V4 Pro 0813 是 DeepSeek 于 2026 年 8 月 12 日发布的旗舰 Mixture-of-Experts（MoE）模型，总参数量 1.6T、激活参数 49B，采用混合注意力机制、三种推理模式，并针对长上下文做了优化（上下文窗口 1,048,576 tokens，最大输出 384,000 tokens）。它通过 DeepSeek API 和 OpenRouter 等平台提供，输入价格约为每百万 token 0.435 美元、输出约 0.87 美元。这些背景信息来自 OpenRouter、LM Market Cap 和 Together AI 的产品页面。

**「影响」** 对于在 Codex 等代理式编码工具中控制 token 成本的开发者，单次对比显示 DeepSeek V4 Pro 能把单任务成本从 1.41 美元降到 0.12 美元，但代价是运行时间更长（12 分 02 秒对 3 分 18 秒）并需要额外修复 bug，因此最终是否划算取决于对修复成本的容忍度。

**「社区讨论」** 评论集中在实际操作体验而非论文式基准：有用户分享与 Grok 4.6 的成本、速度与 bug 对比，有用户强调自己更愿意为能低成本完成任务的模型付费，也有人批评该提交直接链向 OpenRouter 信息太少，应改链官方 API 或基准发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://lmmarketcap.com/model/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - Pricing &amp; Benchmarks 2026 | LM Market Cap</a></li>
<li><a href="https://www.together.ai/models/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 API: Pricing, Benchmarks &amp; Docs | Together AI</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#llm`, `#artificial-intelligence`, `#cost-efficiency`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Tailscale 定位 16 年历史的 SQLite WAL 重置竞态 bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 在一篇事后剖析中披露，其数据库损坏问题源于 SQLite 中一个已存在 16 年的 WAL 重置竞态条件。这种竞态会在多个连接并发操作同一数据库时触发，尽管 Tailscale 控制面采用了 SQLite 推荐的单写者访问模式。团队借助他们资助开发的开源 SQLite VFS shim 快速隔离并定位了竞态，最终解决了数据库损坏问题。该 shim 作为开源工具也可用于未来查找类似 bug，而整个调查过程展现了底层数据库缺陷如何在看似合理的使用方式下仍然显现。Tailscale 还强调了他们对 SQLite 项目的支持，包括签订支持合同并公开分享技术细节。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**「背景」** SQLite 是一种广泛使用的嵌入式数据库，支持预写日志（WAL）模式以提高并发读写性能。Tailscale 在排查去年数据库损坏和中断时发现，问题源于一个隐藏在 SQLite 中至少 16 年的“WAL-Reset”竞态条件：当 WAL 模式启用、同一数据库文件有多个连接，并且读取与写入同时发生时，该缺陷可能被触发。SQLite 开发团队承认该 bug 极其罕见，甚至需要添加专门代码才能刻意触发它。

**「影响」** 对于使用 SQLite WAL 模式的开发者和依赖 Tailscale 服务的用户，这一事后剖析表明即使在单写者设计中也可能遇到隐藏的 WAL 重置竞态，并提供了新的开源 VFS shim 用于诊断和复现此类问题。

**「社区讨论」** 评论普遍称赞文章质量高、故事引人入胜，并认可 Tailscale 资助开源调试工具的做法。有读者最初对单写者设计下为何发生数据竞争感到困惑，直到看到多连接并发细节后才理解；也有人引用 Dijkstra 名言，指出测试只能证明 bug 的存在而无法证明其不存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.theregister.com/databases/2026/08/12/tailscale-says-deeply-buried-16-year-old-sqlite-bug-caused-last-years-outages/5287004">Tailscale says deeply buried 16-year-old SQLite bug caused last year&#x27;s outages</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#database`, `#bug-fix`, `#postmortem`, `#tailscale`

---

<a id="item-tech-news-4"></a>
### [xAI 发布 Grok 4.6，引发 API 与基准测试讨论](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 发布了新版 AI 模型 Grok 4.6，引发开发者社区对其 API 行为、基准测试可信度以及行业竞争格局的讨论。有评论指出，Grok API 会为所有请求添加默认系统提示词，其中关于不提及其存在的规定可能覆盖用户自定义系统提示词，导致模型经常拒绝讨论系统提示词。也有评论质疑，多个主要实验室在 Fable 发布后两个月内都推出水平相近的模型，可能源于人才流动、蒸馏或基准测试作弊，但训练和发布模型通常不应如此之快。另一些评论认为 Grok 4.6 在多数基准测试上超过 GPT-5.6-Sol，API 价格低于 Kimi K3，且在 Cursor 订阅中用量慷慨，因此具有竞争力。部分用户还表示，相比 GPT-5.6 Sol 和 Claude 4.8/5，Grok 4.5 使用体验更简洁直接，更符合智能体应有的表现。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**「背景」** xAI 是埃隆·马斯克创立的人工智能公司，其 Grok 系列模型既面向 X / X Premium+ 用户，也通过 API 和 SuperGrok 等渠道提供给开发者。据 xAI 官方发布，Grok 4.6 被描述为 xAI 的 2 万亿参数前沿模型，宣称在多个智能体编程和知识工作基准上达到前沿水平，并在 Artificial Analysis Intelligence Index 上匹配 GPT-5.6 Sol。第三方资料仍提示该模型可能尚未正式开放，预计通过 xAI API、Grok 应用、SuperGrok 和 X Premium+ 提供；API 定价为每百万输入 token 2 美元、每百万输出 token 6 美元，支持约 50 万 token 的上下文窗口。

**「影响」** 对于依赖 Grok API 的开发者，默认系统提示词可能干扰自定义系统提示词的执行，并导致模型拒绝回应涉及系统提示词的问题，影响需要精细控制提示词的集成场景。

**「社区讨论」** 社区对 Grok 4.6 的反应存在分歧：有人视其为健康的竞争，称赞其价格、性能和简洁体验；也有人对其基准测试真实性及各大实验室快速跟进的现象表示怀疑，猜测可能存在蒸馏或评分操纵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>
<li><a href="https://kie.ai/blog/what-is-grok-4-6">What Is Grok 4 . 6 ? xAI &#x27;s 2T-Param Model Explained</a></li>
<li><a href="https://openrouter.ai/x-ai/grok-4.6">Grok 4 . 6 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#machine-learning`, `#LLM`, `#xAI`, `#technology-industry`

---

<a id="item-tech-news-5"></a>
### [高尔斯论 LLM 擅长的数学与测试时扩展](https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/) ⭐️ 8.0/10

菲尔兹奖得主蒂莫西·高尔斯在博客中分析了大语言模型擅长哪些数学任务，并围绕测试时扩展、AI 辅助证明的本质展开讨论。社区评论进一步指出，测试时扩展如今多指让模型长时间自言自语，但更早的 AlphaCode 通过生成数百万候选程序并筛选，在 2022 年击败普通人类程序员，说明采样才是 AI 真正的强项。高尔斯认为，若 LLM 能提出事后看来优美自然、难以偶然发现的新颖证明方法，才标志着其在更广泛数学问题上达到人类水平。目前讨论仍聚焦于 AI 在寻找反例、解决明确问题方面的优势，以及对并发、时序逻辑等领域的未知表现。

hackernews · ColinWright · 8月12日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49270022)

**「背景」** 蒂莫西·高尔斯（Timothy Gowers）是菲尔兹奖得主、剑桥大学数学家，长期在博客和公开讲座中分析人工智能（尤其是大语言模型）在数学上的实际能力。他这篇 2026 年 8 月的文章结合近期若干 AI 数学成果指出，LLM 在处理某些数学任务上表现惊人，但在整体上尚未全面超越人类数学家。背景中常提到的“测试时扩展”（test-time scaling）指在推理阶段让模型进行更多采样或自我对话来提升表现；评论者认为高尔斯讨论的现象本质上与这一趋势有关，而早期如 Google AlphaCode 通过大规模采样生成并筛选候选程序，已在 2022 年超越普通人类程序员。

**「社区讨论」** 评论者普遍认为，这实际上是关于测试时扩展的争论：LLM 的优势来自大规模采样，例如 AlphaCode 2022 年即通过生成数百万程序击败平均人类程序员；但也有人指出，当前成就多集中在寻找反例和解决明确问题，对并发代码或时序逻辑等领域的表现仍是未知数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/">What sort of maths are LLMs good at? | Gowers&#x27;s Weblog</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#mathematics`, `#AI research`, `#test-time scaling`, `#theorem proving`

---

<a id="item-tech-news-6"></a>
### [损失不感知基，Adam 感知](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

一项新研究指出，Adam 这类按坐标自适应的优化器会破坏因子分解模型中的隐式低秩偏差，因为尽管损失函数在 \(U,V\) 旋转下不变，Adam 的第二动量却依赖具体基。作者在欠定矩阵感知上用九种更新规则做匹配训练损失的对比，得到两个清晰的聚类：GD、共享标量 Adam、Muon 和 Shampoo 保留偏差，而 Adam、RMSProp、Lion、signum 和 Adafactor 丢失偏差。通过一个单参数族把 Adam 的分母从逐坐标变成单一共享标量，恢复误差沿该方向单调改善，证实损伤来源是各向异性而不是自适应性本身。Muon 的行为出乎意料：对真正低秩目标精确，但在谱尾能量接近 4% 时与 GD 交叉并更快退化，同一个轴上同时出现近期文献中互相矛盾的两种结论。作者强调，超光谱数据上 43–44% 的留出误差下降使用训练集学习率规则，而该规则恰好给 Adam 最差的学习率；若各方法自选最佳超参数，差距显著缩小，且理论分析目前只覆盖无记忆规则，动量部分是经验结果。论文见 arXiv:2608.05136，代码见 GitHub。

reddit · r/MachineLearning · /u/EtherealGlyph · 8月12日 16:39

**「背景」** 在分解模型 W = UV^T 中，损失函数对因子间的正交旋转保持不变，梯度下降尊重这一不变性，而 Adam 的逐坐标二阶矩依赖于坐标基，因此破坏旋转不变性——这正是其是否保留隐式低秩偏好的关键。Muon 可被理解为无累积版本的一类近似 Shampoo 优化器，这类方法通常也保留低秩偏好，但论文进一步显示其行为会随目标谱尾的存在而变化。

**「影响」** 对于使用分解模型或低秩矩阵感知的优化研究者，这项发现意味着每坐标自适应优化器（如 Adam、RMSProp）会破坏隐式低秩偏置，而保持旋转等变的优化器（如共享标量 Adam、Muon、Shampoo）能保留该偏置，因此在实际建模中应谨慎选择优化器。在超光谱数据集上，以匹配训练损失比较时，梯度下降在最低采样密度下可将测试误差降低 43%–44%，但这一差距依赖特定学习率选择规则，作者也强调机制才是核心主张，具体数字需谨慎解读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>
<li><a href="https://arxiv.org/html/2608.05136">The Loss Does Not See the Basis, but Adam Does</a></li>
<li><a href="https://arxiv.org/abs/2608.05136">[2608.05136] The Loss Does Not See the Basis , but Adam Does</a></li>
<li><a href="https://deeplearn.org/arxiv/802261/the-loss-does-not-see-the-basis,-but-adam-does">The Loss Does Not See the Basis , but Adam Does - Paper Detail</a></li>

</ul>
</details>

**标签**: `#optimizers`, `#implicit-bias`, `#low-rank`, `#Adam`, `#machine-learning`

---

<a id="item-tech-news-7"></a>
### [微信发布资源高效的 WeLM 大语言模型家族](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 8.0/10

微信团队发布了大语言模型家族 WeLM，以资源效率为核心，推动 AI 在微信生态中规模化落地。该家族包括已应用于微信内 AI 智能体“小微”的 WeLM-80B（仅 3B 激活参数），支持对话、搜索、操作微信原生功能及调用小程序服务；以及研发中的 WeLM-617B（23B 激活参数），采用混合专家（MoE）架构，在中等激活规模下实现更强的通用理解与推理能力，未来将用于小程序智能开发和“微信小微”小工具生成等复杂任务。这是腾讯微信在数十亿用户场景中部署大模型的罕见实践。

telegram · zaihuapd · 8月12日 13:58

**「背景」** WeLM 是腾讯微信团队研发的通用大语言模型系列，核心特色是追求资源效率，旨在推动 AI 能力在微信海量用户场景中规模化落地。该系列包括 WeLM-80B（总参数 800 亿，激活参数 30 亿）和研发中的 WeLM-617B（总参数 6170 亿，激活参数 230 亿），后者采用混合专家（MoE）架构。此前微信团队已在 7 月的一篇论文中提及这两个模型；WeLM-80B 在主要训练阶段使用 11T token 预训练，并额外用 1.4T 高质量 token 进行退火。

**「影响」** 微信内现有及未来的 AI 智能体（如“小微”）和依赖小程序服务的用户将直接受益于更低成本、更强能力的交互与自动化功能；对开发者而言，后续小程序智能开发工具可能降低构建复杂 AI 应用的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.weex.com/news/detail/wechat-launches-welm-large-model-series-to-drive-ai-application-implementation-c0pmz8w994lglikkdnsi3ndr">WeChat Launches WeLM Large Model Series to... | WEEX Crypto News</a></li>
<li><a href="https://en.theblockbeats.news/flash/361266">WeChat Introduces WeLM Dual Model : 80 B Model Empowering Mini...</a></li>
<li><a href="https://welm.weixin.qq.com/en/posts/building-effective-sparse-moe-models-with-moderate-resources/">Building Effective Sparse MoE Models with Moderate... | WeLM Blog</a></li>

</ul>
</details>

**标签**: `#WeLM`, `#large language models`, `#mixture-of-experts`, `#resource efficiency`, `#WeChat AI`

---

<a id="item-tech-news-8"></a>
### [Zed 推出 Delta：协作与 AI 编辑功能引争议](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed 发布 Delta，为编辑器加入协作式与 AI 辅助编辑能力，并因实际用途引发社区讨论。根据社区评论，Delta 的关键特性可能包括实时协作的多人对话，以及“对话即文档”的交互方式，也就是允许用户在 AI agent 对话中直接内联评论。这项更新可被视为主流编辑器把多人协作和 AI 代码摘要进一步整合的一次尝试；不过，开发者对其价值看法不一，也有用户抱怨页面文字对比度过低、影响阅读。

hackernews · khy · 8月12日 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**「背景」** Zed 是一款由 Atom 和 Tree-sitter 创建者打造的高性能多人代码编辑器，以快速和协作编辑为特色。Delta 是 Zed 团队在现有编辑器基础上推出的全新应用形态，后续计划加入 DeltaDB，并强调延续 Zed 对性能与工艺的追求。该公告主要涉及实时协作对话以及将对话作为文档等 AI 辅助编辑能力。

**「影响」** 对使用 Zed 的开发者与团队而言，Delta 可能把 AI 对话变成可审查、可协作的工作流，尤其有助于指导初级工程师或追溯 AI 生成结果的过程；但社区反馈显示，许多人仍认为多人同屏编码和 AI 代码摘要的实际价值有限。

**「社区讨论」** 评论对 Delta 的反应明显两极分化：有人称赞 Zed 速度快、内置 AI 不错，却认为多人在同一编辑器里协作没有实际用途；另一些人则看重其在指导初级工程师和检查 AI 生成 PR 上的潜力。此外，有开发者反感 AI 代码摘要的冗长和遗漏边界情况，还有人批评博客页面低对比度设计影响阅读体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-delta">Introducing Delta — Zed &#x27;s Blog</a></li>
<li><a href="https://github.com/zed-industries/zed">GitHub - zed -industries/ zed : Code at the speed of thought – Zed is...</a></li>

</ul>
</details>

**标签**: `#Zed`, `#collaborative-editing`, `#AI-code-assist`, `#software-engineering`, `#editor`

---

<a id="item-tech-news-9"></a>
### [微小 JPEG 在 Chrome 与 Firefox 中的缩放差异解析](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 7.0/10

这篇技术文章解释了 Chrome 与 Firefox 渲染微小 JPEG 时效果不同的原因：两者采用不同的降采样算法，且 Chrome 近期的优化进一步改变了小尺寸图片的解码与缩放行为。对开发者而言，该差异可能导致图标等小图在 Electron 应用或网页中显示模糊或出现振铃伪影。文章指出 JPEG 适合照片而非图标，建议避免将大幅图片缩小显示，或通过 CSS image-rendering 控制缩放算法。Firefox 正在通过 Bugzilla 2033250 推进在解码阶段直接低分辨率还原的工作。

hackernews · gutechh · 8月12日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=49272549)

**「背景」** 浏览器通常将大图解码为完整位图后再缩放到显示尺寸，缩放算法（如双线性、Lanczos）决定了边缘锐利度与振铃伪影。Chrome 与 Firefox 对同一缩放任务的算法选择不同，因此在微小尺寸下差异更明显。JPEG 的有损压缩还会引入色度抽样等伪影，进一步影响小图显示。

**「影响」** 受影响的开发者可能需要推迟 Electron 升级或为小图标准备匹配分辨率、改用 PNG，并利用 image-rendering 属性来缓解跨浏览器差异。

**「社区讨论」** 评论者注意到 PNG 也存在类似问题，并普遍认同应使用适当分辨率的图片而非大图缩小；有人提到 Firefox 的算法更锐利但略有振铃，且不同浏览器在高 DPI 下选择缩放算法的行为不同。

**标签**: `#web development`, `#browser rendering`, `#image scaling`, `#JPEG`, `#Chrome`

---

<a id="item-tech-news-10"></a>
### [uBlock Origin 放弃屏蔽 Facebook 广告](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 7.0/10

uBlock Origin 已停止专门过滤 Facebook 广告，原因是 Facebook 持续变更代码，使广告拦截变成一场难以取胜的猫鼠游戏。这一决定由 Neowin 报道，并伴随 r/uBlockOrigin 社区的讨论。uBlock Origin 是广泛使用的开源广告拦截扩展，此举标志着广告拦截与平台反制之间对抗的一个重要节点。文中未提供具体版本号、日期或后续替代方案，但确认该扩展不再追逐 Facebook 广告。

hackernews · Markoff · 8月12日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**「背景」** uBlock Origin 是一款流行的开源浏览器扩展，通过维护过滤规则列表来拦截网页广告。Facebook 采用代码混淆、动态加载等对抗手段，使广告元素难以被静态规则稳定识别；经过多年的反复拉锯，开发团队在 Reddit 的 r/uBlockOrigin 板块表示不再对 Facebook 广告进行过滤。这一背景也延续了广告屏蔽领域常见的“猫鼠游戏”模式。

**「影响」** 对依赖 uBlock Origin 屏蔽 Facebook 广告的用户，实际影响是 Facebook 信息流中的广告将更可能被看到；若想继续拦截，可能需要借助其他工具或方法。

**「社区讨论」** 社区评论中有人赞同这一决定，认为人们应认清 Facebook 的本质并减少使用；也有人预测这场攻防战最终会走向基于计算机视觉的广告识别方案，还有人认为唯一彻底的办法是离开 Facebook。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.resetera.com/threads/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them.1601830/">Facebook ads are so hard to block that uBlock Origin stopped ...</a></li>

</ul>
</details>

**标签**: `#ad-blocking`, `#uBlock Origin`, `#Facebook`, `#privacy`, `#open source`

---

<a id="item-tech-news-11"></a>
### [Grok 4.6 获 61 分：编码性能与定价引关注](https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis) ⭐️ 7.0/10

Grok 4.6 在 Artificial Analysis Intelligence Index 上获得 61 分，这是该前沿模型新版本的一项关键基准成绩；该发布属于渐进式改进，而非范式转变。社区讨论显示，用户因 Grok 的沟通质量和交互速度将其作为日常编码助手，并提到 Grok Build 比 Claude Code 快 2-5 倍。与此同时，定价变化引发关注：Grok 4.6 的缓存读取价格从 Grok 4.5 的 0.30 美元几乎翻倍至 0.50 美元，在重度编码会话中缓存读取与写入可能占 token 账单的 80%。分析摘要强调该模型对 AI 从业者重要，但只是增量更新。

hackernews · wertyk · 8月12日 16:54 · [社区讨论](https://news.ycombinator.com/item?id=49275385)

**「背景」** Grok 4.6 是 SpaceXAI 新发布的前沿大模型。根据 Artificial Analysis 的评测，Grok 4.6（high）在 Artificial Analysis Intelligence Index 上取得 61 分，该指数是九项基准的综合分数，用于评估推理、知识、数学与编码能力；它在 AA-Briefcase 这类长程智能体知识工作评测中也达到 Fable 5 层级（Elo 1577），落后于 Claude Opus 5 系列。该指数和榜单用于横向比较各前沿模型在综合智能任务中的表现。

**「影响」** 重度编码用户将直接感受到缓存读取定价从 0.30 美元升至 0.50 美元的成本压力；用户报告的更快响应和更清晰的沟通则可能带来交互效率收益。

**「社区讨论」** 评论者普遍认为 Grok 4.5/4.6 在编码场景中速度快、沟通直接，且 Cursor 订阅相比 OpenAI/Anthropic 更具性价比；但对缓存读取价格翻倍和账单占比存在担忧。另有评论认为，若前沿模型如此易达，Gemini 前景看好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis">Grok 4 . 6 returns SpaceXAI to the intelligence frontier and leads on...</a></li>
<li><a href="https://artificialanalysis.ai/models/grok-4-6">Grok 4 . 6 (high) - Intelligence , Performance &amp; Price Analysis</a></li>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#benchmarks`, `#LLM`, `#machine learning`

---

<a id="item-tech-news-12"></a>
### [LTX-2.5 开源视频模型 单张 RTX 5090 可本地运行](https://ltx.io/model/ltx-2-5) ⭐️ 7.0/10

LTX 发布了开源视频生成基础模型 LTX-2.5，权重、训练代码与推理管线全部开放，并支持在单张 RTX 5090 上本地运行。该模型提供文生视频与图生视频能力，改进多镜头连贯性与提示词遵循，采用新的扩散视频解码器和 Gemma 4 12B 文本编码器。年收入低于 1000 万美元的组织可免费商用，这降低了本地部署高质量视频模型的门槛。在 98 个提示词的文生视频瑕疵评测中，厂商称 LTX 2.5 Pro 在十款模型中排名第一，但该结果尚缺独立验证。

telegram · zaihuapd · 8月12日 02:15

**「背景」** LTX-2.5 是 Lightricks 继 2024 年 11 月开源的 20 亿参数 LTX Video 和 2025 年 5 月开源的 130 亿参数 LTXV 之后发布的最新开源视频生成基础模型。该模型采用开放权重模式，支持用户在自己硬件上本地运行、微调甚至部署，并在年收入低于 1000 万美元的条件下可免费商用。与以往模型不同，LTX-2.5 强调多镜头场景的一次性生成、真实视频编辑以及 EXR 格式导出等专业功能。

**「影响」** 具备 RTX 5090 的开发者和小型团队可直接本地部署并免费商用 LTX-2.5，减少对商用视频生成 API 的依赖；但性能排名目前仅来自厂商披露，实际效果仍需独立评测确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ltx.io/model/ltx-2-5">LTX - 2 . 5 : LTX &#x27;s Latest AI Open - Source Foundation Model | LTX</a></li>
<li><a href="https://www.dreampixelforge.com/blog/ltx-2-5">LTX 2 . 5 : Open Weights, Specs, and How to Run It | Dream Pixel Forge</a></li>

</ul>
</details>

**标签**: `#video generation`, `#open source`, `#LTX`, `#AI models`, `#local inference`

---

<a id="item-tech-news-13"></a>
### [企业级 SSD 占 NAND 出货 48%，长江存储首进前三](https://china.counterpointresearch.com/%e6%9c%8d%e5%8a%a1%e5%99%a8%e9%9c%80%e6%b1%82%e6%8e%a8%e5%8d%87%e4%bc%81%e4%b8%9a%e7%ba%a7-ssd-%e5%8d%a0-nand-%e5%87%ba%e8%b4%a7%e9%87%8f%e7%99%be%e5%88%86%e4%b9%8b-48/) ⭐️ 7.0/10

Counterpoint 报告显示，受 AI 推理工作负载推动，2026 年第二季度企业级 SSD 占全球 NAND 出货量的 48%，同比接近翻倍，行业营收较去年同期增长五倍。三星以 25% 份额居首，SK 海力士以 22% 居次，长江存储以 14% 首次超越铠侠进入前三，但因产品偏消费级，其营收仅排第五。报告预计到年底企业级 SSD 将消耗超过一半的 NAND 位元总量。该趋势显示 AI 基础设施建设正持续重塑存储市场需求与供应商格局。

telegram · zaihuapd · 8月12日 11:00

**「背景」** 企业级 SSD 面向服务器和数据中心，强调高耐用性与稳定性能；消费级 SSD 则用于个人电脑等设备。Counterpoint 的数据按出货量份额统计，因此营收排名可能与出货排名不一致，长江存储凭消费级产品出货量大进入前三，但单位收入较低。AI 推理需要大量读取和高并发访问，推动数据中心对企业级存储的需求。

**「影响」** 长江存储进入出货量前三但营收仅第五，说明其仍需提升企业级产品占比与附加值；对依赖 NAND 供应的服务器与 AI 基础设施厂商而言，企业级 SSD 需求接近翻倍意味着供应紧张与成本压力可能延续到 2026 年底。

**标签**: `#NAND`, `#Enterprise SSD`, `#AI workloads`, `#Memory market`, `#YMTC`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储 9 比 3 投票维持利率不变](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

美联储在 9 比 3 的投票中决定维持利率不变，这是新任主席凯文·沃什（Kevin Warsh）主持下的利率决定。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 此前在 6 月会议上，美联储已一致决定将联邦基金利率维持在 3.50%至 3.75%不变；本次 7 月会议是主席凯文·沃什上任后的第二次会议，9 比 3 的投票结果显示内部对是否应尽快加息出现分歧。

**「影响」** 由于美联储将联邦基金利率维持在 3.50%–3.75%，这也是第五次连续会议按兵不动，企业和家庭的贷款成本将继续保持在高位，按揭、汽车贷款和企业融资的利率短期内不会下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nypost.com/2026/07/29/business/fed-holds-interest-rates-steady-as-dissent-mounts-over-whether-to-hike-rates-soon/">Fed holds interest rates steady as dissent mounts over whether to...</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh</a></li>
<li><a href="https://ops.lightwards.com/article/fed-holds-rates-steady-while-three-economic-systems-clash">Fed Holds Rates Steady Amid Economic System Clash</a></li>
<li><a href="https://tradingeconomics.com/united-states/interest-rate">United States Fed Funds Interest Rate</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#central bank`

---

<a id="item-finance-news-2"></a>
### [美联储主席沃什在众议院就通胀与货币政策作证](https://news.google.com/rss/articles/CBMitwFBVV95cUxNNGoza1B1bFlYakZUZTlfMDZXQW5lak5PUUJmazNOUTZXdzZsb0ZfaUdNRmRZSmRHQmVLM1YweXBYaG5QWko3UE9pWk13MThsazJXZnAxZXQzdjFBNS1JQndtTU5WYzNjbExBWFVmaHRiUGlzNVB6WW9yTmdwQWdyWGNvWktMMWpQcXZrVWFtVGxwYW5WUEY1WEhJUWw2MTFfaFFBREMxQkVfUmx6WGVsNzZoU1AwYjjSAbwBQVVfeXFMTmJaLU9CcDhYZjVFbnJ1OEk5MFdNTzNNNlNQcjZTNnBndmtVMUFaaGVhYVZaR05MMnVKekp6NmlLdXZRbUwyUEdmLUZvT3h1bkVsVEZoR0k3MFN2QXIxTmY5bUtPdVVBODgwMHBiSDlqbl96VU9xSHppMGY4Q1M1VTVRVXl3VldVQ1dMTHoxNndVcDd5VEUySWZhSmU1RWtsSVpvUFVWWkI5T3Bfdy1FWHN2Zy1GT0R4UnhmN1M?oc=5) ⭐️ 9.0/10

据 PBS 报道，美联储主席凯文·沃什（Kevin Warsh）正在众议院听证会上就通胀和货币政策作证，相关过程以直播形式播出。

google\_news · PBS · 7月13日 07:00

**「背景」** 这是美联储主席凯文·沃什首次就半年度货币政策报告赴国会作证；他在众议院金融服务委员会听证会上表示将让高通胀成为过去，但没有给出下一步政策信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/politics/watch-live-fed-chair-kevin-warsh-testifies-on-monetary-policy-in-house-hearing">WATCH: Fed chair Kevin Warsh testifies on inflation and monetary policy in House hearing | PBS News</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/testimony/warsh20260714a.htm">Testimony by Chairman Warsh on the semiannual Monetary Policy Report to Congress - Federal Reserve Board</a></li>
<li><a href="https://www.cnbc.com/2026/07/14/warsh-promises-inflation-will-be-a-thing-of-the-past-cites-benefits-of-ai-investment-boom.html">Warsh pledges Fed policy &#x27;regime change&#x27; to rid inflation &#x27;tax&#x27; on American people</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Congress`, `#Kevin Warsh`

---

<a id="item-finance-news-3"></a>
### [英国央行发布 2026 年 7 月货币政策报告](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

英国央行发布 2026 年 7 月《货币政策报告》，阐述其最新政策立场与对经济的展望。目前可见内容未披露具体利率决定或数据。

google\_news · Bank of England · 7月30日 07:00

**「背景」** 这份季度《货币政策报告》是英国央行货币政策委员会用来作出利率决定的经济分析和通胀预测依据。在 2026 年 7 月 29 日结束的会议上，委员会以 6 比 3 的投票结果将基准利率维持在 3.75%，三名委员主张加息 0.25 个百分点至 4%。

**「影响」** 英国央行将基准利率（Bank Rate）维持在 3.75%，意味着与基准利率挂钩的房贷、企业贷款等借贷成本短期内不会立即变动；货币政策委员会以 6 比 3 投票通过维持利率，其中 3 名委员主张加息至 4%，显示决策层对通胀路径存在分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/2026/july-2026">Monetary Policy Report - July 2026 (to be published at 12pm) | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-summary-and-minutes/2026/july-2026">Bank Rate maintained at 3.75% - July 2026 Monetary Policy Summary and Minutes | Bank of England</a></li>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-summary-and-minutes/2026/july-2026">Bank Rate maintained at 3.75% - July 2026 Monetary Policy Summary and Minutes | Bank of England</a></li>

</ul>
</details>

**标签**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#inflation`, `#economic outlook`

---

<a id="item-finance-news-4"></a>
### [CME 计划推出 AI 算力期货合约，算力有望成为可交易资产类别](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 8.0/10

CME 集团宣布，待监管批准后，将于 10 月 5 日与 Silicon Data 合作推出首批 AI 算力期货合约。合约将基于 Nvidia H100 和 Blackwell B200 GPU 的每小时租赁价格指数，每份合约代表 H100 一个月的租金。

rss · CNBC Finance · 8月12日 14:14

**「背景」** CME 集团与 Silicon Data 最早于 2026 年 5 月 12 日宣布这一合作；Silicon Data 此前发布的“GPU 前瞻曲线”提供了 GPU 租用成本现在和未来的标准化预期，这些期货合约将跟踪该公司编制的 GPU 小时租金指数。

**「影响」** 一旦推出，AI 开发者和数据中心运营商可使用这些合约对冲算力成本或收入，投资者也能在不直接投资数据中心或芯片的情况下获得算力价格敞口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cmegroup.com/media-room/press-releases/2026/8/11/cme_group_and_silicondatatolaunchcomputefuturesonoctober5tounloc.html">CME Group and Silicon Data to Launch Compute Futures on...</a></li>
<li><a href="https://siliconangle.com/2026/05/12/cme-group-silicon-data-launch-ai-compute-futures-market/">CME Group and Silicon Data to launch AI compute futures market</a></li>
<li><a href="https://cryptobriefing.com/cme-group-compute-futures-launch/">CME Group launches compute futures for trading on October 5</a></li>

</ul>
</details>

**标签**: `#AI`, `#futures`, `#CME`, `#Nvidia`, `#financial innovation`

---

<a id="item-finance-news-5"></a>
### [乌克兰袭击导致俄黑海主要谷物码头停运](https://oilprice.com/Geopolitics/Europe/Ukrainian-Attack-Halts-Operations-at-Key-Russian-Black-Sea-Grain-Terminals.html) ⭐️ 8.0/10

乌克兰无人机和导弹袭击俄罗斯新罗西斯克港，损坏黑海谷物出口码头；据路透社援引业内消息人士，俄两大粮食码头已暂停运营。

rss · OilPrice.com · 8月12日 23:00

**「背景」** 俄罗斯是全球最大小麦出口国，大部分经新罗西斯克等黑海港口运出；此前俄海军舰艇因克里米亚塞瓦斯托波尔基地频繁遭袭而转移，部分甚至移至里海。

**「影响」** 报道称，这可能严重影响全球粮食供应，尤其是非洲；俄主要粮食游说团体上月警告，此类袭击可能推高粮价并在非洲和中东引发饥饿。

**标签**: `#Grain Exports`, `#Black Sea`, `#Ukraine Conflict`, `#Russia`, `#Food Security`

---

<a id="item-finance-news-6"></a>
### [EIA：到 2027 年底中东仍有约 60 万桶/日原油停产](https://oilprice.com/Energy/Crude-Oil/EIA-Sees-600000-Bpd-of-Middle-East-Oil-Still-Offline-by-End-2027.html) ⭐️ 8.0/10

美国能源信息署（EIA）在最新短期能源展望中预测，由于霍尔木兹海峡通行持续受限，到 2027 年底中东仍有约 60 万桶/日的原油产量无法恢复；同时将三季度布伦特原油均价预测上调 11 美元/桶，至约 85 美元/桶。

rss · OilPrice.com · 8月12日 22:00

**「背景」** 7 月底以来中东紧张局势再度升级，导致霍尔木兹海峡航运严重受限，中东产油国部分产量关闭。EIA 假设 8 月海峡通行仍将严重受限、9 月起流量缓慢恢复，并估计 7 月中东停产规模平均为 550 万桶/日，低于 3 至 5 月平均的 1010 万桶/日。

**标签**: `#oil supply`, `#Strait of Hormuz`, `#EIA forecast`, `#Middle East`, `#crude oil prices`

---

<a id="item-finance-news-7"></a>
### [炼油设施遇袭加剧全球柴油供应紧张](https://oilprice.com/Energy/Energy-General/Refinery-Attacks-Deepen-Global-Diesel-Supply-Crunch.html) ⭐️ 8.0/10

乌克兰和胡塞武装对俄罗斯及沙特炼油设施的袭击，加剧了全球柴油供应紧张。美国柴油期货周一上涨 7.4%至每加仑 4.19 美元，零售均价为 5.32 美元，高于一个月前的 4.88 美元和一年前的 3.71 美元。

rss · OilPrice.com · 8月12日 20:00

**「背景」** 全球柴油供应此前已因中东冲突和乌克兰无人机袭击俄罗斯炼油网络而失衡，这次袭击正值需求旺季来临前；炼油厂利用率已接近上限，而维护季又将造成额外减产。

**「影响」** 柴油涨价可能首先冲击货运、农业和冬季取暖等用油行业，并随成本转嫁推高消费品价格和整体通胀。

**标签**: `#diesel supply`, `#refinery attacks`, `#refining margins`, `#energy markets`, `#inflation`

---

<a id="item-finance-news-8"></a>
### [普京威胁扣押欧盟船只，回应欧盟对俄影子船队制裁](https://oilprice.com/Latest-Energy-News/World-News/Putin-Opens-New-Front-in-Shadow-Fleet-Fight-With-Threat-to-Seize-EU-Ships.html) ⭐️ 8.0/10

俄罗斯总统普京周三威胁称，如果欧洲国家没收俄罗斯船只或出售被扣船只上的货物，俄方将“对等回应”，并可能扣押欧洲船只。欧盟 7 月 23 日通过的第 21 轮制裁已新增 41 艘“影子船队”船只，使黑名单总数达到 673 艘。

rss · OilPrice.com · 8月12日 17:30

**「背景」** “影子船队”指规避西方制裁运输俄罗斯石油的船只。此前欧洲多国已在执法中扣押涉嫌违规的油轮，英国 6 月也在英吉利海峡拦截了受制裁油轮 Smyrtos；普京是在视察太平洋舰队演习时就俄方反制能力发表上述言论。

**「影响」** 若俄方将威胁付诸行动，欧洲及悬挂第三国旗帜的商业航运可能面临被检查或扣押的风险，并加剧外界对俄罗斯原油出口中断的担忧。

**标签**: `#Russia`, `#Sanctions`, `#Oil`, `#Shipping`, `#Energy`

---

<a id="item-finance-news-9"></a>
### [乌克兰据报应美方请求暂停攻击油轮和 CPC 管道](https://oilprice.com/Latest-Energy-News/World-News/Ukraine-Halts-Oil-Tanker-Attacks-on-JD-Vance-Request.html) ⭐️ 8.0/10

据《金融时报》援引未具名乌克兰官员报道，乌克兰已应美国副总统万斯的请求，暂停对俄罗斯新罗西斯克港油轮及 CPC 管道的无人机攻击，美方还要求基辅停止攻击黑海非俄罗斯油轮。此前相关袭击曾使哈萨克斯坦原油日产量从 6 月的逾 200 万桶降至 7 月底约 100 万桶。

rss · OilPrice.com · 8月12日 14:30

**「背景」** CPC 管道从哈萨克斯坦里海沿岸经新罗西斯克港出口原油，承担哈萨克斯坦约 80%的原油出口，被视为欧洲替代俄罗斯能源供应的重要通道。

**标签**: `#Oil Markets`, `#Geopolitics`, `#Kazakhstan Exports`, `#Ukraine Conflict`, `#Energy Supply`

---

<a id="item-finance-news-10"></a>
### [LME 铝库存降至 1990 年以来最低](https://oilprice.com/Metals/Commodities/LME-Aluminum-Stockpiles-Sink-to-Lowest-Level-Since-1990.html) ⭐️ 8.0/10

伦敦金属交易所（LME）铝库存降至 25 万吨，为 1990 年 11 月以来最低，主因挪威海德罗（Norsk Hydro）旗下 Alunorte 氧化铝精炼厂因天然气供应中断减产 50%。铝价在伦敦上涨近 2%，至每吨 3373 美元，创七周新高。

rss · OilPrice.com · 8月12日 14:00

**「背景」** 天然气为氧化铝精炼提供高温蒸汽；Alunorte 位于巴西、年产能约 630 万吨，海德罗称供气恢复后即恢复满产。

**「影响」** 评论称，铝和铜等工业金属涨价会推高电网扩建、电动汽车等电气化与脱碳项目的成本。

**标签**: `#aluminum`, `#Norsk Hydro`, `#LME inventories`, `#supply disruption`, `#copper`

---

<a id="item-finance-news-11"></a>
### [腾讯第二季度营收超预期，资本开支激增至 528 亿元致自由现金流转负](https://wallstreetcn.com/articles/3779275) ⭐️ 8.0/10

腾讯控股 2026 年第二季度营收 2048 亿元人民币，同比增长 11%，略超彭博预期；净利润同比仅增 0.7%至 560 亿元，低于市场预期。当季资本开支同比近翻三倍至 528 亿元，自由现金流录得-138 亿元；公司称剔除 AI 算力预付款后自由现金流为 376 亿元。

telegram · zaihuapd · 8月12日 10:30

**「背景」** 自由现金流是指经营现金流扣除资本开支后的余额，为负代表当期投入超过经营现金产出；腾讯本季资本开支大增且包含 AI 算力预付款，直接导致该项转负。

**标签**: `#Tencent`, `#earnings`, `#capital expenditure`, `#free cash flow`, `#AI investment`

---

<a id="item-finance-news-12"></a>
### [台积电与索尼在日本成立合资企业，开发智能手机图像传感器](https://finance.yahoo.com/technology/articles/tsmc-sony-establish-jv-japan-133700498.html) ⭐️ 8.0/10

据相关报道，台积电与索尼宣布在日本成立合资企业，专注于开发智能手机图像传感器，显示两家半导体巨头在影像感测领域展开战略合作。

openbb · NVDA · 8月12日 13:37

**「背景」** 台积电与索尼成立合资企业，开发并制造智能手机图像传感器。该合资企业由索尼持股约 60%、台积电持股约 40%，将作为索尼子公司运营，预计最早于 2029 年在日本熊本县开始量产。

**「影响」** 这一合资计划预计将强化索尼在全球手机图像传感器市场的龙头地位，并让台积电进一步深入图像传感器代工供应链，可能影响依赖相关传感器的智能手机厂商的供应格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marketscreener.com/news/sony-group-tsmc-to-form-4-7-billion-image-sensor-joint-venture-ce7859dad081f523">Sony Group, TSMC to Form $4.7 Billion Image - Sensor Joint Venture</a></li>
<li><a href="https://www.mobileworldlive.com/devices/sony-tsmc-agree-4-7b-image-sensor-jv/">Sony , TSMC agree $4.7B image sensor JV - Mobile World Live</a></li>
<li><a href="https://www.khaleejtimes.com/business/sony-tsmc-to-spend-63-billion-to-jointly-make-image-sensors-nikkei-says">Sony , TSMC to spend $6.3 billion to jointly make image sensors ...</a></li>
<li><a href="https://www.nigeriaprivateschools.com/index.php/en/post-detail/3169/Sony-and-TSMC-to-Spend-$6.3-Billion-to-Jointly-Make-Image-Sensors">Sony and TSMC to Spend $6.3 Billion to Jointly Make Image Sensors</a></li>
<li><a href="https://asia.nikkei.com/business/tech/semiconductors/sony-tsmc-to-invest-6.3bn-in-advanced-image-sensor-plant-in-kumamoto">Sony , TSMC to invest $6.3bn in advanced image sensor... - Nikkei Asia</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#Sony`, `#joint venture`, `#semiconductors`, `#image sensors`

---

<a id="item-finance-news-13"></a>
### [台积电 7 月营收同比增 45%，股价较历史高点低 13%](https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductors-july-revenue-rose-075800266.html) ⭐️ 8.0/10

台积电公布 7 月营收同比增长 45%，但其股价目前仍比历史高点低 13%。

openbb · NVDA · 8月12日 07:58

**「背景」** 台积电（TSMC）是全球最大的半导体代工企业，其月度营收数据常被视为 AI 芯片需求的重要风向标。

**「影响」** 强劲的人工智能芯片需求推动台积电 7 月营收同比增长 45%；作为全球最大芯片代工厂，台积电的业绩增长对 AI 芯片供应链上下游企业具有直接意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lFNU5MakVSRUhyQkh1dHBfZkJDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Strong AI demand drives TSMC sales up 45 % in July ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lFNU5MakVSRUhyQkh1dHBfZkJDZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Strong AI demand drives TSMC sales up 45% in July ...</a></li>
<li><a href="https://www.osoulmisrmagazine.com/445176">World&#x27;s biggest chipmaker TSMC &#x27;s sales surge 45% amid buoyant AI...</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductor`, `#revenue`, `#stock market`, `#Taiwan`

---

<a id="item-finance-news-14"></a>
### [微软被曝将上调 Windows OEM 授权费 7%至 10%](https://www.techspot.com/news/113430-microsoft-raises-windows-oem-fees-pc-makers-7.html) ⭐️ 7.0/10

据 TechSpot 报道，微软据称将从 2026 年 7 月起把部分 PC 厂商的 Windows 预装授权费上调 7%至 10%，高于往年个位数涨幅；零售版 Windows 11 价格不变。该消息尚未获得微软证实。

telegram · zaihuapd · 8月12日 02:32

**「背景」** OEM 授权费指 PC 厂商随设备预装 Windows 向微软支付的费用，费率因品牌和产品线而异。报道称，PC 行业已受内存等元件涨价挤压，部分原本 600 至 800 美元的机型已接近 1000 美元。

**「影响」** 若属实，新增授权成本可能被转嫁给消费者，进一步推高部分 PC 终端售价。

**标签**: `#Microsoft`, `#Windows OEM`, `#licensing fees`, `#PC market`, `#price increase`

---