---
layout: default
title: "Horizon Summary: 2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> 从 237 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [OpenAI 称解决纳维-斯托克斯问题，遭合作数学家质疑](#item-tech-news-1) ⭐️ 9.0/10
2. [AlphaGenome Atlas：人类 DNA 单碱基变化预测图谱](#item-tech-news-2) ⭐️ 8.0/10
3. [NeurIPS 用 AI 检测器拒绝 178 篇论文引发争议](#item-tech-news-3) ⭐️ 8.0/10
4. [ASML 与台积电合作推进 High NA EUV 转向 12 英寸光掩模](#item-tech-news-4) ⭐️ 8.0/10
5. [Meta 发布个人 AI 代理 Muse 引发隐私与安全讨论](#item-tech-news-5) ⭐️ 7.0/10
6. [Qwen3.8 27B 量化基准：4 位可用，1 位崩溃](#item-tech-news-6) ⭐️ 7.0/10
7. [马来西亚评估华为 AI 芯片主权项目，或成弃美选华先例](#item-tech-news-7) ⭐️ 7.0/10
8. [张一鸣督导字节跳动空间视频模型](#item-tech-news-8) ⭐️ 7.0/10
9. [中国计划 2030 年智能算力提升至 9800 EFLOPS](#item-tech-news-9) ⭐️ 7.0/10
10. [OpenAI 发布 ChatGPT Images 2.5：图像更清晰、生成更快](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [伊朗石油出口在霍尔木兹对峙中崩溃](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储在新任主席沃什领导下维持利率不变](#item-finance-news-2) ⭐️ 9.0/10
3. [铜价突破每吨 14,500 美元创新高](#item-finance-news-3) ⭐️ 8.0/10
4. [美沙民用核协议绕开最严 IAEA 检查，进入国会 90 天审议](#item-finance-news-4) ⭐️ 8.0/10
5. [国际油价逼近每桶 100 美元](#item-finance-news-5) ⭐️ 8.0/10
6. [NVIDIA 与 ASML 参投 Mistral AI 30 亿欧元融资轮](#item-finance-news-6) ⭐️ 8.0/10
7. [Amkor 宣布 120 亿美元扩建亚利桑那园区，加码美国芯片制造](#item-finance-news-7) ⭐️ 8.0/10
8. [道指大幅下跌，高通因亚马逊合作突破关键价位](#item-finance-news-8) ⭐️ 8.0/10
9. [胡塞武装袭击沙特石油设施，布伦特原油逼近每桶 100 美元](#item-finance-news-9) ⭐️ 8.0/10
10. [美国恢复对伊朗打击，油价大涨加剧通胀担忧](#item-finance-news-10) ⭐️ 8.0/10
11. [美联储维持利率不变，保留未来加息空间](#item-finance-news-11) ⭐️ 8.0/10
12. [美联储维持基准利率不变 鲍威尔举行新闻发布会](#item-finance-news-12) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 称解决纳维-斯托克斯问题，遭合作数学家质疑](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI 在一篇新文章中宣称，其未发布的内部模型系统已经给出纳维-斯托克斯存在性与光滑性问题的解答——这是克雷数学研究所于 2000 年 5 月 24 日设立、每个悬赏 100 万美元的千禧年大奖难题之一。OpenAI 称，相关代理任务 9 月 1 日在听到两个千禧年问题已被解决的传闻后启动，约 88 小时后产出结果，再由 GPT-6 Astra 耗时约 17 小时完成 Lean 形式化验证；所有尝试共发送 490 万条消息、使用约 3000 亿输出 token，其中纳维-斯托克斯部分约占 1300 亿。由于合作研究者 Tristan Buckmaster 和供职于 Anthropic 的数学家 Levent Alpöge 曾用 OpenAI 的 Codex 等工作几乎一年并已在 8 月 15 日取得突破，Buckmaster 指控 OpenAI 是听说他们成果后才跟进，且未正面回答模型是否在其未公开会话数据上训练；OpenAI 则否认看到其工作，但承认不能排除去标识化用户数据用于改进模型，还因与 Anthropic 的竞争关系拒绝把 Alpöge 列为共同作者。该数学结论目前尚未经过独立验证，因而仍是重大但未经证实的声明。

rss · Simon Willison · 9月8日 23:55

**「背景」** 纳维-斯托克斯存在性与光滑性问题是流体力学中的核心数学难题：它要求说明，在给定合适的初始条件下，描述粘性流体运动的纳维-斯托克斯方程是否总存在全局光滑解，还是会在有限时间发展出奇点。该问题被列为克雷数学研究所的七个千禧年大奖难题之一，解决者可获得 100 万美元奖金。这次事件意味着大型语言模型系统声称已经独立完成这类最高级别数学问题的证明，同时还牵涉到 AI 产品用户数据是否可能通过训练影响未来模型决策的争议。

**「影响」** 如果这一解法能通过后续数学验证，AI 系统将首次对流体力学长期未解难题给出得到认可的解答，可能大幅改变数学研究对 AI 辅助证明和成果共享节奏的预期。与此同时，Buckmaster 与 Alpöge 的指控已经提醒研究者：未发表的草稿，甚至只是“有人正在研究某题”的传闻，都可能在未来触发大模型的大规模正面竞争。

**「社区讨论」** Hacker News 评论者普遍关注“抢先”争议，并转引 Terence Tao 的观点：即使只是有传闻称某人在研究某个问题，也可能引来大量 AI 算力平推式攻关，形成“不再和社区分享研究方向”的逆向激励。也有声音指出被掩盖的事实是 OpenAI 内部模型在数学上进步极快，并提醒不应把自然科学研究简化成纯计算问题；还有人转述 OpenAI 声明中的具体主张，即该证明认为流体动力学可在有限时间形成奇点。

**标签**: `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize`, `#AI research`, `#mathematics`

---

<a id="item-tech-news-2"></a>
### [AlphaGenome Atlas：人类 DNA 单碱基变化预测图谱](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 8.0/10

谷歌 DeepMind 发布了 AlphaGenome Atlas，这是一种旨在预测人类基因组中每一个可能的 DNA 字母变化影响的高分辨率图谱。该项目以 DeepMind 的 AlphaGenome 研究为基础，据称会覆盖编码和非编码 DNA，而非编码区域在以往研究中通常注释不足。官方提供了 Atlas 数据集入口，并配有面向科学家的使用讲解视频，以便研究界开始探索该资源。它的潜在意义在于帮助解释遗传变异如何影响基因调控与疾病，但公告本身没有提供验证数据或独立基准，因此实际影响力仍有待检验。

hackernews · utiiiD · 9月8日 14:55 · [社区讨论](https://news.ycombinator.com/item?id=49611251)

**「背景」** AlphaGenome Atlas 是 Google DeepMind 发布的一份高分辨率人类 DNA 预测图谱，旨在预测人类基因组中每一种可能的单核苷酸变异（即 DNA 单个字母改变）可能带来的分子效应。这份图谱覆盖了人类基因组中约 90 亿个单核苷酸变异，并为每个变异提供 AVI 分数等预测指标。其背后的 AlphaGenome 模型于 2025 年 6 月首次亮相，目前已扩展到人类基因组的全部分析位点，并且图谱也包含了对非编码 DNA 区域的预测。

**「影响」** AlphaGenome Atlas 的发布为研究人类基因组中约 90 亿种可能单核苷酸变异的研究人员提供了一个开放的高分辨率调控预测资源，有助于加速对遗传疾病和非编码区变异功能的解析；但由于这些结果源于 AI 预测，仍需通过实验验证后才能用于临床判断。

**「社区讨论」** 评论中有人提出该工具没有专门说明启动子序列，并追问对非编码调控区域的解读能力；也有人分享说访问 Atlas 时“affiliation”一栏可以不填、直接提交即可，还贴出了相关视频教程。另有用户询问能否用 23andMe 的基因组数据查找致病突变，同时有人提醒并非谷歌 DeepMind 推出的每一个生物学深度学习模型都能像 AlphaFold 那样保持持续影响力，实际效果需要更全面的观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas : Molecular predictions for 9 Billion human DNA ...</a></li>
<li><a href="https://theoutpost.ai/news-story/google-deep-mind-unveils-alpha-genome-atlas-with-9-billion-human-genome-mutation-predictions-30577/">Google DeepMind &#x27;s AlphaGenome Atlas Maps 9 Billion Human ...</a></li>
<li><a href="https://www.techeblog.com/google-deepmind-alphagenome-atlas-human-dna-map/">Google DeepMind &#x27;s AlphaGenome Atlas Places a Score... - TechEBlog</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">AlphaGenome Atlas: a high-resolution map of human DNA</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA variants — Google DeepMind</a></li>
<li><a href="https://www.scientificamerican.com/article/new-google-deepmind-alphagenome-atlas-could-transform-our-understanding-of-genetic-diseases/">New Google DeepMind atlas could transform our understanding of genetic diseases | Scientific American</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#genomics`, `#deep learning`, `#bioinformatics`, `#research`

---

<a id="item-tech-news-3"></a>
### [NeurIPS 用 AI 检测器拒绝 178 篇论文引发争议](https://www.reddit.com/r/MachineLearning/comments/1wakf62/neurips_deskrejected_178_papers_for_being/) ⭐️ 8.0/10

NeurIPS Position Paper Track 使用专有 AI 检测器 Pangram 对投稿进行桌面拒稿，共 178 篇（占 18.4%）被直接拒绝，且没有人工评审或申诉流程。独立研究者将三位赛道主席近期论文送入同一检测器，得到的 AI 概率为 24%到 69%；若按相同规则，主席们也可能被拒。检测器最初标记了 42.7%的投稿，主办方缩小文本窗口后才将比例降至 12.7%；另有 22 篇论文因检测得分&gt;0.5 且作者否认 AI 使用而被拒，检测分数被当作作者说谎的证据。斯坦福研究显示 61.22%的真人托福作文会被误判为 AI，而 NeurIPS 未公布任何人口学校准数据，非英语母语研究者面临更高风险。被拒论文不会留下学术不端记录，作者可在 ICLR（9 月 25 日截止）或 ICML 重新投稿。

reddit · r/MachineLearning · /u/tughanbulut · 9月8日 10:19

**「背景」** NeurIPS 2026 的 Position Paper Track（立场论文轨道）是会议中要求作者明确声明是否使用 AI 生成工具的投稿类别。该轨道组织方使用商业 AI 检测器 Pangram 筛查疑似违规投稿，并于 2026 年 6 月公告：经过独立核查后仍维持政策，最终有 178 篇论文（占全部投稿的 18.4%）被直接桌拒（desk reject），且不提供申诉渠道。此前已有社区讨论指出该检测器未经过校准，为后续关于公平性和检测可靠性的争议提供了背景。

**「影响」** 受影响作者的直接后果是无申诉就被拒稿，而会议的公信力因误报和缺乏人口学校准而受到损害，其中非英语母语研究者的误判风险最高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.neurips.cc/2026/06/02/ai-generated-papers-in-the-neurips-2026-position-paper-track/">AI-Generated Papers in the NeurIPS 2026 Position Paper Track – NeurIPS Blog</a></li>
<li><a href="https://casrai.org/news/neurips-2026-pangram-ai-detector-desk-rejection-controversy">NeurIPS 2026: Pangram AI-Detector Desk Rejections — CASRAI</a></li>

</ul>
</details>

**标签**: `#NeurIPS`, `#AI detection`, `#academic publishing`, `#research ethics`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [ASML 与台积电合作推进 High NA EUV 转向 12 英寸光掩模](https://www.nrc.nl/nieuws/2026/09/08/asml-gaat-samenwerken-met-taiwanese-chipgigant-tsmc-om-zijn-nieuwste-chipmachines-te-upgraden-a4936073) ⭐️ 8.0/10

ASML 与台积电于 9 月 7 日宣布产业合作，推动 High NA EUV 从目前的 6 英寸光掩模转向 12 英寸规格，目标是提高设备生产率、降低芯片制造成本并减少拼接限制。双方计划在 2031 年建立 12 英寸光掩模试产线，2033 年推动相关系统用于先进制程量产；台积电则拟于 2030 年起将 High NA 用于先进节点的大规模制造。这一路线图意味着下一代光刻技术将在数年内完成关键基础设施切换，影响主要落在先进逻辑芯片制造和配套材料设备供应链。

telegram · zaihuapd · 9月8日 06:55

**「背景」** High NA EUV 是继标准 EUV 之后的下一代极紫外光刻技术，用于生产更小的芯片制程节点，但当前光掩模尺寸限制了单次曝光的芯片面积。转向 12 英寸光掩模需要改变掩模版、光刻机、工艺和配套设施等多个环节，因此 ASML 与台积电的合作旨在提前构建产业生态。

**「影响」** 对台积电等先进逻辑芯片制造商而言，这一合作将 High NA EUV 的 12 英寸光掩模路线图正式固定到 2031 年试产、2033 年量产的时间点，并使 2030 年启用 High NA 成为台积电先进节点明确可考的计划；相关设备、掩模材料和光刻胶供应商也需要据此调整研发和产能布局。

**标签**: `#semiconductor`, `#photolithography`, `#ASML`, `#TSMC`, `#High NA EUV`

---

<a id="item-tech-news-5"></a>
### [Meta 发布个人 AI 代理 Muse 引发隐私与安全讨论](https://ai.meta.com/muse/) ⭐️ 7.0/10

Meta 在 ai.meta.com/muse 页面发布了名为 Muse 的个人 AI 代理，正式产品细节有限，具体能力和开放范围尚不明确。Hacker News 讨论认为，Meta 的目标是吸引不太了解模型细节的普通用户，因此其庞大的既有用户基础可能成为推广优势。讨论中有人转述 Meta AI 的 David Singleton 关于提示注入防护的说法，称其采用分层防御：模型训练识别和抵抗提示注入、对不可信来源内容加标记、用确定性代码检查结果，并在代理无法触达的位置运行分类器。与此同时，不少评论者对让 Meta 掌握大量个人数据表示强烈顾虑，但也有用户希望用 Muse 重新获取 Facebook 小组中的数据。

hackernews · yks · 9月8日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49615537)

**「背景」** Meta 于 2026 年 9 月推出个人 AI 代理 Muse，将其定位为“个人超级智能”的首个版本，并基于首席 AI 官 Alexandr Wang 带领开发的最新模型构建；产品在美国先行登陆 iOS、Android 与 muse.ai。Meta 在发布中强调安全与隐私主题，并将 Muse 称为 CEO 马克·扎克伯格所描述的长期开发中的关键下一步。

**「社区讨论」** 评论者普遍认为 Meta 正在争夺“普通用户层”，即那些不会追踪模型版本或参数细节的大众用户。明显分歧则集中在隐私与信任：有人认为不会使用 Meta 运营个人代理，也有用户计划将其用于抓取 Facebook 小组评论等具体场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/">Introducing Muse : The World’s First Personal AI Agent Built for...</a></li>
<li><a href="https://www.axios.com/2026/09/08/meta-debuts-muse-personal-ai-agent">Meta debuts Muse personal AI agent</a></li>
<li><a href="https://www.bnnbloomberg.ca/business/company-news/2026/09/08/meta-launches-personal-ai-agent-muse-emphasizes-safety-and-privacy/">Meta launches Muse , personal AI agent emphasizing safety &amp; privacy</a></li>

</ul>
</details>

**标签**: `#Meta`, `#AI agent`, `#personal assistant`, `#prompt injection`, `#tech industry`

---

<a id="item-tech-news-6"></a>
### [Qwen3.8 27B 量化基准：4 位可用，1 位崩溃](https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/) ⭐️ 7.0/10

针对 Qwen3.8 27B 的量化基准测试显示，4 位量化基本保持模型质量，2 位量化得分略低，而 1 位量化质量明显崩溃。这意味着本地部署该模型时，4 位量化是在不明显损失任务表现的情况下节省显存的可行选择，1 位量化则只适合对输出质量要求极低的极端资源场景。该结果对本地模型部署中的量化选型具有直接参考价值，但评论也指出测试在 3 位区间和 KV cache 量化方面仍有空白。

hackernews · stared · 9月8日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49611128)

**「背景」** Qwen3.8 27B 是阿里巴巴 Qwen3.8 系列中可本地运行的多模态稠密模型，完整 BF16 权重约 55GB，通常超过消费级硬件的显存容量。量化（quantization）通过降低权重数值精度来减小模型体积；常见 GGUF 格式中的 Q4\_K\_M 约 17GB，而更极端的 1-bit 量化可将体积压得很低，但会明显损害输出质量。该评测使用 Terminal-Bench 2.1 等智能体编码基准比较不同量化档位，结果显示 4-bit（如 Q4\_K\_M）表现接近原模型，2-bit 略低，1-bit 则严重崩塌。

**「影响」** 计划在个人电脑或有限显存环境部署 Qwen3.8 27B 的用户，可优先选择 4 位量化以平衡质量与资源占用；若显存严重受限，则需要警惕 1 位量化带来的质量崩塌。

**「社区讨论」** 评论者普遍认为低位量化对最终任务质量的影响有限，并猜测模型会通过更长的思考过程来补偿采样概率分布的偏移；同时希望补充 KV cache 量化和面向 16GB 以下显卡的 3 位区间测试。也有评论对文章中置信区间的统计用法提出异议，并出现关于本地运行安全隔离的新手疑问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quesma.com/blog/qwen38-27b-quantizations-benchmarked/">Benchmarking Qwen 3 . 8 27 B quantizations : 4-bit... - Quesma Blog</a></li>

</ul>
</details>

**标签**: `#quantization`, `#qwen`, `#benchmarking`, `#llm-inference`, `#local-models`

---

<a id="item-tech-news-7"></a>
### [马来西亚评估华为 AI 芯片主权项目，或成弃美选华先例](https://www.businesstimes.com.sg/international/malaysia-eyes-huawei-chips-ai-project-despite-us-warning) ⭐️ 7.0/10

马来西亚政府正认真评估采用华为 Ascend 910C 芯片作为其主权 AI 项目的核心，项目规模约为 20 亿令吉（约 4.94 亿美元）。消息人士称，目前尚不清楚计划采购的芯片数量。若该项目落实，将成为首个外国政府公开选择中国 AI 加速器而非美国产品的案例。此前特朗普政府曾警告使用该华为 AI 加速器可能违反美国出口规定，但马来西亚方面认为相关决定纯属商业考量。

telegram · zaihuapd · 9月8日 03:35

**「背景信息」** 华为 Ascend 910C 是华为研发的高端 AI 加速芯片，属于中国在人工智能算力领域挑战美国英伟达等产品的重要代表。由于该芯片可能涉及美国技术或设备，美国政府已警告使用或出口该芯片可能违反美国出口管制规定。马来西亚正评估以 20 亿令吉（约 4.94 亿美元）建立主权 AI 项目，若选用华为芯片，有望成为首个在官方层面选择中国 AI 加速器而非美国产品的外国政府，这一决定还需平衡地缘政治和供应链风险。

**「影响」** 若落地，马来西亚将成为首个在主权 AI 项目中选用中国 AI 加速器而非美国产品的外国政府，为华为芯片进入国家级 AI 基础设施打开重要先例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globalsources.com/sourcing-digest/malaysia-evaluates-huawei-ascend-910c-chips-for-a-landmark-sovereign-ai-initiative/?source=GSOLHP_SKC_5">Malaysia evaluates Huawei Ascend 910 C chips for... | Global Sources</a></li>
<li><a href="https://www.scmp.com/week-asia/politics/article/3366792/will-malaysias-potential-huawei-ai-deal-risk-clash-over-us-trade-pact">Will Malaysia ’s potential Huawei AI deal risk clash with US trade pact?</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#AI chips`, `#Malaysia`, `#export controls`, `#sovereign AI`

---

<a id="item-tech-news-8"></a>
### [张一鸣督导字节跳动空间视频模型](https://www.bloomberg.com/news/articles/2026-09-07/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models) ⭐️ 7.0/10

据彭博社报道，字节跳动创始人张一鸣正亲自督导一款实时空间视频生成模型，该模型最快可能在 2026 年 10 月发布，但时间仍可能调整。模型基于 Seedance，可生成响应 Pico 头显用户语音或动作的互动虚拟世界，据称能以约 0.05 秒延迟、每秒 20 帧生成视频，并将高强度计算转移至云端，以降低 VR 设备的硬件门槛。该消息来自知情人士，目前尚未确认正式发布日期，具体技术细节也未完全公开。

telegram · zaihuapd · 9月8日 04:05

**「背景」** 空间视频模型（又称世界模型）是一种能够根据用户输入实时生成三维交互场景的 AI 系统，类似 Google 的 Genie。字节跳动此前已有视频生成模型 Seedance，并拥有虚拟现实硬件品牌 Pico；张一鸣虽已淡出字节跳动的日常运营，但仍参与这项由 Bloomberg 报道的高层项目。

**「影响」** 若字节跳动按报道在 2026 年 10 月推出该空间视频模型，Pico 头显用户有望在不依赖高价本地显卡的情况下，通过云端生成响应语音和动作的实时互动虚拟世界，从而降低 VR/AR 设备的硬件门槛；同时这将加剧与世界实验室等世界模型头部团队的竞争。不过字节尚未官方确认发布时间，性能数据也来自匿名知情人士，实际效果仍有待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models">ByteDance founder joins AI elite in race to perfect world models</a></li>
<li><a href="https://technode.com/2026/09/08/bytedance-real-time-spatial-video-model-zhang-yiming/">ByteDance is reportedly developing a real-time spatial video model ...</a></li>
<li><a href="https://startupfortune.com/zhang-yiming-is-personally-building-bytedances-real-time-world-model/">Zhang Yiming Is Personally Building ByteDance &#x27;s Real-Time World...</a></li>
<li><a href="https://www.worldlabs.ai/blog/atlas">Atlas: A World Model for Spatial Intelligence | World Labs</a></li>
<li><a href="https://www.straitstimes.com/business/bytedance-founder-joins-ai-elite-in-race-to-perfect-world-models">ByteDance founder joins AI elite in race to perfect world models</a></li>

</ul>
</details>

**标签**: `#ByteDance`, `#spatial video`, `#world models`, `#real-time AI`, `#VR/AR`

---

<a id="item-tech-news-9"></a>
### [中国计划 2030 年智能算力提升至 9800 EFLOPS](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 7.0/10

中国工业和信息化部发布未来五年产业规划，提出到 2030 年将中国智能算力提升至 9800 EFLOPS，并在 2026 年至 2030 年累计投入 3.8 万亿元用于信息基础设施建设。规划还提出有序部署万卡级以及 10 万卡以上的智能计算集群，并加强基础设施与国产算力芯片的适配。截至今年 6 月底，中国智能算力达到 2185 EFLOPS，同比增长 177%，要实现 2030 年目标，算力规模需在此基础上增长至 4 倍以上。这一规划反映了中国强化 AI 基础设施和国产算力供应的政策方向，但仍属于目标设定而非即时技术突破。

telegram · zaihuapd · 9月8日 11:23

**「背景」** EFLOPS 是衡量智能算力的单位，代表每秒百亿亿次（10 的 18 次方）浮点运算。中国工业和信息化部发布的 2026—2030 年信息通信业发展规划，提出到 2030 年将全国智能算力提升至 9800 EFLOPS，较 2025 年 6 月底的 2185 EFLOPS 增长四倍以上；同时计划在相关领域累计投入 3.8 万亿元人民币（约 5660 亿美元），并推动国产算力芯片与基础设施适配。该规划属于国家产业政策方向，反映中国在人工智能算力基础设施和自主芯片生态上的长期部署。

**「影响」** 该规划将为 AI 基础设施相关企业带来长期投资和建设预期，同时可能加速国产算力芯片在大型智能计算集群中的规模部署，但实际推进速度和达标程度仍取决于技术和供应链进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/miit-plan-targets-9800-eflops-of-intelligent-compute-by-2030/">MIIT Plan Targets 9,800 Eflops of Intelligent Compute by 2030</a></li>
<li><a href="https://aiweekly.co/alerts/miit-targets-9800-eflops-of-ai-compute-by-2030-532b-plan">MIIT Targets 9,800 Eflops of AI Compute by 2030 , $532B Plan</a></li>
<li><a href="https://ningbo.chinadaily.com.cn/2026-09/08/c_1212000.htm">China to invest 3.8 trillion yuan in information infrastructure by 2030</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#China`, `#policy`, `#EFLOPS`, `#compute`

---

<a id="item-tech-news-10"></a>
### [OpenAI 发布 ChatGPT Images 2.5：图像更清晰、生成更快](https://openai.com/index/introducing-chatgpt-images-2-5/) ⭐️ 7.0/10

OpenAI 于 9 月 8 日发布 ChatGPT Images 2.5 图像模型，宣称细节更清晰、编辑更精准，图像生成延迟较 2.0 版本最高降低 50%。新模型已向 ChatGPT、ChatGPT Work 和 Codex 全平台用户推出，ChatGPT 界面同步新增 Sketch 手绘引导、模板、图片评论与提示词分享功能。API 也同步上线了 GPT-Image-2.5 Flare 和 Sunburst 两款新模型。此次发布是对现有图像生成能力的一次增量升级，主要面向提升出图质量、编辑精度和生成速度。

telegram · zaihuapd · 9月8日 18:45

**「背景」** ChatGPT Images 是 OpenAI 推出的人工智能图像生成模型系列，此前版本为 ChatGPT Images 2.0，可依据自然语言提示生成和编辑图像。此次发布的 2.5 版本在 2.0 基础上提升了细节清晰度、编辑精准度和生成速度，并将生成延迟最高降低 50%。同时，OpenAI 在 API 中提供 GPT-Image-2.5 Flare 和 Sunburst 两款模型，前者主打速度与质量平衡，后者面向需要更高精度的细致创作、生成时间更长；两款 API 模型均采用相同的 $8/$30 token 费率，并带有 C2PA 和 SynthID 内容来源标记。

**「影响」** 使用 ChatGPT、ChatGPT Work、Codex 以及 API 的用户可以立即获得更清晰的图像生成、更精准的编辑和最高降低 50% 的生成延迟，同时 Sketch 等新增界面功能也同步开放。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2 . 5 | OpenAI</a></li>
<li><a href="https://www.orcarouter.ai/blog/gpt-image-2-5-flare-sunburst">GPT - Image - 2 . 5 Flare vs Sunburst : New OpenAI Image APIs</a></li>
<li><a href="https://bota.chat/chatgpt-images-2-5/">ChatGPT Images 2 . 5 : 50% Faster, Flare vs Sunburst API</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#image-generation`, `#ChatGPT`, `#API`, `#AI-models`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [伊朗石油出口在霍尔木兹对峙中崩溃](https://oilprice.com/Energy/Crude-Oil/Irans-Oil-Exports-Collapse-as-Hormuz-Standoff-Drags-On.html) ⭐️ 9.0/10

美国与伊朗在霍尔木兹海峡的对峙已进入第七个月，伊朗 8 月港口出口装船量估计约为 26 万桶/日，较 2025 年 8 月的 170 万桶/日下降约 80%；油价也因此再次逼近每桶 100 美元。

rss · OilPrice.com · 9月9日 00:00

**「背景」** 美国自 7 月中旬恢复对伊朗的海上封锁，并实施名为“经济放逐行动”的施压，旨在切断伊朗政权最重要的硬通货石油收入。

**「影响」** 美国国内能源价格已受到影响：柴油价格创下纪录，加油站汽油均价超过每加仑 4 美元，在 11 月中期选举前加剧选民的经济压力。

**标签**: `#Iran`, `#oil exports`, `#Strait of Hormuz`, `#U.S. sanctions`, `#oil prices`

---

<a id="item-finance-news-2"></a>
### [美联储在新任主席沃什领导下维持利率不变](https://news.google.com/rss/articles/CBMipgFBVV95cUxOM3c5cXgydnhwSFlrWmlyVjJobnRCbFkxaHg2c3NtTEl6Z2VLSGNIMXN3dmlKS2JZSF9Gc2p1TTVrd1hEcVdxSzBRaU13RVh1eTJRLW1pRkp0cHdKbk9FSU5SZ2FncC1ZangzQzZkZjFSaHNRWm94TlNROExtSm56Zk1qckpwT1JweWVKV1daY0tUMk03eFZJakRpMjNBVzl5N1NEQzFn0gGrAUFVX3lxTE1wYkYxa2NtTktYZkMyQ3VCSG5vYkw3UkE1cGpqaTRwOXE1MVpsd1ZfbDA2X3lGOEF5WG51SHFBbEhXbWs1enFfS1k2ZWRDMzVUU21sT2RMbC04VkoxUXk0Z1pYMVpWejF0ZGNyaUpiVWxjLWZYWVVBU28tb082QWlwT29PX1o3ekFTUk1fdTdGb3drUm5FOEIzZEc3UGlCRjhaUDlsS3Y0Yk8wMA?oc=5) ⭐️ 9.0/10

美国联邦储备委员会在新任主席沃什的主持下决定维持利率不变，即没有加息或降息，显示货币政策短期内不作调整。

google\_news · aljazeera.com · 6月17日 07:00

**「背景」** 凯文·沃什近期接任美联储主席，外界正关注他会如何应对通胀与利率问题。本次利率决定前，美国长期利率因政府赤字扩大及科技企业大量举债投入人工智能基础设施而上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/inflation-federal-reserve-interest-rates-a8661a4be7fcf3076891382cf9df1a5e">New Fed chair Kevin Warsh under pressure to clarify views on inflation, interest rates | AP News</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#US economy`, `#central bank`

---

<a id="item-finance-news-3"></a>
### [铜价突破每吨 14,500 美元创新高](https://oilprice.com/Metals/Commodities/Copper-Surges-Above-14500-as-Supply-Squeeze-Deepens.html) ⭐️ 8.0/10

伦敦金属交易所（LME）三个月期铜周二盘中刷新纪录，达到每吨 14,533 美元，之后涨幅有所收窄；彭博数据显示，铜价今年以来上涨 17%，过去 12 个月上涨 47%。市场普遍认为，对美国关税的预期正把全球可流通铜吸向美国仓库，加剧其他地区的供应紧张。

rss · OilPrice.com · 9月8日 21:00

**「背景」** 铜是人工智能数据中心和电网扩建的关键原材料；关税威胁改变铜的流向，使原本可供全球市场的铜被大量吸入美国仓库，同时全球矿端供应条件也在恶化，推动实物经济重新定价稀缺性。

**「影响」** 铜价走高可能抬高电网、数据中心、电线电缆及相关制造业的原材料成本，并继续向更广泛的工业环节传导。

**标签**: `#copper`, `#commodities`, `#tariffs`, `#supply chain`, `#industrial metals`

---

<a id="item-finance-news-4"></a>
### [美沙民用核协议绕开最严 IAEA 检查，进入国会 90 天审议](https://oilprice.com/Alternative-Energy/Nuclear-Power/US-Saudi-Nuclear-Deal-Clears-Vienna-Hurdle-As-Congress-Review-Continues.html) ⭐️ 8.0/10

美国与沙特阿拉伯的民用核合作协议取得新进展：IAEA 总干事格罗西表示，沙特不会签署允许突击检查的《附加议定书》，但将在铀浓缩、转化和后处理等敏感环节上授予国际原子能机构“非常、非常相似”的核查与监督权。这项双边保障协定仍需提交 IAEA 理事会批准，整体协议则已进入美国国会 90 天审议期。

rss · OilPrice.com · 9月8日 17:00

**「背景」** 该协议基于今年 7 月 22 日美沙签署的“123 协议”，结束了十多年来因沙特不愿放弃铀浓缩权利而反复停滞的谈判；新安排允许美国企业在沙特建造核电站，未来若建浓缩厂，也由美国公司在沙特境内以“黑箱”模式运营，以避免技术转移。

**「影响」** 若国会不否决，西屋等美国核能企业有望竞逐沙特价值数十亿美元的核电建设合同；沙特也借此推进“愿景 2030”的能源多元化目标。

**标签**: `#nuclear energy`, `#Saudi Arabia`, `#IAEA`, `#US foreign policy`, `#nonproliferation`

---

<a id="item-finance-news-5"></a>
### [国际油价逼近每桶 100 美元](https://oilprice.com/Energy/Crude-Oil/Oil-Prices-Are-Once-Again-on-the-Brink-of-100.html) ⭐️ 8.0/10

受也门胡塞武装袭击沙特能源设施和美国打击伊朗油轮影响，国际油价已升至每桶 99 美元以上，逼近 100 美元，创三个月新高。OPEC+已完成每日 165 万桶自愿减产的撤回，并维持 10 月产量目标不变。

rss · OilPrice.com · 9月8日 15:13

**「背景」** 胡塞武装的导弹和无人机袭击已导致沙特多处能源设施暂停运营并造成人员受伤，伊朗还威胁在霍尔木兹海峡附近设立海上禁区，市场担心供应中断将进一步推高油价。

**标签**: `#oil prices`, `#geopolitical risk`, `#European gas`, `#energy markets`, `#OPEC+`

---

<a id="item-finance-news-6"></a>
### [NVIDIA 与 ASML 参投 Mistral AI 30 亿欧元融资轮](https://finance.yahoo.com/technology/ai/articles/nvidia-asml-back-mistral-3-230147307.html) ⭐️ 8.0/10

NVIDIA 和 ASML 参投了欧洲 AI 初创公司 Mistral AI 的新一轮融资，本轮规模为 30 亿欧元。报道称，这两家公司的回报前景可能有很大不同，反映其在 AI 行业的不同战略利益。

openbb · NVDA · 9月8日 23:01

**「背景」** Mistral AI 是一家欧洲人工智能初创公司，主打可自行部署的开源权重 AI 模型。它于 9 月 8 日宣布完成超过 30 亿欧元（约 35 亿美元）的 D 轮融资，投后估值超过 210 亿欧元（约 244 亿美元），据称是欧洲科技企业史上最大规模的股权融资；新投资者包括贝莱德旗下基金和卢森堡大公国，现有投资者 ASML 与英伟达也参与其中。

**「影响」** 对欧洲芯片业与 AI 应用方面而言，ASML 参与 Mistral 融资可能推动欧洲自主建设高性能计算基础设施，把芯片需求留在欧盟并减少对美中 AI 模型的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ca.finance.yahoo.com/news/nvidia-asml-back-mistral-3-230147307.html">NVIDIA and ASML Back Mistral’s €3 Billion Round. Their Payoffs Could Look Very Different</a></li>
<li><a href="https://ventureburn.com/mistral-raises-3-billion-sovereign-open-weight-ai/">Mistral Raises €3 Billion To Build The Future of Secure Open-Weight AI</a></li>
<li><a href="https://www.cryptopolitan.com/mistral-raise-asml-chip-deal-europe-ai-push/">Mistral raises €3B as ASML seals chip deals in European AI push - Cryptopolitan</a></li>
<li><a href="https://ioplus.nl/en/posts/why-asml-is-investing-15b-in-mistral---and-why-it-makes-sense">Why ASML is investing $1.5B in Mistral - and why it makes sense</a></li>
<li><a href="https://finance.yahoo.com/news/asml-invests-billions-nvidia-backed-095358773.html">ASML Invests Billions In Nvidia-Backed Mistral AI To Power Next Era Of Semiconductors</a></li>

</ul>
</details>

**标签**: `#Mistral AI`, `#NVIDIA`, `#ASML`, `#Venture Capital`, `#AI Industry`

---

<a id="item-finance-news-7"></a>
### [Amkor 宣布 120 亿美元扩建亚利桑那园区，加码美国芯片制造](https://finance.yahoo.com/markets/stocks/articles/amkr-stock-gains-hours-amkor-234207542.html) ⭐️ 8.0/10

Amkor Technology 宣布将投资 120 亿美元，扩建其在亚利桑那州的园区，以扩大美国芯片制造产能。消息公布后，Amkor 股价在盘后交易中上涨。

openbb · NVDA · 9月8日 23:42

**「背景」** Amkor Technology 宣布扩建其位于美国亚利桑那州的先进封装与测试园区，使其在该地区的总投资承诺增至约 120 亿美元；二期建设预计 2027 年底启动、2029 年底完成，两期合计预计可支持超过 3500 名当地员工。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stocktitan.net/news/AMKR/amkor-technology-announces-phase-2-of-arizona-advanced-packaging-and-m19aoplwpjtk.html">A roughly $12B expansion to package chips is planned in Arizona. Construction is anticipated to begin late 2027.</a></li>
<li><a href="https://lifestyle.middletownlifemagazine.com/story/676376/amkor-technology-announces-phase-2-of-arizona-advanced-packaging-and-test-campus-expands-investment-to-12-billion/">Amkor Technology Announces Phase 2 of Arizona Advanced Packaging and Test Campus; Expands Investment to $12 Billion | Middletown Life</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#Capital Expenditure`, `#Manufacturing`, `#Amkor`, `#US Supply Chain`

---

<a id="item-finance-news-8"></a>
### [道指大幅下跌，高通因亚马逊合作突破关键价位](https://www.investors.com/market-trend/stock-market-today/dow-jones-sp500-nasdaq-us-iran-attacks-oil-prices-jump-brent-crude/?src=A00220&amp;yptr=yahoo) ⭐️ 8.0/10

据 Investors.com 的盘中报道，受美国与伊朗紧张局势影响，油价大涨，道琼斯工业平均指数当日大幅下挫；与此同时，高通\(Qualcomm\)因与亚马逊达成合作而突破一个关键技术价位，一只化肥龙头股上涨。

openbb · BRK-B · 9月8日 20:51

**「背景」** 美国股市周二恢复交易，此前周一因劳工节休市。道琼斯工业平均指数下跌 511 点，跌幅 0.7%，因伊朗支持的胡塞武装袭击沙特阿拉伯后油价逼近每桶 100 美元，加剧通胀担忧。此外，高通（Qualcomm）与亚马逊（Amazon）达成一项关键交易，化肥行业龙头股上涨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hindustantimes.com/business/stock-market-today-dow-falls-511-points-as-oil-nears-100-us-iran-war-fuels-inflation-fears-101788881180215.html">Stock market today: Dow falls 511 points as oil nears $100, US-Iran war fuels inflation fears | Business News</a></li>
<li><a href="https://www.europesays.com/us/1051686/">Stock Market Today: Dow Dives, Qualcomm Clears Key Level On Amazon Deal; Fertilizer Leader Rises - United States</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/dow-drops-500-points-oil-134409139.html">Dow drops 500 points as oil nears $100 amid Iran war</a></li>

</ul>
</details>

**标签**: `#stock market`, `#Dow Jones`, `#oil prices`, `#Qualcomm`, `#geopolitical risk`

---

<a id="item-finance-news-9"></a>
### [胡塞武装袭击沙特石油设施，布伦特原油逼近每桶 100 美元](https://finance.yahoo.com/energy/articles/brent-crude-nears-100-houthi-122207804.html) ⭐️ 8.0/10

胡塞武装袭击沙特石油设施后，布伦特原油价格逼近每桶 100 美元，凸显全球原油供应中断的风险。

openbb · BRK-B · 9月8日 12:22

**「背景」** 胡塞武装袭击沙特南部能源设施后，沙特暂停部分作业。布伦特原油盘中突破每桶 99 美元，为 7 月底胡塞武装宣布对沙特实施海上封锁并攻击油轮以来最高；相关袭击也威胁红海与全球航运要道曼德海峡的通行。

**「影响」** 受胡塞武装袭击沙特石油设施影响，布伦特原油升至每桶 95.43 美元，已逼近 100 美元；该价格较一个月前上涨 13.92%。这将直接推高汽油、柴油和航空燃料价格，使依赖运输和能源的企业及家庭承受更高的成本，并可能加大通胀压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/energy/articles/brent-crude-nears-100-houthi-122207804.html">Brent crude nears $ 100 as Houthi strikes hit Saudi oil sites</a></li>
<li><a href="https://walletinvestor.com/news/trading-news/oil-nears-100-after-houthi-strikes-hit-saudi-energy-facilities/">Oil Nears $ 100 After Houthi Strikes Hit Saudi ... - WalletInvestor.com</a></li>
<li><a href="https://www.nytimes.com/2026/09/08/business/oil-prices-iran-war.html">Oil Climbs Toward $ 100 a Barrel Following Houthi Attacks</a></li>
<li><a href="https://tradingeconomics.com/commodity/brent-crude-oil">Brent crude oil - Price - Chart - Historical Data - News</a></li>

</ul>
</details>

**标签**: `#oil`, `#geopolitics`, `#energy`, `#supply disruption`, `#crude`

---

<a id="item-finance-news-10"></a>
### [美国恢复对伊朗打击，油价大涨加剧通胀担忧](https://news.google.com/rss/articles/CBMingFBVV95cUxPX1k2M25nYzF5bW1Db3RnMldRZ19jWklIUWthSDVPNkhIRk5QQXZfd2dCMHdvNmdrbU1KMlVwYjJZaEtPZzhEa3R3bTBvTEl4MDJ6Q2dWby1NZlJsYi15TzdnWVZLcmg2TTBkVm1NNWhWYlgtM3VFa3RieUJMN2V6NTBSQTFvck1HVkU5NzQ0aHQ2eXJDNGZIVmVKZVNRZw?oc=5) ⭐️ 8.0/10

据 NBC 新闻报道，美国恢复对伊朗的打击后，石油价格大幅上涨，市场对通胀的担忧随之加剧。报道未提供具体涨幅或更多政策细节。

google\_news · nbcnews.com · 9月1日 17:26

**「背景」** 美国军方宣布再次对伊朗实施打击后，作为全球基准的布伦特原油价格上涨近 4%，至每桶约 94 美元。市场担心，作为重要石油运输通道的霍尔木兹海峡可能出现供应中断，从而加重通胀压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/policy/articles/bond-yields-surge-stocks-tumble-143402187.html">Oil prices surge after U . S . renews Iran strikes , heightening ...</a></li>
<li><a href="https://www.puprime.com/oil-surges-as-hormuz-disruption-deepens-dma260902/">Oil Surges as Hormuz Disruption Deepens</a></li>

</ul>
</details>

**标签**: `#oil prices`, `#Iran`, `#inflation`, `#geopolitical risk`, `#energy markets`

---

<a id="item-finance-news-11"></a>
### [美联储维持利率不变，保留未来加息空间](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

美联储（美国联邦储备委员会）决定维持利率不变，但表示未来仍可能加息。

google\_news · CBS News · 6月17日 07:00

**「背景」** 美联储在议息会议上将基准利率维持在不变的水平，但近半数决策者表示，如果通胀持续偏高，他们可能支持在今年晚些时候加息。基准利率是影响贷款和储蓄利率的央行参考利率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aol.com/articles/federal-holds-interest-rates-steady-181753000.html">Federal Reserve holds interest rates steady but leaves door open ...</a></li>
<li><a href="https://www.kzyx.org/npr-news/2026-07-29/a-divided-federal-reserve-holds-interest-rates-steady-despite-high-inflation">A divided Federal Reserve holds interest rates steady despite high...</a></li>
<li><a href="https://www.usatoday.com/story/money/2017/11/01/fed-holds-interest-rates-steady-leaves-path-clear-dec-hike/821039001/">The Fed kept interest rates unchanged, left door open to a Dec. hike</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-12"></a>
### [美联储维持基准利率不变 鲍威尔举行新闻发布会](https://news.google.com/rss/articles/CBMivAFBVV95cUxObmE2Rm5TNnFlVmNSODAwcFBnekVlTWJHekl5VWEwRzB5UTlxSXNMYUlOTnozX2ZjZ01hZENCTkZPc0ZmOTA2NDVxelFYRVd0Q1BkQ29QeUpHM3YtbTU5aHY1Y2o3M0tmcjdRNTZ5bmN5UVJ0eEhQWXV2QnRlWDU4OTJ0TlZoMk56TGRlX2NCOXlkdkdCS1hJSVdJTGMybGRWMmlCSlcza2JERGFZREp5UTg4VEQwcERkbmc0btIBwgFBVV95cUxNRUVtRTEtNHprakRGTkIwd2s4UnY3bWlEcm40MWwyYnB4SGp2bXpJelNvZ2pya0FBdTJUZ0N2OVVzZDRlcV96ZDlGYkduWlk4dU9wM3d4eHVNZkFGN20wNUc4VzdmVE5JWjB3d0lnREw0U2kxU2l4YjhWNzFQc1p3R0ZUeW1rOE1EWWx1YjVOSGZucjZBZ2VzUDlJS1JmZTFHWDZ4YndYNXVBRGFIcXp5ajhKc2tGYnRBZENzSGhpeDg5Zw?oc=5) ⭐️ 8.0/10

据 PBS 报道，美联储在最近一次政策会议后决定维持基准利率不变，美联储主席鲍威尔随后举行新闻发布会。报道未披露具体利率水平、调整理由或未来政策路径。

google\_news · PBS · 3月18日 07:00

**「背景」** 美联储联邦公开市场委员会（FOMC）将基准利率维持在 4.25%至 4.5%不变，这是继 2024 年连续三次降息后的第二次按兵不动。主席鲍威尔在新闻发布会上表示，他计划在主席任期结束后继续留在美联储理事会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fox7austin.com/money/feds-interest-rate-steady-jerome-powell">Fed holds rates steady in Powell ’s possible final chair... | FOX 7 Austin</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Jerome Powell`, `#Economy`

---