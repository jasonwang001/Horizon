---
layout: default
title: "Horizon Summary: 2026-08-21 (EN)"
date: 2026-08-21
lang: en
---

> From 237 items, 24 important content pieces were selected

---

**Technology News**
1. [GitHub Details August 17 Outage, Cites Retry Loops and VS Code Bug](#item-tech-news-1) ⭐️ 8.0/10
2. [AliExpress silent WebAudio fingerprinting disrupts Bluetooth multipoint](#item-tech-news-2) ⭐️ 8.0/10
3. [Malicious arrayref Rust crate runs build-time payload](#item-tech-news-3) ⭐️ 8.0/10
4. [Terence Tao Warns AI May Trigger a Proof-Surplus Crisis](#item-tech-news-4) ⭐️ 8.0/10
5. [On-Device Piano Autocomplete Trained Into 125M Transformer](#item-tech-news-5) ⭐️ 7.0/10
6. [Linux 7.2 Released with HDMI 2.1 Support for AMD Open-Source Drivers](#item-tech-news-6) ⭐️ 7.0/10
7. [Spectral Neuron: New ML Primitive for Scalable, Interpretable Models](#item-tech-news-7) ⭐️ 7.0/10
8. [OpenAI Previews Zero Data Retention and Private Security Processing](#item-tech-news-8) ⭐️ 7.0/10
9. [Reverse Image Service Breach Exposes Millions of Face Photos](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Evergrande Founder Xu Jiayin Sentenced to Life; Company Fined Billions](#item-finance-news-1) ⭐️ 9.0/10
2. [Fed holds interest rates steady after Iran war spikes oil prices](#item-finance-news-2) ⭐️ 9.0/10
3. [Fed Faces One of Its Most Unpredictable Meetings in Years](#item-finance-news-3) ⭐️ 9.0/10
4. [Federal Reserve Holds Interest Rates Steady, Leaves Door Open to Hike](#item-finance-news-4) ⭐️ 9.0/10
5. [Bank of England Releases July 2026 Monetary Policy Report](#item-finance-news-5) ⭐️ 9.0/10
6. [Houthis Plan to Seize Land Around Bab el-Mandeb Oil Chokepoint](#item-finance-news-6) ⭐️ 8.0/10
7. [EPA Allows Early Switch to Winter-Grade Gasoline](#item-finance-news-7) ⭐️ 8.0/10
8. [China Steps Up Domestic Oil and Gas Output to Bolster Energy Security](#item-finance-news-8) ⭐️ 8.0/10
9. [Alibaba Fiscal Q1 Net Profit Falls 76% to 10.54 Billion Yuan](#item-finance-news-9) ⭐️ 8.0/10
10. [AMD Slips as Google Expands $120 Billion Custom-Chip Push](#item-finance-news-10) ⭐️ 8.0/10
11. [Broadcom seeks over $60 billion in AI debt financing, Bloomberg reports](#item-finance-news-11) ⭐️ 8.0/10
12. [Broadcom Reportedly Seeks Over $60 Billion for AI Debt Deal](#item-finance-news-12) ⭐️ 8.0/10
13. [ASML Gains as TSMC Raises Spending Forecast to $85 Billion](#item-finance-news-13) ⭐️ 8.0/10
14. [TSMC&\#x27;s 2027 Capex Forecast Reaches $85 Billion](#item-finance-news-14) ⭐️ 8.0/10
15. [Stripe agrees to acquire AI model gateway OpenRouter](#item-finance-news-15) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GitHub Details August 17 Outage, Cites Retry Loops and VS Code Bug](https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/) ⭐️ 8.0/10

GitHub published a post-incident analysis of its August 17 outage, identifying client-side retry loops and a latent retry bug in VS Code as key amplification factors that increased traffic by approximately 10x and delayed recovery for the Copilot Token Service. The analysis says errors in internal services triggered the retry loop during recovery, and the company is outlining reliability work ahead to prevent similar cascading failures. It also notes that monthly commits have grown from 1.4 billion to 2.9 billion since April, providing context for the load on the platform. GitHub emphasized the need to address client retry behavior and improve infrastructure resilience.

hackernews · 0xedb · Aug 20, 19:22 · [Discussion](https://news.ycombinator.com/item?id=49378957)

**「Background」** GitHub is a widely used code hosting platform that experienced a major outage on August 17. During the incident, errors in internal services caused a client-side retry loop that increased traffic during recovery, while a delayed reply to a single internal endpoint triggered a latent retry bug in VS Code, amplifying traffic approximately 10x and delaying recovery for the Copilot Token Service. This illustrates how client retry behavior can turn small failures into large-scale cascading problems.

**「Impact」** The outage disrupted GitHub services for users, with the Copilot Token Service recovery delayed by the VS Code retry bug and overall traffic amplified during the incident. The post-mortem highlights the importance of careful retry policy design to avoid worsening outages in large-scale infrastructure.

**「Community Discussion」** Commenters debated the role of retries, with one criticizing the industry trend of hiding errors behind spinners and another questioning retries in desktop services, while others expressed astonishment at GitHub&\#x27;s commit growth from 1.4 billion to 2.9 billion monthly and gratitude for the company&\#x27;s free, ad-free service at scale.

**Tags**: `#outage`, `#reliability`, `#github`, `#retry-bugs`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [AliExpress silent WebAudio fingerprinting disrupts Bluetooth multipoint](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) ⭐️ 8.0/10

A blog post by laserphile documents how AliExpress pages run silent WebAudio fingerprinting that is disruptive enough to break Bluetooth multipoint connections. The technique lets the site identify devices or users through audio-context quirks while producing an apparent audio stream that can confuse Bluetooth stacks and headsets. Multiple users in the Hacker News discussion corroborate Bluetooth anomalies, including hearing-aid amplification changes after visiting sites and car audio misinterpreting the AliExpress iOS app in the background as an audio command. The case highlights a privacy-invasive fingerprinting vector that also causes functional side effects beyond tracking.

hackernews · emctech · Aug 20, 10:08 · [Discussion](https://news.ycombinator.com/item?id=49372583)

**「Background」** WebAudio fingerprinting is a browser-tracking technique that uses subtle differences in how devices process audio signals to build a persistent identifier. AliExpress&\#x27;s anti-abuse scripts reportedly create hidden WebAudio graphs connected to the audio destination with zero gain, so no sound is audible but the system audio path is held open. That open path prevents multipoint Bluetooth headphones from switching audio to another connected device, explaining the Bluetooth anomalies users observe.

**「Impact」** AliExpress visitors with Bluetooth multipoint audio devices can lose incoming audio from a second device while the page is open: one user confirmed that opening the AliExpress page kept the PC-headphone link active and blocked phone audio.

**「Community Discussion」** Commenters mostly agree the behaviour is suspicious and annoying, with several describing concrete Bluetooth side effects on hearing aids and car systems. One developer notes that WebAudio fingerprinting is largely mitigated in Firefox and points to ongoing efforts, while another expects Apple&\#x27;s App Store review to block such apps.

<details><summary>References</summary>
<ul>
<li><a href="https://www.elseif.net/stories/aliexpress-runs-silent-webaudio-fingerprinting-that-breaks-bluetooth-m-4d2c69f">AliExpress silent WebAudio fingerprinting keeps Bluetooth ... — elseif</a></li>
<li><a href="https://www.drweb.de/webaudio-fingerprinting-aliexpress-bluetooth/">WebAudio - Fingerprinting : Wie erkennt AliExpress Ihr Gerät?</a></li>
<li><a href="https://news.ycombinator.com/item?id=49372583">AliExpress runs silent WebAudio fingerprinting that... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#web-audio`, `#fingerprinting`, `#privacy`, `#bluetooth`, `#aliexpress`

---

<a id="item-tech-news-3"></a>
### [Malicious arrayref Rust crate runs build-time payload](https://safedep.io/arrayref-proc-macro1-rust-build-time-malware/) ⭐️ 8.0/10

A malicious version of the widely used Rust crate arrayref executes a payload during the build process, constituting a supply-chain attack. The Rust project has published a security advisory on its official blog, and the issue is tracked in the RustSec advisory database as issue 3161. The incident has sparked community discussion about crates.io&\#x27;s incident response and the need for better build-script sandboxing. Because the malicious crate runs code at build time, crates that depend on arrayref could be compromised when building projects with the affected version.

hackernews · abhisek · Aug 20, 13:23 · [Discussion](https://news.ycombinator.com/item?id=49374269)

**「Background」** The Rust crate arrayref, a popular zero-cost macro-based utility for safely referencing array slices, was compromised in version 0.3.10 published on August 20, 2026. The malicious version added a dependency on proc-macro1, a typosquat of proc-macro2, whose build script downloads and executes a remote binary during compilation. This is a build-time supply-chain attack pattern—executing malicious code simply when a project builds—and similar poisoned crates \(internment, append-only-vec\) have also been identified.

**「Impact」** Rust developers who build projects using the affected arrayref version may execute the malicious build-time payload, potentially compromising their development environments or supply chains. Users should verify their dependency trees and watch for official patched releases or yanked versions.

**「Community discussion」** Commenters criticized crates.io&\#x27;s response, noting that the bad package version disappeared without a clear yank indication and that no advisory is listed for the crate. Others called for Cargo to sandbox build.rs scripts and contrasted the Rust ecosystem&\#x27;s dependency-heavy approach with more &quot;batteries included&quot; standard libraries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/arrayref-rust-crate-supply-chain-attack">Rust Supply-Chain Attack: arrayref, internment, and append-only-vec Poisoned by the proc-macro1 Build-Time Dropper - StepSecurity</a></li>
<li><a href="https://blog.rust-lang.org/2026/08/20/supply-chain-attack-on-arrayref/">Supply chain attack on arrayref | Rust Blog</a></li>

</ul>
</details>

**Tags**: `#supply-chain-security`, `#rust`, `#crates.io`, `#malware`, `#software-engineering`

---

<a id="item-tech-news-4"></a>
### [Terence Tao Warns AI May Trigger a Proof-Surplus Crisis](https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/) ⭐️ 8.0/10

Terence Tao, in an article written for the 2026 International Congress of Mathematicians, argues that the mathematics community should stop debating what AI can do and instead address the avoided question of research goals. He compares the current moment to the foundational crisis between 1900 and 1930 triggered by Russell&\#x27;s paradox and Gödel&\#x27;s incompleteness theorems. Tao cites the First-Proof project&\#x27;s second round, in which 10 unpublished research problems were tested by 4 AI systems and 7 were judged by at least one system as competent, at a cost of tens to hundreds of dollars per problem. He warns that mathematics may shift from proof scarcity to proof surplus, and that a proof no one can clearly explain should be considered incomplete even if it passes formal verification. The warning highlights a looming crisis in how mathematical results are verified and understood.

telegram · zaihuapd · Aug 20, 13:19

**「Background」** Terence Tao is a leading contemporary mathematician whose work includes proving conjectures such as the orchard-planting problem. His current warning compares AI&\#x27;s impact on mathematics to the foundational crisis sparked by Russell&\#x27;s paradox and Gödel&\#x27;s incompleteness theorems in the early 1900s. The First-Proof pilot he cites tested AI systems on unsolved research problems, with multiple systems judged to have produced acceptable proofs, illustrating the shift from proof scarcity to proof surplus.

**「Impact」** Mathematicians, journal referees, and AI researchers may face a wave of AI-generated proofs that are formally checkable but not human-understandable, forcing changes to verification standards, peer review, and community trust in what counts as a complete proof.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terence_Tao">Terence Tao - Wikipedia</a></li>
<li><a href="https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/">Terence Tao says AI could trigger math &#x27;s biggest crisis since Gödel</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mathematics`, `#proof verification`, `#Terence Tao`, `#research`

---

<a id="item-tech-news-5"></a>
### [On-Device Piano Autocomplete Trained Into 125M Transformer](https://simedw.com/2026/08/20/midi-autocomplete/) ⭐️ 7.0/10

A developer released a free app that runs a 125M-parameter transformer on an iPhone 15 to autocomplete piano performances, processing about 108 notes per second entirely on-device. The system works like code autocomplete: a user plays a few MIDI notes and the model continues the piece in real time. The author shared the project as a Show HN and invited questions about the model, training, and Core ML deployment. The approach demonstrates practical on-device music generation rather than a major industry breakthrough.

hackernews · simedw · Aug 20, 12:04 · [Discussion](https://news.ycombinator.com/item?id=49373456)

**「Background」** MIDI \(Musical Instrument Digital Interface\) is a protocol that encodes musical notes and performance data as digital events, allowing keyboards, computers, and software to exchange musical information. The project uses a transformer, a deep-learning architecture for sequential data, to learn from MIDI recordings and predict the next notes after a user plays a few, effectively acting as a musical autocomplete. Apple&\#x27;s Core ML framework lets the 125M-parameter model run entirely on-device on an iPhone, enabling real-time inference without a network connection.

**「Impact」** For iPhone-owning musicians, the app offers a free, real-time MIDI piano autocomplete that runs locally at about 108 notes per second on an iPhone 15.

**「Community Discussion」** Commenters connected the idea to historical classical composition training and to AI-assisted design tools, while one asked about dataset size and another found the model’s unexpected continuation of Für Elise unsettling.

**Tags**: `#on-device ML`, `#transformer`, `#Core ML`, `#music generation`, `#MIDI`

---

<a id="item-tech-news-6"></a>
### [Linux 7.2 Released with HDMI 2.1 Support for AMD Open-Source Drivers](https://www.igalia.com/2026/08/19/Linux-72-Released.html) ⭐️ 7.0/10

Linux kernel 7.2 has been announced as a minor release that adds HDMI 2.1 support to AMD&\#x27;s open-source drivers and includes Raspberry Pi updates. The release matters because it brings modern HDMI 2.1 display output to open-source AMD driver users and provides new kernel improvements for Raspberry Pi owners. The available announcement highlights these features but does not provide a full changelog or detailed compatibility information, so the exact extent of hardware support and performance changes remains unspecified.

hackernews · mariuz · Aug 20, 15:46 · [Discussion](https://news.ycombinator.com/item?id=49376265)

**「Background」** HDMI 2.1&\#x27;s higher resolutions and refresh rates rely on Fixed Rate Link \(FRL\) signaling, a feature that AMD&\#x27;s open-source AMDGPU driver historically lacked because the HDMI Forum restricted open-source implementations. The forum&\#x27;s constraints led to long-standing community frustration, but AMD eventually submitted FRL support patches for Linux 7.2, and these were successfully merged into the DRM subsystem ahead of the 7.2 merge window.

**「Community Discussion」** In the comments, one user asks how AMD&\#x27;s open-source driver now supports HDMI 2.1 given the previous HDMI Forum licensing block, while another asks what audience this kind of release note serves. Others express interest in updating a Raspberry Pi 4 and ask why HDMI would be preferred over DisplayPort, indicating a mix of curiosity and practical excitement.

<details><summary>References</summary>
<ul>
<li><a href="https://media.patentllm.org/news/hardware/amd-gpu-benchmarks-hdmi-2-1-frl-driver-and-multi-device-ai-w-20260604">AMD GPU Benchmarks, HDMI 2 . 1 FRL Driver , and... - PatentLLM Blog</a></li>
<li><a href="https://www.phoronix.com/forums/forum/phoronix/latest-phoronix-articles/1638013-amd-submits-its-long-awaited-hdmi-2-1-frl-support-for-linux-7-2-amdgpu">AMD Submits Its Long-Awaited HDMI 2 . 1 FRL Support For Linux ...</a></li>
<li><a href="https://www.linuxnews.net/articles/initial-amdgpu-hdmi-2-1-frl-support-successfully-merged-for-linux-7-2">Initial AMDGPU HDMI 2 . 1 FRL Support Successfully... - Linux News</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#Kernel`, `#Open Source`, `#HDMI`, `#Raspberry Pi`

---

<a id="item-tech-news-7"></a>
### [Spectral Neuron: New ML Primitive for Scalable, Interpretable Models](https://www.reddit.com/r/MachineLearning/comments/1vtfimo/the_spectral_neuron_an_ml_primitive_for_scalable/) ⭐️ 7.0/10

A researcher from a Yahoo ad team background has released &\#x27;The Spectral Neuron,&\#x27; a preprint and codebase proposing a new machine-learning primitive built around the model f\(x\) = λ\_k\(A0 + Σ\_i x\_i A\_i\), where λ\_k is an eigenvalue of a learned matrix pencil. The work studies how expressive such models become as the matrices grow, what information can be read directly from learned matrices, and which shapes can be guaranteed by construction. It includes a practical initialization and training recipe and reports scaling experiments on synthetic and real data. The author notes that the manuscript was AI-assisted for reference lookup, while the code was heavily AI-written and then reviewed by the author. As a preprint, it has not yet been validated by wide community adoption or independent benchmarks.

reddit · r/MachineLearning · /u/alexsht1 · Aug 20, 10:20

**「Background」** The spectral neuron is a proposed primitive that replaces typical nonlinear activations or layers with an eigenvalue operation on an affine combination of matrices: each input coordinate x\_i adds a learned matrix A\_i to a base matrix A0, and the model output is the k-th eigenvalue λ\_k of the resulting matrix. Such models are of interest because they promise scalable interpretability—learned matrices can be inspected, and structural properties can be enforced—while remaining a simple functional form.

**「Impact」** The posted preprint and GitHub repository give practitioners and researchers a ready-to-test primitive for interpretable and scalable model design, though its real-world value remains to be confirmed by independent benchmarks.

**Tags**: `#machine-learning`, `#interpretability`, `#scalability`, `#research`, `#arxiv`

---

<a id="item-tech-news-8"></a>
### [OpenAI Previews Zero Data Retention and Private Security Processing](https://openai.com/index/offering-zero-data-retention-for-frontier-models/) ⭐️ 7.0/10

OpenAI announced that eligible API customers can receive zero data retention \(ZDR\), meaning prompts and responses are not stored after request processing. It also previewed private security processing, which detects potential abuse across related interactions without exposing raw content to OpenAI personnel, and returns only limited safety signals. Customer content is encrypted with customer-controlled keys, so even flagged content cannot be read by OpenAI staff. The capabilities are being tested with early customers, with a phased rollout planned for September along with a technical whitepaper.

telegram · zaihuapd · Aug 20, 02:33

**「Background」** Zero Data Retention \(ZDR\) is a data-handling commitment under which OpenAI does not retain customers&\#x27; prompts or model responses after a request finishes processing, a policy already available to some API customers. The new preview extends this by adding &\#x27;private security processing,&\#x27; which uses agents inside the API to monitor for abuse on a per-session basis without exposing raw content to OpenAI personnel. The move responds to enterprise pressure for stronger data control and positions OpenAI against competitors such as Anthropic.

**「Impact」** Once rolled out in September, eligible API customers will be able to use frontier models for workloads requiring no retention of prompts or responses, while customer-controlled encryption prevents OpenAI from reading flagged content.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/offering-zero-data-retention-for-frontier-models/">Offering Zero Data Retention for frontier models | OpenAI</a></li>
<li><a href="https://www.business-standard.com/technology/artificial-intelligence/openai-data-privacy-ai-safety-enterprise-api-126082000704_1.html">AI firms sharpen privacy pitch as enterprises demand control over data</a></li>
<li><a href="https://techcrunch.com/2026/08/19/openai-seeks-to-one-up-anthropic-with-new-customer-privacy-protections/">OpenAI seeks to one-up Anthropic with new customer privacy ...</a></li>

</ul>
</details>

**Tags**: `#openai`, `#privacy`, `#security`, `#api`, `#data-retention`

---

<a id="item-tech-news-9"></a>
### [Reverse Image Service Breach Exposes Millions of Face Photos](https://arstechnica.com/gadgets/2026/08/reverse-lookup-service-exposed-millions-of-photos-of-peoples-faces/) ⭐️ 7.0/10

A reverse image search service suffered a data breach that exposed millions of facial photos and associated personal information. The leaked database is about 450 GB and contains over 9 million images, with some records including email addresses, phone numbers, and IP addresses. Because facial images are hard-to-replace biometric data, privacy and identity security concerns have been raised. Experts warn the exposed data could be used for unauthorized identification, personal tracking, or fraud. The service has restricted access to the database, but the full scope of the incident and remediation steps remain unconfirmed, according to Ars Technica.

telegram · zaihuapd · Aug 20, 15:14

**「Background」** Reverse image search services let users upload a photo to find matching images online, often relying on large databases of scraped or user-submitted images. When such a database is compromised, the exposed biometric and contact data becomes especially sensitive because faces cannot be easily changed like passwords or credit card numbers.

**「Impact」** Users whose facial images and contact details were stored by the affected service face heightened risks of unauthorized identity matching, tracking, and targeted fraud, though the precise number of affected individuals and actual misuse have not yet been confirmed.

**Tags**: `#data-breach`, `#privacy`, `#biometrics`, `#security`, `#reverse-image-search`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Evergrande Founder Xu Jiayin Sentenced to Life; Company Fined Billions](https://www.news.cn/legal/20260820/737dfb54ab564fb8a549ba392af9fb0a/c.html) ⭐️ 9.0/10

In a first-instance verdict, the Shenzhen Intermediate People&\#x27;s Court sentenced Evergrande founder Xu Jiayin to life imprisonment, deprived him of political rights for life, and ordered confiscation of all his personal property. The court also fined Evergrande Group 8.82 billion yuan and Evergrande Property 7 billion yuan after finding financial fraud, illegal deposit-taking, fundraising fraud, and fraudulent securities issuance between 2016 and 2021.

telegram · zaihuapd · Aug 20, 04:06

**「Background」** Evergrande, once one of China&\#x27;s largest property developers, defaulted on its debts in late 2021 and was later ordered into liquidation. In the trial, the court found that from 2016 to 2021, Evergrande Group, Evergrande Real Estate and Xu used sustained large-scale financial fraud to raise funds illegally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/legal/20260820/737dfb54ab564fb8a549ba392af9fb0a/c.html">恒大集团、恒大地产、许家印等案一审宣判-新华网</a></li>

</ul>
</details>

**Tags**: `#Evergrande`, `#securities fraud`, `#regulatory enforcement`, `#China real estate`, `#capital markets`

---

<a id="item-finance-news-2"></a>
### [Fed holds interest rates steady after Iran war spikes oil prices](https://news.google.com/rss/articles/CBMilAFBVV95cUxOWVgwU0l2bjYwREJ2NE9WVC1ObnpJa3Qxa2syS0lmUXphVm8zTWpnYVJ5NXpFZmxWYUZlVXpmc3ZFQzk2ZnZlYjNSUHRPb3F1emZhVDdPNEMxak1mM2wzOEZtYnA5dklfUFlfOUdVRU5lSXNmTlhqMy1pUElaMjNBTEFJbV9IRHNkRGt1NHJKVDVFd1Za0gGaAUFVX3lxTE9IOWFDX2MzMVhjUXl2VE1oTGNTTlowMmxkMUZnNEQ1TzhKemJ3TmlSTElmdzVPQ3VmR2E3OGdNLXN2dVBHQ2xiLXl0WWJfdjBUQktuSnNwbTNQV3puQzBJTUVZS295S2lHYU9iQVpFd05FQkw4WmhmZ2EyU3dCUWt0bHNCUy1xX0pHME5ZbVBlZ1RXSkxnSVZ1TWc?oc=5) ⭐️ 9.0/10

The Federal Reserve left interest rates unchanged at its first policy meeting since the Iran war pushed oil prices higher.

google\_news · ABC News - Breaking News, Latest News and Videos · Aug 19, 15:26

**「Background」** The Federal Reserve left its main interest rate unchanged on Wednesday, July 29, after a war with Iran pushed oil prices higher and raised inflation. The central bank said it was waiting for more data because of &\#x27;elevated uncertainty&\#x27; and conflicting economic signals.

**「Impact」** Households and businesses could face higher energy costs as oil prices near $95 a barrel and Iran threatens to keep the Strait of Hormuz closed, while the Fed&\#x27;s rate hold leaves borrowing costs unchanged.

<details><summary>References</summary>
<ul>
<li><a href="https://myv101.iheart.com/content/2026-07-29-fed-holds-interest-rates-steady-amid-inflation-from-iran-conflict/">Fed Holds Interest Rates Steady Amid Inflation From Iran Conflict</a></li>
<li><a href="https://www.aol.com/articles/federal-holds-interest-rates-steady-180125953.html">Federal Reserve holds interest rates steady amid Iran war ... - AOL</a></li>
<li><a href="https://www.2asy.ai/2026-05-02-macro/">Iran War Drives Oil Surge 57% | Daily market brief for May 02, 2026</a></li>
<li><a href="https://www.aljazeera.com/tag/israel-iran-conflict/">US-Israel war on Iran | US-Israel war... | Today&#x27;s latest from Al Jazeera</a></li>
<li><a href="https://qz.com/oil-prices-iran-strikes-rubio-hormuz-072226">Oil prices near $95 as U.S. strikes Iran for 11th straight night</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#oil prices`, `#Iran conflict`

---

<a id="item-finance-news-3"></a>
### [Fed Faces One of Its Most Unpredictable Meetings in Years](https://news.google.com/rss/articles/CBMiwgFBVV95cUxNVGNvM0dQRTJ5MVh3MVN0RHV0R2k5bTVvSUZNeVFDa192eW9WUUZqekhHMzFVQlZ0eXB4ZGdiNU5vRFQ4QmJsZXpBa25ja18xVUxib0Ryb0Nwc29PMnh5V2l6ekluU2xSYmJia1h5NVpIMHZ6WXltTlVXb2ZTWGl3MjR3d2FxUnh5WVRvZk02WUlRZWcxOW1WVWMwd0lpYkcyMmYxYjF6aTFTRXRQaTN3WEI4Rk5UV0I3V1V2c29WZ0ZNZw?oc=5) ⭐️ 9.0/10

The Wall Street Journal reports that the Federal Reserve&\#x27;s next policy meeting is expected to be one of the most unpredictable in years.

google\_news · WSJ · Jul 23, 07:00

**「Background」** The Federal Reserve is widely expected to reduce interest rates at its upcoming meeting, but officials face mixed economic signals, making the exact scope and path of policy changes unusually uncertain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thestreet.com/markets/heres-how-stocks-react-to-fed-interest-rate-cuts">The Federal Reserve is expected to reduce interest rates Wednesday.</a></li>
<li><a href="https://abcstlouis.com/news/economy-bringing-mixed-messages-ahead-of-next-federal-reserve-meeting-policy-stock-market-artificial-intelligence">Economy bringing mixed messages ahead of next federal reserve ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#central bank`, `#markets`

---

<a id="item-finance-news-4"></a>
### [Federal Reserve Holds Interest Rates Steady, Leaves Door Open to Hike](https://news.google.com/rss/articles/CBMihgFBVV95cUxPeWNzVUdhUF9wNFBtSC00WUwwbE5jUEp4WEExREd2cWZoZ21YNkNSTHJ6OGdfMjgwcjN3MXU2S1FDalNjTmpLVXRZNlBGRkphM203c1pENl9hMXdkRkFlc2hnSlJ0bFYxSk5vRVJoNGJzMmtyU2Z6VzhLNXgweV83eGNpYmlBQQ?oc=5) ⭐️ 9.0/10

The Federal Reserve left its benchmark interest rate unchanged but signaled that another increase is still possible.

google\_news · CBS News · Jun 17, 07:00

**「Background」** The Federal Reserve has held its benchmark interest rate unchanged in recent meetings despite resurgent inflation, with its rate-setting committee voting 9 to 3 in July to keep the target range at 3.50%-3.75%. Policymakers remain divided, with nearly half indicating they would support a rate hike later this year if inflation stays elevated.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/fed-meeting-fomc-today-kevin-warsh-interest-rates/">Federal Reserve holds interest rates steady but leaves door open to hike - CBS News</a></li>
<li><a href="https://www.npr.org/2026/07/29/nx-s1-5910558/federal-reserve-interest-rates-inflation">A divided Federal Reserve holds interest rates steady despite high inflation</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Federal Reserve Holds Rates at 3.50%-3.75% in July 2026 | U.S. Bank</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#economy`, `#central bank`

---

<a id="item-finance-news-5"></a>
### [Bank of England Releases July 2026 Monetary Policy Report](https://news.google.com/rss/articles/CBMieEFVX3lxTFBpZV92WU9JUmd5cW1obnRVaGVHRFB3V2o3WktuUy1aRTM4V2RmQktOaDh4aWF0ampYb1lUQlJGaHZROTIzOXVzVDNJSUNpQW9wcldGeVFZQXBsQ3ZpOFZJdlRMZEQ2eUxhSFZadDk3cmdBNmhzMTY1TA?oc=5) ⭐️ 9.0/10

The Bank of England published its July 2026 Monetary Policy Report, outlining the central bank’s latest monetary policy stance and economic outlook for the UK. No specific policy decisions or forecasts were detailed in the announcement itself.

google\_news · Bank of England · Jul 30, 07:00

**「Background」** The Bank of England publishes this quarterly Monetary Policy Report to explain the economic analysis and inflation projections behind the Monetary Policy Committee&\#x27;s \(MPC\) interest rate decisions. In the July 2026 edition, the MPC voted 6-3 to keep Bank Rate at 3.75%, with three members preferring a 0.25 percentage point increase.

**「Impact on borrowers」** With Bank Rate maintained at 3.75%, households and businesses with variable-rate mortgages or loans will keep the same borrowing costs for now, meaning no immediate rise in monthly payments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bankofengland.co.uk/monetary-policy-report/2026/july-2026">Monetary Policy Report - July 2026 - Bank of England</a></li>
<li><a href="https://ebs.publicnow.com/view/198796721B585C9D486667FACA58C1FE32D96706">Bank of England (via Public) / Monetary Policy Report - July 2026</a></li>
<li><a href="https://www.bankofengland.co.uk/">Home | Bank of England</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#Bank of England`, `#interest rates`, `#UK economy`, `#inflation`

---

<a id="item-finance-news-6"></a>
### [Houthis Plan to Seize Land Around Bab el-Mandeb Oil Chokepoint](https://oilprice.com/Geopolitics/Middle-East/Houthis-Move-to-Gain-Complete-Control-Over-Crucial-Bab-el-Mandeb-Oil-Chokepoint.html) ⭐️ 8.0/10

Yemen’s Houthi group is planning to seize land and islands around the Bab el-Mandeb Strait to tighten its control of the oil chokepoint, Yemen’s information minister said, citing Houthi sources. The group says it has carried out 31 attacks on Saudi targets, including eight tankers, and shippers are again avoiding the strait.

rss · OilPrice.com · Aug 20, 23:00

**「Background」** Bab el-Mandeb is a narrow Red Sea chokepoint between Yemen and Djibouti that oil tankers use to reach the Suez Canal. The Houthis, who control parts of Yemen and have ties to Iran, already disrupted Red Sea shipping during the Gaza war and this year announced a blockade on Saudi vessels after Iran shut the Strait of Hormuz in March.

**「Impact」** The attacks have forced Saudi Arabia to reroute some crude exports from Yanbu to Egypt’s Sidi Kerir terminal and prompted the closure of the Jazan refinery after three strikes, adding time and costs to oil shipments.

**Tags**: `#Houthis`, `#Bab el-Mandeb`, `#Oil Trade`, `#Geopolitics`, `#Shipping`

---

<a id="item-finance-news-7"></a>
### [EPA Allows Early Switch to Winter-Grade Gasoline](https://oilprice.com/Latest-Energy-News/World-News/Washington-Eases-Gasoline-Rules-as-Iran-Pressure-Campaign-Jolts-Fuel-Costs.html) ⭐️ 8.0/10

The U.S. Environmental Protection Agency authorized an early switch to cheaper winter-grade gasoline starting September 1, a change the administration says could add hundreds of thousands of barrels per day to domestic supply as average U.S. gasoline prices remain above $4 a gallon.

rss · OilPrice.com · Aug 20, 21:30

**「Background」** The waiver, which lets fuel with 10% ethanol be sold before the normal mid-September seasonal transition, came the same day Treasury Secretary Scott Bessent promised the &\#x27;toughest sanctions in history&\#x27; against Iran. The Energy Department already expects elevated fuel prices to persist through year-end.

**「Impact」** The change may provide some relief at the pump for American drivers, although state-level fuel rules could limit how quickly additional supply reaches some markets.

**Tags**: `#gasoline prices`, `#EPA waiver`, `#Iran sanctions`, `#fuel supply`, `#energy policy`

---

<a id="item-finance-news-8"></a>
### [China Steps Up Domestic Oil and Gas Output to Bolster Energy Security](https://oilprice.com/Energy/Energy-General/Beijing-Bets-on-Fossil-Fuels-Even-as-It-Leads-the-World-in-Renewables.html) ⭐️ 8.0/10

China is expanding domestic oil and gas production while continuing its renewables build-out, targeting 440 million metric tonnes of oil equivalent by 2030 under the 15th Five-Year Plan. In 2025, crude output hit a record 216 million metric tonnes, according to the National Energy Administration.

rss · OilPrice.com · Aug 20, 15:00

**「Background」** China has been raising fossil fuel production to reduce import dependence, a policy that has already cut its crude imports from the Middle East from 55.4% to 44.6% between the first half of 2025 and the same period in 2026, according to S&amp;P Global.

**「Impact」** The strategy has already reduced import reliance; oil imports fell to 7.8 million barrels per day in May, the lowest since 2017.

**Tags**: `#China energy policy`, `#oil production`, `#energy security`, `#fossil fuels`, `#global energy markets`

---

<a id="item-finance-news-9"></a>
### [Alibaba Fiscal Q1 Net Profit Falls 76% to 10.54 Billion Yuan](https://www.alibabagroup.com/en-US/document-2026456290057781248) ⭐️ 8.0/10

Alibaba reported net profit attributable to shareholders of 10.537 billion yuan for the first quarter of fiscal 2027, down 76% year over year. This is the company’s reported result, not an analyst estimate or forecast.

telegram · zaihuapd · Aug 20, 12:08

**「Background」** The decline follows Alibaba&\#x27;s heavy spending on AI infrastructure; its capital expenditure reached 126.06 billion yuan in fiscal 2026, up 46.6% year over year, while AI-related revenue rose 45% in the latest quarter.

<details><summary>References</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/3944384950408836">Alibaba ’s &quot;Mega Ecosystem&quot; Boom Recedes: AI Emerges as Its Sole...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/alibaba-quarterly-profit-drops-75-150542410.html">Alibaba quarterly profit drops 75% as AI investment spending grows</a></li>

</ul>
</details>

**Tags**: `#Alibaba`, `#earnings`, `#net profit`, `#Chinese tech`, `#fiscal Q1`

---

<a id="item-finance-news-10"></a>
### [AMD Slips as Google Expands $120 Billion Custom-Chip Push](https://finance.yahoo.com/technology/articles/amd-falls-google-expands-120-192101116.html) ⭐️ 8.0/10

AMD shares fell after Google expanded its $120 billion custom-chip initiative, intensifying competition in the semiconductor market.

openbb · NVDA · Aug 20, 19:21

**「Background」** Google&\#x27;s custom-chip push includes its tensor processing units \(TPUs\), in-house AI chips that have gained demand as companies seek cheaper alternatives to expensive processors from Nvidia and AMD.

<details><summary>References</summary>
<ul>
<li><a href="https://www.channelnewsasia.com/business/marvell-gives-google-option-buy-122-billion-stake-in-custom-ai-chip-deal-6328781">Marvell gives Google option to buy $12.2 billion stake in custom AI...</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#Google`, `#custom chips`, `#semiconductor industry`, `#competition`

---

<a id="item-finance-news-11"></a>
### [Broadcom seeks over $60 billion in AI debt financing, Bloomberg reports](https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-203818587.html) ⭐️ 8.0/10

Bloomberg News reports that Broadcom is seeking more than $60 billion in debt financing for AI-related investments, though the deal has not been confirmed by the company.

openbb · NVDA · Aug 20, 20:38

**「Background」** Broadcom’s new financing talks follow a $35 billion debt package arranged in June by Apollo and Blackstone for its AI XPV Platform, which funds more than 1 gigawatt of compute for Anthropic.

**「Impact」** The reported borrowing—which could scale to $100 billion—would fund AI chip and infrastructure projects that benefit Anthropic and other companies, and a deal of this size could also affect appetite in corporate debt markets.

<details><summary>References</summary>
<ul>
<li><a href="https://247wallst.com/investing/2026/08/14/broadcom-sinks-6-as-bofa-flags-370b-in-ai-debt-amd-climbs-4-on-bairds-1250-call/">Broadcom Sinks 6% as BofA Flags $370B in AI Debt ... - 24/7 Wall St.</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">AI Infrastructure Boom Drives Broadcom ’s $ 60 Billion Debt ...</a></li>
<li><a href="https://www.newsmax.com/finance/streettalk/broadcom-60-billion-dollars-ai/2026/08/20/id/1266812/">Broadcom Seeks $ 60 Billion in Latest AI Debt Deal | Newsmax.com</a></li>
<li><a href="https://cryptobriefing.com/broadcom-60b-debt-ai-chip-financing/">Broadcom seeks over $ 60 B in debt for AI chip financing deal</a></li>

</ul>
</details>

**Tags**: `#Broadcom`, `#AI`, `#debt financing`, `#capital markets`, `#semiconductors`

---

<a id="item-finance-news-12"></a>
### [Broadcom Reportedly Seeks Over $60 Billion for AI Debt Deal](https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-201702584.html) ⭐️ 8.0/10

Broadcom is reportedly seeking more than $60 billion in debt financing tied to artificial intelligence, according to media reports. The financing would be among the largest AI-related debt raises, but the figure is a reported target rather than a confirmed deal.

openbb · NVDA · Aug 20, 20:17

**「Background」** Broadcom is in talks with a group of lenders to raise more than $60 billion in debt for an AI chip financing deal that will benefit Anthropic and other companies, according to Bloomberg News, which cited unnamed people familiar with the matter.

**「Impact」** The $60 billion-plus debt financing is intended to fund an AI chip vehicle that will benefit Anthropic and other companies, with lenders providing the capital.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">Broadcom Seeks More Than $60 Billion in Latest AI Debt Deal</a></li>
<li><a href="https://kfgo.com/2026/08/20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal-bloomberg-news-reports/">Broadcom seeks more than $60 billion in latest AI debt deal, Bloomberg News reports | The Mighty 790 KFGO | KFGO</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/broadcom-seeks-more-60-billion-203818587.html">Broadcom seeks more than $60 billion in latest AI debt deal, Bloomberg News reports</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-20/broadcom-seeks-more-than-60-billion-in-latest-ai-debt-deal">AI Infrastructure Boom Drives Broadcom ’s $ 60 Billion Debt Financing...</a></li>
<li><a href="https://cryptobriefing.com/broadcom-60b-debt-ai-chip-financing/">Broadcom seeks over $ 60 B in debt for AI chip financing deal</a></li>

</ul>
</details>

**Tags**: `#Broadcom`, `#debt financing`, `#artificial intelligence`, `#capital markets`, `#corporate finance`

---

<a id="item-finance-news-13"></a>
### [ASML Gains as TSMC Raises Spending Forecast to $85 Billion](https://finance.yahoo.com/technology/articles/asml-gains-tsmcs-spending-forecast-190758887.html) ⭐️ 8.0/10

ASML shares rose after TSMC raised its capital spending forecast to $85 billion, signaling strong expected demand for advanced chipmaking equipment. The $85 billion is a forecast for future spending, not reported expenditure.

openbb · NVDA · Aug 20, 19:07

**「Background」** ASML is the world&\#x27;s largest supplier of semiconductor manufacturing equipment, and chipmakers&\#x27; capital spending forecasts are a key indicator of demand for its machines.

**「Impact」** TSMC is a major buyer of ASML&\#x27;s chipmaking equipment, so the higher spending plan points to continued demand for ASML systems used in advanced chip production.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investing.com/news/stock-market-news/strong-asml-tsmc-forecasts-signal-ai-spending-boom-is-intact-4617583">Strong ASML, TSMC forecasts signal AI spending boom is intact By Reuters</a></li>

</ul>
</details>

**Tags**: `#ASML`, `#TSMC`, `#semiconductor equipment`, `#capital expenditure`, `#market reaction`

---

<a id="item-finance-news-14"></a>
### [TSMC&\#x27;s 2027 Capex Forecast Reaches $85 Billion](https://finance.yahoo.com/technology/articles/tsmc-rises-2027-capex-forecast-192841498.html) ⭐️ 8.0/10

TSMC&\#x27;s stock rose after the company&\#x27;s capital expenditure forecast for 2027 reached $85 billion, signaling a major planned expansion of semiconductor manufacturing capacity.

openbb · NVDA · Aug 20, 19:28

**「Background」** TSMC, the world&\#x27;s largest contract chipmaker, had guided for 2026 capital expenditures of about $52–56 billion, with spending expected toward the upper end of that range. The reported 2027 forecast of as much as $85 billion would mark a substantial step up in planned spending on advanced chipmaking capacity.

**「Impact」** The planned spending signals a major increase in advanced chip capacity, a key input for AI infrastructure and global semiconductor supply chains.

<details><summary>References</summary>
<ul>
<li><a href="https://sg.finance.yahoo.com/news/tsmc-rises-2027-capex-forecast-192841498.html">TSMC Rises as 2027 Capex Forecast Reaches $85 Billion</a></li>
<li><a href="https://semiwiki.com/semiconductor-manufacturers/tsmc/371192-tsmcs-raises-the-bar-on-capex/">TSMC’s Raises the Bar on CAPEX! - Semiwiki</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#Semiconductors`, `#Capital Expenditure`, `#AI Infrastructure`, `#Supply Chain`

---

<a id="item-finance-news-15"></a>
### [Stripe agrees to acquire AI model gateway OpenRouter](https://stripe.com/en-jp/newsroom/news/stripe-agrees-to-acquire-openrouter) ⭐️ 7.0/10

Stripe announced on August 19, 2026 that it has agreed to acquire OpenRouter, an AI model gateway that routes requests across more than 400 models from over 80 providers based on task complexity, price, speed, and reliability to help businesses optimize token usage. Financial terms were not disclosed.

telegram · zaihuapd · Aug 20, 07:00

**「Background」** OpenRouter is an AI model gateway and routing platform that helps developers choose among 400+ models from 80+ providers based on cost, speed, and reliability. Bloomberg reported the deal could be worth more than $7 billion in cash and stock, though the companies have not publicly confirmed a final price.

<details><summary>References</summary>
<ul>
<li><a href="https://www.orcarouter.ai/blog/stripe-acquires-openrouter">Stripe OpenRouter Acquisition : $7B, What Changes for Devs</a></li>

</ul>
</details>

**Tags**: `#Stripe`, `#OpenRouter`, `#Acquisition`, `#AI Infrastructure`, `#M&amp;A`

---