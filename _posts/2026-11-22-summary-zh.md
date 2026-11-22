---
layout: default
title: "Horizon Summary: 2026-11-22 (ZH)"
date: 2026-11-22
lang: zh
---

> 从 23 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [黎曼猜想形式化证明据称通过 Lean 验证](#item-tech-news-1) ⭐️ 10.0/10
2. [GnuPG/GPGME 旧版本被披露远程代码执行漏洞](#item-tech-news-2) ⭐️ 8.0/10
3. [浙江大学在超导芯片上首次真机实现 QRAM](#item-tech-news-3) ⭐️ 8.0/10
4. [显示器内置 USB 集线器如何拖慢以太网下载速度](#item-tech-news-4) ⭐️ 7.0/10
5. [mod\_wsgi 作者发布 AI 辅助 Rust 服务器 Muru](#item-tech-news-5) ⭐️ 7.0/10
6. [微软发布 RDMA over USB4 开发者预览，多台 PC 可合跑一个本地 AI 模型](#item-tech-news-6) ⭐️ 7.0/10
7. [OpenRouter 警告 MiniMax 模型提示词疑遭第三方读取](#item-tech-news-7) ⭐️ 7.0/10
8. [daraxonrasib 一线联合化疗早期数据：确认缓解率 60.7%](#item-tech-news-8) ⭐️ 7.0/10
9. [特斯拉海外推送 FSD v15，新增 Reality View 可视化](#item-tech-news-9) ⭐️ 7.0/10

**科技博客**
1. [好代码的关键：少犯灾难性错误](#item-tech-blog-1) ⭐️ 5.0/10

**财经新闻**
1. [中国借峰会扩大全球影响力：习近平今年已接待逾 40 位国家元首](#item-finance-news-1) ⭐️ 7.0/10
2. [特朗普称拟对海外建 AI 数据中心的美国公司征“巨额税款”](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [黎曼猜想形式化证明据称通过 Lean 验证](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 10.0/10

据 Telegram 消息，Levent Alpöge 于 2026 年 11 月 20 日发布黎曼猜想的 Lean 形式化证明，代码库约 1700 万行。次日，Lean FRO 与 Mathlib Initiative 联合声明称，社区已确认该命题与 Mathlib 的 RiemannHypothesis 一致、代码库可无错编译，并有多个独立证明检查器验证证明有效。上述内容来自一条简短社交平台帖文，具体技术细节需以所链接的 Lean community blog 原文为准，目前尚无法在此独立核实。

telegram · zaihuapd · 11月21日 16:48

**「背景」** 黎曼猜想是数学界最著名的未解难题之一，其陈述早已被收录进 Lean 数学库 Mathlib，作为可被形式化引用的命题。此次事件的核心是 Levent Alpöge 于 2026 年 11 月 20 日发布的约 1700 万行 Lean 代码库，随后 Lean FRO 与 Mathlib Initiative 于 11 月 21 日联合认证该命题与 Mathlib 中的 RiemannHypothesis 一致、代码可无错编译，并通过多个独立检查器验证。

**「影响」** 若认证属实，数学界与形式化验证社区将获得一个与 Mathlib 现有命题对齐、可编译且经多个独立检查器验证的黎曼猜想形式化证明，后续工作可直接基于该代码库复核与复用。由于消息仅给出结论性描述，使用者仍应查阅原始代码库与检查器记录，确认所验证命题的确切表述。

**「社区讨论」** 有评论认为，随着多种语言、多个内核及各自一致性证明的出现，证明因内核缺陷而失效的可能性已很小；也有人提醒，过去曾有不成立的 Collatz 反证通过某个所谓独立检查器，因此检查器的独立性不宜高估，不过本次有人类专家参与降低了这一风险。另有评论强调 Alpöge 在借助 AI 完成形式化方面的作用，并讨论此类大结果是否会引出更大的数学问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leanprover-community.github.io/blog/posts/riemann-hypothesis/">Lean verification of the Riemann Hypothesis | Lean community blog</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#Lean`, `#mathematics`, `#Riemann Hypothesis`, `#open source`

---

<a id="item-tech-news-2"></a>
### [GnuPG/GPGME 旧版本被披露远程代码执行漏洞](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

GnuPG 项目于 2026 年 11 月 20 日披露了 GPGME 中的一个漏洞，影响 2.3.0 之前的所有版本，无论以共享库、DLL 还是静态链接方式使用。公告称该漏洞具有远程代码执行潜力，受影响软件包括 Gpg4win、GnuPG Desktop、多数邮件客户端、部分 XMPP 客户端、Samba 和 Flatpak。披露方原定 11 月 25 日协调公开，但因 GitLab 需提前应对另一漏洞而提前发布；GitLab 已于 11 月 12 日获知此事并提供了 Omnibus 补丁。社区评论指出其本质是双重释放缺陷，对“RCE 链”的表述存在争议。

hackernews · gdgghhhhh · 11月21日 08:32 · [社区讨论](https://news.ycombinator.com/item?id=50587208)

**「背景」** GPGME 是供应用程序调用 GnuPG 加密功能的库，邮件客户端、Samba、Flatpak 等软件都依赖它。GnuPG 公告称，该缺陷是一个双重释放（double free），可被用来从应用中窃取数据，例如通过发送签名数据触发；公告同时表示不能排除将其用于远程代码执行（RCE）的可能。修复版本为 GPGME 2.3.1，2.3.0 从未公开发布；原定 11 月 25 日协调披露，因新的 Ruby2Shell 漏洞迫使 GitLab 提前更新，披露提前至 11 月 20 日。

**「影响与应对」** 使用 GPGME 2.3.0 之前版本的应用需升级或打补丁，GitLab 已发布 Omnibus 相关补丁。评论提到 Red Hat 五年前已在其打包中修复该问题而上游未跟进，因此部分发行版用户可能不受影响，但自行编译或静态链接的软件仍需核查。

**「社区讨论」** 有评论者认为这是双重释放缺陷而非完整的 RCE 链，质疑漏洞报告是否刻意夸大；也有人指出 Red Hat 五年前已修复但上游遗漏。另有用户询问该漏洞是否仅存在于 gpgme、不影响 apt 等工具，尚未得到确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html">[Announce] GnuPG Security Advisory for GPGME ...</a></li>
<li><a href="https://thehackernews.com/2026/11/gnupg-warns-critical-gpgme-flaw-could.html">GnuPG Warns Critical GPGME Flaw Could Expose App Data via...</a></li>
<li><a href="https://www.phoronix.com/news/GnuPG-GPGME-Critical">GnuPG&#x27;s GPGME Affected By Critical Security Bug In Turn... - Phoronix</a></li>

</ul>
</details>

**标签**: `#security`, `#gnupg`, `#vulnerability`, `#open-source`, `#cryptography`

---

<a id="item-tech-news-3"></a>
### [浙江大学在超导芯片上首次真机实现 QRAM](https://finance.sina.com.cn/stock/2026-11-21/doc-iniznhsk3530826.shtml) ⭐️ 8.0/10

浙江大学团队报告在自主制备的超导量子芯片「天目 2 号」上首次于真机实现量子随机存储器（QRAM），成果发表于《自然·物理》。芯片上运行的原型可调取 4 位和 8 位数据，准确率分别为 80.9%和 60.4%，线路深度较未优化方案降低 30%以上，并首次验证该架构具备局部抗噪特性。团队表示下一步将推进 QRAM 的规模化研究。上述结果来自论文与团队报告，尚无法从所给材料独立复核。

telegram · zaihuapd · 11月21日 08:31

**「背景」** 量子随机存储器（QRAM）旨在让量子计算机以叠加态按地址并行读取数据，是许多量子算法的关键组件，但此前长期停留在理论或小规模方案阶段。据工具结果，浙江大学团队使用的「天目 2 号」是该校实验室研发的 125 比特超导量子处理器，此次 QRAM 原型即在该芯片上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://phys.org/news/2026-11-quantum-teleportation-method-weaker-entanglement.html">Quantum teleportation method uses weaker entanglement to transfer...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#QRAM`, `#superconducting qubits`, `#research`, `#hardware`

---

<a id="item-tech-news-4"></a>
### [显示器内置 USB 集线器如何拖慢以太网下载速度](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

一篇技术排查文章记录了作者发现显示器内置 USB 集线器会引入额外延迟，使连接其上的以太网适配器来不及确认数据包，导致适配器缓冲区填满并丢包，下载速度下降约 75%。作者通过更换一个确认频率更低的适配器解决了问题。这是单一用户的排查记录，而非受控测试或厂商结论。

hackernews · soheilpro · 11月21日 10:36 · [社区讨论](https://news.ycombinator.com/item?id=50587875)

**「背景」** USB 集线器在主机与下游设备之间转发数据，其引入的延迟通常不透明，用户很难从设备规格中看出影响。以太网适配器依赖及时收到数据包确认来维持吞吐，确认延迟升高会触发重传和丢包。

**「实际影响」** 使用显示器或扩展坞内置 USB 集线器连接以太网适配器的用户，若遇到无法解释的下载速度下降，可优先尝试将适配器直连主机或换用对确认频率要求较低的型号，而不是先怀疑网络线路。

**「社区讨论」** 有评论认为问题本质是“USB 网络交换机”而非显示器，显示器只是无关的载体；也有评论指出许多读者误解了文章，实际机制是额外延迟导致确认不及时、缓冲区溢出后丢包。另有用户表示自己在 MacBook 加雷雳扩展坞上遇到类似问题已一年多，最终通过启用流控缓解。

**标签**: `#networking`, `#usb`, `#hardware-debugging`, `#performance`, `#troubleshooting`

---

<a id="item-tech-news-5"></a>
### [mod\_wsgi 作者发布 AI 辅助 Rust 服务器 Muru](https://simonwillison.net/2026/Nov/21/muru/) ⭐️ 7.0/10

mod\_wsgi 的创建者 Graham Dumpleton 发布了 Muru，这是一个用 Rust 编写、在 AI 辅助下开发的服务器，目标是同时运行 ASGI 和 WSGI 两类 Python Web 应用，覆盖开发与生产环境。项目已在 GitHub 开源，作者从 2026 年 11 月 4 日起连续三周发布详细开发记录，内容涉及 worker 结构、import once/fork many、开发环境 HTTPS、WSGI 与 ASGI 共存、发布而非重启、无服务网格的灰度发布、Kubernetes 集成、按 worker 上报数据扩缩容、缩容到零以及页面工具栏与追踪等设计。目前这些属于作者公开的设计与开发进展，尚不能视为经过广泛生产验证的成熟能力。

rss · Simon Willison · 11月21日 23:56

**「背景」** Muru 的作者 Graham Dumpleton 是 mod\_wsgi 的创建者，该项目始于约 20 年前，长期用于在 Apache 下托管 Python Web 应用。WSGI 是较早期的 Python Web 服务器接口规范，ASGI 则是支持异步应用的后继规范；Muru 的目标是同时承载这两类应用。Simon Willison 此前曾报道过 Dumpleton 以公开开发日志方式推进的 wrapture 项目，本次 Muru 延续了同样的边开发边记录的做法。

**「对使用者的影响」** 对正在维护 WSGI 应用或迁移到 ASGI 的 Python 团队来说，Muru 提供了一个由 mod\_wsgi 原作者主导的新部署选项，其设计直接针对进程模型、发布方式和容器/Kubernetes 环境。但项目仍处于早期阶段，作者本人也表示会持续打磨直到自己愿意信任它，因此现阶段更适合评估和试验，而非直接替换现有生产服务器。

**标签**: `#python`, `#asgi`, `#wsgi`, `#rust`, `#web-servers`

---

<a id="item-tech-news-6"></a>
### [微软发布 RDMA over USB4 开发者预览，多台 PC 可合跑一个本地 AI 模型](https://videocardz.com/newz/microsoft-brings-rdma-over-usb4-to-windows-allowing-multiple-pcs-to-run-one-local-ai-model) ⭐️ 7.0/10

微软发布了 Windows 平台的 RDMA over USB4 开发者预览，允许多台 PC 通过普通 USB4 连接共享内存与 GPU 算力，共同运行同一个本地 AI 大模型，无需专用网卡或交换机。微软给出的示例是三台搭载 AMD Ryzen AI Max+ 395 的机器以 4-bit 量化运行 Qwen3-235B-A22B，速度约 18.5 token/s。该功能将通过 Windows Insider 推送，目前仍是开发者预览，而非面向普通用户的正式版本。

telegram · zaihuapd · 11月21日 06:13

**「背景」** RDMA（远程直接内存访问）允许一台系统直接读写另一台系统获准访问的内存，相比传统网络可减少操作系统与 CPU 的介入。微软此次是把 Windows 数据中心 RDMA 适配器所用的 NetworkDirect API 扩展到 USB4 链路上，让普通 PC 之间也能进行这种低开销的内存共享。

**「影响」** 对希望在本机运行超出单机显存容量的大模型的开发者而言，这一预览提供了一条不依赖专用网络硬件的扩展路径，但需要多台支持 USB4 的机器，且当前仅限 Windows Insider 预览渠道，稳定性和兼容性尚待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoftusbblog/introducing-rdma-over-usb4%C2%AE-on-windows-run-larger-local-ai-models-across-pcs/4574602">Introducing RDMA over USB 4 ® on Windows : run larger local AI ...</a></li>
<li><a href="https://www.guru3d.com/story/microsoft-previews-usb4-links-that-let-windows-pcs-pool-memory-and-gpu-resources/">Microsoft previews USB 4 links that let Windows PCs pool memory ...</a></li>

</ul>
</details>

**标签**: `#RDMA over USB4`, `#local AI inference`, `#Windows`, `#distributed computing`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [OpenRouter 警告 MiniMax 模型提示词疑遭第三方读取](https://news.ycombinator.com/item?id=50585962) ⭐️ 7.0/10

OpenRouter 通过邮件通知用户，发往 MiniMax 模型的请求内容可能已被第三方读取。安全研究者在 2026 年 7 月至 10 月间向 MiniMax 模型发送含测试 URL 的提示词，这些 URL 在 40 到 130 小时后被第三方访问。OpenRouter 将问题归因于 MiniMax 及其转发方 AtlasCloud、Novita、StreamLake，已下架相关端点的「零数据保留」标签，并建议涉及敏感凭证的用户更换 API Key 和密码。OpenRouter 官网尚未发布相关公告，上述信息来自邮件通知与研究者实验，尚无官方公开确认。

telegram · zaihuapd · 11月21日 06:53

**「背景」** “零数据保留”（Zero Data Retention）是模型路由平台向用户承诺不记录、不留存请求内容的一类标签，用户常据此决定是否把敏感数据交给第三方模型端点。此次事件中，安全研究者用植入提示词的测试 URL 作为“金丝雀”来检测请求是否被后续访问，从而判断提示词是否外泄。

**「影响与建议」** 通过 OpenRouter 调用 MiniMax 模型并传输敏感数据的用户应视为提示词可能已外泄，按 OpenRouter 建议轮换 API Key 和密码。依赖「零数据保留」标签判断合规性的用户需注意，该标签已从相关端点移除，不能再据此认定数据不会被留存或转发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://startupfortune.com/openrouter-warns-minimax-prompts-may-have-been-read-by-a-third-party/">OpenRouter warns MiniMax prompts may have been read by a ...</a></li>
<li><a href="https://www.gate.com/news/detail/minimaxs-zero-data-retention-fails-user-prompts-accessed-by-third-parties-25775454">MiniMax&#x27;s Zero Data Retention Fails: User Prompts Accessed by ...</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#LLM APIs`, `#OpenRouter`, `#MiniMax`

---

<a id="item-tech-news-8"></a>
### [daraxonrasib 一线联合化疗早期数据：确认缓解率 60.7%](https://event.eortc.org/ena2026/2026/11/20/metastatic-pancreatic-cancer-responds-well-to-initial-treatment/) ⭐️ 7.0/10

11 月 20 日，在西班牙巴塞罗那举行的 EORTC-NCI-AACR（ENA 2026）大会上，daraxonrasib 一线联合化疗的早期数据以 late-breaking 口头报告形式公布：61 例既往未治疗的转移性胰腺导管腺癌患者每日口服 200 mg，联合吉西他滨/白蛋白紫杉醇，确认客观缓解率为 60.7%，完全缓解率 8.2%（约十二分之一），疾病控制率 90.2%，中位无进展生存 12.8 个月，12 个月总生存率 76.6%，中位随访 18.3 个月。需要说明的是，这是单臂 I/II 期研究，没有化疗对照组，主要研究者明确表示疗效对比要靠正在进行的 III 期试验验证。

telegram · zaihuapd · 11月21日 11:24

**「背景」** daraxonrasib 是 Revolution Medicines 开发的口服 RAS\(ON\) 多选择性抑制剂，作用于活跃态 RAS，覆盖多种 KRAS/NRAS 突变，而非仅针对单一 G12C 突变。据 FDA 公告，该药已于 2026 年 8 月 26 日获批（商品名 RASONQUE），用于既往接受过治疗的转移性胰腺腺癌成人患者，批准依据是 III 期 RASolute 302 试验。此次 ENA 2026 报告的是将其前移至一线、与吉西他滨/白蛋白紫杉醇联用的单臂 I/II 期数据，与已获批的后线适应症属于不同治疗阶段。

**「解读注意」** 化疗的历史参照区间是 1 年生存率 22%–48%（MPACT 试验 35%，mFOLFIRINOX 48%），因此不宜简单称该结果“远高于化疗”。机制上，daraxonrasib 是口服 RAS\(ON\)多选择性抑制剂，作用于活跃态 RAS，覆盖多种 KRAS/NRAS 突变，并非单一 G12C 靶向药；该药已于 8 月 26 日获 FDA 批准（商品名 RASONQUE）用于既往治疗后的患者，依据是 III 期 RMC-302：中位总生存 13.2 个月对 6.7 个月。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fda.gov/drugs/resources-information-approved-drugs/fda-approves-daraxonrasib-metastatic-pancreatic-adenocarcinoma">FDA approves daraxonrasib for metastatic pancreatic ...</a></li>
<li><a href="https://www.cancernetwork.com/view/how-significant-is-the-approval-of-daraxonrasib-in-pancreatic-cancer-">How Significant Is the Approval of Daraxonrasib in Pancreatic ...</a></li>

</ul>
</details>

**标签**: `#biotech`, `#clinical-trials`, `#RAS-inhibitors`, `#pancreatic-cancer`, `#drug-development`

---

<a id="item-tech-news-9"></a>
### [特斯拉海外推送 FSD v15，新增 Reality View 可视化](https://x.com/Tesla/status/2124222447855743019) ⭐️ 7.0/10

特斯拉在海外开始推送 FSD v15。官方称本次更新将安全关键场景的处理能力提升至 25 倍，并新增“Tesla Reality View”可视化界面，可在车机屏幕上叠加摄像头画面与 FSD 行驶规划，支持全屏、地图或分屏视图及安静模式。导航可将转弯等信息叠加显示，转向灯提示音更轻柔并逐渐减弱；更新还优化了坑洼、碎片等路况的行驶体验，以及学校和恶劣天气下的速度控制。上述“25 倍”为特斯拉的官方说法，来源仅为一条社交媒体发布，尚无独立验证或技术细节。

telegram · zaihuapd · 11月22日 00:03

**「背景」** FSD 是特斯拉的高级驾驶辅助软件套件，此前版本以“FSD \(Supervised\)”名义推送，需驾驶员持续监督。据搜索结果，v15 的 Reality View 将原先分散的模型信号整合为单一端到端可视化，并声称占用更少算力；有报道提到该版本前一天还只是预告，随后才开始推送。

<details><summary>参考链接</summary>
<ul>
<li>FSD V15 LOOKS INSANE!!!! : r/TeslaFSD - Reddit</li>
<li>Tesla FSD V15 update rolling out with improved safety and autonomous ...</li>
<li>Tesla just started rolling out FSD v15. Yesterday it was only a teaser, two ...</li>

</ul>
</details>

**标签**: `#autonomous driving`, `#Tesla FSD`, `#AI systems`, `#software release`, `#computer vision`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [好代码的关键：少犯灾难性错误](https://seangoedecke.com/to-code-well-avoid-blunders/) ⭐️ 5.0/10

rss · Sean Goedecke · 11月22日 00:00

**「背景」** 许多工程师把编程想象成追求精妙洞察与漂亮抽象，但作者认为这种取向偏离了重点。在大型商业代码库、多人协作的“不纯工程”场景中，真正决定成败的往往不是灵光一现，而是能否避免那些会把优雅代码库变成别扭代码库的灾难性错误。

**「方案」** 作者用国际象棋和网球作类比：不送子、稳定回球就能赢过大多数对手，编程同样如此，因为软件中无法建立持久的领先优势，一次失误就可能抵消大量正确决策。他列举的典型失误包括引入并行系统做同一件事、为关键数据制造第二个真相来源、把安全的同步操作改成脆弱的异步操作、增加隐蔽的失败点以及复杂化关键接口，其核心可归结为不一致和引入不必要需求。不一致会破坏信任，让工程师不得不四处寻找意外；不必要需求则具有粘性，后来者难以判断能否删除，而且会与新功能产生组合式交互，这正是大代码库难维护的根源。因此作者建议把任务放到代码库中最自然的位置，并把需求裁剪到最小集合，甚至把“我可以用某个巧妙模式实现”视为分心警告。他还猜测，从不犯大错大约相当于国际象棋 1600 到 1700 分，并指出当前编码智能体在一致性上接近人类，但在避免不必要需求方面明显更差。

**「启示」** 做好编程不一定需要聪明，有时聪明反而是劣势；更关键的是保持一致性、砍掉不必要需求，把注意力集中在避免灾难性错误上。

**标签**: `#software engineering practice`, `#codebase maintainability`, `#technical debt`, `#engineering judgment`, `#opinion essay`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国借峰会扩大全球影响力：习近平今年已接待逾 40 位国家元首](https://www.cnbc.com/2026/11/21/china-xi-trump-putin-global-diplomacy-shenzhen.html) ⭐️ 7.0/10

据 CNBC 报道，在深圳举行的亚太经合组织（APEC）领导人会议期间，美国总统特朗普与中国国家主席习近平、俄罗斯总统普京于周四举行了三方会晤，这是三人首次面对面同场会面；习近平在会上宣布中国将向亚太地区提供 2000 万美元支持。

rss · CNBC Finance · 11月21日 06:00

**「背景」** 据 CNBC 基于中国官方通稿的分析，习近平今年以来已接待超过 40 位国家元首，其中至少 8 位是在本周深圳 APEC 会议期间；2025 年他还接待了 60 多次国事访问。

**「影响」** 清华大学的 Jodie Wen 和经济学人智库（EIU）的 Yue Su 表示，北京把这类多边平台视为扩大国际影响力、推动贸易与投资等实际经济合作的渠道，但各国地缘与经济优先事项分化，使多边机制达成共识更加困难。

**标签**: `#China`, `#geopolitics`, `#APEC`, `#diplomacy`, `#trade`

---

<a id="item-finance-news-2"></a>
### [特朗普称拟对海外建 AI 数据中心的美国公司征“巨额税款”](https://apnews.com/article/trump-artificial-intelligence-data-centers-f1ac03b73d13445400eeed8631d9d879) ⭐️ 7.0/10

特朗普 11 月 20 日在白宫记者会上表示，拟对在海外建设 AI 数据中心的美国科技公司征收“巨额税款”，称目的是把数据中心留在美国、保持对华 AI 竞争优势；该计划尚未向政府内部官员透露，也没有具体税率或立法细节。

telegram · zaihuapd · 11月21日 03:26

**「背景」** 特朗普在 11 月 20 日的白宫记者会上称，可能对在海外建设 AI 数据中心的美国科技公司征收“巨额税款”，并称尚未向政府内部官员透露该计划。他同时敦促美国各地接纳数据中心，建议社区与开发商谈判争取付款；目前全美多地社区因担忧用电需求和噪音而反对新建项目。

**「潜在影响」** 该表态目前只是尚未公布细节的提议，没有税率、立法程序或生效时间，因此对企业和市场的具体影响仍不确定。若最终落地，受影响的将是计划在海外建设 AI 数据中心的美国科技公司；而特朗普同时敦促各地接纳数据中心，意味着美国本地社区可能面临更多选址与用电、噪音方面的谈判压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ainewsglobal.online/data-center-anxiety-community-pushback-ai/">Data Center Anxiety: Why Communities Are Fighting Back</a></li>
<li><a href="https://successquarterly.com/data-center-boom-faces-community-opposition/">Data Center Boom Faces Community Opposition - SUCCESS...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#tax policy`, `#US-China tech competition`, `#data centers`, `#technology regulation`

---