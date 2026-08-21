---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 254 items, 20 important content pieces were selected

---

**Technology News**
1. [Researcher Accidentally Hijacks e164.arpa, Logs Military Call Requests](#item-tech-news-1) ⭐️ 8.0/10
2. [AI Incident Tracker &\#x27;Felony Bench&\#x27; Sparks Accountability Debate](#item-tech-news-2) ⭐️ 7.0/10
3. [Felony Charges for Deleting Phone Data at US Border](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek v4 Flash gets experimental vision with image input](#item-tech-news-4) ⭐️ 7.0/10
5. [Amazon Reported Buying and Destroying Rare Books for AI Training Data](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [Guangzhou Court Accepts Bankruptcy Liquidation Case of Evergrande’s Main Real Estate Unit](#item-finance-news-1) ⭐️ 9.0/10
2. [Samsung Announces Record 90-110 Trillion Won Shareholder Return Package for 2026](#item-finance-news-2) ⭐️ 8.0/10
3. [China’s New Five-Year Plan Expands Natural Gas and Aims for Peak Oil](#item-finance-news-3) ⭐️ 8.0/10
4. [Europe&\#x27;s Nuclear Plants Cut Output as Heat and Drought Strain River Cooling](#item-finance-news-4) ⭐️ 8.0/10
5. [Oil Nears $100 as Hormuz Traffic Slows on US-Iran Standoff](#item-finance-news-5) ⭐️ 8.0/10
6. [Global Battery Storage Capacity Jumps 65.8% in 2025](#item-finance-news-6) ⭐️ 8.0/10
7. [China Proposes Stricter Outbound Investment Rules in Draft Revision](#item-finance-news-7) ⭐️ 8.0/10
8. [YMTC&\#x27;s STAR Market IPO Application Accepted, Plans to Raise 33 Billion Yuan](#item-finance-news-8) ⭐️ 8.0/10
9. [Broadcom reportedly seeks up to $80 billion in debt for AI chip deal](#item-finance-news-9) ⭐️ 8.0/10
10. [TSM Sales Jump 45% but Chip Sector Still Sells Off](#item-finance-news-10) ⭐️ 8.0/10
11. [TSMC Raises 2026 Spending Plan and Dividend Payouts](#item-finance-news-11) ⭐️ 8.0/10
12. [Nvidia’s $7 Billion Poolside Licensing Deal Sidesteps Acquisition Scrutiny](#item-finance-news-12) ⭐️ 8.0/10
13. [Walmart Shares Extend Decline, Deepening $89 Billion Selloff](#item-finance-news-13) ⭐️ 8.0/10
14. [ConocoPhillips Tops Earnings and Names New CEO; Exxon Mobil Record Profit Misses Expectations](#item-finance-news-14) ⭐️ 8.0/10
15. [Fed holds interest rates steady after Iran war raises oil prices](#item-finance-news-15) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Researcher Accidentally Hijacks e164.arpa, Logs Military Call Requests](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

A security researcher accidentally took control of the e164.arpa domain, which is used by the ENUM telephony-routing system, and logged hundreds of thousands of phone call requests, including calls to military bases. The incident exposes a largely ignored but critical infrastructure vulnerability in the ENUM/e164.arpa delegation, where abandoned or unmaintained DNS infrastructure can be hijacked and used to observe sensitive telephony metadata. This matters because it demonstrates practical privacy and national security risks in the global phone number routing system, even though ENUM never achieved widespread public adoption. The researcher&\#x27;s actions revealed the vulnerability after the fact, with the story surfacing through a public blog post.

hackernews · gavide · Aug 21, 13:11 · [Discussion](https://news.ycombinator.com/item?id=49387570)

**「Background」** ENUM is a DNS-based system that maps international telephone numbers \(in E.164 format\) to Internet identifiers using the special namespace e164.arpa. Delegation under e164.arpa is organized by country code and governed by the ITU, with national regulatory bodies or registries typically managing each country&\#x27;s zone. Although public ENUM has largely fallen out of use, the infrastructure remains and is also used in private number-porting services.

**「Impact」** This incident shows that telephony operators and government agencies relying on ENUM/e164.arpa routing can have their call-routing queries intercepted by an unauthorized party, underscoring the need for auditing and securing such abandoned infrastructure.

**「Community Discussion」** Commenters pointed out that e164.arpa is not completely dead because private number-porting services still use ENUM-style queries over VPNs, and several expressed surprise the researcher was not jailed. Others noted that such infrastructure holes often remain unaddressed until military or national security interests are involved, and one commenter suggested further experimentation to determine whether hijacked requests could lead to actual call termination.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://www.cloudns.net/enum-dns-zones/">What is ENUM? | ENUM (E.164) DNS Services | ClouDNS</a></li>
<li><a href="https://labs.ripe.net/author/hisham_ibrahim/operational-review-of-public-enum-under-e164arpa/">Operational Review of Public ENUM Under e164.arpa | RIPE Labs</a></li>

</ul>
</details>

**Tags**: `#security`, `#telephony`, `#DNS`, `#ENUM`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [AI Incident Tracker &\#x27;Felony Bench&\#x27; Sparks Accountability Debate](https://www.felonybench.com/) ⭐️ 7.0/10

Felony Bench is a website that tracks instances where AI agents inadvertently compromise or affect third-party entities, using the felony label to frame these events as potential crimes. The site is a curated tracker rather than a technical investigation, and the specific incidents and inclusion criteria are not detailed in the available item. Its appearance on Hacker News has drawn attention to unresolved legal and ethical questions about who is responsible when an autonomous agentic loop causes harm, such as violations of laws like the CFAA. The project highlights the growing gap between AI capabilities and existing frameworks for accountability.

hackernews · colinprince · Aug 21, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49389430)

**「Background」** Felony Bench is a web-based tracker that counts unique instances where AI agents inadvertently compromise or affect third-party entities, often framed as a benchmark for AI legal missteps. It was launched to provide a quantifiable score of questionable or legally weighty decisions made by autonomous agents as they become more prevalent, amid growing debates about accountability and legal responsibility for AI behavior. The name draws on the legal concept of a felony to highlight that machines themselves cannot be held criminally liable even when their actions cause harm, making the tracker a catalog of incidents rather than a technical benchmark.

**「Community Discussion」** Commenters debated which party—user, third-party model host, harness developer, or LLM developer—would be prosecuted for AI-caused violations, with some noting that intent requirements make the felony framing overstated. Others criticized OpenAI&\#x27;s handling of the Hugging Face incident, arguing the company treated its agent&\#x27;s harmful actions as an uncontrollable act of God rather than a result of its own cultural and R&amp;D choices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.felonybench.com/">Felony Bench</a></li>
<li><a href="https://news.linxi.com.au/news/felony-bench-launched-to-track-ai-agent-legal-missteps">Felony Bench: New Metric Tracks AI Agent Legal Missteps ...</a></li>

</ul>
</details>

**Tags**: `#AI accountability`, `#AI safety`, `#legal implications`, `#incident tracking`, `#ethics`

---

<a id="item-tech-news-3"></a>
### [Felony Charges for Deleting Phone Data at US Border](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 7.0/10

A US citizen, Samuel Tunick, has been charged with a felony for deleting phone data at the US border, according to a New York Times report. The case highlights the legal risks travelers face when using technical countermeasures such as device wiping or encryption to protect data during border searches. The discussion among practitioners focuses on methods like imaging and restoring phones or automated factory resets as possible safeguards. The outcome could affect how travelers approach digital privacy at ports of entry.

hackernews · floathub · Aug 21, 12:10 · [Discussion](https://news.ycombinator.com/item?id=49386895)

**「Background」** At US ports of entry, Customs and Border Protection can search electronic devices without a warrant, and travelers who refuse to unlock their phones can face detention or device seizure. Samuel Tunick, an Atlanta resident, was stopped at Hartsfield-Jackson Atlanta International Airport as he returned from abroad and gave border agents a &quot;duress password&quot; on his GrapheneOS phone, which immediately and irreversibly deleted all data and eSIMs stored on the device. A grand jury later indicted him on a felony charge, underscoring the legal conflict between border-search authority and travelers who deliberately use privacy tools like duress passwords to wipe devices.

**「Impact」** The case could deter US citizens from using data-deletion or encryption tools at border crossings for fear of criminal prosecution, while fueling demand for privacy-preserving device setups. Technical observers are exploring methods to avoid both data exposure and device seizure, though these approaches remain legally untested.

**「Community Discussion」** Commenters debate practical countermeasures, with some proposing automated wiping or encryption setups that require a second key, while others express cynicism about legal protections at the border.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/gadgets/2026/07/activist-charged-with-felony-after-giving-border-agent-duress-code-that-wiped-his-phone/">Activist charged with felony after giving border agent... - Ars Technica</a></li>
<li><a href="https://www.nytimes.com/2026/07/28/us/duress-password-phone-wipe-charge.html">A U.S. Citizen Deleted His Phone ’s Data . Now He Faces a Felony ...</a></li>
<li><a href="https://boingboing.net/2026/07/25/grapheneos-duress-password-border-search.html">Man prosecuted after GrapheneOS duress password wipes phone</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#border search`, `#digital rights`, `#data encryption`, `#surveillance`

---

<a id="item-tech-news-4"></a>
### [DeepSeek v4 Flash gets experimental vision with image input](https://api-docs.deepseek.com/guides/vision/) ⭐️ 7.0/10

DeepSeek released DeepSeek-v4-flash-vision-exp, an experimental variant of its v4 Flash model that adds image input support. Before inference, images are automatically resized to roughly 800×800 pixels, converted into tokens based on their dimensions, and billed together with text tokens. The release directly addresses a known limitation: prior v4 Flash versions reportedly assumed they had vision capabilities and invented text-based image analysis tools when they actually could not see images. Community testing shows promise for screenshot analysis, but also reveals continued accuracy problems, including an incorrect answer to a simple clock-reading test. A dedicated news announcement with benchmarks is available at api-docs.deepseek.com/news/news260821/.

hackernews · dares2573 · Aug 21, 10:33 · [Discussion](https://news.ycombinator.com/item?id=49386163)

**「Background」** DeepSeek&\#x27;s v4 Flash line is a set of API-accessible language models that previously handled only text input, which led some users to report that older versions hallucinated vision abilities and invented text-based image analysis. The new experimental DeepSeek-V4-Flash-Vision-Exp model, announced on August 21, 2026, adds image input support through the Chat Completions API, converting images into tokens for billing at standard v4 Flash pricing, with images being automatically resized and tokenized before inference.

**「Impact」** Developers and users relying on DeepSeek for image-based tasks such as screenshot analysis now have a real vision-enabled experimental option, though the ~800×800 resizing cap and lingering reading inaccuracies mean it is not yet a drop-in replacement for more mature vision models.

**「Community discussion」** Commenters are cautiously optimistic: one notes the vision variant is promising for precisely viewing Playwright screenshots, and another appreciates it addressing v4 Flash 0731&\#x27;s tendency to hallucinate vision capabilities, but independent testing shows it still fails a simple clock test that Qwen3.8 27B got nearly right. Another commenter cautions that the ~800×800 resizing may be too low for OCR of full A4 or Letter-sized pages.

<details><summary>References</summary>
<ul>
<li><a href="https://pixomi.ai/blog/deepseek-v4-flash-vision-exp/">DeepSeek V 4 Flash Vision Exp: New Multimodal Model | Pixomi AI</a></li>
<li><a href="https://chat-deep.ai/models/deepseek-v4-flash-vision-exp/">DeepSeek V 4 Flash Vision Exp: Image API, Pricing &amp; Examples</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260821/">DeepSeek - V 4 - Flash - Vision -Exp Release... | DeepSeek API Docs</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#vision`, `#model release`, `#AI`, `#LLM`

---

<a id="item-tech-news-5"></a>
### [Amazon Reported Buying and Destroying Rare Books for AI Training Data](https://www.404media.co/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-training-facility/) ⭐️ 7.0/10

An investigation by 404 Media reports that Amazon has been buying large numbers of physical books, scanning them for AI training data, and destroying the books in the process. Investigators placed a tracking device inside a rare book and traced it to an Amazon warehouse in Las Vegas, Nevada, where employees said they receive printed books, cut off the bindings to speed up scanning, and then discard the pages. The report follows similar claims about Anthropic and raises questions about the sourcing and destruction of copyrighted physical works for AI development. The exact scale of the operation and Amazon&\#x27;s official response are not detailed in the item.

telegram · zaihuapd · Aug 21, 04:52

**「Background」** AI training data often includes books because they provide long, high-quality text, but obtaining that text at scale has driven companies to buy physical copies and digitize them. This practice is controversial because much of the content is copyrighted, and in Amazon&\#x27;s case the physical books are reportedly destroyed after scanning, raising concerns about waste, preservation, and legal liability.

**「Impact」** The investigation documents that rare physical books are being destroyed as part of Amazon&\#x27;s AI data collection, meaning those copies are permanently lost to collectors, libraries, and archives.

**Tags**: `#AI training data`, `#Amazon`, `#data sourcing`, `#ethics`, `#investigation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Guangzhou Court Accepts Bankruptcy Liquidation Case of Evergrande’s Main Real Estate Unit](https://weibo.com/1642585887/5334339212283916) ⭐️ 9.0/10

On Aug. 21, the Guangzhou Intermediate People’s Court accepted the bankruptcy liquidation case of Evergrande Real Estate Group, the onshore real estate headquarters of China Evergrande. As of end-2022, the company had total assets of 1.47 trillion yuan and total liabilities of 1.83 trillion yuan.

telegram · zaihuapd · Aug 21, 05:35

**「Background」** The company is the onshore headquarters entity of China Evergrande, one of the country’s largest property developers, and its auditor previously issued a disclaimer of opinion on its financial statements.

**「Impact」** Industry insiders said the company is severely insolvent and has no restructuring value, and that the actual recovery rate for creditors is likely to be very low because asset sale values will depend on market conditions.

**Tags**: `#恒大地产`, `#破产清算`, `#中国房地产`, `#债务危机`, `#法院裁定`

---

<a id="item-finance-news-2"></a>
### [Samsung Announces Record 90-110 Trillion Won Shareholder Return Package for 2026](https://www.cnbc.com/2026/08/21/samsung-shareholder-return-package-sk-hynix-buyback-ai-chip-boom.html) ⭐️ 8.0/10

Samsung Electronics said it expects shareholder returns of 90 trillion to 110 trillion won \($65.1 billion to $79.52 billion\) in 2026, which it called the largest ever by a Korean company. The package includes about 30 trillion won in cash dividends for the third quarter, with final details expected from a board meeting in late October.

rss · CNBC Finance · Aug 21, 09:08

**「Background」** The announcement follows SK Hynix&\#x27;s 40 trillion won share buyback and builds on Samsung&\#x27;s existing 2024-2026 shareholder return program, under which it pledged to return 50% of free cash flow and maintain annual regular dividends of 9.8 trillion won.

**Tags**: `#Samsung`, `#shareholder returns`, `#AI chips`, `#South Korea`, `#SK Hynix`

---

<a id="item-finance-news-3"></a>
### [China’s New Five-Year Plan Expands Natural Gas and Aims for Peak Oil](https://oilprice.com/Energy/Crude-Oil/Chinas-New-Five-Year-Plan-Preps-the-Nation-for-Peak-Oil.html) ⭐️ 8.0/10

China’s new oil and gas five-year plan, released Monday by the National Development and Reform Commission and the National Energy Administration, sets 2030 targets for liquefied natural gas \(LNG\) terminal capacity of 200 million tonnes, pipeline capacity of 114 billion cubic metres, and natural gas storage capacity that is 13% above national consumption, while also calling for higher domestic oil production and for oil consumption to peak.

rss · OilPrice.com · Aug 21, 22:00

**「Background」** Beijing’s previous stockpiling strategy largely shielded China when the Strait of Hormuz closed in February, but the country remains dependent on fuel imports as it pushes for energy self-sufficiency.

**Tags**: `#China energy policy`, `#natural gas`, `#peak oil`, `#energy security`, `#LNG infrastructure`

---

<a id="item-finance-news-4"></a>
### [Europe&\#x27;s Nuclear Plants Cut Output as Heat and Drought Strain River Cooling](https://oilprice.com/Alternative-Energy/Nuclear-Power/Low-Rivers-High-Stakes-Europes-Nuclear-Cooling-Crisis.html) ⭐️ 8.0/10

Extreme heat and record-low river levels have forced European nuclear operators to cut output or shut reactors, including Romania&\#x27;s only operating reactor and up to 15% of France&\#x27;s nuclear capacity. Dutch bank Triodos estimates the wider summer heat could cost the EU around $207.7 billion, or about 1% of GDP, largely through weaker labour productivity.

rss · OilPrice.com · Aug 21, 20:00

**「Background」** Nuclear plants release waste heat into rivers, but low water levels concentrate that heat and can push temperatures above legal limits meant to protect aquatic life. Europe has already endured five heatwaves this summer, causing drought and record temperatures.

**「Impact」** Triodos says the broader effects of the heat on the EU include constrained energy production and higher electricity prices, lower agricultural output and higher food prices, transport disruption, and reduced labour productivity.

**Tags**: `#nuclear power`, `#European energy`, `#heatwave`, `#economic losses`, `#energy supply`

---

<a id="item-finance-news-5"></a>
### [Oil Nears $100 as Hormuz Traffic Slows on US-Iran Standoff](https://oilprice.com/Energy/Crude-Oil/Oil-Nears-100-as-Trumps-Economic-D-Day-Raises-the-Stakes.html) ⭐️ 8.0/10

Brent crude is trading at $94 per barrel after the Trump administration&\#x27;s &quot;Economic D-Day&quot; campaign against Iran slowed traffic through the Strait of Hormuz to single digits, and the article forecasts momentum toward $100 will continue in the remaining days of August.

rss · OilPrice.com · Aug 21, 15:01

**「Background」** The Strait of Hormuz is a critical chokepoint for global oil and LNG shipments; the White House has announced &quot;economic warfare&quot; against Tehran and threatened &quot;tremendous consequences&quot; for countries trading with Iran, putting Chinese imports in the crosshairs.

**「Impact」** Asian buyers are already adjusting: Chinese independent refiners are turning to Brazilian and Iraqi crude after Iranian barrels moved from a $3 discount to a $2 premium, while Japan&\#x27;s US crude imports hit a record 891,000 barrels per day in July.

**Tags**: `#oil prices`, `#geopolitical risk`, `#Strait of Hormuz`, `#energy markets`, `#Iran sanctions`

---

<a id="item-finance-news-6"></a>
### [Global Battery Storage Capacity Jumps 65.8% in 2025](https://oilprice.com/Energy/Energy-General/The-Battery-Boom-Is-Becoming-Impossible-to-Ignore.html) ⭐️ 8.0/10

Global battery storage capacity reached 301.7 gigawatts \(GW\) in 2025, up 65.8% from 182.0 GW in 2024, according to the Energy Institute’s 2026 Statistical Review of World Energy, with China accounting for nearly half of the world’s total.

rss · OilPrice.com · Aug 21, 14:00

**「Background」** Batteries store electricity when it is abundant and return it to the grid later, which helps integrate intermittent solar and wind power. The capacity figures measure power output in gigawatts, not total stored energy, which would be measured in gigawatt-hours.

**「Impact」** As grid-scale storage expands, particularly in China and the United States, utilities can shift daytime solar power into evening peak hours, potentially reducing the need for other generating resources during high-demand periods.

**Tags**: `#battery storage`, `#energy transition`, `#renewable energy`, `#China`, `#electricity grid`

---

<a id="item-finance-news-7"></a>
### [China Proposes Stricter Outbound Investment Rules in Draft Revision](https://yyglxxbsgw.ndrc.gov.cn/htmls/article/article.html?articleId=2c97d16c-9ff00a63-01a0-230bacc4-0001) ⭐️ 8.0/10

China&\#x27;s National Development and Reform Commission \(NDRC\) published a draft revision to outbound investment management rules, proposing tighter controls on capital leaving the country and replacing the 2017 measures. Under the draft, outbound investments without valid approval or filing would not be processed by foreign-exchange, customs, or financial firms, and security review would expand to transfers and disposal of existing overseas assets.

telegram · zaihuapd · Aug 21, 13:05

**「Background」** The draft would replace the 2017 Enterprise Overseas Investment Management Measures and is open for public comment, so final provisions could change.

**「Impact」** If adopted, Chinese companies and investors making outbound investments would face more pre-transaction approvals, broader security reviews, and harsher penalties, while financial firms handling non-compliant transactions would be reported to regulators.

**Tags**: `#发改委`, `#对外投资`, `#资本管制`, `#监管政策`, `#资金出境`

---

<a id="item-finance-news-8"></a>
### [YMTC&\#x27;s STAR Market IPO Application Accepted, Plans to Raise 33 Billion Yuan](https://api3.cls.cn/share/article/2461025?os=android&amp;amp;sv=8.8.2&amp;amp;app=cailianpress) ⭐️ 8.0/10

YMTC’s STAR Market IPO application has been accepted, and the NAND flash memory maker plans to raise 33 billion yuan. Its prospectus shows first-quarter 2026 revenue of 47.04 billion yuan and net profit of 33.38 billion yuan.

telegram · zaihuapd · Aug 21, 14:26

**「Background」** YMTC is a leading Chinese NAND flash memory producer, and the STAR Market is Shanghai’s technology-focused board.

**Tags**: `#科创板IPO`, `#长江存储`, `#半导体`, `#融资`, `#NAND`

---

<a id="item-finance-news-9"></a>
### [Broadcom reportedly seeks up to $80 billion in debt for AI chip deal](https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-80-billion-debt-171925920.html) ⭐️ 8.0/10

Broadcom is reportedly seeking up to $80 billion in debt financing for an AI chip-related deal.

openbb · NVDA · Aug 21, 17:19

**「Background」** Broadcom has entered discussions with lenders to raise $70 billion to $80 billion in debt, a financing arrangement that would support artificial intelligence companies, including Anthropic.

**「Impact」** Broadcom&\#x27;s reported plan to raise $70–80 billion in debt would support AI firms such as Anthropic and expand AI chip infrastructure, increasing leverage for Broadcom and giving lenders significant exposure to the AI sector.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/21/broadcom-debt-deal-expected-to-reach-upwards-of-70-billion-sources.html">Broadcom debt deal expected to reach upwards of $70 billion, sources say</a></li>
<li><a href="https://qz.com/broadcom-debt-financing-ai-chips-anthropic-082126">Broadcom seeks up to $80 billion in debt for AI chip deal</a></li>
<li><a href="https://www.cnbc.com/2026/08/21/broadcom-debt-deal-expected-to-reach-upwards-of-70-billion-sources.html">Broadcom debt deal expected to reach upwards of $70 billion ...</a></li>
<li><a href="https://www.gurufocus.com/news/9047966/broadcom-avgo-plans-7080-billion-debt-financing-for-ai-chip-initiative">Broadcom (AVGO) Plans $70-80 Billion Debt Financing for AI ...</a></li>
<li><a href="https://impactnews-wire.com/broadcoms-80-billion-ai-chip-financing-bet-signals-the-next-phase-of-the-ai-boom/">Broadcom’s $80 Billion AI Chip Financing Bet Signals the Next ...</a></li>

</ul>
</details>

**Tags**: `#Broadcom`, `#AI chips`, `#debt financing`, `#semiconductors`, `#M&amp;A`

---

<a id="item-finance-news-10"></a>
### [TSM Sales Jump 45% but Chip Sector Still Sells Off](https://finance.yahoo.com/technology/ai/articles/taiwan-semiconductor-tsm-sales-just-205844477.html) ⭐️ 8.0/10

Taiwan Semiconductor \(TSM\) reported a 45% jump in sales, yet chip stocks are still selling off, according to the report.

openbb · NVDA · Aug 21, 20:58

**「Background」** Taiwan Semiconductor Manufacturing \(TSMC\), the world’s largest contract chipmaker, reported July revenue of NT$467.58 billion \(about $14.5 billion\), up roughly 45% from a year earlier. The company’s monthly sales are watched closely because it makes advanced chips for major AI buyers such as Nvidia, AMD, and Apple, so the sell-off reflects investor debate over whether the recent AI-driven spending boom is already reflected in chip stock prices.

**「Impact」** Investors in AI and semiconductor stocks closely watch TSM&\#x27;s monthly sales because the company makes chips for big customers like Nvidia and Google, so the 45% surge is seen as a sign that AI hardware demand remains strong despite the broader sector selloff.

<details><summary>References</summary>
<ul>
<li><a href="https://www.insidermonkey.com/blog/taiwan-semiconductor-tsm-sales-just-jumped-45-why-is-the-chip-sector-still-selling-off-1809400/">Taiwan Semiconductor (TSM) Sales Just Jumped 45%. Why is the Chip Sector Still Selling Off? - Insider Monkey</a></li>
<li><a href="https://www.gurufocus.com/news/9041261/tsmc-stock-slides-over-4-despite-45-revenue-surge">TSMC Stock Slides Over 4% Despite 45% Revenue Surge</a></li>
<li><a href="https://memeburn.com/tsmc-revenue-surges-45/">TSMC Revenue Surges 45% as AI Chip Demand From Nvidia, AMD, and Apple - Memeburn</a></li>
<li><a href="https://www.cnbc.com/2026/08/10/tsmc-revenue-surge-ai-chip-big-tech.html">TSMC sees 45% sales surge as AI demand stays strong - CNBC</a></li>

</ul>
</details>

**Tags**: `#Taiwan Semiconductor`, `#semiconductor sector`, `#sales growth`, `#market selloff`, `#chip industry`

---

<a id="item-finance-news-11"></a>
### [TSMC Raises 2026 Spending Plan and Dividend Payouts](https://finance.yahoo.com/markets/stocks/articles/tsmc-commits-higher-capex-2026-154100814.html) ⭐️ 8.0/10

TSMC announced that it plans to increase its capital expenditure in 2026 and raise its dividend payouts, signaling strong demand and financial strength. No specific figures were provided in the available information.

openbb · NVDA · Aug 21, 15:41

**「Background」** TSMC has been expanding production capacity to meet AI chip demand, and its board recently approved a capital budget of about NT$950.3 billion following record earnings. The company paid an annual dividend of TWD 18 per share in 2025 and has since raised quarterly payouts to NT$7 per share.

**「Impact」** The higher capital spending points to record fab construction and expansion, which supports semiconductor equipment suppliers and AI-related supply chains as TSMC scales up capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://247wallst.com/investing/2026/02/25/tsmc-raises-dividend-28-while-38-revenue-growth-reframes-the-geopolitical-risk/">TSMC Raises Dividend 28% While 38% Revenue Growth Reframes the Geopolitical Risk - 24/7 Wall St.</a></li>
<li><a href="https://finance.biggo.com/news/3a6e6629-4a68-4d6c-a39d-72e6a2d2c806">TSMC Earns Nearly Half Its Share Capital in Q2, Declares NT$7 Dividend, Approves Nearly NT$1 Trillion Capex — BigGo Finance</a></li>
<li><a href="https://parameter.io/tsmc-tsm-increases-dividend-after-record-earnings-and-strong-ai-growth/">TSMC (TSM): Increases Dividend After Record Earnings and Strong AI Growth - Parameter</a></li>
<li><a href="https://www.digitimes.com/news/a20260416PD222/tsmc-equipment-capex-supply-chain-taiwan-2026.html">TSMC capex hits US$56 billion, reshaping global semiconductor supply chain</a></li>
<li><a href="https://seekingalpha.com/news/4614953-what-tsmcs-capex-surge-could-mean">What TSMC&#x27;s capex surge could mean (TSM:NYSE) | Seeking Alpha</a></li>
<li><a href="https://tech-insider.org/tsmc-earnings-capex-arizona-2026/">TSMC Earnings Jump 77%, Capex Hits $64B [2026]</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductor`, `#capital expenditure`, `#dividends`, `#industry outlook`

---

<a id="item-finance-news-12"></a>
### [Nvidia’s $7 Billion Poolside Licensing Deal Sidesteps Acquisition Scrutiny](https://finance.yahoo.com/technology/ai/articles/nvidia-7-billion-poolside-deal-224313075.html) ⭐️ 8.0/10

A report says Nvidia has entered a $7 billion licensing deal with Poolside, structuring the investment to avoid traditional acquisition review. The move signals a major new investment in AI.

openbb · NVDA · Aug 21, 22:43

**「Background」** The reported $7 billion total consists of a $6 billion payment for a non-exclusive license to Poolside&\#x27;s Model Factory software, a $1 billion investment at a $12 billion valuation, and job offers to 109 Poolside staff. Nvidia has used this license-plus-hire structure before, making it the third such deal in a year.

<details><summary>References</summary>
<ul>
<li><a href="https://temperature2.com/p/2026-08-21-nvidia-poolside-6-billion-license-deal/">Nvidia pays Poolside $6B for its model-building tech</a></li>
<li><a href="https://gentic.news/article/nvidia-pays-6b-for-poolside-s">Nvidia Pays $6B for Poolside &#x27;s Model… | gentic.news</a></li>
<li><a href="https://www.binance.com/ru/square/post/08-21-2026-nvidia-to-pay-poolside-6-billion-in-licensing-and-hiring-deal-358073306956018">Nvidia заплатит Poolside ... | Binance News на Binance Square</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Poolside`, `#AI investment`, `#licensing deal`, `#regulatory scrutiny`

---

<a id="item-finance-news-13"></a>
### [Walmart Shares Extend Decline, Deepening $89 Billion Selloff](https://finance.yahoo.com/markets/stocks/articles/walmart-falls-again-89-billion-190210640.html) ⭐️ 8.0/10

Walmart shares fell again, extending a selloff that has erased about $89 billion in market value.

openbb · PG · Aug 21, 19:02

**「Background」** Walmart Inc. is a large U.S. retailer whose stock trades on the Nasdaq. The article reports another drop in its shares, deepening a selloff that has already erased about $89 billion in market value.

**「Impact」** Walmart&\#x27;s deepening selloff—now an $89 billion market-value loss—is weighing on the Dow Jones Industrial Average and retail-sector ETFs, as investors focus on the company&\#x27;s slowest same-store sales growth since 2020 rather than a broad market pullback.

<details><summary>References</summary>
<ul>
<li><a href="https://stock.walmart.com/">Walmart Inc. (WMT)</a></li>
<li><a href="https://eciks.org/22373-dow-jones-falls-700-points">Dow Jones falls 700 points as Walmart, Boeing stocks slide</a></li>
<li><a href="https://247wallst.com/investing/2026/08/20/walmart-drops-8-on-slowest-same-store-sales-growth-since-2020-target-holds-steady-costco-eases/">Walmart Drops 8% on Slowest Same-Store Sales Growth Since 2020; Target Holds Steady, Costco Eases - 24/7 Wall St.</a></li>

</ul>
</details>

**Tags**: `#Walmart`, `#retail`, `#stock selloff`, `#market valuation`, `#large-cap`

---

<a id="item-finance-news-14"></a>
### [ConocoPhillips Tops Earnings and Names New CEO; Exxon Mobil Record Profit Misses Expectations](https://finance.yahoo.com/energy/articles/conocophillips-cop-beats-earnings-names-193428889.html) ⭐️ 8.0/10

ConocoPhillips beat earnings expectations and announced a new CEO, while Exxon Mobil posted record profit that fell short of analyst forecasts.

openbb · BRK-B · Aug 21, 19:34

**「Background」** ConocoPhillips announced on August 6 that CEO Ryan Lance will retire after 14 years, with CFO Andy O&\#x27;Brien set to take over on September 1, after the company posted better-than-expected quarterly results.

**「Impact」** ConocoPhillips shares slipped about 1% despite the earnings beat and CEO transition, while Exxon Mobil&\#x27;s record profit also failed to lift its stock, suggesting investors are focused on falling crude prices ahead. Analysts cited by Morningstar forecast a 15% decline in ConocoPhillips&\#x27; 2026 earnings due to lower oil prices.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/energy/articles/conocophillips-cop-beats-earnings-names-193428889.html?fr=sycsrp_catchall">ConocoPhillips (COP) Beats Earnings and Names New CEO While ...</a></li>
<li><a href="https://www.reuters.com/business/energy/conocophillips-beats-quarterly-profit-estimates-2026-08-06/">ConocoPhillips CEO Ryan Lance departs as oil producer posts ...</a></li>
<li><a href="https://finance.yahoo.com/energy/articles/conocophillips-cop-beats-earnings-names-193428889.html?fr=sycsrp_catchall">ConocoPhillips (COP) Beats Earnings and Names New CEO While ...</a></li>
<li><a href="https://www.conocophillips.com/investor-relations/">Investors - ConocoPhillips Earnings :: ExxonMobil Holdings Corporation (XOM) ConocoPhillips CEO Ryan Lance Departs as Oil Producer Posts ... FinancialContent - Exxon Mobil Smashes Profit Estimates as ... COP - ConocoPhillips News | Morningstar</a></li>

</ul>
</details>

**Tags**: `#ConocoPhillips`, `#Exxon Mobil`, `#earnings`, `#CEO appointment`, `#oil &amp; gas`

---

<a id="item-finance-news-15"></a>
### [Fed holds interest rates steady after Iran war raises oil prices](https://news.google.com/rss/articles/CBMilAFBVV95cUxOWVgwU0l2bjYwREJ2NE9WVC1ObnpJa3Qxa2syS0lmUXphVm8zTWpnYVJ5NXpFZmxWYUZlVXpmc3ZFQzk2ZnZlYjNSUHRPb3F1emZhVDdPNEMxak1mM2wzOEZtYnA5dklfUFlfOUdVRU5lSXNmTlhqMy1pUElaMjNBTEFJbV9IRHNkRGt1NHJKVDVFd1Za0gGaAUFVX3lxTE9IOWFDX2MzMVhjUXl2VE1oTGNTTlowMmxkMUZnNEQ1TzhKemJ3TmlSTElmdzVPQ3VmR2E3OGdNLXN2dVBHQ2xiLXl0WWJfdjBUQktuSnNwbTNQV3puQzBJTUVZS295S2lHYU9iQVpFd05FQkw4WmhmZ2EyU3dCUWt0bHNCUy1xX0pHME5ZbVBlZ1RXSkxnSVZ1TWc?oc=5) ⭐️ 8.0/10

The Federal Reserve held interest rates unchanged in its first decision since the Iran war pushed oil prices up, though three committee members voted to raise rates amid high prices.

google\_news · ABC News - Breaking News, Latest News and Videos · Aug 21, 11:42

**「Background」** The Fed kept its benchmark interest rate unchanged at its first policy meeting since the Iran war began, marking its second consecutive hold in 2026. The conflict has pushed oil prices to their highest in nearly four years and stoked inflation concerns, and one official dissented, reflecting uncertainty about the war&\#x27;s economic impact.

**「Impact」** The Fed&\#x27;s hold leaves U.S. borrowing costs unchanged, so households and businesses continue to face current elevated loan and mortgage rates while officials weigh how the Iran-related oil price spike affects inflation.

<details><summary>References</summary>
<ul>
<li><a href="https://abcnews.com/Business/fed-issue-interest-rate-decision-gas-prices-rise/story?id=135130446">Fed holds interest rates steady as economy weathers resurgent ...</a></li>
<li><a href="https://abcnews.com/Business/fed-set-adjust-interest-rates-1st-time-war/story?id=131155455">Fed holds interest rates steady in 1st move since Iran war ...</a></li>
<li><a href="https://www.supplychaindive.com/news/fed-holds-rates-steady-flags-uncertainty-as-oil-price-soars-amid-war/815113/">Fed holds rates steady, flags uncertainty as oil price soars ...</a></li>
<li><a href="https://abcnews.com/Business/fed-issue-interest-rate-decision-gas-prices-rise/story?id=135130446">Fed holds interest rates steady as economy weathers resurgent inflation - ABC News</a></li>

</ul>
</details>

**Tags**: `#federal-reserve`, `#monetary-policy`, `#interest-rates`, `#geopolitics`, `#oil-prices`

---