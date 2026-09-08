---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 198 items, 18 important content pieces were selected

---

**Technology News**
1. [LLM-guided evolution improves 10 circle-packing records for N=101-114](#item-tech-news-1) ⭐️ 8.0/10
2. [Rustuna Brings Optuna-Compatible HPO to Rust](#item-tech-news-2) ⭐️ 7.0/10
3. [KV Cache as an Agent Runtime: Yandex Research for Interactive LLMs](#item-tech-news-3) ⭐️ 7.0/10
4. [Benchmarking LLMs as longitudinal measurements: 31k repeated runs show large day-to-day drift](#item-tech-news-4) ⭐️ 7.0/10
5. [Huawei Launches Mate XT 2 With First Flagship Kirin Chip in Six Years](#item-tech-news-5) ⭐️ 7.0/10
6. [China Supreme Court Clarifies AI Face-Swap and Pricing Liability](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [US Federal Reserve Leaves Interest Rates Steady Under New Chair Warsh](#item-finance-news-1) ⭐️ 9.0/10
2. [China injects $54 billion into state banks and insurers](#item-finance-news-2) ⭐️ 8.0/10
3. [GM and Ford Turn EV Battery Capacity to Energy Storage](#item-finance-news-3) ⭐️ 8.0/10
4. [Copper Rallies for 10th Week as Supply Shrinks and Tariff Risk Looms](#item-finance-news-4) ⭐️ 8.0/10
5. [TSMC’s $265 Billion U.S. Investment Now Plays a Role in Taiwan’s Chip Diplomacy](#item-finance-news-5) ⭐️ 8.0/10
6. [Kenvue-Kimberly-Clark Deal Nears Close, Analysts Flag Remaining Risks](#item-finance-news-6) ⭐️ 8.0/10
7. [Federal Reserve holds rates steady, signals possible hike](#item-finance-news-7) ⭐️ 8.0/10
8. [Rosneft Ships First Crude From Giant Vostok Oil Project](#item-finance-news-8) ⭐️ 7.0/10
9. [China Pauses Approvals for New Battery Storage Plants](#item-finance-news-9) ⭐️ 7.0/10
10. [L’Uzbekistan limita il ruolo di Rosatom nel progetto nucleare](#item-finance-news-10) ⭐️ 7.0/10
11. [India Ramps Up Rail Coal Deliveries as Power Plant Stockpiles Fall Below Critical Levels](#item-finance-news-11) ⭐️ 7.0/10
12. [TSM Raises Guidance on Strong Demand for Advanced Chips](#item-finance-news-12) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [LLM-guided evolution improves 10 circle-packing records for N=101-114](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

A researcher used an LLM to iteratively evolve an optimization program rather than solve circle packing directly, starting from a simple seed solver and letting the LLM propose algorithmic changes guided by a scoreboard of results and a history of prior attempts. Each candidate was scored by an independent verifier so only genuine improvements were kept. On the Packomania csqv benchmark, this approach improved the best-known sum-of-radii for 10 values of N from 101 to 114, with gains of 2.4% to 5.4%, achieved in 15 iterations and at a total LLM cost of $27.72. Packomania independently accepted the results. The work is described in the paper arXiv:2609.05093, with code and solutions on GitHub.

reddit · r/MachineLearning · /u/SIGH\_I\_CALL · Sep 7, 16:54

**「Background」** The Packomania project catalogs best-known solutions to circle-packing optimization problems, including the csqv subproblem of packing variable-sized circles in a square to maximize the sum of radii; its tables note that results are complete or proven optimal only up to N=100, leaving larger instances open for improvement. Circle packing is a classic geometric optimization benchmark in which even tiny gains in the sum of radii can represent difficult, long-standing improvements. LLM-guided program evolution is a method that treats the optimization algorithm itself as the object of mutation: an LLM proposes algorithmic modifications, an independent verifier scores each candidate solver&\#x27;s results, and only successful changes are retained and iterated upon.

**「Impact」** This demonstration shows that LLM-guided program evolution can cost-effectively improve recognized best-known results on a longstanding optimization benchmark, opening a practical path for AI-driven algorithm discovery in well-scored problem domains.

<details><summary>References</summary>
<ul>
<li><a href="https://packomania.com/csqv/csqv.html">The best known packings of unequal circles in a square</a></li>
<li><a href="https://arxiv.org/html/2609.05093v1">LLM-Guided Program Evolution for Circle Packing:Breaking 10 ...</a></li>

</ul>
</details>

**Tags**: `#LLM-guided evolution`, `#optimization`, `#circle packing`, `#program synthesis`, `#benchmark improvement`

---

<a id="item-tech-news-2"></a>
### [Rustuna Brings Optuna-Compatible HPO to Rust](https://www.reddit.com/r/MachineLearning/comments/1w9nyhz/rustuna_a_highperformance_rust_implementation_of/) ⭐️ 7.0/10

The Optuna team and contributor /u/c-bata announced Rustuna, a high-performance Rust implementation of the Optuna hyperparameter optimization framework, hosted at github.com/optuna/rustuna with a Medium announcement post. Rustuna keeps Optuna&\#x27;s familiar API and concepts so existing users can adopt it with minimal changes, while being built with zero Python dependencies to reduce supply chain attack risk. It also achieves a lower memory footprint through native Rust memory management. The project is positioned as a faster, memory-efficient alternative for Python-based Optuna workflows, though no specific benchmark figures or version numbers were provided in the announcement.

reddit · r/MachineLearning · /u/c-bata · Sep 7, 10:01

**「Background」** Optuna is a widely used open-source Python framework for automated hyperparameter optimization, known for its define-by-run API and algorithms such as TPE. Rustuna is a Rust-based implementation of Optuna hosted under the Optuna GitHub organization that keeps the familiar Optuna API while aiming for higher speed and lower memory usage, and it avoids Python dependencies to reduce supply-chain attack risk. The Rustuna developers note that they do not plan to reimplement Optuna’s visualization features in Rust; instead, they intend to make results accessible through the existing optuna.visualization module or Optuna Dashboard.

**「Impact」** ML practitioners who rely on Optuna for hyperparameter optimization can evaluate Rustuna as a drop-in compatible implementation that may reduce Python supply-chain exposure and memory usage for long-running optimization jobs, but concrete performance advantages remain unverified until benchmarks and compatibility details are published.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/optuna/rustuna">GitHub - optuna/rustuna: A faster Optuna implementation in ...</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Optuna`, `#Hyperparameter Optimization`, `#Machine Learning`, `#Open Source`

---

<a id="item-tech-news-3"></a>
### [KV Cache as an Agent Runtime: Yandex Research for Interactive LLMs](https://www.reddit.com/r/MachineLearning/comments/1w9myqc/kv_cache_as_an_agent_runtime_r/) ⭐️ 7.0/10

Yandex researchers describe an approach that treats the KV cache as an agent runtime, allowing the model&\#x27;s inference state to be modified for more interactive and responsive LLM behavior. The idea builds on their earlier Hogwild\! Inference and AsyncReasoning work, and the blog post previews future research in which a Qwen3.8-27B agent plays a DOOM environment interactively using similar techniques. The authors argue that inference and runtime design is an under-explored axis of agent capabilities, positioned between the abstract harness and costly full model changes.

reddit · r/MachineLearning · /u/\_puhsu · Sep 7, 09:03

**「Background」** Large language models generate text token by token while maintaining a key-value \(KV\) cache that stores the attention keys and values for tokens processed so far. Yandex researchers propose treating this KV cache as an agent runtime, meaning the cache can be shared, scheduled, and manipulated between inference steps to let a pretrained LLM observe, reason, and act concurrently without additional training or fine-tuning. This idea builds on their lab’s earlier work, including Hogwild\! Inference and AsyncReasoning, and the blog post previews a future demo where a Qwen3.8-27B agent controls a DOOM environment interactively using these KV-cache techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://research.yandex.com/blog/the-kv-cache-as-an-agent-runtime">The KV cache as an agent runtime - research.yandex.com</a></li>

</ul>
</details>

**Tags**: `#KV-cache`, `#LLM inference`, `#agent runtime`, `#interactive AI`, `#research`

---

<a id="item-tech-news-4"></a>
### [Benchmarking LLMs as longitudinal measurements: 31k repeated runs show large day-to-day drift](https://www.reddit.com/r/MachineLearning/comments/1w9llr4/measuring_llm_performance_drift_observations_and/) ⭐️ 7.0/10

A Reddit discussion by the founder of AI Stupid Level describes a methodology for measuring LLM performance drift by treating benchmarks as continuous time-series observations rather than static leaderboard scores. The analysis used 31,352 repeated score observations across 49 models and found that the standard deviation of within-day scores was 2.80 points while the standard deviation of between-day daily medians was 8.43 points, roughly a 3:1 ratio. The author argues that this variation is large enough to warrant explicit measurement of temporal changes, while cautioning that confounders such as task composition, sampling, missingness, and provider behavior prevent a direct conclusion that providers are changing models day-to-day. The proposed approach includes versioned benchmark configurations, repeated execution-based evaluation, separation of availability failures from valid task outcomes, tracking of serving/version metadata when available, and change detection on the resulting time series. A public methodology PDF was released that withholds the exact live task bank and operational parameters to reduce benchmark contamination while remaining scientifically inspectable.

reddit · r/MachineLearning · /u/ionutvi · Sep 7, 07:44

**「Background」** Large language models served through APIs are not necessarily static: providers can change infrastructure, configuration, or weights, so performance can drift even when the advertised model name stays the same. Traditional benchmark leaderboards treat evaluations as snapshots, but longitudinal evaluation instead measures models repeatedly over time and applies statistical change detection to distinguish genuine capability changes from ordinary variability and infrastructure issues. The author is the founder of AI Stupid Level, a platform that publicly documents this kind of continuous benchmarking methodology.

**「Impact」** Teams using API-served LLMs and those responsible for model evaluation or MLOps should treat benchmark scores as noisy longitudinal data and monitor for drift, while explicitly separating model-capability changes from infrastructure, availability, or configuration effects.

<details><summary>References</summary>
<ul>
<li><a href="https://aistupidlevel.com/">AI Stupid Level Benchmark | Real AI Model Drift Testing</a></li>

</ul>
</details>

**Tags**: `#LLM evaluation`, `#benchmark drift`, `#model monitoring`, `#MLOps`, `#AI reliability`

---

<a id="item-tech-news-5"></a>
### [Huawei Launches Mate XT 2 With First Flagship Kirin Chip in Six Years](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 7.0/10

Huawei unveiled the Mate XT 2 triple-folding smartphone in Guangzhou on September 7, powered by the Kirin 9050 Pro chipset, and Xinhua reported it was Huawei&\#x27;s first all-new flagship Kirin processor since the Mate 40 global launch six years earlier. Huawei says the Kirin 9050 Pro is the first high-performance chip designed with logic-folding technology, which stacks logic units in layers within a single chip and adds vertical interconnect channels, shortening signal paths. The company claims this reduces latency and improves performance compared with conventional planar chip layouts. The announcement includes no benchmark data or independent validation.

telegram · zaihuapd · Sep 7, 08:20

**「Background」** Logic folding is a chip-architecture concept in which logic units are stacked vertically inside one die instead of laid out on a single plane, with added vertical interconnect channels described as elevator-like. Huawei expects this arrangement to shorten signal paths, lower latency, and improve performance. The Mate 40 global launch was Huawei&\#x27;s previous flagship event to introduce a new Kirin chip, about six years before the Mate XT 2 announcement.

**Tags**: `#hardware`, `#chip-design`, `#Huawei`, `#mobile-computing`, `#semiconductors`

---

<a id="item-tech-news-6"></a>
### [China Supreme Court Clarifies AI Face-Swap and Pricing Liability](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 7.0/10

On September 7, China&\#x27;s Supreme People&\#x27;s Court issued a judicial interpretation on AI disputes, comprising five parts and 24 articles, covering AI face swapping, algorithmic price discrimination, impersonation in endorsements, autonomous driving, and intellectual property. The rules state that using AI without consent to generate identifiable faces or voices may constitute personality-rights infringement. Algorithmic price discrimination that harms consumers&\#x27; rights can result in liability, and AI impersonation used to induce purchases may support claims for punitive damages. The interpretation also targets AI-facilitated “network doxxing” and “human flesh search” as violations of privacy. This clarifies legal responsibility for AI applications and affects developers, platforms, and users.

telegram · zaihuapd · Sep 7, 09:32

**「Background」** China&\#x27;s Supreme People&\#x27;s Court issues judicial interpretations to explain how existing laws apply to specific legal questions, and these interpretations guide lower courts in deciding cases. This interpretation addresses liability questions raised by generative AI and automated algorithms, such as whether deepfakes infringe personality rights and when algorithmic price differentiation becomes illegal.

**「Impact」** AI companies, platform operators, and developers in China must align face-swap tools, algorithmic pricing, and impersonation features with personality-rights and privacy rules to avoid liability, while affected consumers gain clearer legal grounds for lawsuits and punitive damages.

**Tags**: `#AI regulation`, `#judicial interpretation`, `#face swap`, `#algorithmic pricing`, `#privacy`

---

## Financial News

<a id="item-finance-news-1"></a>
### [US Federal Reserve Leaves Interest Rates Steady Under New Chair Warsh](https://news.google.com/rss/articles/CBMipgFBVV95cUxOM3c5cXgydnhwSFlrWmlyVjJobnRCbFkxaHg2c3NtTEl6Z2VLSGNIMXN3dmlKS2JZSF9Gc2p1TTVrd1hEcVdxSzBRaU13RVh1eTJRLW1pRkp0cHdKbk9FSU5SZ2FncC1ZangzQzZkZjFSaHNRWm94TlNROExtSm56Zk1qckpwT1JweWVKV1daY0tUMk03eFZJakRpMjNBVzl5N1NEQzFn0gGrAUFVX3lxTE1wYkYxa2NtTktYZkMyQ3VCSG5vYkw3UkE1cGpqaTRwOXE1MVpsd1ZfbDA2X3lGOEF5WG51SHFBbEhXbWs1enFfS1k2ZWRDMzVUU21sT2RMbC04VkoxUXk0Z1pYMVpWejF0ZGNyaUpiVWxjLWZYWVVBU28tb082QWlwT29PX1o3ekFTUk1fdTdGb3drUm5FOEIzZEc3UGlCRjhaUDlsS3Y0Yk8wMA?oc=5) ⭐️ 9.0/10

Al Jazeera reports that the US Federal Reserve, under its new chair Warsh, has kept interest rates unchanged.

google\_news · Al Jazeera · Jun 17, 07:00

**「Background」** The Federal Reserve, under new Chair Kevin Warsh, decided at its first meeting to keep interest rates at 3.50–3.75 percent, a unanimous policy hold announced Wednesday, as inflationary pressures persist. Warsh has faced scrutiny over his views on inflation and the path for future rate cuts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/6/17/us-federal-reserve-holds-rates-steady-under-new-chair-warsh">US Federal Reserve holds rates steady under new chair Warsh | Inflation News | Al Jazeera</a></li>
<li><a href="https://apnews.com/article/inflation-federal-reserve-interest-rates-a8661a4be7fcf3076891382cf9df1a5e">New Fed chair Kevin Warsh under pressure to clarify views on inflation, interest rates | AP News</a></li>

</ul>
</details>

**Tags**: `#federal-reserve`, `#monetary-policy`, `#interest-rates`, `#warsh`, `#central-bank`

---

<a id="item-finance-news-2"></a>
### [China injects $54 billion into state banks and insurers](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 8.0/10

China’s finance ministry announced a combined 360 billion yuan \($53.6 billion\) capital injection into three state banks and five insurers, the first recapitalization package to include insurers. Citibank described the package as smaller than markets had expected, and Hong Kong-listed shares of the recipients fell on Monday.

rss · CNBC Finance · Sep 7, 23:23

**「Background」** The move follows a 500 billion yuan injection into four major state banks last year and a March pledge to issue 300 billion yuan in special treasury bonds this year for large state lenders.

**Tags**: `#China`, `#banking`, `#capital injection`, `#state-owned enterprises`, `#financial policy`

---

<a id="item-finance-news-3"></a>
### [GM and Ford Turn EV Battery Capacity to Energy Storage](https://oilprice.com/Energy/Energy-General/GM-Ford-Turn-EV-Battery-Bust-Into-Energy-Storage-Bet.html) ⭐️ 8.0/10

Ford and GM are converting underused electric-vehicle battery capacity into energy storage businesses, with Ford saying it will invest roughly $2 billion over two years and target at least 20 GWh of annual battery storage deployments by late 2027.

rss · OilPrice.com · Sep 7, 20:00

**「Background」** The moves follow weak U.S. EV demand, which led Ford to write down $19.5 billion and GM to record $10.9 billion in cumulative charges, leaving both automakers with underutilized battery plants.

**「Impact」** Ford&\#x27;s new storage systems are aimed at utilities, data centers, and large industrial customers, a U.S. market that installed a record 20.2 GWh in the second quarter of 2026, according to SEIA and Benchmark Mineral Intelligence.

**Tags**: `#energy storage`, `#electric vehicles`, `#Ford`, `#General Motors`, `#battery manufacturing`

---

<a id="item-finance-news-4"></a>
### [Copper Rallies for 10th Week as Supply Shrinks and Tariff Risk Looms](https://oilprice.com/Metals/Commodities/Coppers-Longest-Rally-Since-1994-Collides-With-a-Shrinking-Supply-Chain.html) ⭐️ 8.0/10

Copper prices have notched a 10th straight weekly gain on the London Metal Exchange, the longest run since 1994, with prices near $14,300 a ton and close to the record $14,527.50 set in January. The rally is underpinned by tightening physical supply: LME warehouse stocks fell for 42 consecutive days through mid-August, and early-August export restrictions in the Democratic Republic of Congo added fresh disruption.

rss · OilPrice.com · Sep 7, 17:00

**「Background」** This supply squeeze traces back to the Sept. 8, 2025 landslide at Freeport-McMoRan&\#x27;s Grasberg mine in Indonesia, the world&\#x27;s second-largest copper source, which killed two workers, forced a force majeure that allows missed deliveries, and led Freeport to cut its 2026 output guidance at the complex by about a third, with full recovery not expected until 2027 or 2028.

**「Impact」** If the White House imposes the possible 15% tariff on refined copper as soon as January, U.S. manufacturers could face higher input costs; traders&\#x27; efforts to get ahead of that risk have already pushed July refined copper imports to a record of roughly 200,000 tons.

**Tags**: `#copper`, `#commodities`, `#supply chain`, `#mining`, `#trade policy`

---

<a id="item-finance-news-5"></a>
### [TSMC’s $265 Billion U.S. Investment Now Plays a Role in Taiwan’s Chip Diplomacy](https://finance.yahoo.com/technology/articles/tsmcs-265-billion-u-bet-192538926.html) ⭐️ 8.0/10

The article reports that TSMC’s $265 billion U.S. investment is increasingly intertwined with Taiwan’s “chip diplomacy” — Taiwan’s use of its central position in semiconductor production to strengthen international relationships.

openbb · NVDA · Sep 7, 19:25

**「Background」** TSMC, the Taiwan-based chipmaker, raised its planned U.S. investment by $100 billion to a total of $265 billion as part of a U.S.-Taiwan trade and investment deal announced in January 2026. The expansion reflects competing pressures: Taiwan wants to keep advanced chip-making at home, while the U.S. and Europe want more domestic semiconductor production, giving the investment a role in Taiwan&\#x27;s broader diplomatic efforts.

**「Impact」** TSMC’s reported $265 billion U.S. commitment is large enough to reshape advanced-chip supply chains and U.S.-Taiwan diplomacy; in Taiwan, some security analysts and commentators cited here say that moving leading-edge chip production to the United States could weaken the island’s “silicon shield,” the perceived security benefit of its semiconductor dominance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/9069774/tsmcs-265-billion-us-bet-is-becoming-part-of-taiwans-chip-diplomacy">TSMC&#x27;s $265 Billion U.S. Bet Is Becoming Part of Taiwan&#x27;s Chip D</a></li>
<li><a href="https://www.nist.gov/news-events/news/2026/07/trump-administration-secures-additional-100-billion-us-semiconductor">Trump Administration Secures an Additional $100 Billion U.S ...</a></li>
<li><a href="https://www.csis.org/analysis/silicon-island-assessing-taiwans-importance-us-economic-growth-and-security">Silicon Island: Assessing Taiwan’s Importance to U.S. Economic Growth and Security | CSIS</a></li>
<li><a href="https://www.stimson.org/2025/why-taiwan-fears-america-first-risks-eroding-its-silicon-shield/">Why Taiwan Fears ‘America First’ Risks Eroding Its ‘Silicon Shield’ • Stimson Center</a></li>
<li><a href="https://www.dw.com/en/tsmc-chip-plans-in-us-fuel-china-security-fears-in-taiwan/a-71877492">TSMC chip plans in US fuel China security fears in Taiwan</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductor industry`, `#U.S. investment`, `#chip diplomacy`, `#Taiwan`

---

<a id="item-finance-news-6"></a>
### [Kenvue-Kimberly-Clark Deal Nears Close, Analysts Flag Remaining Risks](https://finance.yahoo.com/markets/stocks/articles/kenvues-kimberly-clark-deal-nears-192800397.html) ⭐️ 8.0/10

Kenvue’s deal with Kimberly-Clark is nearing completion, according to an analysis, though key risks remain unresolved before the transaction closes.

openbb · PG · Sep 7, 19:28

**「Background」** Kimberly-Clark agreed in November 2025 to acquire Kenvue for roughly $32 billion in cash and stock; shareholders of both companies voted on Jan. 29, 2026 to approve the deal.

**「Impact」** Analysts warn that if the deal closes, smaller independent consumer-goods brands could be squeezed out of retail shelf space because the combined Kimberly-Clark/Kenvue would bundle essential household staples with over-the-counter medicines, while the merged company may also carry lingering litigation risks tied to Kenvue’s former parent, Johnson &amp; Johnson.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investor.kimberly-clark.com/news-releases/news-release-details/kimberly-clark-and-kenvue-shareholders-overwhelmingly-approve">Kimberly-Clark and Kenvue Shareholders Overwhelmingly Approve ...</a></li>
<li><a href="https://investors.kenvue.com/financial-news/news-details/2025/Kimberly-Clark-to-Acquire-Kenvue-Creating-a-32-Billion-Global-Health-and-Wellness-Leader/default.aspx">Kenvue Inc. - Kimberly-Clark to Acquire Kenvue, Creating a ...</a></li>
<li><a href="https://www.morningstar.com/stocks/kimberly-clark-kenvue-deal-comes-with-considerable-risks-shares-look-cheap">Kimberly-Clark: Kenvue Deal Comes With Considerable Risks, but Shares Look Cheap | Morningstar</a></li>
<li><a href="https://markets.financialcontent.com/stocks/article/marketminute-2026-3-16-the-40-billion-pivot-kimberly-clark-and-kenvue-merger-redefines-the-consumer-staples-landscape">FinancialContent - The $40 Billion Pivot: Kimberly-Clark and Kenvue Merger Redefines the Consumer Staples Landscape</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#Consumer Staples`, `#Kenvue`, `#Kimberly-Clark`, `#Corporate Risk`

---

<a id="item-finance-news-7"></a>
### [Federal Reserve holds rates steady, signals possible hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 8.0/10

The Federal Reserve kept interest rates unchanged but indicated that another increase could still be possible, affecting borrowing costs and market expectations.

google\_news · cbsnews.com · Jun 17, 07:00

**「Background」** The Federal Reserve&\#x27;s rate-setting committee, the FOMC, voted 9-3 on July 29, 2026, to keep its benchmark federal funds rate—the rate banks charge each other for overnight loans, which influences consumer borrowing costs—unchanged at 3.5% to 3.75%. The decision was split, and officials left the door open to another hike later this year if inflation stays elevated.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.com/en-us/money/economy/federal-reserve-holds-interest-rates-steady-but-leaves-door-open-to-hike/ar-AA25TWIp">Federal Reserve holds interest rates steady but leaves door ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-rate-decision-july-2026.html">Fed rate decision July 2026: Divided Fed holds interest rates ...</a></li>
<li><a href="https://www.npr.org/2026/07/29/nx-s1-5910558/federal-reserve-interest-rates-inflation">Divided Fed holds interest rates steady : NPR</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#markets`

---

<a id="item-finance-news-8"></a>
### [Rosneft Ships First Crude From Giant Vostok Oil Project](https://oilprice.com/Energy/Crude-Oil/Rosneft-Ships-First-Crude-From-157-Billion-Vostok-Oil-Project.html) ⭐️ 7.0/10

Rosneft has shipped the first crude cargo from its Vostok Oil project in Russia&\#x27;s Arctic and Siberian regions, a milestone for a development once estimated at about US$157 billion. The project is expected at peak capacity to produce 50–100 million metric tons of crude per year and up to 2 million barrels per day in later phases.

rss · OilPrice.com · Sep 7, 21:00

**「Background」** Vostok Oil is Russia&\#x27;s largest new oil development, combining producing fields and new discoveries in Krasnoyarsk Krai, with reserves Rosneft says total roughly 7 billion tons of low-sulfur crude. Western partners including Trafigura and Vitol pulled out after Western sanctions imposed in 2022, so Rosneft says it used domestically developed drilling equipment.

**Tags**: `#Rosneft`, `#Vostok Oil`, `#Russia oil`, `#sanctions`, `#Arctic energy`

---

<a id="item-finance-news-9"></a>
### [China Pauses Approvals for New Battery Storage Plants](https://oilprice.com/Latest-Energy-News/World-News/China-Halts-New-Battery-Storage-Plant-Approvals.html) ⭐️ 7.0/10

China has temporarily paused approvals for new battery storage plants that have not started construction, according to Chinese financial outlet Cailianshe, which cited industry sources. The government has also announced consumption taxes on most batteries of 2% from September 2026 and 4% from September 2027.

rss · OilPrice.com · Sep 7, 16:30

**「Background」** Years of subsidies for China’s EV, solar, and battery industries led to overcapacity and price wars, prompting regulators to tighten controls on EVs and solar panels before turning to battery storage.

**Tags**: `#China`, `#battery storage`, `#overcapacity`, `#regulation`, `#energy policy`

---

<a id="item-finance-news-10"></a>
### [L’Uzbekistan limita il ruolo di Rosatom nel progetto nucleare](https://oilprice.com/Alternative-Energy/Nuclear-Power/Uzbekistan-Scales-Back-Nuclear-Cooperation-With-Russia.html) ⭐️ 7.0/10

Secondo una nota della presidenza uzbeka del 2 settembre, Tashkent intende ridurre il ruolo di Rosatom nella prima centrale nucleare del paese proponendo una joint venture con società internazionali di ingegneria. La nota fissa nuovi obiettivi di localizzazione: almeno il 30% di produzione domestica, contro il 21% attuale \(1,9 miliardi di dollari su un costo totale stimato di 9,5 miliardi\), il 65% dei lavori di costruzione a imprese nazionali e 7.000 addetti locali.

rss · OilPrice.com · Sep 7, 16:00

**「Contesto」** Il progetto prevede due grandi reattori VVER-1000 e due più piccoli RITM-200N; a giugno era stato avviato simbolicamente con la Russia, ma a gennaio la costruzione era già stata rinviata rispetto al calendario iniziale.

**「Possibili effetti」** Se attuati, questi obiettivi aprirebbero più spazio a imprese e lavoratori uzbeki nel cantiere e ridurrebbero la posizione di Rosatom come esecutore principale del progetto.

**Tags**: `#nuclear energy`, `#Uzbekistan`, `#Rosatom`, `#energy policy`, `#Russia-Central Asia relations`

---

<a id="item-finance-news-11"></a>
### [India Ramps Up Rail Coal Deliveries as Power Plant Stockpiles Fall Below Critical Levels](https://oilprice.com/Latest-Energy-News/World-News/India-Ramps-Up-Rail-Coal-Deliveries-as-Power-Plant-Stockpiles-Dwindle.html) ⭐️ 7.0/10

India’s Ministry of Coal said it is increasing rail coal deliveries to power plants after coal stocks at more than 50 plants fell below the critical level of 25% of normal requirements. The number of plants with critically low stocks rose to 53 as of September 5, from 45 on August 26, according to the Central Electricity Authority.

rss · OilPrice.com · Sep 7, 15:30

**「Background」** Coal is still India’s single largest electricity source, but monsoon disruptions and hotter-than-usual El Niño temperatures have raised power demand and squeezed domestic coal supply and transport.

**「Impact」** The tight coal stocks could increase the risk of power shortages for households and businesses if deliveries do not keep up with demand, though the coal ministry says corrective supply measures are in place.

**Tags**: `#coal`, `#India`, `#power sector`, `#energy security`, `#supply disruption`

---

<a id="item-finance-news-12"></a>
### [TSM Raises Guidance on Strong Demand for Advanced Chips](https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductor-manufacturing-company-tsm-142602670.html) ⭐️ 7.0/10

Taiwan Semiconductor Manufacturing Company \(TSM\) raised its financial outlook, citing strong demand for advanced chips. No specific figures were provided in the available coverage.

openbb · NVDA · Sep 7, 14:26

**「Background」** Taiwan Semiconductor Manufacturing Company \(TSMC\) is the world&\#x27;s largest dedicated chip foundry, holding roughly 70% market share and advanced manufacturing capabilities. The company raised its 2026 revenue growth guidance above 30% and increased its capital expenditure range to $60–64 billion from an initial $52–56 billion, citing surging AI-related demand for advanced chips.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/taiwan-semiconductor-manufacturing-company-tsm-142602670.html">Taiwan Semiconductor Manufacturing Company (TSM) Raises ...</a></li>
<li><a href="https://www.streetbrief.co/article/tsm-stock-revenue-guidance-surges-ai-demand-accelerates-2606/">TSM Stock: Revenue Guidance Surges As AI Demand Accelerates</a></li>
<li><a href="https://www.techtimes.com/articles/326625/20260904/tsmc-equipment-demand-doubled-fab-construction-workers-are-running-out.htm">TSMC Equipment Demand Doubled, But Fab Construction Workers...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Taiwan Semiconductor`, `#guidance`, `#AI demand`, `#earnings`

---