---
layout: default
title: "Horizon Summary: 2026-08-25 (ZH)"
date: 2026-08-25
lang: zh
---

> 从 245 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [MS Paint 与照片应用被曝为本地 AI 图像隐加 GUID 水印](#item-tech-news-1) ⭐️ 8.0/10
2. [seL4 在 AArch64 完成安全证明，覆盖单核且非 MCS](#item-tech-news-2) ⭐️ 8.0/10
3. [可执行文件即 SQLite 数据库](#item-tech-news-3) ⭐️ 8.0/10
4. [AI 编程依赖或致专业能力退化](#item-tech-news-4) ⭐️ 7.0/10
5. [“Bart”：以 1931 年前英文训练的开源复古 LLM](#item-tech-news-5) ⭐️ 7.0/10
6. [AI 空间软件生成器：可编程 3D 对象](#item-tech-news-6) ⭐️ 7.0/10
7. [小米发布三款玄戒芯片，AI 旗舰 SoC 首搭小米 18 Fold](#item-tech-news-7) ⭐️ 7.0/10
8. [阿里云 Wan3.0 上线：30 秒视频 API 最低 0.3 元/秒](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [美联储维持利率不变：9 比 3 投票结果](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储连续第五次会议维持利率不变](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储面临多年来最不可预测的会议](#item-finance-news-3) ⭐️ 9.0/10
4. [胡塞武装袭击沙特红海油轮](#item-finance-news-4) ⭐️ 8.0/10
5. [美国扩大对伊制裁但未点名中国大型银行](#item-finance-news-5) ⭐️ 8.0/10
6. [道达尔能源支持两条绕开霍尔木兹海峡的主要输油管道](#item-finance-news-6) ⭐️ 8.0/10
7. [欧洲多国领导人齐聚基辅 讨论增强乌克兰防空](#item-finance-news-7) ⭐️ 8.0/10
8. [伊朗将 45 艘油轮列入黑名单 霍尔木兹海峡紧张升级](#item-finance-news-8) ⭐️ 8.0/10
9. [英伟达二季度财报：AI 数据中心芯片需求或支撑营收增长](#item-finance-news-9) ⭐️ 8.0/10
10. [壳牌据悉寻求以最高 80 亿美元出售美国化学品业务](#item-finance-news-10) ⭐️ 8.0/10
11. [巴菲特的继任者逆势建仓航空股，规模达 54 亿美元](#item-finance-news-11) ⭐️ 8.0/10
12. [通胀升至 2.9% 加息担忧加剧](#item-finance-news-12) ⭐️ 8.0/10
13. [厦门消杀公司被曝用敌敌畏服务连锁餐厅 多部门介入调查](#item-finance-news-13) ⭐️ 7.0/10
14. [Hugging Face 探索出售，估值或达 130 亿美元](#item-finance-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [MS Paint 与照片应用被曝为本地 AI 图像隐加 GUID 水印](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

据外部分析，微软画图（MS Paint）和照片（Photos）应用会在用户使用 AI 处理图像时，向即使完全在本地生成的输出中静默嵌入不可见的 GUID 水印，且无法关闭；可见水印则可由用户关闭。该 GUID 可能关联到 Microsoft 账户，进而引发隐私与匿名性担忧。目前尚不明确普通的 AI 背景删除等功能是否也会触发该水印。由于水印嵌入过程没有用户提示，用户可能在不知情的情况下分享带有唯一标识符的图像。

hackernews · ComputerGuru · 8月24日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=49421158)

**「背景」** Microsoft Paint 和 Photos 近年加入了基于本地模型的 AI 图像编辑功能，但这些功能并非完全离线：在本地生成 AI 图像之前，应用会向 Microsoft Azure Front Door 端点发起一次强制远程审核请求，并接收一个服务器签发的 16 字节 GUID。逆向工程分析显示，这个 GUID 会被作为不可见水印嵌入到图像的像素中，即使图像完全由本地模型生成且未上传到微软服务器，也无法通过用户设置关闭。

**「影响」** 对于在 Windows 上使用画图或照片应用进行 AI 编辑并分享图像的用户，这种不可见 GUID 水印可能使微软或通过法律程序获取数据的第三方，将图像关联到用户的姓名、地址、邮箱和电话等账户信息，从而削弱互联网匿名性。不过，具体触发条件和数据保留范围仍不明确。

**「社区讨论」** 有评论者认为 AI 话题是干扰项，真正的问题在于软件在用户不知情的情况下为每张图像添加唯一标识符，可能被用于版权追查或破坏匿名性；另有人提到微软曾在 Azure DevOps 错误地为非 AI 提交添加 Copilot 水印，并有人报告此功能误触发，因此建议谨慎使用相关应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as ...</a></li>
<li><a href="https://mangodeveloper.com/articles/microsoft-paint-embeds-invisible-guid-watermarks-in-local-ai-images-via-remote-moderation-server">Microsoft Paint Embeds Invisible GUID Watermarks in Local AI ...</a></li>
<li><a href="https://elsolitario.org/en/2026/08/24/microsoft-paint-invisible-guid-watermark/">Invisible Watermark in Microsoft Paint: How It Works</a></li>

</ul>
</details>

**标签**: `#privacy`, `#watermarking`, `#microsoft`, `#ai`, `#content-provenance`

---

<a id="item-tech-news-2"></a>
### [seL4 在 AArch64 完成安全证明，覆盖单核且非 MCS](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 8.0/10

Proofcraft Systems 于 2026 年 8 月 21 日宣布，seL4 微内核的安全证明已在 AArch64 架构上完成，这是形式化验证领域的一个重要里程碑。该成果覆盖的是非 MCS（混合关键性系统）配置，且仅支持单核（unicore），不包含多核与混合关键性扩展。对于依赖 ARM 平台的安全关键系统，这一证明为后续构建更高置信度的可信基座提供了基础。社区普遍认可其技术分量，但也提醒当前证明范围存在明确限制。

hackernews · snvzz · 8月24日 11:32 · [社区讨论](https://news.ycombinator.com/item?id=49418255)

**「背景」** seL4 是一个以形式化验证著称的开源微内核，其安全属性通过机器可检查的数学证明加以保障。此次 Proofcraft 在 UK NCSC 支持下，完成了 seL4 在 AArch64（64 位 ARM）架构上的机密性证明，补全了该架构安全隔离证明的最后一块，使运行于 seL4 上的应用在数学上被保证无法越权访问信息。这类经过机器验证的证明在量产操作系统中非常罕见，此次成果将已验证的保证扩展到了 Arm 64 位硬件。

**「影响」** seL4 在 AArch64 上完成形式化安全证明，使其经过机器检验的保证扩展到 64 位 ARM 硬件，对依赖 ARM64 处理器的高保障操作系统和关键任务系统具有直接意义。由于该架构广泛用于现代服务器与嵌入式系统，这一进展为相关基础设施和使命关键系统提供了更高级别的可靠性保障。

**「社区讨论」** 评论者一方面肯定该成就，另一方面指出“非 MCS”“单核”等限制，并有人预测侧信道定时攻击可能使结果失效，显示对形式化证明实用边界的审慎态度。讨论还涉及实际使用 seL4 的系统，如 GenodeOS、LionsOS，以及某中国车企将其用作车载 hypervisor 的案例；有评论认为嵌入式与军工市场会继续资助这类工作，但若想真正以能力模型改善系统安全，仍需提供原生 seL4/Linux。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/sel4-microkernel-achieves-full-formal-security-verification-on-aarch64">seL4 Microkernel Formal Security Proofs Completed on AArch64 ...</a></li>
<li><a href="https://zeli.app/story/49418255">seL4 security proofs now complete on AArch64 | Zeli</a></li>
<li><a href="https://www.newswarden.com/story/sel4-security-proofs-complete-aarch64">The seL4 Microkernel&#x27;s Security Proofs Are Now Complete on ...</a></li>
<li><a href="https://news.linxi.com.au/news/sel4-microkernel-achieves-full-formal-security-verification-on-aarch64">seL4 Microkernel Formal Security Proofs Completed on AArch64 ...</a></li>
<li><a href="https://www.newswarden.com/story/sel4-security-proofs-complete-aarch64">The seL4 Microkernel&#x27;s Security Proofs Are Now Complete on ...</a></li>

</ul>
</details>

**标签**: `#seL4`, `#formal verification`, `#microkernel`, `#AArch64`, `#security`

---

<a id="item-tech-news-3"></a>
### [可执行文件即 SQLite 数据库](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database) ⭐️ 8.0/10

这篇文章提出一项新颖思路：将可执行文件视为（或嵌入）SQLite 数据库，从而可以用 SQL 查询和修改二进制结构与元数据。作者 setheron 还介绍了 SQLite 的虚拟表机制，可把文件系统等外部数据“挂载”为数据库，并讨论了 ELF 格式本身已具备数据库特征的观点。文章在 Hacker News 获得 90 条评论和 480 分，社区讨论热烈，尤其关注这种设计对“胖二进制”、自修改程序镜像和替代 AppImage 等场景的潜力。

hackernews · setheron · 8月24日 04:48 · [社区讨论](https://news.ycombinator.com/item?id=49415271)

**「背景」** SQLite 是常见的嵌入式关系数据库，数据以单一文件保存；其文件格式在第 68 字节处预留了 4 字节的 application ID 字段，而 ELF 是 Linux 下通用的可执行文件格式。SQLite 还支持虚拟表机制，让外部数据源（如文件系统）可以像普通表一样被 SQL 查询。这篇文章提出的模式是把 SQLite 文件本身当作可执行文件：将 application ID 设为 &\#x27;SELF&\#x27;，使二进制文件的段与元数据都能用 SQL 查询和改写。

**「社区讨论」** 评论整体非常积极：有读者表示长期想实现类似想法，希望用 WebAssembly 与原生代码混合构建可按机器条件交换的胖可执行文件；也有人惊叹 SQLite 虚拟表可“挂载”文件系统，并设想把自修改的 Lisp 镜像、内建虚拟文件系统和运行时表放进同一文件。作者回应称，该想法在学术圈反馈并不友好，但在 HN 社区获得更多共鸣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database">Your executable is a SQLite database | Farid Zakaria’s Blog</a></li>
<li><a href="https://simonwillison.net/2026/Aug/24/your-executable-is-a-sqlite-database/">Your executable is a SQLite database - simonwillison.net</a></li>
<li><a href="https://system.data.sqlite.org/home/raw/244b0fe4a60f95f5fec80370e45344d4bf0e8ed5?at=vtab.html">The Virtual Table Mechanism Of SQLite - system.data.sqlite.org</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#executable-format`, `#elf`, `#database`, `#software-engineering`

---

<a id="item-tech-news-4"></a>
### [AI 编程依赖或致专业能力退化](https://larsfaye.com/articles/ai-coding-will-prevent-expertise) ⭐️ 7.0/10

一篇观点文章警告，重度依赖 AI 编程助手会使开发者难以形成深厚专业能力，相关讨论在社区引发热烈回应。有评论指出，企业中已出现“手工写代码就是错的”这类管理指令，导致代码产出速度快于人类理解和审查的速度。另一些开发者则强调，采用引导式编码（guided coding）而非完全放任的“氛围编程”，仍能兼顾生产效率与代码质量，并认为刻意保留“摩擦”对长期技能形成很重要。目前这些更多是实践层面的担忧与经验分享，尚无系统性证据证明专业能力必然崩溃。

hackernews · larsfaye · 8月24日 15:52 · [社区讨论](https://news.ycombinator.com/item?id=49421554)

**「背景」** Lars Faye 在文章《AI Coding will Prevent Expertise》中提出，开发者如果过度依赖 AI 编程助手和智能体工作流，将难以形成深度专业技能，并可能产生“认知债务”与技能退化。文中还讨论了从开发者转向“AI 编排者”的趋势，以及这种转变可能导致软件质量与人工审查能力之间的张力。

**「影响」** 如果企业普遍将“手动写代码”视为低效并强制推行 AI 辅助，开发者可能面临更多难以被自己或他人完整理解的代码，同时削弱新手建立深层技能的机会；不过这一影响目前仍属于预测性观点，需要更长期观察。

**「社区讨论」** 评论中既有认同“专业能力下降”的声音，也有反对者认为关键在于使用方式：引导式编码可以在保持质量的同时提升效率，而“刻意摩擦”对技能养成依然重要。还有观点调侃“停止做某事，某事的能力就会下降”，以及对 AI 编程“蛇吞尾巴”式循环表示担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://larsfaye.com/articles/ai-coding-will-prevent-expertise">AI Coding will Prevent Expertise | Lars Faye</a></li>
<li><a href="https://digg.com/ai/dyuzij5t">larsfaye . com article states agentic coding creates cognitive debt and...</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#LLM`, `#expertise`, `#code generation`

---

<a id="item-tech-news-5"></a>
### [“Bart”：以 1931 年前英文训练的开源复古 LLM](https://www.reddit.com/r/MachineLearning/comments/1vx94er/bart_a_vintage_llm_r/) ⭐️ 7.0/10

Unbounded Labs 发布了 Bart（又称 Bartholomew），一个 2.82B 参数的“复古 LLM”，从零开始在 20.1B token 的 1931 年前英文语料上训练，总成本约 807 美元，最终模型在单张 H100 上耗时 5 天完成训练，并保持 60% 的模型浮点利用率（MFU）。发布方称，Bart 是其规模下最好的复古基座模型，在自建的 Vintage CORE 基准上以更小的 token 预算超过了 GPT-1900。团队还开源了清洗后的哈佛机构藏书数据集（从 242B token 清理至 23B token）、首个复古 LLM 基准套件 Vintage CORE（含 20 个基准）、416k 对基于 1930 年前文本的监督微调数据，以及完整的数据集、方法、训练代码、评估和训练记录。整个项目由团队自掏腰包完成，目前正在寻求算力资助、资金和导师支持。

reddit · r/MachineLearning · /u/soggydoggy8 · 8月24日 17:20

**「背景」** 常规大语言模型通常使用现代网络文本进行预训练，而 Bart 的特殊之处在于其训练语料严格限定为 1931 年之前的英文文本。这一项目的灵感来自 Demis Hassabis 提出的设想：LLM 是否可能独立得出过去伟大科学家曾得出的结论，从而帮助检验模型是否具备真正的原创推理能力，而非仅仅进行下一个 token 的预测。

**「影响」** 对于研究复古/历史文本语言模型、历史科学推理或高效预训练的研究者和开发者而言，Bart 项目提供了可复现的开放资源：包括最大的复古 SFT 数据集、Vintage CORE 基准套件、训练代码和实验记录，便于验证和扩展这一方向的方法；不过该项目规模较小，尚未达到行业里程碑级别。

**标签**: `#language-models`, `#ai-research`, `#training-runs`, `#historical-text`, `#llm-evaluation`

---

<a id="item-tech-news-6"></a>
### [AI 空间软件生成器：可编程 3D 对象](https://www.reddit.com/r/MachineLearning/comments/1vxcc1h/r_using_ai_as_a_spatial_software_generator_to/) ⭐️ 7.0/10

一项研究提出用大语言模型生成三维对象作为“空间软件”，而非传统静态网格，作者称这类对象从诞生起就具备可编程逻辑，如动画就绪、层次结构、铰接关节以及根据弱计算环境（如移动端）与强计算环境（如复杂游戏引擎）自动调整显示形式。演示与代码发布在 nova3d.xyz 和 GitHub 仓库；作者也承认在复杂有机形状生成上仍落后于传统 AI 3D 生成器。该提交由共同作者自行发布，目前尚缺独立验证。作者认为工业设计、游戏开发、模拟和 AR/VR/XR 行业最可能受到冲击。

reddit · r/MachineLearning · /u/mhb\_11 · 8月24日 19:10

**「背景」** 传统 AI 3D 生成器通常输出无法直接编辑或复用的单体网格，导致动画、关节和场景适配需要额外离线处理。这项研究探索的是让大语言模型直接编写空间程序，使 3D 对象以软件形式存在，从而在创作时就把结构、逻辑和自适应行为内建进去。

**「影响」** 如果该方向成立，3D 内容生产将从生成静态模型转向生成天然可编程的可交互对象，可能减少游戏开发、工业设计和 XR 场景中的后期加工成本；不过复杂有机形状的差距和缺乏独立验证意味着落地仍需时间。

**标签**: `#AI`, `#3D generation`, `#spatial programming`, `#machine learning`, `#computer graphics`

---

<a id="item-tech-news-7"></a>
### [小米发布三款玄戒芯片，AI 旗舰 SoC 首搭小米 18 Fold](https://mp.weixin.qq.com/s/ceIQbNnZrcNQqGywXCiXTQ) ⭐️ 7.0/10

小米发布新一代玄戒芯片，包括 AI 旗舰 SoC 玄戒 O3、高带宽 AI 加速芯片玄戒 O100 和国内首款 3nm 智驾 AI 芯片玄戒 D100，三款均完成回片验证，覆盖人车家全生态端侧 AI 算力需求。玄戒 O3 采用十核全大核 CPU，多核跑分首破 15000 分，GPU 首发 G2-Ultra NX，性能提升 85%、功耗降低 64%，并成为全球首个支持 LPDDR6 的移动处理器，带宽 113.8GB/s，NPU 端侧 AI 性能提升 45%。玄戒 D100 采用 3nm 工艺，集成 20 核 CPU 与 16 核 NPU，最高支持 160GB 统一内存，可本地部署 200B 参数大模型，计划明年商用。玄戒 O100 采用行业首款 6nm 晶圆级垂直堆叠先进封装与 Hybrid Bonding 混合键合工艺，键合间距 1.4 微米，提供 1.22TB/s 超高带宽和最高 330TPS 端侧推理速度。这些芯片显示小米在端侧 AI 和智驾高算力领域的布局，其中 AI 旗舰 SoC 将首发搭载于小米 18 Fold。

telegram · zaihuapd · 8月24日 07:18

**「背景」** 玄戒（Xuanjie）是小米自研芯片产品线，此前主要用于手机端 SoC。据小米官方介绍，团队在自研芯片赛道已深耕五年多，此次发布的新一代玄戒芯片不再限于手机：玄戒 O3、O100、D100 分别瞄准移动终端、大模型加速与智能驾驶三大场景。三款芯片均已完成回片验证，被视为小米自研芯片从手机 SoC 向人车家全生态 AI 算力底座扩展的一步。

**「影响」** 玄戒 O3 将首发搭载于小米 18 Fold，玄戒 D100 计划明年商用，这为小米手机和智驾车型带来更高的端侧 AI 算力与本地大模型部署能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/993/535.htm">小米玄戒三芯集结：O3 开启规模量产、O100 和 D100 研发完成明年商用 ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260824A0BU0800">小米发布三款玄戒AI芯片：O3跑分破522万，O100/D100明年商用</a></li>
<li><a href="https://www.chinaz.com/ainews/30572.shtml">小米发布玄戒O3/O100/D100三款自研AI芯片，搭建人车家全生态算力底座</a></li>

</ul>
</details>

**标签**: `#Xiaomi`, `#SoC`, `#AI accelerator`, `#semiconductors`, `#automotive chip`

---

<a id="item-tech-news-8"></a>
### [阿里云 Wan3.0 上线：30 秒视频 API 最低 0.3 元/秒](https://mp.weixin.qq.com/s/peeeU6cBz4AaROvFe1zqQQ) ⭐️ 7.0/10

阿里云 Wan3.0 视频生成模型今日正式上线，支持最长 30 秒视频生成，官方强调其在人物质感、参考一致性和非写实风格化方面的表现。用户可在阿里云百炼、万相官网、千问 APP 等平台体验。API 按分辨率计价：480P、720P、1080P 分别为 0.3、0.6、1.2 元/秒。8 月 24 日至 9 月 23 日，阿里云百炼和千问 AI 平台开启 API 限时 7 折优惠。这为开发者和企业提供了新的可集成视频生成选项，但公告未包含更深层的技术参数与基准测试。

telegram · zaihuapd · 8月24日 10:14

**「背景」** Wan3.0 是阿里云万相（Wan）系列的最新视频生成模型，目前已上线阿里云百炼（Model Studio），支持文生视频、图生视频（首帧/首尾帧）以及基于参考的视频生成，可生成最长 30 秒的视频。阿里云在推出该模型前一天刚完成了一笔 102 亿美元的股份发行，用于资助其 AI 扩张，因此 Wan3.0 被视作其在 AI 视频生成领域的重要布局。

**「影响」** 对开发者与 AI 工程师而言，阿里云 Wan3.0 API 以 0.3 元/秒（480P）的起步价和 8 月 24 日至 9 月 23 日的 7 折优惠，提供了生成最长 30 秒视频的低成本调用方式；结合公开的 2025 年 AI 视频生成模型定价与基准对比，这将直接影响企业在选择视频生成 API 时的成本评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.yahoo.com/ai/articles/alibaba-wan3-0-ai-video-174537190.html">Alibaba Wan3.0 AI video model launch: 30-second video generation</a></li>
<li><a href="https://www.alibabacloud.com/blog/wan3-0-30-second-ai-video-generation-from-any-input_603452">Wan3.0: 30-Second AI Video Generation from Any Input</a></li>
<li><a href="https://aifreeforever.com/blog/best-ai-video-generation-models-pricing-benchmarks-api-access">17 Best AI Video Generation Models Pricing, Benchmarks &amp; API ...</a></li>

</ul>
</details>

**标签**: `#video generation`, `#Alibaba Cloud`, `#API`, `#AI model`, `#Wan3.0`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储维持利率不变：9 比 3 投票结果](https://news.google.com/rss/articles/CBMipwFBVV95cUxPQnEyZnQ5dWh6NGJkdk0wNGlXY3NfSWswOWhlZmp0Y1lUSnhqdjl6VGVoWkR3OHNOdWs1YVZJaWVIS2xxd1dlMWtkU2kwRFplX25PU3pldS14c1BYeS1WSkU2cVBxUXpDNFV2eFk2YXZoTDh5ajRsT216Sk91cXMzaGFvTkF1TnI3ajFLdnNETk5HRF9IY1BUTmwyRFZkVi0tbWp0d2Nvd9IBrAFBVV95cUxOeUItMlRiT0NXQjFoZS0xMndmWUpHOTNsM0ZabWJkZ0JRMEZxb0ZvLXVkTWEydk1KRlRGSXhYUWNvc3dHSjNsRmp1OEtrLXpDdERCVnBuUXlLNXdXWnFJeXhOOV9Hdk5OTjByeVBMZkRGWTc3TmFNb0pkZmU4Zkd4ZHZYRndvQXdIby1uUHJsQUpvcEw2OC01UFRrWEszNVhxdDJxbXEtZzV0c3pZ?oc=5) ⭐️ 9.0/10

美联储在 9 比 3 的投票中决定维持利率不变，据 ABC7 洛杉矶报道。

google\_news · ABC7 Los Angeles · 7月29日 07:00

**「背景」** 美联储在 9 比 3 的投票中决定维持利率不变，将联邦基金利率保持在 3.5%至 3.75%区间，这一利率水平自 1 月以来一直未变；三名委员投票支持加息，市场普遍预期 9 月会议可能加息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>
<li><a href="https://abc7news.com/post/federal-reserve-is-expected-keep-rates-unchanged-now-despite-high-prices/19595693/">Federal Reserve leaves interest rate unchanged in 9-3 vote - ABC7 San Francisco</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-2"></a>
### [美联储连续第五次会议维持利率不变](https://news.google.com/rss/articles/CBMinwFBVV95cUxNbVA1MzJGNXllN1RjSG43b0xUam1seWRjUmI2bHdXdlZndHhEQ1pRZDI5WVE3MGg1NnBCMk9Gcm42MUZab29ZRFY3OTd3OTZERlZmLUtFbGhUOG5jQXlDREFuMGVkSmtyTlJvVzJhS1A0OG5zaGhWZkZ1VHlQRXNGcGcxczNOMW82ckdRdVJmRUZzRDI4OEV4SHRfSjh6Wms?oc=5) ⭐️ 9.0/10

美联储连续第五次会议决定维持利率不变，凸显出政策制定者对通胀持续的担忧。

google\_news · NBC News · 7月29日 07:00

**「背景」** 美联储已连续第五次会议将基准利率维持在 3.75%，主席凯文·沃什表示需等待更明确的通胀和经济趋势后再调整政策。目前通胀仍高于美联储 2%的目标，且本次会议有三位官员投反对票，显示出决策层对下一步行动存在分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.benzinga.com/markets/economic-data/26/07/60773453/fed-meeting-decision-interest-rates-july-2026">Fed Holds Rates at 3.75%, But Three Members Voted to... - Benzinga</a></li>
<li><a href="https://www.livemint.com/market/stock-market-news/us-federal-reserve-holds-rates-steady-for-fifth-consecutive-meeting-11785346712831.html">US Federal Reserve holds rates steady for fifth consecutive ...</a></li>
<li><a href="https://english.ajel.sa/business/orl7sxcp3">US Fed holds rates steady, markets eye September... — Ajel English</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#economy`

---

<a id="item-finance-news-3"></a>
### [美联储面临多年来最不可预测的会议](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 9.0/10

据《华尔街日报》报道，美联储即将召开的会议被形容为多年来最不可预测的会议之一，可能涉及重大货币政策调整。目前报道未给出具体的利率目标或政策方向。

google\_news · WSJ · 7月23日 07:00

**「背景」** 美联储的联邦公开市场委员会（FOMC）每年定期举行八次会议。据《华尔街日报》报道，下周的会议因油价冲击和主张加息的力量与更温和的通胀数据相互碰撞，正成为多年来最难以预测的会议之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm?embed=true">The Fed - Meeting calendars and information - Federal Reserve Board</a></li>
<li><a href="https://www.wsj.com/economy/central-banking/the-fed-is-heading-into-one-of-its-most-unpredictable-meetings-in-years-849198f5">The Fed Is Heading Into One of Its Most Unpredictable Meetings in Years</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#markets`

---

<a id="item-finance-news-4"></a>
### [胡塞武装袭击沙特红海油轮](https://oilprice.com/Geopolitics/Middle-East/Houthis-Target-Saudi-Oil-Tanker-in-Red-Sea-Missile-and-Drone-Attack.html) ⭐️ 8.0/10

也门胡塞武装周一在红海延布附近海域用弹道导弹和无人机袭击了沙特油轮“Amzan”，沙特政府及沙特航运公司 Bahri 证实这艘船在地区水域遭遇敌对事件。

rss · OilPrice.com · 8月24日 20:00

**「背景」** 胡塞武装与沙特近期再次爆发冲突，胡塞武装已宣布对沙特航运实施“以围困回应围困”的海上限制，并声称将打击沙特军事集结；此前数周，沙特阿美设施已至少四次成为目标。红海及曼德海峡是全球关键的石油运输通道。

**标签**: `#oil tanker`, `#Red Sea`, `#Houthi attack`, `#Saudi Arabia`, `#oil supply risk`

---

<a id="item-finance-news-5"></a>
### [美国扩大对伊制裁但未点名中国大型银行](https://oilprice.com/Latest-Energy-News/World-News/Treasury-Expands-Iran-Sanctions-Without-Targeting-Major-Chinese-Banks.html) ⭐️ 8.0/10

美国财政部周一扩大对伊朗的“二级制裁”，首轮针对近 60 名个人、实体和船只，并把数字资产、科技、黄金、航空和航运列为新制裁领域，但没有直接点名制裁中国的大型银行。中国 8 月从伊朗进口的原油估计为每日 53.4 万桶，低于 7 月的 82.3 万桶。

rss · OilPrice.com · 8月24日 19:13

**「背景」** 中国购买伊朗超过 80%的海运原油；美国 7 月中旬重启封锁后，伊朗在波斯湾和阿曼湾以外的可用海上原油库存已从逾 1 亿桶降至约 8300 万桶。

**「影响」** 由于新制裁瞄准运输和销售伊朗原油的经纪商、企业及“影子船队”，中国等伊朗原油买家获得的供应可能进一步收紧；但大型中资银行暂未被切断美国金融体系准入，系统性冲击有限。

**标签**: `#Iran sanctions`, `#oil market`, `#Treasury`, `#China`, `#geopolitics`

---

<a id="item-finance-news-6"></a>
### [道达尔能源支持两条绕开霍尔木兹海峡的主要输油管道](https://oilprice.com/Latest-Energy-News/World-News/TotalEnergies-Backs-Two-Major-Oil-Pipelines-to-Bypass-Hormuz.html) ⭐️ 8.0/10

法国道达尔能源 CEO 周一表示，公司将投资两条绕开霍尔木兹海峡的输油管道：参与阿布扎比把富查伊拉出口管线运力翻倍，并支持一条从伊拉克经叙利亚到地中海的拟建管线；具体投资额和持股尚未披露。

rss · OilPrice.com · 8月24日 18:27

**「背景」** 在伊朗战争导致海峡油轮通行严重受阻后，道达尔能源两个月前已将投资替代海湾出口路线列为“绝对优先”；现有 Habshan-Fujairah 管道日输 180 万桶，走阿曼湾出口，无需经过海峡。

**「影响」** 若项目推进，伊拉克-叙利亚管道据估计耗资约 150 亿美元、至少 4 年建成，可为伊拉克原油提供地中海出口；阿布扎比则计划到明年让绕行能力翻倍，有助于缓解海湾原油出口的运输瓶颈。

**标签**: `#TotalEnergies`, `#Oil Pipelines`, `#Strait of Hormuz`, `#Energy Infrastructure`, `#Geopolitics`

---

<a id="item-finance-news-7"></a>
### [欧洲多国领导人齐聚基辅 讨论增强乌克兰防空](https://oilprice.com/Geopolitics/Europe/European-Leaders-Gather-in-Kyiv-as-Ukraine-Seeks-More-Air-Defense.html) ⭐️ 8.0/10

欧洲多国领导人 8 月 24 日在基辅出席“意愿联盟”会议，乌克兰借此寻求更多防空支持；英国同意防务企业 MBDA 公开 SCALP 导弹英方部件信息以探讨在乌设组装线，挪威则承诺明年提供 90 亿美元援助。泽连斯基还呼吁欧洲议会通过立法，以释放 300 亿欧元援乌资金。

rss · OilPrice.com · 8月24日 15:00

**「背景」** “意愿联盟”是由英法牵头的约 34 国非正式组织，此次会议正值乌克兰独立 35 周年，讨论焦点包括继续军援、防空和长期安全安排。

**「影响」** 英国政府放行 MBDA 分享英方部件信息，为 SCALP 导弹在乌克兰本地组装铺路，可能影响欧洲防务产业链布局。

**标签**: `#Ukraine`, `#air defense`, `#European aid`, `#geopolitics`, `#defense spending`

---

<a id="item-finance-news-8"></a>
### [伊朗将 45 艘油轮列入黑名单 霍尔木兹海峡紧张升级](https://oilprice.com/Energy/Energy-General/Iran-Blacklists-45-Tankers-as-Hormuz-Standoff-Escalates.html) ⭐️ 8.0/10

伊朗将 45 艘使用霍尔木兹海峡的油轮列入黑名单，威胁罚款、扣船和没收货物，以回应美国即将对伊实施的新一轮经济措施；该海峡通常承载全球约 20%的石油和 LNG 供应。

rss · OilPrice.com · 8月24日 14:00

**「背景」** 伊朗新设立的波斯湾海峡管理局称这些船只违反通行规则；伊朗此前已要求船只在过境前获得许可并支付安全等服务费。美国财长贝森特定于周一公布新一轮经济措施，伊朗周日威胁称若华盛顿推进，将阻止任何石油离开波斯湾。

**「影响」** Kpler 数据显示，周日仅有 4 艘商品船穿越海峡，英国海上贸易行动办公室估计 AIS 探测到的通行量较战前低约 90%；若黑名单扩大，依赖中东原油的亚洲买家将面临更严重的供应和运输风险。

**标签**: `#Strait of Hormuz`, `#Iran`, `#oil tankers`, `#geopolitics`, `#energy markets`

---

<a id="item-finance-news-9"></a>
### [英伟达二季度财报：AI 数据中心芯片需求或支撑营收增长](https://finance.yahoo.com/technology/ai/articles/nvidias-q2-earnings-ai-data-141300944.html) ⭐️ 8.0/10

报道预计，英伟达（NVIDIA）第二季度财报将受强劲的 AI 数据中心芯片需求提振，该需求有望助其营收增长。目前财报数据尚未公布。

openbb · NVDA · 8月24日 14:13

**「背景」** 英伟达（NVIDIA）第二季度业绩预计受益于人工智能数据中心芯片需求，主要因为企业和超大规模云服务商为训练和部署 AI 模型大规模采购英伟达 GPU；其新一代 Blackwell 和 Vera Rubin 平台因性能和能效优势获得客户采用。

**「影响」** 英伟达数据中心业务单季收入达 752 亿美元、同比增长 92%，显示云服务商和 AI 企业仍在大量采购用于训练和推理的 AI 芯片，这对 AI 基础设施供应链及数据中心设备相关行业具有直接拉动作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theglobeandmail.com/investing/markets/stocks/TSM/pressreleases/4004491/nvidias-q2-earnings-ai-data-center-chip-demand-to-aid-revenue-growth/">NVIDIA&#x27;s Q2 Earnings: AI Data Center Chip Demand to Aid Revenue Growth - The Globe and Mail</a></li>
<li><a href="https://www.tradingview.com/news/zacks:fa735f20d094b:0-nvidia-s-q2-earnings-ai-data-center-chip-demand-to-aid-revenue-growth/">NVIDIA&#x27;s Q2 Earnings: AI Data Center Chip Demand to Aid Revenue Growth — TradingView News</a></li>
<li><a href="https://techjournal.org/nvidia-record-earnings-ai-economy-2026">Nvidia&#x27;s $81.6B Quarter: What Record AI Chip Profits Tell Us About the ...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI`, `#Data Center`, `#Earnings`, `#Chip Demand`

---

<a id="item-finance-news-10"></a>
### [壳牌据悉寻求以最高 80 亿美元出售美国化学品业务](https://finance.yahoo.com/markets/stocks/articles/shell-seeking-buyers-u-chemicals-175341275.html) ⭐️ 8.0/10

据报道，壳牌正在为其美国化学品业务寻找买家，潜在交易估值最高约为 80 亿美元。该交易尚未完成，目前仍处于寻求买方的阶段。

openbb · BRK-B · 8月24日 17:53

**「背景」** 据媒体报道，壳牌（Shell）正为其美国化学品业务寻找买家，该业务估值可能高达 80 亿美元，涉及位于路易斯安那州、得克萨斯州和宾夕法尼亚州的四座工厂。据英国《金融时报》报道，埃克森美孚（Exxon Mobil）和利安德巴塞尔（LyondellBasell）等公司被视为潜在竞购方。

**「影响」** 若交易完成，这笔潜在出售将标志着壳牌退出美国化工业务，可能影响相关工厂的员工和所在社区；公司 CEO 已表示化工业务“回报不足”，壳牌正将重心转向液化天然气等利润更高的领域。行业层面，这也反映出化工企业为改善盈利而普遍进行的资产重组。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/shell-seeking-buyers-u-chemicals-175341275.html">Shell seeking buyers for U.S. chemicals business at up to $8 billion</a></li>
<li><a href="https://www.fool.com/investing/2026/08/24/exxonmobil-is-eyeing-an-8-billion-bet-on-shells-us-chemical-plants-heres-what-it-means-for-xom-stock/">ExxonMobil Is Eyeing a Potential $8 Billion Bet on Shell&#x27;s U.S. Chemical Plants. Here&#x27;s What It Means for XOM Stock. | The Motley Fool</a></li>
<li><a href="https://www.tradingpedia.com/2026/08/24/shell-asset-sale-draws-exxon-lyondell-and-more/">Shell Asset Sale Draws Exxon, Lyondell, And More</a></li>
<li><a href="https://inspectioneering.com/news/2025-03-05/11479/wsj-reports-shell-is-considering-divesting-chemicals-assets-in-us-and-europe">Shell Mulls Sale of Chemicals Assets in U.S. and Europe</a></li>
<li><a href="https://cen.acs.org/business/petrochemicals/Shell-pull-back-chemicals/103/web/2025/03">Shell to pull back from chemicals - C&amp;EN</a></li>
<li><a href="https://www.chemanalyst.com/NewsAndDeals/NewsDetails/shell-considers-selling-us-and-european-chemical-assets-to-focus-on-profits-34927">Shell Considers Selling U.S. and European Chemical Assets to Focus on Profits</a></li>

</ul>
</details>

**标签**: `#Shell`, `#chemicals`, `#divestiture`, `#M&amp;A`, `#energy`

---

<a id="item-finance-news-11"></a>
### [巴菲特的继任者逆势建仓航空股，规模达 54 亿美元](https://finance.yahoo.com/markets/stocks/articles/warren-buffett-called-airlines-worst-142928918.html) ⭐️ 8.0/10

巴菲特曾称航空业是“最糟糕的生意”，而其继任者却已建立约 54 亿美元的航空股仓位。

openbb · BRK-B · 8月24日 14:29

**「背景」** 格雷格·阿贝尔是沃伦·巴菲特在伯克希尔·哈撒韦的长期继任者，自 2026 年 1 月起出任首席执行官；而巴菲特曾公开把航空业称为“最糟糕的生意”，因此阿贝尔如今建立 54 亿美元航空股仓位与这一判断形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Greg_Abel">Greg Abel - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Berkshire Hathaway`, `#Airlines`, `#Investment Strategy`, `#Greg Abel`, `#Equities`

---

<a id="item-finance-news-12"></a>
### [通胀升至 2.9% 加息担忧加剧](https://news.google.com/rss/articles/CBMijAFBVV95cUxNU2Vib0FIUXVTS2ZiZlBXbkxpdjNTVWRSaU5nQjE4ZktjOFlGTkdFWGFPeU1oQUhwSWViUWYybllXWHNOb1VwSzlMQXdscHd6eHlLX2NZbjVSRWIwRjhERGctOUVSMGRJUDFDYkhZcjM4a0dvUVhsYnVBdGtlYmlkRlU4WU81RmpyQjFYdg?oc=5) ⭐️ 8.0/10

据《福布斯》报道，通胀率升至 2.9%，加剧了市场对央行可能很快加息的担忧。

google\_news · Forbes · 8月19日 11:50

**「背景」** 据《福布斯》报道，美国通胀率升至 2.9%，高于美联储 2%的目标，引发市场对再次加息的担忧。美联储 7 月会议纪要显示，多名官员认为如果通胀不回落可能需要加息；目前联邦基金利率维持在 3.5%至 3.75%，下次决策会议在 9 月。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=CPd9PB6ki-k">Fed Minutes Show Many Officials Wanted a Rate Hike - YouTube</a></li>
<li><a href="https://www.rrfn.com/2026/08/20/an-interest-rate-hike-in-september/">An Interest Rate Hike in September? | Red River Farm Network</a></li>

</ul>
</details>

**标签**: `#inflation`, `#interest rates`, `#Federal Reserve`, `#monetary policy`, `#economy`

---

<a id="item-finance-news-13"></a>
### [厦门消杀公司被曝用敌敌畏服务连锁餐厅 多部门介入调查](https://mp.weixin.qq.com/s/f5OHkMhtZBbcHrSSFJZVMA) ⭐️ 7.0/10

新京报调查发现，厦门绿林森环境科技有限公司长期使用高毒杀虫剂敌敌畏，为绿茶、先启半步颠等数十家连锁餐厅进行消杀，员工曾把原液装入矿泉水瓶并撕掉标签；目前厦门多部门已介入调查。

telegram · zaihuapd · 8月24日 02:14

**「背景」** 敌敌畏（DDVP）是一种有机磷杀虫剂，毒性较强，吸入、误食或皮肤接触都可能引起中毒，按规定不得用于可能污染食品和饮用水的环境。调查还显示，该公司在监管部门介入当晚表面改用合规药“残杀威”，实际仍在用敌敌畏。

**「影响」** 曾由该公司消杀服务的数十家连锁餐厅及其顾客，可能面临农药残留带来的食品安全风险，相关门店也可能受到监管和声誉影响。

**标签**: `#food safety`, `#pesticide`, `#restaurant industry`, `#regulatory investigation`, `#company scandal`

---

<a id="item-finance-news-14"></a>
### [Hugging Face 探索出售，估值或达 130 亿美元](https://www.bloomberg.com/news/articles/2026-08-23/hugging-face-gauging-interest-for-potential-sale-business-insider-says) ⭐️ 7.0/10

据 Business Insider 援引知情人士报道，AI 模型托管平台 Hugging Face 正探索出售，估值可能达 130 亿美元或更高，相比 2023 年融资时 45 亿美元的估值明显提高；公司已与银行合作评估买家兴趣，目前尚未达成交易。

telegram · zaihuapd · 8月24日 05:45

**「背景」** Hugging Face 是一家 2016 年创立的机器学习模型分享与部署平台，也是开发者常用的开源 AI 社区。该公司 2023 年完成 2.35 亿美元融资后，估值约为 45 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tracxn.com/d/companies/hugging-face/___89yhA9z0-ZrLstW87xWDVe15Bkl70IZOkQf38SXzmQ">Hugging Face - 2026 Company Profile, Team, Funding ... - Tracxn Hugging Face – Funding, Valuation, Investors, News Hugging Face 2026 Company Profile: Valuation, Funding ... Hugging Face: Valuation, Funding &amp; Metrics | Sterling Hugging Face reportedly in talks to be acquired for $13B Hugging Face Valuation, Funding &amp; IPO Status 2026 — WOWLS Hugging Face Funding: How Much Did They Raise &amp; Key Investors</a></li>

</ul>
</details>

**标签**: `#AI`, `#M&amp;A`, `#Hugging Face`, `#Valuation`, `#Tech`

---