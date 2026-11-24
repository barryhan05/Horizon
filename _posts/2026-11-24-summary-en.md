---
layout: default
title: "Horizon Summary: 2026-11-24 (EN)"
date: 2026-11-24
lang: en
---

> From 39 items, 16 important content pieces were selected

---

**Technology News**
1. [Anthropic 称 Claude 模型发现 VP≠VNP，并发布 Lean 4 证明](#item-tech-news-1) ⭐️ 9.0/10
2. [Ladybird Browser Enters Alpha With macOS and Linux Builds](#item-tech-news-2) ⭐️ 8.0/10
3. [Z.ai Releases GLM-5.4, Its First Loop Transformer for Coding](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia Board Reinstates Jensen Huang as CEO After Brief Ouster](#item-tech-news-4) ⭐️ 8.0/10
5. [Codex2api 疑似遭供应链投毒，3.1.10–3.1.12 版本受影响](#item-tech-news-5) ⭐️ 8.0/10
6. [ChatGPT Chat Page Adds GPT-6.2 Sol for Paid Users](#item-tech-news-6) ⭐️ 8.0/10
7. [NariQ ships sub-3-bit Qwen3.8-27B GGUF quants with a custom llama.cpp fork](#item-tech-news-7) ⭐️ 7.0/10
8. [Stalwart Claims Drop-In Exchange Replacement, Community Questions Outlook Fit](#item-tech-news-8) ⭐️ 7.0/10
9. [黎曼猜想「AI 证明」被指空转，作者承认代码满是垃圾](#item-tech-news-9) ⭐️ 7.0/10
10. [45,000 EU businesses urge Commission to open Apple browser case](#item-tech-news-10) ⭐️ 7.0/10
11. [新加坡总理黄循财承诺不让新加坡成为规避美国芯片管制的通道](#item-tech-news-11) ⭐️ 7.0/10

**Technology Blog**
1. [vLLM Day-0 Support for ERNIE 5.5 Flash Preview](#item-tech-blog-1) ⭐️ 6.0/10

**Financial News**
1. [New York Fed&\#x27;s Williams Says More Rate Work Needed to Reach 2% Inflation](#item-finance-news-1) ⭐️ 8.0/10
2. [AI Selloff Clouds Planned Listings by DeepSeek and Moonshot AI](#item-finance-news-2) ⭐️ 7.0/10
3. [Shanghai Adjusts Subway Fares for First Time in 21 Years](#item-finance-news-3) ⭐️ 7.0/10
4. [SpaceX 据报向 Anthropic 和 Google 出租算力，月入数十亿美元](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic 称 Claude 模型发现 VP≠VNP，并发布 Lean 4 证明](https://github.com/anthropics/formal-math/blob/main/vp-vnp/README.md) ⭐️ 9.0/10

Anthropic 于 11 月 24 日发布论文《VP ≠ VNP over every field》及 Lean 4 形式化证明，仓库称该结果由内部研究用 Claude 模型发现，论文与代码均由 AI 撰写。论文给出哈密顿圈多项式的超多项式算术电路下界，据此推出 VP 是 VNP 的真子类；若成立，即解决 Valiant 1979 年的代数复杂度猜想，但该结果仅针对算术电路，不涉及 P 与 NP。经三条标准公理审计与独立内核 nanoda 复核，除预留文件外无 sorry；但尚无人类数学家通读，Lean 无法确认形式化陈述与声称命题一致，附录 Q 列出出入，结果仍待独立审阅。

telegram · zaihuapd · Nov 24, 06:02

**「Background」** Valiant&\#x27;s 1979 conjecture is the algebraic analogue of P vs NP: it asks whether the class VP of polynomials computable by polynomial-size arithmetic circuits is strictly smaller than VNP, whose canonical complete problem is the permanent. The claim concerns arithmetic circuits only and does not address P vs NP. External coverage describes the release as a roughly 70-page paper plus about 324 Lean files, with the README stating that no human mathematician has checked the proof.

**「Impact」** Because the Lean 4 formalization has passed automated checks but no human mathematician has reviewed the paper or confirmed that the formal statements match the claimed theorem, the result should be treated as an unverified claim rather than an established resolution of Valiant&\#x27;s conjecture. Anyone relying on it for research or citation should wait for independent human review, particularly of the discrepancies listed in Appendix Q.

<details><summary>References</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/claude-proves-vp-not-vnp-valiant-conjecture">Claude claims to prove VP ≠ VNP in Valiant&#x27;s 47-year-old ...</a></li>
<li><a href="https://explainx.ai/blog/anthropic-claude-vp-vnp-valiant-lean-proof-claimed-vs-verified-2026">VP ≠ VNP Lean Proof: Claimed vs Verified (2026) - explainx.ai</a></li>
<li><a href="https://www.besthub.dev/articles/claude-proves-vp-vnp-ai-cracks-47-year-algebraic-p-vs-np-conjecture-2454d374b036">Claude Proves VP ≠ VNP: AI Cracks 47-Year Algebraic P vs NP ...</a></li>
<li><a href="https://casrai.org/news/anthropic-claude-authored-vp-vnp-proof-unverified-lean-2026">Claude-Authored VP ≠ VNP Proof Posted, Unchecked — CASRAI</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-publishes-claude-authored-vp-vnp-proof-unverified">Anthropic Publishes Claude-Authored VP ≠ VNP Proof ...</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/claude-proves-vp-not-vnp-valiant-conjecture">Claude claims to prove VP ≠ VNP in Valiant&#x27;s 47-year-old ...</a></li>

</ul>
</details>

**Tags**: `#complexity-theory`, `#formal-verification`, `#Lean 4`, `#AI-for-math`, `#Anthropic`

---

<a id="item-tech-news-2"></a>
### [Ladybird Browser Enters Alpha With macOS and Linux Builds](https://ladybird.org/posts/alpha/) ⭐️ 8.0/10

The independent Ladybird browser released its first alpha, letting users install prebuilt binaries on macOS and Linux instead of compiling from source. Ladybird implements most of its engine in-house—HTML parsing, CSS, layout, JavaScript, and WebAssembly—while relying on external components including HarfBuzz for text shaping, Skia for 2D graphics, ffmpeg for video, and SQLite. The project cautions that some sites will not work and the browser will sometimes crash, and it invites users to report broken sites from within the browser and to review crash reports before sending them. The alpha follows an October 2026 surge in development that the project attributes largely to AI coding agents.

hackernews · janvdberg · Nov 23, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50614249)

**「Background」** Ladybird is an independent browser built on its own engine rather than Blink, WebKit, or Gecko, and it has been developed for roughly four years before this alpha, according to coverage of the release. The project grew out of SerenityOS, whose from-scratch culture explains why Ladybird still reuses some SerenityOS libraries while relying on external components such as Skia, HarfBuzz, ffmpeg, and SQLite.

**「Impact」** Early testers report that many sites render correctly, but at least one complex case fails: Datasette Lite, which combines Pyodide with service workers and web workers, throws an error because \`navigator.serviceWorker.startMessages\` is unimplemented, and the source carries a FIXME annotation for it. Users evaluating the alpha should expect gaps in service-worker support and other web-platform features rather than treating it as a daily driver.

**「Community Discussion」** Commenters reported strong hands-on results, with one saying every site they tried rendered correctly and another calling NoVNC snappier than in Firefox, though one noted slightly jerky scrolling. Others debated tradeoffs: one lamented the loss of the original SerenityOS hacker spirit after Ladybird adopted production-grade libraries like SQLite and Skia, while another urged the project to prioritize anti-fingerprinting measures and more granular permissions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/355140/independent-web-browser-engine-ladybird-goes-into-alpha-release">Independent Web Browser/Engine &quot;Ladybird&quot; Goes Into Alpha ...</a></li>
<li><a href="https://ladybird.org/">Ladybird Ladybird, the first new browser engine in years, is now ... Ladybird Browser is now officially available in alpha for ... Ladybird browser reaches alpha after four years of development Ladybird browser releases its first alpha for macOS and Linux</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#web-platform`, `#open-source`, `#systems-engineering`, `#privacy`

---

<a id="item-tech-news-3"></a>
### [Z.ai Releases GLM-5.4, Its First Loop Transformer for Coding](https://z.ai/blog/glm-5.4) ⭐️ 8.0/10

Z.ai has released GLM-5.4, which it describes as its first model built on a looped transformer architecture, where a group of weight-shared layers runs for multiple iterations to deepen the network without increasing parameter count. The model is not yet available as open weights, and according to Simon Willison&\#x27;s write-up it cannot currently be reached through Z.ai&\#x27;s regular API plan; access required signing up for the Coding Plan subscription, whose API keys work against the same OpenAI-compatible Responses API at https://api.z.ai/api/v1. Willison&\#x27;s informal pelican-SVG tests found GLM-5.4 roughly comparable in quality to GLM-5.3, and both look more like OpenAI or Anthropic outputs than the distinctive earlier GLM-5.1 and 5.2 generations. No independent benchmark results for the looped architecture were provided.

hackernews · foohis · Nov 23, 10:06 · [Discussion](https://news.ycombinator.com/item?id=50609685)

**「Background」** A loop transformer reuses a shared group of layers for multiple iterations per forward pass, deepening the effective network without adding parameters. Z.ai&\#x27;s GLM-5.4 follows Thinking Machines Lab&\#x27;s Inkling 2 Mini, released around November 20, 2026, which runs its middle layers three times per token and is described as an open-weight looped transformer. The source notes GLM-5.4 is not yet available as open weights and is currently reachable through Z.ai&\#x27;s Coding Plan subscription rather than the regular API plan.

**「Impact」** Developers wanting to try GLM-5.4 must use the Coding Plan subscription rather than the standard API plan, and existing tooling may lag: Willison shipped a new llm-glm plugin only because the existing llm-zai plugin did not yet support the model, and he expects to retire his once it does. The source gives no evidence on whether or how the looped architecture improves coding performance over GLM-5.3.

**「Community Discussion」** Commenters praised Zhipu&\#x27;s willingness to publish architectural details, with one calling it a refreshing contrast to more closed Western labs and arguing looped transformers are an obvious direction because the original Transformer is like an unrolled loop that pairs unrelated weights. Another commenter reported that Chinese models&\#x27; long &quot;marathon thinking&quot; sessions make simple tasks slow and frustrating, speculating this is how they close benchmark gaps.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://openrouter.ai/thinkingmachines/inkling-2-mini">Inkling 2 Mini - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#transformer-architecture`, `#coding-models`, `#open-source-AI`, `#model-releases`

---

<a id="item-tech-news-4"></a>
### [Nvidia Board Reinstates Jensen Huang as CEO After Brief Ouster](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 8.0/10

Nvidia&\#x27;s board reportedly reinstated Jensen Huang as CEO after a brief ouster, according to CNBC and an Nvidia newsroom statement. The board said it received input from senior levels of the U.S. government and concluded that Huang&\#x27;s reinstatement poses no national security risk. The supplied material is thin and partly speculative, so the exact timeline, vote details, and conditions of the reinstatement are not fully established.

hackernews · jaz · Nov 23, 14:00 · [Discussion](https://news.ycombinator.com/item?id=50611576)

**「Background」** Nvidia&\#x27;s board reinstated Huang as President, CEO, and board member effective immediately, according to the company&\#x27;s announcement. The Guardian reported that Huang had resigned on November 13, 2026, after reports of extramarital affairs, including with an alleged Chinese spy, making the reinstatement a reversal of a roughly ten-day-old departure. The board&\#x27;s statement said it received input from senior levels of the U.S. government before concluding that Huang&\#x27;s reinstatement poses no national security risk.

**「Impact」** Nvidia&\#x27;s board said it received input from senior levels of the U.S. government before reinstating Huang, and that it is confident his return &quot;poses no national security risk&quot; — a condition that ties the leadership decision to export-control and national-security scrutiny. CNBC reported the stock rose 31% on the news, while members of Congress have raised national security questions about the reinstatement, according to USA Today. The practical consequence for Nvidia&\#x27;s customers and partners is that the company&\#x27;s leadership now rests on an explicit government signal rather than an independent board judgment alone, leaving the board&\#x27;s exposure to later political or legal challenge unresolved.

**「Community Reaction」** Commenters focused on the board&\#x27;s statement that it received input from senior U.S. government officials, with one calling it the most operative part of the announcement. Others debated board liability under Delaware&\#x27;s Caremark standard, expressed surprise at a unanimous reversal within two weeks, and drew a parallel to the 2023 OpenAI board episode as evidence that nominal governance structures may not reflect real decision-making power.

<details><summary>References</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-board-reinstates-jensen-huang-as-president-ceo-and-board-director">NVIDIA Board Reinstates Jensen Huang as President, CEO and...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/23/jensen-huang-reinstated-as-nvidia-chief-executive">Jensen Huang reinstated as Nvidia CEO | Jensen ... | The Guardian</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-board-reinstates-jensen-huang-as-president-ceo-and-board-director">NVIDIA Board Reinstates Jensen Huang as President, CEO and ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html">Jensen Huang reinstated as Nvidia CEO. Stock skyrockets 31%</a></li>
<li><a href="https://www.usatoday.com/story/news/politics/2026/11/23/congress-reaction-to-jensen-huang-nvidia-return/92925133007/">Congress raises national security questions over Jensen Huang ...</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#corporate-governance`, `#semiconductors`, `#export-controls`, `#tech-industry`

---

<a id="item-tech-news-5"></a>
### [Codex2api 疑似遭供应链投毒，3.1.10–3.1.12 版本受影响](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

一则 Telegram 报告称，Codex2api 项目作者的账号遭到入侵，攻击者绕过 main 分支保护直接推送 tag，使 Release 构建出带后门的版本。报告称 v3.1.11 移除了鉴权，等同于无密码远程执行命令，另有 workflow 将仓库的 16 个 Actions secrets 外传，波及同一账号下至少 21 个仓库。报告建议安装或更新过 3.1.10–3.1.12 的用户立即停用并回退到 3.1.9，同时轮换 GitHub token、SSH key、数据库及 DeepSeek 等相关密钥。上述内容来自单一 Telegram 帖子的指控，尚未获得独立验证。

telegram · zaihuapd · Nov 23, 11:21

**「Background」** The alleged attack exploits a common gap in GitHub&\#x27;s permission model: branch protection rules on \`main\` do not necessarily prevent an account from pushing tags, and tag pushes can trigger release workflows. Codex2api&\#x27;s reported compromise follows a broader pattern of open-source supply-chain incidents in which attackers inject backdoors into build or release pipelines rather than the source tree itself, as documented in analyses of the XZ Utils and PyPI cases.

**「影响与处置」** 使用 3.1.10–3.1.12 版本的用户面临未授权远程命令执行风险，且相关仓库的 Actions secrets 可能已泄露，因此需要按报告建议回退版本并轮换所有可能暴露的凭据。

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/chapter/10.1007/978-981-96-1624-4_24">Plotting OSS-Based Supply Chain Attack Strategies and the ...</a></li>

</ul>
</details>

**Tags**: `#supply-chain-security`, `#open-source-security`, `#github-actions`, `#incident-report`, `#codex2api`

---

<a id="item-tech-news-6"></a>
### [ChatGPT Chat Page Adds GPT-6.2 Sol for Paid Users](https://x.com/ChatGPT/status/2124942186425069836) ⭐️ 8.0/10

ChatGPT announced on November 23 that it has added GPT-6.2 Sol to the Chat tab, with rollout starting that day to Plus, Pro, Business, and Enterprise users. According to the official announcement, the version is aimed at everyday conversation and improves handling of complex requests, especially detailed instructions or requests to search the web. ChatGPT also claims gains in recognizing photo details such as label text and road-sign symbols, narrowing online options by criteria like price or location, and deciding when to proactively offer follow-up suggestions, such as asking whether to alert the user about a price drop. These capability claims come from the vendor announcement and have not been independently verified.

telegram · zaihuapd · Nov 24, 00:44

**「Background」** GPT-6.2 Sol is a follow-up to GPT-6, with MacRumors reporting that the new version improves on GPT-6 at detecting fine details in photos, such as symbols on a sign or text on a label. The Chat-tab version is being pushed to Plus, Pro, Business, and Enterprise tiers, the same paid tiers that received the earlier GPT-6 Astra rollout.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/11/23/openai-gpt-6-2-sol-chatgpt/">OpenAI Brings GPT - 6 . 2 Sol to ChatGPT &#x27;s Chat Tab - MacRumors</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT - 6 Astra: A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#ChatGPT`, `#OpenAI`, `#product release`, `#AI`

---

<a id="item-tech-news-7"></a>
### [NariQ ships sub-3-bit Qwen3.8-27B GGUF quants with a custom llama.cpp fork](https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF) ⭐️ 7.0/10

NariQ released 3-bit, 2.5-bit, and 2-bit GGUF quantizations of Qwen3.8-27B, claiming near-BF16 quality on agentic, math, multilingual, and image-understanding benchmarks, with the 3-bit file reported at roughly 10 GB. In the project&\#x27;s own tables, the 3-bit and 2.5-bit variants match or slightly exceed BF16 on DeepSWE \(41.0 and 41.9 vs 39.8\) and Terminal-Bench 2.1 \(63.8 and 60.2 vs 62.6\), while the 2-bit variant drops sharply \(28.6 and 52.4\). The authors say decode speed is comparable to other quants on an RTX PRO 6000, but running these files currently requires the project&\#x27;s own llama.cpp fork, and all figures are self-reported rather than independently measured.

hackernews · toebee · Nov 23, 13:42 · [Discussion](https://news.ycombinator.com/item?id=50611402)

**「Background」** GGUF is the file format used by llama.cpp and downstream tools such as LM Studio and Ollama to run quantized models locally, so a new quantization scheme typically needs loader support before it can be used. Nari Labs&\#x27; release page describes Qwen3.8-27B as a 27B-parameter image-text-to-text model, and a secondary report states the NariQ files use trellis-coded post-training quantization calibrated on real coding-agent traces, shrinking the model from 53.8 GB at BF16 to 10.12 GB at 3 bits per weight.

**「Practical impact」** Users cannot run these files with stock llama.cpp; the project states its own fork is currently required, so anyone testing the 3-bit, 2.5-bit, or 2-bit GGUFs must build and maintain that fork. The 2-bit variant is the clear weak point in the self-reported tables, dropping to 28.6 on DeepSWE and 52.4 on Terminal-Bench 2.1 versus 39.8 and 62.6 for BF16, so the near-BF16 claim holds mainly for the 3-bit and 2.5-bit files. A commenter reports roughly 3.8 tok/s decode on an 18 GB M3 Pro with the 3.0bpw file, far slower than CUDA, which limits usefulness on Apple hardware.

**「Community discussion」** Commenters welcomed the multi-task and held-out evaluation but remained skeptical: one argued that most of the reported gains come from a harness difference rather than the model, and another asked what information is actually lost as file size shrinks. A Mac user reported about 3.8 tok/s decode with the 3.0bpw file on an 18 GB M3 Pro, far slower than CUDA, and wondered whether a 16 GB machine could run it.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF">nari-labs/Qwen3.8-27B-NariQ-GGUF · Hugging Face</a></li>
<li><a href="https://aiweekly.co/alerts/nari-labs-nariq-quant-compresses-qwen38-27b-to-10gb-while-matching-bf16-on">Nari Labs&#x27; NariQ Quant Compresses Qwen3.8-27B to 10GB While ...</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#llm-inference`, `#llama.cpp`, `#gguf`, `#local-llm`

---

<a id="item-tech-news-8"></a>
### [Stalwart Claims Drop-In Exchange Replacement, Community Questions Outlook Fit](https://stalw.art/blog/microsoft-exchange-replacement/) ⭐️ 7.0/10

Stalwart announced in a blog post that its mail server can serve as a drop-in replacement for Microsoft Exchange. The announcement is a vendor claim rather than an independently verified result, and no source content was supplied detailing which Exchange features, protocols, or versions are covered. Commenters immediately challenged the framing, pointing to Outlook&\#x27;s shift toward cloud-only Exchange support and Microsoft&\#x27;s new Outlook syncing IMAP mail to Microsoft servers.

hackernews · shaunpud · Nov 23, 22:32 · [Discussion](https://news.ycombinator.com/item?id=50620349)

**「Background」** Stalwart is an open-source, all-in-one mail and collaboration server that supports IMAP, JMAP, SMTP, CalDAV, CardDAV, and WebDAV. The vendor&\#x27;s announcement ties the Exchange-replacement claim to the release of Stalwart 1.2.0, framing it as an alternative to the long-standing pairing of Microsoft Exchange as the server and Outlook as the client.

**「Practical impact」** Administrators evaluating Stalwart as an Exchange replacement face a client-side constraint: the new Outlook does not support on-premises Exchange accounts but does accept IMAP accounts, so migration may depend on IMAP rather than native Exchange connectivity. Commenters also flag that Stalwart&\#x27;s regular and open-source plans lack the tamper-proof, long-term archiving that German GoBD rules require, which could block adoption for affected organizations.

**「Community Discussion」** Several commenters argued &quot;drop-in replacement&quot; oversells the claim: hobo123 and traceroute66 noted that if Outlook drops on-premises Exchange support, Stalwart customers would still need a different client, and traceroute66 added that the new Outlook forces IMAP mail to sync to Microsoft. rmoriz flagged a regulatory gap, saying Stalwart&\#x27;s regular plans and open-source variants lack the tamper-proof, up-to-10-year archiving German tax rules \(GoBD\) require, while andreashaerter argued that extending Microsoft&\#x27;s protocol stack ultimately harms the open email ecosystem. markstos noted that Stalwart is the mail server behind Mozilla&\#x27;s Thundermail.

<details><summary>References</summary>
<ul>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop - in replacement for Microsoft Exchange</a></li>
<li><a href="https://github.com/stalwartlabs/stalwart">GitHub - stalwartlabs/ stalwart : All-in-one Mail &amp; Collaboration server .</a></li>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange | Stalwart</a></li>

</ul>
</details>

**Tags**: `#email`, `#open-source`, `#microsoft-exchange`, `#self-hosting`, `#interoperability`

---

<a id="item-tech-news-9"></a>
### [黎曼猜想「AI 证明」被指空转，作者承认代码满是垃圾](https://x.com/i/web/status/2124987173439209561) ⭐️ 7.0/10

Alpöge 与 Claude 宣称证明了黎曼猜想及其广义版本，但只公开了 1700 万行 Lean 代码、17.5 万个文件，没有提供人类可读的证明。Lean 与 Mathlib 社区次日表示，对代码证明了这一命题「有充分信心」。随后有研究者指出，关键定义被写成恒真、几何条件形同虚设，证明可能只是空转。23 日 Alpöge 承认「25 万页是玩笑」，代码「满是垃圾但能编译」，并称批评完全合理。

telegram · zaihuapd · Nov 24, 01:29

**「Background」** The Riemann Hypothesis is a long-standing conjecture about the zeros of the Riemann zeta function. According to a Wikipedia entry, the Lean formalization effort behind this claim ran from 6 October to 16 November, and a University of Waterloo page states that Levent Alpöge announced on 20 November 2026 a proof of the Riemann Hypothesis and the Generalized Riemann Hypothesis for Dirichlet L-functions found with Anthropic&\#x27;s Claude. The resulting artifact was 17 million lines of Lean built in about six weeks, which, per a YouTube account, dozens of people compiled and checked but which is far too long for anyone to read.

**「影响」** 这一事件表明，机器可检查的 Lean 代码通过编译，并不等于数学证明有效：如果定义被写成恒真、条件形同虚设，形式化验证仍可能空转。对依赖 Lean/Mathlib 审查 AI 生成数学结果的研究者而言，需要同时检查定义是否非平凡、条件是否真正起作用，而不能只看代码能否编译。

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Riemann_hypothesis">Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://www.youtube.com/watch?v=-Tzliv3mzds">AI Helped Prove the Riemann Hypothesis . Nobody Can... - YouTube</a></li>
<li><a href="https://math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/">Alpöge / Claude proof of the Generalized Riemann Hypothesis</a></li>

</ul>
</details>

**Tags**: `#AI for mathematics`, `#Lean theorem proving`, `#formal verification`, `#Riemann Hypothesis`, `#AI reliability`

---

<a id="item-tech-news-10"></a>
### [45,000 EU businesses urge Commission to open Apple browser case](https://appleinsider.com/articles/26/11/23/eu-urges-to-challenge-apples-grip-on-iphone-browsers?utm_source=rss) ⭐️ 7.0/10

A coalition of businesses and civil-society groups, including Mozilla and Shopify, has sent a letter asking the European Commission to open a case against Apple&\#x27;s iPhone browser restrictions. The signatories say they collectively represent roughly 45,000 to 55,000 EU businesses and organizations, and the letter remains open for signatures until December 3, 2026. They argue that although the Digital Markets Act lets rival browsers use their own engines in the EU, technical and legal requirements prevent vendors from migrating existing EU users away from WebKit, while businesses remain dependent on the App Store to reach users. The coalition estimates that if half of native iOS apps moved to the web, EU businesses would save €11 billion a year in development costs and €1.3 billion in App Store fees; this is a lobbying claim in a letter, not a confirmed regulatory action.

telegram · zaihuapd · Nov 24, 03:02

**「背景」** The EU&\#x27;s Digital Markets Act, in force since 2024, required Apple to let iPhone users choose a default browser and opened a path for third-party browser engines on iOS. Mozilla has reported that Firefox daily use on iOS doubled in the EU after the DMA default-browser requirement took effect, while critics such as the Open Web Advocacy group argue Apple&\#x27;s browser-engine ban has persisted in practice despite the rules. The coalition&\#x27;s letter now presses the European Commission to move from rulemaking to enforcement, and the DMA allows fines of up to 10% of a gatekeeper&\#x27;s global annual turnover for confirmed breaches.

**「Impact」** The letter targets the Commission&\#x27;s enforcement discretion rather than a specific product change, so no compliance deadline or remedy is yet in play. For browser vendors and app developers, the coalition&\#x27;s argument is that DMA-mandated engine choice has not translated into practical migration paths for existing users, which is the condition any future case would likely test.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.mozilla.org/en/mozilla/internet-policy/apple-ios-browser-engine-rules/">Why there are still no non- WebKit browsers on iOS</a></li>
<li><a href="https://techcrunch.com/2024/01/26/apple-dma-webkit/">A closer look at Apple &#x27;s browser -related changes to iOS... | TechCrunch</a></li>
<li><a href="https://open-web-advocacy.org/blog/apples-browser-engine-ban-persists-even-under-the-dma/">Apple &#x27;s Browser Engine Ban Persists, Even Under the DMA</a></li>

</ul>
</details>

**Tags**: `#apple`, `#eu-regulation`, `#dma`, `#browsers`, `#antitrust`

---

<a id="item-tech-news-11"></a>
### [新加坡总理黄循财承诺不让新加坡成为规避美国芯片管制的通道](https://www.bloomberg.com/news/articles/2026-11-24/singapore-won-t-be-conduit-to-skirt-us-chip-curbs-wong-says) ⭐️ 7.0/10

新加坡总理黄循财表示，新加坡不会被用作企业规避美国芯片出口管制的通道，当局正在调查 Megaspeed 采购英伟达芯片的交易。此前一天，美国商务部将 Megaspeed 及另外 6 家东南亚企业列入贸易黑名单，《联邦公报》称这些企业存在向未获授权用户转移先进计算产品的「重大风险」，名单包括其在马来西亚、泰国的关联实体。路透社报道，阿里巴巴新加坡子公司 Apex Enterprise Solutions 同样在列，阿里称从未转移受管制的先进计算芯片。

telegram · zaihuapd · Nov 24, 05:03

**「背景」** 美国商务部于周一发布正式通知，将总部位于新加坡的 Megaspeed 及其在泰国和马来西亚的子公司列入贸易黑名单，限制其购买先进半导体芯片。该部门同时将另外六家亚洲公司列入名单，理由是在一项持续进行的调查中，这些公司存在向未获授权用户转移先进计算产品的风险。

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/nov/23/megaspeed-us-trade-blacklist-nvidia">US adds Megaspeed, AI firm at center of Nvidia scandal, to ...</a></li>
<li><a href="https://www.ibtimes.com/us-blacklists-megaspeed-southeast-asian-firms-nvidia-chips-3810114">US Blacklists Nvidia-Linked Firm Over China Chip Fears. Six ...</a></li>

</ul>
</details>

**Tags**: `#export controls`, `#semiconductors`, `#Nvidia`, `#AI hardware supply chain`, `#Singapore`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [vLLM Day-0 Support for ERNIE 5.5 Flash Preview](https://vllm.ai/blog/2026-11-24-ernie-5-5-flash-preview) ⭐️ 6.0/10

rss · vLLM Blog · Nov 24, 00:00

**「Background」** ERNIE 5.5 Flash Preview is a sparse mixture-of-experts model with 280B total parameters and 14B activated per token, a 1M-token context, and agent-oriented tool calling. The Baidu ERNIE team and vLLM aimed to make it runnable on release day without maintaining a fork or waiting for a model-specific Docker image or nightly wheel.

**「Solution」** The authors deliver support through the vLLM-ERNIE plugin, a standalone package installed alongside the official vllm==0.32.0 wheel and discovered automatically via the vllm.general\_plugins entrypoint. The plugin registers ERNIE architectures as module paths, so model code loads only when a config names those architectures, and it adds config, tokenizer, chat renderer, and parser registrations; setting VLLM\_PLUGINS=&quot;&quot; disables it. Most of the technical detail concerns inference cost. The model uses 37 Heavily Compressed Attention layers and 6 MLA-DSA layers, plus a low-rank attention gate \(VHA\), Multi-Router Latent MoE, mHC residual streams, and a MultiMax output head. For each new structure, the authors fuse kernels and fold fixed inference-time parameters into weights at load time: VHA mixing becomes one small matmul with FP8 quantization in the same kernel \(1.56x-1.73x per kernel\), router weights are concatenated for a single GEMM with a fused routing chain \(3.54x-6.10x\), MultiMax runs as a single pass over roughly 200K logits \(4.33x-6.53x\), and gated attention merges gate projection and sigmoid gating \(1.55x-1.75x in prefill\). They report 1.55x-6.53x per-kernel speedups and bitwise-identical outputs for several fusions, though without benchmark methodology or hardware specifics. FlashIndexer adds a small head router that picks sparse indexer heads per token, trained by distilling the original DSA token selections with the backbone frozen; about 1B tokens suffice, and threshold pre-filtering shrinks the top-k candidate set, yielding a reported 1.4x speedup at 1M context. The default checkpoint stores routed experts in MXFP4 \(W4A8\) with QAT whose fake quantization matches inference granularity, scales, and rounding, while other weights are FP8 and the KV cache is FP8. A bundled 3-layer DSpark draft model proposes up to 7 tokens per step and reaches a mean acceptance length above 4.0 on coding and agent workloads, supported by multi-stage training and on-policy distillation. The authors also list data-parallel attention with expert parallelism, attention tensor parallelism at TP2/4/8, PD disaggregation over Mooncake, and CPU KV offload, but do not examine tradeoffs of the plugin approach or FlashIndexer.

**「Takeaway」** The authors present day-0 vLLM support for ERNIE 5.5 Flash as a case study in combining a lightweight plugin integration with aggressive kernel fusion, weight pre-folding, and a distilled sparse indexer to cut inference cost. The reported speedups are vendor claims without disclosed benchmark conditions, so they are most useful as directional evidence for readers deploying this model or building vLLM plugins.

**Tags**: `#inference-optimization`, `#vllm`, `#mixture-of-experts`, `#kernel-fusion`, `#quantization`

---

## Financial News

<a id="item-finance-news-1"></a>
### [New York Fed&\#x27;s Williams Says More Rate Work Needed to Reach 2% Inflation](https://www.cnbc.com/2026/11/23/john-williams-fed-inflation-rate-hikes.html) ⭐️ 8.0/10

New York Fed President John Williams said the Fed still has &quot;work to do&quot; to bring inflation back to its 2% target, indicating further rate action can unfold &quot;over time&quot; ahead of the Dec. 8-9 FOMC meeting, where markets fully price a quarter-point increase from the current 3.75%-4% target range.

rss · CNBC Finance · Nov 23, 21:02

**「Background」** Williams attributed current inflation pressures to the conflict in Iran, AI-related demand and tariffs, and said he expects inflation to approach 2% in 2027 and reach it the following year; his remarks were consistent with prior statements and did not explicitly address December expectations.

**「Impact」** A quarter-point increase would raise borrowing costs for households and businesses tied to the Fed&\#x27;s benchmark rate, though Williams framed further moves as gradual rather than immediate.

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [AI Selloff Clouds Planned Listings by DeepSeek and Moonshot AI](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

A global AI stock selloff that followed Anthropic&\#x27;s record $119.5 billion IPO is weighing on Chinese tech shares and casting doubt on planned listings by DeepSeek, Moonshot AI, and StepFun, Bloomberg reported. Chinese tech stocks have lost a cumulative $1.7 trillion in market value since the end of June, according to the report.

telegram · zaihuapd · Nov 23, 09:31

**「Background」** Anthropic&\#x27;s IPO was the largest ever, surpassing SpaceX&\#x27;s June listing, but its shares fell in the days after the debut as a broader AI selloff hit tech stocks \(tool-1-3, tool-1-2\). DeepSeek, Moonshot AI and StepFun are among a group of Chinese AI startups that had been accelerating plans to list \(tool-2-2, tool-2-3\).

**「Impact」** The selloff directly affects investors holding Chinese AI stocks, such as Zhipu and MiniMax, whose shares have fallen sharply, and it could delay or shrink the planned listings of DeepSeek, Moonshot AI, and StepFun, limiting their access to public capital.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/20/anthropic-ipo-ai-stock-market-selloff.html">Why Anthropic &#x27;s IPO couldn&#x27;t escape the stock market correction</a></li>
<li><a href="https://www.france24.com/en/business/20261119-anthropic-begins-trading-1-5-trillion-company-biggest-ipo-record-ai">Anthropic blows past $2 trillion in Nasdaq debut, beating... - France 24</a></li>
<li><a href="https://www.outlookbusiness.com/deeptech/deepseek-moonshot-gigaai-why-chinas-ai-startups-are-rushing-for-ipo">DeepSeek , Moonshot , GigaAI: Why China&#x27;s AI Startups Are Rushing...</a></li>
<li><a href="https://fortune.com/2026/07/23/moonshot-deepseek-great-chinese-ai-ipo-rush/">Moonshot , DeepSeek , and the Great Chinese AI IPO Rush | Fortune</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-23/china-ai-model-stocks-150-billion-drop-shows-no-sign-of-easing">China AI Model Stocks’ $150 Billion Drop Shows No Sign of ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-22/china-s-1-7-trillion-ai-rout-turns-hot-trade-into-losing-bet">China’s $1.7 Trillion AI Rout Turns Hot Trade Into Losing Bet</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IPO`, `#China tech`, `#market selloff`, `#equities`

---

<a id="item-finance-news-3"></a>
### [Shanghai Adjusts Subway Fares for First Time in 21 Years](https://weibo.com/1699432410/5368461393397183) ⭐️ 7.0/10

Shanghai announced its first subway fare adjustment in 21 years, keeping a 3-yuan base fare for trips of 0-4 km and adding 1 yuan for each subsequent 4, 4, 4, 7, 7, 10 and 10 km, then 1 yuan per 15 km beyond 50 km, effective December 1. To soften the impact on frequent riders, four multi-ride passes priced at 190, 210, 270 and 390 yuan for 35, 45, 60 and 90 rides go on sale November 26, and riders spending 90 yuan in a month through one payment channel get a 10% discount.

telegram · zaihuapd · Nov 23, 10:45

**「Background」** Shanghai&\#x27;s subway fares had not changed for 21 years before this adjustment; according to a report on the plan, the average fare per trip was projected to rise from 4.23 yuan to 5.22 yuan, an increase of 0.99 yuan, under one of the proposed options.

**「Who is affected」** Frequent Shanghai commuters face higher per-trip costs under the new distance-based fares, but the four multi-ride passes \(190–390 yuan\) and the 10% discount after 90 yuan in monthly spending on one payment channel are designed to limit that increase for heavy users.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260819A0ARAE00">时隔 21 ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260819A0A7CX00">news.qq.com/rain/a/20260819A0A7CX00</a></li>
<li><a href="https://hi.online.sh.cn/content/2026-08/21/content_10481931.htm">hi.online.sh.cn/content/2026-08/21/content_10481931.htm</a></li>
<li><a href="https://c.m.163.com/news/a/L4NE02LA0514R9P4.html">c.m.163.com/news/a/L4NE02LA0514R9P4.html</a></li>

</ul>
</details>

**Tags**: `#public transit`, `#pricing`, `#Shanghai`, `#consumer costs`, `#policy`

---

<a id="item-finance-news-4"></a>
### [SpaceX 据报向 Anthropic 和 Google 出租算力，月入数十亿美元](https://www.nytimes.com/2026/11/23/business/elon-musk-ai-anthropic-google.html) ⭐️ 7.0/10

据《纽约时报》11 月 23 日报道，SpaceX 自今年 5 月起每月向 Anthropic、Google 等公司出租其数据中心的算力，月收入达数十亿美元；报道援引三名知情人士称，马斯克向员工表示 SpaceX 在 AI 上落后，出租算力比自用更赚钱。

telegram · zaihuapd · Nov 24, 02:06

**「Background」** The New York Times reported that SpaceX has been renting data-center computing power to competitors including Anthropic since May, and that this rental business is making it harder for Musk&\#x27;s own AI effort. The report cites three people familiar with the matter; the specific revenue figures have not been independently verified.

**「Impact」** 若该报道属实，SpaceX 将成为 AI 算力的重要供应商，为 Anthropic 和 Google 提供训练与运行模型所需的计算资源，而这一收入此前未公开披露。

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/23/business/elon-musk-ai-anthropic-google.html">Elon Musk Faces an A.I. Dilemma at SpaceX - The New York Times</a></li>
<li><a href="https://qz.com/spacex-leases-computing-power-anthropic-google-ai-112326">SpaceX leases computing power to Anthropic, Google ... - Quartz</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#SpaceX`, `#Anthropic`, `#Google`, `#compute rental`

---