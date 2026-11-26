---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 35 items, 11 important content pieces were selected

---

**Technology News**
1. [1Password Discloses November 2026 Security Incident](#item-tech-news-1) ⭐️ 8.0/10
2. [Shorter Lean Formalization of GRH Verification Released](#item-tech-news-2) ⭐️ 8.0/10
3. [Minecraft Java Edition RCE Flaw Affects Versions 1.20.5 and Later](#item-tech-news-3) ⭐️ 8.0/10
4. [HN reacts to Aaronson post on 9/4 matrix multiplication exponent](#item-tech-news-4) ⭐️ 7.0/10
5. [SemiAnalysis Launches GDPx Benchmark, Reports Opus 5.5 at 12%](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI Bets on Cybersecurity as Next Growth Engine](#item-tech-news-6) ⭐️ 7.0/10
7. [Tencent open-sources GGUF quantized weights for 224B Hy4 flash](#item-tech-news-7) ⭐️ 7.0/10
8. [Samsung and SK Hynix reportedly to license YMTC Xtacking NAND tech](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Report: US Commerce Department pressured Intel to hand over 10% stake](#item-finance-news-1) ⭐️ 8.0/10
2. [美国拟对14个贸易伙伴加征新关税](#item-finance-news-2) ⭐️ 8.0/10
3. [Nvidia Swings Test Fed Chair Warsh&\#x27;s Market-Signal Approach](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [1Password Discloses November 2026 Security Incident](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password published an update on a November 2026 security incident, according to its blog post and the accompanying Hacker News discussion. The available material does not include the vendor&\#x27;s own text, so the specific scope, affected systems, and confirmed data exposure cannot be verified here. Commenters describe the pattern as an attacker pushing malicious code to backend services, and one user reports receiving a phishing email referencing a shared vault link shortly after the disclosure. Treat the incident details as a vendor statement pending the full write-up rather than an independently confirmed finding.

hackernews · lxhrstn · Nov 25, 17:18 · [Discussion](https://news.ycombinator.com/item?id=50644817)

**「Background」** 1Password has faced earlier credential-related pressure: Horizon&\#x27;s October 2023 coverage noted that after the Okta breach, attackers tried to compromise 1Password and Cloudflare using stolen data, and both companies said they detected the intrusion before Okta alerted them. The current November 2026 update concerns a different vector—malicious code pushed to backend services—which commenters connect to the broader SaaS pattern of employee-laptop compromise leading to code deployment.

**「Impact」** Users should treat any unsolicited 1Password-branded message about shared vault items or links as suspect: one commenter reported a phishing email that included personal details and a fake shared-vault notification dated November 26, 2026. Commenters also pressed for clarity on whether branch protection or push restrictions on backend code were in place, since that determines how far a compromised employee laptop could reach.

**「Community Discussion」** Commenters argued that compromise of an employee laptop leading to code pushed to production is the standard SaaS breach pattern, with tptacek calling it the single most important attack vector for SaaS companies. ctidd said the announcement did not sufficiently address whether push to main was restricted or branch protection bypassed, while ChrisHardie, a longtime user with a local-only vault, questioned whether online vault architecture can fully mitigate that risk.

<details><summary>References</summary>
<ul>
<li>Okta breach: Hackers attempt to compromise 1Password and Cloudflare using stolen data</li>

</ul>
</details>

**Tags**: `#security`, `#password-managers`, `#supply-chain`, `#phishing`, `#saas`

---

<a id="item-tech-news-2"></a>
### [Shorter Lean Formalization of GRH Verification Released](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

A GitHub repository by lsernau presents a much shorter Lean formalization of the GRH verification, which commenters describe as reducing the proof from roughly 17 million lines to about 76,000 lines, a 99.56% reduction. Commenters say the more readable version separates &quot;known math&quot; from &quot;new math&quot; and includes human-readable documentation throughout. These figures and characterizations come from community comments rather than the item itself, and the repository&\#x27;s correctness and completeness have not been independently confirmed here.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**「Background」** The repository relates to a claimed proof of the Generalized Riemann Hypothesis attributed to Anthropic mathematician Levent Alpöge and Claude, which was distributed as a large Lean archive of roughly 175,000 source files and about 239MB of data. Reporting on that claim noted it had not been independently verified by experts. The new repository presents a much shorter Lean formalization of the same verification effort, which commenters describe as reducing the code from about 17 million lines to roughly 76,000.

**「Impact」** For readers trying to assess the GRH formalization, the practical consequence is that the shorter proof&\#x27;s readability and documented &quot;known math&quot; versus &quot;new math&quot; split make it easier to audit and digest than the multi-million-line version, according to commenters. However, the reduction figures \(~17M to ~76k lines\) and the claim of a 300kloc readable proof come from community comments rather than an independently verified source, so the correctness and mathematical significance of the shorter formalization remain unconfirmed.

**「Community Discussion」** Commenters praised the shorter proof&\#x27;s readability and documentation, with one saying it should greatly aid digesting the result. Others questioned whether the formalization offers genuine mathematical insight: one asked whether it undercuts a recent point by Terence Tao that huge proofs without insight are a problem, and another said they would like to see an actual mathematical paper explaining the core argument, presented by someone who understands it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/anthropic-167-year-old-riemann-hypothesis-claude">Claude helped prove 167-year-old Riemann hypothesis , researcher...</a></li>
<li><a href="https://www.nacionale.com/en/articles/has-riemann-hypothesis-been-proved-levent-alpoge-claude-anthropic-claim-lean">Riemann hypothesis proof claimed with Claude, unverified</a></li>

</ul>
</details>

**Tags**: `#formal-verification`, `#Lean`, `#mathematics`, `#AI-assisted-proofs`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Minecraft Java Edition RCE Flaw Affects Versions 1.20.5 and Later](https://github.com/bikini/minecraft2shell) ⭐️ 8.0/10

A publicly disclosed vulnerability, minecraft2shell, published on November 22, shows that a crafted TrueType font in a server resource pack can trigger a native out-of-bounds write in FreeType 2.14.3 and earlier, leading to arbitrary code execution on Windows clients running Minecraft Java Edition 26.3. Affected versions are reported as 1.20.5 through 1.21.10 and snapshots 26.1 through 26.4, while 1.20.4 and earlier and Bedrock Edition are said to be unaffected. Mojang still ships lwjgl-freetype 3.4.3 and has no official patch, according to the report. A community fix, m2sfix 1.0.0, released November 24, disables hinting via a Java agent or mod.

telegram · zaihuapd · Nov 25, 12:46

**「Background」** The flaw sits in FreeType, the font-rendering library Minecraft&\#x27;s Java client uses through lwjgl-freetype 3.4.3, which the source says Mojang has not yet updated. FreeType has a track record of memory-safety bugs in its TrueType parsing paths, including a TrueType bytecode interpreter issue reported to the oss-security list and a 2025 CVE patched in downstream distributions, so font files are a known attack surface rather than a novel one.

**「Impact」** Until an official patch exists, the submitter advises players not to add resource packs and to set multiplayer server resource pack permissions to &quot;disabled,&quot; or to install the community m2sfix mod. Server operators and players on affected Java versions should treat untrusted resource packs as a code-execution risk.

<details><summary>References</summary>
<ul>
<li>oss-security - Project Zero discloses 4 bugs in FreeType - Openwall</li>
<li>[kirkstone][PATCH] freetype: patch CVE-2025-27363 - main@lists.openembedded.org | Home</li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#minecraft`, `#freetype`, `#remote-code-execution`

---

<a id="item-tech-news-4"></a>
### [HN reacts to Aaronson post on 9/4 matrix multiplication exponent](https://scottaaronson.blog/?p=10379) ⭐️ 7.0/10

A Hacker News thread with roughly 953 comments reacts to a Scott Aaronson blog post that appears to concern a major mathematics result, which the discussion links to a paper titled &quot;The matrix multiplication exponent is nine fourths.&quot; The supplied material is a pointer plus community comments, not the paper itself, so the claimed exponent of 9/4 and any proof details are unverified here. Commenters debate what such a result would mean for AI and scientific progress rather than the mathematics itself.

hackernews · Kotlopou · Nov 25, 19:11 · [Discussion](https://news.ycombinator.com/item?id=50646108)

**「Background」** The discussion follows an OpenAI paper dated November 24, 2026, which claims the matrix multiplication exponent is exactly 9/4, with matching upper and lower bounds and a Lean development proving the result for division-free circuits over every field. The matrix multiplication exponent, conventionally denoted omega, describes the asymptotic cost of multiplying large matrices; a smaller exponent implies faster algorithms for a problem underlying much of scientific computing and machine learning. The Hacker News thread also links a separate PDF titled &quot;The matrix multiplication exponent is nine fourths.&quot;

**「Why it matters」** If the 9/4 exponent claim holds, it would bear on the asymptotic cost of matrix multiplication, a core primitive in numerical computing and machine learning. Readers should treat the figure as an unconfirmed claim from a linked paper until the proof is checked, since the supplied source does not present the argument.

**「Community debate」** Commenters split on implications: jsLavaGoat argues that AI strength in axiomatic math does not imply it will &quot;solve&quot; other fields or play a destructive sci-fi role, while Nevermark contends humans systematically underestimate the scale of change. utopiah asks whether the result would have arrived with Lean, MathLib, and compute alone, without LLMs, and sunir invokes Latour&\#x27;s &quot;centers of calculation&quot; to frame the moment.

<details><summary>References</summary>
<ul>
<li><a href="https://interestingengineering.com/culture/openai-exact-2-25-matrix-multiplication-exponent">OpenAI establishes exact 2.25 exponent for matrix multiplication</a></li>
<li><a href="https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/README.md">math/preprints/The- matrix - multiplication - exponent -is...</a></li>
<li><a href="https://www.alphaxiv.org/abs/2611.matrix-multiplication-exponent-lower-bound">The Matrix Multiplication Exponent Is Nine Fourths | alphaXiv</a></li>

</ul>
</details>

**Tags**: `#algorithms`, `#matrix-multiplication`, `#complexity-theory`, `#AI`, `#research`

---

<a id="item-tech-news-5"></a>
### [SemiAnalysis Launches GDPx Benchmark, Reports Opus 5.5 at 12%](https://newsletter.semianalysis.com/p/evaluating-recent-model-releases) ⭐️ 7.0/10

SemiAnalysis released GDPx, a benchmark covering 11 domains it considers most valuable for frontier intelligence — including chip design, cybersecurity, biology, finance, legal, quant trading, recursive self-improvement, hardware design, materials science, alignment, and software engineering — built from 206 tasks made with 14 specialized data partners. The firm argues that comprehensive benchmarks like GDPVal and Agent&\#x27;s Last Exam err by selecting domains via share of GDP or the O\*NET taxonomy, since AI&\#x27;s impact is unevenly distributed across the economy. On release day, Opus 5.5 was the highest-scoring model at just 12%, which SemiAnalysis presents as evidence the benchmark has headroom to discriminate between future releases, unlike saturated benchmarks such as Terminal Bench 4.0. The post also says safety classifiers depressed overall scores for models including Fable 5.2 and GPT-6.2 Astra, and that excluding cyber, biology, and alignment while switching legal and finance to partial grading produces a different leaderboard; the excerpt is truncated before those results are shown.

rss · Semianalysis · Nov 26, 00:05

**「Background」** SemiAnalysis launched GDPx earlier in November 2026, describing it as a benchmark for general agentic capability across 11 economically valuable domains, built with domain-specialist partners and published with a live leaderboard and per-domain results. The current article evaluates model releases since that launch, so its leaderboard figures reflect the benchmark&\#x27;s first weeks of operation rather than a long-tracked record.

**「Impact」** Practitioners comparing frontier models should note that GDPx scores are not directly comparable across the two leaderboards SemiAnalysis describes: the adjusted view drops three domains and changes legal and finance from binary to partial grading, so a model&\#x27;s ranking can shift with the scoring method rather than capability alone. The 12% top score also means small absolute differences at the low end may carry more noise than the headline percentages suggest.

<details><summary>References</summary>
<ul>
<li><a href="https://gdpx.semianalysis.com/">gdpx.semianalysis.com - GDPx: The General Agentic Benchmark</a></li>
<li><a href="https://newsletter.semianalysis.com/p/gdpx-measuring-frontier-model-capabilities">GDPx: Measuring Frontier Model Capabilities Across the Most ...</a></li>

</ul>
</details>

**Tags**: `#AI benchmarks`, `#model evaluation`, `#frontier models`, `#AI economics`

---

<a id="item-tech-news-6"></a>
### [OpenAI Bets on Cybersecurity as Next Growth Engine](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 7.0/10

OpenAI is positioning cybersecurity as a potential growth engine larger than its coding business, according to a Telegram summary of a paywalled The Information report. CFO Sarah Friar said external estimates putting the cybersecurity market above $300 billion are still far too low, and President Greg Brockman said cybersecurity will become a bigger business segment for OpenAI than coding. The company has released GPT-6 Cyber for security research and is expanding its Daybreak trusted-access program, which as of September covered thousands of verified defenders and about 2,000 approved organizations and workspaces, supporting vulnerability discovery, codebase analysis, and binary reverse engineering. The report says competition with Anthropic and Google and the prospects for scaled commercialization remain unclear, and the market-size and business-size claims are company projections rather than verified results.

telegram · zaihuapd · Nov 25, 04:51

**「Background」** OpenAI&\#x27;s cybersecurity push builds on its Daybreak trusted-access program, which earlier releases expanded with security-focused models. Web results describe a June 2026 release of GPT-5.5-Cyber alongside Codex Security updates and Patch the Planet, and a November 2026 launch of GPT-6 Cyber limited to Daybreak Red customers, with claims of 81 new Firefox vulnerabilities and exploits for 948 Linux kernel bugs. The current report frames GPT-6 Cyber and Daybreak&\#x27;s growth to roughly 2,000 approved organizations as the base for OpenAI&\#x27;s claim that cybersecurity could outgrow its coding business.

**「Impact」** Security teams evaluating AI-assisted vulnerability discovery and binary reverse engineering now have a named OpenAI offering, GPT-6 Cyber, but access runs through the gated Daybreak program rather than open availability, so organizations outside the roughly 2,000 approved workspaces cannot yet use it. The report does not detail pricing, general-availability timing, or how Daybreak eligibility is determined.

<details><summary>References</summary>
<ul>
<li>OpenAI Expands Daybreak With GPT-5.5-Cyber to Help Defenders Patch Security Flaws</li>
<li>OpenAI launches GPT-6 Cyber for a limited set of Daybreak Red customers – claims 81 new Firefox vulns and exploits for 948 Linux kernel bugs : r/cybersecurity - Reddit</li>
<li>OpenAI introduces GPT-6 Cyber under Daybreak Red access limits | Paul Derrington</li>

</ul>
</details>

**Tags**: `#OpenAI`, `#cybersecurity`, `#AI industry`, `#business strategy`, `#trusted access`

---

<a id="item-tech-news-7"></a>
### [Tencent open-sources GGUF quantized weights for 224B Hy4 flash](https://mp.weixin.qq.com/s/o0xxShVQX6g2UllrrEv1WQ) ⭐️ 7.0/10

Tencent Hunyuan has released GGUF quantized weights for its 224B-parameter Hy4 flash model through AngelSlim, its model compression and acceleration toolkit. The original weights are about 410.27GiB, while the smallest IQ2-AH variant is 125.73GiB, roughly 30% of the original, and Tencent says it can run on a 64GB Mac mini using the Strata offload framework. The release cites 89 tokens per second at 10K context on a device with 48GB of VRAM, and 47 tokens per second at 32K context on an M5 Max with 128GB using the Q3\_K version. Tencent also claims Q3\_K scores within 0.4 points of the original model on evaluations including DeepSWE v1.1; these figures come from the vendor and have not been independently verified.

telegram · zaihuapd · Nov 25, 09:29

**「Background」** Tencent previously released Hy4 flash as an open-weight model of roughly 220B parameters with about 12B active, and its Hugging Face model card points users to AngelSlim as the compression toolkit. AngelSlim&\#x27;s GitHub repository describes itself as a model compression toolkit supporting INT8/FP8/INT4 quantization for Hunyuan, Qwen, and DeepSeek-R1-Distill-Qwen models. The new release applies that same toolkit to produce GGUF quantized weights for Hy4 flash.

**「Impact」** The IQ2-AH variant lowers the memory floor for running a 224B model to a 64GB Mac mini, but only with Strata offload, so users should expect offloading overhead rather than full in-memory inference. Those with more memory or VRAM can choose Q3\_K, which Tencent reports as closer to the original model&\#x27;s quality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=85Gm68lK0sI">Tencent Hy 4 Flash Is Out. Time to Ditch Qwen 3.8 Flash ... - YouTube</a></li>
<li><a href="https://huggingface.co/tencent/Hy4-flash">tencent / Hy 4 - flash · Hugging Face</a></li>
<li><a href="https://github.com/Tencent/AngelSlim">GitHub - Tencent / AngelSlim : Model compression toolkit engineered...</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#open-source`, `#large-language-models`, `#local-inference`, `#model-compression`

---

<a id="item-tech-news-8"></a>
### [Samsung and SK Hynix reportedly to license YMTC Xtacking NAND tech](https://tech.ifeng.com/c/8yLRPKxQy4L) ⭐️ 7.0/10

Samsung Electronics and SK Hynix have reportedly agreed, through a cross-licensing arrangement, to use parts of Yangtze Memory Technologies&\#x27; \(YMTC\) Xtacking stacking technology in 3D NAND flash. All three companies declined to comment, so the arrangement remains unconfirmed. Xtacking fabricates the memory cells and the CMOS control circuitry on separate wafers and then bonds them together, allowing each part to be produced and optimized independently. An Omdia senior analyst cited in the report said this lets manufacturers make the memory array themselves while outsourcing logic circuitry to foundries, gaining access to more advanced process nodes.

telegram · zaihuapd · Nov 25, 14:33

**「Background」** Xtacking is YMTC&\#x27;s proprietary 3D NAND architecture, in which memory cells and peripheral CMOS logic are fabricated on separate wafers and then joined face-to-face through hybrid bonding, allowing each part to be produced and optimized independently. TechInsights analysis traces the technology from Xtacking1.0 \(64-layer TLC\) to Xtacking4.0 \(160-layer TLC\), describing hybrid bonding as the backbone of YMTC&\#x27;s high-density 3D NAND.

**「Potential impact」** If the reported cross-licensing deals hold, Samsung and SK Hynix would gain access to a production-tested wafer-bonding approach as they push NAND toward hundreds of layers, where single-wafer processes reportedly face limits. The arrangement would also give YMTC licensing leverage built on its patent portfolio, which reports describe as more than 4,000 US patent applications since 2018. Because all three companies declined to comment, the scope of the licensed technology and any effect on product roadmaps remain unconfirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techinsights.com/blog/ymtc-xtacking40-breaking-new-ground-3d-nand-technology">YMTC Xtacking4.0: Breaking New Ground in 3D NAND Technology</a></li>
<li><a href="https://www.techinsights.com/blog/ymtc-3d-nand-waveform-analysis-xtacking10-40">YMTC 3D NAND Waveform Analysis: From Xtacking1.0 to 4.0</a></li>
<li><a href="https://www.semiconductor-digest.com/unlocking-the-secrets-of-the-ymtc-64-layer-3d-xtacking-nand-flash/">Unlocking the Secrets of the YMTC 64-Layer 3D Xtacking® NAND ... Xtacking — Grokipedia Excellent Reliability of Xtacking™ Bonding Interface www.ymtc.com Samsung and SK hynix to License YMTC&#x27;s Xtacking Technology</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/25/news-sk-hynix-reportedly-joins-samsung-in-licensing-ymtcs-xtacking-technology-as-nand-race-heats-up/">[News] SK hynix Reportedly Joins Samsung in Licensing YMTC’s ...</a></li>
<li><a href="https://aiweekly.co/alerts/samsung-and-sk-hynix-tap-ymtcs-xtacking-tech-in-cross-license">Samsung and SK Hynix cross-license YMTC&#x27;s Xtacking 3D NAND</a></li>
<li><a href="https://www.techpowerup.com/355199/samsung-and-sk-hynix-to-license-ymtcs-xtacking-technology">Samsung and SK hynix to License YMTC&#x27;s Xtacking Technology</a></li>

</ul>
</details>

**Tags**: `#3D NAND`, `#semiconductor manufacturing`, `#hybrid bonding`, `#memory industry`, `#YMTC`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Report: US Commerce Department pressured Intel to hand over 10% stake](https://www.wired.com/story/inside-trumps-demands-to-another-chips-ceo/) ⭐️ 8.0/10

Court filings reportedly show that in August 2025, lawyers for the US Commerce Department told Intel&\#x27;s CFO that refusing to hand over a 10% equity stake would bring unpredictable consequences, and the board complied days later; President Trump then announced the US government fully owned and controlled the stake without paying for it, now worth about $11 billion, according to WIRED.

telegram · zaihuapd · Nov 25, 13:25

**「Background」** The reported pressure came in August 2025, during a push tied to $8.9 billion in federal semiconductor subsidies Intel had already been granted, according to unsealed filings in a shareholder lawsuit cited by WIRED. Intel publicly described the arrangement at the time as an $8.9 billion government investment in its common stock.

**「Impact」** If accurate, the arrangement gives the US government a direct ownership role in a major chipmaker, a precedent that could affect how other semiconductor firms weigh government requests.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/wired-commerce-lawyer-warned-intel-cfo-rejecting-us-10-stake-would-carry">Court records: Commerce threatened Intel CFO over 10% US stake</a></li>
<li><a href="https://www.gate.com/news/detail/us-commerce-department-threatened-intel-over-10-equity-stake-for-89b-25860002">U.S. Commerce Department Threatened Intel Over 10% Equity ...</a></li>
<li><a href="https://www.intel.com/content/www/us/en/newsroom/news/corporate/intel-and-trump-administration-reach-historic-agreement.html">Intel and Trump Administration Reach Historic Agreement to ...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#US policy`, `#Intel`, `#government equity stake`, `#corporate governance`

---

<a id="item-finance-news-2"></a>
### [美国拟对14个贸易伙伴加征新关税](https://www.cnbc.com/2026/11/25/us-tariffs-trump-section-301.html) ⭐️ 8.0/10

美国政府拟依据1974年《贸易法》第301条，对中国、欧盟、日本、印度等14个贸易伙伴加征新关税，理由是这些国家存在制造业结构性产能过剩。关税按国别设定，中国将在2018年已加征的25%之上再加征20%；若中国未遵守2025年10月在韩国釜山达成的贸易休战协议，对华新关税可能升至40%。

telegram · zaihuapd · Nov 25, 13:59

**「Background」** The proposal follows an eight-month US investigation into subsidized foreign manufacturing and is intended to replace levies struck down by the Supreme Court earlier this year, according to Fox Business. It also comes after the October 2025 Busan summit, where the US and China agreed a trade truce that included cutting US fentanyl tariffs on Chinese imports by 10 percentage points.

**「影响」** 若该提案落地，向美国出口上述商品的制造商和美国进口商将面临更高成本，其中中国商品叠加后的税率最高。

<details><summary>References</summary>
<ul>
<li><a href="https://www.foxbusiness.com/fox-news-global-economy/trump-admin-raise-tariffs-china-eu-other-trading-partners">Trump administration proposes sweeping Section 301 ... | Fox Business</a></li>
<li><a href="https://en.wikipedia.org/wiki/China%E2%80%93United_States_trade_war">China – United States trade war - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#trade policy`, `#tariffs`, `#Section 301`, `#US-China trade`, `#manufacturing`

---

<a id="item-finance-news-3"></a>
### [Nvidia Swings Test Fed Chair Warsh&\#x27;s Market-Signal Approach](https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html) ⭐️ 7.0/10

CNBC&\#x27;s Steve Liesman reports that sharp Nvidia-driven market swings are testing Federal Reserve Chairman Kevin Warsh&\#x27;s preference for reading market signals over forecasts, after the Goldman Sachs Financial Conditions Index eased 22 basis points on Monday, reversing nearly half of the prior week&\#x27;s tightening and restoring market-implied odds of December and January rate hikes.

rss · CNBC Finance · Nov 25, 12:26

**「Background」** Kevin Warsh took office as Federal Reserve chairman on May 22, 2026, succeeding Jerome Powell, whose term ended May 15, 2026. The Goldman Sachs Financial Conditions Index that Warsh is said to favor is a weighted gauge of short-term bond yields, long-term corporate yields, the exchange rate, and stock prices.

**「Impact」** If Warsh leans more on market-based indicators, households and businesses could see interest-rate policy react to short-lived swings in stocks and credit spreads rather than to forecasts, making the path of borrowing costs harder to predict.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/aboutthefed/bios/board/warsh.htm">Federal Reserve Board - Kevin Warsh, Chairman</a></li>
<li><a href="https://sites.lsa.umich.edu/mje/2026/03/07/2026-monetary-policy-outlook/">2026 Monetary Policy Outlook – Michigan Journal of Economics</a></li>
<li>[PDF] NBER WORKING PAPER SERIES FINANCIAL CONDITIONS INDEXES: A FRESH LOOK AFTER THE FINANCIAL CRISIS Jan Hatzius Peter Hooper Frederi</li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#Nvidia`, `#market volatility`, `#Kevin Warsh`

---