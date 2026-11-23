---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 28 items, 9 important content pieces were selected

---

**Technology News**
1. [OpenAI Essay Links Lower Perplexity to Model Intelligence](#item-tech-news-1) ⭐️ 7.0/10
2. [Phison launches space-rated Pascari SSDs, 488 TB planned for orbit](#item-tech-news-2) ⭐️ 7.0/10
3. [Google Built Simulated Internet to Test Chrome AI Agent](#item-tech-news-3) ⭐️ 7.0/10
4. [Windows Server 2028 to drop WoW64 by default, blocking 32-bit apps](#item-tech-news-4) ⭐️ 7.0/10

**Technology Blog**
1. [Flailing as a Strategy for Ambiguous Problems](#item-tech-blog-1) ⭐️ 6.0/10

**Financial News**
1. [US Tech Selloff Prompts Asian Market Stabilization Measures](#item-finance-news-1) ⭐️ 9.0/10
2. [FT Report Alleges Nvidia Chip Smuggling Network Linked to Cambodia&\#x27;s Prince Group](#item-finance-news-2) ⭐️ 7.0/10
3. [中国要求美国撤销电话号段接入限制](#item-finance-news-3) ⭐️ 7.0/10
4. [Ant Group Leads $100M Round in Chinese Robotics Startup Simplexity](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Essay Links Lower Perplexity to Model Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 7.0/10

An OpenAI essay argues that lower perplexity—the model&\#x27;s degree of surprise when predicting the next token—correlates with greater model intelligence, and the piece drew substantial debate on Hacker News \(513 points, 353 comments\). The article is a position piece rather than a release or independently measured result, and commenters noted it does not itself define perplexity. Discussion centered on whether cross-entropy loss remains meaningful as reinforcement learning becomes more common, and on compression-as-intelligence arguments. One commenter cited a tweet from Mustafa Suleyman saying Microsoft reported its MAI-2 Base model on OpenAI&\#x27;s evaluation set with a log-perplexity of 0.819, described as in the same ballpark as a GPT-5.6 Sol base model.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**「Background」** Perplexity is a long-standing language-model training metric: it measures how surprised a model is when predicting each next token, ranging from 1 for perfect prediction to roughly the vocabulary size for a random predictor. OpenAI&\#x27;s essay, attributed in coverage to Chief Scientist Jakub Pachocki, argues that lower perplexity tracks with greater capability and proposes it as a shared yardstick; secondary coverage reports the piece ties specific log-perplexity values on an OpenAI evaluation set to model generations, such as GPT-3.5 near 0.99 and GPT-4 near 0.91. The essay is a position piece rather than a release, and the reported figures come from that evaluation set rather than independent measurement.

**「Impact」** If perplexity becomes a shared yardstick, model developers may face pressure to report pre-training loss on common held-out sets, as one commenter claims Microsoft&\#x27;s Mustafa Suleyman said the company would do for its MAI models. That would give buyers and researchers a simpler cross-vendor comparison than task-specific benchmarks, but it would also reward optimizing for next-token prediction rather than downstream behavior.

**「Community Discussion」** Commenters supplied the definition the essay omitted: perplexity ranges from 1 for a perfect predictor to the vocabulary size for a random one. One commenter said the clear cross-entropy trend was surprising given the rise of RL and welcomed a simpler benchmark over increasingly convoluted ones, while another argued that prediction and compression rates on raw data are exactly the metric that captures progress toward world models, citing a 2008 paper. A third relayed Suleyman&\#x27;s claim that Microsoft is committing to share pre-training progress on a common held-out evaluation set.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence - OpenAI</a></li>
<li><a href="https://www.datastudios.org/post/openai-proposes-perplexity-limits-frontier-ai-development">OpenAI proposes perplexity limits on frontier AI and ...</a></li>
<li><a href="https://officechai.com/ai/openai-wants-perplexity-to-become-the-industrys-shared-yardstick-for-ai-progress-and-safety-limits/">OpenAI Wants &#x27;Perplexity&#x27; To Become The Industry&#x27;s Shared ...</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#language-models`, `#perplexity`, `#benchmarking`, `#openai`

---

<a id="item-tech-news-2"></a>
### [Phison launches space-rated Pascari SSDs, 488 TB planned for orbit](https://videocardz.com/newz/phison-announces-488tb-of-ssd-storage-for-space-data-centers-pricing-expected-to-be-astronomical) ⭐️ 7.0/10

Phison announced the Pascari Space SSD family for spacecraft, satellites, and in-orbit data centers, split into Flight Critical, Main Storage, and Orbital Data Center tiers with capacities up to 128 TB per drive. The company confirmed the line will be used in Lonestar Data Holdings&\#x27; StarVault-001 orbital data center, which is planned to launch in the first half of 2027 carrying 488 TB of Phison storage, with roughly 370 TB usable once in low Earth orbit. Phison claims pSLC mode on some models raises write endurance by up to 60 times, a vendor figure not independently verified in the source. The products are described as already available.

telegram · zaihuapd · Nov 22, 10:31

**「Background」** Lonestar Data Holdings is the operator behind StarVault-001, the orbital data center that will carry Phison&\#x27;s 488 TB of flash storage; the company has separately contracted outside firms for related services, including a deal announced in August for satellite protection. Phison&\#x27;s Pascari Space line is split into Flight Critical, Main Storage, and Orbital Data Center tiers, with the top capacity at 128 TB per drive.

**「Impact」** The 488 TB figure is an aggregate across the StarVault-001 payload, not a single drive, so capacity planning for orbital deployments depends on how many 128 TB-class units are combined. The endurance claim rests on pSLC provisioning, which trades capacity for write life, meaning operators choosing that mode will see less usable storage than the raw tier capacity suggests.

<details><summary>References</summary>
<ul>
<li><a href="https://www.space.com/space-exploration/satellites/satellite-defense-ares-shield-contract-lonestar-data-holdings">Polish startup Ares Shield hired to protect data center ... | Space</a></li>
<li><a href="https://dzen.ru/a/awLShV56vGiwFBoU">Она включает категории Flight Critical, Main Storage и Orbital Data ...</a></li>

</ul>
</details>

**Tags**: `#storage`, `#hardware`, `#space-computing`, `#data-centers`, `#ssd`

---

<a id="item-tech-news-3"></a>
### [Google Built Simulated Internet to Test Chrome AI Agent](https://www.landian.news/archives/128701.html) ⭐️ 7.0/10

Google reportedly built a simulated internet environment called Mirror Dimension to test a Chrome AI agent in isolation. According to Landian News, the environment contains thousands of simulated websites, with each engineer testing in a separate isolated setup, and runs more than 1,000 test cases per day. The tests cover agent actions such as opening sites, searching and browsing, logging in, adding items to a cart, and completing tasks, with a focus on defending against prompt-injection attacks from malicious web pages. The report is a secondary summary without primary documentation or independent verification, so the scale figures and security emphasis remain unconfirmed vendor claims.

telegram · zaihuapd · Nov 23, 01:30

**「Background」** Google&\#x27;s security blog describes Mirror Dimension as a synthetic version of the web used to evaluate &quot;auto browse,&quot; the Chrome agent capability that opens sites, searches, logs in, and completes tasks. The environment contains thousands of simulated websites modeled on everyday user journeys, letting engineers test the agent without exposing real accounts or sites to risky behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents: Evaluating Browser-Use Agents ...</a></li>
<li><a href="https://explainx.ai/blog/google-mirror-dimension-synthetic-web-chrome-auto-browse-agents-prompt-injection-testing-2026">Google Mirror Dimension: Fake Web for Chrome AI Agents ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#browser automation`, `#prompt injection`, `#AI security`, `#Chrome`

---

<a id="item-tech-news-4"></a>
### [Windows Server 2028 to drop WoW64 by default, blocking 32-bit apps](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 7.0/10

Microsoft said at Ignite 2026 that Windows Server 2028 will ship without the WoW64 compatibility subsystem, so 32-bit applications will not run out of the box. The release is planned for fall 2027 alongside Windows 11 27H2. Administrators can add WoW64 back as an on-demand feature \(FoD\), typically via PowerShell or DISM on Server Core. Microsoft cited reducing attack surface and blocking 32-bit malware as the rationale; Windows 11 keeps WoW64 for now, with no removal plan announced.

telegram · zaihuapd · Nov 23, 03:03

**「Background」** WoW64 is the Windows subsystem that lets 64-bit Windows run 32-bit applications, so removing it from the default install breaks legacy software unless the component is added back. Microsoft&\#x27;s own documentation for Windows Server 2028 also lists .NET Framework 3.5 as no longer an inbox optional component or Feature on Demand, indicating a broader reduction of legacy components in that release.

**「Impact」** Server operators running legacy 32-bit software will need to install the WoW64 FoD during deployment or upgrade planning, and should verify that their tooling supports adding it on Server Core. Because the change is an announced roadmap item rather than a shipped release, the exact default state and installation steps could still change before fall 2027.

<details><summary>References</summary>
<ul>
<li>Features Removed or No Longer Developed in Windows Server - Microsoft Learn</li>

</ul>
</details>

**Tags**: `#windows-server`, `#wow64`, `#32-bit-compatibility`, `#microsoft`, `#platform-deprecation`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Flailing as a Strategy for Ambiguous Problems](https://seangoedecke.com/when-in-doubt-flail-about/) ⭐️ 6.0/10

rss · Sean Goedecke · Nov 23, 00:00

**「Background」** When you lack clear guidance or don&\#x27;t know what will help, the instinct is often to be cautious and wait for better understanding. Sean Goedecke argues this is typically the wrong move, though he acknowledges the advice is dangerous: flailing badly can damage your reputation at a tech company.

**「Solution」** Goedecke&\#x27;s central insight is that deliberate, broad experimentation with tight feedback loops is the fastest way to gain understanding. He lays out three principles: try many different things, pay careful attention to feedback, and ruthlessly drop anything not getting positive feedback. Trying many things matters because most plans will be bad, and having many plans prevents over-investment in any single one. He applies this to three contexts. In product flailing, he cites his work on GitHub Models \(now retired\), where most features didn&\#x27;t work but one—running AI inference from a GitHub Actions token—was surprisingly sticky and seeded &quot;Continuous AI.&quot; In engineering flailing, he recommends making speculative changes to large, complex systems rather than trying to understand them fully first, noting AI agents help generate multiple refactors to skim. In organizational flailing, relevant to senior and staff engineers, he suggests trying many things that might help when problems aren&\#x27;t technical, while warning that this is where feedback sensitivity matters most: dropping failing plans builds trust, but pressing on can direct anger at you. He calls it &quot;flailing&quot; because it feels like failure from the inside, even if it looks like proactive experimentation from the outside.

**「Takeaway」** Goedecke&\#x27;s thesis is that the unpleasant feeling of flailing is a psychological barrier to push through, not a sign you&\#x27;re in trouble. So long as you stay sensitive to feedback and drop failing plans instantly, flailing can be an incredibly effective approach to difficult engineering and organizational problems.

**Tags**: `#engineering-practice`, `#decision-making`, `#experimentation`, `#organizational-dynamics`, `#career-advice`

---

## Financial News

<a id="item-finance-news-1"></a>
### [US Tech Selloff Prompts Asian Market Stabilization Measures](https://news.bjd.com.cn/2026/11/22/12039852.shtml) ⭐️ 9.0/10

US AI and tech stocks fell sharply on Friday, with the Nasdaq down 5.28% in one day and the Philadelphia Semiconductor Index down nearly 11%, according to the report. In response, mainland China, South Korea, and Taiwan announced market stabilization measures, including margin and short-selling restrictions.

telegram · zaihuapd · Nov 22, 13:24

**「Background」** The measures aim to curb selling pressure: mainland China lowered the minimum margin financing ratio to 80%, South Korea eased daily share buyback limits for three months starting November 24, and Taiwan banned short-selling below the previous close from November 23 and raised short-sale margin from 130% to 150%.

**「Impact」** These rules directly affect investors and listed companies in the three markets by making short-selling and margin trading more costly or restrictive, which can reduce liquidity and limit hedging options.

**Tags**: `#US tech stocks`, `#semiconductor selloff`, `#market stabilization policy`, `#short-selling rules`, `#Asian markets`

---

<a id="item-finance-news-2"></a>
### [FT Report Alleges Nvidia Chip Smuggling Network Linked to Cambodia&\#x27;s Prince Group](https://www.ft.com/content/f3ad8a81-3890-4a8a-8853-ff0a94b08ba9?syn-25a6b1a6=1) ⭐️ 7.0/10

The Financial Times, citing people familiar with the matter, reported that Hu Xiaowei, described by the U.S. Treasury as the &quot;number two&quot; figure at Cambodia&\#x27;s Prince Group, allegedly helped move Nvidia chips into China, with trade data showing about $4.6 billion in declared imports by Megaspeed&\#x27;s Malaysian subsidiary between December 2024 and December 2025. Prince Group denies that Hu worked for it and says the allegations of an illegal network and private-jet smuggling lack factual basis.

telegram · zaihuapd · Nov 22, 04:34

**「Background」** The US Treasury has previously sanctioned Cambodia&\#x27;s Prince Group and associates, and Singapore is investigating Hu Xiaowei for money laundering, according to the Straits Times. Separately, Malaysia said in November 2026 it was investigating whether AI chips imported by a Megaspeed unit were re-exported, Reuters reported.

**「Who is affected」** The report points to a gap in US export controls, which have struggled to stop chip smuggling despite enforcement actions \(tool-3-1\). Nvidia&\#x27;s board has since formed a committee to oversee compliance with those controls amid heightened scrutiny \(tool-3-3\).

<details><summary>References</summary>
<ul>
<li><a href="https://www.straitstimes.com/singapore/courts-crime/spore-investigating-2-men-linked-to-prince-group-after-us-sanctions-600m-in-assets-seized-so-far">S’pore investigating 2 men linked to Prince Group hit by US sanctions ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/malaysia-says-it-is-investigating-if-any-chips-linked-speedmatrix-were-re-2026-11-13/">Malaysia probing whether chips linked to Megaspeed unit were ...</a></li>
<li><a href="https://www.atlanticcouncil.org/dispatches/beyond-the-spy-scandal-what-the-nvidia-megaspeed-case-reveals-about-export-controls/">Beyond the spy scandal: What the Nvidia-Megaspeed case ...</a></li>
<li><a href="https://www.cbsnews.com/news/nvidia-export-control-committee-china-chips/">Nvidia&#x27;s board forms export oversight panel after scrutiny ...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export controls`, `#Nvidia`, `#smuggling`, `#Cambodia`

---

<a id="item-finance-news-3"></a>
### [中国要求美国撤销电话号段接入限制](https://www.bloomberg.com/news/articles/2026-11-22/china-objects-to-us-curbs-on-telecoms-access-to-phone-numbers) ⭐️ 7.0/10

中国商务部于11月22日敦促美国撤销一项措施，该措施禁止中国移动、中国电信和中国联通直接获取美国电话号码；商务部称此举违反非歧视与公平竞争原则，并指美国联邦通信委员会（FCC）在缺乏事实依据的情况下援引国家安全风险。

telegram · zaihuapd · Nov 22, 06:44

**「Background」** On November 19, the U.S. Federal Communications Commission voted to bar China Mobile, China Telecom and China Unicom from directly obtaining U.S. phone numbers, adding national-security certifications aimed at equipment and services on its Covered List. The three carriers were already barred from offering international telecom services to the United States.

**「影响」** 若该限制维持，这三家中国国有运营商将无法直接接入美国电话号码，而商务部警告称，近期举措正把两国推向电信、通信及检测认证领域的脱钩。

<details><summary>References</summary>
<ul>
<li><a href="https://www.fcc.gov/document/fcc-cracks-down-bad-actors-access-us-phone-numbers-0">FCC Cracks Down on Bad Actors&#x27; Access to U.S. Phone Numbers</a></li>
<li><a href="https://www.reuters.com/world/fcc-votes-ban-chinese-telecoms-direct-access-us-phone-numbers-2026-11-19/">FCC votes to ban Chinese telecoms from direct access to US ...</a></li>
<li><a href="https://finance.biggo.com/news/af7ccb0c-75c7-434b-834c-ced72af0d3c4">FCC Blocks China Mobile, Telecom and Unicom From Direct ...</a></li>

</ul>
</details>

**Tags**: `#telecom regulation`, `#US-China relations`, `#FCC`, `#China carriers`, `#policy dispute`

---

<a id="item-finance-news-4"></a>
### [Ant Group Leads $100M Round in Chinese Robotics Startup Simplexity](https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race) ⭐️ 7.0/10

Ant Group led a $100 million pre-A funding round in Chinese embodied-AI startup Simplexity Robotics at a $1.6 billion post-money valuation, with Alibaba, Tencent, HongShan and BlueRun also investing, chairman and co-founder Wang Kai confirmed to Bloomberg. The Hangzhou-based company, founded in July 2025 by a team from Li Auto, had previously disclosed raising 2 billion yuan across five rounds within its first six months, when its valuation already exceeded $1 billion.

telegram · zaihuapd · Nov 23, 02:02

**「Background」** Simplexity Robotics was founded in Hangzhou in July 2025 by a core team from Li Auto, and by March 2026 it had disclosed five funding rounds totaling 2 billion yuan within six months of launch, at a post-money valuation already above $1 billion. Ant Group has been assembling a portfolio of humanoid-robotics investments in China, with external reports describing roughly a dozen such deals over about 18 months.

**「Impact」** The funding gives Simplexity capital to compete for China&\#x27;s humanoid-robot market against more established makers such as Unitree and UBTech, a sector Bloomberg reports accounts for about 97% of global humanoid robot shipments.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/ant-group-humanoid-robots-dozen-deals/">Ant Group rushes into humanoid robots with dozen deals in 18 months</a></li>
<li><a href="https://lanceum.com/analysis/ant-group-humanoid-bets-fintech-robot-future">Twelve Deals in Eighteen Months: Why Ant Group Is... | Lanceum</a></li>

</ul>
</details>

**Tags**: `#funding`, `#robotics`, `#China tech`, `#venture capital`, `#Ant Group`

---