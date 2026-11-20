---
layout: default
title: "Horizon Summary: 2026-11-20 (EN)"
date: 2026-11-20
lang: en
---

> From 33 items, 14 important content pieces were selected

---

**Technology News**
1. [Anthropic Debuts on Nasdaq as AI Valuation Test](#item-tech-news-1) ⭐️ 8.0/10
2. [Reported &\#x27;java4shell&\#x27; Java Bug Surfaces via OpenJDK PR](#item-tech-news-2) ⭐️ 8.0/10
3. [PostgreSQL 19 Adds WAIT FOR LSN for Standby Read-Your-Writes](#item-tech-news-3) ⭐️ 8.0/10
4. [OpenAI models cut chip cell area, lift AMD GPU PPA up to 14%](#item-tech-news-4) ⭐️ 8.0/10
5. [PHP 流包装器在混合大小写 scheme 下静默禁用 TLS](#item-tech-news-5) ⭐️ 8.0/10
6. [Gemini 4 Neon Tops Models Engineering Index, Users Report Mixed Results](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic says Claude helped solve two black hole physics problems](#item-tech-news-7) ⭐️ 7.0/10
8. [UK tribunal forces government to admit secret Apple encryption order](#item-tech-news-8) ⭐️ 7.0/10
9. [European Commission Runs Matrix for Over 40,000 Staff](#item-tech-news-9) ⭐️ 7.0/10
10. [PHP to ship CRITICAL-severity security release](#item-tech-news-10) ⭐️ 7.0/10
11. [Gemini 开始在 Mac 上替用户操作，并支持后台运行和暂停](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Anthropic Shares Open 34% Above IPO Price on Nasdaq Debut](#item-finance-news-1) ⭐️ 9.0/10
2. [拼多多三季度营收1083亿元，盘前股价涨逾8%](#item-finance-news-2) ⭐️ 7.0/10
3. [AI Investment Doubts Weigh on Asian Stocks After Anthropic IPO](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic Debuts on Nasdaq as AI Valuation Test](https://www.reuters.com/business/finance/anthropics-historic-debut-put-ais-promise-peril-wall-st-test-2026-11-19/) ⭐️ 8.0/10

Anthropic began trading on Nasdaq, an event Reuters framed as a major test of AI valuations. Community commenters cited specific figures: shares priced at $83, opened at $111.50, and closed at $97.17, up 17.07% from the IPO price but down 12.85% from the opening price. The supplied material contains no company statement, filing details, or independent confirmation of these numbers, so the pricing figures should be treated as commenter-reported rather than verified.

hackernews · wslh · Nov 19, 17:02 · [Discussion](https://news.ycombinator.com/item?id=50562754)

**「Background」** Anthropic&\#x27;s listing follows a record-setting offering: Reuters reported the Claude maker raised $81.3 billion and priced shares at $83 ahead of its Nasdaq debut under the ticker ANT. Earlier reporting had indicated a target range of $70 to $78 per share and a valuation of roughly $1 trillion or more, so the final pricing came in above that range.

**「Impact」** Commenters noted that the gap between the IPO price and the opening price means investors who bought at the open were down on the day, while those allocated shares at $83 were up. One commenter argued the resulting valuation sits below what OpenAI has reportedly sought in private markets, though that comparison is an opinion offered without supporting evidence in the supplied material.

**「Community Discussion」** Several commenters, including self-described software engineers, debated whether the debut signals the end of well-paid programming careers, with one calling the &quot;gravy train&quot; over and another describing it as the sunset of a way of making a living. Others focused on the trading mechanics, pointing out that the same closing price can be read as a gain or a loss depending on the entry point.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/live/anthropic-ipo-live-claude-maker-goes-public-nasdaq-after-record-share-offering-2026-11-19/">Anthropic IPO live: Claude maker breaks $2 trillion valuation ...</a></li>
<li><a href="https://cryptobriefing.com/anthropic-ipo-november-19-trillion-valuation/">Anthropic targets November 19 Nasdaq debut at valuation above ...</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#Anthropic`, `#IPO`, `#software engineering careers`, `#AI valuations`

---

<a id="item-tech-news-2"></a>
### [Reported &\#x27;java4shell&\#x27; Java Bug Surfaces via OpenJDK PR](https://github.com/openjdk/jdk/pull/32781) ⭐️ 8.0/10

A reported Java vulnerability nicknamed &quot;java4shell&quot; surfaced through an OpenJDK pull request \(jdk\#32781\), according to the item. Community comments describe a disclosure sequence in which the PR author said on October 1 that Oracle had emailed asking them not to proceed with the PR until approval, and on October 28 that the work had been &quot;taken over by Oracle.&quot; The supplied evidence is secondhand and does not establish the vulnerability&\#x27;s technical details, affected versions, or severity, so the specific impact of the bug remains unverified.

hackernews · notmine1337 · Nov 19, 11:47 · [Discussion](https://news.ycombinator.com/item?id=50558906)

**「Background」** The vulnerability discussed here is tracked as CVE-2026-114938, which researchers at Calif disclosed on November 17 as &quot;Java 4 Shell,&quot; describing remote code execution in OpenJDK when it processes Base64 input. OpenJDK is the open implementation underlying Oracle Java SE and most other Java distributions, so the affected code is widely deployed. The community thread adds disclosure context: the PR author says Oracle asked them on October 1 not to proceed with a PR until approval, and by October 28 the work was &quot;taken over by Oracle.&quot;

**「Impact」** Because the item provides no confirmed affected versions, exploit conditions, or patch status, Java users and operators cannot yet assess exposure from this report alone; the practical consequence is to watch the OpenJDK PR and Oracle&\#x27;s advisory for authoritative details rather than act on the nickname or community accounts.

**「Community Discussion」** Commenters debated whether the LLM-assisted researchers independently discovered the bug or whether the model may have read the earlier bug report or the repository&\#x27;s issues and PRs, with one commenter noting that simultaneous disclosures are now common and that judging criticality and building an exploit still require supervision. Another commenter said they independently found the issue ahead of disclosure via a fuzzing harness without internet access and reported it to Oracle, while acknowledging it could have been in the model&\#x27;s training data.

<details><summary>References</summary>
<ul>
<li><a href="https://securitylabs.datadoghq.com/articles/java4shell-remote-code-execution-in-openjdk-cve-2026-114938/">Java 4 Shell : Remote Code Execution in OpenJDK (CVE-2026-114938)</a></li>
<li><a href="https://www.comss.ru/page.php?id=22943">Java 4 Shell : критическая уязвимость в OpenJDK позволяет...</a></li>

</ul>
</details>

**Tags**: `#java`, `#security`, `#vulnerability-disclosure`, `#openjdk`, `#llm-assisted-research`

---

<a id="item-tech-news-3"></a>
### [PostgreSQL 19 Adds WAIT FOR LSN for Standby Read-Your-Writes](https://simonwillison.net/2026/Nov/19/postgresql-19/) ⭐️ 8.0/10

PostgreSQL 19 has been released, roughly two months later than the usual September cadence; the source attributes the delay mainly to the volume of issues the team had to address amid ongoing AI-reported vulnerabilities. The release adds a \`WAIT FOR LSN\` command that lets a session on a standby replica wait until the standby has replayed the write-ahead log up to a specified log sequence number \(LSN\) before running a query, giving applications that send reads to standbys read-your-writes consistency. In the illustrated pattern, an application records the value returned by \`pg\_current\_wal\_insert\_lsn\(\)\` after a write on the primary, then issues \`WAIT FOR LSN &\#x27;0/0306EE20&\#x27; WITH \(TIMEOUT &\#x27;0.1s&\#x27;\)\` on the standby before reading; the timeout is optional, and when supplied it produces an error if the replica does not catch up in time.

rss · Simon Willison · Nov 19, 20:43

**「Background」** PostgreSQL&\#x27;s annual major releases have typically shipped in September, so this year&\#x27;s arrived about two months later than usual. The source attributes the delay mainly to the volume of issues the PostgreSQL team had to address amid what it calls the ongoing wave of AI-reported vulnerabilities. The read-your-writes pattern itself is not new: the source notes Wikipedia&\#x27;s MediaWiki has long implemented a hand-rolled version against MySQL replication, saving the primary&\#x27;s binlog position and waiting for a replica to catch up before reading.

**「Impact」** Applications that route reads to standbys can now enforce read-your-writes consistency in the database rather than hand-rolling a replication-lag check, as the source notes Wikipedia&\#x27;s MediaWiki does against MySQL using \`WAIT\_FOR\_EXECUTED\_GTID\_SET\(\)\` and \`SOURCE\_POS\_WAIT\(\)\`. Teams adopting the pattern must persist the primary&\#x27;s LSN between requests and choose a timeout, since a too-short timeout turns replica lag into a query error.

**Tags**: `#postgresql`, `#databases`, `#replication`, `#open-source`, `#security`

---

<a id="item-tech-news-4"></a>
### [OpenAI models cut chip cell area, lift AMD GPU PPA up to 14%](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 8.0/10

OpenAI says its models contributed to the design of its own Jalapeño inference chip, reducing standard-cell area by about 13% in vector units and about 10% in matrix units, with the optimizations validated during chip bring-up. In work with AMD, OpenAI reports power, performance, and area \(PPA\) gains of up to 14% over a highly optimized baseline for flagship GPU IP, with some changes already in designs sent to manufacturing. OpenAI also announced a collaboration with Synopsys to train a GPT-Synopsys model. These are vendor-reported results from OpenAI with limited independent detail, and the Synopsys model is described as a training collaboration rather than a shipped product.

telegram · zaihuapd · Nov 19, 09:30

**「Background」** Jalapeño is OpenAI&\#x27;s own inference-only chip, developed with Broadcom; external reporting from June 2026 said OpenAI would still rely on Nvidia hardware for pre-training workloads. Earlier coverage in late October 2026 already reported that OpenAI used AI to help design Jalapeño, including a roughly 10% reduction in matrix-unit size versus a human-optimized design, so the new announcement extends those claims to vector units and to AMD GPU IP.

**「Impact」** The reported gains suggest AI-assisted optimization is being applied to production-bound chip designs rather than only research prototypes, since OpenAI says some AMD changes are already in designs sent to manufacturing. Readers evaluating the claims should note that the baselines are described as already highly optimized and that no independent measurements were provided.

<details><summary>References</summary>
<ul>
<li>Broadcom and OpenAI Unveil Jalapeño LLM Inference Chip | AI Weekly</li>
<li>OpenAI and Synopsys Use AI to Design Chips Like Jalapeno | Sergey Kochnev - Facebook</li>

</ul>
</details>

**Tags**: `#AI for chip design`, `#OpenAI`, `#AMD`, `#hardware`, `#EDA`

---

<a id="item-tech-news-5"></a>
### [PHP 流包装器在混合大小写 scheme 下静默禁用 TLS](https://x.com/ljachowicz/status/2123477025268924514) ⭐️ 8.0/10

PHP 的 HTTP 和 FTP 流包装器在匹配 URL scheme 时不区分大小写，但只有在第五个字符为小写“s”时才启用 TLS。因此，像 \`httpS://\`、\`HTTPS://\` 和 \`FTPS://\` 这样的 URL 会静默地以明文 HTTP 或 FTP 发送，暴露令牌、Basic 认证凭据、Cookie、POST 请求体和 FTP 登录信息；被第三方重定向到此类地址也会触发该问题。该缺陷被追踪为 CVE-2026-128064（GHSA-f6gg-rchx-xw8j），CVSS 4.0 评分为 8.2，并已在 PHP 8.2.36、8.3.37、8.4.28、8.5.13 和 8.6.0 中修复。PHP 8.1 及更早版本已停止支持（EOL），不会获得修复，因此这些版本上的用户必须自行将 URL scheme 规范化为小写。

telegram · zaihuapd · Nov 20, 03:04

**「Background」** PHP&\#x27;s HTTP and FTP stream wrappers are the built-in handlers behind functions such as file\_get\_contents\(\) and fopen\(\), which accept URLs and route them to the matching protocol. The wrappers matched scheme names case-insensitively, but the TLS decision depended on a lowercase &quot;s&quot; at a fixed position, so mixed-case schemes were routed as plaintext. CVE-2026-128064 describes this behavior, including URLs received as HTTP redirect targets.

**「影响」** 任何在 PHP 8.1 或更早版本上使用 HTTP/FTP 流包装器并接受用户提供或重定向 URL 的代码，仍会暴露于静默明文传输的风险，因为该分支不会获得补丁。在受支持的版本上，升级到已修复的版本即可解决该问题；在无法升级的情况下，在将 scheme 传给流包装器之前将其转换为小写，是来源中提到的变通方法。

<details><summary>References</summary>
<ul>
<li><a href="https://app.opencve.io/cve/CVE-2026-128064">CVE-2026-128064 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://www.tenable.com/cve/CVE-2026-128064">CVE-2026-128064 | Tenable®</a></li>
<li><a href="https://www.rapid7.com/db/vulnerabilities/cve-2026-128064/">CVE-2026-128064: PHP Group PHP: Mixed-case HTTPS and FTPS ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#php`, `#tls`, `#vulnerability`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [Gemini 4 Neon Tops Models Engineering Index, Users Report Mixed Results](https://git-aarvin.github.io/mei/) ⭐️ 7.0/10

A Hacker News post claims that Gemini 4 Neon is now ranked \#1 on the Models Engineering Index, a third-party benchmark site. The claim comes from the post itself, and the supplied material contains no independent verification of the ranking or its methodology. Commenters describe hands-on use of Neon for coding, documentation, and long-running porting work, but their impressions are anecdotal and mixed. One commenter notes that Google has made it difficult to try the model without significant spending.

hackernews · hn-aarvin · Nov 19, 23:35 · [Discussion](https://news.ycombinator.com/item?id=50568130)

**「Background」** Google released Gemini 4 Neon on November 18, 2026, positioning it for complex software engineering, analytical reasoning, and science workflows, adapted from Gemini 4 Carbon. The Models Engineering Index, which the Hacker News post cites, describes itself as measuring language models&\#x27; practical performance on engineering tasks. The community comparisons in the post reference Opus 5.5 and Carbon as prior models users had been running.

**「Practical impact」** For developers weighing a switch, the reported advantage is speed and cost rather than a decisive quality gap: one commenter says Neon &quot;high&quot; ran faster and cheaper than Opus 5.5 &quot;medium&quot; with similar results on long-running language porting in a large monorepo. Access is a practical constraint, since another commenter notes Google has made it hard to try the model without significant spending. These are anecdotal hands-on impressions, not independently measured results.

**「Community Reaction」** Several commenters say Neon is now their preferred model: one calls it equivalent to Opus 5.5/Fable for coding and strong at documentation, and another reports Neon &quot;high&quot; as faster and cheaper than Opus 5.5 &quot;medium&quot; with similar results on long-running language porting in a large monorepo. A third says it is predictable and avoids security refusals that annoyed them with other models. One commenter cautions that earlier posters had not actually used the model, and another points to additional lesser-known benchmarks as supporting evidence.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/">Introducing Gemini 4 Neon</a></li>
<li><a href="https://kie.ai/gemini-4-neon">Gemini 4 Neon API: 1M-Context Gemini 4 Model | Kie.ai</a></li>
<li><a href="https://git-aarvin.github.io/mei/">Models Engineering Index</a></li>

</ul>
</details>

**Tags**: `#LLM benchmarks`, `#AI models`, `#coding assistants`, `#model evaluation`, `#Hacker News`

---

<a id="item-tech-news-7"></a>
### [Anthropic says Claude helped solve two black hole physics problems](https://www.anthropic.com/research/claude-black-hole-physics) ⭐️ 7.0/10

Anthropic published a research post stating that Claude contributed to solving two open problems in black hole physics, and the work was also listed as a bullet point in the company&\#x27;s Fable 5.2 announcement. According to a commenter quoting the post, Anthropic says neither result describes our own universe directly and neither has practical applications, though both contribute to theoretical work on reconciling quantum mechanics and relativity. The post is a vendor account, and the supplied material does not include the underlying papers or the prompts used, so the extent and nature of Claude&\#x27;s contribution cannot be independently assessed from this item alone.

hackernews · cybermango · Nov 19, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50563148)

**「Background」** Anthropic&\#x27;s research post attributes the results to Claude Fable 5.2, describing two black-hole problems tied to the search for a theory of quantum gravity. Secondary coverage reports that one is a Hawking-Page phase-transition calculation left incomplete since 2003 and the other a modular bootstrap bound previously estimated only from numerics, with the work documented through multi-agent runs, Lean checks, and linked preprints. Anthropic&\#x27;s own post states that neither result describes our universe directly and neither has practical applications.

**「Impact」** Because the results are described as having no direct practical application, the immediate consequence is less about physics applications than about how AI-assisted theoretical work is reported and evaluated: readers assessing the claims would need the papers and prompt details, which the supplied material does not provide.

**「Community discussion」** Commenters questioned the framing: dap argued that &quot;Claude solves&quot; anthropomorphizes the model and noted the word &quot;prompt&quot; does not appear in the blog post or either paper, while easterncalculus observed that none of the roughly 80 comments addressed the papers or the article itself. chunky1994, reading the blog post, called the first result a complex error-prone calculation and the second more significant, describing it as an upper limit on black hole mass consistent with a given central charge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-black-hole-physics">Claude solves two open problems in the physics of black holes</a></li>
<li><a href="https://explainx.ai/blog/claude-fable-black-hole-physics-hawking-page-2026">Claude Fable 5.2 Black Hole Physics: Two Open Problems Solved</a></li>

</ul>
</details>

**Tags**: `#AI for science`, `#large language models`, `#theoretical physics`, `#research`, `#attribution`

---

<a id="item-tech-news-8"></a>
### [UK tribunal forces government to admit secret Apple encryption order](https://macanorak.com/uk-government-forced-to-admit-it-issued-apple-a-secret-encryption-order/) ⭐️ 7.0/10

A UK tribunal compelled the government to acknowledge that it served Apple with a secret technical capability notice related to encryption, according to a report on the judgment. The notice&\#x27;s contents remain classified, so its scope and any demands on Apple&\#x27;s products are not publicly known. The report says the media learned of the notice through confidential security briefings rather than a leak. The disclosure establishes that the order exists, not what it requires.

hackernews · Terretta · Nov 19, 16:21 · [Discussion](https://news.ycombinator.com/item?id=50562113)

**「Background」** The notice was issued under section 253 of the Investigatory Powers Act 2016, which lets the Home Secretary give a &quot;relevant operator&quot; a technical capability notice. The Investigatory Powers Tribunal judgment in Apple Inc v Home Secretary, handed down 19 November 2026, addressed the government&\#x27;s refusal to confirm the notice&\#x27;s existence, which had been widely reported for almost two years before the tribunal ended that official silence.

**「Why it matters」** Because the notice&\#x27;s terms are still secret, users and developers cannot verify whether it affects end-to-end encryption guarantees in Apple products sold in the UK. Security practitioners should treat claims about UK-specific encryption protections as unresolved until the order&\#x27;s scope is disclosed or Apple states how it has responded.

**「Community reaction」** Commenters focused on Apple&\#x27;s wording, with one arguing that shifting from &quot;not even Apple can access your data&quot; to &quot;Apple cannot access your data&quot; weakens the assurance, and another pointing to the tribunal judgment as the primary source while noting the notice&\#x27;s contents stay secret. Others said the UK&\#x27;s surveillance posture was already well known and questioned why it is so overt compared with other Western countries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.judiciary.uk/judgments/apple-inc-v-home-secretary-and-others/">Apple Inc -v- Home Secretary and others - Courts and ...</a></li>
<li><a href="https://investigatorypowerstribunal.org.uk/judgement/1-mr-vincent-kearney-2-british-broadcasting-corporation-v-1-chief-constable-of-the-police-service-of-northern-ireland-2-chief-constable-of-durham-constabulary-3-security-service-4-governme/">Apple Inc and Secretary of State for the Home Department and ...</a></li>
<li><a href="https://therecord.media/apple-uk-encryption-notice">UK court confirms British government served Apple with secret ...</a></li>

</ul>
</details>

**Tags**: `#encryption`, `#surveillance`, `#privacy`, `#apple`, `#uk-policy`

---

<a id="item-tech-news-9"></a>
### [European Commission Runs Matrix for Over 40,000 Staff](https://element.io/blog/how-the-european-commission-rolled-out-matrix-to-more-than-40-000-staff/) ⭐️ 7.0/10

Element&\#x27;s blog describes the European Commission&\#x27;s deployment of Matrix to more than 40,000 staff, including operational trade-offs such as disabling live presence because the real-time online/away indicator began affecting performance as users joined. The account is vendor-published by Element, so the deployment details are the vendor&\#x27;s description rather than an independent audit. The post does not, per the available material, establish a timeline or independently measured reliability figures.

hackernews · liotier · Nov 19, 10:58 · [Discussion](https://news.ycombinator.com/item?id=50558533)

**「Background」** Matrix is an open, federated messaging protocol, and Element is the main vendor behind its flagship clients. A recurring concern in the community is the protocol&\#x27;s encryption roadmap: the arewemlsyet.com tracker states that work on bringing MLS \(Messaging Layer Security\) to Matrix is still at an investigation stage, with basic encryption/decryption and membership changes working in demos. That context matters for reading the Commission&\#x27;s deployment, since the source describes operational trade-offs such as disabling live presence under load.

**「Impact」** For public-sector IT teams considering Matrix, the reported decision to switch off live presence under load is a concrete capacity-planning concern: presence features can impose costs that scale with user count and may need to be disabled or redesigned at large deployments.

**「Community Discussion」** Commenters debated encryption maturity, with one calling Matrix&\#x27;s E2EE a &quot;tire fire&quot; and claiming the move to MLS appears abandoned, while another said they hope the Commission&\#x27;s adoption adds development resources despite real problems with client fragmentation, session verification, and encryption errors. Others reported using self-hosted Matrix with Element X among friends for privacy, and one predicted the Commission would migrate away within 12 months.

<details><summary>References</summary>
<ul>
<li><a href="https://arewemlsyet.com/">Are We MLS Yet? | arewemlsyet .com</a></li>

</ul>
</details>

**Tags**: `#matrix`, `#open-source`, `#e2ee`, `#enterprise-deployment`, `#public-sector`

---

<a id="item-tech-news-10"></a>
### [PHP to ship CRITICAL-severity security release](https://www.php.net/archive/2026.php) ⭐️ 7.0/10

PHP&\#x27;s security team announced a security release scheduled for 2026-11-19 between 14:00 and 14:30 UTC, fixing a vulnerability that affects all supported PHP versions and is rated CRITICAL, the highest severity level. The release falls within PHP&\#x27;s regular four-week release cycle. Officials said the CRITICAL-rated issue is only triggered under non-default configurations or uncommon environments, and advised users to upgrade soon after the release goes live. Technical details and the fixed version numbers will be published together with the release, so no CVE identifier or specific affected versions are known yet.

telegram · zaihuapd · Nov 19, 07:10

**「Background」** PHP issues security releases on a regular four-week cadence, and the notice frames this one as part of that cycle rather than an emergency out-of-band fix. Search results describe an earlier PHP security release around October 2026 covering CVE-2026-109618 and CVE-2026-109619, with patched versions 8.5.12, 8.4.27, 8.3.36 and 8.2.35; those results are not confirmed by the source item and the current notice does not state whether the November release is related. The source says the CRITICAL rating applies to a flaw that only triggers under non-default configurations or uncommon environments, and that the CVE and fixed version numbers will be published with the release itself.

**「Impact」** Because the flaw is reported to affect every supported PHP version, operators running PHP in production should plan to apply the patched release promptly once it is published, rather than waiting for the next scheduled maintenance window. The stated non-default or uncommon configuration requirement suggests exposure may be narrower than the CRITICAL rating alone implies, but the affected configurations cannot be confirmed until the advisory and fixed version numbers are released.

<details><summary>References</summary>
<ul>
<li>Php security update for cve-2026-109618 and cve-2026-109619 - Facebook</li>
<li>PHP RCE Vulnerabilities 2026: Patches and Next Steps | Pixel Shield</li>
<li>PHP Critical Security Update - Two (RCE) vulnerabilities : r/blackpointcyber - Reddit</li>

</ul>
</details>

**Tags**: `#php`, `#security`, `#vulnerability`, `#open-source`, `#patching`

---

<a id="item-tech-news-11"></a>
### [Gemini 开始在 Mac 上替用户操作，并支持后台运行和暂停](https://www.bloomberg.com/news/articles/2026-11-19/google-s-gemini-can-now-control-mac-devices-on-users-behalf) ⭐️ 7.0/10

Google Gemini 新增了一项“computer use”功能，可在 Mac 上点击、输入、浏览菜单并填写表单，以替用户完成任务。该功能面向美国地区使用 Mac 版 Gemini 应用、且订阅 Google AI Plus、Pro 或 Ultra 的用户开放。用户可以让 Gemini 在独立的后台窗口中运行，同时继续使用主屏幕和光标；还可以限制它能访问哪些应用、实时查看其操作、随时暂停，并在关键操作前进行审批。该消息来自一份简短的 Telegram 摘要，其中链接到 Bloomberg，未提供独立测试或性能证据。

telegram · zaihuapd · Nov 20, 02:51

**「Background」** Google&\#x27;s announcement, attributed to Gemini group product manager Michael Friedman, describes computer use as running inside an isolated background window with a live preview, so Gemini can work across local files, desktop apps, and the web while the user keeps the main screen and cursor. The feature is initially English-only in the U.S. and requires the Gemini app for Mac plus a Google AI Plus, Pro, or Ultra subscription. The source item does not provide independent performance testing or verification of the safety controls.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-app/computer-use-mac/">Automate Mac tasks with Gemini computer use - The Keyword</a></li>
<li><a href="https://techcrunch.com/2026/11/19/google-gives-gemini-the-ability-to-use-your-mac-for-you/">Google gives Gemini the ability to use your Mac for you</a></li>
<li><a href="https://explainx.ai/blog/gemini-app-mac-computer-use-background-window-ai-plus-pro-ultra-november-2026">Gemini Computer Use on Mac: Who Gets It and How It Works ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Google Gemini`, `#macOS`, `#human-computer interaction`, `#AI safety controls`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Anthropic Shares Open 34% Above IPO Price on Nasdaq Debut](https://www.cls.cn/detail/2539480) ⭐️ 9.0/10

Anthropic began trading on the Nasdaq at $111.5 per share, 34% above its $83 IPO price, implying a market value of about $1.5 trillion, according to a 财联社 report relayed on Telegram. The IPO sold 980 million shares for about $81.34 billion, and Anthropic said it would raise a further $26 billion through a concurrent private placement involving Google, Nvidia, Microsoft, AMD, Broadcom, Micron and TSMC.

telegram · zaihuapd · Nov 19, 16:56

**「Background」** Anthropic had priced its IPO at $83 per share, a level that already implied a valuation of about $1.5 trillion, according to AP and Zacks. Reuters reported the $81.3 billion offering was the largest IPO on record, surpassing SpaceX&\#x27;s listing in June.

**「Impact」** If confirmed, the roughly $107.3 billion combined IPO and private placement would rank among the largest capital raises on record, giving the named chip and cloud investors direct stakes in a leading AI developer and tying their returns to its commercial performance.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/anthropic-ipo-pricing-70b660ddf900d90bbf484ecdf1fb441c">Anthropic reportedly prices its IPO at $83 per share | AP News</a></li>
<li><a href="https://www.zacks.com/featured-articles/761/anthropic-ipo">Anthropic IPO 2026 Guide: Price Predictions, Dates, and ...</a></li>
<li><a href="https://www.reuters.com/live/anthropic-ipo-live-claude-maker-goes-public-nasdaq-after-record-share-offering-2026-11-19/">Anthropic IPO live: Claude maker breaks $2 trillion valuation ...</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#AI`, `#capital markets`, `#Anthropic`, `#private placement`

---

<a id="item-finance-news-2"></a>
### [拼多多三季度营收1083亿元，盘前股价涨逾8%](https://mp.weixin.qq.com/s/vMtfWkFZ0hRTDU54BlD80Q) ⭐️ 7.0/10

拼多多公布截至9月30日的2026年第三季度财报，营收1083亿元、净利润295亿元；财报发布后，其股价盘前上涨逾8.6%。

telegram · zaihuapd · Nov 19, 12:56

**「Background」** The results cover the quarter ended September 30, 2026; Pinduoduo said it continued its &quot;100 billion yuan support&quot; program and supply-chain upgrades while increasing platform-governance spending, according to Chinese media reports on the release.

<details><summary>References</summary>
<ul>
<li><a href="https://original.ifeng.com/c/8yBYMtxN2XD">拼多多2026年第三季度营收1083亿元，净利润295亿元_凤凰网</a></li>
<li><a href="https://finance.sina.com.cn/jjxw/2026-11-19/doc-inizhrsf0889641.shtml">拼多多发布Q3财报：营收1083亿元，净利润295亿元_新浪财经_新浪网</a></li>
<li><a href="https://finance.china.com/TMT/13004688/20261120/49890469.html">拼多多三季度营收1083亿元，净利润295亿元_财经频道_中华网</a></li>

</ul>
</details>

**Tags**: `#拼多多`, `#财报`, `#电商`, `#股价异动`

---

<a id="item-finance-news-3"></a>
### [AI Investment Doubts Weigh on Asian Stocks After Anthropic IPO](https://www.bloomberg.com/news/articles/2026-11-19/stock-market-today-dow-s-p-live-updates) ⭐️ 7.0/10

Asian equities fell broadly, with the MSCI Asia-Pacific index down 1.7% for a seventh consecutive session, as doubts about AI investment intensified after Anthropic&\#x27;s post-IPO drop of more than 5% to below $92. Chip stocks led the declines, including Tokyo Electron \(-7.19%\), Renesas \(-6.71%\), SK Hynix \(-6%\), and Samsung Electronics \(-4.7%\), while South Korea&\#x27;s Kospi fell 3.66%.

telegram · zaihuapd · Nov 20, 01:58

**「Background」** Anthropic listed on Nasdaq on November 19, 2026, pricing shares above its initial $70–$78 range and closing its first trading day up 17% from the IPO price, according to press reports. SoftBank had completed its $64.6 billion investment in OpenAI in early October 2026, a stake of about 13%.

**「Impact」** The selloff directly affects investors holding Asian semiconductor and AI-linked shares, as doubts about whether large AI spending will generate matching returns spread from Anthropic&\#x27;s IPO performance to chipmakers across Japan and South Korea.

<details><summary>References</summary>
<ul>
<li><a href="https://www.euronews.com/2026/11/19/anthropic-shares-open-34-above-ipo-price-in-nasdaq-debut-after-record-listing">Anthropic shares open 34% above IPO price in Nasdaq... | Euronews</a></li>
<li><a href="https://finance.yahoo.com/technology/live/anthropic-ipo-live-anthropic-stock-begins-trading-in-record-81b-raise-with-15t-valuation-192410598.html">Anthropic IPO live: Anthropic stock closes up 17% from initial price...</a></li>
<li><a href="https://trendandticker.com/markets/capital-markets/softbank-openai-final-10-billion-tranche-64-6-billion-stake-shares-fall-october-2-2026">SoftBank OpenAI Stake Hits $64.6 Billion, Shares Drop 6%</a></li>
<li><a href="https://www.ainvest.com/news/softbank-64-6-billion-openai-check-cleared-hard-part-2610/">SoftBank&#x27;s $64.6 Billion OpenAI Check Cleared. Now Comes the ...</a></li>

</ul>
</details>

**Tags**: `#AI investment`, `#Asian equities`, `#semiconductors`, `#market selloff`, `#Anthropic IPO`

---