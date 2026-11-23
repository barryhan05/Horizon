---
layout: default
title: "Horizon Summary: 2026-11-23 (ZH)"
date: 2026-11-23
lang: zh
---

> 从 28 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [OpenAI 发文论证困惑度与模型智能相关，引发技术争论](#item-tech-news-1) ⭐️ 7.0/10
2. [Phison 发布太空级 SSD，488 TB 将随 StarVault-001 入轨](#item-tech-news-2) ⭐️ 7.0/10
3. [谷歌搭建模拟互联网测试 Chrome AI 代理](#item-tech-news-3) ⭐️ 7.0/10
4. [Windows Server 2028 默认移除 WoW64，32 位应用需手动装回](#item-tech-news-4) ⭐️ 7.0/10

**科技博客**
1. [在不确定时，广泛试错比谨慎分析更有效](#item-tech-blog-1) ⭐️ 6.0/10

**财经新闻**
1. [美股科技股大跌，亚洲多地出台稳市措施](#item-finance-news-1) ⭐️ 9.0/10
2. [英媒报道：太子集团相关人员被指参与英伟达芯片对华走私](#item-finance-news-2) ⭐️ 7.0/10
3. [中国要求美国撤销电话号段接入限制](#item-finance-news-3) ⭐️ 7.0/10
4. [蚂蚁集团领投 Simplexity Robotics 1 亿美元融资，投后估值 16 亿美元](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发文论证困惑度与模型智能相关，引发技术争论](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 7.0/10

OpenAI 发布一篇立场性文章，主张更低的困惑度（perplexity）与更强的模型智能相关。文章未在正文中给出困惑度的定义，社区评论者 hazrmard 补充说明：困惑度衡量模型预测下一个 token 时的“意外程度”，最差情况等于词表大小，最好情况为 1。该文在 Hacker News 获得 513 分、353 条评论，讨论集中在交叉熵损失、强化学习与“压缩即智能”等方向。需要说明的是，这是一篇论述性文章，而非新模型发布或经独立验证的突破。

hackernews · acossta · 11月22日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=50601525)

**「背景」** OpenAI 首席科学家 Jakub Pachocki 在题为《Perplexity and Intelligence》的文章中主张，这一长期用于训练的指标可作为衡量模型能力进展的共享标尺。文章把 OpenAI 主评测集上的具体对数困惑度数值与各阶段出现的能力对应起来，例如 GPT-3.5 约为 0.99、GPT-4 约为 0.91，而约 0.76 的模型开始在长期未解的开放数学问题上取得突破。

**「对模型评测的影响」** 若这一相关性成立，团队可能获得一个比现有复杂基准更简单的基础模型能力比较指标；但评论者指出，文章未给出困惑度的定义，且该指标依赖统一的留出评测集与分词方式，跨厂商比较前需先确认这些条件一致。

**「社区讨论」** 评论者 jrflo 表示，在强化学习日益普及的背景下，交叉熵损失仍呈现如此清晰的趋势令人意外，并认为这种简单基准比日益复杂的评测更有价值。d\_burfoot 认为困惑度与智能的对应关系“事后看只能如此”，理由是智能的本质是从原始数据中提取世界模型，而预测率即压缩率正好刻画这一进展，并称自己早在 2008 年的论文中就提出过类似观点。reasonableklout 则引用 Mustafa Suleyman 的推文称，微软已加入该评估，报告 MAI-2 Base 的 log-perplexity 为 0.819，与 GPT-5.6 Sol base 处于同一量级；该说法来自厂商自述，未经独立核实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence - OpenAI</a></li>
<li><a href="https://www.datastudios.org/post/openai-proposes-perplexity-limits-frontier-ai-development">OpenAI proposes perplexity limits on frontier AI and ...</a></li>
<li><a href="https://officechai.com/ai/openai-wants-perplexity-to-become-the-industrys-shared-yardstick-for-ai-progress-and-safety-limits/">OpenAI Wants &#x27;Perplexity&#x27; To Become The Industry&#x27;s Shared ...</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#language-models`, `#perplexity`, `#benchmarking`, `#openai`

---

<a id="item-tech-news-2"></a>
### [Phison 发布太空级 SSD，488 TB 将随 StarVault-001 入轨](https://videocardz.com/newz/phison-announces-488tb-of-ssd-storage-for-space-data-centers-pricing-expected-to-be-astronomical) ⭐️ 7.0/10

Phison 发布面向航天器、卫星和在轨数据中心的 Pascari Space SSD 系列，分为 Flight Critical、Main Storage 与 Orbital Data Center 三类，单盘最高 128 TB。该系列已上市，并确认将用于 Lonestar Data Holdings 的轨道数据中心 StarVault-001：后者计划于 2027 年上半年发射，搭载合计 488 TB 的 Phison SSD，进入低地球轨道后可用容量约 370 TB。Phison 还称，部分型号采用 pSLC 可将写入寿命提高至多 60 倍，但这一耐久性说法尚无独立验证。

telegram · zaihuapd · 11月22日 10:31

**「背景」** Lonestar Data Holdings 是一家推进在轨数据中心的公司，其 StarVault-001 计划部署于低地球轨道。Phison 此次公布的 Pascari Space SSD 正是为该任务提供存储，488 TB 为整机合计容量，入轨后可用容量约 370 TB。

**「影响」** 对在轨计算项目而言，这意味着存储容量和写入耐久性开始按航天环境单独设计，而不是直接沿用地面数据中心 SSD；StarVault-001 的实际可用容量约为标称值的 76%，规划在轨存储预算时需按此折算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dzen.ru/a/awLShV56vGiwFBoU">Она включает категории Flight Critical, Main Storage и Orbital Data ...</a></li>

</ul>
</details>

**标签**: `#storage`, `#hardware`, `#space-computing`, `#data-centers`, `#ssd`

---

<a id="item-tech-news-3"></a>
### [谷歌搭建模拟互联网测试 Chrome AI 代理](https://www.landian.news/archives/128701.html) ⭐️ 7.0/10

据报道，谷歌为 Chrome 的 AI 代理搭建了一个名为 Mirror Dimension 的模拟互联网，在隔离环境中测试其打开网站、搜索浏览、登录、加购和完成任务等操作。该环境包含数千个模拟网站，每名工程师单独隔离测试，每天运行超过 1000 个测试案例，重点防御恶意网页的提示词注入等攻击。上述信息来自蓝点网的二手报道，尚无谷歌官方文档或独立验证，具体上线时间和适用范围不明。

telegram · zaihuapd · 11月23日 01:30

**「背景」** 谷歌在 2026 年 11 月 19 日的安全博客中介绍了 Mirror Dimension，Wired 同日报道了这一环境。它是一个由数千个模拟网站构成的隔离“合成网络”，用于在接近真实的上网场景中评估 Chrome 的自动浏览（auto browse）代理，而不必承担真实世界中的安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents: Evaluating Browser-Use Agents ...</a></li>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘Mirror Dimension’ Internet to Test Its ...</a></li>
<li><a href="https://explainx.ai/blog/google-mirror-dimension-synthetic-web-chrome-auto-browse-agents-prompt-injection-testing-2026">Google Mirror Dimension: Fake Web for Chrome AI Agents ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#browser automation`, `#prompt injection`, `#AI security`, `#Chrome`

---

<a id="item-tech-news-4"></a>
### [Windows Server 2028 默认移除 WoW64，32 位应用需手动装回](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 7.0/10

微软在 Ignite 2026 上宣布，Windows Server 2028 将默认不再包含 WoW64 兼容子系统，因此系统开箱即无法运行 32 位应用。该版本计划于 2027 年秋季与 Windows 11 27H2 一同发布。需要运行 32 位软件的用户可通过按需功能（FoD）将 WoW64 装回，在 Server Core 上一般使用 PowerShell 或 DISM 添加。微软称此举旨在减少攻击面、阻止 32 位恶意软件；Windows 11 目前仍保留 WoW64，微软未公布移除计划。

telegram · zaihuapd · 11月23日 03:03

**「背景」** WoW64 是 Windows 中负责在 64 位系统上运行 32 位应用的兼容层，此前一直作为系统内置组件随 Windows 提供。微软在 Ignite 2026 上宣布的这项调整属于其逐步削减 32 位支持的一部分，同一版本中 .NET Framework 3.5 也不再作为内置可选组件或按需功能提供。

**「影响与应对」** 服务器运维方在升级到 Windows Server 2028 前，需要盘点仍依赖 32 位组件的应用，并规划通过 FoD 安装 WoW64 的部署流程，否则这些程序在默认配置下将无法启动。由于该功能改为可选安装，自动化部署脚本和镜像模板也需相应调整。

<details><summary>参考链接</summary>
<ul>
<li>Features Removed or No Longer Developed in Windows Server - Microsoft Learn</li>
<li>32-bit apps&#x27; days are numbered as Microsoft strips support bit by bit, starting with Windows Server 2028, but Windows 11 is safe for now</li>

</ul>
</details>

**标签**: `#windows-server`, `#wow64`, `#32-bit-compatibility`, `#microsoft`, `#platform-deprecation`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [在不确定时，广泛试错比谨慎分析更有效](https://seangoedecke.com/when-in-doubt-flail-about/) ⭐️ 6.0/10

rss · Sean Goedecke · 11月23日 00:00

**「背景」** 面对缺乏明确指引、不知道什么会有帮助的模糊处境，工程师的本能往往是先谨慎分析、等理解清楚再行动。Sean Goedecke 认为这种直觉常常是错的：在信息不足时，等待并不会自动带来理解，反而可能把精力耗在注定失败的方向上。

**「方案」** 作者提出，更好的做法是“乱撞”（flailing）：大量尝试不同方案，密切关注来自同事和现实结果的反馈，并果断放弃没有获得积极反馈的尝试。多试几件事不仅扩大与现实的接触面，也因为大多数计划本来就会失败，只有试得足够多才可能撞上一个好方向；同时，手里有多个计划能避免对单一方案过度投入，从而更容易及时止损。作者把这种策略对应到三类场景：产品尚未找到市场契合点时，围绕核心价值在边缘快速试错，他以自己在 GitHub Models 的经历为例，许多功能没有成功，但“用 GitHub Actions token 运行 AI 推理”意外地有粘性，后来成为“Continuous AI”的种子；面对过于复杂或庞大的系统时，与其通读全貌再提改动，不如先做一批试探性修改，看效果再决定是否深挖，AI 代理可以帮忙快速生成多个重构方案；在组织层面，当问题不是技术性的、相关方也说不清想要什么时，可以主动尝试自动化手工工作、接手任务或提出长期计划，但此时最需要对反馈敏感，及时放弃失败方案才能建立信任，否则不满会转向自己。作者强调，从内部感受看这确实像在乱撞、反复失败，但这种不适是成为有效工程师需要穿过的心理障碍之一。

**「启示」** 作者的核心论点是：在高度不确定的环境中，有纪律的广泛试错加紧密反馈循环，比先求完整理解再行动更快、更可靠；前提是必须对反馈敏感并愿意立刻放弃失败方案，否则“乱撞”就会变成损害声誉的坏习惯。

**标签**: `#engineering-practice`, `#decision-making`, `#experimentation`, `#organizational-dynamics`, `#career-advice`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美股科技股大跌，亚洲多地出台稳市措施](https://news.bjd.com.cn/2026/11/22/12039852.shtml) ⭐️ 9.0/10

美国 AI 科技股周五大幅下跌，纳斯达克指数单日下跌 5.28%，费城半导体指数下跌近 11%；随后中国内地、韩国和中国台湾地区相继出台融资、卖空和回购方面的稳定市场措施。

telegram · zaihuapd · 11月22日 13:24

**「背景」** 费城半导体指数是追踪美国主要芯片股表现的行业指数，其近 11%的单日跌幅反映出市场对 AI 相关股票的集中抛售。

**「影响」** 中国台湾地区自 11 月 23 日起禁止平盘以下卖空，并将融券保证金比例从 130%提高到 150%，这会直接提高当地投资者做空股票的资金门槛；韩国自 11 月 24 日起为期三个月放宽上市公司每日回购订单数量限制，可能影响当地回购市场的操作空间。

**标签**: `#US tech stocks`, `#semiconductor selloff`, `#market stabilization policy`, `#short-selling rules`, `#Asian markets`

---

<a id="item-finance-news-2"></a>
### [英媒报道：太子集团相关人员被指参与英伟达芯片对华走私](https://www.ft.com/content/f3ad8a81-3890-4a8a-8853-ff0a94b08ba9?syn-25a6b1a6=1) ⭐️ 7.0/10

英国《金融时报》援引知情人士报道，被美国财政部指为柬埔寨太子集团“二号人物”的胡小伟涉嫌参与将英伟达芯片运入中国；该报援引的贸易数据显示，2024 年 12 月至 2025 年 12 月，Megaspeed 马来西亚子公司进口货物申报价值约 46 亿美元。太子集团否认胡小伟曾为其工作，并称有关非法网络和私人飞机走私的指控缺乏事实依据。

telegram · zaihuapd · 11月22日 04:34

**「背景」** 美国财政部此前已对柬埔寨太子集团及其关联人员实施制裁，其中包括被新加坡调查洗钱的胡小伟（相关报道见 tool-1-2）。此次报道涉及的 Megaspeed 是一家总部位于新加坡的云计算服务商，马来西亚方面正调查其子公司进口的人工智能芯片是否被再出口（tool-2-3）。

**「影响」** 若相关指控成立，美国出口管制的执行缺口可能使受管制的人工智能芯片继续经第三国流入中国，从而削弱管制效果；英伟达董事会已设立委员会监督出口合规，显示企业正面临更严格的审视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.straitstimes.com/singapore/courts-crime/spore-investigating-2-men-linked-to-prince-group-after-us-sanctions-600m-in-assets-seized-so-far">S’pore investigating 2 men linked to Prince Group hit by US sanctions ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/malaysia-says-it-is-investigating-if-any-chips-linked-speedmatrix-were-re-2026-11-13/">Malaysia probing whether chips linked to Megaspeed unit were ...</a></li>
<li><a href="https://www.atlanticcouncil.org/dispatches/beyond-the-spy-scandal-what-the-nvidia-megaspeed-case-reveals-about-export-controls/">Beyond the spy scandal: What the Nvidia-Megaspeed case ...</a></li>
<li><a href="https://www.cbsnews.com/news/nvidia-export-control-committee-china-chips/">Nvidia&#x27;s board forms export oversight panel after scrutiny ...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#export controls`, `#Nvidia`, `#smuggling`, `#Cambodia`

---

<a id="item-finance-news-3"></a>
### [中国要求美国撤销电话号段接入限制](https://www.bloomberg.com/news/articles/2026-11-22/china-objects-to-us-curbs-on-telecoms-access-to-phone-numbers) ⭐️ 7.0/10

中国商务部 11 月 22 日敦促美国撤销一项禁止中国移动、中国电信、中国联通直接获取美国电话号码的措施，称其违反非歧视与公平竞争原则。美国联邦通信委员会（FCC）于 11 月 19 日投票收紧对申请直接接入美国号码的互联网语音服务商的安全要求，新增国家安全认证，以阻止其“涵盖清单”上的实体、设备和服务接入美国网络。

telegram · zaihuapd · 11月22日 06:44

**「背景」** 美国联邦通信委员会（FCC）于 11 月 19 日投票通过新规，要求申请直接接入美国电话号码的互联网语音服务商通过新的国家安全认证，以阻止其“涵盖清单”上的实体、设备和服务接入美国网络。这三家中国运营商此前已被禁止向美国提供国际电信服务。

**「影响」** 若该措施维持，三家中国国有运营商将无法直接取得美国号码资源，中美之间的语音通话与短信等通信服务可能需经第三方转接，成本与合规负担随之上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fcc.gov/document/fcc-cracks-down-bad-actors-access-us-phone-numbers-0">FCC Cracks Down on Bad Actors&#x27; Access to U.S. Phone Numbers</a></li>
<li><a href="https://www.reuters.com/world/fcc-votes-ban-chinese-telecoms-direct-access-us-phone-numbers-2026-11-19/">FCC votes to ban Chinese telecoms from direct access to US ...</a></li>
<li><a href="https://finance.biggo.com/news/af7ccb0c-75c7-434b-834c-ced72af0d3c4">FCC Blocks China Mobile, Telecom and Unicom From Direct ...</a></li>

</ul>
</details>

**标签**: `#telecom regulation`, `#US-China relations`, `#FCC`, `#China carriers`, `#policy dispute`

---

<a id="item-finance-news-4"></a>
### [蚂蚁集团领投 Simplexity Robotics 1 亿美元融资，投后估值 16 亿美元](https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race) ⭐️ 7.0/10

彭博报道，中国具身智能公司 Simplexity Robotics 完成 1 亿美元 pre-A 轮融资，由蚂蚁集团领投，投后估值 16 亿美元；阿里巴巴、腾讯、HongShan（红杉中国）和蓝驰创投跟投，董事长兼联合创始人 Wang Kai 已向彭博确认。

telegram · zaihuapd · 11月23日 02:02

**「背景」** Simplexity Robotics 于 2025 年 7 月在杭州成立，核心团队来自理想汽车；据彭博报道，该公司今年 3 月披露成立半年内已完成五轮融资、累计融资 20 亿元人民币，当时投后估值已超过 10 亿美元。蚂蚁集团近两年持续投资中国人形机器人领域，据 CryptoBriefing 报道，其在 18 个月内已达成十余笔相关交易。

**「影响」** 这笔资金将用于与宇树、优必选等更成熟的人形机器人厂商争夺市场，可能加剧中国具身智能行业的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cryptobriefing.com/ant-group-humanoid-robots-dozen-deals/">Ant Group rushes into humanoid robots with dozen deals in 18 months</a></li>

</ul>
</details>

**标签**: `#funding`, `#robotics`, `#China tech`, `#venture capital`, `#Ant Group`

---