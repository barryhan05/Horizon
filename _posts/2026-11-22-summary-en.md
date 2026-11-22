---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 23 items, 12 important content pieces were selected

---

**Technology News**
1. [Lean 社区认证 1700 万行黎曼猜想形式化证明](#item-tech-news-1) ⭐️ 10.0/10
2. [GnuPG/GPGME Flaw Disclosed as RCE, Community Disputes Severity](#item-tech-news-2) ⭐️ 8.0/10
3. [Zhejiang University reports first hardware QRAM demo on superconducting chip](#item-tech-news-3) ⭐️ 8.0/10
4. [Monitor&\#x27;s USB Hub Cut Ethernet Download Speed by 75%](#item-tech-news-4) ⭐️ 7.0/10
5. [Muru: AI-Assisted Rust Server for ASGI and WSGI Python Apps](#item-tech-news-5) ⭐️ 7.0/10
6. [Microsoft previews RDMA over USB4 for multi-PC AI inference on Windows](#item-tech-news-6) ⭐️ 7.0/10
7. [OpenRouter 警告 MiniMax 模型提示词疑遭第三方读取](#item-tech-news-7) ⭐️ 7.0/10
8. [Daraxonrasib 一线胰腺癌数据：61 例中 8.2% 完全缓解](#item-tech-news-8) ⭐️ 7.0/10
9. [Tesla begins overseas rollout of FSD v15](#item-tech-news-9) ⭐️ 7.0/10

**Technology Blog**
1. [Good Programming Is About Avoiding Blunders](#item-tech-blog-1) ⭐️ 5.0/10

**Financial News**
1. [China Uses APEC Summit to Expand Global Diplomatic Role](#item-finance-news-1) ⭐️ 7.0/10
2. [Trump Says U.S. Firms Building AI Data Centers Abroad Could Face &\#x27;Huge Taxes&\#x27;](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lean 社区认证 1700 万行黎曼猜想形式化证明](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 10.0/10

2026 年 11 月 20 日，Levent Alpöge 发布了黎曼猜想的 Lean 形式化证明，代码库约 1700 万行。次日，Lean FRO 与 Mathlib Initiative 联合声明称，该命题与证明均正确：社区确认其陈述与 Mathlib 的 RiemannHypothesis 一致，代码库可无错编译，且多个独立证明检查器验证了证明有效。上述认证内容来自 Telegram 帖子对 Lean 社区博客的转述，具体细节无法在此独立核实。

telegram · zaihuapd · Nov 21, 16:48

**「Background」** The Riemann Hypothesis is one of mathematics&\#x27; longstanding open problems, and Lean is an interactive theorem prover in which proofs are checked by machine kernels rather than by human referees. Levent Alpöge, a number theorist who has also worked at Anthropic, released the formalization on November 20, 2026, according to the Lean community blog post that the Telegram item links to. The following day, the Lean and Mathlib communities issued a joint statement, endorsed by the Lean FRO and the Mathlib Initiative, certifying the statement and proof.

**「影响」** 若认证成立，该形式化将黎曼猜想与 Mathlib 的既有陈述绑定，使后续工作可直接在该代码库上构建，而无需重新形式化相关数学。评论者指出，这一规模意味着大量现代数学被一并形式化，其价值可能超出黎曼猜想本身。

**「社区讨论」** 有评论者认为，由于存在多个独立实现和内核一致性证明，证明依赖检查器漏洞的可能性已很小；但也有人提醒，过去曾有伪造的 Collatz 反证通过某个独立检查器，因此“独立”程度有限，不过此次有人类专家参与降低了这一风险。另有评论者强调，应把主要功劳归于 Levent Alpöge 对工具的驾驭能力，而非仅归于模型本身。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>
<li><a href="https://leanprover-community.github.io/blog/posts/riemann-hypothesis/">Lean verification of the Riemann Hypothesis | Lean community blog</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#Lean`, `#mathematics`, `#Riemann Hypothesis`, `#open source`

---

<a id="item-tech-news-2"></a>
### [GnuPG/GPGME Flaw Disclosed as RCE, Community Disputes Severity](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

A GnuPG/GPGME vulnerability affecting versions prior to 2.3.0 was publicly disclosed on 2026-11-20, earlier than the originally planned 2026-11-25 coordinated date. According to a commenter citing the disclosure, the bug was found by Johan Carlsson and reported to the project by GitLab on 2026-11-12; the earlier release was attributed to GitLab needing to update ahead of the Ruby2Shell bug. The disclosure is framed as remote code execution, but commenters dispute that characterization, with one describing it as a double free rather than an RCE chain. The affected surface is broad: one commenter says all software using GPGME before 2.3.0 is affected, whether as a shared library, DLL, or statically linked, citing Gpg4win, GnuPG Desktop, GnuPG VS-Desktop, most mail clients, many XMPP clients, Samba, and Flatpak as examples.

hackernews · gdgghhhhh · Nov 21, 08:32 · [Discussion](https://news.ycombinator.com/item?id=50587208)

**「Background」** GPGME is the library applications use to integrate GnuPG, so the flaw&\#x27;s reach depends on which GPGME version a program links against rather than on the GnuPG command-line tool itself. The advisory describes the bug as a double free that can be triggered by sending signed data, allowing data exfiltration, and states that RCE &quot;can&\#x27;t be ruled out.&quot; The first fixed release is GPGME 2.3.1; version 2.3.0 was never publicly available, and the disclosure was moved up from November 25 because of the Ruby2Shell bug.

**「Who Is Affected」** Users and integrators of GPGME versions before 2.3.0 need to check their dependency, including statically linked builds where a system package update may not reach the vulnerable code. GitLab is directly implicated because it supports signed commits, and a commenter links a GitLab Omnibus patch; another commenter notes Red Hat reportedly fixed the issue in its packaging five years ago while upstream missed it, so downstream patches may already cover some deployments.

**「Community View」** Commenters disagree on severity: one argues the report is a double free bug rather than an RCE chain and asks whether such reports are intentionally overstated, while another stresses that code execution in GitLab&\#x27;s signed-commit path would be serious. A commenter also questions whether the flaw is confined to GPGME and does not affect tools like apt, which the supplied comments do not resolve.

<details><summary>References</summary>
<ul>
<li><a href="https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html">[Announce] GnuPG Security Advisory for GPGME ...</a></li>
<li><a href="https://thehackernews.com/2026/11/gnupg-warns-critical-gpgme-flaw-could.html">GnuPG Warns Critical GPGME Flaw Could Expose App Data via...</a></li>
<li><a href="https://www.phoronix.com/news/GnuPG-GPGME-Critical">GnuPG&#x27;s GPGME Affected By Critical Security Bug In Turn... - Phoronix</a></li>

</ul>
</details>

**Tags**: `#security`, `#gnupg`, `#vulnerability`, `#open-source`, `#cryptography`

---

<a id="item-tech-news-3"></a>
### [Zhejiang University reports first hardware QRAM demo on superconducting chip](https://finance.sina.com.cn/stock/2026-11-21/doc-iniznhsk3530826.shtml) ⭐️ 8.0/10

A Zhejiang University team reportedly demonstrated a quantum random access memory \(QRAM\) prototype on its self-fabricated superconducting chip &quot;Tianmu-2,&quot; described as the first real-hardware implementation of QRAM, with results published in Nature Physics. The prototype retrieved 4-bit and 8-bit data with 80.9% and 60.4% accuracy, respectively, and the team reports circuit depth reduced by more than 30% versus an unoptimized scheme. The work also claims the first verification that the architecture has local noise resilience. The team says next steps are scaling up QRAM research; the accuracy figures are modest and the claims come from a brief secondary report rather than independent verification.

telegram · zaihuapd · Nov 21, 08:31

**「Background」** QRAM is a proposed quantum memory architecture meant to let a quantum computer fetch stored data in superposition, a capability standard quantum circuits lack. The Zhejiang University work was run on the team&\#x27;s own superconducting chip, &quot;Tianmu-2,&quot; which a separate November 2026 report describes as a 125-qubit superconducting processor developed in Wang&\#x27;s lab at the university.

**「Impact」** The reported 60.4% accuracy for 8-bit retrieval indicates the prototype is far from error-corrected, reliable memory, so practical use would depend on improving fidelity as the design scales. The claimed local noise resilience and reduced circuit depth are the details most relevant to groups evaluating QRAM architectures for future quantum processors.

<details><summary>References</summary>
<ul>
<li><a href="https://phys.org/news/2026-11-quantum-teleportation-method-weaker-entanglement.html">Quantum teleportation method uses weaker entanglement to transfer...</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#QRAM`, `#superconducting qubits`, `#research`, `#hardware`

---

<a id="item-tech-news-4"></a>
### [Monitor&\#x27;s USB Hub Cut Ethernet Download Speed by 75%](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

A blog post by tymscar documents a single-user investigation in which a monitor&\#x27;s built-in USB hub added enough latency to an attached Ethernet adapter that the adapter dropped packets and download speeds fell by 75%. The author traced the regression to the hub&\#x27;s added latency, which slowed packet acknowledgements until a buffer on the adapter filled and overflowed. Switching to a different adapter that required less frequent acknowledgement resolved the problem. The finding is a troubleshooting anecdote from one setup, not a measured result across hardware.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**「Why it matters」** USB hubs, including those built into monitors and docks, can add latency that is invisible in normal use but matters for timing-sensitive network traffic. TCP throughput depends on timely acknowledgements, so a delay in the path between host and adapter can cause buffer overruns and packet loss even when raw link speed is unchanged.

**「Practical takeaway」** Users seeing unexplained throughput drops on a USB Ethernet adapter should test it connected directly to the host rather than through a monitor or dock hub, and compare adapters, since the author&\#x27;s fix was a different adapter with different acknowledgement behavior.

**「Community reaction」** Commenters pushed back on the framing: manarth argued the monitor is largely irrelevant and the issue is better described as a USB network switch cutting speed. fancyfredbot summarized the mechanism as added latency preventing timely packet acknowledgement, filling the adapter&\#x27;s buffer and causing drops, and called the post a good account of opaque USB hub behavior. gh123man reported a similar year-long problem with a MacBook and Thunderbolt dock, saying enabling flow control was good enough after trying multiple adapter brands.

**Tags**: `#networking`, `#usb`, `#hardware-debugging`, `#performance`, `#troubleshooting`

---

<a id="item-tech-news-5"></a>
### [Muru: AI-Assisted Rust Server for ASGI and WSGI Python Apps](https://simonwillison.net/2026/Nov/21/muru/) ⭐️ 7.0/10

Graham Dumpleton, who started mod\_wsgi 20 years ago, has released Muru, an AI-assisted Rust server for running ASGI and WSGI Python applications in development and production. He has documented the project in a public series of 18 posts published between November 4 and November 21, 2026, covering worker internals, running WSGI and ASGI together, releases without restarts, canary deployments without a service mesh, Kubernetes integration, scaling to zero, and a per-page toolbar with tracing. Dumpleton describes the AI as doing much of the surface work while he judges what is not good enough yet, and says he intends to keep polishing Muru until he would trust it. The material presents an early-stage project and its author&\#x27;s stated intentions rather than independently measured production results.

rss · Simon Willison · Nov 21, 23:56

**「Background」** Graham Dumpleton created mod\_wsgi, an Apache module for hosting WSGI Python applications, roughly 20 years before Muru&\#x27;s release. Horizon&\#x27;s September 11 digest covered his earlier project wrapture, which he documented through the same kind of detailed public development write-up now accompanying Muru.

**「Impact」** Python teams evaluating deployment servers now have a documented alternative that targets both WSGI and ASGI apps and addresses container and Kubernetes workflows, but the evidence so far is the author&\#x27;s own write-ups, so adoption should follow testing rather than the announcement alone.

**Tags**: `#python`, `#asgi`, `#wsgi`, `#rust`, `#web-servers`

---

<a id="item-tech-news-6"></a>
### [Microsoft previews RDMA over USB4 for multi-PC AI inference on Windows](https://videocardz.com/newz/microsoft-brings-rdma-over-usb4-to-windows-allowing-multiple-pcs-to-run-one-local-ai-model) ⭐️ 7.0/10

Microsoft released a Windows developer preview of RDMA over USB4 that lets multiple PCs pool memory and GPU compute to run a single local AI model over ordinary USB4 connections, without dedicated network cards or switches. In a reported demonstration, three AMD Ryzen AI Max+ 395 systems ran Qwen3-235B-A22B at 4-bit quantization at roughly 18.5 tokens per second. The preview is being distributed through Windows Insider, so it is an announced developer capability rather than a broadly shipped feature.

telegram · zaihuapd · Nov 21, 06:13

**「Background」** RDMA lets one system read or write approved memory on another with less OS and CPU involvement than conventional networking, and Windows already exposes it through the NetworkDirect API used with datacenter RDMA adapters. Microsoft&\#x27;s preview adapts that same API to USB4 links, so the pooled-memory setup relies on existing Windows networking interfaces rather than a new stack. The approach targets Windows 11 PCs connected by USB4, per coverage of the announcement.

<details><summary>References</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoftusbblog/introducing-rdma-over-usb4%C2%AE-on-windows-run-larger-local-ai-models-across-pcs/4574602">Introducing RDMA over USB 4 ® on Windows : run larger local AI ...</a></li>
<li><a href="https://www.guru3d.com/story/microsoft-previews-usb4-links-that-let-windows-pcs-pool-memory-and-gpu-resources/">Microsoft previews USB 4 links that let Windows PCs pool memory ...</a></li>
<li><a href="https://www.techpowerup.com/355062/microsoft-brings-rdma-over-usb4-to-windows-11-for-daisy-chained-pcs">Microsoft Brings RDMA over USB 4 to Windows 11... | TechPowerUp</a></li>

</ul>
</details>

**Tags**: `#RDMA over USB4`, `#local AI inference`, `#Windows`, `#distributed computing`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [OpenRouter 警告 MiniMax 模型提示词疑遭第三方读取](https://news.ycombinator.com/item?id=50585962) ⭐️ 7.0/10

OpenRouter 通过邮件通知用户，发往 MiniMax 模型的请求内容可能已被第三方读取。安全研究者在 2026 年 7 月至 10 月间向 MiniMax 模型发送含测试 URL 的提示词，这些 URL 在 40 到 130 小时后被第三方访问。OpenRouter 将问题归因于 MiniMax 及其转发方 AtlasCloud、Novita 和 StreamLake，已下架相关端点的「零数据保留」标签，并建议涉及敏感凭证的用户更换 API Key 和密码。OpenRouter 官网尚未公布相关消息，该事件目前缺乏官方确认。

telegram · zaihuapd · Nov 21, 06:53

**「Background」** OpenRouter routes requests to many model providers and labels some endpoints &quot;Zero Data Retention,&quot; a designation users rely on when sending sensitive material. The warning concerns MiniMax models reached through OpenRouter and the intermediaries AtlasCloud, Novita, and StreamLake; reports say the same canary-URL test against other models did not show the same access.

**「影响与建议」** 通过 OpenRouter 向 MiniMax 模型发送过敏感数据的用户应假定提示词内容可能已外泄，并按 OpenRouter 建议轮换 API Key 和相关密码。依赖「零数据保留」标签判断数据不会被留存或转交的用户，需要重新评估经第三方转发商路由请求的隐私风险。

<details><summary>References</summary>
<ul>
<li><a href="https://www.hallattorneys.com/investigations/openrouter-minimax">OpenRouter MiniMax Prompt Exposure Investigation - Hall Attorneys</a></li>
<li><a href="https://startupfortune.com/openrouter-warns-minimax-prompts-may-have-been-read-by-a-third-party/">OpenRouter warns MiniMax prompts may have been read by a ...</a></li>
<li><a href="https://www.gate.com/news/detail/minimaxs-zero-data-retention-fails-user-prompts-accessed-by-third-parties-25775454">MiniMax&#x27;s Zero Data Retention Fails: User Prompts Accessed by ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#LLM APIs`, `#OpenRouter`, `#MiniMax`

---

<a id="item-tech-news-8"></a>
### [Daraxonrasib 一线胰腺癌数据：61 例中 8.2% 完全缓解](https://event.eortc.org/ena2026/2026/11/20/metastatic-pancreatic-cancer-responds-well-to-initial-treatment/) ⭐️ 7.0/10

在 ENA 2026 大会的 late-breaking 口头报告中，daraxonrasib 联合吉西他滨/白蛋白紫杉醇用于 61 例既往未治疗的转移性胰腺导管腺癌患者，口服 200 mg 每日一次，确认客观缓解率为 60.7%，完全缓解率为 8.2%（约十二分之一），疾病控制率为 90.2%。中位无进展生存期为 12.8 个月，12 个月总生存率为 76.6%，中位随访 18.3 个月。研究者强调这是单臂 I/II 期研究、没有化疗对照组，疗效对比需由正在进行的 III 期试验验证。

telegram · zaihuapd · Nov 21, 11:24

**「Background」** Daraxonrasib is an oral RAS\(ON\) multi-selective inhibitor that targets active-state RAS across multiple KRAS/NRAS mutations rather than a single G12C alteration. The FDA approved it on August 26, 2026, under the brand name RASONQUE for adults with previously treated metastatic pancreatic adenocarcinoma, based on the phase III RMC-302 trial, which reported median overall survival of 13.2 versus 6.7 months. The ENA 2026 report now covers first-line use combined with gemcitabine/nab-paclitaxel, a setting where the drug is not yet approved.

**「解读注意」** 化疗的历史参照为 1 年生存率 22%–48%（MPACT 试验 35%，mFOLFIRINOX 48%），因此不宜直接把单臂结果描述为“远高于化疗”。daraxonrasib 是口服 RAS\(ON\) 多选择性抑制剂，覆盖多种 KRAS/NRAS 突变，并非单一 G12C 靶向药；该药已于 8 月 26 日获 FDA 批准（商品名 RASONQUE）用于既往治疗后的患者，依据是 III 期 RMC-302 的中位总生存 13.2 个月对 6.7 个月。

<details><summary>References</summary>
<ul>
<li><a href="https://www.fda.gov/drugs/resources-information-approved-drugs/fda-approves-daraxonrasib-metastatic-pancreatic-adenocarcinoma">FDA approves daraxonrasib for metastatic pancreatic ...</a></li>
<li><a href="https://www.cancernetwork.com/view/how-significant-is-the-approval-of-daraxonrasib-in-pancreatic-cancer-">How Significant Is the Approval of Daraxonrasib in Pancreatic ...</a></li>

</ul>
</details>

**Tags**: `#biotech`, `#clinical-trials`, `#RAS-inhibitors`, `#pancreatic-cancer`, `#drug-development`

---

<a id="item-tech-news-9"></a>
### [Tesla begins overseas rollout of FSD v15](https://x.com/Tesla/status/2124222447855743019) ⭐️ 7.0/10

Tesla has started rolling out FSD v15 overseas, according to a brief repost of the company&\#x27;s announcement. The update adds a &quot;Tesla Reality View&quot; interface that overlays camera footage and the FSD driving plan on the in-car screen, with full-screen, map, and split-screen views plus a quiet mode. It also overlays navigation cues such as turns, softens and gradually fades the turn-signal chime, and adjusts driving for potholes and debris and speed control near schools and in bad weather. The post claims safety-critical scenario handling improved 25-fold, but the source gives no basis for that figure and no independent verification.

telegram · zaihuapd · Nov 22, 00:03

**「Background」** Tesla&\#x27;s FSD software has been distributed as over-the-air updates to its customer fleet, with each version adding driving-behavior and interface changes. The v15 release described here follows that pattern, pairing claimed safety-scenario improvements with a new in-car visualization layer called Tesla Reality View. The source does not specify which countries or vehicle models receive the overseas rollout, so the scope of availability remains unclear.

**Tags**: `#autonomous driving`, `#Tesla FSD`, `#AI systems`, `#software release`, `#computer vision`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Good Programming Is About Avoiding Blunders](https://seangoedecke.com/to-code-well-avoid-blunders/) ⭐️ 5.0/10

rss · Sean Goedecke · Nov 22, 00:00

**「Background」** Engineers often equate good programming with brilliant insights and elegant new abstractions, but Sean Goedecke argues this framing misses the main thing. Drawing on chess and tennis, he suggests that in domains where a single catastrophic error can erase any accumulated advantage, avoiding blunders matters more than producing moments of brilliance.

**「Solution」** Goedecke&\#x27;s central claim is that programming, unlike basketball, offers no durable winning advantage: one blunder can turn an elegant codebase into a janky one. He lists representative blunders—introducing a parallel system for the same task, creating a second source of truth, converting a safe sync operation into a delicate async one, adding subtle failure points, and complicating a key interface—and reduces them to two cardinal sins: inconsistency and unnecessary requirements. Inconsistency is dangerous because it breaks trust, forcing engineers to hunt for surprises instead of assuming sensible behavior. Unnecessary requirements are dangerous for two reasons: they are sticky, since a reader must assume an existing requirement is necessary unless willing to research it, and they interact combinatorially, so every new feature must be checked against every existing one. The practical prescription is to fit each task as normally as possible into the current codebase and trim it to the smallest set of requirements, treating clever-pattern impulses as a warning sign of distraction. Goedecke notes this advice targets large commercial codebases with big teams, and adds that current coding agents are roughly human-level at consistency but far worse at avoiding unnecessary requirements.

**「Takeaway」** Goedecke concludes that great programming does not require cleverness—and that cleverness can even be a disadvantage—because the dominant failure modes in large codebases are inconsistency and unnecessary requirements. Attention to detail and a laser focus on avoiding blunders, rather than discovering beautiful abstractions, are what carry the work.

**Tags**: `#software engineering practice`, `#codebase maintainability`, `#technical debt`, `#engineering judgment`, `#opinion essay`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China Uses APEC Summit to Expand Global Diplomatic Role](https://www.cnbc.com/2026/11/21/china-xi-trump-putin-global-diplomacy-shenzhen.html) ⭐️ 7.0/10

U.S. President Donald Trump met Chinese President Xi Jinping and Russian President Vladimir Putin together in Shenzhen on Thursday, the first in-person trilateral meeting of the three leaders, held around the APEC summit China hosted there. At the meeting, Xi announced $20 million in support for the Asia-Pacific region, according to CNBC.

rss · CNBC Finance · Nov 21, 06:00

**「Background」** China has increasingly hosted multilateral forums, including brokering the restoration of Saudi-Iranian ties in 2023, and Xi has hosted more than 40 heads of state this year, CNBC reported, citing official Chinese readouts.

**「Impact」** The summit gives China a platform to pursue trade, investment and technology cooperation with other economies, though analysts cited by CNBC note that diverging national priorities make consensus harder to reach.

**Tags**: `#China`, `#geopolitics`, `#APEC`, `#diplomacy`, `#trade`

---

<a id="item-finance-news-2"></a>
### [Trump Says U.S. Firms Building AI Data Centers Abroad Could Face &\#x27;Huge Taxes&\#x27;](https://apnews.com/article/trump-artificial-intelligence-data-centers-f1ac03b73d13445400eeed8631d9d879) ⭐️ 7.0/10

At a White House press conference on November 20, President Trump said he may impose &quot;huge taxes&quot; on U.S. tech companies that build AI data centers overseas, a plan he said he has not yet shared with officials inside his administration. He said the goal is to keep data centers in the U.S. and preserve AI competitiveness with China; no rate, legal mechanism, or timeline has been announced.

telegram · zaihuapd · Nov 21, 03:26

**「Background」** Trump has framed the threat as part of the U.S.-China race for AI leadership, saying Washington and Beijing remain locked in heated competition for supremacy in the industry. He has not released any tax rate, legislative text, or timeline, and said he had not yet told officials inside his own government about the plan.

**「Potential impact」** If enacted, the tax threat would directly affect U.S. tech companies planning AI data centers abroad, though no rate, scope, or legislative path has been specified. Separately, Trump&\#x27;s call for communities to negotiate payments with developers addresses local opposition driven by concerns over electricity demand and noise.

<details><summary>References</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/11/20/trump-overseas-data-center-tax-01178999">Trump says he’ll tax companies building data centers outside US</a></li>
<li><a href="https://www.thefiscaltimes.com/2026/11/20/Trump-Defends-Data-Centers-Threatens-Tax-Companies-Build-Them-Outside-US">Trump Defends Data Centers, Threatens to Tax Companies That ...</a></li>
<li><a href="https://ainewsglobal.online/data-center-anxiety-community-pushback-ai/">Data Center Anxiety: Why Communities Are Fighting Back</a></li>
<li><a href="https://successquarterly.com/data-center-boom-faces-community-opposition/">Data Center Boom Faces Community Opposition - SUCCESS...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#tax policy`, `#US-China tech competition`, `#data centers`, `#technology regulation`

---