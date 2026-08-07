---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 187 items, 26 important content pieces were selected

---

**Technology News**
1. [DeepSeek V4 Flash 0731 Delivers Fast, Cheap Inference](#item-tech-news-1) ⭐️ 8.0/10
2. [New Rust Query Engine Makes Postgres Hundreds of Times Faster for Analytics](#item-tech-news-2) ⭐️ 8.0/10
3. [Cloudflare&\#x27;s Kitesurf brings agent-first browsing to V8 isolates and Blitz](#item-tech-news-3) ⭐️ 8.0/10
4. [2027 Memory Capacity Reportedly Sold Out Amid AI HBM Demand](#item-tech-news-4) ⭐️ 8.0/10
5. [A year of fighting scrapers on a 1.5 million-page website](#item-tech-news-5) ⭐️ 8.0/10
6. [Starlink 10GW by 2027: The $300B ARR and Microsoft Inference Case](#item-tech-news-6) ⭐️ 8.0/10
7. [OpenAI Says Astra May Reach Critical Cyber Capability, Expanding Safety Tests](#item-tech-news-7) ⭐️ 8.0/10
8. [Oracle Bans AI-Generated Code from OpenJDK Under Interim Policy](#item-tech-news-8) ⭐️ 7.0/10
9. [New Mexico court orders Meta to pay $567m for children&\#x27;s mental health harms](#item-tech-news-9) ⭐️ 7.0/10
10. [Codex with GPT-5.6 Sol Ultra Outshines Claude Fable 5 on Raccoon Heist](#item-tech-news-10) ⭐️ 7.0/10
11. [Accenture&\#x27;s AI Token Costs Surge on Non-Engineers and PDF Conversions](#item-tech-news-11) ⭐️ 7.0/10
12. [US Probes Chinese AI Firms&\#x27; Offshore Access to Nvidia Chips](#item-tech-news-12) ⭐️ 7.0/10
13. [SK Hynix confirms 375-layer V10 NAND with wafer bonding](#item-tech-news-13) ⭐️ 7.0/10
14. [sub2api OAuth Flaw Allows Account Takeover with Just Email](#item-tech-news-14) ⭐️ 7.0/10
15. [AWS Cracks Down on Internal CPU Waste Amid Agentic AI Demand](#item-tech-news-15) ⭐️ 7.0/10

**Financial News**
1. [CBP Pays $100 Billion in IEEPA Tariff Refunds](#item-finance-news-1) ⭐️ 9.0/10
2. [Weak July jobs report lowers odds of September Fed rate hike](#item-finance-news-2) ⭐️ 8.0/10
3. [SEC Approves Nasdaq’s 23-Hour Trading; Launch Set for Dec 6, 2026](#item-finance-news-3) ⭐️ 8.0/10
4. [Chevrolet Ends New-Car Sales in China, SAIC-GM Confirms](#item-finance-news-4) ⭐️ 8.0/10
5. [Beijing Cuts Social Security Requirement for Non-Beijing Homebuyers to 1 Year](#item-finance-news-5) ⭐️ 8.0/10
6. [Johnson &amp; Johnson Reaches $5.5 Billion Talc Settlement](#item-finance-news-6) ⭐️ 8.0/10
7. [Premarket movers: Atlassian surges on earnings beat, Trade Desk slides](#item-finance-news-7) ⭐️ 7.0/10
8. [Australia proposes A$31.30 minimum pay for delivery riders](#item-finance-news-8) ⭐️ 7.0/10
9. [Molson Coors Beats Q2 Earnings Estimates on Pricing and Cost Savings](#item-finance-news-9) ⭐️ 7.0/10
10. [Diageo FY26 Preliminary Earnings Show North America Pressure](#item-finance-news-10) ⭐️ 7.0/10
11. [Constellation Signs 920 MW of New Power Deals, Including Walmart PPA](#item-finance-news-11) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek V4 Flash 0731 Delivers Fast, Cheap Inference](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek V4 Flash 0731 is an updated release of DeepSeek&\#x27;s Flash model family, dated July 31, and is being tracked on the ARC Prize results page. Community users report that it is good enough for almost any task and so cheap that costs become irrelevant: one user running it on the Oh My Pi agent with 5–6 active sessions \(about 12 streams\) struggled to spend more than $5 per day, and another noted that OpenCode Go temporarily offers double limits, so $10 effectively buys $140 of tokens. The update is described as a clear step up from the earlier preview version, with particularly strong performance on debugging and document/data analysis. On 2x RTX Pro 6000 Blackwell hardware, users measured roughly 8,000 tokens/s prefill and about 250 tokens/s per stream, with peaks near 1,000 tokens/s. However, not all feedback is positive: some users report regressions in agentic behavior, such as infinite loops and tool-call failures that waste tokens.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**「Background」** DeepSeek V4 Flash 0731 is the generally available release of DeepSeek&\#x27;s efficiency-tier Flash model, announced on July 31, 2026, with a 1M token context window and a GPQA score of 88.1. According to DeepSeek&\#x27;s model card, it outperforms DeepSeek V4-Pro \(Preview\) on listed benchmarks despite having a far smaller activated parameter count, and is broadly competitive with the strongest proprietary models. The ARC Prize is an abstract reasoning benchmark \(ARC-AGI\), and this result page reports how the model performs on those reasoning tasks.

**「Impact」** For AI practitioners and developers using DeepSeek&\#x27;s Flash line, the 0731 release offers substantially lower cost and higher throughput for everyday agentic and analytical workloads, though users should watch for token-wasting loop behavior in tool-calling scenarios.

**「Community Discussion」** Commenters largely praise the updated model&\#x27;s speed and cost-efficiency, with one describing it as a whole tier up from the earlier preview, but another reports recurring infinite loops and self-talk without tool execution compared with the previous Flash version.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek -ai/ DeepSeek - V 4 - Flash - 0731 · Hugging Face</a></li>
<li><a href="https://hokai.io/hub/models/deepseek-v4-flash-0731">DeepSeek - V 4 - Flash - 0731 : 1M Context &amp; GPQA 88.1 (2026) | HokAI</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#large-language-models`, `#arc-agi`, `#model-release`, `#ai-inference`

---

<a id="item-tech-news-2"></a>
### [New Rust Query Engine Makes Postgres Hundreds of Times Faster for Analytics](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

A new Postgres query engine called pgrust claims to make analytics hundreds of times faster using batching, operator fusion, and SIMD. The project, written in Rust, emphasizes correctness through formal verification and differential fuzz testing, with the author stating that over 1,000 user-facing functions have been proven to have identical logic to Postgres. The approach includes adaptive planning, a feature some developers have long wanted from the Postgres core team. While performance gains are significant, the project faces practical adoption challenges because it is not built by the trusted Postgres core team.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**「Background」** Traditional PostgreSQL evaluates queries row-by-row using a volcano-style iterator model, which adds overhead and limits cache and CPU efficiency, especially for analytical workloads. pgrust is a project that rewrites PostgreSQL in Rust and, in its version 0.2 release, replaced the query engine&\#x27;s execution model with batching \(processing many rows together\), operator fusion \(combining steps to reduce per-row overhead\), and SIMD instructions to boost analytical performance. The project also uses differential fuzz testing and formal verification to check that the rewritten functions match PostgreSQL&\#x27;s behavior.

**「Impact」** For Postgres users running analytical workloads, pgrust could deliver order-of-magnitude query speedups, but its real-world impact depends on trust, ongoing maintenance, and whether it can be adopted without replacing core Postgres infrastructure.

**「Community Discussion」** In the comments, the author highlighted correctness work and invited questions, while commenters expressed skepticism about replacing Postgres due to trust and continuity concerns, welcomed the adaptive planning feature, and asked about I/O scheduling and thread scheduling architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching, operator fusion, and SIMD - malisper.me</a></li>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now faster than Postgres and Clickhouse · GitHub</a></li>

</ul>
</details>

**Tags**: `#postgres`, `#query-engine`, `#SIMD`, `#analytics`, `#rust`

---

<a id="item-tech-news-3"></a>
### [Cloudflare&\#x27;s Kitesurf brings agent-first browsing to V8 isolates and Blitz](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare announced Kitesurf, an agent-first browser that runs in V8 isolates and is built on the open-source Blitz engine, targeting edge-based browser automation and AI agents. The design centers on V8-isolate execution and edge infrastructure to give agents a lightweight, scriptable browser environment. Nicoburns, Blitz&\#x27;s author, said he was not involved in building Kitesurf but is informed that the team intends to open source and upstream its patches to Blitz. The announcement matters because browser-based agents increasingly need low-latency, distributed execution, and edge-native isolation is a plausible fit. No availability dates, performance data, or compatibility constraints were provided.

hackernews · m3h · Aug 7, 10:42 · [Discussion](https://news.ycombinator.com/item?id=49208393)

**「Background」** Kitesurf is a new Cloudflare browser that runs in V8 isolates on Cloudflare Workers, built on top of Blitz, an open-source modular browser engine developed by Dioxus Labs over the past 2.5 years. Kitesurf splits the browser into isolated Workers components, with the Engine as the only public-facing piece that speaks Chrome DevTools Protocol \(CDP\) over WebSocket plus HTTP REST and stores each session&\#x27;s state. Cloudflare describes the browser as stateless, highly scalable, and cost-effective for AI agents and edge-based automation, and the team reportedly plans to open-source and upstream its patches back to Blitz.

**「Community Discussion」** Several commenters questioned Cloudflare&\#x27;s dual role as both an anti-bot/CDN provider and an agent/browser automation platform, asking whether Kitesurf instances would bypass Cloudflare&\#x27;s own anti-bot protections or be blocked like other scrapers. Others asked for concrete examples of browser agents in practice, while Blitz author nicoburns clarified that Kitesurf builds on Blitz and that upstreaming of Cloudflare&\#x27;s patches is intended.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf/">Introducing Kitesurf: The agent-first browser that runs in V8 isolates on Cloudflare Workers | Cloudflare Blog</a></li>
<li><a href="https://www.reddit.com/r/rust/comments/1vhetlq/introducing_kitesurf_cloudflares_new_headless_web/">r/rust on Reddit: Introducing Kitesurf: Cloudflare&#x27;s new headless web browser that runs in V8 Isolates, powered by Dioxus Blitz</a></li>

</ul>
</details>

**Tags**: `#browser automation`, `#AI agents`, `#Cloudflare`, `#V8 isolates`, `#edge computing`

---

<a id="item-tech-news-4"></a>
### [2027 Memory Capacity Reportedly Sold Out Amid AI HBM Demand](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

Industry reports indicate that memory capacity for 2027 is already sold out, extending a supply crunch driven overwhelmingly by AI demand for high-bandwidth memory \(HBM\). The shortage is not simply a matter of total production limits: producing HBM3E consumes roughly three times the wafer supply as DDR5 to yield the same number of bits on the same technology node, so ramping HBM directly constrains supply growth for non-HBM memory products. This sustained demand pressure has implications for memory pricing and availability well beyond the AI data center market, affecting consumer desktop memory and embedded systems alike. The report underscores the structural tradeoff between HBM and conventional DRAM capacity, with no immediate relief indicated for the 2027 allocation cycle.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**「Memory supply context」** High-bandwidth memory \(HBM\) is a specialized, stacked DRAM package used in AI accelerators, while conventional DRAM such as DDR5 serves servers and PCs. Reports indicate that the three major memory makers—Samsung, SK hynix, and Micron—have sold out their combined DRAM and HBM capacity for 2027, driven by AI data centers buying HBM for accelerators and conventional DRAM for host servers. Because HBM production consumes roughly three times the wafer area of DDR5 for the same bit count, this AI-driven demand is also constraining supply of non-HBM memory.

**「Impact」** PC builders and consumers buying DDR4 or DDR5 memory will likely continue to face elevated prices and tighter availability because wafer capacity diverted to HBM reduces output of conventional memory. The effect also extends to embedded developers, who may see cost or supply pressure when their designs depend on DRAM capacity in the same strained market.

**「Community Discussion」** Commenters highlighted the concrete wafer-capacity tradeoff between HBM and DDR5, noting HBM&\#x27;s roughly three-to-one penalty in wafer consumption per bit. Several users shared practical signs of the shortage, including paying $120 for 16 GB of DDR4, a cancelled order that likely preceded a price increase, and an embedded developer feeling pressure to stockpile even relatively modest microcontroller RAM. Another user cited the memory and storage strain as a reason to limit reliance on AI tools.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tweaktown.com/news/113004/memory-capacity-for-all-of-2027-has-reportedly-been-booked-and-sold-with-no-more-dram-or-hbm-available/index.html">Memory capacity for all of 2027 has reportedly been booked and sold ...</a></li>
<li><a href="https://www.remio.ai/post/samsung-sk-hynix-and-micron-reportedly-sell-out-2027-memory-supply">Samsung, SK Hynix, and Micron Reportedly Sell Out 2027 Memory ...</a></li>
<li><a href="https://spilled.gg/memory-makers-production-capacity/">Memory makers have reportedly sold out their entire 2027 production...</a></li>

</ul>
</details>

**Tags**: `#memory`, `#HBM`, `#AI infrastructure`, `#hardware`, `#supply chain`

---

<a id="item-tech-news-5"></a>
### [A year of fighting scrapers on a 1.5 million-page website](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A website operator shared a year-long experience fighting scrapers on a 1.5 million-page website, highlighting the enormous scale of bot traffic and the trade-offs of mitigation strategies. The account underscores how AI/LLM crawlers and automated scrapers impose real operational costs and force hard choices between openness and protection. The analysis sees this as a timely, high-value technical issue with practical implications for site operators.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**「Background」** The PatronView project is a 1.5 million-page website hosted on Cloudflare&\#x27;s edge platform, where the operator reports that over 99% of traffic comes from bots and scrapers. According to the article, this scale of bot traffic would be an existential problem on a traditional VPS, but on an edge platform it is merely a nuisance because the scrapers&\#x27; costs have fallen faster than defenses improved. This context frames the operator&\#x27;s year-long mitigation effort and the community debate about relying on centralized services like Cloudflare to decide who can access a website.

**「Impact」** For site operators behind Cloudflare, the scraper fight now has a formal economic lever: Cloudflare&\#x27;s pay-per-crawl marketplace \(launched July 2025\) lets content owners charge AI crawlers and returns HTTP 402 when payment isn&\#x27;t configured, positioning Cloudflare as the gatekeeper for AI access to the open web. Meanwhile, operators not relying on Cloudflare are turning to proof-of-work challenges like Anubis to filter bots, and cost spikes from services such as Cloudflare D1 can push smaller sites toward static architectures.

**「Community discussion」** Commenters expressed concern about ceding website-access decisions to centralized providers like Cloudflare, with some recommending self-hosted proof-of-work solutions such as Anubis. Others shared concrete cost impacts, including a 500% monthly bill spike and an example of Claude-searchbot fetching roughly 205,000 pages in 72 hours while sending only one referral, and the author&\#x27;s irony about scraping public documents.

<details><summary>References</summary>
<ul>
<li><a href="https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/">99% of My Website Traffic Is Bots | PatronView</a></li>
<li><a href="https://blog.cloudflare.com/introducing-pay-per-crawl/">Introducing pay per crawl: Enabling content owners to charge AI crawlers for access | Cloudflare Blog</a></li>
<li><a href="https://www.remio.ai/post/cloudflare-reveals-the-true-cost-of-ai-scrapers-on-the-open-web">Cloudflare Reveals the True Cost of AI Scrapers on the Open Web</a></li>
<li><a href="https://techcrunch.com/2025/07/01/cloudflare-launches-a-marketplace-that-lets-websites-charge-ai-bots-for-scraping/">Cloudflare launches a marketplace that lets websites charge AI bots for scraping | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#scraping`, `#bots`, `#web operations`, `#Cloudflare`, `#AI crawlers`

---

<a id="item-tech-news-6"></a>
### [Starlink 10GW by 2027: The $300B ARR and Microsoft Inference Case](https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real) ⭐️ 8.0/10

An analysis in SemiAnalysis by Jeremie Eliahou Ontiveros argues that SpaceX’s Starlink constellation can reach 10 GW of capacity by 2027, generating roughly $300 billion in annual recurring revenue \(ARR\) and making Microsoft the largest offtaker of space-based AI inference. The argument rests on an inference efficiency assumption of $100B per GW per year, SpaceX’s past launch and deployment pace, and Microsoft’s projected 10 GW datacenter demand awakening by 2026, with Azure able to grow at triple-digit rates. The piece treats these projections as forward-looking scenarios rather than confirmed plans, and their realization depends on continued Starlink launches, power, and enterprise demand. For technology strategists, the core claim is that satellite-based compute could become a meaningful complement to terrestrial cloud for AI inference workloads.

rss · Semianalysis · Aug 7, 20:08

**「Starlink, AI compute, and Microsoft」** Starlink is SpaceX&\#x27;s low Earth orbit satellite internet constellation, and the company plans a roughly 100-fold expansion of its capacity alongside a rapid AI infrastructure buildout, expecting significant NVIDIA GPU allocations in 2027. According to reporting, about 10% of that compute may go to training Grok models, with the rest used for inference services or rented to external customers. SpaceX already has a partnership with Microsoft to bring Starlink connectivity to Azure customers, which is why the article projects Microsoft as the largest offtaker of SpaceX&\#x27;s future inference capacity.

**「Impact」** If SpaceX&\#x27;s projection holds, Starlink could reach 10 GW of capacity by 2027 and generate roughly $300 billion in annual recurring revenue, with Microsoft Azure as the largest offtaker for space-based AI inference. That would give Microsoft a potentially triple-digit growth engine for Azure and reshape cloud inference economics, though the numbers depend on SpaceX maintaining its current deployment pace and on inference demand materializing at the assumed 100B/GW/year efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real">SpaceX 10GW in 2027 – Why It’s Real, Will Drive $500B ARR for SpaceX, and Why Microsoft Will Be the Largest Offtaker</a></li>
<li><a href="https://convergedigest.com/spacex-starlink-v3-ai-infrastructure-expansion/">SpaceX Maps 100-Fold Starlink Capacity Expansion and Rapid AI Infrastructure Buildout - Converge Digest</a></li>
<li><a href="https://www.juniorstocks.com/spacex-announces-strong-partnership-microsoft">Juniorstocks | SpaceX announces strong partnership with Microsoft</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starlink`, `#AI inference`, `#Microsoft Azure`, `#satellite internet`

---

<a id="item-tech-news-7"></a>
### [OpenAI Says Astra May Reach Critical Cyber Capability, Expanding Safety Tests](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 8.0/10

On August 7, 2026, OpenAI disclosed that its upcoming Astra model showed significant progress in agentic coding and cybersecurity during internal evaluations, with initial results strong enough that OpenAI cannot rule out the model reaching the &\#x27;critical&\#x27; cyber capability threshold. Previous models such as GPT-5.6-Sol had only been rated &\#x27;high&\#x27; on the same evaluation. Under OpenAI&\#x27;s preparedness framework, reaching the critical threshold means the model could autonomously discover and exploit zero-day vulnerabilities in hardened real systems without human intervention, or plan and execute end-to-end novel cyberattacks from high-level objectives. In response, OpenAI has paused Astra-related internal activities that do not meet enhanced security requirements, implemented isolated test environments, stronger encryption, and universal monitoring, and plans to work with government agencies and AI safety organizations on third-party testing. The expanded safety testing may delay Astra&\#x27;s release.

telegram · zaihuapd · Aug 7, 16:44

**「Background」** OpenAI&\#x27;s Preparedness Framework categorizes frontier models by escalating risk levels, with &\#x27;high&\#x27; indicating significant cyber capabilities and &\#x27;critical&\#x27; reserved for models that can autonomously compromise hardened systems or devise novel, end-to-end cyber attacks from high-level goals. The same internal evaluation previously rated GPT-5.6-Sol as &\#x27;high,&\#x27; which provides context for why Astra&\#x27;s preliminary results are notable enough to trigger stricter safety protocols.

**「Impact」** For users and developers awaiting Astra, the expanded safety testing may delay its release and signals that OpenAI is applying more stringent security controls to its most capable agentic coding models, with third-party oversight from government agencies and AI safety organizations.

**Tags**: `#AI safety`, `#OpenAI`, `#cybersecurity`, `#large language models`, `#preparedness framework`

---

<a id="item-tech-news-8"></a>
### [Oracle Bans AI-Generated Code from OpenJDK Under Interim Policy](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 7.0/10

Oracle has adopted an interim policy banning AI-generated code from OpenJDK contributions, a governance move that affects one of the most widely used open-source platforms. The policy, outlined in an OpenJDK legal page titled &quot;Interim Policy on Generative AI,&quot; appears designed to address legal and provenance concerns, especially given Oracle&\#x27;s history of copyright litigation around Java. Oracle&\#x27;s lawyers are reportedly drafting the final version, and the interim measure is framed around protecting the already limited time of human reviewers from low-quality AI-generated contributions. The decision is notable because Oracle has publicly promoted AI heavily, making the ban appear inconsistent with its broader AI messaging. The policy is likely to shape how other large open-source projects handle AI-assisted contributions.

hackernews · delduca · Aug 7, 17:36 · [Discussion](https://news.ycombinator.com/item?id=49213754)

**「Background」** OpenJDK is the open-source reference implementation of the Java platform, stewarded by Oracle, which also owns Java trademarks. OpenJDK has published an &\#x27;Interim Policy on Generative AI&\#x27; that permits contributors to use AI tools privately for comprehension, debugging, and research, but forbids submitting AI-generated content, with a final version still being drafted by their lawyers. The policy arrives amid Oracle CEO Larry Ellison&\#x27;s public statements that AI now writes most of Oracle&\#x27;s own code, highlighting the tension between corporate AI adoption and open-source governance.

**「Impact」** OpenJDK contributors must immediately refrain from submitting AI-generated code under the interim policy, potentially slowing AI-assisted development workflows while Oracle&\#x27;s legal team finalizes the rules. The final policy could set precedent for how major open-source projects governed by large corporations treat AI-generated contributions.

**「Community Discussion」** Commenters largely understand the legal and review-burden rationale, but many are skeptical of Oracle&\#x27;s motives, with one suggesting the company wants to preserve its ability to sue over AI-washing while another doubts the final proposal will improve. Some also point out the irony of Oracle banning AI code while allegedly using AI for its own release notes, and others note the linked article is a poor summary of a better Register piece and the original OpenJDK policy page.

<details><summary>References</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://www.tiktok.com/discover/oracle-ai-explained">Oracle Ai Explained | TikTok</a></li>

</ul>
</details>

**Tags**: `#OpenJDK`, `#Oracle`, `#AI-generated code`, `#open-source policy`, `#software licensing`

---

<a id="item-tech-news-9"></a>
### [New Mexico court orders Meta to pay $567m for children&\#x27;s mental health harms](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 7.0/10

A New Mexico court ordered Meta to pay $567 million for harms to children&\#x27;s mental health, marking a significant legal ruling against the social media company. The judgment, which also requires Meta to make changes for underage users, stems from a lawsuit alleging that the company&\#x27;s platforms contributed to a public nuisance harming minors. The decision adds to mounting legal and regulatory pressure on social media companies over youth mental health, though the penalty is small relative to Meta&\#x27;s global revenue.

hackernews · boplicity · Aug 7, 00:06 · [Discussion](https://news.ycombinator.com/item?id=49204352)

**「Background」** Meta, the parent company of Facebook and Instagram, was found liable under New Mexico&\#x27;s public-nuisance law for contributing to adverse mental health impacts on young users. A New Mexico court ordered Meta to pay $567 million into a fund aimed at redressing those harms. The ruling reflects ongoing legal and regulatory pressure on social media platforms over their effects on children.

**「Impact」** The ruling requires Meta to pay $567 million into a New Mexico fund and change how its platforms function for young users in the state, adding direct compliance costs and operational constraints while strengthening momentum for similar state-level action against social media companies.

**「Community Discussion」** Commenters noted that while the $567 million figure is small compared to Meta&\#x27;s global revenue, it is enormous for a jurisdiction with only about 2 million people, and some cited a reported $942 million figure. Others pointed to the specific New Mexico public-nuisance law violated, and several compared Instagram Reels and TikTok to addictive substances, expressing concerns about algorithmic design&\#x27;s impact on younger users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta">New Mexico court orders Meta to pay $ 567 m over... | The Guardian</a></li>
<li><a href="https://english.news.cn/20260807/a5e12666e9b444df8c546248735d0934/c.html">Meta ordered to pay 567 mln USD to address children &#x27;s mental health</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta">New Mexico court orders Meta to pay $567m over... | The Guardian</a></li>
<li><a href="https://www.aljazeera.com/news/2026/8/7/new-mexico-court-orders-meta-to-pay-567m-over-harm-to-youths">New Mexico court orders Meta to pay $567m over harm to... | Al Jazeera</a></li>

</ul>
</details>

**Tags**: `#legal`, `#regulation`, `#Meta`, `#social media`, `#technology policy`

---

<a id="item-tech-news-10"></a>
### [Codex with GPT-5.6 Sol Ultra Outshines Claude Fable 5 on Raccoon Heist](https://simonwillison.net/2026/Aug/7/moonlight-mayhem/#atom-everything) ⭐️ 7.0/10

Simon Willison ran the exact same Raccoon Heist game prompt through Codex Desktop with GPT-5.6 Sol Ultra, the mode that aggressively uses sub-agents, and compared the result with his earlier Claude Fable 5 version. Codex produced a much better game, &quot;Moonlight &amp; Mayhem,&quot; placing the player in a museum where you rescue two raccoon crewmates and stack them to bust a golden sardine out of its case, complete with textures and prompts generated using gpt-image-2. The one-shot version had a visual bug where every raccoon had an enormous black sphere eyeball floating over its head, which Codex failed to spot despite reviewing screenshots; Willison fixed it by prompting &quot;Why do the raccoons have huge black spheres on them?&quot; followed by &quot;Fix it&quot;. Codex spent 52 minutes on the project, and the session would have cost $23.28 at full API prices according to AgentsView, with 700.7K input tokens, 32.5M cached tokens, and 148K output tokens. The full transcript and source code are available in Willison&\#x27;s GitHub repository.

rss · Simon Willison · Aug 7, 19:18

**「Background」** Simon Willison previously had Claude Fable 5 build a working Raccoon Heist game from a premise he generated four years ago with GPT-3 and DALL-E, resulting in a single raccoon collecting coins and fish in a back yard. Codex is OpenAI&\#x27;s coding agent, and GPT-5.6 Sol Ultra is a model mode that makes aggressive use of sub-agents, which can plan and execute more complex tasks. This comparison is a practical test of whether the newer model and agent setup can handle the same natural-language game specification more ambitiously.

**「Impact」** Developers evaluating AI coding agents can expect Codex with GPT-5.6 Sol Ultra to produce more ambitious interactive game output than Claude Fable 5 on the same one-shot prompt, but they should still plan to review and correct visual bugs that the agent may miss even during screenshot review.

**Tags**: `#AI coding agents`, `#Codex`, `#GPT-5.6`, `#game generation`, `#Simon Willison`

---

<a id="item-tech-news-11"></a>
### [Accenture&\#x27;s AI Token Costs Surge on Non-Engineers and PDF Conversions](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 7.0/10

Simon Willison highlighted a 404 Media article from June 24th reporting that Accenture is seeing surprisingly high AI token consumption driven largely by non-engineers rather than engineers. In leaked meeting audio, Justice Kwak, Accenture&\#x27;s agentic AI strategy lead, confirmed that converting PDFs into images and then into markdown files is one of the biggest token chewers. Stuart Henderson, Accenture&\#x27;s client group lead, joked about the PDF-to-markdown practice, and Kwak said the data backs it up. The anecdote underscores how document-processing workflows, especially those involving PDFs, can significantly drive up enterprise AI costs. Willison adds that PDFs being a terrible medium for communicating information should prompt business-wide reconsideration.

rss · Simon Willison · Aug 7, 16:18

**「Background」** In AI systems, &quot;tokens&quot; are the individual units of text that large language models process, and providers charge by the token, so token consumption directly drives cost. Enterprises increasingly use LLMs to convert documents such as PDFs into markdown for easier processing, but PDFs are image-heavy and verbose when parsed, making them a large token consumer. A reportedly leaked internal Accenture meeting revealed that non-engineers were driving a surge in token spend, with PDF-to-markdown conversion singled out as a major contributor.

**「Impact」** For Accenture, the leaked comments reveal that internal AI spending is being propelled by non-engineer workflows and costly PDF-to-markdown conversions, meaning cost-control efforts may need to target these user behaviors and document formats.

<details><summary>References</summary>
<ul>
<li><a href="https://www.404media.co/the-tokenpocalypse-is-here-companies-are-scrambling-to-stop-spending-so-much-on-ai/">The Tokenpocalypse Is Here : Companies Are Scrambling To Stop ...</a></li>

</ul>
</details>

**Tags**: `#AI costs`, `#token consumption`, `#enterprise AI`, `#PDF processing`, `#AI economics`

---

<a id="item-tech-news-12"></a>
### [US Probes Chinese AI Firms&\#x27; Offshore Access to Nvidia Chips](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 7.0/10

The US Commerce Department&\#x27;s Bureau of Industry and Security \(BIS\) has launched a systematic review of how Chinese AI companies obtain and use Nvidia chips overseas, including remote access through cloud computing in other countries and smuggling networks. Investigators are compiling two country lists: one for black markets suspected of smuggling restricted chips into China, and another for nations where Chinese firms remotely rent chips. The review was triggered by Moonshot AI&\#x27;s Kimi K3 model released last month, whose performance approached US rivals; a White House official publicly accused the company of illegally obtaining Nvidia chips and accessing them remotely via Thailand, with BIS enforcement starting days later. Legal authority remains uncertain because remote access itself is not illegal, and although the House has passed a bipartisan bill to clarify such power, it faces expected opposition from Nvidia and other tech firms. The report also says Alibaba controlled a Singapore shell company via a Cayman entity to use Nvidia chips in Malaysia through Megaspeed, which is currently under US investigation.

telegram · zaihuapd · Aug 7, 11:18

**「Background」** The US Commerce Department&\#x27;s Bureau of Industry and Security \(BIS\) enforces export controls that have, for the past three years, blocked direct sales of Nvidia&\#x27;s top-end chips such as H100 and A100 to Chinese buyers. In July 2026, Chinese startup Moonshot AI released Kimi K3, a 2.8-trillion-parameter model with a 1-million-token context window, whose performance and pricing pressured Western labs. Because Chinese firms cannot legally buy the most advanced Nvidia chips directly, they reportedly rely on overseas cloud computing and intermediary companies to gain access, which is what BIS is now scrutinizing.

**「Impact」** If BIS gains explicit authority over remote access to controlled computing \(as proposed by the Remote Access Security Act\) or reinterprets existing rules to cover it, Chinese AI firms that depend on offshore Nvidia compute—such as the Alibaba-linked Singapore shell using Megaspeed in Malaysia—could face new enforcement actions and disruption of cloud-based AI training. Today, however, BIS’s authority over remote cloud access remains legally uncertain and has not historically been exercised, leaving current offshore access in a gray area.

<details><summary>References</summary>
<ul>
<li><a href="https://carussignal.com/kimi-k3-2-8-trillion-parameters-compute-wall/">Kimi K 3 in Three Numbers: 2.8 Trillion Parameters, $15 Tokens, and...</a></li>
<li><a href="https://temperature2.com/p/2026-07-31-moonshot-kimi-alibaba-nvidia-chips/">Moonshot&#x27;s Kimi K 3 runs on 20,000 Alibaba Nvidia chips</a></li>
<li><a href="https://www.linkedin.com/pulse/kimi-k3-how-one-chinese-model-triggered-two-american-reflexes-ibcgf">Kimi K 3 : How One Chinese Model Triggered Two American Reflexes</a></li>
<li><a href="https://carnegieendowment.org/research/2026/05/the-geopolitical-debates-over-controlling-cloud-compute">The Geopolitical Debates Over Controlling Cloud Compute</a></li>
<li><a href="https://www.iaps.ai/research/remote-access-security-act">Remote Access Security Act (RASA) — Institute for AI Policy and...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#semiconductors`, `#export-controls`, `#Nvidia`, `#China`

---

<a id="item-tech-news-13"></a>
### [SK Hynix confirms 375-layer V10 NAND with wafer bonding](https://www.gelonghui.com/live/2599953) ⭐️ 7.0/10

SK Hynix has confirmed that its next-generation V10 NAND flash will use a 375-layer stacked design, succeeding its 321-layer V9 &quot;4D NAND&quot; and marking the company&\#x27;s first NAND product to adopt wafer bonding. The company announced the details in its FMS 2026 summit press release. SK Hynix claims V10 delivers 2.5 times the performance per watt of the previous generation and is optimized for AI infrastructure environments requiring both efficiency and performance. The announcement does not include production or availability dates.

telegram · zaihuapd · Aug 7, 12:19

**「Background」** NAND flash stores data by stacking memory cells vertically to increase density without expanding the chip footprint. SK Hynix&\#x27;s current V9 generation is a 321-layer &quot;4D NAND&quot; product. Wafer bonding joins two processed wafers instead of building all layers sequentially, and SK Hynix is using this technique for the first time in V10, potentially enabling higher layer counts and better manufacturability.

**「Impact」** For AI infrastructure operators and memory buyers, the confirmed 375-layer V10 points to a major power-efficiency uplift in high-capacity NAND, though the source does not state when the product will ship or at what cost.

**Tags**: `#NAND`, `#SK Hynix`, `#semiconductors`, `#AI infrastructure`, `#memory`

---

<a id="item-tech-news-14"></a>
### [sub2api OAuth Flaw Allows Account Takeover with Just Email](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 7.0/10

A critical OAuth account-takeover vulnerability \(CVSS 8.8\) affects sub2api v0.1.171 and earlier. An attacker who knows only the victim&\#x27;s registered email can bind their own OAuth identity to the victim&\#x27;s account through the pending-session flow&\#x27;s existingUser branch, which fails to verify the password or verification code and requires no user interaction. Once bound, every subsequent OAuth login resolves to the victim&\#x27;s account, giving the attacker full control of API keys, billing balance, and subscription quotas.

telegram · zaihuapd · Aug 7, 14:59

**「Background」** sub2api is an open-source AI API gateway platform that distributes and manages API quotas from AI product subscriptions. Its OAuth sign-in flow uses a pending session mechanism; the vulnerability lies in the existingUser branch of that flow, which failed to verify the user&\#x27;s password or verification code before binding an OAuth identity to an account. This allowed an attacker who knows only the victim&\#x27;s registered email address to complete the binding and take over the account.

**「Impact」** An attacker who knows only the registered email can fully take over an affected sub2api account, controlling API keys, billing balance, and quotas without any user interaction; the report names no patched version.

<details><summary>References</summary>
<ul>
<li><a href="https://github--com.proxy.hfzk.net.cn/Wei-Shaw/sub2api">GitHub - Wei-Shaw/ sub 2 api : Sub 2 API ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#oauth`, `#vulnerability`, `#open-source`, `#account-takeover`

---

<a id="item-tech-news-15"></a>
### [AWS Cracks Down on Internal CPU Waste Amid Agentic AI Demand](https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity) ⭐️ 7.0/10

Amazon AWS is cracking down on internal CPU waste among engineers, asking them since May to reduce EC2 instance usage to preserve customer capacity. As a result, internal engineers now wait days instead of hours for EC2 instances, with one engineer noting they had never waited so long in years of work. The pressure stems from the rise of agentic AI workloads, which involve numerous CPU-based tool calls and complex GPU orchestration, unlike traditional inference tasks. This shift is driving data center GPU-to-CPU ratios from the previous 8:1 or 4:1 down toward 1:1. In response, AMD and Nvidia are both expanding their data center CPU offerings to compete for this growing demand.

telegram · zaihuapd · Aug 7, 16:31

**「Background」** Agentic AI refers to AI systems that autonomously plan and execute multi-step tasks, often involving many tool calls and orchestration steps. Unlike single inference requests, these workflows run heavily on CPU resources to coordinate GPU workloads, shifting data center GPU-to-CPU ratios from around 8:1 or 4:1 toward 1:1. Amazon AWS, which provides compute capacity through EC2 instances to both customers and its own engineers, has begun reclaiming underutilized internal CPU allocations to preserve customer capacity, while AMD and Nvidia have also increased data-center CPU offerings to capture this demand.

**「Impact」** AWS engineers now face multi-day waits for internal EC2 instances, potentially slowing internal development and testing, while the broader shift toward near 1:1 GPU-to-CPU ratios indicates rising demand for CPU-heavy capacity that could influence cloud provisioning strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity">Amazon cracks down on &#x27; CPU waste&#x27; among engineers as agentic AI ...</a></li>
<li><a href="https://artvoice.com/2026/05/26/amd-stock-is-rising-because-of-something-nvidias-ceo-just-said/">AMD Stock Is Rising Because Of Something Nvidia &#x27;s CEO Just Said</a></li>

</ul>
</details>

**Tags**: `#AWS`, `#EC2`, `#Agentic AI`, `#CPU`, `#Cloud Computing`

---

## Financial News

<a id="item-finance-news-1"></a>
### [CBP Pays $100 Billion in IEEPA Tariff Refunds](https://finance.yahoo.com/economy/policy/articles/cbp-paid-100-billion-ieepa-101617141.html) ⭐️ 9.0/10

U.S. Customs and Border Protection has paid out $100 billion in refunds for tariffs collected under the International Emergency Economic Powers Act \(IEEPA\), the law presidents use to impose tariffs during national emergencies. The figure is the total amount refunded to businesses that paid tariffs under this authority.

openbb · PG · Aug 7, 10:16

**「Background」** The refunds follow a Supreme Court ruling that struck down tariffs imposed under the International Emergency Economic Powers Act \(IEEPA\), with duties plus interest being returned to importers.

**「Impact」** The refunds reduce federal revenue by the amount returned and have prompted U.S. consumers to sue companies, alleging they did not pass any of the refund money on to them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chinadaily.com.cn/a/202608/06/WS6a7445a7a310986e2b4695be.html">Trump administration hands back 100 billion USD in tariff refunds</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/8/6/trump-administration-refunds-100bn-in-tariffs-struck-down-by-supreme-court">Trump administration refunds $ 100 bn in tariffs struck... | Al Jazeera</a></li>
<li><a href="https://fortune.com/2026/08/05/what-happened-trump-tariff-refunds-from-companies-consumers-class-action/">U.S. companies got $100 billion in tariff refunds , but... | Fortune</a></li>
<li><a href="https://theamericannews.com/100-billion-tariff-refund-supreme-court-ieepa-2026/">$100 Billion Tariff Refund Supreme Court IEEPA 2026</a></li>

</ul>
</details>

**Tags**: `#tariffs`, `#IEEPA`, `#trade policy`, `#fiscal policy`, `#CBP`

---

<a id="item-finance-news-2"></a>
### [Weak July jobs report lowers odds of September Fed rate hike](https://www.cnbc.com/2026/08/07/odds-the-fed-hikes-in-september-tumble-following-big-july-jobs-miss.html) ⭐️ 8.0/10

A weak July US jobs report, which surprisingly showed job losses, sharply cut market expectations of a September Federal Reserve rate hike. Kalshi odds that the Fed holds rates steady jumped to 65% from about 50-50 before the data, and CME FedWatch put the chance at 60%, up from 45% Thursday.

rss · CNBC Finance · Aug 7, 13:34

**「Background」** The Fed held rates steady at its July meeting, with three members of its policy committee dissenting in favor of a hike amid higher energy prices tied to the U.S.-Iran war. Investors are now focused on July inflation data due Aug. 12; Morgan Stanley&\#x27;s Ellen Zentner said weak payrolls may ease pressure to hike, but hot inflation could still revive calls for hikes.

**Tags**: `#Federal Reserve`, `#interest rates`, `#jobs report`, `#monetary policy`, `#market expectations`

---

<a id="item-finance-news-3"></a>
### [SEC Approves Nasdaq’s 23-Hour Trading; Launch Set for Dec 6, 2026](https://finance.sina.com.cn/stock/bxjj/2026-08-07/doc-inimnkup0012339.shtml) ⭐️ 8.0/10

The SEC approved Nasdaq’s 23/5 trading schedule, which will launch on Dec 6, 2026 and keep U.S. equity trading open 23 hours a day, closing only from 20:00 to 21:00 ET for system processing.

telegram · zaihuapd · Aug 7, 10:03

**「Background」** NYSE Arca already received SEC approval for 22-hour trading, Cboe has proposed nearly 24×5 trading, and all these changes target December 2026; retail investors have also used overnight venues such as Blue Ocean ATS, while the SEC will hold a Sept 17 roundtable on investor protection.

**「Impact」** For investors and brokers, nearly round-the-clock trading means more flexibility, but overnight sessions are expected to have thinner liquidity and wider spreads, so execution costs may be higher.

**Tags**: `#nasdaq`, `#SEC`, `#trading-hours`, `#market-structure`, `#regulation`

---

<a id="item-finance-news-4"></a>
### [Chevrolet Ends New-Car Sales in China, SAIC-GM Confirms](https://m.mydrivers.com/newsview/1142126.html) ⭐️ 8.0/10

SAIC-GM announced that Chevrolet is ending its new-car retail business in China, and after-sales service for its 7.5 million owners will be handled through Buick’s authorized dealer network.

telegram · zaihuapd · Aug 7, 11:12

**「Background」** Chevrolet entered China through the SAIC-GM joint venture 21 years ago and once sold more than 600,000 vehicles in a peak year, but its 2025 sales fell to 52,000 as domestic electric-vehicle makers gained ground.

**Tags**: `#雪佛兰`, `#上汽通用`, `#中国汽车市场`, `#合资品牌`, `#通用汽车`

---

<a id="item-finance-news-5"></a>
### [Beijing Cuts Social Security Requirement for Non-Beijing Homebuyers to 1 Year](https://www.peopleapp.com/column/30052875352-500007640471) ⭐️ 8.0/10

Beijing’s housing authority lowered the social security or individual income tax payment requirement for non-Beijing resident families buying homes within the Fifth Ring Road to one consecutive year before purchase, and raised the maximum first-home housing provident fund loan for couples who both contribute to 2.4 million yuan.

telegram · zaihuapd · Aug 7, 13:57

**「Background」** Previously, non-Beijing households buying a home inside the 5th Ring Road needed 2 consecutive years of social security or individual income tax payments; the new policy lowers this requirement to 1 year.

<details><summary>References</summary>
<ul>
<li><a href="https://m.163.com/dy/article/L3OQOHEI0534A4SC.html">m.163.com/dy/article/L3OQOHEI0534A4SC.html</a></li>

</ul>
</details>

**Tags**: `#Beijing real estate`, `#property policy`, `#housing provident fund`, `#China economy`, `#home purchase restriction`

---

<a id="item-finance-news-6"></a>
### [Johnson &amp; Johnson Reaches $5.5 Billion Talc Settlement](https://finance.yahoo.com/healthcare/articles/johnson-johnson-jnj-reaches-5-191035095.html) ⭐️ 8.0/10

Johnson &amp; Johnson has reached a $5.5 billion settlement to close years of talc-related lawsuits.

openbb · BRK-B · Aug 7, 19:10

**「Background」** The settlement would cover about 76,000 lawsuits claiming Johnson &amp; Johnson&\#x27;s talc-based products caused cancers such as ovarian cancer and mesothelioma. The company says it will pay up to $3 billion next year, with no additional payments due before 2028.

**「Impact」** If accepted, the settlement would end roughly 15 years of litigation and remove a legal overhang that has weighed on J&amp;J&\#x27;s shares, but it still needs support from plaintiffs&\#x27; law firms; a rejection could extend costly court battles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sokolovelaw.com/product-liability/talcum-powder/johnson-and-johnson/">Johnson &amp; Johnson Talcum Powder Lawsuit | Updated 2026</a></li>
<li><a href="https://www.bbc.com/news/articles/clyqnz52rp6o">Johnson &amp; Johnson offers to pay $5.5bn to settle baby powder lawsuits</a></li>
<li><a href="https://www.zerohedge.com/markets/jjs-proposed-55-billion-talc-settlement-may-lift-remaining-overhang-shares-says-guggenheim">J&amp;J&#x27;s Proposed $5.5 Billion Talc Settlement May &quot;Lift Remaining Overhang&quot; On Shares, Says Guggenheim | ZeroHedge</a></li>
<li><a href="https://solwd.net/jjs-proposed-5-5-billion-talc-settlement-may-lift-remaining-overhang-on-shares-says-guggenheim/">J&amp;J’s Proposed $5.5 Billion Talc Settlement May “Lift Remaining Overhang” On Shares, Says Guggenheim</a></li>
<li><a href="https://www.whalesbook.com/news/English/healthcarebiotech/Johnson-and-Johnson-Offers-dollar55-Billion-to-Resolve-Talc-Lawsuits/6a6964cb288da18bdd3ac212">Johnson &amp; Johnson Offers $5.5 Billion to Resolve Talc Lawsuits | Whalesbook</a></li>

</ul>
</details>

**Tags**: `#Johnson &amp; Johnson`, `#talc settlement`, `#litigation`, `#consumer health`, `#corporate legal`

---

<a id="item-finance-news-7"></a>
### [Premarket movers: Atlassian surges on earnings beat, Trade Desk slides](https://www.cnbc.com/2026/08/07/stocks-making-the-biggest-moves-premarket-atlassian-corporation-wendys-vista-corp-first-solar-airbnb-more.html) ⭐️ 7.0/10

Premarket trading was dominated by earnings and guidance, with Atlassian jumping more than 29% after beating FactSet consensus on fiscal fourth-quarter revenue and earnings, while Trade Desk fell 27% after missing LSEG consensus on second-quarter adjusted earnings and revenue.

rss · CNBC Finance · Aug 7, 13:23

**「Background」** The moves follow quarterly reports and came as President Donald Trump imposed tariffs on products imported to make solar panels, helping lift solar stocks such as First Solar by more than 5%.

**Tags**: `#earnings`, `#premarket`, `#guidance`, `#tech stocks`, `#stock movers`

---

<a id="item-finance-news-8"></a>
### [Australia proposes A$31.30 minimum pay for delivery riders](https://www.twu.com.au/press/food-delivery-workers-to-get-world-first-minimum-standards-on-pay-and-conditions-from-august/) ⭐️ 7.0/10

Australia&\#x27;s Fair Work Commission has proposed a minimum income guarantee of A$31.30 per hour for food delivery riders on platforms such as Uber Eats and DoorDash, with the rules potentially starting as early as August 17, 2026. If approved, platforms would top up a rider&\#x27;s income for a settlement period when it falls below that hourly rate.

telegram · zaihuapd · Aug 7, 15:44

**「Background」** The proposal follows an application by the Transport Workers&\#x27; Union and a joint submission with two major platforms. It is not globally unprecedented: similar minimum-payment rules for delivery platforms already exist in New York, Seattle, and British Columbia.

**Tags**: `#Australia`, `#gig economy`, `#minimum wage`, `#food delivery`, `#labor regulation`

---

<a id="item-finance-news-9"></a>
### [Molson Coors Beats Q2 Earnings Estimates on Pricing and Cost Savings](https://finance.yahoo.com/markets/stocks/articles/molson-coors-q2-earnings-beat-164500953.html) ⭐️ 7.0/10

Molson Coors reported second-quarter earnings that beat analysts&\#x27; estimates, supported by higher pricing and cost savings.

openbb · PG · Aug 7, 16:45

**「Background」** Molson Coors, a major beverage company, reported second-quarter 2025 results that beat analyst estimates as higher pricing, a better sales mix, and cost management helped offset softer demand and cost inflation. Those pressures were visible in the first half of the year: consolidated financial volumes fell 10.2%, operating income dropped 16%, and operating cash flow fell 30%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zacks.com/stock/news/2971371/molson-coors-q2-earnings-beat-estimates-on-pricing-and-cost-savings">Molson Coors Q 2 Earnings Beat Estimates on Pricing and Cost ...</a></li>
<li><a href="https://www.panabee.com/news/molson-coors-beverage-earnings-q2-2025-report">Molson Coors Beverage Earnings Q 2 2025 - Report | Molson Coors ...</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#Molson Coors`, `#beverage`, `#pricing`, `#cost savings`

---

<a id="item-finance-news-10"></a>
### [Diageo FY26 Preliminary Earnings Show North America Pressure](https://finance.yahoo.com/markets/stocks/articles/deo-fy26-preliminary-earnings-show-154700605.html) ⭐️ 7.0/10

Diageo&\#x27;s preliminary fiscal 2026 earnings indicate weakness in North America, signaling potential headwinds for the spirits sector.

openbb · PG · Aug 7, 15:47

**「Background」** Diageo&\#x27;s preliminary results for the fiscal year ended 30 June 2026 show growth in Europe, Latin America and the Caribbean, and Africa, offset by weakness in North America and Asia Pacific; the company assumes the North American market will decline 3% in fiscal 2026 while it improves its share performance.

**「Impact」** The preliminary results signal caution for spirits-sector investors, as North America weakness offset growth in Europe, Latin America, Africa, and Asia-Pacific, with Diageo guiding to organic sales growth similar to fiscal 2025 and only mid-single-digit organic operating profit growth for fiscal 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/deo-fy26-preliminary-earnings-show-154700605.html">DEO FY 26 Preliminary Earnings Show Pressure on North America ...</a></li>
<li><a href="https://www.diageo.com/en/investors/results-reports-and-events/2026-preliminary-results">Fiscal 26 Preliminary Results | Diageo</a></li>
<li><a href="https://www.zacks.com/stock/news/2971291/deo-fy26-preliminary-earnings-show-pressure-on-north-america-weakness">DEO FY 26 Preliminary Earnings Show Pressure on North America ...</a></li>
<li><a href="https://www.diageo.com/en/investors/results-reports-and-events/2026-preliminary-results">Fiscal 26 Preliminary Results | Diageo</a></li>
<li><a href="https://markets.ft.com/data/announce/full?dockey=1323-17167819-5GGLDB98493503CA6H8LP0I25H">Diageo Preliminary Results 2025 – Company Announcement - FT.com</a></li>

</ul>
</details>

**Tags**: `#Diageo`, `#Earnings`, `#North America`, `#Spirits`, `#FY26`

---

<a id="item-finance-news-11"></a>
### [Constellation Signs 920 MW of New Power Deals, Including Walmart PPA](https://finance.yahoo.com/energy/articles/constellation-signed-920-megawatts-power-164558421.html) ⭐️ 7.0/10

Constellation Energy signed 920 megawatts of new power purchase agreements, including one with Walmart, signaling stronger commercial momentum for its clean-energy business. Financial terms of the deals were not disclosed.

openbb · PG · Aug 7, 16:45

**「Background」** Constellation Energy is a clean energy company that sells nuclear power through long-term power purchase agreements \(PPAs\). The 920 megawatts of new agreements, which include a contract with Walmart, were signed in the second quarter and run for 15 to 20 years, with deliveries set to begin between 2029 and 2032.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/08/07/constellation-signed-920-megawatts-of-new-power-deals-including-a-walmart-ppa-heres-what-it-means-for-ceg-stock/">Constellation Signed 920 Megawatts of New Power ... | The Motley Fool</a></li>
<li><a href="https://energynews.pro/en/constellation-energy-raises-2026-guidance-to-1150-1250-per-share">Constellation Energy Raises 2026 Guidance to... | energynews.pro</a></li>

</ul>
</details>

**Tags**: `#Constellation Energy`, `#Power Purchase Agreement`, `#Walmart`, `#Clean Energy`, `#Utility Sector`

---