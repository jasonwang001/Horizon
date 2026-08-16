---
layout: default
title: "Horizon Summary: 2026-08-17 (EN)"
date: 2026-08-17
lang: en
---

> From 150 items, 16 important content pieces were selected

---

**Technology News**
1. [Anthropic Publishes Claude System Prompts, Enabling Model Behavior Comparison](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B is strong but defaults to overthinking](#item-tech-news-2) ⭐️ 8.0/10
3. [SSOG-Attention: Sub-Quadratic Sum-of-Separable-Gaussians Alternative to SDPA](#item-tech-news-3) ⭐️ 7.0/10

**Financial News**
1. [Fed’s Upcoming Meeting Is Seen as Highly Unpredictable](#item-finance-news-1) ⭐️ 9.0/10
2. [Eight Oil Majors Reap More Than $90 Billion in Q2 Profits as Hormuz Closure Spurs Prices](#item-finance-news-2) ⭐️ 8.0/10
3. [Anthropic&\#x27;s preliminary Q2 revenue tops $11.5 billion, up 14x year over year](#item-finance-news-3) ⭐️ 8.0/10
4. [NVIDIA Announces $3 Billion Investment in AI Power Infrastructure](#item-finance-news-4) ⭐️ 8.0/10
5. [Greg Abel Put Nearly $35 Billion of Cash to Work at Berkshire Hathaway](#item-finance-news-5) ⭐️ 8.0/10
6. [Fed leaves rates unchanged at July meeting](#item-finance-news-6) ⭐️ 8.0/10
7. [Fed Chair Kevin Warsh testifies on inflation and monetary policy in House hearing](#item-finance-news-7) ⭐️ 8.0/10
8. [U.S. Says Middle East Oil Flows Rebounded, but Ship Data Disagree](#item-finance-news-8) ⭐️ 7.0/10
9. [Europe Faces Lowest Natural Gas Storage Levels in 17 Years Ahead of Winter](#item-finance-news-9) ⭐️ 7.0/10
10. [AI Boom Is Raising Big Tech Emissions and Could Extend Fossil Fuel Dominance](#item-finance-news-10) ⭐️ 7.0/10
11. [AMD Raises $4.75 Billion in Bond Sale](#item-finance-news-11) ⭐️ 7.0/10
12. [Gold Reaches $4,400 and Mining Stocks Rally](#item-finance-news-12) ⭐️ 7.0/10
13. [Kraft, McDonald’s and Whirlpool CEOs warn US consumers are ‘running out of money’](#item-finance-news-13) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic Publishes Claude System Prompts, Enabling Model Behavior Comparison](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic has published the system prompts used by Claude models in its release notes, a transparency step that lets researchers and developers inspect and compare the instructions shaping Claude&\#x27;s behavior across versions. The dumps include prompts for models such as Opus 4.8 and Opus 5; community members have already turned them into git commit histories to track diffs over time. One notable addition in the Opus 5 prompt references Claude Fable 5 and Claude Mythos 5, while another instructs Claude to verify whether an image is actually present rather than trust an assertion in the conversation. This kind of disclosure is practically relevant for prompt engineers and AI researchers because it turns prompt changes into observable, versionable artifacts rather than hidden implementation details.

hackernews · tosh · Aug 16, 12:48 · [Discussion](https://news.ycombinator.com/item?id=49319556)

**「Background」** Anthropic publishes the system prompts used by Claude&\#x27;s web and mobile apps as part of its release notes, updating them with each model release. These prompts are instructions given to Claude at the start of every conversation, providing up-to-date information such as the current date and shaping behavior around tone, format, and safety guidelines. The release notes therefore offer a transparent look at how Anthropic adjusts model behavior over time.

**「Impact」** The publication gives prompt engineers and researchers a concrete, versioned record of how Anthropic tunes Claude&\#x27;s behavior, enabling diff-based analysis of new releases instead of guessing from output changes alone. It also offers early visibility into planned model-behavior directions such as stronger crisis-response priorities.

**「Community Discussion」** Commenters welcomed the transparency, with Simon Willison providing a git history of the prompts and highlighting the Opus 4.8-to-Opus 5 diff. Others expressed skepticism that Anthropic relies on system-prompt wording for common-sense checks like verifying uploaded images, and one user raised concerns about HN moderation of AI-critical stories, while another reminded readers that system prompts are only one layer of a larger behavior-shaping system.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs</a></li>
<li><a href="https://tactiq.io/learn/claude-system-prompt">Claude System Prompt Explained: What&#x27;s Inside and Why It Matters</a></li>
<li><a href="https://simonwillison.net/2025/May/25/claude-4-system-prompt/">Highlights from the Claude 4 system prompt</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#System Prompts`, `#Transparency`, `#Prompt Engineering`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B is strong but defaults to overthinking](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

Alibaba&\#x27;s Qwen lab released Qwen 3.8 27B, an Apache 2 licensed 27B-parameter vision-capable LLM, with self-reported benchmarks ahead of Qwen 3.6 27B and the closed Qwen 3.7-Plus. Early testing by Simon Willison on a 128GB M5 Max MacBook Pro and an NVIDIA DGX Spark used LM Studio&\#x27;s 17GB Q4\_K\_M quantized build, and he found the model impressive but hampered by a default reasoning\_effort of xhigh. Under that default, the model can overthink even simple prompts: one pelican SVG request consumed 22,276 reasoning tokens and took 21 minutes, while the same prompt without reasoning produced 3,715 tokens in 137 seconds. Willison had to increase the context from 8,192 to 262,144 tokens to avoid exhaustion and recommends running Qwen 3.8 27B with low or no reasoning first.

rss · Simon Willison · Aug 16, 22:00

**「Background」** Qwen 3.8 27B is the latest in Alibaba&\#x27;s Qwen family of open-weight models, sized to run locally on high-end laptops; its predecessor Qwen 3.6 27B was already notable, and Qwen 3.7-Plus was a strong closed model released in May. Reasoning effort is a model setting that controls how much chain-of-thought token budget the model uses before answering: xhigh is intended for complex tasks, while low and off prioritize speed and cost.

**「Impact」** Developers running the quantized local build should change reasoning\_effort away from the default xhigh to avoid spending minutes and exhausting context on trivial prompts, while still benefiting from the model&\#x27;s strong local vision and SVG-generation abilities.

**Tags**: `#Qwen`, `#LLM`, `#open source`, `#AI benchmarks`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [SSOG-Attention: Sub-Quadratic Sum-of-Separable-Gaussians Alternative to SDPA](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 7.0/10

The author introduces SSOG-Attention, a sum-of-separable-Gaussians attention mechanism designed as a sub-quadratic alternative to scaled dot-product attention \(SDPA\). Instead of computing similarity scores for all token pairs, SSOG learns Gaussian atoms for each head and geometrically steers them based on the query token, factorizing the attention computation into a separable sum that reduces complexity from O\(N²·d\) to O\(N·√N·d\). Experiments reported by the author show that SSOG clearly outperforms SDPA on CIFAR-100, achieves equivalent performance on ImageNet \(IN1k\), and converges much faster while being more memory efficient at larger scales. The work includes a blog post and a public repository, and the author notes that AI was used for some code and writing but that they stand behind the project.

reddit · r/MachineLearning · /u/4rtemi5 · Aug 16, 10:06

**「Background」** Scaled dot-product attention \(SDPA\) computes attention as the dot-product similarity between all query and key tokens, which grows quadratically with the number of tokens and limits scalability for large images or long sequences. SSOG-Attention instead approximates attention with a sum of separable Gaussian functions, which can be factorized along spatial dimensions to avoid explicit all-pairs computation while still allowing query-dependent steering.

**「Impact」** For practitioners training vision models on large inputs, SSOG-Attention offers a concrete way to cut attention complexity from quadratic to O\(N·√N·d\) while maintaining accuracy on ImageNet-scale benchmarks and improving accuracy on smaller datasets such as CIFAR-100.

**Tags**: `#attention mechanism`, `#efficient attention`, `#machine learning`, `#computer vision`, `#Gaussian kernels`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed’s Upcoming Meeting Is Seen as Highly Unpredictable](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 9.0/10

The Federal Reserve is heading into one of its most unpredictable policy meetings in years, according to The Wall Street Journal, with the path of interest rates seen as highly uncertain.

google\_news · WSJ · Jul 23, 07:00

**「Background」** The Federal Reserve’s next meeting is described by the Wall Street Journal as one of its most unpredictable in years; that backdrop includes a new Fed chairman, Kevin Warsh, pressure from the president to lower rates, and inflation that has run above the Fed’s 2% target since 2021.

**「Impact」** The Fed&\#x27;s Sept. 17 statement lowered the interest rate paid on reserve balances to 4.15%, and a market analysis says the cut can affect global assets including gold, silver, and exchange rates.

<details><summary>References</summary>
<ul>
<li><a href="https://abc3340.com/news/nation-world/economy-bringing-mixed-messages-ahead-of-next-federal-reserve-meeting-policy-stock-market-artificial-intelligence">Economy bringing mixed messages ahead of next federal reserve ...</a></li>
<li><a href="https://www.dailywire.com/news/fed-holds-rates-after-its-most-unpredictable-meeting-of-the-year">Fed Holds Rates After Its Most Unpredictable Meeting Of The Year</a></li>
<li><a href="https://www.federalreserve.gov/monetarypolicy/files/monetary20250917a1.pdf">Federal Reserve issues FOMC statement</a></li>
<li><a href="https://www.markets.com/analysis/fed-rate-decision-september-2025-global-market-impact-1054-en">Fed Rate Decision September 2025: Impact of Rate Cuts on ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#economy`, `#markets`

---

<a id="item-finance-news-2"></a>
### [Eight Oil Majors Reap More Than $90 Billion in Q2 Profits as Hormuz Closure Spurs Prices](https://oilprice.com/Energy/Energy-General/Oil-Majors-Reap-93-Billion-Windfall-From-the-Iran-War.html) ⭐️ 8.0/10

Eight of the largest oil companies earned combined profits of more than $90 billion in Q2 2025, after the Iran war and near-total closure of the Strait of Hormuz drove oil prices sharply higher and renewed debate over windfall taxes on oil profits.

rss · OilPrice.com · Aug 16, 19:00

**「Background」** The Strait of Hormuz, the waterway between Iran and Oman that connects the Persian Gulf with global markets, was almost completely shut after a U.S.-Israeli attack on Iran and the war that followed; the article calls it the biggest disruption of fossil fuel supplies in market history.

**「Impact」** The price surge is raising household energy bills worldwide, and governments are considering windfall taxes on oil companies to help subsidize those bills, while environmentalists say the extra revenue could help pay for climate damage.

**Tags**: `#oil prices`, `#Strait of Hormuz`, `#oil majors`, `#energy profits`, `#geopolitical risk`

---

<a id="item-finance-news-3"></a>
### [Anthropic&\#x27;s preliminary Q2 revenue tops $11.5 billion, up 14x year over year](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

Bloomberg, citing documents, reported that Anthropic&\#x27;s preliminary second-quarter revenue exceeded $11.5 billion, up more than 14 times from $787 million a year earlier and above $4.73 billion in the first quarter of 2026, with adjusted operating profit turning positive. The figures are preliminary and may change as the company prepares for a possible IPO this fall.

telegram · zaihuapd · Aug 16, 07:26

**「Background」** Anthropic is a privately held AI safety company best known for building the Claude AI assistant and the Claude Code developer tool. It has not formally announced an IPO, though the reported revenue figures are described as preliminary and tied to a potential public listing later this year.

**「Impact」** The preliminary revenue surge could bolster Anthropic&\#x27;s planned IPO, and reports say the filing may set a valuation benchmark that influences AI-sector investors, including those in ASX-listed AI shares.

<details><summary>References</summary>
<ul>
<li><a href="https://forgeglobal.com/insights/how-to-invest-in-anthropic-pre-ipo/">Insights: How to Invest in Anthropic Pre-IPO - Forge</a></li>
<li><a href="https://listenlabs.ai/case-studies/anthropic">Anthropic &amp; Listen Labs | Customer Stories</a></li>
<li><a href="https://www.bnnbloomberg.ca/investing/investor-outlook/2026/06/03/investor-outlook-anthropic-ipo-filing-heats-up-ai-industry-race/">Anthropic filing puts spotlight on AI valuations</a></li>
<li><a href="https://www.fool.com.au/2026/06/10/the-spacex-and-anthropic-ipos-will-massively-impact-asx-ai-shares/">The SpaceX and Anthropic IPOs will massively impact ASX AI shares</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#revenue growth`, `#AI industry`, `#IPO`, `#earnings`

---

<a id="item-finance-news-4"></a>
### [NVIDIA Announces $3 Billion Investment in AI Power Infrastructure](https://finance.yahoo.com/technology/ai/articles/nvidia-3-billion-bet-power-202314612.html) ⭐️ 8.0/10

NVIDIA announced a $3 billion investment aimed at the power infrastructure that supports artificial intelligence.

openbb · NVDA · Aug 16, 20:23

**「Background」** Nvidia plans to invest up to $3 billion in Lancium, a Texas-based developer that builds power infrastructure and land for data center sites, to secure electricity for AI computing, including the Stargate campus that consumes 1.2 gigawatts.

**「Impact」** The $3 billion investment is part of NVIDIA&\#x27;s collaboration with energy leaders to address grid constraints for AI factories, including hybrid projects that use co-located power to accelerate time to power, directly affecting energy providers and data center operators.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gurufocus.com/news/9020455/nvidia-to-invest-3-billion-in-lancium-for-ai-infrastructure-development-nvda">Nvidia to Invest $3 Billion in Lancium for AI Infrastructure Development (NVDA)</a></li>
<li><a href="https://datacenters.economictimes.indiatimes.com/news/ai-compute-infrastructure/nvidia-invests-3-billion-in-lancium-for-ai-power-access/133141093">Nvidia invests $3 billion in Lancium for AI power access, ETDatacenters</a></li>
<li><a href="https://truescho.com/en/blog/nvidia-stargate-lancium-3-billion-ai-infrastructure-2026">Nvidia $3B Stargate Investment 2026: AI Infrastructure | Truescho</a></li>
<li><a href="https://blogs.nvidia.com/blog/energy-efficiency-ai-factories-grid/">NVIDIA, Energy Leaders Accelerating Power‑Flexible AI ...</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#AI`, `#investment`, `#energy`, `#data centers`

---

<a id="item-finance-news-5"></a>
### [Greg Abel Put Nearly $35 Billion of Cash to Work at Berkshire Hathaway](https://finance.yahoo.com/markets/stocks/articles/warren-buffetts-successor-greg-abel-102200832.html) ⭐️ 8.0/10

Greg Abel, the Berkshire Hathaway executive set to succeed Warren Buffett, deployed nearly $35 billion in cash during the latest quarter, according to the report, which says it details the purchases he made.

openbb · BRK-B · Aug 16, 10:22

**「Background」** Berkshire Hathaway’s Greg Abel, Warren Buffett’s successor as CEO, put nearly $35 billion to work last quarter across marketable equities, acquisitions, and share repurchases, breaking a streak of net selling and marking a more active deployment of Berkshire’s cash pile. Known details include roughly $10 billion invested in Alphabet \(Google’s parent\) and about $4.5 billion in Berkshire share buybacks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.com/en-us/money/top-stocks/warren-buffett-s-successor-greg-abel-put-nearly-35-billion-of-cash-to-work-last-quarter-here-s-what-he-bought/ar-AA2adZZH">Warren Buffett&#x27;s successor, Greg Abel, put nearly $35 billion of ... - MSN</a></li>
<li><a href="https://apnews.com/article/berkshire-hathaway-warren-buffett-greg-abel-buybacks-e36ed92787eef9c9c67502501b345174">Berkshire Hathaway CEO Greg Abel spends cash on buybacks | AP News</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#Greg Abel`, `#Capital Allocation`, `#Portfolio Management`, `#Investment Strategy`

---

<a id="item-finance-news-6"></a>
### [Fed leaves rates unchanged at July meeting](https://news.google.com/rss/articles/CBMiiwFBVV95cUxNUVVUMW1Hb2g1N2cyQkJneFl4YXJ1aFVvOGQzX19Oc2IxZUFyVUcwOXI0VmlpaW04d0N0MWZxVFlhSkJLUTltY3VxOVVHVGFBZHc5eVRzUTRQN1FXSEQ1Qm16U1pJMC1rOHNSdFd6UTEyWTF4cUpjX3NJUGs1alI3VGtLSmdNZmpOdjM0?oc=5) ⭐️ 8.0/10

At its July meeting, the Federal Reserve decided to keep interest rates unchanged, a decision that was closely watched.

google\_news · Fortune · Jul 29, 07:00

**「Background」** The Federal Reserve&\#x27;s rate-setting committee left its benchmark interest rate unchanged again, continuing a pause in a period when inflation has stayed above the central bank&\#x27;s 2% target and officials are weighing the economic impact of tariffs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-29-2026">July FOMC: Fed holds interest rates steady | Fox Business</a></li>
<li><a href="https://www.foxbusiness.com/economy/federal-reserve-interest-rate-decision-july-2025">Federal Reserve leaves key interest rate unchanged for fifth straight ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#central bank`, `#economy`

---

<a id="item-finance-news-7"></a>
### [Fed Chair Kevin Warsh testifies on inflation and monetary policy in House hearing](https://news.google.com/rss/articles/CBMitwFBVV95cUxNNGoza1B1bFlYakZUZTlfMDZXQW5lak5PUUJmazNOUTZXdzZsb0ZfaUdNRmRZSmRHQmVLM1YweXBYaG5QWko3UE9pWk13MThsazJXZnAxZXQzdjFBNS1JQndtTU5WYzNjbExBWFVmaHRiUGlzNVB6WW9yTmdwQWdyWGNvWktMMWpQcXZrVWFtVGxwYW5WUEY1WEhJUWw2MTFfaFFBREMxQkVfUmx6WGVsNzZoU1AwYjjSAbwBQVVfeXFMTmJaLU9CcDhYZjVFbnJ1OEk5MFdNTzNNNlNQcjZTNnBndmtVMUFaaGVhYVZaR05MMnVKekp6NmlLdXZRbUwyUEdmLUZvT3h1bkVsVEZoR0k3MFN2QXIxTmY5bUtPdVVBODgwMHBiSDlqbl96VU9xSHppMGY4Q1M1VTVRVXl3VldVQ1dMTHoxNndVcDd5VEUySWZhSmU1RWtsSVpvUFVWWkI5T3Bfdy1FWHN2Zy1GT0R4UnhmN1M?oc=5) ⭐️ 8.0/10

PBS is broadcasting Federal Reserve Chair Kevin Warsh’s testimony on inflation and monetary policy before a House hearing.

google\_news · PBS · Jul 13, 07:00

**「Background」** This is Kevin Warsh&\#x27;s first semiannual monetary-policy testimony to Congress as Federal Reserve chair, a regular hearing where the Fed updates lawmakers on inflation and interest rates.

**「Impact」** Investopedia reports that markets have increasingly priced in rate hikes after Warsh pledged to restore 2% inflation, which could raise borrowing costs for households and businesses and affect investment portfolios.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/newsevents/testimony/warsh20260714a.htm">Testimony by Chairman Warsh on the semiannual Monetary Policy ...</a></li>
<li><a href="https://cryptobriefing.com/warsh-monetary-policy-report-house-committee/">Federal Reserve Chairman Warsh presents first Monetary Policy ...</a></li>
<li><a href="https://www.investopedia.com/new-fed-chair-kevin-warsh-declines-forward-guidance-yet-his-inflation-stance-sent-a-clear-signal-12001496">New Fed Chair Kevin Warsh Is Squarely Focused on Inflation ...</a></li>
<li><a href="https://www.lpl.com/research/weekly-market-commentary/kevin-warsh-could-shake-up-fed.html">Kevin Warsh and the Fed&#x27;s Shifting Policy Approach</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Congressional Hearing`

---

<a id="item-finance-news-8"></a>
### [U.S. Says Middle East Oil Flows Rebounded, but Ship Data Disagree](https://oilprice.com/Energy/Crude-Oil/Have-Middle-East-Oil-Flows-Rebounded-to-15-Million-Bpd-as-US-Claims.html) ⭐️ 7.0/10

U.S. Energy Secretary Chris Wright claimed Middle East oil exports have rebounded to 15 million barrels per day and that Sunday&\#x27;s flows topped the 20-million-bpd pre-war average, but independent ship-tracking firms estimate regional exports at only about 9–10 million bpd this month.

rss · OilPrice.com · Aug 16, 23:00

**「Background」** The Strait of Hormuz is a narrow oil-export chokepoint, and the U.S. Energy Information Administration says traffic there remains severely constrained after the conflict in Iran and stalled U.S.–Iran talks; the U.S. official says private trackers miss ships moving covertly, but the gap remains unexplained.

**Tags**: `#Oil exports`, `#Middle East`, `#Energy policy`, `#Gasoline prices`, `#Tanker tracking`

---

<a id="item-finance-news-9"></a>
### [Europe Faces Lowest Natural Gas Storage Levels in 17 Years Ahead of Winter](https://oilprice.com/Energy/Natural-Gas/Europes-Gas-Storage-Crunch-Deepens-Ahead-of-Heating-Season.html) ⭐️ 7.0/10

European gas storage is at its lowest level in 17 years less than three months before the heating season, and available supply is tighter than in 2022. Natural gas prices are about twice as high as before the Feb. 28 U.S.-Israeli strike on Iran, and the article says Europe will likely pay high prices for winter gas.

rss · OilPrice.com · Aug 16, 21:00

**「Background」** The EU shifted most of its gas purchases to U.S. and Qatari LNG after sanctions cut Russian pipeline supplies, and from January a new EU ban will halt purchases of Russian LNG after a record year of such imports.

**「Impact」** Higher winter gas costs would add further pressure on European households, businesses, and already strained economies as electricity prices are already high.

**Tags**: `#natural gas`, `#Europe`, `#energy security`, `#LNG`, `#sanctions`

---

<a id="item-finance-news-10"></a>
### [AI Boom Is Raising Big Tech Emissions and Could Extend Fossil Fuel Dominance](https://oilprice.com/Energy/Energy-General/AI-Set-to-Extend-Fossil-Fuel-Dominance.html) ⭐️ 7.0/10

Google and Microsoft each reported a 25% year-over-year rise in total carbon emissions from 2025 to 2026, and Amazon reported a 16% rise, according to figures cited by Oilprice.com; an NPJ Climate Action study warns that AI&\#x27;s net effect will likely increase fossil fuel use unless policy steers it.

rss · OilPrice.com · Aug 16, 17:00

**「Background」** AI data centers are expanding faster than clean-energy supplies, prompting Amazon to plan a natural-gas power plant in South Texas that would be permitted to release 33 million tons of CO2 a year if built as specified, according to the report.

**「Impact」** The study estimates that if AI provides equal economic gains to fossil fuels and renewables, global CO2 emissions could rise by 0.47 billion to 1.8 billion tons a year—roughly Mexico&\#x27;s annual emissions, according to co-author Holly Alpine.

**Tags**: `#AI`, `#fossil fuels`, `#carbon emissions`, `#data centers`, `#energy policy`

---

<a id="item-finance-news-11"></a>
### [AMD Raises $4.75 Billion in Bond Sale](https://finance.yahoo.com/markets/stocks/articles/amd-just-borrowed-4-75-023900183.html) ⭐️ 7.0/10

AMD borrowed $4.75 billion in a bond sale, more than triple the size of its last bond issuance.

openbb · NVDA · Aug 16, 02:39

**「Background」** AMD&\#x27;s $4.75 billion bond sale is its largest ever, more than triple its previous offering. The senior notes were sold in four tranches maturing between 2029 and 2036.

**「Impact」** The $4.75 billion senior-note sale signals AMD’s large cash needs, likely tied to the AI buildout, and adds fixed interest obligations to bond investors whose claims run through 2036.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/amd-plans-to-raise-as-much-as-5-billion-from-debt-offering">AMD Raises $4.75 Billion From Bond Sale as AI Demand Surges - Bloomberg</a></li>
<li><a href="https://www.fool.com/investing/2026/08/15/amd-just-borrowed-475-billion-more-than-triple-its/">AMD Just Borrowed $4.75 Billion, More Than Triple Its Last Bond Sale | The Motley Fool</a></li>
<li><a href="https://www.briefs.co/news/chipmaker-s-largest-debt-deal-yet-4-75-billion-for-ai-growth/">AMD&#x27;s $4.75 Billion Bond Sale Funds AI Growth - briefs.co</a></li>
<li><a href="https://www.fool.com/investing/2026/08/15/amd-just-borrowed-475-billion-more-than-triple-its/">AMD Just Borrowed $4.75 Billion, More Than Triple Its Last Bond Sale</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#Debt Financing`, `#Semiconductor Industry`, `#Capital Markets`, `#Bond Sale`

---

<a id="item-finance-news-12"></a>
### [Gold Reaches $4,400 and Mining Stocks Rally](https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html) ⭐️ 7.0/10

Gold hit $4,400 an ounce, and mining stocks are starting to catch up with the rally, according to the article.

openbb · GLD · Aug 16, 14:21

**「Background」** Gold had been rallying for months, breaking past $4,000 an ounce in October 2025, but mining stocks had trailed bullion until the gap began narrowing in July.

**「Impact」** The record gold price above $4,400 an ounce has begun lifting mining stocks after they lagged bullion for years, and the narrowing gap can boost revenues and margins for gold miners and their investors.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html">Gold Just Hit $4,400 and the Miners Are Finally Catching Up</a></li>
<li><a href="https://www.cnbc.com/2025/10/08/gold-zooms-past-4000-for-first-time-in-historic-flight-to-safety.html">Gold shatters $4,000 milestone, silver belts record high as ... - CNBC</a></li>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/gold-just-hit-4-400-142144156.html?fr=sycsrp_catchall">Gold Just Hit $4,400 and the Miners Are Finally Catching Up</a></li>
<li><a href="https://thescjournal.com/business/gold-prices-surge-to-record-highs-surpassing-4400-an-ounce/">Gold Prices Surge to Record Highs, Surpassing $4,400 an Ounce</a></li>

</ul>
</details>

**Tags**: `#gold`, `#commodity prices`, `#mining stocks`, `#precious metals`, `#market milestone`

---

<a id="item-finance-news-13"></a>
### [Kraft, McDonald’s and Whirlpool CEOs warn US consumers are ‘running out of money’](https://finance.yahoo.com/economy/articles/running-money-kraft-mcdonald-whirlpool-114500035.html) ⭐️ 7.0/10

The chief executives of Kraft Heinz, McDonald’s and Whirlpool have warned during recent earnings commentary that US consumers are running out of money, signaling possible weakness in consumer spending.

openbb · PG · Aug 16, 11:45

**「Background」** The warnings came in recent earnings commentary: Kraft Heinz CEO Steve Cahillane pointed to financial strain among lower-income consumers, and executives at McDonald’s and Whirlpool similarly described shoppers saving less and using credit cards for everyday purchases like gas.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/articles/running-money-kraft-mcdonald-whirlpool-114500035.html">‘ Running out of money ’: Kraft , McDonald ’ s , Whirlpool CEOs all flag...</a></li>
<li><a href="https://www.linkedin.com/posts/matthewsboyle_americans-are-running-out-of-money-the-ceos-activity-7458252875631276033-VFx8">CEOs Warn Americans Are Running Out of Money | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#Consumer Spending`, `#Economic Slowdown`, `#Corporate Earnings`, `#Retail`, `#US Economy`

---