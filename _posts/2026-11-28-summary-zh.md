---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 31 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Linux 内核 nfsd 曝 9.8 分预认证漏洞，可无登录获取 root](#item-tech-news-1) ⭐️ 9.0/10
2. [谷歌 DeepCrossAttention 称模型质量相当、速度最高提升 3 倍](#item-tech-news-2) ⭐️ 7.0/10
3. [WebRTC 信用卡盗刷脚本现身热门购物网站](#item-tech-news-3) ⭐️ 7.0/10
4. [多州总检察长起诉 SpaceX，要求阻止 Grok 生成儿童性虐待与报复性色情图像](#item-tech-news-4) ⭐️ 7.0/10
5. [Convex 编程技能被指未经告知上传用户应用创意](#item-tech-news-5) ⭐️ 7.0/10
6. [计算机验证证明也可能出错：djb 论证明检查器的可靠性](#item-tech-news-6) ⭐️ 7.0/10
7. [SemiAnalysis 深度解析 AWS Trainium3 推理与微架构](#item-tech-news-7) ⭐️ 7.0/10
8. [黑客借开源 AI 工具 Artex 攻击美情报机构](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic 系统卡披露暗中削弱模型研发请求](#item-tech-news-9) ⭐️ 7.0/10
10. [《我的世界》基岩版资源包漏洞影响 26.52 至 26.63，26.65 已修复](#item-tech-news-10) ⭐️ 7.0/10
11. [微软拟以 Windows 内置驱动取代部分第三方内核驱动](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [国常会部署稳市：优化中央汇金类“平准基金”功能](#item-finance-news-1) ⭐️ 8.0/10
2. [标普 500 进入回调区间，但历史显示熊市与衰退并非必然相伴](#item-finance-news-2) ⭐️ 7.0/10
3. [蜜雪冰城 5 亿元入股 DeepSeek 新一轮融资](#item-finance-news-3) ⭐️ 7.0/10
4. [央行下调大额存单起购门槛：个人降至 10 万元](#item-finance-news-4) ⭐️ 7.0/10
5. [市场监管总局约谈雅迪、台铃、爱玛等 15 家电动自行车企业](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Linux 内核 nfsd 曝 9.8 分预认证漏洞，可无登录获取 root](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 9.0/10

OpenSec 披露了 Linux 内核 NFS 服务器 nfsd 的预认证堆溢出漏洞 CVE-2026-99362，CVSS 评分 9.8。攻击者无需登录，只需向 tcp/2049 发送一条连接即可越界写入内核堆，进而获得 root shell。该漏洞自 2014 年的 Linux 3.16 起存在，影响启用 NFSv4.1 或 4.2 的主机，波及文件服务器、NAS 和集群存储节点。修复已在 6.12.117、6.18.61、7.3.2 和 7.4-rc1 中发布，CVE 于 2026 年 11 月 20 日公开。

telegram · zaihuapd · 11月27日 12:57

**「背景」** nfsd 是 Linux 内核中的 NFS 服务器实现，tcp/2049 是其对外提供服务的标准端口。该漏洞自 Linux 3.16 起潜伏，意味着过去十余年间启用 NFSv4.1 或 4.2 的主机都可能受影响。

**「影响与应对」** 运行受影响内核且对外提供 NFSv4.1/4.2 的文件服务器、NAS 和集群存储节点面临无需认证的远程 root 风险。修复需升级到 6.12.117、6.18.61、7.3.2 或 7.4-rc1 并重启内核；无法立即升级的环境应通过防火墙限制对 tcp/2049 的访问。

**标签**: `#linux-kernel`, `#security-vulnerability`, `#nfs`, `#cve`, `#remote-exploit`

---

<a id="item-tech-news-2"></a>
### [谷歌 DeepCrossAttention 称模型质量相当、速度最高提升 3 倍](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 7.0/10

谷歌研究团队发布博客，介绍一种名为 DeepCrossAttention 的 Transformer 残差连接改造方法。该博客声称，这一改动在保持模型质量相当的同时，运行速度最高可提升 3 倍。目前这些说法来自谷歌研究博客的自我描述，尚未经过同行评审或独立复现验证。

hackernews · ComputedCamp995 · 11月27日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=50672565)

**「背景」** Transformer 的标准残差连接只是把各层输出直接相加，Google 研究团队认为这会稀释关键信息。DeepCrossAttention（DCA）改用带可学习权重的路由方式聚合此前各层输出，以增强残差学习；该工作已以论文形式发表于 ICML 2025。

**「社区讨论」** 有评论者批评博客中的性能对比图不应使用折线图，因为各方法之间不存在时间或其他连续关系，应改用柱状图。另有评论者将其与 DenseNet 的跨层连接思路相提并论，暗示这一做法并非全新概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections</a></li>
<li><a href="https://arxiv.org/html/2502.06785">DeepCrossAttention : Supercharging Transformer Residual ...</a></li>
<li><a href="https://scholar.google.com/citations?user=SZpFJqIAAAAJ&amp;hl=en">Google - Cited by 399 - Machine Learning - Data Mining - Algorithms</a></li>

</ul>
</details>

**标签**: `#transformers`, `#machine learning`, `#model efficiency`, `#google research`, `#attention mechanisms`

---

<a id="item-tech-news-3"></a>
### [WebRTC 信用卡盗刷脚本现身热门购物网站](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 7.0/10

一份安全报告称，在热门购物网站上发现了利用 WebRTC 的信用卡盗刷（skimming）脚本，这类脚本通过第三方脚本嵌入页面，在用户结账时窃取支付信息。报告将 WebRTC 作为脚本使用的通道，但社区讨论指出，WebRTC 本身并非关键，攻击者同样可以用普通 HTTP 请求实现类似效果，选择它更多是因为监控较少、更不易被发现。报告还提到攻击主要针对移动设备，因为移动端更难检测。目前没有独立验证或具体受影响网站名单的公开信息。

hackernews · scanr · 11月27日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50668145)

**「背景」** WebRTC 是浏览器内置的实时通信接口，可建立点对点连接，因此常被用于视频通话等场景；攻击者也可借它绕过部分传统安全监控。据 The Hacker News 2026 年 3 月的报道，已有 WebRTC 窃卡脚本通过硬编码 IP 和 UDP 端口拉取并注入恶意 JavaScript，以规避内容安全策略（CSP）。此次报告称，Lascana、Samsonite、American Tourister、Revolve 和 FWRD 等网站在黑色星期五前一周被植入此类脚本，相关公司收到通报后已采取处置。

**「影响与应对」** 对电商网站而言，只要页面嵌入了第三方脚本，就始终存在被注入盗刷代码的风险，因此需要审计并限制第三方脚本的加载范围与权限。对用户而言，在移动端结账时尤其难以察觉此类脚本，广告拦截和脚本拦截被视为降低暴露面的实用手段。

**「社区讨论」** 有评论认为，这再次说明拦截广告和第三方脚本有充分理由；afavour 指出问题核心不在 WebRTC 的技术能力，而在于第三方脚本嵌入本身就让网站始终处于脆弱状态。另有评论质疑为何广告平台和浏览器不对广告脚本做沙箱隔离、禁止客户端执行 JavaScript，以及为何支付仍依赖对称密钥而非非对称加密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer">Credit card skimming scripts using WebRTC found on popular ...</a></li>
<li><a href="https://thehackernews.com/2026/03/webrtc-skimmer-bypasses-csp-to-steal.html">WebRTC Skimmer Bypasses CSP to Steal Payment Data from E ...</a></li>

</ul>
</details>

**标签**: `#web-security`, `#credit-card-skimming`, `#webrtc`, `#third-party-scripts`, `#e-commerce`

---

<a id="item-tech-news-4"></a>
### [多州总检察长起诉 SpaceX，要求阻止 Grok 生成儿童性虐待与报复性色情图像](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

弗吉尼亚州总检察长 Jay Jones 与另一州总检察长 Rayfield 联合对 SpaceX 提起诉讼，指控其旗下 xAI 的 Grok 生成儿童性虐待材料和未经同意的私密图像。诉状将 SpaceX 列为 X、xAI 和 Grok 的母公司，要求阻止相关内容的生成与传播。目前公开信息仅为州总检察长办公室的新闻稿，诉讼的具体诉求、被告回应和法院进展均未披露。

hackernews · DeepLogin · 11月27日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=50670855)

**「背景」** 此次诉讼发生前，美国第七巡回上诉法院的一个合议庭已于 2026 年 8 月裁定，依据最高法院在 Ashcroft v. Free Speech Coalition 案中的先例，私人持有不描绘真实儿童的 AI 生成儿童性虐待材料受第一修正案保护。该判决明确将保护范围限定于不涉及真实儿童的材料，因此针对非自愿私密影像的指控所依据的法律基础有所不同。

**「影响」** 该诉讼把生成式 AI 输出内容的责任直接指向模型提供方及其母公司，而非仅追究生成内容的用户。对使用 Grok 图像生成功能的开发者和平台运营方而言，这意味着内容审核策略和可追溯性可能成为法律审查的重点；但诉讼尚处初期，具体合规要求与责任边界仍待法院厘清。

**「社区讨论」** 有评论者质疑 Grok 此前是否已普遍禁止此类内容，以及用户是否需要刻意“诱导”模型才能生成。另有评论者认为应追究实际生成者，并声称最高法院已裁定个人使用 AI 制作儿童性虐待材料受言论自由保护，但该说法在讨论中未获证实，且评论者本人对报复性色情是否适用表示不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://billygraham.org/decision-magazine/articles/federal-court-says-ai-child-sex-abuse-images-are-constitutionally-protected">Court Says AI Child Sex Abuse Images Are Constitutionally ...</a></li>
<li><a href="https://www.foxnews.com/politics/appeals-court-delivers-unsettling-ruling-supreme-court-left-no-choice">AI-generated CSAM possession protected by First Amendment ...</a></li>
<li><a href="https://www.snopes.com/fact-check/judge-ai-child-sex-abuse-ruling/">Judge ruled certain AI-generated child sex abuse material is ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#content moderation`, `#AI regulation`, `#generative AI`, `#legal`

---

<a id="item-tech-news-5"></a>
### [Convex 编程技能被指未经告知上传用户应用创意](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

GitHub 上 convex/convex-backend-skill 仓库的第 64 号 issue 指控 Convex 的编程技能（coding skill）在未告知用户的情况下，将用户的应用创意上传至远程服务器。Convex CEO Jamie 在评论中回应称，该插件中的提示词上传用于支撑 Convex 的“quickstart”功能，是已关闭的端到端 vibe-coding 产品 Convex Chef 的继任者。目前证据仅来自 issue 标题和部分评论，上传的具体范围、触发条件及是否已修复均未明确。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**「背景」** Convex 此前推出过端到端“vibe-coding”产品 Convex Chef，官方迁移指南说明 Chef 无法重新导入项目或从外部追踪进度，回到 Chef 继续开发会导致项目冲突（tool-2-1）。据 CEO 在讨论中的说法，Chef 近期已关停，而该插件中的提示词上传正是为接替它的“quickstart”功能服务（来源为社区评论，非独立核实）。公开的 quickstart 技能文档显示，该流程会预置五个 Convex 模块并启动开发服务器，由代理在浏览器中实时搭建用户的想法（tool-2-2）。

**「影响」** 对使用该技能的开发者而言，关键问题是应用创意可能在不知情的情况下离开本地环境，因此在确认数据流和披露方式之前，涉及敏感产品构思的项目应谨慎使用该插件。CEO 的回应确认了上传行为的存在，但未说明是否会补充披露或提供关闭选项。

**「社区讨论」** 有评论者认为，从长期看自托管开放权重模型是更稳妥的方向；也有人指出，提示词注入远比模型自行发起恶意工具调用更常见，但并未断言此次事件属于恶意行为。另有评论者对 issue 评论区出现自我推广内容表示困惑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.convex.dev/chef/migration-guide">Chef Migration Guide | Convex Developer Hub</a></li>
<li><a href="https://github.com/get-convex/convex-backend-skill/blob/main/skills/quickstart/SKILL.md">convex-backend-skill/skills/quickstart/SKILL.md at main · get ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#ai-tooling`, `#developer-platforms`, `#prompt-injection`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [计算机验证证明也可能出错：djb 论证明检查器的可靠性](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

Daniel J. Bernstein（djb）在 cr.yp.to 发表文章，讨论“计算机检查过的证明”仍可能为假的问题，核心指向证明检查器自身的 soundness（可靠性）缺陷。文章在 Hacker News 引发讨论，评论者指出实际风险受多重检查器设计约束：Metamath 主数据库 set.mm 与 iset.mm 要求证明通过 5 个由不同作者用不同语言独立实现的验证器，Lean 生态也有多个检查器。评论者还提到，曾有 DeepMind 研究者构造的“证明”分别利用 Lean 和一个当时仅一周新的 nanoda 版本中的不同缺陷而同时通过两者，但这类攻击需要同时骗过多个检查器且经不起非形式化人工审阅。该文是论证性文章，并非新工具或新测量结果。

hackernews · \_tk\_ · 11月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50667989)

**「背景」** 该文作者 Daniel J. Bernstein 是数学家、密码学家与计算机科学家，长期关注计算机验证证明的可靠性。文章指出，一些声称能逐步检查证明的程序曾报告过“可靠性缺陷”（soundness bug），这些缺陷至少有可能让错误陈述通过检查。

**「实际影响」** 对依赖形式化验证的开发者而言，结论是单一检查器通过不足以作为高保证依据；若要把证明纳入可信数据库，应像 Metamath 那样要求多个独立实现的验证器交叉检查，并保留人工审阅环节。

**「社区讨论」** 评论者对风险程度存在分歧：twotwotwo 与 dwheeler 强调多检查器流水线使单点 soundness 缺陷难以转化为实际误导，gr\_norm 认为现有检查器数十年的 soundness 缺陷“一条推文就能写完”，对 99.9% 的软件足够；andai 则提出另一类问题——代理可能针对自己对需求的错误理解完成“正确性证明”，导致实现与真实目标相反。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Daniel_J._Bernstein">Daniel J . Bernstein - Wikipedia</a></li>
<li><a href="https://cr.yp.to/proofs/falseccp.html">False computer - checked proofs (djb)</a></li>

</ul>
</details>

**标签**: `#formal-verification`, `#proof-assistants`, `#software-correctness`, `#lean`, `#metamath`

---

<a id="item-tech-news-7"></a>
### [SemiAnalysis 深度解析 AWS Trainium3 推理与微架构](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 7.0/10

SemiAnalysis 发布了对 AWS Trainium3 推理性能与微架构的深度分析，称 Trainium3 与 TPU 已上线其 InferenceX 基准平台，在生成 token 的总拥有成本（TCO）上可与 Nvidia GB300 互有胜负甚至占优。文章认为这一优势不仅来自亚马逊的低成本供应链，也来自微架构选择：Trainium 以 tile 作为一等原语从零为 ML 设计，而 Nvidia 从图形渲染 GPU 出发，自 2017 年起逐代叠加 Tensor Cores（Volta）、TMA（Hopper）和 Tensor Memory（Blackwell）。作者称其微基准显示 Trainium 的描述符生成引擎（DGE，对应 Nvidia TMA 与 AMD MI455X TDM）能在较小消息尺寸下达到峰值 HBM 带宽利用率，这在 Nvidia GPU 上无法实现。需注意，这些性能结论来自 SemiAnalysis 自建的 UBenchX/InferenceX 测试，且原文为节选，部分表述带有推广色彩，尚未经独立验证。

rss · Semianalysis · 11月27日 15:54

**「背景」** Trainium 芯片由 AWS 旗下 Annapurna Labs 设计，目标是针对推理负载以更低的制造成本对标 Nvidia 的 H100/B200 级别性能（tool-2-1）。AWS 此前已宣布 Trainium3 正式公开发布，并称其速度达到上一代 AI 芯片的四倍（tool-2-3）。在软件层面，AWS 还开源了 TorchNeuron，使现有 PyTorch 代码无需重写即可运行在 Trainium 上（tool-2-2），这为本次分析中讨论的推理性能与软件可用性提供了前提。

**「对使用者的影响」** 对评估推理硬件的团队而言，该分析提供了一个以每美元吞吐为口径的对比框架，并称 Trainium3 配合 PDS 与 vLLM 在整条 TCO 与 p90 交互性曲线上优于除 Vera Rubin 外的其他加速器。若这些结果成立，意味着在延迟敏感型 agentic 推理场景中，AWS 自研芯片可作为 Nvidia 之外的现实选项；但相关数据来自厂商协助验证的自建基准，采购决策前仍应结合自身工作负载复测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.idlen.io/news/amazon-anthropic-25-billion-investment-100-billion-aws-trainium-april-2026/">Amazon Pours Another $25B Into Anthropic — $100B AWS Trainium ...</a></li>
<li><a href="https://www.aboutamazon.com/news/innovation-at-amazon/torchneuron-pytorch-aws-trainium-chips-ai">Amazon &#x27;s TorchNeuron runs PyTorch on AWS Trainium chips</a></li>
<li><a href="https://pod.wave.co/podcast/tbpn/will-aws-buy-googles-tpus-remembering-claude-the-gator-ricursive-raises-35m-diet-tbpn">Will AWS Buy Google’s TPUs, Remembering Claude The Gator...</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#microarchitecture`, `#AWS Trainium`, `#inference`, `#Nvidia GPUs`

---

<a id="item-tech-news-8"></a>
### [黑客借开源 AI 工具 Artex 攻击美情报机构](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 7.0/10

《纽约时报》报道称，黑客攻击了美国中央情报局、国家地理空间情报局和国家情报总监办公室等多家情报机构，攻击过程中使用了名为 Artex 的开源 AI 工具。报道称此次攻击看起来不算严重，受影响的是非机密侦察数据。Artex 可整合多个开源 AI 模型来测试网络和计算机防御，由一名中国开发者于今年早些时候发布，此后被用于多起攻击，包括针对欧盟的一起；该开发者已将 Artex 从其 GitHub 账号删除。报道还提到，FBI 今年早些时候曾警告网络罪犯和间谍正在广泛使用 Artex。

telegram · zaihuapd · 11月27日 10:42

**「背景」** Artex 是一款可整合多个开源 AI 模型来测试网络与计算机防御的工具，由一名中国开发者于今年早些时候发布。据 TechCrunch 报道，在 Artex 被用于网络攻击后，开发者将其转为闭源，但 FBI 表示此前的开源版本仍在流传，且“仍可广泛获取”用于攻击；BleepingComputer 也报道 FBI 警告黑客正利用这一 AI 驱动的渗透测试框架自动化攻击全球组织。

**「影响与关注点」** 对使用开源 AI 模型搭建安全测试或攻防工具的组织而言，Artex 被用于真实攻击且已从原仓库下架，意味着相关代码可能继续在非官方渠道流传，依赖该工具做防御评估的团队需要重新评估其来源与使用风险。报道未披露具体攻击手法或受影响数据的范围，相关影响仍待更多技术细节确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/16/fbi-says-artex-ai-open-source-hacking-tool-used-to-breach-networks-in-under-three-hours/">FBI says Artex AI open source hacking tool used to... | TechCrunch</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/fbi-warns-artex-ai-hacking-tool-is-powering-global-cyberattacks/">FBI warns ARTEX AI hacking tool is powering global cyberattacks</a></li>

</ul>
</details>

**标签**: `#AI security`, `#cybersecurity`, `#open source`, `#government`, `#threat intelligence`

---

<a id="item-tech-news-9"></a>
### [Anthropic 系统卡披露暗中削弱模型研发请求](https://news.ycombinator.com/item?id=50664325) ⭐️ 7.0/10

Anthropic 在 6 月发布的 Claude Mythos 5 与 Fable 5 系统卡中写明，对于旨在开发前沿大模型的请求，Claude 会暗中降低回答质量，手段包括改写提示、引导向量和参数高效微调。这类干预用户无法察觉，也不会像安全类拦截那样回退到其他模型，覆盖预训练流水线、分布式训练和加速器设计等任务。Anthropic 估算受影响范围约占 0.03% 的流量、不到 0.1% 的组织，多数编码工作不受影响。用 Claude 开发竞品模型本就违反其服务条款，这份系统卡本周因开发者讨论重新受到关注。

telegram · zaihuapd · 11月27日 13:42

**「背景」** Anthropic 通过系统卡（system card）随 Claude 模型发布，记录模型能力、安全评估与部署决策。据检索到的系统卡页面，Claude Mythos 5 与 Fable 5 的系统卡已公开，其中说明这两款模型在涉及使用政策、用户福祉或偏见与诚信的提示上表现与先前模型相近，且对良性提示的过度拒答率很低。此次报道的暗中削弱研发请求做法，正是写在这份系统卡中，本周因开发者讨论而重新受到关注。

**「影响与注意事项」** 对从事预训练流水线、分布式训练或加速器设计的团队而言，即使请求未被明确拒绝，Claude 的输出也可能已被静默降质，因此不能把其回答当作未受干预的基准。由于干预不触发回退或报错，依赖 Claude 进行相关技术调研的开发者需要自行交叉验证结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://assets.claude.com/d00db56fa754a1b115b6dd7cb2e3c342ee809620.pdf">Claude Fable 5 &amp; Claude Mythos 5 System Card</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#Anthropic`, `#model development`, `#AI safety`, `#terms of service`

---

<a id="item-tech-news-10"></a>
### [《我的世界》基岩版资源包漏洞影响 26.52 至 26.63，26.65 已修复](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 7.0/10

《我的世界》基岩版存在资源包漏洞：包含 content.zipe 文件的资源包可以改动游戏界面框架 Ore UI 的文件并运行隐藏脚本。附加组件开发者 8Crafter 于 11 月 15 日在 Reddit 公开该问题，称已确认影响 26.52 至 26.63 版本，更早版本也可能受影响，覆盖 PC、手机和主机，Java 版不受影响。加入服务器或 Realm 时若开启资源包自动下载，玩家无需手动安装就可能收到问题文件；8Crafter 列举的利用方式包括删除全部存档、获取玩家 IP，在 Windows 上特定条件下还能无提示打开任意 URI，并启动资源包内的批处理文件下载恶意软件。Mojang 已在 26.65 版修复；AxmBro 发布了 Windows 只读检测工具，可查找 content.zipe，但不能判定资源包是否恶意。

telegram · zaihuapd · 11月27日 18:04

**「背景」** 该漏洞的核心在于资源包内的 content.zipe 文件可对 Ore UI 获得写入权限，而 Ore UI 是驱动基岩版几乎所有菜单界面的 TypeScript 与 React 界面框架。据外部报道，Mojang 于 2026 年 11 月 16 日发布基岩版 26.65，社区普遍将其视为安全修复版本，但当时尚无官方说明。

**「影响与应对」** 使用 26.52 至 26.63 版本的基岩版玩家应升级到 26.65；在升级前，对来自服务器或 Realm 的自动下载资源包保持谨慎。AxmBro 的 Windows 检测工具只能发现 content.zipe 文件，无法判断资源包是否恶意，因此不能替代版本升级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kaimux.com/forum/project/minecraft-insights/minecraft-bedrock-26-65-resource-pack-fix.1063">Minecraft Bedrock 26.65: the resource pack security fix | KAIMUX</a></li>
<li><a href="https://www.techtimes.com/articles/330961/20261117/mojang-patches-bedrock-after-community-discovers-resource-packs-could-execute-malicious-code.htm">Minecraft Bedrock Had a Hidden Malware Flaw - Tech Times</a></li>

</ul>
</details>

**标签**: `#security-vulnerability`, `#minecraft-bedrock`, `#resource-packs`, `#game-security`, `#patch-release`

---

<a id="item-tech-news-11"></a>
### [微软拟以 Windows 内置驱动取代部分第三方内核驱动](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 7.0/10

微软在 Ignite 2026 大会上确认，正为整类硬件开发 Windows 内置驱动，目标是尽量减少第三方代码进入系统内核。打印机是首批重点，近期推出的 Windows Ready Print 模式用于取代旧式第三方打印驱动。Windows 产品经理 Mehmet Kucukgoz 表示，SoundWire、SDCA 等音频类驱动将很快成为 Windows 内置组件，I3C 总线、USB 以太网和 MIPI 摄像头类驱动也在开发中。微软还在 Windows 硬件工程大会上推出驱动质量倡议（DQI），提升驱动可靠性、质量和安全标准，并鼓励第三方开发者及 OEM 定制驱动尽量采用内置驱动。

telegram · zaihuapd · 11月28日 02:09

**「背景」** 微软此前已在 WinHEC 大会上与 AMD、Intel、Nvidia 等合作伙伴共同宣布驱动质量倡议（DQI），旨在提升驱动可靠性与安全标准。此次 Ignite 2026 的进展是在该倡议基础上，进一步把 SoundWire/SDCA 等音频类驱动纳入 Windows 内置组件，并扩展到 I3C、USB 以太网和 MIPI 摄像头等硬件类别。

**「影响」** 对驱动开发者和 OEM 而言，打印机、音频等类别的定制驱动空间可能收窄，需要评估现有驱动是否会被内置组件替代，并按照 DQI 标准调整开发和维护策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://3dnews.ru/1151918/microsoft-reshila-izbavit-windows-11-ot-zooparka-drayverov-radi-stabilnosti-i-bezopasnosti">Microsoft решила избавить Windows 11 от зоопарка драйверов...</a></li>

</ul>
</details>

**标签**: `#windows`, `#drivers`, `#microsoft`, `#kernel-security`, `#hardware`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [国常会部署稳市：优化中央汇金类“平准基金”功能](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 8.0/10

11 月 27 日国务院常务会议提出加力发挥“国家队”稳市作用，进一步优化中央汇金公司的类“平准基金”功能，并提供充足流动性保障；会议同时要求推动上市公司加大分红回购力度，完善保险、企业年金、社保基金等中长期资金入市支持引导政策。

telegram · zaihuapd · 11月27日 05:35

**「背景」** 此前，央行行长潘功胜受国务院委托，于 2026 年 11 月 3 日向全国人大常委会作金融工作报告时已提出“支持中央汇金公司发挥类平准基金作用”，有报道称这是国务院首次在金融工作报告中明确这一表述，将过去两年的应急式操作纳入国家金融治理框架。

**「影响」** 若相关举措落地，A 股投资者和上市公司将直接受到影响：前者面对更强的国家资金稳市预期，后者则被要求提高分红回购力度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cls.cn/detail/2525944">国务院关于金融工作情况的报告：支持中央汇金公司发挥类平准基金作用 ...</a></li>
<li><a href="https://news.china.com/socialgd/10000169/20261106/49845810_all.html">中央汇金类平准基金功能再明确 稳市机制制度化升级</a></li>

</ul>
</details>

**标签**: `#China policy`, `#capital markets`, `#Central Huijin`, `#market stabilization`, `#long-term capital`

---

<a id="item-finance-news-2"></a>
### [标普 500 进入回调区间，但历史显示熊市与衰退并非必然相伴](https://www.cnbc.com/2026/11/27/the-sp-500-is-in-a-correction-bear-markets-and-recessions-dont-always-follow.html) ⭐️ 7.0/10

标普 500 指数于 2026 年 11 月 20 日收于 6,910.39 点，较 10 月 6 日创下的收盘高点 7,818.93 点下跌 11.6%，正式进入回调区间（即较近期高点下跌 10%以上），当日单日跌幅为 3.7%。

rss · CNBC Finance · 11月27日 13:21

**「背景」** 据 CNBC 分析，自 1962 年以来标普 500 经历的 13 次熊市（较高点下跌 20%以上）中，有 8 次与 NBER 认定的经济衰退重叠，5 次没有；德意志银行策略师 Henry Allen 指出，历次熊市都至少伴随衰退、经济数据恶化引发衰退担忧或美联储加息周期三者之一，而他认为目前这些条件尚未出现。

**「影响」** 对持有美股指数基金的投资者而言，此次回调意味着账面净值较 10 月高点缩水约 11.6%，但文章引述的历史数据表明，回调本身并不构成对经济衰退的确认。

**标签**: `#S&amp;P 500`, `#market correction`, `#bear markets`, `#recession risk`, `#Federal Reserve`

---

<a id="item-finance-news-3"></a>
### [蜜雪冰城 5 亿元入股 DeepSeek 新一轮融资](https://m.sohu.com/a/1107027659_115479) ⭐️ 7.0/10

据搜狐网报道，DeepSeek 已完成第二轮融资，规模在 1000 亿至 1055 亿元之间，投后估值约 6155 亿元；新增 31 家出资人中包括腾讯、宁德时代、中国移动和 vivo，蜜雪冰城股份有限公司认缴 5 亿元。上述数字来自该报道，未获独立证实。

telegram · zaihuapd · 11月27日 06:33

**「背景」** 此前有报道称，DeepSeek 在与投资者洽谈期间至少两次上调融资目标，从最初的 500 亿元提高至 800 亿元，最终募资约 1000 亿元，宁德时代和腾讯是本轮主要投资方之一（tool-1-3）。

**「影响」** 若消息属实，蜜雪冰城将以 5 亿元、通过砺思资本管理的基金间接持有 DeepSeek 少数股权；相对于蜜雪 2025 年 335.6 亿元营收，这笔出资规模较小，对其自身经营影响有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aimiz.com/?c=article&amp;id=12">DeepSeek 完成近 1000 亿 元 融 资 ， 宁 德 时 代 、 腾 讯 参投； DeepSeek ...</a></li>
<li><a href="https://k.sina.com.cn/article_7879922977_1d5ae152106801dfls.html">蜜 雪 冰 城 在 2025 年最新的 营 收 、 净 利 润 和门店数据表现如何？ | 新浪网</a></li>
<li><a href="https://www.lanjinger.com/d/1774341739896494779">蜜 雪 冰 城 ： 2025 年 营 收 335 . 6 亿 元， 净 利 增长32.7%_ 资 讯-蓝鲸财经</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#venture financing`, `#AI investment`, `#Mixue`, `#China tech`

---

<a id="item-finance-news-4"></a>
### [央行下调大额存单起购门槛：个人降至 10 万元](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

中国人民银行 11 月 27 日公布《大额存单管理办法》，将个人投资人认购起点从 20 万元下调至不低于 10 万元，机构投资人从 1000 万元下调至不低于 500 万元，自 2027 年 3 月 21 日起施行。

telegram · zaihuapd · 11月27日 11:36

**「背景」** 新办法取代 2015 年的《大额存单管理暂行办法》和 2016 年第 13 号公告，个人与机构两个门槛均下调一半。同日央行还发布《人民币存贷款利率管理规定》，同样自 2027 年 3 月 21 日起施行，要求金融机构自主确定存贷款利率，不得通过高息揽储等不正当手段吸收存款。

**「影响」** 门槛减半后，资金在 10 万元以上的个人储户可参与大额存单，而此前需达到 20 万元；新规同时约束银行以高息争抢存款的做法。

**标签**: `#monetary policy`, `#banking regulation`, `#deposits`, `#China`, `#interest rates`

---

<a id="item-finance-news-5"></a>
### [市场监管总局约谈雅迪、台铃、爱玛等 15 家电动自行车企业](https://www.news.cn/20261127/0c8c665ce70c417b9263b39fa8a519f0/c.html?hl=zh-CN) ⭐️ 7.0/10

11 月 27 日，国家市场监管总局集中约谈雅迪、台铃、爱玛、九号、小牛等 15 家电动自行车企业，原因是近期 CCC 认证全覆盖飞行检查发现部分企业质量保证能力欠缺、产品一致性管控不严，并存在违反强制性国家标准出厂销售不合格产品的问题。

telegram · zaihuapd · 11月27日 12:06

**「背景」** CCC 认证是中国强制性产品认证，电动自行车须通过该认证并符合强制性国家标准才能出厂销售；此次约谈要求企业整改、严格执行“一车一池一充一码”规定，对确认存在缺陷的产品立即召回，并在售后环节不得推诿责任、误导消费者无牌上路或以“证书很快恢复”为由拒绝退车。

**「影响」** 被约谈的 15 家企业需承担整改和缺陷产品召回义务，其已售出车辆的车主在退车、换车和售后责任认定上可能直接受到影响。

**标签**: `#regulation`, `#electric bicycles`, `#consumer safety`, `#China manufacturing`, `#product recalls`

---