---
layout: default
title: "Horizon Summary: 2026-11-26 (ZH)"
date: 2026-11-26
lang: zh
---

> 从 35 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [1Password 披露 2026 年 11 月安全事件](#item-tech-news-1) ⭐️ 8.0/10
2. [GRH 的 Lean 验证出现大幅精简版本](#item-tech-news-2) ⭐️ 8.0/10
3. [Minecraft Java 版曝高危 RCE 漏洞，暂无官方补丁](#item-tech-news-3) ⭐️ 8.0/10
4. [Aaronson 博客引发矩阵乘法指数 9/4 的热议](#item-tech-news-4) ⭐️ 7.0/10
5. [SemiAnalysis 推出 GDPx 基准，评估前沿模型新发布](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI 押注网络安全，称其规模或超编程业务](#item-tech-news-6) ⭐️ 7.0/10
7. [腾讯开源 Hy4 flash 量化权重，64GB Mac mini 可运行](#item-tech-news-7) ⭐️ 7.0/10
8. [三星与 SK 海力士据报交叉许可采用长江存储 Xtacking 技术](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [美商务部被曝施压英特尔交出 10%股权](#item-finance-news-1) ⭐️ 8.0/10
2. [美国拟对 14 个贸易伙伴加征新关税，中国面临额外 20%](#item-finance-news-2) ⭐️ 8.0/10
3. [市场剧烈波动考验沃什“读市场”的货币政策思路](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [1Password 披露 2026 年 11 月安全事件](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password 发布博客，披露了一起发生在 2026 年 11 月的安全事件。根据社区讨论中引述的公告内容，攻击者曾向 1Password 的后端服务推送恶意代码，但公司称最坏情况因客户数据加密而得到缓解。公告未说明是否缺少分支保护规则、推送权限是否被绕过，也未明确声明用户的加密保险库未被下载。

hackernews · lxhrstn · 11月25日 17:18 · [社区讨论](https://news.ycombinator.com/item?id=50644817)

**「背景」** 1Password 并非首次面对与第三方或供应链相关的安全风险：2023 年 Okta 泄露事件后，1Password 曾表示在 Okta 通知前就已自行检测到相关入侵尝试（tool-2-3）。此次 2026 年 11 月事件的不同之处在于，据社区讨论，攻击者据称能够向 1Password 的后端服务推送恶意代码，这使讨论焦点从凭证泄露转向代码部署与分支保护等工程控制。

**「影响与关注点」** 对 1Password 用户而言，直接风险集中在后续钓鱼：有评论者称收到一封非官方域名、但包含其个人细节的高质量钓鱼邮件，内容伪造了“保险库项目被分享给外部账号”的通知。维护本地保险库、停留在旧版应用的用户则需权衡：他们规避了云端代码推送风险，但也无法获得新版修复与功能。

**「社区讨论」** 安全从业者 tptacek 认为，员工笔记本电脑被攻陷后攻击者得以向 GitHub 推送代码，是 SaaS 公司的标准攻击路径，且随员工规模增长几乎必然发生。ctidd 批评公告未说明是否禁用向主分支推送、是否缺少分支保护规则；fn-mote 则希望官方明确声明“加密保险库未被下载”。ChrisHardie 作为长期用户表示，正因担心此类事件而坚持本地保险库，并质疑“恶意代码进入生产服务”正是中间人攻击的基础。

<details><summary>参考链接</summary>
<ul>
<li>Okta breach: Hackers attempt to compromise 1Password and Cloudflare using stolen data</li>

</ul>
</details>

**标签**: `#security`, `#password-managers`, `#supply-chain`, `#phishing`, `#saas`

---

<a id="item-tech-news-2"></a>
### [GRH 的 Lean 验证出现大幅精简版本](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

GitHub 仓库 lsernau/grh-lean 发布了一个大幅缩短的广义黎曼猜想（GRH）验证的 Lean 形式化版本。据社区评论，代码规模从约 1700 万行降至约 7.6 万行，缩减约 99.56%，并配有较清晰的人工可读文档，以及“已知数学”与“新数学”的分区。上述行数对比来自评论者而非仓库本身的独立说明，该版本是否在数学上等价于原验证、以及正确性如何，目前尚无独立确认。

hackernews · nb-t · 11月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=50648050)

**「背景」** 此前有报道称，Anthropic 数学家 Levent Alpöge 表示 Claude 协助找到了广义黎曼猜想的证明，但该证明以 Lean 代码形式给出，且尚未得到专家验证。据当时报道，这份 Lean 存档包含约 175,187 个源文件、239MB 数据。此次仓库展示的是同一验证工作的更短版本，社区评论称其从约 1700 万行缩减到约 7.6 万行。

**「影响」** 对形式化验证社区而言，这一缩减若属实，意味着审阅者需要通读的代码量从约 1700 万行降至约 7.6 万行，并可按“已知数学”与“新数学”分区阅读，从而降低独立核查该证明的成本。不过，目前规模数字与正确性均来自仓库和评论者说法，尚未见独立验证；在将其作为可信依据前，仍需以 Lean 编译器实际检查结果为准。

**「社区讨论」** 评论者普遍肯定其可读性和文档，认为这有助于理解原证明；但也有人（如 AIShill101）希望有数学家真正吃透核心论证，写成正式数学论文并在会议上讲解，而不只是 Lean 代码。gre 则提出，这是否回应了陶哲轩此前关于“巨大但缺乏洞见的证明是个问题”的观点，并追问更聪明的 LLM 是否已能通过精简和解释证明来跨过这一障碍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/anthropic-167-year-old-riemann-hypothesis-claude">Claude helped prove 167-year-old Riemann hypothesis , researcher...</a></li>
<li><a href="https://www.nacionale.com/en/articles/has-riemann-hypothesis-been-proved-levent-alpoge-claude-anthropic-claim-lean">Riemann hypothesis proof claimed with Claude, unverified</a></li>

</ul>
</details>

**标签**: `#formal-verification`, `#Lean`, `#mathematics`, `#AI-assisted-proofs`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Minecraft Java 版曝高危 RCE 漏洞，暂无官方补丁](https://github.com/bikini/minecraft2shell) ⭐️ 8.0/10

11 月 22 日公开的 minecraft2shell 漏洞显示，服务器资源包中的特制 TrueType 字体可触发 FreeType 2.14.3 及更早版本的原生越界写，从而在 Windows 客户端的 Java 版上执行任意代码。受影响版本为 1.20.5 至 1.21.10 以及 26.1 至 26.4 快照，1.20.4 及更早版本和基岩版不受影响。Mojang 目前仍使用 lwjgl-freetype 3.4.3，尚无官方补丁；社区于 11 月 24 日发布 m2sfix 1.0.0，通过 Java agent 或 mod 关闭 hinting 作为临时缓解。上述信息来自单一公开披露，尚无独立验证或官方安全公告。

telegram · zaihuapd · 11月25日 12:46

**「背景」** 该漏洞的根源在 Minecraft 使用的字体渲染库 FreeType：特制 TrueType 字体可触发其原生越界写，而 Java 版通过 lwjgl-freetype 3.4.3 调用该库。FreeType 此前已多次出现 TrueType 字体解析相关的安全问题，例如 2025 年 3 月的 CVE-2025-27363 补丁针对字体子字形结构解析，说明字体文件是这类原生库的常见攻击面。

**「影响与应对」** 在官方修复发布前，Java 版玩家应避免添加任何资源包，并将多人游戏服务器资源包权限设为“禁用”，或安装社区临时修复 mod。由于漏洞通过服务器资源包触发，加入不受信任的服务器时风险最高。

<details><summary>参考链接</summary>
<ul>
<li>[kirkstone][PATCH] freetype: patch CVE-2025-27363 - main@lists.openembedded.org | Home</li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#minecraft`, `#freetype`, `#remote-code-execution`

---

<a id="item-tech-news-4"></a>
### [Aaronson 博客引发矩阵乘法指数 9/4 的热议](https://scottaaronson.blog/?p=10379) ⭐️ 7.0/10

Hacker News 上出现一条指向 Scott Aaronson 博客文章的讨论帖，相关链接标题为《矩阵乘法指数是九分之四》（The matrix multiplication exponent is nine fourths）。该帖获得 953 条评论，讨论集中在数学突破对 AI 与科学进展的意义。但所给材料只有指向性链接和社区评论，没有论文原文、作者身份、证明是否经过同行评审或独立验证等技术细节，因此“指数为 9/4”目前只能视为被讨论的声称，而非已确认的结果。

hackernews · Kotlopou · 11月25日 19:11 · [社区讨论](https://news.ycombinator.com/item?id=50646108)

**「背景」** 矩阵乘法指数 ω 描述将两个 n×n 矩阵相乘所需的最小运算量级，长期是算法与复杂性理论的核心开放问题。据工具结果，OpenAI 于 2026 年 11 月 24 日发布论文，声称证明了 ω 恰为 9/4，并给出相匹配的上界与下界；其 Lean 形式化开发针对无除法电路、在任意域上计算形式多项式恒等式的情形。该结果目前属于论文与形式化证明中的声明，尚待独立验证。

**「社区讨论」** 有评论者认为，人类在生物上无法对如此量级的认知变化产生“相称的恐慌”，并称多数人会低估变化的规模；另一条评论则反驳说，AI 擅长公理化数学这类分析性先验领域，并不能由此推出它会在其他领域取得突破或带来生存风险。还有评论借 Bruno Latour 的“计算中心”概念，把当前进展类比为第谷·布拉赫整理天文数据之于开普勒定律的意义，并追问若只有 Lean、MathLib 和算力而没有大模型，类似进展是否早已发生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interestingengineering.com/culture/openai-exact-2-25-matrix-multiplication-exponent">OpenAI establishes exact 2.25 exponent for matrix multiplication</a></li>
<li><a href="https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/README.md">math/preprints/The- matrix - multiplication - exponent -is...</a></li>
<li><a href="https://www.alphaxiv.org/abs/2611.matrix-multiplication-exponent-lower-bound">The Matrix Multiplication Exponent Is Nine Fourths | alphaXiv</a></li>

</ul>
</details>

**标签**: `#algorithms`, `#matrix-multiplication`, `#complexity-theory`, `#AI`, `#research`

---

<a id="item-tech-news-5"></a>
### [SemiAnalysis 推出 GDPx 基准，评估前沿模型新发布](https://newsletter.semianalysis.com/p/evaluating-recent-model-releases) ⭐️ 7.0/10

SemiAnalysis 本月早些时候发布了 GDPx 基准，用于衡量前沿模型在“最有价值领域”的表现，并据此评估近期一批新模型。GDPx 刻意不按 GDP 占比或 O\*NET 职业分类选域，而是覆盖芯片设计、网络安全、生物学、金融、法律、量化交易、递归自我改进、硬件设计、材料科学、对齐和软件工程共 11 个领域，由 14 家专业数据合作方制作了 206 个任务。该基准以难度为卖点：发布日得分最高的 Opus 5.5 仅得 12%，远低于其他基准首日常超 50% 的水平。文章还指出，Fable 5.2 和 GPT-6.2 Astra 因安全分类器在网络安全、生物学和对齐三个领域触发，整体分数被压低；剔除这三域并改用部分评分后，排名会发生变化。

rss · Semianalysis · 11月26日 00:05

**「背景」** SemiAnalysis 于 2026 年 11 月 1 日发布 GDPx，定位为衡量前沿智能最具价值领域的通用智能体基准，覆盖 11 个经济价值较高的领域，并与领域专家合作构建任务。该基准的官方页面提供实时排行榜、分领域结果以及前沿模型的单任务成本数据。

**「对使用者的影响」** 对关注前沿模型能力的团队而言，GDPx 的低分区间意味着它短期内仍能区分模型进步，而不会像 Terminal Bench 4.0 那样趋于饱和；但解读榜单时需注意安全分类器导致的分数失真，以及法律和金融领域默认二元评分带来的信号损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gdpx.semianalysis.com/">gdpx.semianalysis.com - GDPx: The General Agentic Benchmark</a></li>
<li><a href="https://newsletter.semianalysis.com/p/gdpx-measuring-frontier-model-capabilities">GDPx: Measuring Frontier Model Capabilities Across the Most ...</a></li>

</ul>
</details>

**标签**: `#AI benchmarks`, `#model evaluation`, `#frontier models`, `#AI economics`

---

<a id="item-tech-news-6"></a>
### [OpenAI 押注网络安全，称其规模或超编程业务](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 7.0/10

OpenAI 将网络安全定位为下一个增长引擎，公司总裁格雷格·布罗克曼表示，网络安全将成为比编程更大的业务板块；CFO 则称外界对网络安全市场规模超过 3000 亿美元的估算仍被严重低估。公司已推出面向安全研究的 GPT-6 Cyber，并扩大名为 Daybreak 的“网络安全受信访问”计划，截至今年 9 月覆盖数千名经过验证的防御者、约 2000 个获批组织及工作空间，用于漏洞发现、代码库分析和二进制逆向。上述市场规模与业务排序均为公司高管的判断和预测，而非已实现的收入结果；报道同时指出，OpenAI 与 Anthropic、Google 的竞争格局以及规模化商业化前景仍不清晰。

telegram · zaihuapd · 11月25日 04:51

**「背景」** OpenAI 此前已通过 Daybreak 计划向经过验证的安全防御者提供专用模型：据搜索结果，2026 年 6 月公司发布 GPT-5.5-Cyber 及 Codex Security 更新，用于验证和修补漏洞；11 月初又推出 GPT-6 Cyber，最初仅向 Daybreak Red 客户限量开放，并声称发现 81 个新的 Firefox 漏洞及 948 个 Linux 内核漏洞的利用方式。此次报道中的说法，是把这一产品线从限量安全研究工具进一步定位为可能超过编程业务的商业板块。

**「对安全团队的影响」** 对安全研究团队而言，实际可用的入口是 Daybreak 的受信访问机制：需要以组织或工作空间为单位申请获批，而非直接开放使用，因此接入前需评估审批门槛与数据使用条件。由于该计划的具体准入标准和商业化定价尚未在报道中披露，企业不宜据此提前调整安全工具采购计划。

<details><summary>参考链接</summary>
<ul>
<li>OpenAI Expands Daybreak With GPT-5.5-Cyber to Help Defenders Patch Security Flaws</li>
<li>OpenAI launches GPT-6 Cyber for a limited set of Daybreak Red customers – claims 81 new Firefox vulns and exploits for 948 Linux kernel bugs : r/cybersecurity - Reddit</li>
<li>OpenAI introduces GPT-6 Cyber under Daybreak Red access limits | Paul Derrington</li>

</ul>
</details>

**标签**: `#OpenAI`, `#cybersecurity`, `#AI industry`, `#business strategy`, `#trusted access`

---

<a id="item-tech-news-7"></a>
### [腾讯开源 Hy4 flash 量化权重，64GB Mac mini 可运行](https://mp.weixin.qq.com/s/o0xxShVQX6g2UllrrEv1WQ) ⭐️ 7.0/10

腾讯混元通过大模型压缩加速工具箱 AngelSlim 开源了 224B 参数模型 Hy4 flash 的 GGUF 量化权重。原权重约 410.27GiB，最小的 IQ2-AH 版本为 125.73GiB，约为原版的 30%，借助 Strata offload 框架可在 64 GB Mac mini 上运行。来源给出的数据显示，48 GB 显存设备在 10K 上下文下每秒生成 89 个 token，M5 Max 128 GB 上 Q3\_K 版本在 32K 上下文下每秒生成 47 个 token；在 DeepSWE v1.1 等评测中，Q3\_K 与原模型得分差距不超过 0.4 分。上述性能与评测数字均来自单一来源，尚未经独立验证。

telegram · zaihuapd · 11月25日 09:29

**「背景」** Hy4 flash 是腾讯混元此前已开放权重的约 220B 参数模型（约 12B 激活参数），其 Hugging Face 模型卡已指向 AngelSlim 作为配套的大模型压缩工具包。AngelSlim 是腾讯开源的模型压缩工具箱，此前已支持 Hunyuan、Qwen2.5、Qwen3、DeepSeek-R1-Distill-Qwen 等模型的 INT8/FP8/INT4 量化。此次发布是在该模型原有权重基础上补充 GGUF 量化版本，并首次给出借助 Strata offload 在 64 GB Mac mini 上运行最小版本的具体条件。

**「影响」** 对希望在本地运行大模型的开发者而言，这次发布提供了从约 126GiB 的 IQ2-AH 到 Q3\_K 等多档 GGUF 权重，其中最小版本需配合 Strata offload 才能在 64 GB 内存的 Mac mini 上运行，实际可用性取决于该框架的 offload 支持与内存占用。若 Q3\_K 的精度损失确如来源所述不超过 0.4 分，则显存或统一内存有限的设备可在质量基本持平的前提下选择更低比特版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=85Gm68lK0sI">Tencent Hy 4 Flash Is Out. Time to Ditch Qwen 3.8 Flash ... - YouTube</a></li>
<li><a href="https://huggingface.co/tencent/Hy4-flash">tencent / Hy 4 - flash · Hugging Face</a></li>
<li><a href="https://github.com/Tencent/AngelSlim">GitHub - Tencent / AngelSlim : Model compression toolkit engineered...</a></li>

</ul>
</details>

**标签**: `#quantization`, `#open-source`, `#large-language-models`, `#local-inference`, `#model-compression`

---

<a id="item-tech-news-8"></a>
### [三星与 SK 海力士据报交叉许可采用长江存储 Xtacking 技术](https://tech.ifeng.com/c/8yLRPKxQy4L) ⭐️ 7.0/10

据凤凰网报道，三星电子和 SK 海力士已通过交叉许可协议，同意在 3D NAND 闪存中采用长江存储 Xtacking 堆叠技术的部分内容。Xtacking 将存储单元与控制电路（CMOS）分别制作在两片晶圆上，再通过键合工艺合二为一，使两部分可独立生产和优化。报道称三方均拒绝置评，因此该协议的存在与具体授权范围尚未得到任何当事方确认。Omdia 高级分析师指出，这种分工让厂商可自行生产存储阵列，把逻辑电路交给晶圆代工厂以使用更先进制程。

telegram · zaihuapd · 11月25日 14:33

**「背景」** Xtacking 是长江存储自研的 3D NAND 架构，其核心是把存储单元阵列与外围 CMOS 逻辑电路分别制造在两片晶圆上，再通过混合键合（hybrid bonding）面对面连接。第三方分析机构 TechInsights 的拆解显示，该技术已从 Xtacking 1.0（64 层 TLC）迭代至 Xtacking 4.0（160 层 TLC），混合键合工艺的成熟度是其实现高层数堆叠的关键。

**「潜在影响」** 若该交叉许可属实，三星和 SK 海力士可把存储阵列与 CMOS 逻辑电路分到两片晶圆上分别制造，并可将逻辑部分交由晶圆代工厂使用更先进制程，从而在数百层 3D NAND 的单晶圆工艺限制下获得更大工艺灵活性。不过三方均拒绝置评，相关报道尚未获官方确认，具体授权范围、生效时间和量产应用条件均不明确，现阶段不宜视为已落地的产能或产品变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techinsights.com/blog/ymtc-xtacking40-breaking-new-ground-3d-nand-technology">YMTC Xtacking4.0: Breaking New Ground in 3D NAND Technology</a></li>
<li><a href="https://www.techinsights.com/blog/ymtc-3d-nand-waveform-analysis-xtacking10-40">YMTC 3D NAND Waveform Analysis: From Xtacking1.0 to 4.0</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/25/news-sk-hynix-reportedly-joins-samsung-in-licensing-ymtcs-xtacking-technology-as-nand-race-heats-up/">[News] SK hynix Reportedly Joins Samsung in Licensing YMTC’s ...</a></li>
<li><a href="https://aiweekly.co/alerts/samsung-and-sk-hynix-tap-ymtcs-xtacking-tech-in-cross-license">Samsung and SK Hynix cross-license YMTC&#x27;s Xtacking 3D NAND</a></li>
<li><a href="https://www.techpowerup.com/355199/samsung-and-sk-hynix-to-license-ymtcs-xtacking-technology">Samsung and SK hynix to License YMTC&#x27;s Xtacking Technology</a></li>

</ul>
</details>

**标签**: `#3D NAND`, `#semiconductor manufacturing`, `#hybrid bonding`, `#memory industry`, `#YMTC`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美商务部被曝施压英特尔交出 10%股权](https://www.wired.com/story/inside-trumps-demands-to-another-chips-ceo/) ⭐️ 8.0/10

据 WIRED 报道，法庭文件显示，2025 年 8 月美国商务部律师在与英特尔首席财务官通话时警告，董事会可以拒绝交出 10%股权，但会面临“无法预测的后果”；几天后英特尔董事会照办，特朗普随后宣布美国政府“完全拥有并控制”这 10%股份且未支付对价，这批股份现值约 110 亿美元。

telegram · zaihuapd · 11月25日 13:25

**「背景」** 2025 年 8 月，英特尔宣布与美国政府达成协议，美方以 89 亿美元投资换取英特尔约 9.9%的普通股，这笔投资与英特尔此前获得的联邦补贴相关。据称，解封的股东诉讼法庭文件显示，商务部律师在协议达成前曾警告英特尔首席财务官，拒绝交出约 10%股权将面临无法预料的后果。

**「影响」** 若报道属实，这将是美国政府直接持有大型芯片企业股权的罕见案例，可能影响其他半导体公司对政府干预边界的预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/wired-commerce-lawyer-warned-intel-cfo-rejecting-us-10-stake-would-carry">Court records: Commerce threatened Intel CFO over 10% US stake</a></li>
<li><a href="https://finance.biggo.com/news/1eea079d-982e-483f-be72-28381b50b545">Unsealed Filings Allege White House Pressured Intel Board ...</a></li>
<li><a href="https://www.gate.com/news/detail/us-commerce-department-threatened-intel-over-10-equity-stake-for-89b-25860002">U.S. Commerce Department Threatened Intel Over 10% Equity ...</a></li>
<li><a href="https://www.intel.com/content/www/us/en/newsroom/news/corporate/intel-and-trump-administration-reach-historic-agreement.html">Intel and Trump Administration Reach Historic Agreement to ...</a></li>
<li><a href="https://enkiai.com/ai-infrastructure/intel-ai-trump-deal/">Intel AI Strategy 2025, $8.9B Trump Administration Deal - ENKI</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#US policy`, `#Intel`, `#government equity stake`, `#corporate governance`

---

<a id="item-finance-news-2"></a>
### [美国拟对 14 个贸易伙伴加征新关税，中国面临额外 20%](https://www.cnbc.com/2026/11/25/us-tariffs-trump-section-301.html) ⭐️ 8.0/10

美国政府拟依据 1974 年《贸易法》第 301 条，对中国、欧盟、日本、印度等 14 个贸易伙伴加征针对制造业产能过剩的新关税，税率按国别设定；其中中国将在 2018 年已加征的 25%基础上再加征 20%，若中国未遵守 2025 年 10 月釜山贸易休战协议，对华税率可能升至 40%。

telegram · zaihuapd · 11月25日 13:59

**「背景」** 此次拟议关税源于美国贸易代表办公室 2026 年 3 月中旬启动的第 301 条调查，该调查针对制造业“结构性产能过剩”，即美方所称的补贴生产压价冲击美国厂商。据福克斯商业频道报道，这些拟议关税还意在替代今年早些时候被最高法院裁定无效的关税。

**「影响」** 若落地，中国出口美国的相关制造企业将面临叠加关税成本，而其他 13 个伙伴的输美商品税率不会与现有关税叠加，受影响程度相对有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.foxbusiness.com/fox-news-global-economy/trump-admin-raise-tariffs-china-eu-other-trading-partners">Trump administration proposes sweeping Section 301 ... | Fox Business</a></li>
<li><a href="https://parisbusinesstimes.com/business/ustr-launches-wide-ranging-probes-into-global-manufacturing-overcapacity/">USTR Launches Wide-Ranging Probes into Global Manufacturing ...</a></li>

</ul>
</details>

**标签**: `#trade policy`, `#tariffs`, `#Section 301`, `#US-China trade`, `#manufacturing`

---

<a id="item-finance-news-3"></a>
### [市场剧烈波动考验沃什“读市场”的货币政策思路](https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html) ⭐️ 7.0/10

CNBC 的 Steve Liesman 分析称，英伟达引发的市场剧烈震荡，正在考验美联储主席凯文·沃什更依赖市场信号而非经济预测来制定政策的做法；上周市场下跌后，市场对加息的预期一度降温，而周一高盛金融状况指数回落 22 个基点，又让 12 月和 1 月加息的预期重新升温。

rss · CNBC Finance · 11月25日 12:26

**「背景」** 凯文·沃什于 2026 年 5 月 22 日就任美联储主席，任期四年，同时兼任联邦公开市场委员会主席（tool-1-2）。他主张更多依据市场指标而非经济模型预测来制定政策，而高盛金融状况指数正是由短期债券收益率、长期企业债收益率、汇率和股市等变量加权构成的综合指标（tool-2-3）。

**「影响」** 若美联储更多依据波动较大的市场指标决策，利率路径的不确定性可能上升，进而影响房贷、企业融资成本以及股票和债券投资者的预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/aboutthefed/bios/board/warsh.htm">Federal Reserve Board - Kevin Warsh, Chairman</a></li>
<li>[PDF] NBER WORKING PAPER SERIES FINANCIAL CONDITIONS INDEXES: A FRESH LOOK AFTER THE FINANCIAL CRISIS Jan Hatzius Peter Hooper Frederi</li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#Nvidia`, `#market volatility`, `#Kevin Warsh`

---