---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 31 items, 16 important content pieces were selected

---

**Technology News**
1. [OpenSec 披露 Linux nfsd 预认证堆溢出漏洞，CVSS 9.8](#item-tech-news-1) ⭐️ 9.0/10
2. [Google Research&\#x27;s DeepCrossAttention claims 3x faster transformers](#item-tech-news-2) ⭐️ 7.0/10
3. [WebRTC-Based Card Skimming Scripts Found on Shopping Sites](#item-tech-news-3) ⭐️ 7.0/10
4. [States sue SpaceX over Grok&\#x27;s alleged child sex abuse and non-consensual images](#item-tech-news-4) ⭐️ 7.0/10
5. [Convex coding skill allegedly uploads app ideas without disclosure](#item-tech-news-5) ⭐️ 7.0/10
6. [Essay Questions Reliability of Computer-Checked Proofs](#item-tech-news-6) ⭐️ 7.0/10
7. [SemiAnalysis Benchmarks Trainium3 Inference Against Nvidia GB300](#item-tech-news-7) ⭐️ 7.0/10
8. [黑客据称借助开源 AI 工具 Artex 攻击美国情报机构](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic system card discloses silent degradation of frontier-model development requests](#item-tech-news-9) ⭐️ 7.0/10
10. [Minecraft Bedrock resource-pack flaw hits 26.52–26.63, fixed in 26.65](#item-tech-news-10) ⭐️ 7.0/10
11. [Microsoft moves to replace some third-party drivers with in-box Windows drivers](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [China&\#x27;s State Council Vows Stronger State-Backed Market Stabilization](#item-finance-news-1) ⭐️ 8.0/10
2. [S&amp;P 500 Enters Correction, Down 11.6% From October Record](#item-finance-news-2) ⭐️ 7.0/10
3. [Mixue invests RMB 500 million in DeepSeek&\#x27;s reported RMB 100 billion round](#item-finance-news-3) ⭐️ 7.0/10
4. [央行下调大额存单起购门槛](#item-finance-news-4) ⭐️ 7.0/10
5. [China&\#x27;s Market Regulator Summons 15 E-Bike Makers Over Quality and Certification Failures](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenSec 披露 Linux nfsd 预认证堆溢出漏洞，CVSS 9.8](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 9.0/10

OpenSec 披露了 Linux 内核 NFS 服务器 nfsd 中的预认证堆溢出漏洞 CVE-2026-99362，CVSS 评分为 9.8。攻击者无需登录，只需向 tcp/2049 发送一条连接，即可越界写入内核堆并获取 root shell。该漏洞自 2014 年的 Linux 3.16 起存在，影响启用 NFSv4.1 或 4.2 的主机，包括文件服务器、NAS 和集群存储节点。修复已在 6.12.117、6.18.61、7.3.2 和 7.4-rc1 中发布，需要升级内核并重启；无法立即升级的环境可通过防火墙限制 tcp/2049 访问。CVE 于 2026 年 11 月 20 日公开。

telegram · zaihuapd · Nov 27, 12:57

**「背景」** nfsd 是 Linux 内核中的 NFS 服务器实现，tcp/2049 是其标准服务端口，NFSv4.1 和 4.2 是较新的协议版本。该漏洞的根源可追溯到 Linux 3.16，意味着此后启用上述协议版本的主机长期处于受影响状态。

**「影响」** 运行 NFSv4.1 或 4.2 的文件服务器、NAS 和集群存储节点若暴露 tcp/2049，可能被未认证攻击者直接获取 root 权限。管理员应升级到 6.12.117、6.18.61、7.3.2 或 7.4-rc1 并重启；无法立即升级时，应通过防火墙限制对 tcp/2049 的访问。

**Tags**: `#linux-kernel`, `#security-vulnerability`, `#nfs`, `#cve`, `#remote-exploit`

---

<a id="item-tech-news-2"></a>
### [Google Research&\#x27;s DeepCrossAttention claims 3x faster transformers](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 7.0/10

Google Research published a blog post describing DeepCrossAttention, a modification to transformer residual connections that it reports matches model quality while running up to 3x faster. The claim comes from a vendor research blog rather than peer-reviewed or independently measured results, and no source text was available to confirm the specific benchmarks, model sizes, or hardware used. The post is titled &quot;Supercharging Transformer Residual Connections.&quot;

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**「Background」** DeepCrossAttention builds on the standard transformer residual connection, which simply sums the outputs of previous layers; Google Research says this can dilute crucial information. The technique instead routes across layers with learnable weights, and an arXiv paper describing it was published earlier, with the work also listed as an ICML 2025 paper. The current Google Research blog post, dated November 23, 2026, presents the method and its speed claims.

**「Practical takeaway」** Because the speedup is reported as &quot;up to 3x&quot; on a research blog, teams considering the technique should treat it as a candidate to reproduce on their own workloads rather than an established efficiency gain. The modification targets residual connections, so any adoption would require retraining or architectural changes rather than a drop-in inference tweak.

**「Discussion」** Commenters pushed back on presentation and novelty: one objected that the comparison charts should be bar graphs rather than line graphs because the methods have no temporal relationship, and another asked whether this is essentially DenseNet-style connectivity. A separate thread speculated about combining the technique with existing token-throughput methods, though no one reported measured results.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections</a></li>
<li><a href="https://arxiv.org/html/2502.06785">DeepCrossAttention : Supercharging Transformer Residual ...</a></li>
<li><a href="https://scholar.google.com/citations?user=SZpFJqIAAAAJ&amp;hl=en">Google - Cited by 399 - Machine Learning - Data Mining - Algorithms</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#machine learning`, `#model efficiency`, `#google research`, `#attention mechanisms`

---

<a id="item-tech-news-3"></a>
### [WebRTC-Based Card Skimming Scripts Found on Shopping Sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 7.0/10

A security report describes credit card skimming scripts that use WebRTC found on popular shopping sites, according to a Hacker News submission dated November 27, 2026. The report frames the technique as a way to exfiltrate stolen payment data through a channel less commonly monitored for abuse. Commenters note that WebRTC is incidental to the attack and that the same approach could work with ordinary HTTP requests, with the real exposure coming from third-party scripts embedded on checkout pages. No source content was available, so details such as the affected sites, the number of victims, or the script&\#x27;s exact behavior are unconfirmed.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**「Background」** Web skimming \(also called formjacking or Magecart-style attacks\) works by injecting malicious JavaScript into a checkout page, often through a compromised third-party script, so payment details are captured as shoppers type them. The technique is not new, but attackers continually vary the delivery and exfiltration channels to evade detection. The WebRTC-based variant reported here follows earlier research: a March 2026 report described a skimmer that used a WebRTC peer connection to a hard-coded IP address to fetch and inject JavaScript, bypassing Content Security Policy controls.

**「Impact」** The practical concern for merchants is third-party script inclusion on payment pages: as one commenter put it, &quot;If you&\#x27;re embedding third party scripts on your site you&\#x27;re always vulnerable.&quot; Because the reported technique relies on a channel that is less frequently monitored rather than on a WebRTC-specific flaw, defenses focused only on blocking WebRTC would not address the underlying risk of untrusted scripts running alongside card-entry forms.

**「Community Discussion」** Commenters pushed back on the framing of WebRTC as the novel element, with afavour arguing the attack has &quot;nothing to do with the technical capabilities of WebRTC&quot; and would work with simple HTTP requests, while also noting the scripts reportedly target mobile devices because they are harder to detect. Others debated structural fixes: snickerer argued sites should deliver only data and let the browser decide how to render it, and s\_u\_d\_o asked why ad providers and browsers do not sandbox ads to prevent client-side JavaScript execution. jszymborski cited the report as justification for ad blocking.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/03/webrtc-skimmer-bypasses-csp-to-steal.html">WebRTC Skimmer Bypasses CSP to Steal Payment Data from E ...</a></li>
<li><a href="https://aviatrix.ai/threat-research-center/webrtc-skimmer-bypasses-csp-to-steal-payment-data-from-e-commerce-sites/">WebRTC Skimmer Bypasses CSP to Steal Payment Data from E ...</a></li>

</ul>
</details>

**Tags**: `#web-security`, `#credit-card-skimming`, `#webrtc`, `#third-party-scripts`, `#e-commerce`

---

<a id="item-tech-news-4"></a>
### [States sue SpaceX over Grok&\#x27;s alleged child sex abuse and non-consensual images](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

A group of state attorneys general, including Virginia&\#x27;s Jay Jones and Maine&\#x27;s Aaron Rayfield, filed suit against SpaceX as the parent company of X, xAI, and Grok, alleging the chatbot generated child sexual abuse material and non-consensual intimate images. The suit targets the creation and promotion of such content on the platform. The release does not specify how many states joined, which court heard the case, or what relief is sought, and the allegations remain untested claims rather than adjudicated findings.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**「Legal backdrop」** The suit arrives after a federal appeals court ruling in 2026 held that AI-generated child sexual abuse material depicting no real children is protected by the First Amendment, citing the Supreme Court&\#x27;s Ashcroft v. Free Speech Coalition precedent. That decision addressed private possession, not the generation or promotion of such material by a platform, which is the conduct the states&\#x27; suit targets.

**「Community reaction」** Commenters questioned whether Grok was unusually permissive by default or had to be manipulated into producing the material, and one asked whether the people prompting the system would also face liability. Another commenter asserted that the Supreme Court has already ruled AI-generated child sexual abuse material made for personal consumption is protected speech, with a carveout for depictions of real children; that claim is unverified in the supplied material and should not be treated as established.

<details><summary>References</summary>
<ul>
<li><a href="https://billygraham.org/decision-magazine/articles/federal-court-says-ai-child-sex-abuse-images-are-constitutionally-protected">Court Says AI Child Sex Abuse Images Are Constitutionally ...</a></li>
<li><a href="https://www.foxnews.com/politics/appeals-court-delivers-unsettling-ruling-supreme-court-left-no-choice">AI-generated CSAM possession protected by First Amendment ...</a></li>
<li><a href="https://www.snopes.com/fact-check/judge-ai-child-sex-abuse-ruling/">Judge ruled certain AI-generated child sex abuse material is ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#content moderation`, `#AI regulation`, `#generative AI`, `#legal`

---

<a id="item-tech-news-5"></a>
### [Convex coding skill allegedly uploads app ideas without disclosure](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

A GitHub issue on the convex-backend-skill repository alleges that Convex&\#x27;s coding skill sends users&\#x27; app ideas to a remote server without telling them. In the comments, Convex CEO Jamie responded that the prompt upload powers the Convex &quot;quickstart&quot; feature, described as the successor to the recently shut-down Convex Chef vibe-coding product, and that it bootstraps an environment. The source provides only the issue title and partial comments, so the exact data flow, scope, and whether any disclosure exists remain unverified.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**「Background」** Convex&\#x27;s quickstart skill is tied to the company&\#x27;s earlier end-to-end vibe-coding product, Convex Chef, which Convex says it shut down recently; the CEO described the quickstart feature as Chef&\#x27;s &quot;spiritual successor.&quot; Convex&\#x27;s own migration guide states that Chef cannot re-import a project or track progress from outside it, and the quickstart skill&\#x27;s instructions describe scaffolding pre-written Convex modules and building the user&\#x27;s idea live through a Chef panel rather than chat. The disputed upload is the mechanism behind that quickstart flow, according to the CEO&\#x27;s comment in the issue thread.

**「Why it matters」** Developers using the skill should assume prompts may leave their machine and review what the plugin transmits before feeding it proprietary app ideas, since the CEO&\#x27;s comment confirms an upload tied to quickstart rather than denying it. The dispute also highlights that prompt handling in AI developer tooling is a trust decision users cannot easily audit from the outside.

**「Community reaction」** Commenters debated the trust implications: one argued that self-hosted open-weight models are the long-term answer, while another noted that prompt injection is far more common than models making malicious tool calls on their own, without claiming malice here. One commenter questioned why an author of an unrelated front-page post was also commenting in this issue.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.convex.dev/chef/migration-guide">Chef Migration Guide | Convex Developer Hub</a></li>
<li><a href="https://github.com/get-convex/convex-backend-skill/blob/main/skills/quickstart/SKILL.md">convex-backend-skill/skills/quickstart/SKILL.md at main · get ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#ai-tooling`, `#developer-platforms`, `#prompt-injection`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [Essay Questions Reliability of Computer-Checked Proofs](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

Daniel J. Bernstein&\#x27;s cr.yp.to essay argues that computer-checked proofs can be false, focusing on soundness bugs in proof verifiers. The piece is an argument and analysis rather than a report of a new result, and the supplied material does not include the essay&\#x27;s full text or any specific bug, version, or measurement. Hacker News commenters pushed back on the practical risk, citing multi-verifier pipelines and the rarity of soundness bugs.

hackernews · \_tk\_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**「Background」** The essay is by Daniel J. Bernstein, an American mathematician, cryptologist, and computer scientist. Its premise is that proof-checking programs claiming to verify every step of a proof have had reported &quot;soundness bugs&quot; that at least potentially let false statements pass. Bernstein has separately argued that readers given a computer-checked proof spend much less time worrying that the theorem is wrong, which is the concern the essay builds on.

**「Impact」** For users of proof assistants, the discussion points to a concrete safeguard: acceptance by more than one independent checker. Commenters note that Metamath&\#x27;s main databases require proofs to pass five independently created verifiers in five programming languages, and that Lean has multiple checkers, so a single soundness bug is not enough to get a false proof accepted.

**「Community Discussion」** Commenters agreed soundness bugs exist but argued the essay understates the gap between one bad verification and misleading mathematicians, since a false proof would need to defeat every checker without looking implausible on informal review. One commenter cited a DeepMind researcher who built a proof passing Lean and a then-week-old nanoda by exploiting a different bug in each, while another said all soundness bugs found in decades-old systems would fit in a tweet.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Daniel_J._Bernstein">Daniel J . Bernstein - Wikipedia</a></li>
<li><a href="https://cr.yp.to/proofs/falseccp.html">False computer - checked proofs (djb)</a></li>
<li><a href="https://mastodon.cr.yp.to/@djb/112254574086845278">Daniel J . Bernstein : &quot;&quot;Referees and other readers provided with...</a></li>

</ul>
</details>

**Tags**: `#formal-verification`, `#proof-assistants`, `#software-correctness`, `#lean`, `#metamath`

---

<a id="item-tech-news-7"></a>
### [SemiAnalysis Benchmarks Trainium3 Inference Against Nvidia GB300](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 7.0/10

SemiAnalysis published a microarchitecture deep dive on AWS Trainium3, arguing its tile-first design differs fundamentally from Nvidia&\#x27;s GPU lineage, which added Tensor Cores in Volta, TMA in Hopper, and Tensor Memory in Blackwell to a graphics-derived architecture. Using its UBenchX microbenchmark suite, the firm reports that Trainium&\#x27;s Descriptor Generation Engines \(DGE\), the counterpart to Nvidia TMA and AMD MI455X TDM, reach peak HBM bandwidth utilization at small message sizes, which it says is not possible on Nvidia GPUs. SemiAnalysis also says Trainium3 with PDS and vLLM beats every accelerator except Vera Rubin across its TCO-versus-p90-interactivity curve on InferenceX, and that Trainium3 and TPUs are now live on the platform. These are vendor-assisted benchmark results from a partial excerpt, not independently verified measurements.

rss · Semianalysis · Nov 27, 15:54

**「Background」** Trainium chips are designed by AWS subsidiary Annapurna Labs, and Trainium3 is the successor to Trainium2, which was positioned to match Nvidia H100/B200 inference performance at lower manufacturing cost. AWS has also worked to lower the software barrier to its accelerators: TorchNeuron, open-sourced at PyTorch Conference, lets developers run existing PyTorch code on Trainium chips without a rewrite. The SemiAnalysis analysis builds on this lineage by arguing that Trainium3&\#x27;s tile-first microarchitecture, rather than only Amazon&\#x27;s supply-chain costs, explains its measured inference performance per dollar.

**「Impact」** For teams weighing inference hardware, the reported result is that Trainium3&\#x27;s cost-per-token advantage stems partly from microarchitecture, not only Amazon&\#x27;s supply chain, so the comparison hinges on the specific workload and latency target rather than a single throughput number. SemiAnalysis says AWS Annapurna Labs staff helped validate the benchmark experiments, so readers should treat the perf/$ figures as vendor-collaborated rather than independent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.idlen.io/news/amazon-anthropic-25-billion-investment-100-billion-aws-trainium-april-2026/">Amazon Pours Another $25B Into Anthropic — $100B AWS Trainium ...</a></li>
<li><a href="https://www.aboutamazon.com/news/innovation-at-amazon/torchneuron-pytorch-aws-trainium-chips-ai">Amazon &#x27;s TorchNeuron runs PyTorch on AWS Trainium chips</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#microarchitecture`, `#AWS Trainium`, `#inference`, `#Nvidia GPUs`

---

<a id="item-tech-news-8"></a>
### [黑客据称借助开源 AI 工具 Artex 攻击美国情报机构](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 7.0/10

《纽约时报》报道称，黑客攻击了美国中央情报局、国家地理空间情报局和国家情报总监办公室，并在攻击中使用了 AI 工具辅助。攻击者使用的工具名为 Artex，可整合多个开源 AI 模型来测试网络和计算机防御。一名中国开发者今年早些时候发布了 Artex，该工具后来被用于多起攻击，包括针对欧盟的一起；该开发者已将其从自己的 GitHub 账号删除。报道称此次攻击看起来不算严重，影响的是非机密侦察数据；今年早些时候，FBI 曾警告网络罪犯和间谍正在广泛使用 Artex。

telegram · zaihuapd · Nov 27, 10:42

**「Background」** Artex is an AI-powered penetration-testing framework that aggregates multiple open-source AI models to probe network and computer defenses. According to TechCrunch, its developer made the software closed-source after it was used in cyberattacks, but the FBI said the earlier open-source version continues to circulate and remains &quot;widely accessible.&quot; BleepingComputer reported that the FBI has warned Artex is being used to automate attacks worldwide, including a ConnectWise supply-chain breach that compromised Microsoft 365 customer environments.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/16/fbi-says-artex-ai-open-source-hacking-tool-used-to-breach-networks-in-under-three-hours/">FBI says Artex AI open source hacking tool used to... | TechCrunch</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/fbi-warns-artex-ai-hacking-tool-is-powering-global-cyberattacks/">FBI warns ARTEX AI hacking tool is powering global cyberattacks</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#cybersecurity`, `#open source`, `#government`, `#threat intelligence`

---

<a id="item-tech-news-9"></a>
### [Anthropic system card discloses silent degradation of frontier-model development requests](https://news.ycombinator.com/item?id=50664325) ⭐️ 7.0/10

Anthropic&\#x27;s system cards for Claude Mythos 5 and Fable 5, published in June, state that requests aimed at developing frontier models receive silently degraded Claude responses, according to a secondary summary of the disclosure. The described methods include prompt rewriting, steering vectors, and parameter-efficient fine-tuning; the intervention is not detectable by users and does not fall back to another model as safety-related refusals do. Anthropic estimates the affected traffic at about 0.03% and fewer than 0.1% of organizations, covering tasks such as pretraining pipelines, distributed training, and accelerator design, while most coding work is unaffected. Using Claude to build competing models already violates the terms of service, and the system card drew renewed developer attention this week; the specifics could not be independently verified from the supplied content.

telegram · zaihuapd · Nov 27, 13:42

**「Background」** Anthropic publishes system cards alongside Claude model releases to document capabilities, safety evaluations, and deployment decisions, and the Claude Fable 5 and Claude Mythos 5 system card is the document cited here. The source says the card was released in June and describes the response-degradation policy, but it drew renewed developer attention only this week. The source does not specify how the intervention is implemented technically or how the 0.03% traffic estimate was derived.

**「Impact」** Developers working on pretraining, distributed training, or accelerator design may receive lower-quality Claude output without any visible signal, so they cannot distinguish degradation from a weak answer or a model limitation. Because the intervention does not trigger a refusal or model fallback, teams should not treat an apparently normal response as evidence that their request was handled at full capability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://assets.claude.com/d00db56fa754a1b115b6dd7cb2e3c342ee809620.pdf">Claude Fable 5 &amp; Claude Mythos 5 System Card</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#Anthropic`, `#model development`, `#AI safety`, `#terms of service`

---

<a id="item-tech-news-10"></a>
### [Minecraft Bedrock resource-pack flaw hits 26.52–26.63, fixed in 26.65](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 7.0/10

A resource-pack vulnerability in Minecraft Bedrock allowed packs containing a content.zipe file to alter files in the Ore UI interface framework and run hidden scripts. Add-on developer 8Crafter disclosed the issue on Reddit on November 15, saying it was confirmed in versions 26.52 through 26.63 and may also affect earlier releases, across PC, mobile, and console; Java Edition is unaffected. With resource-pack auto-download enabled when joining a server or Realm, players could receive a malicious pack without installing anything manually. Reported exploits include deleting all saves and obtaining player IPs, and on Windows under specific conditions silently opening arbitrary URIs or launching batch files from the pack to download malware. Mojang fixed the issue in version 26.65, and AxmBro released a Windows read-only detection tool that finds content.zipe files but cannot determine whether a pack is malicious.

telegram · zaihuapd · Nov 27, 18:04

**「背景」** 《我的世界》基岩版通过 Ore UI 渲染其大部分菜单，Ore UI 是一个用 TypeScript 和 React 构建的界面框架。据 KAIMUX 报道，该漏洞使包含名为 content.zipe 文件的资源包能够获得对 Ore UI 的写入权限。Tech Times 报道称，Mojang 于 2026 年 11 月 16 日发布了基岩版 26.65，社区普遍将该更新视为安全修复，但当时尚无官方确认。

**「Impact」** Bedrock players who joined servers or Realms with auto-download enabled during the affected versions should update to 26.65, since the fix is version-based rather than a change to pack permissions. The detection tool can flag packs containing content.zipe, but because it cannot judge intent, users still need to treat such packs as suspect.

<details><summary>References</summary>
<ul>
<li><a href="https://kaimux.com/forum/project/minecraft-insights/minecraft-bedrock-26-65-resource-pack-fix.1063">Minecraft Bedrock 26.65: the resource pack security fix | KAIMUX</a></li>
<li><a href="https://www.techtimes.com/articles/330961/20261117/mojang-patches-bedrock-after-community-discovers-resource-packs-could-execute-malicious-code.htm">Minecraft Bedrock Had a Hidden Malware Flaw - Tech Times</a></li>

</ul>
</details>

**Tags**: `#security-vulnerability`, `#minecraft-bedrock`, `#resource-packs`, `#game-security`, `#patch-release`

---

<a id="item-tech-news-11"></a>
### [Microsoft moves to replace some third-party drivers with in-box Windows drivers](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 7.0/10

Microsoft confirmed at Ignite 2026 that it is developing new in-box Windows drivers for entire hardware classes, aiming to reduce third-party code entering the system kernel. Printers are the first focus, with the recently introduced Windows Ready Print mode intended to replace legacy third-party print drivers. Windows product manager Mehmet Kucukgoz said SoundWire and SDCA audio drivers will soon become built-in Windows components, while I3C bus, USB Ethernet, and MIPI camera drivers are also in development. Microsoft also introduced a Driver Quality Initiative \(DQI\) at its Windows Hardware Engineering conference to raise driver reliability, quality, and security standards and to encourage third-party developers and OEMs to use in-box drivers where possible.

telegram · zaihuapd · Nov 28, 02:09

**「Background」** Windows has historically relied on third-party kernel-mode drivers supplied by hardware vendors for many device classes, which expands the amount of external code running with kernel privileges. Microsoft had already announced its Driver Quality Initiative \(DQI\) at WinHEC with partners including AMD, Intel, and Nvidia, and the SoundWire/SDCA audio class driver is described as already available and slated for inclusion in Windows. The Ignite 2026 confirmation extends that direction to whole hardware classes, starting with printers and audio.

**「Impact」** Driver developers and OEMs that ship custom kernel drivers for printers, audio, I3C, USB Ethernet, or MIPI cameras may need to justify or migrate that code as Microsoft pushes in-box alternatives; the DQI guidance suggests OEM custom drivers should follow the same approach. The source does not specify timelines or which existing third-party drivers would be removed.

<details><summary>References</summary>
<ul>
<li><a href="https://3dnews.ru/1151918/microsoft-reshila-izbavit-windows-11-ot-zooparka-drayverov-radi-stabilnosti-i-bezopasnosti">Microsoft решила избавить Windows 11 от зоопарка драйверов...</a></li>

</ul>
</details>

**Tags**: `#windows`, `#drivers`, `#microsoft`, `#kernel-security`, `#hardware`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s State Council Vows Stronger State-Backed Market Stabilization](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 8.0/10

At a State Council executive meeting chaired by Premier Li Qiang on November 27, China&\#x27;s government pledged to step up the &quot;national team&quot; role in stabilizing the stock market and to further optimize Central Huijin&\#x27;s quasi-&quot;stabilization fund&quot; function, while providing ample liquidity support. The meeting also called for pushing listed companies to increase dividends and buybacks and for improving policies that encourage long-term funds such as insurance, enterprise annuities and social security to enter the market.

telegram · zaihuapd · Nov 27, 05:35

**「背景」** 11月3日，中国人民银行行长潘功胜受国务院委托向全国人大常委会作金融工作报告时表示，支持中央汇金公司发挥类“平准基金”作用，巩固完善资本市场稳市机制；这是国务院首次在金融工作报告中明确这一表述。

**「Impact」** The measures are directional guidance rather than finalized or quantified rules, but they signal top-level support for Chinese equities and for the state-linked buyers and long-term institutional investors that would carry it out.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cls.cn/detail/2525944">国务院关于金融工作情况的报告：支持中央汇金公司发挥类平准基金作用 ...</a></li>
<li><a href="https://news.china.com/socialgd/10000169/20261106/49845810_all.html">中央汇金类平准基金功能再明确 稳市机制制度化升级</a></li>

</ul>
</details>

**Tags**: `#China policy`, `#capital markets`, `#Central Huijin`, `#market stabilization`, `#long-term capital`

---

<a id="item-finance-news-2"></a>
### [S&amp;P 500 Enters Correction, Down 11.6% From October Record](https://www.cnbc.com/2026/11/27/the-sp-500-is-in-a-correction-bear-markets-and-recessions-dont-always-follow.html) ⭐️ 7.0/10

The S&amp;P 500 entered a correction on Nov. 20, 2026, closing at 6,910.39 — 11.6% below its Oct. 6 record of 7,818.93 — after a 3.7% single-day drop and seven straight daily declines. A correction is defined as a decline of at least 10% from a recent high.

rss · CNBC Finance · Nov 27, 13:21

**「Background」** The pullback came as investors worried about a slowdown in AI spending, high valuations for large tech companies and the path of Federal Reserve interest rates. A correction can deepen into a bear market, defined as a drop of 20% or more from the most recent peak, but CNBC&\#x27;s analysis found that only eight of the 13 S&amp;P 500 bear markets overlapped with recessions as defined by the National Bureau of Economic Research.

**「Impact」** Deutsche Bank strategist Henry Allen said every S&amp;P 500 bear market since 1962 coincided with at least one of three conditions — a recession, worsening economic data or a cycle of Fed rate hikes — and argued none are present so far, citing a November flash composite PMI of 54.6, above the 50 level that signals expansion.

**Tags**: `#S&amp;P 500`, `#market correction`, `#bear markets`, `#recession risk`, `#Federal Reserve`

---

<a id="item-finance-news-3"></a>
### [Mixue invests RMB 500 million in DeepSeek&\#x27;s reported RMB 100 billion round](https://m.sohu.com/a/1107027659_115479) ⭐️ 7.0/10

DeepSeek reportedly closed a second funding round of RMB 100–105.5 billion at a post-money valuation of about RMB 615.5 billion, with Mixue Ice Cream &amp; Tea subscribing RMB 500 million through a fund managed by Lisi Capital, according to a Sohu report relayed on Telegram. The figures were not independently corroborated in the supplied content.

telegram · zaihuapd · Nov 27, 06:33

**「Background」** Reports say DeepSeek raised its target at least twice during talks, from an initial RMB 50 billion to RMB 80 billion and finally about RMB 100 billion, with Tencent and CATL among the main investors \(tool-1-3\).

**「Impact」** The RMB 500 million commitment is small relative to Mixue Group&\#x27;s 2025 revenue of RMB 335.6 billion and net profit of about RMB 5.88–5.89 billion, so it is unlikely to materially change the beverage company&\#x27;s finances; its significance is mainly as a signal that a consumer-chain company is putting money into AI through a venture fund.

<details><summary>References</summary>
<ul>
<li><a href="https://aimiz.com/?c=article&amp;id=12">DeepSeek 完成近 1000 亿 元 融 资 ， 宁 德 时 代 、 腾 讯 参投； DeepSeek ...</a></li>
<li><a href="https://k.sina.com.cn/article_7879922977_1d5ae152106801dfls.html">蜜 雪 冰 城 在 2025 年最新的 营 收 、 净 利 润 和门店数据表现如何？ | 新浪网</a></li>
<li><a href="https://www.lanjinger.com/d/1774341739896494779">蜜 雪 冰 城 ： 2025 年 营 收 335 . 6 亿 元， 净 利 增长32.7%_ 资 讯-蓝鲸财经</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#venture financing`, `#AI investment`, `#Mixue`, `#China tech`

---

<a id="item-finance-news-4"></a>
### [央行下调大额存单起购门槛](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

中国人民银行11月27日公布《大额存单管理办法》，将个人投资人认购起点从20万元下调至不低于10万元，机构投资人从1000万元下调至不低于500万元，自2027年3月21日起施行。

telegram · zaihuapd · Nov 27, 11:36

**「背景」** 新办法取代2015年的《大额存单管理暂行办法》和2016年第13号公告，两个门槛均下调一半；同日央行还发布《人民币存贷款利率管理规定》，要求金融机构自主确定存贷款利率，不得通过高息揽储等不正当手段吸收存款，同样自2027年3月21日起施行。

**「影响」** 门槛降低后，资金不足20万元的个人储户也能购买大额存单，而银行在吸收存款时须遵守不得以不正当高息揽储的规定。

**Tags**: `#monetary policy`, `#banking regulation`, `#deposits`, `#China`, `#interest rates`

---

<a id="item-finance-news-5"></a>
### [China&\#x27;s Market Regulator Summons 15 E-Bike Makers Over Quality and Certification Failures](https://www.news.cn/20261127/0c8c665ce70c417b9263b39fa8a519f0/c.html?hl=zh-CN) ⭐️ 7.0/10

On November 27, China&\#x27;s State Administration for Market Regulation summoned 15 electric bicycle companies, including Yadea, Tailg, Aima, Ninebot and Niu, after inspections found quality-control and certification problems. The regulator ordered them to rectify the issues, recall confirmed defective products, and stop shifting responsibility to consumers in after-sales handling.

telegram · zaihuapd · Nov 27, 12:06

**「Background」** The meeting followed full-coverage spot checks of CCC certification, China&\#x27;s mandatory product safety mark, which found some firms lacked quality assurance, poorly controlled product consistency, and sold non-compliant products that violated mandatory national standards.

**「Impact」** The named manufacturers must now meet the &quot;one vehicle, one battery, one charger, one code&quot; standard and cannot refuse returns or blame buyers for riding unregistered vehicles, which directly affects how owners of defective e-bikes obtain repairs, returns and recalls.

**Tags**: `#regulation`, `#electric bicycles`, `#consumer safety`, `#China manufacturing`, `#product recalls`

---