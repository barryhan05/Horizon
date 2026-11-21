---
layout: default
title: "Horizon Summary: 2026-11-21 (EN)"
date: 2026-11-21
lang: en
---

> From 39 items, 18 important content pieces were selected

---

**Technology News**
1. [Levent Alpöge Claims Proof of Generalized Riemann Hypothesis](#item-tech-news-1) ⭐️ 9.0/10
2. [GitHub Repo Claims Finite-Time Blow-Up for Unforced Navier–Stokes](#item-tech-news-2) ⭐️ 9.0/10
3. [Tao Post Reportedly Links Unforced Navier-Stokes Singularity to GRH](#item-tech-news-3) ⭐️ 9.0/10
4. [Levent Alpöge Claims Claude-Assisted Riemann Hypothesis Proof](#item-tech-news-4) ⭐️ 9.0/10
5. [Vakil Announces Proposed Proof of Generalized Riemann Hypothesis](#item-tech-news-5) ⭐️ 8.0/10
6. [KVM flaw lets VMs read AMD host memory](#item-tech-news-6) ⭐️ 8.0/10
7. [TSMC Pauses 16nm and Below Orders for Chinese Firms](#item-tech-news-7) ⭐️ 8.0/10
8. [Inkling 2 Mini: Open-Weights Looped Transformer Draws Local Inference Reports](#item-tech-news-8) ⭐️ 7.0/10
9. [Paper Claims Language Models Can Rewrite Their Own Weights](#item-tech-news-9) ⭐️ 7.0/10
10. [Signal Moves to Block AI Agents From Capturing Mobile Data](#item-tech-news-10) ⭐️ 7.0/10
11. [Aaronson Blog Post and HN Debate Ask Whether LLMs Can Do Real Math](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI adds async background mode with 2h/8h windows and token discounts](#item-tech-news-12) ⭐️ 7.0/10
13. [Cursor Weighs Phasing Out Chinese Open-Weight AI Models](#item-tech-news-13) ⭐️ 7.0/10
14. [OpenAI 加强反蒸馏防护，称提取成功率降至 0.2%](#item-tech-news-14) ⭐️ 7.0/10

**Technology Blog**
1. [Why Caching LLM Outputs Barely Saves Tokens](#item-tech-blog-1) ⭐️ 6.0/10

**Financial News**
1. [Fed Officials Speak More as Warsh Stays Quiet on Rate Path](#item-finance-news-1) ⭐️ 7.0/10
2. [US Tightens Chip Exports as India Expands AI Capacity](#item-finance-news-2) ⭐️ 7.0/10
3. [特朗普提议对海外建AI数据中心的美国公司征收“巨额税款”](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Levent Alpöge Claims Proof of Generalized Riemann Hypothesis](https://alpo.ge/remark.pdf) ⭐️ 9.0/10

Levent Alpöge has posted a PDF at alpo.ge/remark.pdf claiming a proof of the Generalized Riemann Hypothesis, reportedly accompanied by a Lean formalization of roughly 1.3GB and about 15 million lines of code. The claim is unverified: the item is an announcement plus community discussion, not a peer-reviewed or independently checked result. Commenters also point to a separate, apparently fully human proof posted the same day on a math blog, and to an earlier related announcement from two days before.

hackernews · iamronaldo · Nov 20, 14:16 · [Discussion](https://news.ycombinator.com/item?id=50574968)

**「Context」** Levent Alpöge is a Turkish-American number theorist known for work in arithmetic statistics who later joined Anthropic as a member of its technical staff, according to Wikipedia. Reports describe the claim as a Riemann hypothesis proof produced with the AI model Claude and released only as Lean code rather than a conventional paper, with the note stating the formalization is finished. A commenter also points to a separate, human-authored announcement of a Generalized Riemann Hypothesis proof, indicating the claim is being weighed alongside other recent work.

**「Impact」** If the formalization holds up, the practical consequence is that the proof&\#x27;s correctness could be checked by machine rather than by years of expert review, though the 1.3GB, ~15-million-line artifact is large enough that independent verification would itself be a substantial undertaking. Until then, mathematicians and formal-verification practitioners should treat both the GRH claim and the Lean build as unconfirmed.

**「Community Discussion」** Commenters focused on the scale of the artifact, with one posting commands to download and unpack the 14-part Lean archive and reporting its size and line counts. Others linked a same-day human proof on math216.wordpress.com and an earlier related announcement, while one commenter framed the news as a possible turning point and raised concerns about AI-driven pace and calls for a pause.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>
<li><a href="https://www.nacionale.com/en/articles/has-riemann-hypothesis-been-proved-levent-alpoge-claude-anthropic-claim-lean">Riemann hypothesis proof claimed with Claude, unverified</a></li>
<li><a href="https://clashreport.com/world/articles/anthropic-mathematician-claims-claude-helped-prove-riemann-hypothesis-opkw9bqkqhh">Riemann Hypothesis : Anthropic’s Alpöge Claims Proof Made With...</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#Lean`, `#formal-verification`, `#theorem-proving`, `#research`

---

<a id="item-tech-news-2"></a>
### [GitHub Repo Claims Finite-Time Blow-Up for Unforced Navier–Stokes](https://github.com/tristanbuckmaster/navier-stokes/) ⭐️ 9.0/10

A GitHub repository attributed to Tristan Buckmaster claims a finite-time blow-up result for the unforced Navier–Stokes equations, and the claim drew substantial Hacker News discussion. The supplied material contains no paper, proof outline, or technical detail, so the result&\#x27;s validity and scope cannot be assessed from the available evidence. Commenters describe it as the unforced counterpart to an earlier forced-equation example they attribute to OpenAI, but that comparison is community characterization rather than verified fact.

hackernews · trotro · Nov 20, 15:34 · [Discussion](https://news.ycombinator.com/item?id=50576232)

**「Background」** The Navier–Stokes existence and smoothness problem is one of the Clay Mathematics Institute&\#x27;s Millennium Prize Problems, asking whether smooth initial data in three dimensions can develop a singularity in finite time. The repository&\#x27;s claim concerns the unforced equations, distinguishing it from a reported result involving a carefully designed external forcing term. Community discussion also references a separate finite-time blow-up result for the inviscid Boussinesq system with smooth forcing, attributed to Buckmaster and Alpöge.

**「Impact」** If the claim holds, it would bear directly on the Navier–Stokes existence and smoothness problem, which asks whether smooth solutions in three dimensions can develop singularities from smooth initial data. Until a proof is available for independent review, researchers should treat the repository as an unverified claim rather than an established result.

**「Community Discussion」** Commenters debated how the result relates to prior work: tancop said this is the unforced version, while an earlier example used a carefully designed external force, making this one more &quot;realistic&quot; in their view. Others, including ninkendo and Ericson2314, asked whether a simulation could show the blow-up in real time or a physical demonstration could reproduce it, questions that the supplied comments leave unanswered.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_priority_controversy">Navier – Stokes priority controversy - Wikipedia</a></li>
<li><a href="https://www.unite.ai/buckmaster-and-alpoge-post-ai-fluid-blowup-proofs-dispute-openai-contact/">Buckmaster and Alpöge Post AI Fluid Blowup Proofs, Detail OpenAI...</a></li>

</ul>
</details>

**Tags**: `#navier-stokes`, `#mathematics`, `#fluid-dynamics`, `#research`, `#scientific-computing`

---

<a id="item-tech-news-3"></a>
### [Tao Post Reportedly Links Unforced Navier-Stokes Singularity to GRH](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 9.0/10

A Terry Tao blog post dated November 20, 2026 reportedly presents results on an unforced Navier-Stokes singularity and the Generalized Riemann Hypothesis. The supplied evidence is limited to the post&\#x27;s title, URL, and Hacker News comments, so the mathematical claims themselves cannot be independently confirmed here. Commenters say two independent Lean kernels accepted the proof, which they read as evidence against kernel-bug exploitation rather than as external mathematical verification. The post is also described as drawing on the Langlands program and arithmetic geometry, but no source text is available to substantiate that characterization.

hackernews · archon1410 · Nov 20, 17:21 · [Discussion](https://news.ycombinator.com/item?id=50578358)

**「Background」** The Navier–Stokes existence and smoothness problem asks whether smooth solutions to the incompressible Navier–Stokes equations can develop singularities in finite time; a 2016 result by Terence Tao addressed a related averaged version, and a 2026 blowup result was disputed by Alpöge and Buckmaster and could not be extended to the unforced case, according to Wikipedia. The same day&\#x27;s TechCrunch report says Alpöge and Buckmaster also released a separate Navier–Stokes-related proof amid a race between frontier labs and mathematicians over outstanding problems. The item&\#x27;s own title links the unforced singularity question to the Generalized Riemann Hypothesis, but the supplied evidence does not establish the content or status of those claims.

**「Impact」** If the reported Lean acceptance holds, the result would shift scrutiny from whether a proof exists to whether its formal statement matches the intended theorem, since kernel acceptance checks derivation, not the faithfulness of the formalization. Readers evaluating the claim should look for the formal statement and its assumptions rather than treating kernel acceptance alone as confirmation of the mathematical result.

**「Community Discussion」** Commenters reported that two independent Lean kernels accept the result, which one described as making kernel-bug exploitation unlikely. Others debated whether AI-assisted proof generation can produce genuinely new abstractions rather than recombine existing ones, and several commenters described feeling both excited and uneasy about the implications for research careers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_existence_and_smoothness">Navier – Stokes existence and smoothness - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/11/20/ai-claimed-a-solution-to-the-167-year-old-riemann-hypothesis-and-a-human-did-too/">AI claimed a solution to the 167-year-old Riemann Hypothesis — and...</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#Navier-Stokes`, `#Riemann Hypothesis`, `#formal verification`, `#AI for science`

---

<a id="item-tech-news-4"></a>
### [Levent Alpöge Claims Claude-Assisted Riemann Hypothesis Proof](https://simonwillison.net/2026/Nov/20/levent-alpoge/) ⭐️ 9.0/10

In a PDF posted at alpo.ge/remark.pdf and quoted by Simon Willison, mathematician Levent Alpöge states that he believes he has, working with Claude, discovered a proof of the Riemann Hypothesis, and that the method extends to the Generalized Riemann Hypothesis, with the Extended Riemann Hypothesis expected given more time. Alpöge also says he and Claude formalized the arguments without assumptions. The supplied material contains only the quoted claim and a link to the PDF, with no independent verification, peer review, or technical detail, so the result&\#x27;s validity remains unconfirmed.

rss · Simon Willison · Nov 20, 16:30

**「Background」** The Riemann Hypothesis is one of mathematics&\#x27; best-known unsolved problems, and the Generalized and Extended Riemann Hypotheses extend its claims to broader classes of functions. Levent Alpöge is described in press coverage as a mathematician and employee at Anthropic, the company behind Claude, which contextualizes why an AI-assisted claim would draw attention.

**「Impact」** Because the claim has not been independently checked, readers should treat it as an unverified assertion rather than an established result; anyone assessing it would need to examine the linked PDF and the claimed formalization directly.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">Anthropic mathematician claims to prove Riemann hypothesis ...</a></li>
<li><a href="https://futurism.com/artificial-intelligence/anthropic-riemann-hypothesis">Anthropic Mathematician Claims He’s Solved the Riemann ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mathematics`, `#Anthropic`, `#research`, `#formal-verification`

---

<a id="item-tech-news-5"></a>
### [Vakil Announces Proposed Proof of Generalized Riemann Hypothesis](https://simonwillison.net/2026/Nov/20/ravi-vakil/) ⭐️ 8.0/10

Ravi Vakil announced on his blog that Alessandro Masullo has a proposed proof of the Generalized Riemann Hypothesis, which Brian Conrad has been reviewing closely for months and has given extensive feedback on, with Vakil saying it is &quot;so far looking good.&quot; Vakil said the plan had been to bring Masullo to Stanford for a year to polish the writing and run it by enough people before announcing, but that it now seems best to release the current draft early. Vakil explicitly stated the work is &quot;all human, with no AI.&quot; The proof is unverified and the announcement provides no technical detail.

rss · Simon Willison · Nov 20, 19:21

**「Background」** The Riemann hypothesis is one of mathematics&\#x27; most important open conjectures, a statement about the zeros of the Riemann zeta function; the Generalized Riemann Hypothesis extends the claim to a broader class of L-functions. Brian Conrad, the reviewer Vakil cites, is a Stanford number theorist. According to Scientific American, Vakil is president of the American Mathematical Society, and the same report describes Masullo as a young mathematician at Stanford.

**「Impact」** Because the proof is an unreviewed draft, mathematicians should treat it as a claim to examine rather than an established result; Vakil&\#x27;s note says Brian Conrad has reviewed it for months and that feedback is still being incorporated. If it holds, GRH would make results that currently depend on it unconditional, such as deterministic polynomial-time primality testing, according to a secondary commentary source.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis">Generalized Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://www.scientificamerican.com/article/dueling-claims-of-riemann-hypothesis-proofs-emerge/">Dueling claims of Riemann hypothesis proofs ... | Scientific American</a></li>
<li><a href="https://en.wikipedia.org/wiki/Brian_Conrad">Brian Conrad - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/pulse/7-consequences-riemann-hypothesis-narrative-frank-pkbgc">The 7 Consequences of the Riemann Hypothesis - A Narrative...</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#research`, `#proof-verification`, `#ai-and-mathematics`

---

<a id="item-tech-news-6"></a>
### [KVM flaw lets VMs read AMD host memory](https://thehackernews.com/2026/11/new-linux-kvm-flaw-cve-2026-99312-lets.html) ⭐️ 8.0/10

Linux kernel KVM contains CVE-2026-99312, a vulnerability that affects only AMD hosts with nested virtualization enabled. Researchers reported reading roughly 127 GB of host memory from inside a virtual machine on DigitalOcean. An upstream fix shipped on November 18 with stable kernel 7.3.5 and related releases, but distribution kernels such as Debian&\#x27;s and Ubuntu&\#x27;s had not yet been patched. Until those updates arrive, operators can mitigate by disabling nested virtualization.

telegram · zaihuapd · Nov 20, 14:23

**「Background」** KVM is the hypervisor built into the Linux kernel, and nested virtualization lets a guest VM itself run hypervisors, a configuration that expands the code paths a guest can exercise. According to Terra Security&\#x27;s research write-up, the flaw sat in the kernel for just under four years and was introduced by an earlier security fix, with a stale pointer allowing access to host memory. DigitalOcean&\#x27;s disclosure describes the same stale-pointer mechanism and lists the patched kernels and mitigations.

**「Impact」** Operators running AMD hosts with nested virtualization enabled should treat guest workloads as potentially able to read host memory, which can expose data belonging to other tenants or the host itself. Because the upstream fix is not yet in Debian and Ubuntu kernels, affected deployments need either a patched kernel or nested virtualization turned off until distribution updates land.

<details><summary>References</summary>
<ul>
<li><a href="https://www.terra.security/blog/kvm-guest-to-host-escape">KVM Guest-to- Host Escape | Terra Security Research</a></li>
<li><a href="https://www.digitalocean.com/blog/cve-2026-99312-kvm-patch">Virtualization , Responsible Disclosure, and CVE - 2026 - 99312</a></li>

</ul>
</details>

**Tags**: `#linux-kvm`, `#vulnerability`, `#virtualization`, `#amd`, `#kernel-security`

---

<a id="item-tech-news-7"></a>
### [TSMC Pauses 16nm and Below Orders for Chinese Firms](https://appleinsider.com/articles/26/11/20/apple-supplier-tsmc-cuts-off-china-chip-orders-amid-tighter-export-controls) ⭐️ 8.0/10

TSMC has reportedly notified customers that it is pausing orders from Chinese companies for advanced processes at 16nm and below. Under tightened US semiconductor export rules, TSMC may not supply these nodes without prior US export approval or an exemption, and the company must now require customers to apply in advance rather than assessing exemption eligibility itself. Chinese firms are consequently pushed to older 28nm and 40nm processes and cannot access the high-bandwidth memory needed for AI data centers. The US approved list reportedly includes Apple, AMD, and Nvidia but no Chinese companies; TSMC said it will comply with the new rules. The account comes from a brief secondary summary, and details such as the approved-list specifics warrant verification against primary sources.

telegram · zaihuapd · Nov 21, 02:01

**「背景」** 此前，台积电可以自行评估中国客户的设计是否符合美国出口豁免条件；收紧后的规则将这一判断改为由客户事先申请美国许可或豁免。据路透社报道，新规旨在堵住一个制造环节的漏洞，而美国批准的芯片设计商名单包括英伟达、AMD、苹果，以及台湾的联发科和瑞昱。TrendForce 也报道称，三星同样暂停了部分面向中国的消费级芯片出货，并指出冗长的审批流程可能打乱生产计划。

**「Impact」** Chinese chip designers relying on TSMC for 16nm-and-below production face a shift to 28nm and 40nm processes or the need to secure US approval before orders can proceed, which affects access to advanced nodes and HBM for AI data-center work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.trendforce.com/news/2026/11/20/news-tsmc-samsung-reportedly-pause-china-consumer-chip-shipments-under-new-u-s-rules-16nm-orders-affected/">[News] TSMC, Samsung Reportedly Pause China Consumer Chip ...</a></li>
<li><a href="https://www.reuters.com/world/china/tsmc-tightens-china-ai-chip-curbs-new-us-rules-close-manufacturing-loophole-2026-11-19/">TSMC tightens China AI chip curbs as new US rules close ...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export-controls`, `#TSMC`, `#AI-hardware`, `#supply-chain`

---

<a id="item-tech-news-8"></a>
### [Inkling 2 Mini: Open-Weights Looped Transformer Draws Local Inference Reports](https://thinkingmachines.ai/news/inkling-2-mini/) ⭐️ 7.0/10

Thinking Machines released an open-weights model called Inkling 2 Mini that uses a looped transformer architecture, according to the company&\#x27;s announcement discussed on Hacker News. The supplied evidence is limited to the title and community comments, so the model&\#x27;s benchmark claims remain unverified; commenters compare it to Qwen3.8-27B and describe it as promising in quick coding tests. Local users report roughly 27 tokens/s decode on a Ryzen 395 with llama.cpp Vulkan and about 10 tokens/s on a 32GB M1 Pro MacBook at q4, with one commenter noting unmerged llama.cpp pull requests \(32694, 32657, 32429, 32704\) plus a small patch for an additional speed boost. A GGUF build for Ollama/llama.cpp is also referenced.

hackernews · jasondavies · Nov 20, 20:12 · [Discussion](https://news.ycombinator.com/item?id=50581260)

**「Background」** Inkling 2 Mini is an open-weights model from Thinking Machines Lab, published with a 26B-parameter image-text-to-text checkpoint on Hugging Face. Its distinguishing design is a looped transformer: the model reuses its middle layers to reason more per token and reach answers in fewer tokens, rather than adding depth through new layers. That architecture is what makes the local-inference reports and llama.cpp patches in the discussion relevant, since running it requires tooling support for the looped structure.

**「Impact」** Users who want to run the model locally should expect to apply pending llama.cpp patches and may see uneven quality: one commenter reported strong Python code generation but a failure on a coin-identification test after roughly 12,000 tokens of output. Reported throughput varies widely by hardware, from about 10 tokens/s on an M1 Pro to about 27 tokens/s on a Ryzen 395.

**「Community Discussion」** Commenters debated the significance of an open-weights looped transformer, with one arguing that most open models may adopt the architecture and raising questions about safety and interpretability at this level of availability. Others focused on practical local results, sharing hardware-specific token rates and llama.cpp patches, while cautioning that the benchmark comparisons depend on whether the numbers hold up in real-world use.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://huggingface.co/thinkingmachines/Inkling-2-Mini">thinkingmachines/Inkling-2-Mini - Hugging Face</a></li>

</ul>
</details>

**Tags**: `#open-weights models`, `#looped transformers`, `#local inference`, `#llama.cpp`, `#model architecture`

---

<a id="item-tech-news-9"></a>
### [Paper Claims Language Models Can Rewrite Their Own Weights](https://arxiv.org/abs/2611.21885) ⭐️ 7.0/10

An arXiv paper \(2611.21885\) claims a language model can rewrite its own weights through its own reasoning, with no gradients and no training, testing edits on practice problems and submitting only those that work. The supplied evidence is limited to the title, URL, and community comments, so the paper&\#x27;s methods and measured results cannot be independently assessed here. Commenters report that the only self-improvement observed was shortening reasoning traces to avoid token limits, and question whether the process amounts to training under another name.

hackernews · lwhsiao · Nov 20, 16:29 · [Discussion](https://news.ycombinator.com/item?id=50577265)

**「Background」** The claim builds on recent work on models modifying weights directly rather than through conventional training. Google&\#x27;s SLEEP framework, described in an October 2026 research post, has a deployed model update its numerical weights during an offline phase using self-generated practice examples, while keeping its core codebase unchanged. Separately, a weight-space programming write-up argues that a model able to inspect, debug, and improve its own weights offers a more native path to recursive self-improvement than writing code that launches training jobs.

**「Community Discussion」** Commenters questioned the novelty and framing: aesthesia said the only modification the model made was reducing reasoning-trace length to avoid the token limit, likening it to a recent weight-space programming article, while gavinray pointed to Google&\#x27;s SLEEP framework, which updates numerical weights using self-generated practice examples during an offline phase. Toutouxc argued the described process—testing edits on practice problems and keeping only what works—sounds a lot like training, and LarsDu88 raised a safety concern that an autonomous model could direct itself to suppress safety-relevant activations.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/the-sleep-framework-a-new-way-for-llms-to-retain-knowledge-in-continual-learning/">The sleep framework: A new way for LLMs to retain knowledge ...</a></li>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight - Space Programming : LLMs can natively read...</a></li>

</ul>
</details>

**Tags**: `#language-models`, `#self-modification`, `#ai-safety`, `#research`, `#machine-learning`

---

<a id="item-tech-news-10"></a>
### [Signal Moves to Block AI Agents From Capturing Mobile Data](https://signal.org/blog/protecting-your-privacy/) ⭐️ 7.0/10

Signal published a blog post describing its efforts to prevent AI agents on mobile operating systems from capturing user data, and says it is &quot;cautiously optimistic&quot; about progress, according to a commenter&\#x27;s paraphrase of the post. The supplied excerpt contains no technical specifics on the mechanisms, versions, or platform conditions involved, so the concrete scope of what Signal has shipped versus what it is still pursuing is not established here. The post drew a large Hacker News discussion \(310 comments\) focused on OS-level control, transparency, and gaps in Signal&\#x27;s own privacy posture.

hackernews · dotcoma · Nov 20, 09:42 · [Discussion](https://news.ycombinator.com/item?id=50572348)

**「Background」** Signal&\#x27;s post frames the issue as OS-level AI agents that can read data from other apps, which the company says undermines protections independent developers build at the application layer. Coverage of the post describes Signal rolling out screenshot blocks alongside its warning about agents such as Meta&\#x27;s Muse, so the restriction is presented as a defensive measure against platform capabilities rather than a new messaging feature.

**「Impact」** Commenters point to a structural limit on the approach: even users who install no AI app can have their Signal chats exposed through a contact&\#x27;s device, as Meredith Whittaker reportedly described in a Machine Gods interview. One commenter argues that relying on an app to block screenshots will not hold up long term and that users need control at the operating-system level, while another asks Signal to publish its forensics findings so smaller app developers can reuse them.

**「Community Discussion」** Several commenters questioned Signal&\#x27;s broader privacy record rather than the AI-agent work itself: one reported that adding a contact over a VPN triggers repeated captchas, arguing this forces users such as journalists and sources to reveal their IP addresses, and another complained that screenshot blocking now extends to Signal chats on Windows. Others welcomed the direction, with one calling for Signal to warn users about spyware-like systems and recommend alternatives such as GrapheneOS or Linux.

<details><summary>References</summary>
<ul>
<li><a href="https://signal.org/blog/protecting-your-privacy/">Signal &gt;&gt; Blog &gt;&gt; Signal is Serious About Protecting...</a></li>
<li><a href="https://www.inc.com/aaron-mok/signal-blocks-screenshots-ai-agents-privacy/91440348">Signal Blocks Screenshots Over AI Agent Risks - Inc.com</a></li>
<li><a href="https://gizmodo.com/signal-is-fighting-to-keep-ai-agents-out-of-your-private-messages-2000843160">Signal Is Fighting to Keep AI Agents Out of Your ... - Gizmodo</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#mobile-security`, `#ai-agents`, `#signal`, `#operating-systems`

---

<a id="item-tech-news-11"></a>
### [Aaronson Blog Post and HN Debate Ask Whether LLMs Can Do Real Math](https://scottaaronson.blog/?p=10344) ⭐️ 7.0/10

A Scott Aaronson blog post, discussed on Hacker News, probes whether LLM-style systems can produce meaningful mathematical results and what that would imply for human understanding and interpretability. The item is commentary and analysis rather than a reported technical breakthrough; the supplied evidence is limited to the post&\#x27;s title and a handful of comments, so no specific mathematical claim is established. Commenters drew an analogy to computer chess, where engine evaluations are explanations only in the sense of aggregated calculations stacked on a neural evaluator.

hackernews · stratos123 · Nov 20, 20:03 · [Discussion](https://news.ycombinator.com/item?id=50581084)

**「Background」** The &quot;stochastic parrot&quot; label comes from a 2021 critique of large language models, and Aaronson&\#x27;s post responds to social-media claims that systems so described have now proved the Riemann Hypothesis. The post itself frames the situation as an apparent AI-assisted proof rather than a verified result, and the Hacker News thread discusses it as commentary on AI reasoning and interpretability rather than a primary technical announcement.

**「Community Discussion」** One commenter argued that chess engines left people in an unsatisfying position: Stockfish&\#x27;s evaluation is an &quot;explanation&quot; only as an aggregate of calculations built atop a neural evaluator, which does not answer &quot;why&quot; questions intuitively. Another commenter asked whether humans can accept becoming progressively worse at understanding scientific and engineering results, while a third wondered how many mathematicians could reach similar breakthroughs given near-infinite compute.

<details><summary>References</summary>
<ul>
<li><a href="https://scottaaronson.blog/?p=10344">Shtetl-Optimized » Blog Archive » The stochastic parrots have ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50581084">The stochastic parrots have apparently proved the Riemann ...</a></li>
<li><a href="https://cho.sh/mini/news/ai-2/riemann-hypothesis-ai-proof">Aaronson&#x27;s blog post on an apparent AI-assisted Riemann ...</a></li>

</ul>
</details>

**Tags**: `#AI reasoning`, `#interpretability`, `#mathematics`, `#LLMs`, `#epistemology`

---

<a id="item-tech-news-12"></a>
### [OpenAI adds async background mode with 2h/8h windows and token discounts](https://developers.openai.com/api/docs/guides/background) ⭐️ 7.0/10

OpenAI has reportedly introduced a background mode that moves long-running API requests to asynchronous execution: developers set \`background: true\` and choose a completion window of 2h or 8h via \`background\_options.completion\_window\`, with token rates 30% and 40% below standard pricing respectively. Leaving the option unset uses a default &quot;soonest&quot; mode with no discount. The discount is in public beta on GPT-6.2 Astra, GPT-6.2 Sol, GPT-6.1 Terra and GPT-6 Luna, according to the secondary-source summary. The same summary notes that background mode temporarily stores response data even when \`store\` is set to false or zero data retention is enabled.

telegram · zaihuapd · Nov 20, 11:15

**「Background」** OpenAI&\#x27;s Responses API normally handles a request synchronously: the app sends input and waits for the final output on the same connection, which makes long-running jobs vulnerable to timeouts. Background mode instead starts the task asynchronously and lets developers poll the response object for status, as OpenAI&\#x27;s API documentation describes. The new completion-window options and token discounts build on that asynchronous mechanism.

**「Data-retention caveat for ZDR users」** Developers who rely on \`store: false\` or Zero Data Retention should note that background mode still temporarily stores response data, encrypted at rest, to run the request and make results retrievable; OpenAI&\#x27;s data-controls documentation states that projects with ZDR can use the 2h and 8h windows. Teams with strict no-retention requirements should confirm this temporary storage fits their compliance posture before routing long-running workloads through background mode.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/background">Background mode | OpenAI API</a></li>
<li><a href="https://kissapi.ai/blog/openai-background-mode-api-guide-2026.html">OpenAI Background Mode API : Run Long Tasks Without Timeouts...</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/background">Background mode | OpenAI API</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/your-data">Data controls in the OpenAI platform</a></li>

</ul>
</details>

**Tags**: `#openai`, `#api`, `#asynchronous-processing`, `#pricing`, `#data-retention`

---

<a id="item-tech-news-13"></a>
### [Cursor Weighs Phasing Out Chinese Open-Weight AI Models](https://www.cnbc.com/2026/11/20/cursor-chinese-ai-models-geopolitical-risk.html) ⭐️ 7.0/10

Cursor, the AI coding platform described in the item as SpaceX-owned, said it is considering phasing out Chinese-developed open-weight AI models because of &quot;geopolitical risk.&quot; The item states that Cursor&\#x27;s Composer 2 coding model is built on Moonshot AI&\#x27;s Kimi K2.5. The position follows a report from the US House Homeland Security Committee and the House Select Committee on China, which recommends a &quot;US national open-weight plan&quot; and would extend an executive order barring DeepSeek from federal systems to prohibit federal use of Chinese-developed AI models. The item does not specify a timeline, which models would be affected, or whether any phase-out has begun.

telegram · zaihuapd · Nov 20, 16:13

**「Background」** Cursor&\#x27;s Composer 2 coding model was built on Moonshot AI&\#x27;s open-weight Kimi K2.5, a dependency that became public after an independent developer identified the base model through code and API analysis, and Cursor subsequently acknowledged it. The congressional report cited in the item follows a joint investigation by the House Select Committee on China and the House Committee on Homeland Security into Chinese open-weight models in U.S. consumer platforms; it builds on the October 2026 DHS order barring DeepSeek from federal civilian IT systems.

**「Impact」** If Cursor proceeds, developers relying on Composer 2 would face a change in the model underlying the tool, and the item gives no indication of a replacement or migration path. The congressional recommendation targets federal systems, while Cursor&\#x27;s consideration is a separate vendor decision, so the two should not be treated as the same restriction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.idlen.io/news/cursor-composer-2-kimi-moonshot-ai-chinese-model-scandal/">Cursor and Kimi : Composer 2 Was Built on a Hidden Chinese Model</a></li>
<li><a href="https://www.linkedin.com/posts/dataconomy-media_cursor-admits-composer-2-based-on-moonshot-activity-7441789642393247744-x273">Cursor admits Composer 2 based on Moonshot AI’s Kimi ...</a></li>
<li><a href="https://chinaselectcommittee.house.gov/media/reports/joint-investigation-report-china-is-trying-to-get-us-companies-addicted-to-chinese-ai-models">Joint Investigation Report: China is Trying to Get U.S ...</a></li>
<li><a href="https://chinaselectcommittee.house.gov/media/press-releases/dhs-blocks-china-based-deepseek-from-federal-it-systems">DHS Blocks China-Based DeepSeek From Federal IT Systems</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open-weight models`, `#geopolitics`, `#developer tools`, `#open source`

---

<a id="item-tech-news-14"></a>
### [OpenAI 加强反蒸馏防护，称提取成功率降至 0.2%](https://openai.com/index/combatting-adversarial-distillation/) ⭐️ 7.0/10

OpenAI 于 11 月 20 日发布文章，介绍针对“对抗性蒸馏”的防御措施，称 GPT-6.2 Astra 与 Sol 已加强对推理链的保护。OpenAI 表示，在其红队测试中，提取历史请求推理的成功率从 54.0% 降至 0.2%。OpenAI 还称，今年每周对数千至数万个蒸馏账号采取执法，并曾就 DeepSeek 疑似蒸馏行为向国会汇报。上述数字均为 OpenAI 自述，所涉具体模型版本与执法规模无法从现有材料独立核实。

telegram · zaihuapd · Nov 21, 01:30

**「Background」** Adversarial distillation is the practice of extracting a model&\#x27;s capabilities—here, its reasoning chains—by querying it and training on the outputs, which OpenAI says it addresses through a layered mix of training, safeguards, detection, and enforcement. OpenAI&\#x27;s post ties a model&\#x27;s protected reasoning to the conversation history that produced it in GPT-6.2 Astra and GPT-6.2 Sol, the two models named in the source. The 54.0% to 0.2% figure comes from OpenAI&\#x27;s own red-team testing, so it is a vendor-reported result rather than an independent measurement.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/combatting-adversarial-distillation/">Combatting adversarial distillation | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#model distillation`, `#OpenAI`, `#red teaming`, `#LLM`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Why Caching LLM Outputs Barely Saves Tokens](https://seangoedecke.com/why-output-caching-doesnt-work/) ⭐️ 6.0/10

rss · Sean Goedecke · Nov 21, 00:00

**「Background」** LLM inference economics already relies on caching inputs in the KV cache so the whole conversation history isn&\#x27;t recomputed each turn. The author asks whether outputs should be cached the same way, since agents visibly repeat code snippets, evidence docs, and sample outputs, and output tokens cost far more to generate than input tokens cost to ingest.

**「Solution」** The proposed fix is to train or prompt models to emit references like &quot;src/script.py:12-15&quot; instead of regurgitating content, with the harness expanding them transparently. But the author argues this only optimizes visible output, which he estimates at about 6% of output tokens based on his own agent histories; roughly 50% are reasoning tokens and 44% are tool calls. Applying Amdahl&\#x27;s law, even saving two-thirds of visible output yields only about 4% of total output tokens. He is only moderately confident that frontier models rarely repeat themselves in chain of thought, and notes tool calls may contain some repetition. Real savings must come from the invisible 94%, which depends on model intelligence: a model 5x more expensive per token but needing 6x fewer tokens can be cheaper overall. Better harnesses help, though he doubts much durable advantage there since everyone can copy each other.

**「Takeaway」** Output caching targets a small visible slice of token spend, so Amdahl&\#x27;s law caps its benefit; the larger lever is reducing invisible reasoning and tool-call tokens through smarter models.

**Tags**: `#LLM inference economics`, `#output caching`, `#token cost`, `#Amdahl&\#x27;s law`, `#AI agents`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed Officials Speak More as Warsh Stays Quiet on Rate Path](https://www.cnbc.com/2026/11/20/warsh-fed-forward-guidance-rate-hikes.html) ⭐️ 7.0/10

Federal Reserve officials have been speaking publicly more often than in any two-week stretch since the start of 2025, according to a Bank of America analysis, as new Chair Kevin Warsh declines to signal where rates are headed. Most officials favor raising rates soon, with some, including Governor Christopher Waller, raising the possibility of a half-percentage-point hike at the December meeting.

rss · CNBC Finance · Nov 20, 21:10

**「Background」** Warsh said in June 2026 that the Fed would move away from forecasting its future actions, and he has argued that forward guidance — telling markets in advance where rates are headed — is poorly suited to current conditions \(tool-1-2, tool-1-3\).

**「Market impact」** Traders are pricing a 100% chance of at least a quarter-point rate hike in December, according to CME Group&\#x27;s FedWatch, and Bank of America&\#x27;s Aditya Bhave warns the public back-and-forth is producing &quot;undue rates volatility&quot; in already turbulent times.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/mediacenter/files/FOMCpresconf20260617.pdf">Transcript of Chairman Warsh&#x27;s Press Conference -- June 17, 2026</a></li>
<li><a href="https://thehill.com/business/5929155-warsh-ends-fed-forecasts/">Federal Reserve shifts away from forward guidance under new ...</a></li>
<li><a href="https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool">FedWatch</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#forward guidance`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [US Tightens Chip Exports as India Expands AI Capacity](https://www.bloomberg.com/news/articles/2026-11-20/nvidia-scandal-fallout-india-ai-yotta-ambani-adani-am-intelligence-e2e-networks) ⭐️ 7.0/10

The US tightened exports of advanced chips to Malaysia, Thailand, and Singapore, and Indian AI firms see an opening to absorb the diverted demand. Yotta said it will add about 100,000 GPUs over the next year, roughly a 10% increase on India&\#x27;s current computing capacity, according to a brief report citing Bloomberg.

telegram · zaihuapd · Nov 20, 07:31

**「Background」** The new US rules require licenses to export, re-export, or transfer advanced AI chips to Malaysia, Singapore, Thailand, Indonesia, and Brazil, according to reports on the controls \(tool-1-2, tool-1-1\). India&\#x27;s Adani group has pledged $100 billion and Reliance $110 billion for AI infrastructure, per Hindustan Times \(tool-2-1\).

**「Impact」** India&\#x27;s stated buildout — Reliance&\#x27;s commitment of up to $110 billion and Adani&\#x27;s $100 billion for AI infrastructure — could draw data-center and chip demand toward India, though these are announced commitments rather than confirmed spending.

<details><summary>References</summary>
<ul>
<li><a href="https://techwireasia.com/2026/11/us-ai-chip-restrictions-malaysia-singapore/">US AI chip restrictions put Malaysia and Singapore data ...</a></li>
<li><a href="https://www.channelnewsasia.com/singapore/us-export-controls-ai-chips-6556831">Singapore assessing impact of new US chip export controls ...</a></li>
<li><a href="https://www.hindustantimes.com/opinion/todays-ai-infrastructure-could-be-toast-tomorrow-101793905721069.html">Today’s AI infrastructure could be toast tomorrow | Hindustan Times</a></li>

</ul>
</details>

**Tags**: `#semiconductor export controls`, `#India AI infrastructure`, `#data centers`, `#Nvidia`, `#US trade policy`

---

<a id="item-finance-news-3"></a>
### [特朗普提议对海外建AI数据中心的美国公司征收“巨额税款”](https://apnews.com/article/trump-artificial-intelligence-data-centers-f1ac03b73d13445400eeed8631d9d879) ⭐️ 7.0/10

特朗普11月20日在白宫记者会上表示，拟对在海外建设AI数据中心的美国科技公司征收“巨额税款”，称此举旨在把数据中心留在美国、保持对中国的AI竞争优势；他并称尚未向政府内部官员透露该计划。

telegram · zaihuapd · Nov 21, 03:26

**「Background」** Trump made the remarks at a White House press briefing on Nov. 20, after returning from a trip to China, and said the goal is to keep AI data centers in the U.S. rather than let China &quot;take&quot; them. The proposal comes as local opposition to data centers grows over their electricity and water use, higher utility bills and noise.

**「影响」** 若该提议落地，在海外布局AI算力的美国科技公司可能面临额外税负，而美国各地社区则被鼓励以谈判方式换取开发商付款，以缓解当地对用电和噪音的反对。

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/trump-artificial-intelligence-data-centers-f1ac03b73d13445400eeed8631d9d879">Trump plans to penalize US tech firms that build AI data ...</a></li>
<li><a href="https://www.usatoday.com/story/tech/nation-now/2026/11/20/trump-tax-ai-data-centers/92881622007/">Trump wants to tax US companies that build AI data centers abroad</a></li>
<li><a href="https://www.linkedin.com/posts/adriaanrainsobotha_a-new-gallup-poll-found-that-71-of-americans-activity-7484964265003634689-2eK0">71% of Americans Oppose Building AI Data Centers in Local ...</a></li>
<li><a href="https://time.com/article/2026/07/22/community-backlash-ai-data-centers/">Community Backlash to AI Data Centers Is Growing Across the U . S .</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#tax policy`, `#US tech companies`, `#data centers`, `#US-China competition`

---