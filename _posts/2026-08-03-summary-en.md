---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 98 items, 12 important content pieces were selected

---

**Technology News**
1. [Qwen Announces Open-Weight Qwen 3.8-Max: 2.4T-Parameter MoE](#item-tech-news-1) ⭐️ 9.0/10
2. [Open letters: 235 firms defend open-weight AI, Anthropic cautions](#item-tech-news-2) ⭐️ 8.0/10
3. [Kakehashi: Experimental macOS Binary Runtime for Linux ARM](#item-tech-news-3) ⭐️ 7.0/10
4. [Apple Limits Bug Reports Amid AI-Generated Security Report Flood](#item-tech-news-4) ⭐️ 7.0/10

**Financial News**
1. [Fed Holds Rates Steady for Second Straight Meeting Under Warsh](#item-finance-news-1) ⭐️ 9.0/10
2. [Goldman Sachs on pace for record trading year as equities revenue jumps 72%](#item-finance-news-2) ⭐️ 8.0/10
3. [China Drafts Broader Housing Provident Fund Rules](#item-finance-news-3) ⭐️ 8.0/10
4. [Japan and US reportedly intervene to support yen near 40-year low](#item-finance-news-4) ⭐️ 8.0/10
5. [Earnings Week Ahead: SpaceX, Disney, AMD, McDonald&\#x27;s](#item-finance-news-5) ⭐️ 7.0/10
6. [Dow Jones Futures Rise; Oil Prices Dive as Trump Shifts on Iran, Major Earnings Loom](#item-finance-news-6) ⭐️ 7.0/10
7. [Bezos-Backed AI Startup Valued at $2.6 Billion Partners With Nvidia and Meta](#item-finance-news-7) ⭐️ 7.0/10
8. [Qualcomm&\#x27;s Q3 Results and Guidance May Reframe Its AI Investment Narrative](#item-finance-news-8) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen Announces Open-Weight Qwen 3.8-Max: 2.4T-Parameter MoE](https://qwen.ai/blog?id=qwen3.8) ⭐️ 9.0/10

Qwen announced Qwen 3.8-Max, a 2.4-trillion-parameter Mixture-of-Experts model with 95B active parameters, described as the strongest Qwen model yet and the first Max-tier weights release. Based on the Qwen 3.5 architecture, it targets coding, work, research, and long-horizon tasks; the team says it can autonomously run for over 10 days to build and self-evolve a project, and within 24 hours placed ahead of 458 of 526 teams in the WWW2025 multimodal dialogue intent recognition competition. The model weights are scheduled to open-source next week, and QwenCloud already offers it via API.

telegram · zaihuapd · Aug 3, 02:31

**「Background」** Qwen is Alibaba&\#x27;s flagship family of large language models, and its Max tier has historically represented the largest, most capable models, which were released only through APIs and not as downloadable weights. Qwen 3.8-Max, previewed on July 19, 2026, is a 2.4-trillion-parameter sparse Mixture-of-Experts \(MoE\) multimodal model with a 1M-token context window. The significance of the announcement is Alibaba&\#x27;s public commitment to open the model&\#x27;s weights, unlike the previous Qwen 3.7-Max and earlier Max-tier flagships. It lands in a week when Moonshot AI&\#x27;s Kimi K3 \(2.8T parameters\) also shipped as the largest open-weight model ever released, underscoring a shift toward open-weight giant models from Chinese AI labs.

**「Impact」** If the open-weights release happens as planned, researchers and developers outside QwenCloud will gain access to a Max-tier MoE model for the first time; API users can begin testing it immediately through QwenCloud.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/qwen38-max-review">Qwen 3 . 8 Max review: Alibaba&#x27;s 2 . 4 T flagship, tested (2026) | eesel AI</a></li>
<li><a href="https://saascity.io/blog/kimi-k3-vs-qwen38-max-china-trillion-parameter-open-models-2026">Kimi K3 vs Qwen 3 . 8 - Max : China Shipped Two Trillion - Parameter ...</a></li>
<li><a href="https://shaam.blog/articles/qwen-3-8-max-honest-review-2026">Qwen 3 . 8 Max : An Honest Review of Alibaba&#x27;s 2 . 4 T Parameter AI...</a></li>

</ul>
</details>

**Tags**: `#qwen`, `#large language models`, `#open-source`, `#Mixture-of-Experts`, `#AI research`

---

<a id="item-tech-news-2"></a>
### [Open letters: 235 firms defend open-weight AI, Anthropic cautions](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

Microsoft shepherded an open letter titled &\#x27;Open Weights and American AI Leadership,&\#x27; dated July 24, signed by 235 AI-adjacent companies including NVIDIA, Amazon, Y Combinator, The Linux Foundation, and later OpenAI, arguing against US government limits on open-weight models. The letter defends open-weight models as safer than concentrating capabilities in closed models, and explicitly supports distillation as a legitimate model-development technique. Anthropic did not sign and published &\#x27;Our position on open-weights models&\#x27; three days later, with CEO Dario Amodei warning about authoritarian governments and cyberattacks or biological attacks, while calling for a crackdown on industrial-scale distillation operations and stating Anthropic has never advocated for a ban on open-weights models. On July 28, &\#x27;Pacing the Frontier&\#x27; was published with signatures from 1,324 employees of frontier AI companies, including Jakub Pachocki, Ilya Sutskever, Dario Amodei, and Jack Clark, calling for an international effort to develop tools to deliberately pace the frontier of automated AI development.

rss · Simon Willison · Aug 2, 04:16

**「Background」** Open-weight models publish trained model weights so external researchers can inspect, modify, and build on them, unlike closed models whose internals remain proprietary. The letters respond to reported US government instincts to restrict open-weight models over safety concerns—such as a US government directive that suspended access to Claude Fable 5—and to rising worry about automated AI research accelerating frontier progress through techniques like distillation and AI-assisted coding.

**「Impact」** The most concrete consequence so far is the public commitment of 235 companies and 1,324 frontier-AI employees to these positions, giving US policymakers a record of industry alignment and opposition ahead of any restrictions, while the high-profile absence of Anthropic highlights a live industry split over open-weight releases and distillation practices.

**Tags**: `#AI policy`, `#open source`, `#open-weight models`, `#industry letters`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [Kakehashi: Experimental macOS Binary Runtime for Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi is an experimental userspace project by vlad\_kalinkin that aims to run macOS command-line binaries natively on Linux ARM systems. It currently has working prototypes for 7-Zip, which passes multithreaded compression tests on an 8,000-file tree at about 5.2x slower than native Linux execution; curl, with over 200 commands and options passing an automated Docker test script; and Xcode Tools Git, which supports basic version control. The project is still early-stage, but the author reports a clear optimization plan to reduce the performance gap. It is notable because it pursues macOS binary compatibility through a userspace implementation rather than a full OS-level compatibility layer.

hackernews · vlad\_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**「Background」** Running macOS binaries outside Apple hardware normally requires reimplementing the Mach-O executable format, the dyld dynamic linker, and macOS system libraries, since macOS uses different ABIs and APIs than Linux. Prior efforts such as Darling provide a compatibility layer for this purpose, and there is an open ARM64 pull request in that project; Kakehashi instead focuses specifically on Linux ARM userspace support.

**「Impact」** Linux ARM users and developers can now experimentally run select macOS CLI tools without macOS hardware, but the ~5.2x slowdown observed with 7-Zip and limited tool coverage mean the project is not yet practical for everyday use.

**「Community Discussion」** Commenters drew parallels to WINE/Proton and asked whether the author plans to coordinate with Darling, which has an open ARM64 PR; one called the project promising but early-stage, while another criticized the name.

**Tags**: `#macOS compatibility`, `#Linux ARM`, `#userspace`, `#binary translation`, `#experimental`

---

<a id="item-tech-news-4"></a>
### [Apple Limits Bug Reports Amid AI-Generated Security Report Flood](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

Apple has restricted the number of vulnerability reports security researchers can submit at once, imposing a 30-day cooldown period since June to handle a surge of low-quality reports generated by AI models. The change was confirmed by Apple after Italian security startup Bynario said it used ChatGPT to discover more than 50 vulnerabilities in the latest macOS within three weeks, including privilege escalation chains that could let attackers take full control of a computer, but was unable to report them because of the submission quota. Apple said it has contacted Bynario and reviewed its submissions. Apple also said it is using AI to strengthen its own defenses, and this week&\#x27;s system security update fixed roughly five times as many vulnerabilities as usual, crediting tools from Anthropic and OpenAI for helping find the bugs.

telegram · zaihuapd · Aug 2, 05:50

**「Background」** Vulnerability reporting programs, such as Apple&\#x27;s bug bounty, depend on researchers submitting detailed reports so vendors can patch flaws before they are exploited. The rise of AI-generated security reports has overwhelmed these systems with low-quality or duplicate submissions, prompting vendors to limit report volumes and seek AI assistance for detection.

**「Impact」** Security researchers now face reduced submission quotas and cooldown periods, which may delay disclosure of legitimate vulnerabilities even as Apple accelerates its own AI-assisted patching, leaving affected macOS users caught between slower external reporting and faster internal fixes.

**Tags**: `#Apple`, `#AI security`, `#vulnerability reporting`, `#macOS`, `#ChatGPT`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed Holds Rates Steady for Second Straight Meeting Under Warsh](https://finance.yahoo.com/economy/policy/articles/fed-held-interest-rates-steady-015000677.html) ⭐️ 9.0/10

The Federal Reserve kept interest rates unchanged for a second consecutive meeting under Kevin Warsh, with three officials dissenting, according to the report. No further details on the rate level or the dissenting officials&\#x27; positions were provided.

openbb · NVDA · Aug 3, 01:50

**「Background」** The Federal Open Market Committee \(FOMC\), the Fed&\#x27;s rate-setting body, left its benchmark interest rate at 3.5% to 3.75%, and Chairman Kevin Warsh reiterated the Fed&\#x27;s commitment to its 2% inflation target. Three regional Fed presidents dissented, voting instead for a quarter-point rate hike amid concerns that inflation could persist.

**「Impact」** Investors now expect a quarter-point rate increase in September, and long-term Treasury yields have already moved higher, which can feed into costlier borrowing for households and businesses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/tylerroush/2026/07/29/fed-keeps-interest-rates-unchanged-as-dissent-mounts/">Kevin Warsh’s Fed Holds Interest Rates Steady Again—But Dissent Among Officials Mounts</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/fed-meeting-today-live-updates.html">Fed meeting recap: Warsh says Fed won&#x27;t hesitate to stop inflation, but bond market has doubts</a></li>
<li><a href="https://www.cnn.com/2026/07/29/business/live-news/federal-reserve-interest-rate-07-29-26">Fed holds interest rates steady after cliffhanger meeting, but three officials dissent | CNN Business</a></li>
<li><a href="https://www.cnbc.com/2026/07/29/kevin-warsh-fed-treasury-yields-inflation-credibility-interest-rates.html">Analysis: Fed Chairman Warsh&#x27;s credibility in question after leaving interest rates unchanged</a></li>
<li><a href="https://www.nytimes.com/live/2026/07/29/business/fed-meeting-rates-kevin-warsh">Fed Leaves Interest Rates Unchanged, Despite Three Votes for an Increase - The New York Times</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Kevin Warsh`, `#Dissents`

---

<a id="item-finance-news-2"></a>
### [Goldman Sachs on pace for record trading year as equities revenue jumps 72%](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

Goldman Sachs is on pace for a record trading year: equities revenue jumped 72% to a record $7.42 billion in the second quarter, and the Global Banking &amp; Markets unit generated $15.5 billion, over 75% of the bank&\#x27;s total revenue.

rss · CNBC Finance · Aug 2, 13:52

**「Background」** The growth came from a strategy shift within Global Banking &amp; Markets that pushes clients who use investment banking or wealth management to also use Goldman&\#x27;s equities services, with fees from SpaceX&\#x27;s IPO and Alphabet&\#x27;s $85 billion equity raise contributing to investment banking revenue.

**Tags**: `#Goldman Sachs`, `#equities trading`, `#earnings`, `#investment banking`, `#market volatility`

---

<a id="item-finance-news-3"></a>
### [China Drafts Broader Housing Provident Fund Rules](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 8.0/10

China&\#x27;s housing regulator has published a draft revision to the Housing Provident Fund regulations for public comment, proposing that flexible workers such as self-employed people, delivery riders and ride-hailing drivers may contribute voluntarily, and that members may withdraw funds for home renovation and property management fees.

telegram · zaihuapd · Aug 2, 06:32

**「Background」** The current fund system is generally tied to formal employment, and withdrawals have typically been limited to buying or renting a home, so the draft would expand fund use to repairing and maintaining homes and add mutual recognition of fund records across regions.

**「Impact」** If adopted, this could give gig-economy workers a route into the fund and give current contributors more flexibility in using accumulated savings for housing-related expenses.

**Tags**: `#housing`, `#policy`, `#China`, `#provident fund`, `#flexible employment`

---

<a id="item-finance-news-4"></a>
### [Japan and US reportedly intervene to support yen near 40-year low](https://www.zaobao.com.sg/news/world/story20260802-9457369) ⭐️ 8.0/10

Japan and the US have reportedly intervened jointly to buy yen as the currency neared a 40-year low of about ¥164 per dollar. Japan&\#x27;s finance minister is expected to announce the move on August 3, and market sources cite planned purchases of $5 billion to $10 billion.

telegram · zaihuapd · Aug 3, 01:29

**「Background」** Japan and the U.S. confirmed a coordinate yen-buying intervention on Friday, their first joint action in about 30 years, to halt the yen’s slide to 40-year lows. The finance ministry signaled readiness to take further action if needed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.japantimes.co.jp/business/2026/08/03/markets/japan-us-joint-yen-intervention/">Japan confirms joint yen intervention with U.S., signaling readiness for more action - The Japan Times</a></li>
<li><a href="https://www.cnbc.com/2026/08/03/yen-intervention-us-japan-trump-bessent-katayama.html">U.S., Japan confirm coordinated yen intervention, signal readiness for more</a></li>
<li><a href="https://www.chosun.com/english/market-money-en/2026/08/02/TDIKXF57NZEEBPPGI72QI7ALSQ/">U.S. and Japan Intervene to Buy Yen for First Time in 30 Years</a></li>

</ul>
</details>

**Tags**: `#forex`, `#yen`, `#Japan`, `#US`, `#intervention`

---

<a id="item-finance-news-5"></a>
### [Earnings Week Ahead: SpaceX, Disney, AMD, McDonald&\#x27;s](https://finance.yahoo.com/video/earnings-watch-week-spacexs-first-180000072.html) ⭐️ 7.0/10

This week&\#x27;s earnings preview highlights upcoming reports from SpaceX \(its first\), Disney, AMD, and McDonald&\#x27;s; no figures or results have been released yet.

openbb · NVDA · Aug 2, 18:00

**「Background」** SpaceX, Elon Musk’s rocket and satellite company, is expected to report its first quarterly earnings on Aug. 4, 2026, according to CNBC; that date also triggers a major lock-up expiration for early investors. Morningstar data cited in reports shows SpaceX had about $18.7 billion in sales but lost nearly $5.0 billion in 2025, and lost roughly $4.28 billion in Q1 2026; several other big consumer and tech names, including Disney, AMD, McDonald’s, Spotify, Paramount Skydance, and Wendy’s, are also reporting this week.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/21/spacex-spcx-earnings-lock-up-expiration.html">SpaceX snaps 7-day losing streak, sets earnings date that triggers first big share unlock</a></li>
<li><a href="https://www.investopedia.com/what-to-expect-in-markets-this-week-spacex-s-first-earnings-report-earnings-from-chip-and-memory-giants-spcx-elon-musk-12031285">What to Expect in Markets this Week: SpaceX’s First Earnings Report; Earnings From Chip and Memory Giants</a></li>
<li><a href="https://www.morningstar.com/stocks/5-charts-what-watch-spacex-earnings">5 Charts on What to Watch in SpaceX Earnings | Morningstar</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#SpaceX`, `#Disney`, `#AMD`, `#McDonald&\#x27;s`

---

<a id="item-finance-news-6"></a>
### [Dow Jones Futures Rise; Oil Prices Dive as Trump Shifts on Iran, Major Earnings Loom](https://www.investors.com/market-trend/stock-market-today/dow-jones-futures-spacex-amd-sandisk-eli-lilly-earnings-loom/?src=A00220&amp;yptr=yahoo) ⭐️ 7.0/10

According to Investor&\#x27;s Business Daily, Dow Jones futures rose while oil prices fell sharply after President Trump shifted his stance on Iran, with upcoming earnings from AMD, Sandisk, and Eli Lilly also in focus.

openbb · NVDA · Aug 3, 01:59

**「Background」** Earlier reports of a threatened U.S. strike on Iran had pushed oil prices sharply higher; the reported shift in President Trump&\#x27;s stance is the immediate context for the current drop. Several major companies, including AMD, SanDisk, and Eli Lilly, are scheduled to release quarterly earnings in the coming days.

<details><summary>References</summary>
<ul>
<li><a href="https://oilprice.com/">Crude Oil Prices Today | OilPrice .com</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262068819-weekly-preview-us-july-non-farm-payrolls-data-market-focus-pltr-sandisk-amd-spacex-earnings-reports-tradingkey">The Week Ahead: US July Non-Farm Payrolls in Focus; PLTR, SanDisk, AMD, and SpaceX Earnings Ahead</a></li>

</ul>
</details>

**Tags**: `#Oil Prices`, `#Iran Policy`, `#Earnings`, `#Stock Market`, `#Dow Jones`

---

<a id="item-finance-news-7"></a>
### [Bezos-Backed AI Startup Valued at $2.6 Billion Partners With Nvidia and Meta](https://finance.yahoo.com/technology/ai/articles/jeff-bezos-backed-2-6-233300700.html) ⭐️ 7.0/10

A Jeff Bezos-backed AI startup has been valued at $2.6 billion and is partnering with Nvidia and Meta to develop new chip materials.

openbb · NVDA · Aug 2, 23:33

**「Background」** The startup is CuspAI, which raised $450 million in private funding, valuing it at $2.6 billion, with backing from Jeff Bezos&\#x27; venture fund Bezos Expeditions; it is working with Nvidia and Meta to use AI to discover next-generation chip materials.

**「Impact」** For semiconductor manufacturers, CuspAI&\#x27;s partnerships with Nvidia and Meta could speed up the discovery of next-generation chip materials and reduce the time and cost required to identify them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/02/jeff-bezos-backed-a-26-billion-ai-startup-thats-pa/">Jeff Bezos Backed a $2.6 Billion AI Startup That&#x27;s Partnering With Nvidia and Meta on New Chip Materials | The Motley Fool</a></li>
<li><a href="https://www.benzinga.com/markets/private-markets/26/07/60549441/jeff-bezos-backs-2-6-billion-ai-startup-teaming-up-with-nvidia-and-meta-to-tackle-one-of-the-chip-industrys-biggest-challenges">Jeff Bezos Backs $2.6 Billion AI Startup Teaming Up With Nvidia and Meta to Tackle One of the Chip Indust - Benzinga</a></li>
<li><a href="https://www.cnbc.com/2026/07/20/bezos-cuspai-new-chip-materials-nvidia.html">Bezos backs CuspAI as startup hunts for new chip materials ...</a></li>
<li><a href="https://www.flowerclaw.tech/en/articles/meta-nvidia-ai-materials-semiconductor-discovery-en">Meta and Nvidia Back AI Materials Startup: How AI Is ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/nvidia-meta-join-bezos-backed-124650337.html?fr=sycsrp_catchall">Nvidia, Meta Join Bezos-Backed AI Startup Speed Next ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#semiconductors`, `#startups`, `#Nvidia`, `#Meta`

---

<a id="item-finance-news-8"></a>
### [Qualcomm&\#x27;s Q3 Results and Guidance May Reframe Its AI Investment Narrative](https://news.google.com/rss/articles/CBMi0gFBVV95cUxQcUZwUjdtX2tIN3NUbmFrSnEwRDFKZC1EMmpkVmxHd0JjVmxxM0k5QjNsU1JmeXBBN1VJaFBNdGJJTTVVQzA2SVhwYklzTXRTWVBfRFNEZ0MxVWNLR214X1M3cXY1c1lwcnRSQWxEM295TUwzbGp4eV95ZDUxRTZ2NkFzOS0xcDd6dUFRMXROZ0dzTi1EbjhoZ2tOOExMakNOZEdZOVpMX0hVaUMtOXFFZFMzRGRUY0puUU1fYnNDdjlTY0d6QjMyNHFabXNXTUZfUWfSAdIBQVVfeXFMUHFGcFI3bV9rSDdzVG5ha0pxMEQxSmQtRDJqZFZsR3dCY1ZscTNJOUIzbFNSZnlwQTdVSWhQTXRiSU01VUMwNklYcGJJc010U1lQX0RTRGdDMVVjS0dteF9TN3F2NXNZcHJ0UkFsRDNveU1MM2xqeHlfeWQ1MUU2djZBczktMXA3enVBUTF0TmdHc04tRG44aGdrTjhMTGpDTmRHWTlaTF9IVWlDLTlxRWRTM0RkVGNKblFNX2JzQ3Y5U2NHekIzMjRxWm1zV01GX1Fn?oc=5) ⭐️ 7.0/10

According to an analysis by simplywall.st, Qualcomm&\#x27;s Q3 results and guidance may be reshaping its AI-first investment narrative, though the article does not provide specific figures.

google\_news · simplywall.st · Aug 2, 10:23

**「Background」** Qualcomm announced its fiscal third-quarter 2025 results, saying its leadership in AI processing, high-performance computing, and connectivity positions it to become the industry platform of choice as AI scales at the edge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qualcomm.com/news/releases/2025/07/qualcomm-announces-third-quarter-fiscal-2025-results">Qualcomm Announces Third Quarter Fiscal 2025 Results</a></li>

</ul>
</details>

**Tags**: `#Qualcomm`, `#Q3 earnings`, `#guidance`, `#AI`, `#semiconductors`

---