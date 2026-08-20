---
layout: default
title: "Horizon Summary: 2026-08-21 (ZH)"
date: 2026-08-21
lang: zh
---

> 从 237 条内容中筛选出 24 条重要资讯。

---

**科技新闻**
1. [GitHub 8 月 17 日故障复盘](#item-tech-news-1) ⭐️ 8.0/10
2. [AliExpress 静默 WebAudio 指纹识别被曝破坏蓝牙多设备连接](#item-tech-news-2) ⭐️ 8.0/10
3. [恶意 Rust crate arrayref 在构建时执行载荷](#item-tech-news-3) ⭐️ 8.0/10
4. [陶哲轩警告 AI 或引发数学界最大危机](#item-tech-news-4) ⭐️ 8.0/10
5. [125M 参数 Transformer 实现 iPhone 端实时钢琴自动补全](#item-tech-news-5) ⭐️ 7.0/10
6. [Linux 7.2 发布：AMD 开源驱动新增 HDMI 2.1 支持](#item-tech-news-6) ⭐️ 7.0/10
7. [谱神经元：一种可扩展可解释的机器学习原语](#item-tech-news-7) ⭐️ 7.0/10
8. [OpenAI 预览零数据留存与私密安全处理](#item-tech-news-8) ⭐️ 7.0/10
9. [反向查询服务泄露数百万张面部照片](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [恒大及许家印案一审宣判：许家印获无期徒刑](#item-finance-news-1) ⭐️ 9.0/10
2. [美联储维持利率不变，为伊朗战争推高油价后首次决策](#item-finance-news-2) ⭐️ 9.0/10
3. [美联储会议不确定性升高](#item-finance-news-3) ⭐️ 9.0/10
4. [美联储维持利率不变，保留未来加息可能](#item-finance-news-4) ⭐️ 9.0/10
5. [英国央行发布 2026 年 7 月《货币政策报告》](#item-finance-news-5) ⭐️ 9.0/10
6. [胡塞武装计划扩大曼德海峡控制，沙特部分石油出口改道](#item-finance-news-6) ⭐️ 8.0/10
7. [美国提前放开冬季级汽油销售以缓解高油价](#item-finance-news-7) ⭐️ 8.0/10
8. [中国在扩大可再生能源的同时继续增产油气](#item-finance-news-8) ⭐️ 8.0/10
9. [阿里巴巴第一财季净利 105.37 亿元，同比下滑 76%](#item-finance-news-9) ⭐️ 8.0/10
10. [AMD 股价因谷歌扩大定制芯片计划下跌](#item-finance-news-10) ⭐️ 8.0/10
11. [博通据报寻求超 600 亿美元债务融资用于 AI 投资](#item-finance-news-11) ⭐️ 8.0/10
12. [Broadcom 寻求逾 600 亿美元债务融资用于 AI 项目](#item-finance-news-12) ⭐️ 8.0/10
13. [台积电上调资本支出预测至 850 亿美元，ASML 股价上涨](#item-finance-news-13) ⭐️ 8.0/10
14. [台积电 2027 年资本支出预测达 850 亿美元，股价上涨](#item-finance-news-14) ⭐️ 8.0/10
15. [Stripe 同意收购 OpenRouter](#item-finance-news-15) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GitHub 8 月 17 日故障复盘](https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/) ⭐️ 8.0/10

GitHub 于 8 月 17 日发生服务故障，并在事后公布了详细复盘。故障根源是单个内部端点响应延迟，而客户端重试循环和 VS Code 中一个潜在的重试缺陷将流量放大至约 10 倍，导致 Copilot Token Service 恢复延迟。GitHub 还披露，自 4 月以来月提交量从 14 亿增至 29 亿，凸显了规模增长带来的可靠性压力。公司表示将推进一系列可靠性改进，以降低类似事件再次发生的风险。

hackernews · 0xedb · 8月20日 19:22 · [社区讨论](https://news.ycombinator.com/item?id=49378957)

**「背景」** GitHub 是广泛使用的代码托管与协作平台，Copilot Token Service 用于管理 GitHub Copilot 的授权令牌。8 月 17 日的故障源于内部服务响应延迟，并由客户端重试进一步放大，最终影响了依赖该服务的功能。

**「影响」** GitHub Copilot 用户在故障期间可能因 Token 服务恢复延迟而受到影响；GitHub 表示将推进可靠性改进以减少类似事件。

**「社区讨论」** 评论者对故障原因展开讨论：有的批评服务方倾向于向用户隐藏错误、导致用户长时间等待；有的认可 GitHub 在免费且无广告的情况下提供大规模服务。另有人惊叹月提交量从 14 亿增至 29 亿的快速增长，并质疑客户端重试机制是否合理。

**标签**: `#outage`, `#reliability`, `#github`, `#retry-bugs`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [AliExpress 静默 WebAudio 指纹识别被曝破坏蓝牙多设备连接](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) ⭐️ 8.0/10

一篇博客文章披露，AliExpress（速卖通）网页会执行静默 WebAudio 指纹识别，并因此破坏蓝牙多设备连接（multipoint），导致部分用户的蓝牙耳机或汽车音响出现异常。多个用户在评论区报告了类似经历：访问网站或使用 App 后蓝牙音频行为改变，甚至让汽车认为收到语音指令；有人指出 Firefox 等浏览器已在缓解 WebAudio 指纹识别。该现象既涉及隐私追踪技术，也造成实际功能干扰，对重视隐私和音频连接的用户具有现实影响。

hackernews · emctech · 8月20日 10:08 · [社区讨论](https://news.ycombinator.com/item?id=49372583)

**「背景」** WebAudio 指纹识别是一种利用浏览器音频处理 API 提取设备硬件或软件特征的技术，通常以不可闻的方式运行。AliExpress 的反滥用脚本创建了连接到音频输出且增益为零的隐藏 WebAudio 图，这会持续占用系统音频通道，从而阻止支持多点连接的蓝牙耳机自动切换到其他已连接设备（如手机）。这种静默音频方案既构成隐私追踪手段，也会造成实际的功能干扰。

**「影响」** 根据用户报告，打开 AliExpress 网页会触发静音音频流，导致电脑与耳机之间的蓝牙多点连接持续占用链路，从而阻断手机音频，影响依赖蓝牙多点连接的用户；同时，该静音行为与 WebAudio 指纹追踪技术相关，可能进一步带来隐私风险。

**「社区讨论」** 评论区中，多位用户确认阿里系应用或网站会触发蓝牙异常：有人发现 iPhone 上后台运行 AliExpress 会让汽车音响误判收到语音指令，还有人注意到旧款助听器的环境噪声放大被网站访问改变。另有评论提到 Firefox 已对 WebAudio 指纹识别进行缓解，并有人质疑苹果对恶意应用的应用商店审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.elseif.net/stories/aliexpress-runs-silent-webaudio-fingerprinting-that-breaks-bluetooth-m-4d2c69f">AliExpress silent WebAudio fingerprinting keeps Bluetooth ... — elseif</a></li>
<li><a href="https://upstract.com/x/56150fe846bd9a27">AliExpress runs silent WebAudio fingerprinting that breaks...</a></li>
<li><a href="https://www.drweb.de/webaudio-fingerprinting-aliexpress-bluetooth/">WebAudio - Fingerprinting : Wie erkennt AliExpress Ihr Gerät?</a></li>
<li><a href="https://news.ycombinator.com/item?id=49372583">AliExpress runs silent WebAudio fingerprinting that... | Hacker News</a></li>

</ul>
</details>

**标签**: `#web-audio`, `#fingerprinting`, `#privacy`, `#bluetooth`, `#aliexpress`

---

<a id="item-tech-news-3"></a>
### [恶意 Rust crate arrayref 在构建时执行载荷](https://safedep.io/arrayref-proc-macro1-rust-build-time-malware/) ⭐️ 8.0/10

一个恶意版本的 Rust crate arrayref 会在构建阶段执行载荷，构成针对 Rust 生态的供应链攻击。Rust 官方博客于 2026-08-20 发布事件说明，GitHub 上的 rustsec/advisory-db issue \#3161 也被创建用于跟踪。恶意包版本在 crates.io 上直接消失，且未显示 yanked 标记，也没有安全公告，导致用户难以确认受影响范围。该事件暴露了 crates.io 对安全事件响应不足，以及 Cargo build.rs 脚本缺少沙箱的问题。

hackernews · abhisek · 8月20日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=49374269)

**「背景」** 2026 年 8 月 20 日，Rust 生态中广泛使用的 crate \`arrayref\` 发布了恶意版本 0.3.10，它静默依赖了一个名为 \`proc-macro1\` 的拼写混淆包（仿冒 \`proc-macro2\` 并冒充维护者 dtolnay），其构建脚本会在编译时从 Hostwinds VPS 下载并执行远程二进制文件。Rust 安全响应团队确认了该事件，并发现 \`internment\` 0.8.7、\`append-only-vec\` 0.1.9 等 crate 也遭到类似投毒，相关恶意包已被删除，\`arrayref\` 的受影响版本已被 yank。此类“构建时载荷”攻击意味着仅执行 \`cargo build\` 即可触发恶意代码，无需调用 crate 中的任何函数。

**「影响」** 受到影响的是依赖了该恶意 arrayref 版本的 Rust 项目开发者：编译时即会执行攻击者载荷，可能造成构建机被入侵或数据泄露；同时 crates.io 未明确标注 yanked 也增加了补救难度。

**「社区讨论」** 社区评论多数批评 crates.io 的处置：恶意版本直接消失却没有 yanked 标识或安全公告；也有开发者呼吁 Cargo 为 build.rs 提供沙箱，并认为 Rust 依赖膨胀令此类攻击难以避免。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/arrayref-rust-crate-supply-chain-attack">Rust Supply-Chain Attack: arrayref, internment, and append-only-vec Poisoned by the proc-macro1 Build-Time Dropper - StepSecurity</a></li>
<li><a href="https://blog.rust-lang.org/2026/08/20/supply-chain-attack-on-arrayref/">Supply chain attack on arrayref | Rust Blog</a></li>
<li><a href="https://daily.dev/posts/rust-supply-chain-attack-arrayref-0-3-10-and-the-proc-macro1-typosquat-execute-a-remote-payload-at--8zkhailuk">Rust Supply-Chain Attack: arrayref 0.3.10 and the proc-macro1 Typosquat Execute a Remote Payload at Build Time | daily.dev</a></li>

</ul>
</details>

**标签**: `#supply-chain-security`, `#rust`, `#crates.io`, `#malware`, `#software-engineering`

---

<a id="item-tech-news-4"></a>
### [陶哲轩警告 AI 或引发数学界最大危机](https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/) ⭐️ 8.0/10

陶哲轩在为 2026 年国际数学家大会撰写的文章中警告，人工智能可能导致数学界自哥德尔以来最大的危机，数学可能从证明稀缺转向证明过剩。他援引 First-Proof 项目第二轮结果：10 道未发表研究题由 4 个 AI 系统测试，其中 7 道至少被一个系统判定为合格，每题成本仅数十至数百美元。陶哲轩认为数学界应停止争论 AI 能做什么，转而正视研究目标这一此前被回避的问题。他还强调，无人能清晰讲解的证明即使通过形式验证也应视为不完整。

telegram · zaihuapd · 8月20日 13:19

**「背景」** 陶哲轩是国际知名数学家，曾解决多个猜想，并长期关注数学严谨性与证明的文化。20 世纪初，罗素悖论与哥德尔不完备定理动摇了数学基础，引发所谓基础危机；陶哲轩认为 AI 可能带来类似规模的危机，但这次考验的不是数学真理，而是数学界的价值观。First-Proof 项目是该背景下的一项尝试，用 AI 系统验证未解决问题，为讨论提供了具体数据。

**「影响」** 对数学研究者和 AI 辅助证明工具开发者而言，这一警告凸显了可解释性和验证标准的重要性；若 AI 生成证明大量涌现，期刊审稿、形式验证和数学共同体共识都将面临新的可信度挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terence_Tao">Terence Tao - Wikipedia</a></li>
<li><a href="https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/">Terence Tao says AI could trigger math &#x27;s biggest crisis since Gödel</a></li>
<li><a href="https://terrytao.wordpress.com/career-advice/theres-more-to-mathematics-than-rigour-and-proofs/">There’s more to mathematics than rigour and proofs | What&#x27;s new</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#proof verification`, `#Terence Tao`, `#research`

---

<a id="item-tech-news-5"></a>
### [125M 参数 Transformer 实现 iPhone 端实时钢琴自动补全](https://simedw.com/2026/08/20/midi-autocomplete/) ⭐️ 7.0/10

开发者 simedw 训练了一个 1.25 亿参数的 Transformer 模型，在 iPhone 15 上以约每秒 108 个音符的速度实时自动补全钢琴演奏，原理类似 GitHub Copilot：用户通过 MIDI 钢琴弹奏几个音符，模型就会在设备端继续生成。该应用免费提供，项目以 MIDI 为基础实现音乐“自动补全”，并涉及 Core ML 部署。社区讨论提到它与古典作曲训练、AI UX 工具、算法生成旋律抗版权诉讼等话题相关。

hackernews · simedw · 8月20日 12:04 · [社区讨论](https://news.ycombinator.com/item?id=49373456)

**「背景」** 这项项目借鉴了“音乐自动补全”的概念，即根据用户演奏的少量音符，由模型续写后续的钢琴旋律。这种类似“套用公式”的作曲训练方式在西方古典音乐传统中早有渊源：音乐理论学者罗伯特·耶尔丁根（Robert Gjerdingen）在其文章《Gebrauchs-Formulas》中记录了 1896 年拉赫玛尼诺夫等人以“模式识别与生成”游戏进行即兴创作的历史案例。现代技术则将该理念转化为基于 Transformer 的端侧生成模型，并通过 Core ML 部署到 iPhone 上实现低延迟推理。

**「影响」** 钢琴用户可免费在 iPhone 上使用该应用，以 MIDI 音符作为提示获得实时的设备端续写结果，从而探索 AI 辅助即兴创作的可能性。

**「社区讨论」** 评论者将这种自动补全类比为古典作曲家的模式训练和 AI UX 设计中的“品味”筛选，也有人询问训练数据规模，并提到用算法穷举所有旋律应对版权诉讼的项目；还有用户表示听到《致爱丽丝》开头被引向完全不同方向会感到不安。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Robert_Gjerdingen">Robert Gjerdingen - Wikipedia</a></li>
<li><a href="https://www.researchgate.net/publication/259731561_Gebrauchs-Formulas">(PDF) Gebrauchs - Formulas</a></li>

</ul>
</details>

**标签**: `#on-device ML`, `#transformer`, `#Core ML`, `#music generation`, `#MIDI`

---

<a id="item-tech-news-6"></a>
### [Linux 7.2 发布：AMD 开源驱动新增 HDMI 2.1 支持](https://www.igalia.com/2026/08/19/Linux-72-Released.html) ⭐️ 7.0/10

Linux 内核 7.2 已发布，这是一个次要版本更新，重点包括为 AMD 开源驱动添加 HDMI 2.1 支持，并包含 Raspberry Pi 相关改进。该版本属于常规演进，而非重大主版本或范式转变，对 Linux 爱好者和开发者而言是重要的增量更新。具体发布详情和完整更新列表以官方公告为准。

hackernews · mariuz · 8月20日 15:46 · [社区讨论](https://news.ycombinator.com/item?id=49376265)

**「背景」** Linux 内核 7.2 是继 7.1 之后的常规版本，其 DRM 合并窗口中最受关注的变化是 AMDGPU 开源驱动终于加入 HDMI 2.1 Fixed Rate Link（FRL）补丁。此前，由于 HDMI 论坛的授权与保密限制，开源驱动无法完整实现 HDMI 2.1；此次 AMD 提交并合入的补丁旨在支持更高的分辨率和刷新率。对于使用现代 Radeon 显卡和开源驱动的用户，这代表 HDMI 2.1 功能在主线内核中的实质性进展。

**「影响」** 最直接的影响是使用 AMD GPU 并依赖开源驱动的用户将获得 HDMI 2.1 支持，Raspberry Pi 用户也能通过更新到 7.2 内核获得相关改进。

**「社区讨论」** 评论中有人追问 AMD 开源驱动此前因 HDMI 论坛限制而无法支持 HDMI 2.1 的情况，另有人表示期待升级 Raspberry Pi 4 的内核，也有人询问这类发布对非深度 Linux 用户有何参考价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://media.patentllm.org/news/hardware/amd-gpu-benchmarks-hdmi-2-1-frl-driver-and-multi-device-ai-w-20260604">AMD GPU Benchmarks, HDMI 2 . 1 FRL Driver , and... - PatentLLM Blog</a></li>
<li><a href="https://www.phoronix.com/forums/forum/phoronix/latest-phoronix-articles/1638013-amd-submits-its-long-awaited-hdmi-2-1-frl-support-for-linux-7-2-amdgpu">AMD Submits Its Long-Awaited HDMI 2 . 1 FRL Support For Linux ...</a></li>
<li><a href="https://www.linuxnews.net/articles/initial-amdgpu-hdmi-2-1-frl-support-successfully-merged-for-linux-7-2">Initial AMDGPU HDMI 2 . 1 FRL Support Successfully... - Linux News</a></li>

</ul>
</details>

**标签**: `#Linux`, `#Kernel`, `#Open Source`, `#HDMI`, `#Raspberry Pi`

---

<a id="item-tech-news-7"></a>
### [谱神经元：一种可扩展可解释的机器学习原语](https://www.reddit.com/r/MachineLearning/comments/1vtfimo/the_spectral_neuron_an_ml_primitive_for_scalable/) ⭐️ 7.0/10

Reddit 用户 alexsht1 发布了预印本《The Spectral Neuron》，提出一种新的机器学习原语，模型形式为 f\(x\)=λ\_k\(A0+Σ x\_i A\_i\)，目标是同时满足简单、可扩展、可解释和可控。该研究源自作者在雅虎广告团队的思考，文中给出了表达能力分析、可从学习到的矩阵直接解读的信息、可保证的形状，以及实用的初始化和训练方案，并在合成与真实数据上进行了扩展性实验。相关代码已开源，作者称论文写作有人工智能辅助查找文献，代码主要由 AI 编写并由作者审查。该成果目前尚未获得广泛社区验证或基准测试。

reddit · r/MachineLearning · /u/alexsht1 · 8月20日 10:20

**「背景」** 传统机器学习常需要在简单可解释模型与复杂高精度模型之间取舍。谱神经元尝试通过矩阵线性函数的形式把可解释性和扩展性结合起来，使模型参数以矩阵形式组织，从而可能直接从矩阵结构中解读特征作用。

**「影响」** 对于关注可解释机器学习的研究者和工程师，这一预印本提供了一个可复现的新建模原语，附有开源代码、初始化与训练配方；但其实际效果仍需独立基准和社区验证。

**标签**: `#machine-learning`, `#interpretability`, `#scalability`, `#research`, `#arxiv`

---

<a id="item-tech-news-8"></a>
### [OpenAI 预览零数据留存与私密安全处理](https://openai.com/index/offering-zero-data-retention-for-frontier-models/) ⭐️ 7.0/10

OpenAI 宣布面向符合条件的 API 客户重申“零数据留存”（ZDR）承诺，请求处理完毕后不保留提示词与回复。同时，OpenAI 预览“私密安全处理”机制，可在不向 OpenAI 人员暴露原始内容的前提下，跨相关交互识别潜在滥用并仅回传有限安全信号。客户内容由客户控制的密钥加密存储，即使被标记，OpenAI 人员也无法获取原文。该功能目前正在与早期客户测试，计划于 9 月逐步上线，并发布技术白皮书。

telegram · zaihuapd · 8月20日 02:33

**「背景」** OpenAI 面向符合条件的 API 客户提供“零数据留存”（ZDR）承诺，即在请求处理完毕后不保留提示词与模型回复；此前该公司已通过 API 中的代理按会话监控滥用来落实这一政策。此次预览的“私密安全处理”机制旨在跨相关交互识别潜在滥用，同时仅向 OpenAI 返回有限的安全信号，使安全审查无需暴露客户原始内容。相关功能与早期客户测试中，计划 9 月逐步上线并发布技术白皮书。

**「影响」** 对于关注数据隐私的 API 客户，这项功能一旦上线将显著降低敏感数据暴露风险，尤其是处理机密提示词的企业；但因其仍处于早期测试阶段，实际效果需等待 9 月正式上线及技术白皮书的验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/offering-zero-data-retention-for-frontier-models/">Offering Zero Data Retention for frontier models | OpenAI</a></li>
<li><a href="https://www.business-standard.com/technology/artificial-intelligence/openai-data-privacy-ai-safety-enterprise-api-126082000704_1.html">AI firms sharpen privacy pitch as enterprises demand control over data</a></li>

</ul>
</details>

**标签**: `#openai`, `#privacy`, `#security`, `#api`, `#data-retention`

---

<a id="item-tech-news-9"></a>
### [反向查询服务泄露数百万张面部照片](https://arstechnica.com/gadgets/2026/08/reverse-lookup-service-exposed-millions-of-photos-of-peoples-faces/) ⭐️ 7.0/10

据 Ars Technica 报道，一家反向图像搜索服务发生数据泄露，导致数百万张人物面部照片及相关个人信息被公开暴露。泄露的数据库规模约 450 GB，包含超过 900 万份图像，部分涉及邮箱、电话及 IP 地址。由于人脸属于难以更换的生物识别信息，此次事件引发了对隐私与身份安全的严重担忧。专家警告，泄露数据可能被用于未经授权的身份识别、个人追踪或诈骗。目前服务方已限制数据库访问，但事件影响范围及后续补救措施仍待确认。

telegram · zaihuapd · 8月20日 15:14

**「背景」** 反向图像搜索服务通常允许用户上传图片以查找相似图片或来源，因此会存储大量用户提交或索引的图片及其元数据。人脸照片属于生物识别信息，一旦泄露，无法像密码一样重置，可能长期被用于身份冒用或精准诈骗。

**「影响」** 相关用户面临面部生物识别信息和个人联系方式被滥用的风险，且可能遭受身份盗窃、定向追踪或诈骗。服务方虽已限制数据库访问，但仍需进一步评估数据是否已被复制或利用。

**标签**: `#data-breach`, `#privacy`, `#biometrics`, `#security`, `#reverse-image-search`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [恒大及许家印案一审宣判：许家印获无期徒刑](https://www.news.cn/legal/20260820/737dfb54ab564fb8a549ba392af9fb0a/c.html) ⭐️ 9.0/10

8 月 20 日，深圳市中级人民法院对恒大集团、恒大地产及创始人许家印案作出一审宣判：恒大集团被判处罚金 88.2 亿元，恒大地产被判处罚金 70 亿元；许家印因多项罪名并罚，被判处无期徒刑、剥夺政治权利终身，并处没收个人全部财产。法院认定，2016 年至 2021 年间，相关方通过大规模财务造假等手段实施非法吸收公众存款、集资诈骗、欺诈发行证券等犯罪；另有 56 名涉案人员被判处十八年至一年十个月不等的有期徒刑。

telegram · zaihuapd · 8月20日 04:06

**「背景」** 法院查明，2016 年至 2021 年间，恒大集团、恒大地产在许家印实际控制下，通过持续性、大规模财务造假、虚增资产、隐瞒负债等手段，实施了非法吸收公众存款、集资诈骗、欺诈发行证券等犯罪；许家印还被控利用职务便利侵占公司财产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news.cn/legal/20260820/737dfb54ab564fb8a549ba392af9fb0a/c.html">恒大集团、恒大地产、许家印等案一审宣判-新华网</a></li>

</ul>
</details>

**标签**: `#Evergrande`, `#securities fraud`, `#regulatory enforcement`, `#China real estate`, `#capital markets`

---

<a id="item-finance-news-2"></a>
### [美联储维持利率不变，为伊朗战争推高油价后首次决策](https://news.google.com/rss/articles/CBMilAFBVV95cUxOWVgwU0l2bjYwREJ2NE9WVC1ObnpJa3Qxa2syS0lmUXphVm8zTWpnYVJ5NXpFZmxWYUZlVXpmc3ZFQzk2ZnZlYjNSUHRPb3F1emZhVDdPNEMxak1mM2wzOEZtYnA5dklfUFlfOUdVRU5lSXNmTlhqMy1pUElaMjNBTEFJbV9IRHNkRGt1NHJKVDVFd1Za0gGaAUFVX3lxTE9IOWFDX2MzMVhjUXl2VE1oTGNTTlowMmxkMUZnNEQ1TzhKemJ3TmlSTElmdzVPQ3VmR2E3OGdNLXN2dVBHQ2xiLXl0WWJfdjBUQktuSnNwbTNQV3puQzBJTUVZS295S2lHYU9iQVpFd05FQkw4WmhmZ2EyU3dCUWt0bHNCUy1xX0pHME5ZbVBlZ1RXSkxnSVZ1TWc?oc=5) ⭐️ 9.0/10

报道称，美联储在伊朗战争推高油价后的首次政策会议上决定维持利率不变。这是一个实际政策决定，但报道未说明具体利率水平或调整幅度。

google\_news · ABC News - Breaking News, Latest News and Videos · 8月19日 15:26

**「背景」** 美联储在 2026 年 7 月 29 日决定维持基准利率不变，这是伊朗战争推高油价以来的首次政策决定。委员会称通胀因战争和油价上涨承压，存在高度不确定性，需要更多数据再作调整。

**「影响」** 受美国与伊朗冲突持续影响，国际油价已逼近每桶 95 美元，这可能推高家庭和企业的能源成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://myv101.iheart.com/content/2026-07-29-fed-holds-interest-rates-steady-amid-inflation-from-iran-conflict/">Fed Holds Interest Rates Steady Amid Inflation From Iran Conflict</a></li>
<li><a href="https://www.aol.com/articles/federal-holds-interest-rates-steady-180125953.html">Federal Reserve holds interest rates steady amid Iran war ... - AOL</a></li>
<li><a href="https://www.aljazeera.com/tag/israel-iran-conflict/">US-Israel war on Iran | US-Israel war... | Today&#x27;s latest from Al Jazeera</a></li>
<li><a href="https://qz.com/oil-prices-iran-strikes-rubio-hormuz-072226">Oil prices near $95 as U.S. strikes Iran for 11th straight night</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#oil prices`, `#Iran conflict`

---

<a id="item-finance-news-3"></a>
### [美联储会议不确定性升高](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 9.0/10

据《华尔街日报》报道，美联储下次会议将是多年来最难以预测的会议之一。

google\_news · WSJ · 7月23日 07:00

**「背景」** 美联储即将召开下一次政策会议。由于近期经济数据好坏参半，市场对是否降息看法分歧，这次利率决定被认为比往年更难预测。

**「影响」** 鉴于美联储下一次会议可能给出加息、降息或按兵不动等多种结果，房屋贷款、信用卡和企业贷款等借贷成本的不确定性可能上升。此前美国核心通胀仍高于目标（6 月核心 PCE 为 3.3%），而就业市场保持稳健，使政策路径更难预判。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thestreet.com/markets/heres-how-stocks-react-to-fed-interest-rate-cuts">The Federal Reserve is expected to reduce interest rates Wednesday.</a></li>
<li><a href="https://abcstlouis.com/news/economy-bringing-mixed-messages-ahead-of-next-federal-reserve-meeting-policy-stock-market-artificial-intelligence">Economy bringing mixed messages ahead of next federal reserve ...</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-tapering-asset-purchases.html">What Federal Reserve monetary policy means for investors</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#markets`

---

<a id="item-finance-news-4"></a>
### [美联储维持利率不变，保留未来加息可能](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

据 CBS 新闻报道，美联储在最近一次会议上决定维持利率不变，但同时暗示未来仍可能加息。这一决定释放出货币政策将根据经济数据灵活调整的信号。

google\_news · CBS News · 6月17日 07:00

**「背景」** 美联储在 2026 年 6 月的会议上将基准利率维持不变，但近半数政策制定者表示支持在今年晚些时候加息，原因是通胀再度抬头。此前的 7 月会议上，委员会以 9 比 3 的投票结果再次维持利率在 3.50%-3.75%不变，同时暗示若通胀持续高企，未来可能加息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door open to hike - CBS News</a></li>
<li><a href="https://www.npr.org/2026/07/29/nx-s1-5910558/federal-reserve-interest-rates-inflation">A divided Federal Reserve holds interest rates steady despite high inflation</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#central bank`

---

<a id="item-finance-news-5"></a>
### [英国央行发布 2026 年 7 月《货币政策报告》](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

英国央行发布 2026 年 7 月《货币政策报告》，阐述最新政策立场与英国经济展望。

google\_news · Bank of England · 7月30日 07:00

**「背景」** 英国央行每季度发布《货币政策报告》，阐述货币政策委员会（MPC）制定利率决策所依据的经济分析与通胀预测。2026 年 7 月 30 日发布的最新报告同时宣布，MPC 以 6 比 3 的投票结果决定维持基准利率在 3.75%不变。

**「影响」** 由于英国央行在 2026 年 7 月将基准利率维持在 3.75%，英国浮动利率抵押贷款借款人的还款压力短期内不会进一步上升，房地产市场的信心也因此受到支撑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/2026/july-2026">Monetary Policy Report - July 2026 - Bank of England</a></li>
<li><a href="https://ebs.publicnow.com/view/198796721B585C9D486667FACA58C1FE32D96706">Bank of England (via Public) / Monetary Policy Report - July 2026</a></li>
<li><a href="https://www.bankofengland.co.uk/">Home | Bank of England</a></li>
<li><a href="https://www.search-acumen.co.uk/news/search-acumen-comments-on-bank-of-englands-interest-rate-decision/">Search Acumen comments on Bank of England ’s interest rate ...</a></li>
<li><a href="https://www.theguardian.com/business/bankofenglandgovernor">Bank of England | The Guardian</a></li>

</ul>
</details>

**标签**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#UK economy`, `#inflation`

---

<a id="item-finance-news-6"></a>
### [胡塞武装计划扩大曼德海峡控制，沙特部分石油出口改道](https://oilprice.com/Geopolitics/Middle-East/Houthis-Move-to-Gain-Complete-Control-Over-Crucial-Bab-el-Mandeb-Oil-Chokepoint.html) ⭐️ 8.0/10

也门政府信息部长穆阿马尔·埃里亚尼说，胡塞武装正计划夺取曼德海峡沿岸土地和红海战略岛屿，以扩大对这条全球重要石油运输通道的控制；三名胡塞消息人士也证实了该计划。近期胡塞武装已袭击多艘沙特油轮，并三次攻击沙特贾赞炼油厂，迫使沙特将部分从延布港出口的原油改经苏伊士运河和埃及塞得基里尔港运输。

rss · OilPrice.com · 8月20日 23:00

**「背景」** 曼德海峡连接红海与亚丁湾，是亚洲与欧洲之间最繁忙的航运通道之一；胡塞武装控制也门部分地区并获伊朗支持，两年前曾袭击与以色列或西方有关联的船只以实质上封锁海峡，而伊朗今年 3 月关闭霍尔木兹海峡后，沙特经红海的出口路线变得更加关键。

**「影响」** 近期袭击已让多家船东再次避开曼德海峡，改走经由非洲的好望角长航线；部分亚洲炼油商还要求沙特阿美在塞得基里尔港交货，贾赞炼油厂也因遇袭于 7 月底关闭，石油出口的时间和成本因此增加。

**标签**: `#Houthis`, `#Bab el-Mandeb`, `#Oil Trade`, `#Geopolitics`, `#Shipping`

---

<a id="item-finance-news-7"></a>
### [美国提前放开冬季级汽油销售以缓解高油价](https://oilprice.com/Latest-Energy-News/World-News/Washington-Eases-Gasoline-Rules-as-Iran-Pressure-Campaign-Jolts-Fuel-Costs.html) ⭐️ 8.0/10

美国环境保护署（EPA）批准从 9 月 1 日起提前销售更便宜的冬季级汽油，而不是等到通常 9 月中旬的换季时间，以缓解国内汽油供应压力。据 AAA 数据，全美平均汽油价格自 7 月中旬以来一直保持在每加仑 4 美元以上，比战争开始时约高 1 美元，也是历年此时段的最高水平。

rss · OilPrice.com · 8月20日 21:30

**「背景」** 夏季级汽油为减少雾霾而要求低挥发性，生产成本更高；提前改用冬季级汽油可增加供应。同日，美国财政部长贝森特称将对伊朗实施“史上最严厉制裁”，但市场仍担忧石油供应中断，油价维持高位。

**「影响」** 对驾车者来说，这一措施可能在加油站带来一定价格缓解，但各州自己的燃料规定可能限制部分市场获得额外供应。

**标签**: `#gasoline prices`, `#EPA waiver`, `#Iran sanctions`, `#fuel supply`, `#energy policy`

---

<a id="item-finance-news-8"></a>
### [中国在扩大可再生能源的同时继续增产油气](https://oilprice.com/Energy/Energy-General/Beijing-Bets-on-Fossil-Fuels-Even-as-It-Leads-the-World-in-Renewables.html) ⭐️ 8.0/10

中国在领跑全球可再生能源的同时，仍继续扩大国内石油和天然气生产。国家能源局数据显示，2025 年原油产量创纪录至 2.16 亿公吨；政府计划到 2030 年将国内油气产量提高至 4.4 亿公吨油当量。

rss · OilPrice.com · 8月20日 15:00

**「背景」** 为降低进口依赖，中国在增加从西非、拉美和俄罗斯采购的同时，计划通过扩建油气管网、天然气储备和 LNG 接收能力来应对中东供应中断风险。

**「影响」** 实际贸易数据已显示出一定效果：5 月中国石油进口降至 2017 年以来最低，平均每日 780 万桶；据标普全球测算，来自中东的原油进口占比从 2025 年上半年的 55.4%降至 2026 年同期的 44.6%。

**标签**: `#China energy policy`, `#oil production`, `#energy security`, `#fossil fuels`, `#global energy markets`

---

<a id="item-finance-news-9"></a>
### [阿里巴巴第一财季净利 105.37 亿元，同比下滑 76%](https://www.alibabagroup.com/en-US/document-2026456290057781248) ⭐️ 8.0/10

阿里巴巴公布 2027 财年第一财季业绩，归属母公司净利润为 105.37 亿元人民币，同比下降 76%。

telegram · zaihuapd · 8月20日 12:08

**「背景」** 阿里巴巴正在加大对人工智能基础设施的投入，2026 财年资本开支达 1260.63 亿元人民币，同比增长 46.63%；当季净利润同比下滑主要受此类投资支出影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/3944384950408836">Alibaba ’s &quot;Mega Ecosystem&quot; Boom Recedes: AI Emerges as Its Sole...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/alibaba-quarterly-profit-drops-75-150542410.html">Alibaba quarterly profit drops 75% as AI investment spending grows</a></li>

</ul>
</details>

**标签**: `#Alibaba`, `#earnings`, `#net profit`, `#Chinese tech`, `#fiscal Q1`

---

<a id="item-finance-news-10"></a>
### [AMD 股价因谷歌扩大定制芯片计划下跌](https://finance.yahoo.com/technology/articles/amd-falls-google-expands-120-192101116.html) ⭐️ 8.0/10

谷歌扩大其总额 1200 亿美元的定制芯片计划，加剧半导体行业竞争，AMD 股价应声下跌。

openbb · NVDA · 8月20日 19:21

**「背景」** Google 正在扩大其定制芯片（custom chip）计划，投入规模达 1,200 亿美元。这类自研芯片（如 Google 的张量处理单元 TPU）是比 Nvidia 高价图形处理器（GPU）更便宜、更适合推理（即运行已训练 AI 模型的过程）的替代方案，需求因此增加；同时，Google 也在增加定制芯片供应商，可能影响 Marvell、Broadcom 等现有供应商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.channelnewsasia.com/business/marvell-gives-google-option-buy-122-billion-stake-in-custom-ai-chip-deal-6328781">Marvell gives Google option to buy $12.2 billion stake in custom AI...</a></li>
<li><a href="https://ts2.tech/en/broadcom-stock-faces-google-supplier-risk-as-370-billion-ai-financing-estimate-looms/">Broadcom Shares Exposed to Google Supplier Concerns as $370...</a></li>

</ul>
</details>

**标签**: `#AMD`, `#Google`, `#custom chips`, `#semiconductor industry`, `#competition`

---

<a id="item-finance-news-11"></a>
### [博通据报寻求超 600 亿美元债务融资用于 AI 投资](https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-203818587.html) ⭐️ 8.0/10

据彭博新闻社报道，博通正寻求超过 600 亿美元的债务融资，用于人工智能相关投资。这一数字为报道中的目标金额，尚未得到公司正式确认。

openbb · NVDA · 8月20日 20:38

**「背景」** 今年 6 月，阿波罗和黑石曾牵头为博通的 AI 基础设施平台（AI XPV）提供 350 亿美元融资，该平台目前为 Anthropic 提供超过 1 吉瓦算力。

**「影响」** Broadcom 的股东和债权人将面对新增逾 600 亿美元债务带来的杠杆风险；据报 Anthropic 等 AI 公司将成为该芯片融资安排的受益方，可能获得更稳定的 AI 芯片供应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://247wallst.com/investing/2026/08/14/broadcom-sinks-6-as-bofa-flags-370b-in-ai-debt-amd-climbs-4-on-bairds-1250-call/">Broadcom Sinks 6% as BofA Flags $370B in AI Debt ... - 24/7 Wall St.</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">AI Infrastructure Boom Drives Broadcom ’s $ 60 Billion Debt ...</a></li>
<li><a href="https://www.newsmax.com/finance/streettalk/broadcom-60-billion-dollars-ai/2026/08/20/id/1266812/">Broadcom Seeks $ 60 Billion in Latest AI Debt Deal | Newsmax.com</a></li>
<li><a href="https://cryptobriefing.com/broadcom-60b-debt-ai-chip-financing/">Broadcom seeks over $ 60 B in debt for AI chip financing deal</a></li>

</ul>
</details>

**标签**: `#Broadcom`, `#AI`, `#debt financing`, `#capital markets`, `#semiconductors`

---

<a id="item-finance-news-12"></a>
### [Broadcom 寻求逾 600 亿美元债务融资用于 AI 项目](https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-201702584.html) ⭐️ 8.0/10

Broadcom 正寻求超过 600 亿美元的债务融资，用于人工智能相关项目。

openbb · NVDA · 8月20日 20:17

**「背景」** 据彭博社援引知情人士报道，博通正与一组贷款机构洽谈，计划筹集超过 600 亿美元债务，用于一项 AI 芯片融资交易，将使 Anthropic 等公司受益。

**「影响」** 据知情人士，若这笔超过 600 亿美元的债务融资最终完成，将为 Anthropic 等公司的 AI 芯片需求提供资金支持，可能推动更大规模的 AI 基础设施投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">Broadcom Seeks More Than $60 Billion in Latest AI Debt Deal</a></li>
<li><a href="https://kfgo.com/2026/08/20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal-bloomberg-news-reports/">Broadcom seeks more than $60 billion in latest AI debt deal, Bloomberg News reports | The Mighty 790 KFGO | KFGO</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-203818587.html">Broadcom seeks more than $60 billion in latest AI debt deal, Bloomberg News reports</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">AI Infrastructure Boom Drives Broadcom ’s $ 60 Billion Debt Financing...</a></li>
<li><a href="https://cryptobriefing.com/broadcom-60b-debt-ai-chip-financing/">Broadcom seeks over $ 60 B in debt for AI chip financing deal</a></li>

</ul>
</details>

**标签**: `#Broadcom`, `#debt financing`, `#artificial intelligence`, `#capital markets`, `#corporate finance`

---

<a id="item-finance-news-13"></a>
### [台积电上调资本支出预测至 850 亿美元，ASML 股价上涨](https://finance.yahoo.com/technology/articles/asml-gains-tsmcs-spending-forecast-190758887.html) ⭐️ 8.0/10

台积电将资本支出预测上调至 850 亿美元，带动 ASML 股价上涨，因市场预期先进制程芯片制造设备需求将增强。这一数字是预测值，并非已实际支出的金额。

openbb · NVDA · 8月20日 19:07

**「背景」** ASML 是全球最大的芯片制造设备供应商。台积电（TSMC）是其主要客户之一，也是英伟达（Nvidia）的主要芯片供应商，因人工智能芯片需求旺盛而提高资本支出预测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/articles/asml-gains-tsmcs-spending-forecast-190758887.html">ASML Gains as TSMC&#x27;s Spending Forecast Hits $85 Billion</a></li>
<li><a href="https://finance.yahoo.com/markets/article/tsmc-raises-capex-and-revenue-forecast-highlighting-growing-ai-chip-demand-113101950.html">TSMC raises capex and revenue forecast, highlighting growing AI chip demand</a></li>
<li><a href="https://www.investing.com/news/stock-market-news/strong-asml-tsmc-forecasts-signal-ai-spending-boom-is-intact-4617583">Strong ASML, TSMC forecasts signal AI spending boom is intact By Reuters</a></li>

</ul>
</details>

**标签**: `#ASML`, `#TSMC`, `#semiconductor equipment`, `#capital expenditure`, `#market reaction`

---

<a id="item-finance-news-14"></a>
### [台积电 2027 年资本支出预测达 850 亿美元，股价上涨](https://finance.yahoo.com/technology/articles/tsmc-rises-2027-capex-forecast-192841498.html) ⭐️ 8.0/10

台积电股价上涨，因 2027 年资本支出预测达到 850 亿美元，显示其计划大幅扩大先进半导体制造产能。

openbb · NVDA · 8月20日 19:28

**「背景」** 台积电在 2026 年初曾表示当年资本支出约为 520 亿至 560 亿美元；此次关于其 2027 年资本支出最高可达 850 亿美元的预测，显示该公司计划大幅扩产先进半导体制造产能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sg.finance.yahoo.com/news/tsmc-rises-2027-capex-forecast-192841498.html">TSMC Rises as 2027 Capex Forecast Reaches $85 Billion</a></li>
<li><a href="https://semiwiki.com/semiconductor-manufacturers/tsmc/371192-tsmcs-raises-the-bar-on-capex/">TSMC’s Raises the Bar on CAPEX! - Semiwiki</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#Semiconductors`, `#Capital Expenditure`, `#AI Infrastructure`, `#Supply Chain`

---

<a id="item-finance-news-15"></a>
### [Stripe 同意收购 OpenRouter](https://stripe.com/en-jp/newsroom/news/stripe-agrees-to-acquire-openrouter) ⭐️ 7.0/10

Stripe 于 2026 年 8 月 19 日宣布同意收购 AI 模型网关平台 OpenRouter；后者可在 80 多家提供商的 400 多个模型之间动态分配请求。

telegram · zaihuapd · 8月20日 07:00

**「背景」** OpenRouter 是一个 AI 模型网关和路由平台，可在 80 多家提供商的 400 多个模型之间动态分配请求，帮助企业优化 Token（AI 模型计费单位）使用。据彭博社报道，Stripe 已同意以超过 70 亿美元的现金和股票收购 OpenRouter，不过截至报道时两家公司均未公开确认，最终价格仍可能有变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.orcarouter.ai/blog/stripe-acquires-openrouter">Stripe OpenRouter Acquisition : $7B, What Changes for Devs</a></li>
<li><a href="https://qz.com/stripe-acquiring-openrouter-ai-model-gateway-7-billion-081726">Stripe acquires AI model gateway OpenRouter for $7 billion</a></li>

</ul>
</details>

**标签**: `#Stripe`, `#OpenRouter`, `#Acquisition`, `#AI Infrastructure`, `#M&amp;A`

---