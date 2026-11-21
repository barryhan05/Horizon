---
layout: default
title: "Horizon Summary: 2026-11-21 (ZH)"
date: 2026-11-21
lang: zh
---

> 从 39 条内容中筛选出 18 条重要资讯。

---

**科技新闻**
1. [Levent Alpöge 宣称证明广义黎曼猜想，附 1.3GB Lean 形式化](#item-tech-news-1) ⭐️ 9.0/10
2. [GitHub 仓库声称无外力 Navier–Stokes 方程有限时间爆破](#item-tech-news-2) ⭐️ 9.0/10
3. [陶哲轩博客讨论无外力纳维-斯托克斯奇点与广义黎曼猜想](#item-tech-news-3) ⭐️ 9.0/10
4. [数学家称与 Claude 合作证明黎曼猜想](#item-tech-news-4) ⭐️ 9.0/10
5. [Vakil 宣布 Masullo 提出广义黎曼猜想证明草案](#item-tech-news-5) ⭐️ 8.0/10
6. [KVM 漏洞 CVE-2026-99312 致 AMD 主机内存可被虚拟机读取](#item-tech-news-6) ⭐️ 8.0/10
7. [台积电暂停对中国企业 16nm 及以下芯片订单](#item-tech-news-7) ⭐️ 8.0/10
8. [Inkling 2 Mini：开放权重循环 Transformer 模型引发本地推理讨论](#item-tech-news-8) ⭐️ 7.0/10
9. [论文称语言模型可凭推理改写自身权重](#item-tech-news-9) ⭐️ 7.0/10
10. [Signal 限制移动端 AI 代理抓取用户数据](#item-tech-news-10) ⭐️ 7.0/10
11. [Aaronson 博客引发争论：LLM 能否产出有意义的数学成果](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI 推出后台模式：长任务异步执行，token 最高便宜 40%](#item-tech-news-12) ⭐️ 7.0/10
13. [Cursor 拟逐步停用中国开源权重模型](#item-tech-news-13) ⭐️ 7.0/10
14. [OpenAI 称反蒸馏防护将推理链提取成功率降至 0.2%](#item-tech-news-14) ⭐️ 7.0/10

**科技博客**
1. [输出缓存为何收效甚微：LLM 令牌预算分析](#item-tech-blog-1) ⭐️ 6.0/10

**财经新闻**
1. [沃什希望美联储官员少发声，官员们反而说得更多](#item-finance-news-1) ⭐️ 7.0/10
2. [美国收紧芯片出口，印度企业加码 AI 算力](#item-finance-news-2) ⭐️ 7.0/10
3. [特朗普称美企海外建 AI 数据中心将面临“巨额税款”](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Levent Alpöge 宣称证明广义黎曼猜想，附 1.3GB Lean 形式化](https://alpo.ge/remark.pdf) ⭐️ 9.0/10

Levent Alpöge 在个人网站发布 PDF，宣称证明了广义黎曼猜想（GRH），并附有一套据称规模达 1.3GB、约 1500 万行的 Lean 形式化代码，代码以 14 个分卷压缩包形式提供下载。该声明目前仅为作者本人的公告，尚未经过同行评审或独立验证，来源本身也只是 PDF 公告与社区讨论。社区评论还提到存在一份“完全由人类完成”的证明，链接指向 math216.wordpress.com 上同日发布的“Hurried Announcement”文章。

hackernews · iamronaldo · 11月20日 14:16 · [社区讨论](https://news.ycombinator.com/item?id=50574968)

**「背景」** 广义黎曼猜想（GRH）是黎曼猜想向一般狄利克雷 L 函数的推广，其证明若成立将影响数论中大量依赖该假设的结论。据外部报道，提出者 Levent Alpöge 是数论与算术统计方向的研究者，后加入 Anthropic；相关报道称他主张与 Claude 共同完成证明，且仅以 Lean 形式化代码发布、没有传统论文，形式化据称已完成，但结论尚未经专家核验。

**「影响与待验证点」** 若该证明成立，GRH 将从长期未解猜想变为可用于推理的前提，直接影响依赖该猜想的数论结果与相关算法分析；而 1.3GB 的 Lean 代码若可编译通过，也将成为形式化数学规模上的重要参照。但在独立复核 Lean 工程能否无错误构建、以及证明是否真正覆盖 GRH 陈述之前，这些都应视为待验证的声明而非既成结果。

**「社区讨论」** 有评论者实际下载并统计了分卷压缩包，称证明约 1.3GB、约 1500 万行代码，并感叹证明规模之大。另有评论者指出存在一份纯人类撰写的证明，也有人将此事与 AI 辅助数学的进展联系起来，表达了对节奏加快的复杂情绪；这些均为个人观点，不构成对证明正确性的验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Levent_Alp%C3%B6ge">Levent Alpöge - Wikipedia</a></li>
<li><a href="https://www.nacionale.com/en/articles/has-riemann-hypothesis-been-proved-levent-alpoge-claude-anthropic-claim-lean">Riemann hypothesis proof claimed with Claude, unverified</a></li>
<li><a href="https://clashreport.com/world/articles/anthropic-mathematician-claims-claude-helped-prove-riemann-hypothesis-opkw9bqkqhh">Riemann Hypothesis : Anthropic’s Alpöge Claims Proof Made With...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#Lean`, `#formal-verification`, `#theorem-proving`, `#research`

---

<a id="item-tech-news-2"></a>
### [GitHub 仓库声称无外力 Navier–Stokes 方程有限时间爆破](https://github.com/tristanbuckmaster/navier-stokes/) ⭐️ 9.0/10

一个 GitHub 仓库声称给出了无外力 Navier–Stokes 方程的有限时间爆破结果，并在 Hacker News 上被讨论为可能的重大数学突破。所提供的内容没有给出证明细节、版本或验证状态，因此该声明目前只是仓库作者的宣称，尚未得到独立确认。讨论中有人将其与据称由 OpenAI 给出的带外力反例区分开来，认为无外力版本更贴近“现实”情形。

hackernews · trotro · 11月20日 15:34 · [社区讨论](https://news.ycombinator.com/item?id=50576232)

**「背景」** 纳维–斯托克斯方程解的存在性与光滑性是克雷数学研究所悬赏的千禧年难题之一，其核心问题正是三维无外力情形下解是否会在有限时间内发生爆破。据社区评论所述，此前 OpenAI 曾给出一个借助精心设计的外力使方程失效的算例，而本次仓库声称的是无外力版本，两者条件并不相同。

**「影响」** 如果该结果成立，它将直接关系到流体动力学和科学计算中对 Navier–Stokes 方程解的正则性假设；但在证明经过同行评审或独立复现之前，开发者和研究者不应据此修改数值方法或理论前提。

**「社区讨论」** 评论者 tancop 指出这是无外力版本，并称 OpenAI 此前找到的是借助精心设计的外力破坏方程的例子，因此这一结果在某种意义上更“现实”。ninkendo 询问能否得到遵循 Navier–Stokes 方程、实时展示爆破的模拟，以帮助直观理解方程与现实不符之处；Ericson2314 则希望有人做出物理演示。另有评论提到 Buckmaster、Alpoge 以及关于 Anthropic 的传闻，但这些说法在所提供的材料中未获证实。

**标签**: `#navier-stokes`, `#mathematics`, `#fluid-dynamics`, `#research`, `#scientific-computing`

---

<a id="item-tech-news-3"></a>
### [陶哲轩博客讨论无外力纳维-斯托克斯奇点与广义黎曼猜想](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 9.0/10

陶哲轩（Terry Tao）博客发布一篇题为《Unforced Euler Singularity, Unforced Navier-Stokes Singularity, and the Generalized Riemann Hypothesis》的文章，据称涉及无外力欧拉方程与纳维-斯托克斯方程的奇点问题，以及广义黎曼猜想。目前可获得的证据仅有标题、链接和社区评论，无法独立核实文中具体结论、证明范围或是否已正式发表。评论者称，Lean 的 Zulip 讨论显示两个独立内核接受了相关结果，但这只是社区转述，尚不构成对数学结论本身的确认。

hackernews · archon1410 · 11月20日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=50578358)

**「背景」** Navier–Stokes 方程解的存在性与光滑性是克雷数学研究所悬赏的千禧年难题之一，其核心问题是三维空间中给定光滑初值是否可能产生有限时间奇点。维基百科条目提到，Terence Tao 曾在 2016 年就此发表结果，而 2026 年出现了一个爆破（blowup）结果，并伴随与 Alpöge、Buckmaster 的争议，以及该结果无法推广到无外力情形的问题。TechCrunch 同日报道称，Alpöge 与 Buckmaster 还发布了另一项与 Navier–Stokes 方程相关的重要证明。

**「社区讨论」** 有评论者引用 Lean Zulip 的讨论称，两个独立内核接受了该结果，因此认为证明中不太可能存在内核漏洞利用，但这属于社区对验证状态的转述。另有评论者提出更根本的疑问：现有方法擅长在已有抽象（如朗兰兹纲领）之上生成并验证证明，但新的数学抽象和概念本身如何产生；也有人表达了对 AI 在数学领域进展的兴奋与职业不安。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_existence_and_smoothness">Navier – Stokes existence and smoothness - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/11/20/ai-claimed-a-solution-to-the-167-year-old-riemann-hypothesis-and-a-human-did-too/">AI claimed a solution to the 167-year-old Riemann Hypothesis — and...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#Navier-Stokes`, `#Riemann Hypothesis`, `#formal verification`, `#AI for science`

---

<a id="item-tech-news-4"></a>
### [数学家称与 Claude 合作证明黎曼猜想](https://simonwillison.net/2026/Nov/20/levent-alpoge/) ⭐️ 9.0/10

数学家 Levent Alpöge 在一份 PDF 声明中表示，他相信自己与 Claude 合作发现了黎曼猜想的证明，并称该方法可推广至广义黎曼猜想，预计假以时日还能覆盖扩展黎曼猜想。他还声称双方已在无额外假设的情况下形式化了论证。该说法目前仅见于其个人声明，所提供内容中没有独立验证、同行评审或技术细节，因此其真实性高度不确定。

rss · Simon Willison · 11月20日 16:30

**「背景」** 黎曼猜想是数学界最著名的未解难题之一，其核心断言是黎曼ζ函数的所有非平凡零点都位于临界线上；广义黎曼猜想则把这一断言推广到更一般的狄利克雷 L 函数。据 Scientific American 报道，Levent Alpöge 是人工智能公司 Anthropic 的一名数学家，他于周五声称借助大语言模型证明了这一难题。

**「影响与待验证点」** 若该证明成立，将直接解决数学界最著名的未解问题之一，并成为 AI 辅助数学研究的标志性案例；但在独立复核和形式化证明被公开检查之前，研究者和开发者不应将其视为已确立的结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">Anthropic mathematician claims to prove Riemann hypothesis ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#Anthropic`, `#research`, `#formal-verification`

---

<a id="item-tech-news-5"></a>
### [Vakil 宣布 Masullo 提出广义黎曼猜想证明草案](https://simonwillison.net/2026/Nov/20/ravi-vakil/) ⭐️ 8.0/10

斯坦福数学家 Ravi Vakil 在博客中宣布，Alessandro Masullo 提出了一份广义黎曼猜想（GRH）的证明草案。Vakil 表示，Brian Conrad 已仔细审阅数月并给出大量反馈，这些反馈正在被纳入修改，目前“看起来不错”。原计划是邀请 Masullo 到斯坦福用一年时间打磨写作、并让足够多的人审阅后再公布，现在决定提前发布当前草案。Vakil 特别强调，这项工作完全由人类完成，没有使用 AI。该证明尚未经过正式验证，Vakil 的表述也只是初步判断。

rss · Simon Willison · 11月20日 19:21

**「背景」** 广义黎曼猜想是黎曼猜想的推广形式，而黎曼猜想本身是数学中最重要的未解猜想之一，其内容涉及黎曼ζ函数零点的分布。据《科学美国人》报道，Ravi Vakil 是美国数学会主席、斯坦福大学数学家，他于周五在博客中公布了这一由同样来自斯坦福的年轻数学家 Alessandro Masullo 提出的证明。

**「潜在影响」** 若该证明最终成立，广义黎曼猜想的推论将不再依赖条件性假设，例如确定性多项式时间的素性测试可变为无条件成立。但当前仅为早期草稿，Vakil 明确表示尚未经过充分审阅，因此在验证完成前不应据此调整任何依赖 GRH 条件性结论的研究或应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis">Generalized Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://www.scientificamerican.com/article/dueling-claims-of-riemann-hypothesis-proofs-emerge/">Dueling claims of Riemann hypothesis proofs ... | Scientific American</a></li>
<li><a href="https://www.linkedin.com/pulse/7-consequences-riemann-hypothesis-narrative-frank-pkbgc">The 7 Consequences of the Riemann Hypothesis - A Narrative...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#research`, `#proof-verification`, `#ai-and-mathematics`

---

<a id="item-tech-news-6"></a>
### [KVM 漏洞 CVE-2026-99312 致 AMD 主机内存可被虚拟机读取](https://thehackernews.com/2026/11/new-linux-kvm-flaw-cve-2026-99312-lets.html) ⭐️ 8.0/10

Linux 内核 KVM 被披露存在 CVE-2026-99312 漏洞，仅影响启用了嵌套虚拟化的 AMD 主机。研究人员在 DigitalOcean 上从虚拟机内部读取到约 127 GB 宿主内存。上游修复已于 11 月 18 日随稳定内核 7.3.5 等版本发布，但 Debian、Ubuntu 等发行版内核尚未修复；在补丁到位前，可通过关闭嵌套虚拟化来规避。

telegram · zaihuapd · 11月20日 14:23

**「背景」** 该漏洞位于 Linux 内核内置的 KVM 虚拟机监控器中，仅影响启用嵌套虚拟化的 AMD 主机。据 Terra Security 研究，这一缺陷在约四年前由一次安全修复引入内核，属于陈旧指针问题，使虚拟机得以访问本不属于它的宿主内存。上游修复已随 11 月 18 日发布的稳定内核 7.3.5 等版本提供，但 Debian、Ubuntu 等发行版内核尚未跟进。

**「影响与应对」** 在 AMD 平台上启用嵌套虚拟化的运维方，其宿主内存可能被租户虚拟机读取，构成跨租户数据泄露风险。由于发行版内核尚未跟进上游修复，受影响环境需先关闭嵌套虚拟化，或等待发行版发布包含该修复的内核更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.terra.security/blog/kvm-guest-to-host-escape">KVM Guest-to- Host Escape | Terra Security Research</a></li>
<li><a href="https://www.digitalocean.com/blog/cve-2026-99312-kvm-patch">Virtualization , Responsible Disclosure, and CVE - 2026 - 99312</a></li>

</ul>
</details>

**标签**: `#linux-kvm`, `#vulnerability`, `#virtualization`, `#amd`, `#kernel-security`

---

<a id="item-tech-news-7"></a>
### [台积电暂停对中国企业 16nm 及以下芯片订单](https://appleinsider.com/articles/26/11/20/apple-supplier-tsmc-cuts-off-china-chip-orders-amid-tighter-export-controls) ⭐️ 8.0/10

台积电已通知客户，暂停承接中国公司 16nm 及以下先进制程订单。按收紧后的美国半导体出口新规，除非事先取得美国出口许可或豁免，否则不得供货；此前台积电可自行评估客户设计是否符合豁免条件，现在则须由客户提前申请。报道称，美国获批名单中有苹果、AMD、英伟达，尚无中国公司，台积电表示将遵守新规。受限的中国企业因此只能使用 28nm、40nm 等旧制程，也无法获得 AI 数据中心所需的高带宽内存。

telegram · zaihuapd · 11月21日 02:01

**「背景」** 此前，台积电可自行评估中国客户的设计是否符合美国出口豁免条件；据路透社报道，2026 年 11 月生效的新规堵住了这一“制造漏洞”，把豁免判断改为由客户事先向美方申请许可。TrendForce 同期报道称，台积电与三星均据新规暂停了部分面向中国客户的消费级芯片出货，16nm 订单受到影响。

**「影响」** 受影响的中国芯片设计企业需要把 16nm 及以下产品转向 28nm、40nm 等成熟制程，或等待美国出口许可与豁免审批，先进制程与 HBM 的获取渠道因此收窄。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.trendforce.com/news/2026/11/20/news-tsmc-samsung-reportedly-pause-china-consumer-chip-shipments-under-new-u-s-rules-16nm-orders-affected/">[News] TSMC, Samsung Reportedly Pause China Consumer Chip ...</a></li>
<li><a href="https://www.reuters.com/world/china/tsmc-tightens-china-ai-chip-curbs-new-us-rules-close-manufacturing-loophole-2026-11-19/">TSMC tightens China AI chip curbs as new US rules close ...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#export-controls`, `#TSMC`, `#AI-hardware`, `#supply-chain`

---

<a id="item-tech-news-8"></a>
### [Inkling 2 Mini：开放权重循环 Transformer 模型引发本地推理讨论](https://thinkingmachines.ai/news/inkling-2-mini/) ⭐️ 7.0/10

Thinking Machines 发布了开放权重的 Inkling 2 Mini 模型，其采用循环 Transformer 架构。Hacker News 讨论中，有用户报告在 Ryzen 395 上通过 llama.cpp Vulkan 后端达到约 27 tokens/s 的解码速度，在 32GB 内存的 M1 Pro MacBook 上使用 q4 量化约 10 tokens/s；另有用户提到需要若干尚未合并的 llama.cpp PR，并给出一个据称可提升约 30% 速度的小补丁。评论者称该模型在部分基准上接近 Qwen3.8-27B，但这些基准结果尚未得到独立验证。

hackernews · jasondavies · 11月20日 20:12 · [社区讨论](https://news.ycombinator.com/item?id=50581260)

**「背景」** Inkling 2 Mini 是 Thinking Machines Lab 发布的开放权重模型，官方称其体积小到可在笔记本电脑上运行，并通过循环中间层让每个 token 进行更多推理、以更少 token 得出答案。Hugging Face 页面显示其为 26B 参数的图文转文本模型。

**「对本地用户的影响」** 希望本地运行该模型的用户需要关注 llama.cpp 的兼容性：评论提到相关 PR 尚未合并，且可能需要额外补丁才能获得较好速度，因此直接使用现有发行版可能无法达到报告中的性能。

**「社区讨论」** 有评论者认为，若基准在真实场景中成立，开放权重的循环架构模型达到这一水平“非常惊人”，并推测多数开放模型可能跟进采用循环架构；也有用户报告快速编码测试表现不错，但在识别硬币类型与年份的测试中失败，在约 12000 tokens 后仍在反复猜测。上述均为个人测试与观点，不构成独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://huggingface.co/thinkingmachines/Inkling-2-Mini">thinkingmachines/Inkling-2-Mini - Hugging Face</a></li>

</ul>
</details>

**标签**: `#open-weights models`, `#looped transformers`, `#local inference`, `#llama.cpp`, `#model architecture`

---

<a id="item-tech-news-9"></a>
### [论文称语言模型可凭推理改写自身权重](https://arxiv.org/abs/2611.21885) ⭐️ 7.0/10

一篇 arXiv 论文（编号 2611.21885）声称，语言模型首次能通过自身推理改写权重并变得更好，且不使用梯度、不进行训练；论文称模型在练习题上测试每次编辑、只提交有效的改动，连续八次会话中准确率持续上升。但现有材料只有标题、链接和社区评论，缺少论文细节，因此这些说法仍属作者主张而非独立验证的结果。评论者指出，实际观察到的自我改进范围很窄：模型只是缩短推理轨迹以避免触及 token 上限。

hackernews · lwhsiao · 11月20日 16:29 · [社区讨论](https://news.ycombinator.com/item?id=50577265)

**「背景」** 此前已有研究探索让模型在部署后自行更新权重。Google 的 SLEEP 框架在离线“睡眠”阶段解锁预分配的 MoE 记忆块，用自生成练习题更新数值权重，以吸收新知识并保持原有能力（tool-1-1）。另一条相关路线是“权重空间编程”：有研究称 GPT-6 Astra 能直接读取原始权重并判断网络训练目标，进而检查、调试和改进权重（tool-2-2、tool-2-1）。本次论文声称模型仅靠推理、无需梯度和训练即可改写自身权重，与上述依赖离线更新或直接读写权重的工作形成对照。

**「影响与疑点」** 若该机制成立，模型可在不重新训练的情况下自行修改权重，但评论者提醒，这种能力也可能被用来抑制与安全对齐相关的激活，构成新的安全风险。对开发者而言，在论文方法与评测细节公开前，不宜把“无训练自我改进”当作已验证的工程手段。

**「社区讨论」** 评论者质疑其新颖性：gavinray 认为 Google 的 SLEEP 框架已展示模型在离线阶段用自生成样本更新 MoE 权重；aesthesia 称这与近期“权重空间编程”文章结论类似，即模型只能靠修复明显缺陷来提升。Toutouxc 则指出“只提交有效编辑”听起来仍像训练，要求作者澄清与梯度下降的区别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/the-sleep-framework-a-new-way-for-llms-to-retain-knowledge-in-continual-learning/">The sleep framework: A new way for LLMs to retain knowledge ...</a></li>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight - Space Programming : LLMs can natively read...</a></li>
<li><a href="https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/">Qwen 3.8 27B on my laptop can interpret model weights , too</a></li>

</ul>
</details>

**标签**: `#language-models`, `#self-modification`, `#ai-safety`, `#research`, `#machine-learning`

---

<a id="item-tech-news-10"></a>
### [Signal 限制移动端 AI 代理抓取用户数据](https://signal.org/blog/protecting-your-privacy/) ⭐️ 7.0/10

Signal 在其博客中说明，正在设法阻止移动操作系统平台上的 AI 代理抓取用户数据，并称对部分进展持“谨慎乐观”态度。由于提供的原文内容缺失，具体技术措施、覆盖平台和生效时间均无法确认，目前只能视为厂商披露的防护方向，而非已独立验证的能力。

hackernews · dotcoma · 11月20日 09:42 · [社区讨论](https://news.ycombinator.com/item?id=50572348)

**「背景」** Signal 此次表态针对的是操作系统层面集成的 AI 代理：这类代理可读取其他应用的数据，从而绕过应用自身的加密与隐私边界。据 Gizmodo 和 Inc.com 报道，Signal 在博文中警告 OS 级 AI 代理威胁隐私，并推出了阻止截图等措施。Signal 在博文中称，当前 AI 代理与操作系统的整合若缺乏常识性补救措施，将对应用层隐私构成“生存性威胁”，并削弱独立开发者保护用户敏感数据的能力。

**「社区讨论」** 有评论者援引 Meredith Whittaker 的访谈指出，问题不只在于用户自己安装了 AI 应用：即使本人没有安装，联系人设备上的 AI 应用仍可能读取聊天内容。另有开发者希望 Signal 公开其“取证调查”的发现，以便资源较少的团队复用；也有用户批评 Signal 的垃圾信息防护与 VPN 冲突，称在 VPN 下添加联系人会反复遭遇验证码，影响记者等高风险用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://signal.org/blog/protecting-your-privacy/">Signal &gt;&gt; Blog &gt;&gt; Signal is Serious About Protecting...</a></li>
<li><a href="https://www.inc.com/aaron-mok/signal-blocks-screenshots-ai-agents-privacy/91440348">Signal Blocks Screenshots Over AI Agent Risks - Inc.com</a></li>
<li><a href="https://gizmodo.com/signal-is-fighting-to-keep-ai-agents-out-of-your-private-messages-2000843160">Signal Is Fighting to Keep AI Agents Out of Your ... - Gizmodo</a></li>

</ul>
</details>

**标签**: `#privacy`, `#mobile-security`, `#ai-agents`, `#signal`, `#operating-systems`

---

<a id="item-tech-news-11"></a>
### [Aaronson 博客引发争论：LLM 能否产出有意义的数学成果](https://scottaaronson.blog/?p=10344) ⭐️ 7.0/10

Scott Aaronson 的博客文章《The stochastic parrots have apparently proved the Riemann Hypothesis》在 Hacker News 上引发讨论，帖子获得 233 分、210 条评论。讨论的核心是：LLM 这类被批评为“随机鹦鹉”的系统，能否产出真正有意义的数学结果，以及这对人类理解和可解释性意味着什么。现有材料只有标题和部分评论，没有提供任何具体模型、证明过程或验证结果，因此无法确认是否真的存在可核验的数学突破。

hackernews · stratos123 · 11月20日 20:03 · [社区讨论](https://news.ycombinator.com/item?id=50581084)

**「背景」** “随机鹦鹉”（stochastic parrots）一词源自 2021 年一篇批评大语言模型的论文，此后常被用来质疑这类系统只是复述训练数据、并不真正理解内容。Scott Aaronson 此次在博客中回应了社交媒体上的一种说法：既然这些“随机鹦鹉”似乎证明了黎曼猜想，那么再用这个贬义标签称呼它们是否还合适。

**「社区讨论」** 有评论者用国际象棋引擎作类比：Stockfish 的评估看似给出了“解释”，但本质上是大量计算的汇总，底层还依赖 NNUE 这类神经网络评估器，因此仍无法回答人类真正想问的“为什么”。另有评论者担忧，人类可能越来越擅长“不理解”，在科学与工程中逐渐失去实质贡献能力；也有人反问，如果数学家拥有近乎无限算力，会有多少人能取得类似突破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scottaaronson.blog/?p=10344">Shtetl-Optimized » Blog Archive » The stochastic parrots have ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50581084">The stochastic parrots have apparently proved the Riemann ...</a></li>

</ul>
</details>

**标签**: `#AI reasoning`, `#interpretability`, `#mathematics`, `#LLMs`, `#epistemology`

---

<a id="item-tech-news-12"></a>
### [OpenAI 推出后台模式：长任务异步执行，token 最高便宜 40%](https://developers.openai.com/api/docs/guides/background) ⭐️ 7.0/10

OpenAI 上线 API 后台模式，将长耗时请求改为异步执行：请求中设置 background: true，并通过 background\_options.completion\_window 选择 2 小时或 8 小时完成时限，对应 token 费率分别比标准价低 30% 和 40%；不设置则使用默认的 soonest，不享受折扣。该折扣目前在 GPT-6.2 Astra、GPT-6.2 Sol、GPT-6.1 Terra 和 GPT-6 Luna 上公测。另需注意，后台模式会临时存储响应数据，即使 store 设为 false 或启用零数据保留也不例外。上述信息来自二手来源摘要，尚未获得独立验证。

telegram · zaihuapd · 11月20日 11:15

**「背景」** OpenAI 的 Responses API 常规调用是同步的：应用发出输入后，模型在同一连接上完成推理并返回最终结果，长耗时任务容易受超时限制。后台模式则把这类请求改为异步执行，开发者设置 background: true 后可通过轮询 response 对象查看状态，而不必保持连接等待。

**「对开发者的影响」** 使用后台模式的开发者需要留意数据留存边界：OpenAI 文档明确，即使将 store 设为 false 或启用零数据保留（ZDR），后台模式仍会临时存储响应数据以执行请求并供结果检索，所有完成时限下的临时存储内容均静态加密。这意味着依赖 ZDR 承诺“请求处理后不保留提示与响应”的合规场景，需重新评估该功能是否适用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/background">Background mode | OpenAI API</a></li>
<li><a href="https://kissapi.ai/blog/openai-background-mode-api-guide-2026.html">OpenAI Background Mode API : Run Long Tasks Without Timeouts...</a></li>
<li><a href="https://aiengineerguide.com/til/openai-background-mode/">Handling Async Inference with OpenAI &#x27;s API Background mode</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/background">Background mode | OpenAI API</a></li>
<li><a href="https://openai.com/index/offering-zero-data-retention-for-frontier-models/">Offering Zero Data Retention for frontier models - OpenAI</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/your-data">Data controls in the OpenAI platform</a></li>

</ul>
</details>

**标签**: `#openai`, `#api`, `#asynchronous-processing`, `#pricing`, `#data-retention`

---

<a id="item-tech-news-13"></a>
### [Cursor 拟逐步停用中国开源权重模型](https://www.cnbc.com/2026/11/20/cursor-chinese-ai-models-geopolitical-risk.html) ⭐️ 7.0/10

据 CNBC 报道，AI 编程平台 Cursor 表示正考虑以“地缘政治风险”为由逐步停用中国开发的开源权重模型，其 Composer 2 编程模型基于月之暗面的 Kimi K2.5 构建。这一表态出现在美国众议院国土安全委员会与美中特别委员会的一份报告之后，该报告建议推出“美国国家开源权重计划”，并在现有禁止 DeepSeek 进入联邦系统的行政令基础上，进一步禁止联邦系统使用中国开发的 AI 模型。目前这仍是考虑中的计划，而非已完成的停用。

telegram · zaihuapd · 11月20日 16:13

**「背景」** Cursor 的 Composer 2 编程模型此前被曝基于月之暗面（Moonshot AI）的 Kimi K2.5 开源权重模型构建，Cursor 随后承认了这一基础关系。2026 年 10 月，美国国土安全部发布命令，将 DeepSeek 产品从联邦文职机构 IT 系统中排除；众议院中国问题特别委员会与国土安全委员会随后联合发布调查报告，聚焦中国企业开发的开源权重模型被整合进美国公司消费级平台的问题，并建议进一步限制联邦系统使用中国开发的 AI 模型。

**「影响」** 若 Cursor 落实停用，依赖其 Composer 2 的开发者可能面临模型底层更换带来的行为与输出差异，需要重新评估代码生成质量与兼容性；同时，以中国开源权重模型为基础构建产品的美国平台，将面临把联邦政策建议转化为产品决策的压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.idlen.io/news/cursor-composer-2-kimi-moonshot-ai-chinese-model-scandal/">Cursor and Kimi : Composer 2 Was Built on a Hidden Chinese Model</a></li>
<li><a href="https://www.linkedin.com/posts/dataconomy-media_cursor-admits-composer-2-based-on-moonshot-activity-7441789642393247744-x273">Cursor admits Composer 2 based on Moonshot AI’s Kimi ...</a></li>
<li><a href="https://chinaselectcommittee.house.gov/media/reports/joint-investigation-report-china-is-trying-to-get-us-companies-addicted-to-chinese-ai-models">Joint Investigation Report: China is Trying to Get U.S ...</a></li>
<li><a href="https://chinaselectcommittee.house.gov/media/press-releases/dhs-blocks-china-based-deepseek-from-federal-it-systems">DHS Blocks China-Based DeepSeek From Federal IT Systems</a></li>
<li><a href="https://www.congress.gov/crs_external_products/IF/PDF/IF13336/IF13336.1.pdf">Removing PRC Artificial Intelligence Models from Federal ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open-weight models`, `#geopolitics`, `#developer tools`, `#open source`

---

<a id="item-tech-news-14"></a>
### [OpenAI 称反蒸馏防护将推理链提取成功率降至 0.2%](https://openai.com/index/combatting-adversarial-distillation/) ⭐️ 7.0/10

OpenAI 于 11 月 20 日发文介绍针对「对抗性蒸馏」的防御措施，称 GPT-6.2 Astra 与 Sol 已加强对推理链的保护。OpenAI 表示，在其红队测试中，提取历史请求推理的成功率从 54.0% 降至 0.2%。OpenAI 还称今年每周对数千至数万个蒸馏账号采取执法，并曾就 DeepSeek 疑似蒸馏行为向国会汇报。上述数字均为 OpenAI 自述的红队测试结果，来源未提供独立验证。

telegram · zaihuapd · 11月21日 01:30

**「背景」** 所谓对抗性蒸馏，是指攻击者通过大量查询模型、诱导其输出推理过程，从而提取模型能力的行为。OpenAI 表示，其防护采用训练、安全措施、检测与执法相结合的分层方式；在 GPT‑6.2 Astra 与 GPT‑6.2 Sol 上，模型会把受保护的推理与其产生时的对话历史绑定，使脱离原始上下文的推理提取更难奏效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/combatting-adversarial-distillation/">Combatting adversarial distillation | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI security`, `#model distillation`, `#OpenAI`, `#red teaming`, `#LLM`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [输出缓存为何收效甚微：LLM 令牌预算分析](https://seangoedecke.com/why-output-caching-doesnt-work/) ⭐️ 6.0/10

rss · Sean Goedecke · 11月21日 00:00

**「背景」** LLM 推理成本优化的常规做法是缓存输入（KV cache），避免每轮对话重算全部历史。作者由此提出一个自然延伸的问题：既然智能体在输出中大量重复引用代码片段、证据文档和模型样例，是否也应缓存或压缩输出？

**「方案」** 作者设想的输出缓存机制是让模型输出“src/script.py:12-15”这类引用而非整段复述，再由运行框架透明展开，从而省下昂贵的输出令牌。但他认为这条路走不通，因为可优化的只是用户可见的输出。根据他自己智能体历史的非正式统计，可见输出仅占输出令牌约 6%，推理令牌占 50%，工具调用占 44%。按 Amdahl 定律，即便乐观地省掉可见输出三分之二的令牌，总输出也只减少约 4%。真正的节省空间在不可见的 94%：模型越聪明，达到正确答案所需的推理与工具调用令牌越少，因此单价贵 5 倍的模型若少用 6 倍令牌，总成本反而更低。作者对“前沿模型链式思考很少自我重复”只有中等信心，并指出更好的运行框架也有帮助，但认为框架优势容易被复制。

**「启示」** 作者的核心结论是：输出缓存的收益被 Amdahl 定律锁死，降低 LLM 成本应聚焦于减少不可见的推理与工具调用令牌，而这主要取决于模型智能而非输出压缩技巧。

**标签**: `#LLM inference economics`, `#output caching`, `#token cost`, `#Amdahl&\#x27;s law`, `#AI agents`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [沃什希望美联储官员少发声，官员们反而说得更多](https://www.cnbc.com/2026/11/20/warsh-fed-forward-guidance-rate-hikes.html) ⭐️ 7.0/10

美联储主席凯文·沃什上任六个月来一直避免就利率走向给出前瞻指引，但据美国银行分析，过去两周美联储官员的公开表态次数为 2025 年初以来同期最多，部分官员主张更快加息，其中理事克里斯托弗·沃勒提出 12 月可能加息半个百分点。

rss · CNBC Finance · 11月20日 21:10

**「背景」** 新任主席沃什自 2026 年 6 月上任以来推动美联储放弃“前瞻指引”（即提前向市场预告未来利率路径），他在 6 月 17 日记者会上称该做法不适合当前政策环境。

**「影响」** 据 CME Group 的 FedWatch 数据，交易员目前认为 12 月至少加息 25 个基点的概率为 100%，这意味着家庭和企业的短期借贷成本可能上升。美国银行经济学家 Aditya Bhave 警告，美联储官员公开表态相互矛盾，会在本已动荡的时期造成利率过度波动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/mediacenter/files/FOMCpresconf20260617.pdf">Transcript of Chairman Warsh&#x27;s Press Conference -- June 17, 2026</a></li>
<li><a href="https://thehill.com/business/5929155-warsh-ends-fed-forecasts/">Federal Reserve shifts away from forward guidance under new ...</a></li>
<li><a href="https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool">FedWatch</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#forward guidance`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [美国收紧芯片出口，印度企业加码 AI 算力](https://www.bloomberg.com/news/articles/2026-11-20/nvidia-scandal-fallout-india-ai-yotta-ambani-adani-am-intelligence-e2e-networks) ⭐️ 7.0/10

美国收紧对马来西亚、泰国和新加坡的先进芯片出口，印度 AI 业界认为可承接外溢需求；Yotta 称未来一年新增约 10 万块 GPU，相当于印度现有算力再增约 10%。

telegram · zaihuapd · 11月20日 07:31

**「背景」** 美国新规要求向马来西亚、新加坡、泰国、印度尼西亚等国出口或转移先进 AI 芯片须获许可，东南亚数据中心因此需美国批准才能采购此类芯片（tool-1-1、tool-1-2、tool-1-3）。印度方面，信实承诺投入至多 1100 亿美元、阿达尼 1000 亿美元建设 AI 基础设施（tool-2-1）。

**「影响」** 若这些承诺落地，印度数据中心和 AI 算力供给将明显扩张，但信实至多 1100 亿美元、阿达尼 1000 亿美元的投入目前只是公布的计划，并非已确认支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techwireasia.com/2026/11/us-ai-chip-restrictions-malaysia-singapore/">US AI chip restrictions put Malaysia and Singapore data ...</a></li>
<li><a href="https://www.channelnewsasia.com/singapore/us-export-controls-ai-chips-6556831">Singapore assessing impact of new US chip export controls ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/18/nvidia-us-ai-chip-export-controls-data-centers-.html">New U.S. chip curbs put Southeast Asia&#x27;s data center ... - CNBC</a></li>
<li><a href="https://www.hindustantimes.com/opinion/todays-ai-infrastructure-could-be-toast-tomorrow-101793905721069.html">Today’s AI infrastructure could be toast tomorrow | Hindustan Times</a></li>

</ul>
</details>

**标签**: `#semiconductor export controls`, `#India AI infrastructure`, `#data centers`, `#Nvidia`, `#US trade policy`

---

<a id="item-finance-news-3"></a>
### [特朗普称美企海外建 AI 数据中心将面临“巨额税款”](https://apnews.com/article/trump-artificial-intelligence-data-centers-f1ac03b73d13445400eeed8631d9d879) ⭐️ 7.0/10

特朗普 11 月 20 日在白宫记者会上表示，拟对在海外建设 AI 数据中心的美国科技公司征收“巨额税款”，称此举旨在把数据中心留在美国、维持对中国的 AI 竞争优势；他同时承认尚未向政府内部官员透露该计划，也未公布税率或立法时间表。

telegram · zaihuapd · 11月21日 03:26

**「背景」** 特朗普长期公开支持美国人工智能发展，此次表态是在他结束访华行程后于白宫记者会上作出的。与此同时，全美多地社区因担忧数据中心的用电、用水需求和噪音而反对新建项目，一项民调显示约 71%的美国人反对在自家附近建设 AI 数据中心。

**「影响」** 若该设想落地，在海外布局 AI 算力的美国科技公司将直接受影响，其数据中心选址和投资成本可能上升；但目前这只是总统表态，尚无具体税率或立法安排，实际影响取决于后续政策是否成文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.usatoday.com/story/tech/nation-now/2026/11/20/trump-tax-ai-data-centers/92881622007/">Trump wants to tax US companies that build AI data centers abroad</a></li>
<li><a href="https://www.linkedin.com/posts/adriaanrainsobotha_a-new-gallup-poll-found-that-71-of-americans-activity-7484964265003634689-2eK0">71% of Americans Oppose Building AI Data Centers in Local ...</a></li>
<li><a href="https://time.com/article/2026/07/22/community-backlash-ai-data-centers/">Community Backlash to AI Data Centers Is Growing Across the U . S .</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#tax policy`, `#US tech companies`, `#data centers`, `#US-China competition`

---