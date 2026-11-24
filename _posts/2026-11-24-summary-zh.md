---
layout: default
title: "Horizon Summary: 2026-11-24 (ZH)"
date: 2026-11-24
lang: zh
---

> 从 39 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Anthropic 称 Claude 发现 VP≠VNP 并公开 Lean 4 证明](#item-tech-news-1) ⭐️ 9.0/10
2. [Ladybird 浏览器发布首个 Alpha 版](#item-tech-news-2) ⭐️ 8.0/10
3. [智谱发布 GLM-5.4：首个循环 Transformer 编码模型](#item-tech-news-3) ⭐️ 8.0/10
4. [英伟达董事会恢复黄仁勋 CEO 职务](#item-tech-news-4) ⭐️ 8.0/10
5. [Codex2api 疑遭供应链投毒，3.1.10–3.1.12 版本被指含后门](#item-tech-news-5) ⭐️ 8.0/10
6. [ChatGPT 聊天页上线 GPT-6.2 Sol，向付费用户推送](#item-tech-news-6) ⭐️ 8.0/10
7. [NariQ 发布 10GB 内近 BF16 质量的 Qwen3.8-27B 量化](#item-tech-news-7) ⭐️ 7.0/10
8. [Stalwart 宣称可替代 Microsoft Exchange](#item-tech-news-8) ⭐️ 7.0/10
9. [黎曼猜想「AI 证明」被指空转，作者承认代码能编译但无实质内容](#item-tech-news-9) ⭐️ 7.0/10
10. [4.5 万家企业联名致信欧盟，要求调查苹果 iPhone 浏览器限制](#item-tech-news-10) ⭐️ 7.0/10
11. [黄循财：新加坡不会成为规避美国芯片管制的通道](#item-tech-news-11) ⭐️ 7.0/10

**科技博客**
1. [vLLM 首日支持 ERNIE 5.5 Flash 的插件与推理加速](#item-tech-blog-1) ⭐️ 6.0/10

**财经新闻**
1. [纽约联储主席威廉姆斯：通胀仍高，加息需“随时间推进”](#item-finance-news-1) ⭐️ 8.0/10
2. [AI 抛售波及中国科技股，DeepSeek 与月之暗面上市计划承压](#item-finance-news-2) ⭐️ 7.0/10
3. [上海地铁票价 21 年来首次调整](#item-finance-news-3) ⭐️ 7.0/10
4. [马斯克承认 SpaceX 在 AI 领域落后，转而向 Anthropic 和 Google 出租算力](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 称 Claude 发现 VP≠VNP 并公开 Lean 4 证明](https://github.com/anthropics/formal-math/blob/main/vp-vnp/README.md) ⭐️ 9.0/10

Anthropic 于 11 月 24 日公开论文《VP ≠ VNP over every field》及配套 Lean 4 形式化证明，仓库称结果由内部研究用 Claude 模型发现，论文与代码均由 AI 撰写。论文给出哈密顿圈多项式的超多项式算术电路下界，据此推出 VP 是 VNP 的真子类；若成立，即解决 Valiant 1979 年提出的代数复杂度猜想，但该结论仅针对算术电路，不涉及 P 与 NP。形式化部分经三条标准公理审计与独立内核 nanoda 复核，除预留文件外无 sorry。不过目前尚无人类数学家通读，Lean 无法确认形式化陈述与所声称命题一致，附录 Q 还列出了出入，结果仍待独立审阅。

telegram · zaihuapd · 11月24日 06:02

**「背景」** VP 与 VNP 是 Valiant 于 1979 年提出的代数复杂度类，被视为 P 与 NP 问题的代数类比；该猜想主张 VP 是 VNP 的真子类，而永久式（permanent）是典型的 VNP 完全问题。据外部报道，Anthropic 于 2026 年 11 月 23 日在 GitHub 的 formal-math 仓库新增 vp-vnp 项目，包含约 324 个 Lean 文件及一份署名 Claude 的预印本，README 明确说明尚无人类数学家核验该证明。

**「影响与待验证事项」** 在人类数学家独立审阅并确认 Lean 形式化陈述与论文命题一致之前，这一结果不应被视为已解决的复杂度定理；附录 Q 已列出形式化与声称命题之间的出入，说明当前证据只能证明代码通过了公理审计与 nanoda 内核复核，不能证明所证内容就是 VP≠VNP。即便最终成立，其结论也仅针对算术电路模型下 VP 是 VNP 的真子类，不涉及 P 与 NP 问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/anthropic-claude-vp-vnp-valiant-lean-proof-claimed-vs-verified-2026">VP ≠ VNP Lean Proof: Claimed vs Verified (2026) - explainx.ai</a></li>
<li><a href="https://www.besthub.dev/articles/claude-proves-vp-vnp-ai-cracks-47-year-algebraic-p-vs-np-conjecture-2454d374b036">Claude Proves VP ≠ VNP: AI Cracks 47-Year Algebraic P vs NP ...</a></li>
<li><a href="https://casrai.org/news/anthropic-claude-authored-vp-vnp-proof-unverified-lean-2026">Claude-Authored VP ≠ VNP Proof Posted, Unchecked — CASRAI</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-publishes-claude-authored-vp-vnp-proof-unverified">Anthropic Publishes Claude-Authored VP ≠ VNP Proof ...</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/claude-proves-vp-not-vnp-valiant-conjecture">Claude claims to prove VP ≠ VNP in Valiant&#x27;s 47-year-old ...</a></li>

</ul>
</details>

**标签**: `#complexity-theory`, `#formal-verification`, `#Lean 4`, `#AI-for-math`, `#Anthropic`

---

<a id="item-tech-news-2"></a>
### [Ladybird 浏览器发布首个 Alpha 版](https://ladybird.org/posts/alpha/) ⭐️ 8.0/10

独立浏览器项目 Ladybird 发布了首个 alpha 版本，macOS 和 Linux 用户现在可以直接下载安装，无需自行编译。该项目自行实现了 HTML 解析、CSS 引擎、布局、JavaScript 和 WebAssembly 等大部分核心组件，仅复用 HarfBuzz、Skia、ffmpeg 和 SQLite 等少数外部库。官方明确说明这是 alpha 版：部分网站无法使用，浏览器有时会崩溃，用户可从浏览器内报告问题站点，并在崩溃后自行决定是否发送崩溃报告。

hackernews · janvdberg · 11月23日 16:13 · [社区讨论](https://news.ycombinator.com/item?id=50614249)

**「背景」** Ladybird 是一个从零构建独立浏览器引擎的项目，其 HTML 解析、CSS 引擎、布局、JavaScript 和 WebAssembly 等核心组件大多为自行实现，仅复用 HarfBuzz、Skia、ffmpeg 和 SQLite 等少数外部库，部分代码继承自更早的 SerenityOS 项目。据外部报道，该项目经过约四年的独立开发才进入 alpha 阶段，此前一直没有面向公众的可用版本。

**「实际影响」** 早期试用显示，多数常规网站能正常渲染，WebAssembly 应用（如 ffmpeg 编译版、Pyodide REPL）可以运行，但依赖 service worker 与 web worker 组合的 Datasette Lite 会报错，源码中对应位置仍留有 FIXME 标注。Ladybird 采用每个标签页独立进程的隔离方式，试用中单个 WebContent 进程内存可达数百 MB，因此现阶段更适合作为测试和反馈用途，而非日常主力浏览器。

**「社区讨论」** 多位评论者报告了正面体验：freakynit 称测试的网站全部正确渲染，仅滚动略显卡顿；alentred 表示 ProxMox 等复杂站点正常，NoVNC 甚至比 Firefox 更流畅。kvuj 认为改用 SQLite、Skia 等成熟库大幅提升了质量，但也怀念 SerenityOS 时期自研一切的黑客精神；drnick1 则希望 Ladybird 未来认真处理指纹识别问题，提供随机化或伪造的 JS 值以及更细粒度的权限控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ladybird.org/posts/alpha/">Ladybird is now in alpha - Ladybird</a></li>
<li><a href="https://www.techpowerup.com/355140/independent-web-browser-engine-ladybird-goes-into-alpha-release">Independent Web Browser/Engine &quot;Ladybird&quot; Goes Into Alpha ...</a></li>
<li><a href="https://ladybird.org/">Ladybird Ladybird, the first new browser engine in years, is now ... Ladybird Browser is now officially available in alpha for ... Ladybird browser reaches alpha after four years of development Ladybird browser releases its first alpha for macOS and Linux</a></li>

</ul>
</details>

**标签**: `#browsers`, `#web-platform`, `#open-source`, `#systems-engineering`, `#privacy`

---

<a id="item-tech-news-3"></a>
### [智谱发布 GLM-5.4：首个循环 Transformer 编码模型](https://z.ai/blog/glm-5.4) ⭐️ 8.0/10

智谱（Z.ai）发布 GLM-5.4，这是其首个采用循环 Transformer（Loop Transformer）架构的模型，定位为通用编码。按官方描述，该架构让一组共享权重的层在一次前向传播中迭代运行多次，以细化隐藏状态，从而在不增加参数量的情况下加深网络。GLM-5.4 目前未开放权重，也无法通过常规 API 套餐访问，需订阅其 Coding Plan 才能调用；该套餐与常规 API 共用 OpenAI 兼容的 Responses API（https://api.z.ai/api/v1）。上述架构与能力描述均来自厂商，尚无独立验证。

hackernews · foohis · 11月23日 10:06 · [社区讨论](https://news.ycombinator.com/item?id=50609685)

**「背景」** 循环 Transformer 的核心思路是让一组共享权重的层在一次前向传播中重复运行多次，从而在不增加参数量的情况下加深网络。据 Thinking Machines Lab 于 11 月 20 日发布的 Inkling 2 Mini 介绍，该模型对每个 token 将中间层运行三次，以便用更少 token 完成推理，尤其面向依赖推理质量的智能体编程任务。GLM-5.4 是 Z.ai 首个采用该架构的模型，目前尚未提供开放权重。

**「对使用者的影响」** 开发者若想试用 GLM-5.4，需要改用 Coding Plan 订阅，其 API key 可在同一 OpenAI 兼容端点上使用；现有工具链需等待适配，例如 llm-zai 插件尚未支持该模型，Simon Willison 因此临时另写了 llm-glm 插件。评论者还提到，部分中国模型推理耗时明显偏长，在简单任务上也会反复自我检查，实际接入时需评估延迟成本。

**「社区讨论」** 有评论者赞赏智谱披露了较多技术细节，认为这与西方公司的封闭做法形成对比，并称循环 Transformer 是顺理成章的方向，只是仍有问题待解决。另一位评论者从推理瓶颈角度解释：逐层搬运权重受限于内存带宽，循环结构可减少这类搬运。也有用户抱怨中国模型“马拉松式思考”在简单任务上耗时过长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://openrouter.ai/thinkingmachines/inkling-2-mini">Inkling 2 Mini - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#LLM`, `#transformer-architecture`, `#coding-models`, `#open-source-AI`, `#model-releases`

---

<a id="item-tech-news-4"></a>
### [英伟达董事会恢复黄仁勋 CEO 职务](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 8.0/10

据 CNBC 报道，英伟达董事会在短暂解除黄仁勋 CEO 职务后，又将其恢复。公司声明称，董事会在决策过程中听取了美国联邦政府高层意见，并据此确信黄仁勋复职不构成国家安全风险。报道未说明解除职务的具体原因、持续时间或董事会投票细节，相关说法目前主要来自公司声明与媒体转述，尚缺乏独立核实。

hackernews · jaz · 11月23日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=50611576)

**「背景」** 据《卫报》报道，黄仁勋于 2026 年 11 月 13 日辞去英伟达 CEO 一职，此前有报道称其存在婚外情，其中涉及一名被指为中国间谍的女性。英伟达随后于 11 月 23 日发布公告，宣布黄仁勋即刻恢复总裁、CEO 及董事会成员职务。

**「影响」** 董事会声明称，其决定参考了美国政府高层意见，并据此认定黄仁勋复职不构成国家安全风险；CNBC 报道复职消息后英伟达股价上涨 31%。这一表述把公司治理决定与政府背书直接挂钩，可能使投资者和合规团队更关注英伟达在出口管制议题上的政策风险，而非仅评估管理层变动本身。

**「社区讨论」** 多位评论者认为，声明中“听取政府高层意见”一句才是关键，反映出公司治理受到外部政治力量影响。有评论者援引特拉华州 Caremark 判例指出，董事会在此类事务中被追责的门槛很高，若司法部表示不起诉，董事个人责任可能被排除；也有人对董事会在不到两周内从罢免转为一致同意复职感到意外。另有评论者质疑，美国要求 ASML 和日本芯片企业遵守对华制裁，却对英伟达给予特殊待遇，属于双重标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-board-reinstates-jensen-huang-as-president-ceo-and-board-director">NVIDIA Board Reinstates Jensen Huang as President, CEO and...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/23/jensen-huang-reinstated-as-nvidia-chief-executive">Jensen Huang reinstated as Nvidia CEO | Jensen ... | The Guardian</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-board-reinstates-jensen-huang-as-president-ceo-and-board-director">NVIDIA Board Reinstates Jensen Huang as President, CEO and ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html">Jensen Huang reinstated as Nvidia CEO. Stock skyrockets 31%</a></li>

</ul>
</details>

**标签**: `#nvidia`, `#corporate-governance`, `#semiconductors`, `#export-controls`, `#tech-industry`

---

<a id="item-tech-news-5"></a>
### [Codex2api 疑遭供应链投毒，3.1.10–3.1.12 版本被指含后门](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

一则 Telegram 报告称，Codex2api 项目作者账号被入侵，攻击者绕过 main 分支保护直接推送 tag，使 Release 构建出带后门的版本。据该报告，v3.1.11 移除了鉴权，等同于可无密码远程执行命令；另有 workflow 将仓库的 16 个 Actions secrets 外传，波及同一账号下至少 21 个仓库。报告建议安装或更新过 3.1.10–3.1.12 的用户立即停用并回退到 3.1.9，同时轮换 GitHub token、SSH key、数据库及 DeepSeek 等相关密钥。上述内容目前仅来自单一 Telegram 帖子和一份事件复盘，尚未获得独立验证。

telegram · zaihuapd · 11月23日 11:21

**「背景」** 该事件的核心机制是攻击者利用被入侵的账号直接推送 Git tag，从而绕过对 main 分支的保护，让 CI 在 tag 上构建并发布带后门的 Release。GitHub Actions 的 secrets 一旦被恶意 workflow 读取，就可能被外传，进而波及同一账号下的其他仓库。

**「影响与处置」** 若报告属实，使用 3.1.10–3.1.12 的部署可能暴露在无需鉴权的远程命令执行风险下，且相关仓库的 Actions secrets 可能已泄露。受影响用户应按报告建议回退到 3.1.9，并轮换所有可能暴露的凭据，包括 GitHub token、SSH key 和数据库、DeepSeek 等密钥。

**标签**: `#supply-chain-security`, `#open-source-security`, `#github-actions`, `#incident-report`, `#codex2api`

---

<a id="item-tech-news-6"></a>
### [ChatGPT 聊天页上线 GPT-6.2 Sol，向付费用户推送](https://x.com/ChatGPT/status/2124942186425069836) ⭐️ 8.0/10

ChatGPT 官方账号 11 月 23 日宣布，在 Chat 标签页上线 GPT-6.2 Sol 版本，主打日常对话场景，当天起向 Plus、Pro、Business 和 Enterprise 用户推送。官方称新版本更能处理复杂请求，尤其是用户给出详细指令或要求联网查找信息时，并在识别照片细节（如标签文字、路牌符号）、按价格或位置等关注点缩小在线选项范围、判断何时主动给出后续建议（例如询问是否要在降价时提醒）方面有所改进。上述能力描述均来自官方发布，未经独立验证，公告也未给出基准测试数据或具体技术细节。

telegram · zaihuapd · 11月24日 00:44

**「背景」** GPT-6.2 Sol 是 GPT-6 系列的新版本；据 MacRumors 报道，与 GPT-6 相比，它在识别照片中的路牌符号、标签文字等细节方面有所改进。OpenAI 此前已推出 GPT-6 Astra，并逐步向 Plus、Pro、Business 和 Enterprise 用户开放，此次 Chat 标签页的 Sol 版本延续了面向付费层级的推送方式。

**「影响」** 此次推送仅覆盖 Plus、Pro、Business 和 Enterprise 付费层级，免费用户暂未包含在内；依赖联网搜索、图片细节识别或主动提醒功能的付费用户需在 Chat 标签页确认是否已切换到该版本，而官方未公布回滚或版本切换选项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/11/23/openai-gpt-6-2-sol-chatgpt/">OpenAI Brings GPT - 6 . 2 Sol to ChatGPT &#x27;s Chat Tab - MacRumors</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT - 6 Astra: A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#LLM`, `#ChatGPT`, `#OpenAI`, `#product release`, `#AI`

---

<a id="item-tech-news-7"></a>
### [NariQ 发布 10GB 内近 BF16 质量的 Qwen3.8-27B 量化](https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF) ⭐️ 7.0/10

NariQ 发布了 Qwen3.8-27B 的 3-bit 及更低比特 GGUF 量化版本，称在智能体、数学、多语言推理和图像理解任务上接近 BF16 质量，其中 3-bit 文件约 10 GB。项目自报的基准显示，3-bit 在 DeepSWE 上为 41.0、Terminal-Bench 2.1 为 63.8、AIME 25+26 为 98.3，均与 BF16 的 39.8、62.6、97.7 相当；2-bit 则明显下降，DeepSWE 降至 28.6、AIME 降至 86.0。这些数字均为项目方自测，且目前运行需要其自建的 llama.cpp fork。

hackernews · toebee · 11月23日 13:42 · [社区讨论](https://news.ycombinator.com/item?id=50611402)

**「背景」** GGUF 是 llama.cpp 生态常用的模型文件格式，量化则通过降低权重精度来压缩模型体积，使大模型能在消费级硬件上运行。据 AI Weekly 报道，Nari Labs 于 11 月 23 日发布的 NariQ 采用基于真实编码智能体轨迹校准的网格编码（trellis-coded）训练后量化，将 Qwen3.8-27B 从 BF16 的 53.8GB 压缩到 3 比特每权重下的 10.12GB。

**「实际影响」** 目前要运行这些量化文件必须使用 NariQ 自建的 llama.cpp 分支，因此现有 llama.cpp 用户无法直接加载，需要自行编译该分支。社区反馈显示，在 Apple M3 Pro（18 GB）上以 3.0bpw 文件解码约为 3.8 tok/s，明显慢于 CUDA 环境，16 GB 内存的 Mac 能否运行尚未验证。

**「社区讨论」** 有评论者肯定该项目在多种长周期任务上做了“held out”验证，认为比常见的高算力 QAT 量化更审慎；但也有人指出，从图表看大部分提升来自评测 harness 的差异而非模型本身。另有用户追问文件变小时究竟丢失了什么信息，并报告在 M3 Pro（18 GB）上 3.0bpw 文件解码约 3.8 tok/s、2.0bpw 约 4.9 tok/s，远慢于 CUDA。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/nari-labs-nariq-quant-compresses-qwen38-27b-to-10gb-while-matching-bf16-on">Nari Labs&#x27; NariQ Quant Compresses Qwen3.8-27B to 10GB While ...</a></li>

</ul>
</details>

**标签**: `#quantization`, `#llm-inference`, `#llama.cpp`, `#gguf`, `#local-llm`

---

<a id="item-tech-news-8"></a>
### [Stalwart 宣称可替代 Microsoft Exchange](https://stalw.art/blog/microsoft-exchange-replacement/) ⭐️ 7.0/10

开源邮件服务器 Stalwart 在官方博客中宣布，它可以作为 Microsoft Exchange 的“直接替代品”（drop-in replacement）。该说法目前来自厂商公告，而非独立验证的兼容性测试结果；来源未给出具体版本号、支持范围或可用条件。社区讨论随即指出，这一表述可能被夸大：新版 Outlook 对 IMAP 的处理方式、Exchange 本地部署支持的变化，以及德国 GoBD 等合规归档要求，都可能限制实际替换的可行性。

hackernews · shaunpud · 11月23日 22:32 · [社区讨论](https://news.ycombinator.com/item?id=50620349)

**「背景」** Stalwart 是一个开源的一体化邮件与协作服务器，支持 IMAP、JMAP、SMTP、CalDAV、CardDAV 和 WebDAV 等协议。此次发布的是 Stalwart 1.2.0 版本，官方称其由此成为 Microsoft Exchange 的直接替代品。

**「对管理员的影响」** 对仍依赖本地 Exchange 账户的管理员而言，迁移前需先确认客户端路径：Stalwart 官方博客指出，新版 Outlook 已不再支持本地 Exchange 账户，但可接受 IMAP 账户，这可能是绕开 Exchange 协议的方式。因此“直接替换”的实际可行性取决于组织能否接受改用 IMAP 或更换客户端，而非仅替换服务器端。

**「社区讨论」** 多位评论者对“直接替代”提出质疑：traceroute66 认为，若新版 Outlook 强制将 IMAP 邮件同步到微软云端，Outlook 与 Exchange 的集成将难以复现；hobo123 也追问，在 Outlook 不再支持本地 Exchange 的情况下，客户如何继续使用 Stalwart。rmoriz 指出，Stalwart 的常规方案和开源版本都缺少德国税务审计所需的不可篡改、最长 10 年归档功能；andreashaerter 则认为，支持 MAPI 等微软协议虽能节省授权成本，却会进一步削弱开放邮件生态。markstos 补充称，Stalwart 是 Mozilla Thundermail 所用的邮件服务器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop - in replacement for Microsoft Exchange</a></li>
<li><a href="https://github.com/stalwartlabs/stalwart">GitHub - stalwartlabs/ stalwart : All-in-one Mail &amp; Collaboration server .</a></li>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange | Stalwart</a></li>

</ul>
</details>

**标签**: `#email`, `#open-source`, `#microsoft-exchange`, `#self-hosting`, `#interoperability`

---

<a id="item-tech-news-9"></a>
### [黎曼猜想「AI 证明」被指空转，作者承认代码能编译但无实质内容](https://x.com/i/web/status/2124987173439209561) ⭐️ 7.0/10

Alpöge 与 Claude 宣称证明了黎曼猜想及其广义版本，但只公开了约 1700 万行 Lean 代码、17.5 万个文件，没有提供人类可读的证明。Lean 与 Mathlib 社区次日表示对代码证明了该命题「有充分信心」，随后有研究者指出关键定义被写成恒真、几何条件形同虚设，证明可能只是空转。23 日 Alpöge 承认「25 万页是玩笑」，代码「满是垃圾但能编译」，并称批评完全合理。

telegram · zaihuapd · 11月24日 01:29

**「背景」** 据滑铁卢大学数学系页面记录，Levent Alpöge 于 2026 年 11 月 20 日宣布与 Anthropic 的 Claude 合作，给出了黎曼猜想及 Dirichlet L 函数广义黎曼猜想的证明；维基百科条目称该 Lean 证明的开发从 10 月 6 日持续到 11 月 16 日。相关视频介绍称，这份约 1700 万行的 Lean 代码由 Alpöge 与 Claude 在约六周内完成，已有数十人编译检查，但篇幅远超任何人可通读的范围。

**「影响」** 这一事件说明，Lean 能编译通过并不等于数学命题得到了实质证明：如果定义被写成恒真、前提条件形同虚设，形式化检查仍会通过。对依赖机器验证来评估 AI 生成数学结果的研究者而言，需要同时审查定义与假设是否承载了真实数学内容，而不能只看代码规模或编译结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Riemann_hypothesis">Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://www.youtube.com/watch?v=-Tzliv3mzds">AI Helped Prove the Riemann Hypothesis . Nobody Can... - YouTube</a></li>
<li><a href="https://math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/">Alpöge / Claude proof of the Generalized Riemann Hypothesis</a></li>

</ul>
</details>

**标签**: `#AI for mathematics`, `#Lean theorem proving`, `#formal verification`, `#Riemann Hypothesis`, `#AI reliability`

---

<a id="item-tech-news-10"></a>
### [4.5 万家企业联名致信欧盟，要求调查苹果 iPhone 浏览器限制](https://appleinsider.com/articles/26/11/23/eu-urges-to-challenge-apples-grip-on-iphone-browsers?utm_source=rss) ⭐️ 7.0/10

包括 Mozilla 和 Shopify 在内的企业及民间组织联名致信欧盟委员会，要求对苹果 iPhone 浏览器限制正式立案调查。信方称署名方合计代表约 4.5 万至 5.5 万家欧盟企业组织，联署将持续到 2026 年 12 月 3 日。信方主张，苹果虽依《数字市场法》允许欧盟竞品浏览器使用自有引擎，但技术与法律要求使厂商无法将现有欧盟用户迁出 WebKit，企业也仍依赖 App Store 触达用户。联名方测算，若半数原生 iOS 应用转为 Web 应用，欧盟企业每年可节省 110 亿欧元开发成本和 13 亿欧元 App Store 费用。

telegram · zaihuapd · 11月24日 03:02

**「背景」** 欧盟《数字市场法》（DMA）自 2024 年起要求苹果允许用户选择默认浏览器，并允许第三方浏览器在欧盟使用自有引擎。Mozilla 曾表示，DMA 生效后数百万欧盟用户选择了 Firefox，iOS 端日活翻倍；但 Mozilla 与开放网络倡导组织也指出，苹果设置的引擎迁移程序与技术条件仍使厂商难以真正脱离 WebKit。此次联名信正是在这一“名义开放、实际受限”的背景下，要求欧盟委员会正式立案调查。

**「影响与关注点」** 这封信目前只是向欧盟委员会提出的立案请求，并非已确认的监管行动，因此对苹果的实际约束尚未确定。对在欧盟运营的浏览器厂商和依赖 iOS 应用的企业而言，关键问题是现有用户能否真正迁出 WebKit，以及 App Store 分发依赖是否会被纳入调查范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mozilla.org/en/mozilla/internet-policy/apple-ios-browser-engine-rules/">Why there are still no non- WebKit browsers on iOS</a></li>
<li><a href="https://open-web-advocacy.org/blog/apples-browser-engine-ban-persists-even-under-the-dma/">Apple &#x27;s Browser Engine Ban Persists, Even Under the DMA</a></li>

</ul>
</details>

**标签**: `#apple`, `#eu-regulation`, `#dma`, `#browsers`, `#antitrust`

---

<a id="item-tech-news-11"></a>
### [黄循财：新加坡不会成为规避美国芯片管制的通道](https://www.bloomberg.com/news/articles/2026-11-24/singapore-won-t-be-conduit-to-skirt-us-chip-curbs-wong-says) ⭐️ 7.0/10

新加坡总理黄循财表示，新加坡不会被用作企业规避美国芯片出口管制的通道，当局正在调查 Megaspeed 采购英伟达芯片的交易。此前一天，美国商务部已将 Megaspeed 及另外 6 家东南亚企业列入贸易黑名单，《联邦公报》称这些企业存在向未获授权用户转移先进计算产品的“重大风险”，名单包括其在马来西亚、泰国的关联实体。路透社报道，阿里巴巴新加坡子公司 Apex Enterprise Solutions 同样在列，阿里称从未转移受管制的先进计算芯片。

telegram · zaihuapd · 11月24日 05:03

**「背景」** 美国商务部于 11 月 23 日在《联邦公报》发布正式通知，将总部位于新加坡的 Megaspeed 及其泰国、马来西亚子公司列入贸易黑名单，同时被列入的还有另外 6 家东南亚企业。据 CBS 新闻报道，美方此举源于 Megaspeed 涉嫌与中国存在关联，相关调查也牵出了围绕英伟达 CEO 黄仁勋的争议。黄循财的表态正是在这一黑名单公布后作出的。

**「影响」** 被列入黑名单的 Megaspeed 及其东南亚关联实体将面临美国出口限制，与其有芯片采购或转售往来的企业需要重新核查交易对手和最终用户，以避免触碰管制红线。新加坡总理的公开表态意味着当地监管机构可能加强对芯片流向的审查，在该地区处理英伟达等先进计算硬件的企业应准备应对更严格的合规问询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/megaspeed-trade-blacklist-nvidia-jensen-huang/">Trump administration adds Megaspeed to trade blacklist after ...</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/nov/23/megaspeed-us-trade-blacklist-nvidia">US adds Megaspeed, AI firm at center of Nvidia scandal, to ...</a></li>
<li><a href="https://www.ibtimes.com/us-blacklists-megaspeed-southeast-asian-firms-nvidia-chips-3810114">US Blacklists Nvidia-Linked Firm Over China Chip Fears. Six ...</a></li>

</ul>
</details>

**标签**: `#export controls`, `#semiconductors`, `#Nvidia`, `#AI hardware supply chain`, `#Singapore`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [vLLM 首日支持 ERNIE 5.5 Flash 的插件与推理加速](https://vllm.ai/blog/2026-11-24-ernie-5-5-flash-preview) ⭐️ 6.0/10

rss · vLLM Blog · 11月24日 00:00

**「背景」** ERNIE 5.5 Flash Preview 是百度推出的稀疏 MoE 模型，总参数 280B、每 token 激活 14B，支持 1M 上下文，并面向长程 Agent 任务。新模型通常需要等待 vLLM 合并代码或专用镜像，而这次团队希望发布当天就能在官方 vLLM 上运行。

**「方案」** 作者的核心做法是把模型集成做成独立插件 vLLM-ERNIE，安装到 vllm==0.32.0 同一环境即可，通过 vllm.general\_plugins 入口自动注册架构、配置、分词器和解析器，且只在 config.json 命中 ERNIE 架构时才导入模型代码，不影响同环境其他模型。性能上，团队针对 VHA 跨头混合、Multi-Router Latent MoE、MultiMax 输出头和门控注意力分别设计融合 kernel，并把推理期固定参数预折叠进权重，将 FP8 量化并入生产者 kernel，报告单 kernel 加速 1.55×–6.53×，并强调数值与逐算子实现一致。FlashIndexer 用轻量 head router 按当前 token 动态选择稀疏 indexer 头，仅需约 1B token 蒸馏微调，配合阈值预过滤，在 1M 上下文下报告 1.4× 索引加速。量化方面，路由专家采用 MXFP4（W4A8）QAT，训练与推理的量化粒度、scale 和舍入规则对齐；DSpark 草稿模型经多阶段训练，报告平均接受长度超过 4.0。不过这些加速数字缺少基准方法、硬件和基线说明，插件与 FlashIndexer 的取舍也基本未展开。

**「启示」** 作者想说明的是，插件机制可以让新模型在官方 vLLM 上首日可用，同时把 kernel 融合、索引器路由和 QAT 等模型侧优化快速交付；但性能收益仍需读者结合自身负载独立验证。

**标签**: `#inference-optimization`, `#vllm`, `#mixture-of-experts`, `#kernel-fusion`, `#quantization`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [纽约联储主席威廉姆斯：通胀仍高，加息需“随时间推进”](https://www.cnbc.com/2026/11/23/john-williams-fed-inflation-rate-hikes.html) ⭐️ 8.0/10

纽约联储主席约翰·威廉姆斯 11 月 23 日表示，美联储在把通胀降回 2%目标上“仍有工作要做”，并称相关行动可以“随时间推进”；美联储下次议息会议定于 12 月 8 日至 9 日，市场已完全计入在当前 3.75%至 4%的目标区间基础上加息 25 个基点的预期。

rss · CNBC Finance · 11月23日 21:02

**「背景」** 威廉姆斯预计通胀将在 2027 年更接近 2%、并在随后一年达到目标，他把当前通胀压力归因于伊朗冲突、人工智能建设带来的商品需求以及关税，同时称关税作为压力来源“已基本消退”。

**「影响」** 若美联储如市场预期在 12 月加息，与利率挂钩的信用卡、浮动利率贷款和部分企业融资成本将随之上升，而储蓄类产品收益率可能提高。

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [AI 抛售波及中国科技股，DeepSeek 与月之暗面上市计划承压](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

Anthropic 创纪录的 1195 亿美元 IPO 后全球 AI 股遭抛售，中国科技股自 6 月底以来累计蒸发 1.7 万亿美元，DeepSeek、月之暗面（Moonshot AI）和阶跃星辰的上市计划因此蒙上阴影。

telegram · zaihuapd · 11月23日 09:31

**「背景」** Anthropic 于 2026 年 11 月 19 日在纳斯达克上市，募资规模超过 SpaceX 6 月的上市，成为史上最大 IPO（tool-1-3）。此前，DeepSeek、月之暗面等中国 AI 初创公司已在推进上市计划（tool-2-2、tool-2-3）。

**「影响」** 抛售已直接冲击中国 AI 上市公司的估值：智谱较 6 月高点跌超 85%，MiniMax 本月跌破发行价，这使 DeepSeek、月之暗面、阶跃星辰等未上市 AI 公司的发行定价和上市窗口面临更大不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.france24.com/en/business/20261119-anthropic-begins-trading-1-5-trillion-company-biggest-ipo-record-ai">Anthropic blows past $2 trillion in Nasdaq debut, beating... - France 24</a></li>
<li><a href="https://www.outlookbusiness.com/deeptech/deepseek-moonshot-gigaai-why-chinas-ai-startups-are-rushing-for-ipo">DeepSeek , Moonshot , GigaAI: Why China&#x27;s AI Startups Are Rushing...</a></li>
<li><a href="https://fortune.com/2026/07/23/moonshot-deepseek-great-chinese-ai-ipo-rush/">Moonshot , DeepSeek , and the Great Chinese AI IPO Rush | Fortune</a></li>

</ul>
</details>

**标签**: `#AI`, `#IPO`, `#China tech`, `#market selloff`, `#equities`

---

<a id="item-finance-news-3"></a>
### [上海地铁票价 21 年来首次调整](https://weibo.com/1699432410/5368461393397183) ⭐️ 7.0/10

上海宣布轨道交通票价时隔 21 年首次调整，新起乘价为 3 元、起步覆盖 0 至 4 公里，之后按 4、4、4、7、7、10、10 公里分段加 1 元，50 公里以上每 15 公里加 1 元，新票价与优惠自 12 月 1 日起实施。

telegram · zaihuapd · 11月23日 10:45

**「背景」** 上海地铁现行票价自 2005 年前后沿用至今，此次是 21 年来首次调整。据腾讯新闻援引有关部门初步测算，新票价机制叠加优惠措施后，平均每人次票价将从 4.23 元提高至 5.22 元，提高 0.99 元。

**「影响」** 高频通勤乘客可通过计次票或当月同一支付渠道累计满 90 元后享 9 折来部分抵消涨价影响，但具体节省幅度取决于个人出行次数和里程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260819A0ARAE00">时隔 21 ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260819A0A7CX00">news.qq.com/rain/a/20260819A0A7CX00</a></li>
<li><a href="https://hi.online.sh.cn/content/2026-08/21/content_10481931.htm">hi.online.sh.cn/content/2026-08/21/content_10481931.htm</a></li>
<li><a href="https://c.m.163.com/news/a/L4NE02LA0514R9P4.html">c.m.163.com/news/a/L4NE02LA0514R9P4.html</a></li>

</ul>
</details>

**标签**: `#public transit`, `#pricing`, `#Shanghai`, `#consumer costs`, `#policy`

---

<a id="item-finance-news-4"></a>
### [马斯克承认 SpaceX 在 AI 领域落后，转而向 Anthropic 和 Google 出租算力](https://www.nytimes.com/2026/11/23/business/elon-musk-ai-anthropic-google.html) ⭐️ 7.0/10

据《纽约时报》11 月 23 日报道，自今年 5 月起，SpaceX 每月从其数据中心向 Anthropic、Google 等公司出租算力，月收入达数十亿美元；三名知情人士称，马斯克向员工表示 SpaceX 在 AI 上落后，出租算力比自用更赚钱。

telegram · zaihuapd · 11月24日 02:06

**「背景」** 据《纽约时报》报道，SpaceX 自今年 5 月起将自有数据中心的算力出租给 Anthropic、Google 等竞争对手，马斯克向员工表示公司在 AI 上落后，出租算力比自用更赚钱。此前有报道称，Anthropic 自 5 月起每月支付约 12.5 亿美元租用孟菲斯 Colossus 数据中心算力，Google 则从 10 月起每月支付约 9.2 亿美元租用约 11 万块 GPU，但这些具体金额尚未获得独立证实。

**「影响」** 若这一收入规模属实，SpaceX 将获得可观的经常性现金流，而 Anthropic 和 Google 则能以租用方式快速扩充算力，无需自建同等规模的数据中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/23/business/elon-musk-ai-anthropic-google.html">Elon Musk Faces an A.I. Dilemma at SpaceX - The New York Times</a></li>
<li><a href="https://www.techtimes.com/articles/331389/20261124/spacex-compute-rentals-outearn-grok-musk-ranks-revenue-per-gpu-above-benchmarks-nyt-says.htm">SpaceX Compute Rentals Outearn Grok as Musk ... - Tech Times</a></li>
<li><a href="https://www.linkedin.com/posts/fillidefilla_so-grok-belongs-to-spacex-now-and-theyre-activity-7480238218051846146-PN_V">SpaceX Rents Data Center to Anthropic for 1.25 Billion ... | LinkedIn</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2oxaGNhVUVSSFBqY0hSdzBFWlFDZ0FQAQ?hl=en-IN&amp;gl=IN&amp;ceid=IN:en">Google News - Anthropic to pay SpaceX $45 billion for computing ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#SpaceX`, `#Anthropic`, `#Google`, `#compute rental`

---