---
layout: default
title: "Horizon Summary: 2026-09-30 (ZH)"
date: 2026-09-30
lang: zh
---

> 从 54 条内容中筛选出 20 条重要资讯。

---

**科技新闻**
1. [OpenAI DevDay 2026：Dots 智能体等 20 余项更新](#item-tech-news-1) ⭐️ 9.0/10
2. [Anthropic 评估：GLM-5.3 与 Claude 突破二进制利用门槛](#item-tech-news-2) ⭐️ 8.0/10
3. [从 PostgreSQL 视角看 Linux 内核：Andres Freund 谈性能改进](#item-tech-news-3) ⭐️ 8.0/10
4. [从词袋到 JEV：文本分类模型演进图解指南](#item-tech-news-4) ⭐️ 8.0/10
5. [CoWindow 与 MassAlloc 注意力：集体覆盖与自适应计算分配](#item-tech-news-5) ⭐️ 8.0/10
6. [A Privacy Analysis of Web and Mobile Conversational AI Agents \[pdf\]](#item-tech-news-6) ⭐️ 7.0/10
7. [星际之门数据中心延期 甲骨文发不可抗力通知](#item-tech-news-7) ⭐️ 7.0/10
8. [CNNIC 报告：中国生成式 AI 用户破 7 亿](#item-tech-news-8) ⭐️ 7.0/10
9. [Cloudflare 发布面向 AI Agent 的 CLI 工具 cf](#item-tech-news-9) ⭐️ 7.0/10
10. [谷歌修复 Firebase iOS 崩溃问题](#item-tech-news-10) ⭐️ 7.0/10
11. [PS5 Relapse Exploit 瞄准 WebKit JavaScriptCore 漏洞](#item-tech-news-11) ⭐️ 6.0/10
12. [Tcl/Tk 9.1 发布：轻量级脚本语言与 GUI 工具包更新](#item-tech-news-12) ⭐️ 6.0/10
13. [Rust 原生 GPU 目标愿景：无需专用库](#item-tech-news-13) ⭐️ 6.0/10
14. [AI Has Taste 推翻数学论文猜想获原作者确认](#item-tech-news-14) ⭐️ 6.0/10
15. [开源新书：从芯片到智能体的 ML 性能优化指南](#item-tech-news-15) ⭐️ 6.0/10

**财经新闻**
1. [特朗普市政债券持仓或高达 10 亿美元，引发利益冲突关注](#item-finance-news-1) ⭐️ 8.0/10
2. [高盛 CEO 接班面临变数：所罗门迟疑，沃尔德伦等待有限](#item-finance-news-2) ⭐️ 7.0/10
3. [盘前异动：Fair Isaac 跌 18%，AMD 宣布 820 亿美元收购 World Labs](#item-finance-news-3) ⭐️ 7.0/10
4. [中国为人形机器人 IPO 设立三项新标准，多数初创企业或难达标](#item-finance-news-4) ⭐️ 7.0/10
5. [三部门：10 月 1 日起首套房贷获财政贴息，年化 1%最长 5 年](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI DevDay 2026：Dots 智能体等 20 余项更新](https://openai.com/zh-Hant/index/devday-2026-recap/) ⭐️ 9.0/10

OpenAI 于 DevDay 2026 发布 20 余项更新，包括全天候自主运转的伴生智能体 Dots、专精编程与电脑操控的 GPT-6.1 Sol（价格仅为 Astra 的五分之一），以及速度最高提升 8 倍（API 提升 6 倍）的 Astra Ultrafast。同时推出 Codex 云端版（支持语音操控与自动修障）、Agents API（原生电脑操控与 AWS Bedrock 托管）、Decisions API、Sign in with ChatGPT 账户互通，以及算力额度为 Plus 25 倍的 Pro 500 套餐。缓存输入价格降至每百万 token 0.10 美元，较 GPT-6 Sol 的缓存价格再降 50%。

telegram · zaihuapd · 9月29日 17:52

**「背景信息」** 在 DevDay 2026 之前，OpenAI 的 Ultrafast 模式仅限受邀用户使用，预览时基于 GPT-5.6 Sol 可实现每秒 750 tokens、比标准层快 14 倍的推理速度。此次大会正式推出 Astra Ultrafast，速度提升最高达 8 倍（API 6 倍），并将该模式向更多开发者开放。

**「影响」** 缓存输入价格大幅降低 95%（较标准输入）使 Codex 成为对高缓存用量开发者更具成本优势的编码助手，此前 GPT-6 Sol 的质量问题已推动部分用户转向 Anthropic Opus 5.5，GPT-6.1 Sol 能否挽回声誉仍待验证。

**「社区讨论」** 多位用户对比定价与模型质量：有用户认为 DeepSeek 在速度和性价比上均优于 OpenAI，无法 justify 每月 200–500 美元的订阅费；另有评论指出 Sol 6 表现大幅退步，转而使用 Opus 5.5，对 GPT-6.1 持怀疑态度。minimaxir 强调缓存降价 50% 才是本次实质性亮点，gradus\_ad 则担忧价格战对行业的冲击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/">2026-09-27 — OpenAI reportedly expands Ultrafast API access around DevDay</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6.1`, `#Dots agent`, `#AI agent`, `#DevDay`

---

<a id="item-tech-news-2"></a>
### [Anthropic 评估：GLM-5.3 与 Claude 突破二进制利用门槛](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 8.0/10

Anthropic Frontier Red Team 发布评估，称 GLM-5.3 与 Claude Mythos Preview 在内部二进制利用基准测试中分别有 4% 和 6% 的试验成功实现控制流劫持，而之前的 Claude Opus 4.6 与 GLM-5.2 则完全无法达成。这一结果出自 100 个随机选取的测试任务，标志着 AI 模型在自主漏洞利用能力上跨越了有意义的门槛——尽管成功率仍低，但此前该能力完全不存在。

rss · Simon Willison · 9月29日 22:20

**「背景」** 控制流劫持是二进制利用中的核心技术，攻击者通过篡改程序执行流程来劫持控制权。在此之前，前沿语言模型尚未在任何标准二进制利用任务中展示出该能力，因此 Anthropic 的测试结果被视为一项能力阈值突破。

**「影响」** 该发现意味着 AI 已开始具备辅助自动化漏洞利用的实用能力。Anthropic 同时指出，GLM-5.3 的开放权重可被用户修改以绕过安全拒答，且其安全防护在模拟测试中可被简单方法绕过（成功率 64%–100%），可能扩大恶意行为者可用的网络攻击工具范围。安全团队应警惕低门槛自动化利用工具的潜在风险。

**标签**: `#anthropic`, `#AI security`, `#cyber capabilities`, `#LLM capabilities`, `#binary exploitation`

---

<a id="item-tech-news-3"></a>
### [从 PostgreSQL 视角看 Linux 内核：Andres Freund 谈性能改进](https://lwn.net/Articles/1096827/) ⭐️ 8.0/10

LWN 报道，PostgreSQL 主要贡献者 Andres Freund 在 2026 年 Kernel Recipes 会议上，从 PostgreSQL 的角度分享了他如何利用或绕开 Linux 内核特性来提升数据库性能，并讨论了内核未来可如何更好支持此类应用以及 PostgreSQL 领域的一些新进展。

rss · LWN.net · 9月29日 15:42

**「背景」** Andres Freund 是长期致力于提升 PostgreSQL 性能的核心贡献者，其优化工作常需应对或绕开 Linux 内核的特定行为与特性。在 2026 年 Kernel Recipes 会议上，他系统分享了内核与数据库交互的经验，并探讨内核如何更好地支持 PostgreSQL 这类应用。

**「影响」** 对同时关注内核与数据库的开发者而言，这场报告梳理了 PostgreSQL 工作负载与 Linux 内核交互的实际经验，可作为评估数据库性能优化方向以及潜在内核改进思路的参考。

**标签**: `#PostgreSQL`, `#Linux kernel`, `#database performance`, `#kernel development`, `#systems engineering`

---

<a id="item-tech-news-4"></a>
### [从词袋到 JEV：文本分类模型演进图解指南](https://magazine.sebastianraschka.com/p/classifier-history-and-jev) ⭐️ 8.0/10

Sebastian Raschka 于 9 月 29 日发布《Language Models for Text Classification: From Bag-of-Words to Jev》，这是一篇面向文本分类工程师与研究者的可视化指南。文章从词袋模型讲到 JEV，覆盖 RNN、CNN、Transformer 与校准方法，并配有关于准确性和效率的动手实验；内容属于作者的教学性评测，而非产品发布或第三方基准。

rss · Ahead of AI · 9月29日 10:50

**「背景」** Jev 是近期发布的 AI 模型。在 Raschka 约一周前的文章中，他指出长期以来用于分类的编码器式模型多为专用模型、能力有限，而 Jev 的突破在于泛化能力——同一模型可处理邮件分类、玩游戏、交易股票等不同任务。本文则是在此基础上，以图文形式梳理文本分类方法从词袋模型到 Jev 的演进，并配合准确率与效率的动手实验。

**「影响」** 希望选择文本分类架构的读者可直接参考文中实验，对比不同模型在准确性与效率上的表现；但应将这些结果视为作者个人实验，并在自己的数据集和任务上复核后再做技术选型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sebastianraschka.com/blog/2026/jev-classification-generalization.html">Jev and Generalization | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**标签**: `#text classification`, `#language models`, `#machine learning`, `#transformers`, `#tutorial`

---

<a id="item-tech-news-5"></a>
### [CoWindow 与 MassAlloc 注意力：集体覆盖与自适应计算分配](https://www.reddit.com/r/MachineLearning/comments/1wt1gbk/cowindow_and_massalloc_attention_collective/) ⭐️ 8.0/10

CoWindow Attention（CoWA）与 MassAlloc Attention（MALA）是作者提出的两种新注意力机制：CoWA 把远处上下文分散到不同 KV 头、以互补窗口实现全历史覆盖；MALA 保留完整因果 QK 打分，再用 softmax 统计决定是否继续执行后续分块计算。作者报告在 8×H100、TP=8、128K 上下文下，与 FullAttn 相比注意力算子加速：CoWA 前向 7.4×、反向 8.6×、解码 3.0×；MALA 前向 2.2×、反向 3.0×、解码 1.6×。在 14B、32K 上下文继续训练中，总训练 FLOPs 分别下降 28.5% 和 23.1%，报告评估中能力与 FullAttn 相当。需注意这些是注意力算子而非端到端加速，作者也明确表示两种方法都没有证明与密集注意力普遍无损等价。

reddit · r/MachineLearning · /u/BitExternal4608 · 9月29日 05:16

**「背景」** 标准因果注意力在每个位置都要对所有历史键做打分，长上下文时计算量随序列二次增长；许多稀疏注意力方法因此只保留局部、前缀或滑动窗口。CoWA 与 MALA 属于这类减少冗余计算的探索，但分别从“集体覆盖的位置模式”和“按 softmax 统计自适应分配后计算”两条路径切入。

**「影响」** 对长上下文内核开发者而言，若注意力分布常有低贡献分块，MALA 的自适应跳过可能更合用，但仍需承担完整因果 QK 打分；若希望使用不依赖学习路由的固定稀疏覆盖，CoWA 的位置定义模式更易移植。采用前应在目标负载上独立复现算子级加速，再评估端到端收益。

**标签**: `#attention mechanisms`, `#long-context`, `#efficiency`, `#transformer`, `#sparse attention`

---

<a id="item-tech-news-6"></a>
### [A Privacy Analysis of Web and Mobile Conversational AI Agents \[pdf\]](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A privacy analysis of conversational AI agents highlights emerging data-exposure and tracking risks across web and mobile chat platforms.

hackernews · damaru2 · 9月29日 09:03 · [社区讨论](https://news.ycombinator.com/item?id=49890226)

**标签**: `#privacy`, `#conversational AI`, `#security`, `#tracking`, `#AI agents`

---

<a id="item-tech-news-7"></a>
### [星际之门数据中心延期 甲骨文发不可抗力通知](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

甲骨文已就星际之门在新墨西哥州的 Project Jupiter 数据中心向项目开发方发出不可抗力通知，计划在因外部因素导致延期时推迟部分付款。该项目配套 2.45GW 微电网的环境与供电审批尚未落地，2028 年投运面临延期风险。市场由此担忧超大型 AI 数据中心建设进度，相关 180 亿美元银团贷款已出现折价交易；星际之门多数项目仍处土建、审批和能源配套阶段，得州也已暂停新数据中心项目审批。

telegram · zaihuapd · 9月29日 05:46

**「背景」** 不可抗力条款允许合同方在外部不可控事件导致履约困难时暂缓义务。据报道，Oracle 于 2026 年 9 月 24 日通知开发商 Stack Infrastructure，若天然气管道审批拖延导致新墨西哥州 Project Jupiter 2.45GW 园区无法在 2028 年前供电，可能推迟支付租金；该项目是 Stargate AI 基础设施计划的关键部分。此前融资环境已趋紧：9 月 28 日的 Horizon 摘要提到美债收益率升至 2007 年以来最高，10 年期约 5.17%，推高 AI 数据中心融资成本，JPMorgan 估算到 2030 年将有 4.1 万亿美元 AI 相关债务发行。

**「影响」** 对参与星际之门的贷款方和承建方而言，电力审批与微电网配套的不确定性已直接反映在融资成本上：180 亿美元银团贷款出现折价交易，得州暂停新数据中心审批也会抬高后续项目的获取成本和排期风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/27/debt-hungry-data-center-companies-increased-risk-bond-yields-spike.html">2026-09-28 — Treasury Yield Spike Raises Costs for AI Data-Center Buildout</a></li>
<li><a href="https://coloprice.com/guides/oracle-force-majeure-project-jupiter/">Oracle Invokes Force Majeure on Stargate&#x27;s Project Jupiter as…</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#Oracle`, `#energy grid`, `#Stargate`

---

<a id="item-tech-news-8"></a>
### [CNNIC 报告：中国生成式 AI 用户破 7 亿](https://ysxw.cctv.cn/article.html?toc_style_id=feeds_default&amp;amp;item_id=187569887152346976&amp;amp;channelId=1119) ⭐️ 7.0/10

9 月 29 日，中国互联网络信息中心（CNNIC）发布《生成式人工智能应用发展报告（2026）》。报告称，截至 2026 年上半年，中国生成式人工智能用户规模突破 7 亿人，普及率超过 50.0%；智能问答是最主要应用场景，76.0%的用户用它回答问题，AI 综合助手和 AI 效率办公的使用次数同比均增长超 100%。同期，中国智能算力规模达 2185 EFLOPS，同比增长 177%。这些数字来自官方统计报告，尚非独立第三方测量结果。

telegram · zaihuapd · 9月29日 06:39

**「背景」** 生成式人工智能（Generative AI）能够根据用户输入生成文本、图像等内容，其应用在中国迅速普及。中国互联网络信息中心（CNNIC）定期发布《生成式人工智能应用发展报告》，此次报告是衡量该技术在中国应用规模的重要官方统计。

**「影响」** 对应用开发者而言，报告中的数据提供了场景优先级依据：智能问答已是最大场景，AI 综合助手与效率办公增速最快，均可视为已获大规模用户验证的方向。报告未披露用户构成、付费或留存数据，因此不宜据此推断具体商业表现。

**标签**: `#generative AI`, `#China`, `#AI adoption`, `#user statistics`, `#intelligent computing`

---

<a id="item-tech-news-9"></a>
### [Cloudflare 发布面向 AI Agent 的 CLI 工具 cf](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare 发布了 cf CLI 开放测试版，开发者和 AI Agent 可以通过命令行调用其 API。该工具由 API Schema 生成，覆盖超过 3,000 项 API 操作，并以 JSON 作为默认输出，支持命令搜索和引导；对比之下，现有 Wrangler 覆盖约 280 种操作。Cloudflare 举例说，Agent 可以用同一工具创建和部署 Worker、监控服务、配置 Access 与 WAF，甚至购买域名。

telegram · zaihuapd · 9月29日 13:46

**「背景」** Cloudflare 此前提供的 Wrangler CLI 主要面向 Workers 开发，覆盖约 280 种 API 操作；新的 cf CLI 在覆盖范围上大幅扩展到了超过 3,000 项操作。

**「影响」** 对开发者和 AI Agent 构建者而言，cf 提供了一个统一的命令行入口，能够以结构化 JSON 输出完成从部署到配置的多种 Cloudflare 操作。由于仍处开放测试版，用户在生产环境采用前应验证命令行为与输出格式是否稳定。

**标签**: `#Cloudflare`, `#CLI`, `#AI Agents`, `#DevTools`, `#API`

---

<a id="item-tech-news-10"></a>
### [谷歌修复 Firebase iOS 崩溃问题](https://github.com/firebase/firebase-ios-sdk/issues/16728) ⭐️ 7.0/10

谷歌确认，Google Analytics for Firebase 的 iOS 服务端曾返回格式错误数据，导致大量集成该组件的 iOS 应用启动时崩溃。问题始于 2026 年 9 月 28 日 17:41（美国太平洋夏令时），修复于 19:52 完成推出。谷歌表示无需更新 SDK 或应用；受缓存影响，部分应用最长可能在修复后继续崩溃约 4 小时，残余问题将自行消退。

telegram · zaihuapd · 9月29日 16:29

**「背景」** Google Analytics for Firebase 是 Firebase 在 iOS 上的分析组件，应用启动时会请求并解析服务端返回的数据。此次事故中该服务端返回了格式错误的数据，客户端解析逻辑无法容错，导致集成该组件的应用在启动阶段崩溃；由于根因在服务端而非 SDK 代码，修复后开发者无需更新 SDK 或重新发布应用。

**「影响」** 受影响的 iOS 开发者无需更新 SDK 或应用，但需注意修复后因缓存导致的 4 小时残存崩溃窗口，无需额外操作即可自动恢复。

**标签**: `#Firebase`, `#iOS`, `#crash`, `#Google Analytics`, `#bug fix`

---

<a id="item-tech-news-11"></a>
### [PS5 Relapse Exploit 瞄准 WebKit JavaScriptCore 漏洞](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 6.0/10

GitHub 上出现了一个名为 Relapse Exploit 的 PS5 越狱利用项目，并在 Hacker News 引发讨论；该项目针对 PS5 的 WebKit JavaScriptCore 引擎漏洞。目前公开信息只表明这是一次早期披露，尚没有漏洞细节或独立验证能证明该利用已经稳定可用。对关注主机安全和越狱的用户来说，这更像是研究进展，而非可直接部署的越狱工具。

hackernews · therepanic · 9月29日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=49895304)

**「背景」** Relapse 是针对 PS5 固件 7.00 至 13.60 的越狱漏洞链，利用 WebKit 的 JavaScriptCore 漏洞来突破浏览器沙盒，随后通过内核漏洞获取完整系统权限。该漏洞链需要多次尝试才能稳定执行，浏览器页面可能卡死，内核漏洞也可能导致主机死机。

**「社区讨论」** 评论者 MaxBarraclough 指出该利用看起来针对 WebKit 的 JavaScriptCore JavaScript 引擎，并怀疑 PS5 上是否启用 JIT，以及索尼是否会通过禁用 JIT 收窄攻击面；Muromec 则认为相关社区往往握有一批零日漏洞储备。另有用户感叹，用户需要破解自己合法拥有的硬件才能获得完全控制并不合理——这些均为讨论中的观点，而非已证实结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/ Relapse - Exploit : Exploit chain for PS 5 7.00 - 13.60</a></li>
<li><a href="https://www.superpsx.com/ps5-relapse-jailbreak-13-60-and-lower-complete-guide/">PS 5 Relapse Jailbreak 13.60 and Lower – Complete Guide</a></li>

</ul>
</details>

**标签**: `#security`, `#exploit`, `#PS5`, `#WebKit`, `#jailbreak`

---

<a id="item-tech-news-12"></a>
### [Tcl/Tk 9.1 发布：轻量级脚本语言与 GUI 工具包更新](https://www.tcl-lang.org/software/tcltk/9.1.html) ⭐️ 6.0/10

Tcl/Tk 9.1 于 2026 年 9 月 29 日正式发布，是 9.x 系列的增量版本，面向使用这一长寿命脚本语言和 GUI 工具包的开发者与爱好者。官方发布公告指出该版本延续了 Tk 的简易 GUI 开发传统，并提供了持续的现代平台支持。用户可从 tcl-lang.org 获取源代码和二进制包。

hackernews · dmux · 9月29日 17:13 · [社区讨论](https://news.ycombinator.com/item?id=49896712)

**「背景」** Tcl/Tk 9.0 是此前的稳定版本线，而 9.1 是在其基础上继续开发的新版本。官方页面将 Tcl/Tk 9.1.0 描述为在 9.0 基础上增加新特性与接口的当前开发成果，目标是在 2026 年 9 月发布稳定版；Tcl 9.1a1 的发布说明也已列出相对 9.0 的主要变化，包括面向 Tcl 库用户和脚本编写者的新命令与选项。

**「社区讨论」** 在 Hacker News 评论中，多位用户称赞 Tcl/Tk 9.1 保持了其简单易用的 GUI 开发体验，例如用户 trebligdivad 称其为“最简单的 GUI 系统”，认为上手几乎无需费力。同时，也有用户（如 srean）指出 Tcl 语言的字符串元编程和 upvar/uplevel 等特性虽然有趣，但需谨慎用于专业项目，另一位用户 neilv 则回顾了 Tk 在早期 Unix/X Window 时代作为 GUI 简易方案的历史地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tcl-lang.org/software/tcltk/9.1.html?ref=upstract.com">Tcl / Tk 9 . 1</a></li>
<li><a href="https://comp.lang.tcl.narkive.com/KwC5CCg9/tcl-9-1a1-released">Tcl 9 . 1 a 1 RELEASED</a></li>

</ul>
</details>

**标签**: `#Tcl/Tk`, `#release`, `#GUI toolkit`, `#scripting language`, `#programming languages`

---

<a id="item-tech-news-13"></a>
### [Rust 原生 GPU 目标愿景：无需专用库](https://lwn.net/Articles/1095731/) ⭐️ 6.0/10

在 RustConf 2026 上，rust-gpu 与 Rust CUDA 的维护者 Christian Legnitto 阐述了他的愿景：让 GPU 成为普通 Rust 代码的标准编译器目标，无需专用库或新的生态支持。他同时表示已有一个准备发布的原型，但该愿景尚未完全实现，演讲内容仍属于计划与方向，而非已落地的完整能力。

rss · LWN.net · 9月29日 17:57

**「背景」** 目前从 Rust 编写 GPU 程序主要依赖 rust-gpu 和 Rust CUDA 这类专门库，它们负责把 Rust 代码与 GPU 硬件或相关运行时衔接起来。RustConf 2026 上的这场演讲提出的愿景是，把这种支持直接下沉到编译器层面，让 GPU 像 CPU 一样成为普通 Rust 代码的标准编译目标，从而不再需要这些专门库或额外的生态支持。

**「影响」** 对于目前依赖 rust-gpu 或 Rust CUDA 编写 GPU 代码的开发者，这一方向意味着未来可能可以脱离这些专用库，直接用普通 Rust 代码面向 GPU 编译。但原型尚未发布，现阶段仍应以现有库和生态作为实际开发选择。

**标签**: `#Rust`, `#GPU`, `#compilers`, `#programming languages`, `#open source`

---

<a id="item-tech-news-14"></a>
### [AI Has Taste 推翻数学论文猜想获原作者确认](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+AI%E6%89%BE%E5%87%BA%E6%95%B0%E5%AD%A6%E5%8F%8D%E4%BE%8B%E6%8E%A8%E7%BF%BB%E8%AE%BA%E6%96%87%EF%BC%8C%E4%BD%9C%E8%80%85%E7%A1%AE%E8%AE%A4%EF%BC%81453%E7%AF%87%E6%89%8B%E7%A8%BF%EF%BC%8CAI%E5%BC%80%E5%A7%8B%E8%87%AA%E5%B7%B1%E5%87%BA%E9%A2%98%E4%BA%86) ⭐️ 6.0/10

思特雅大学研究员曾仔健开发的 AI Has Taste 系统，在输入一篇数学论文的猜想后，自动构造出反例并推翻该猜想，经原作者回信确认反例成立。该项目并非专注于证明定理，而是将 AI 的角色从“生成答案”转向“生成研究议程”，目前公开仓库已收录 453 份数学研究手稿，其中 6 篇被归类为 AI 提出的猜想。

rss · 新智元 · 9月29日 03:40

**「背景」** 以往 AI 数学研究的重点，是让模型求解已知难题或写出严谨证明，本质上仍是“从已知问题生成答案”。AI Has Taste 项目的意图是从“答案生成”走向“研究议程生成”：让 AI 不仅证明或推翻具体猜想，还负责选题、反例搜索、失败管理和提出可证伪的新猜想。项目负责人曾仔健称，转折点来自一次测试——AI 没有顺着论文“证明”猜想，而是构造出反例，经写信向原论文作者核实后，对方回信确认该反例成立。

**「影响」** 对数学研究者和论文审稿人而言，AI Has Taste 提供了一个可操作的反例筛查方式：在依赖或发表公开猜想前，可用类似系统搜索可能推翻猜想的反例。本例中，原论文作者已经确认 AI 构造的反例成立，说明这类验证流程可能发现人类审稿阶段遗漏的错误命题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conjecture">Conjecture - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI for Mathematics`, `#Automated Theorem Proving`, `#Counterexample Search`, `#AI Research`, `#Research Integrity`

---

<a id="item-tech-news-15"></a>
### [开源新书：从芯片到智能体的 ML 性能优化指南](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 6.0/10

作者发布了免费开源的《How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents》，面向 ML 性能工程从业者，覆盖从硬件/roofline 分析、内核、编译器、量化、剪枝，到推理服务与智能体的系统级优化内容。该书的核心主张是，降低 FLOPs 并不等于让模型更快，应先判断系统受限于计算、带宽、内存还是系统，再选择真正有效的优化手段。目前这是作者自述的成果，尚无外部验证；全书内容与开源仓库托管在 GitHub，作者欢迎 ML 系统、推理、编译器、边缘 AI 和性能工程从业者反馈与贡献。

reddit · r/MachineLearning · /u/SoloTiger\_ · 9月29日 10:35

**「背景」** 机器学习模型的实际运行速度并非仅由浮点运算次数（FLOPs）决定，内存带宽、系统开销和硬件特性往往成为真正的瓶颈。这本书的出发点正是填补这一认知鸿沟，帮助开发者理解如何系统性地分析模型与硬件之间的性能边界。

**「影响」** 关注 ML 性能工程的开发者现在可以直接免费获取该书的第一版（v1.0），并可在 GitHub 上阅读、下载或参与贡献；对希望从硬件原理、内核优化、量化与剪枝一路学到 serving 和 agent 系统的自学者而言，这提供了一条无需付费课程即可从入门走向实战的完整路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/usamahz/make-your-model-fast/releases/tag/v1.0">Release How to Make Your Model Fast, first edition · usamahz/make-your-model-fast</a></li>

</ul>
</details>

**标签**: `#ML performance`, `#Systems optimization`, `#Open source`, `#LLM inference`, `#Hardware`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [特朗普市政债券持仓或高达 10 亿美元，引发利益冲突关注](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 8.0/10

据 CNBC 对其财务披露的分析，特朗普的市政债券持仓超过 1000 笔、总值在 3 亿至 10 亿美元之间，其中包括 2026 年已披露的至少 243 笔购买（约 6820 万美元至 2.338 亿美元）；CNBC 未发现其利用政策信息交易的证据。

rss · CNBC Finance · 9月29日 14:37

**「背景」** CNBC 对特朗普财务披露的分析显示，截至 2026 年 9 月，特朗普的市政债券（地方政府和公共机构发行的债务）持仓已增至 1000 多笔、总额约 3 亿至 10 亿美元，其中许多债券来自受其政府政策影响的市政府、医院和公用事业机构；CNBC 称未发现他利用内部信息交易或直接指挥具体交易的证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html">Trump municipal bond portfolio valued at up to $ 1 billion</a></li>
<li><a href="https://qz.com/trump-municipal-bond-portfolio-billion-conflict-interest-092926">Trump municipal bond portfolio approaching $ 1 billion</a></li>

</ul>
</details>

**标签**: `#Municipal Bonds`, `#Trump Administration`, `#Conflict of Interest`, `#Financial Disclosures`, `#Ethics`

---

<a id="item-finance-news-2"></a>
### [高盛 CEO 接班面临变数：所罗门迟疑，沃尔德伦等待有限](https://www.cnbc.com/2026/09/29/goldman-sachs-ceo-succession-planning.html) ⭐️ 7.0/10

据《华尔街日报》报道，高盛董事会正讨论最快明年将 CEO 戴维·所罗门转为执行主席、由总裁约翰·沃尔德伦接任的交接计划，并可能在数月内表决；但所罗门或不愿让位，沃尔德伦也可能不愿无限期等待，接班仍存不确定性。

rss · CNBC Finance · 9月29日 20:50

**「背景」** 高盛是全球最大的纯投资银行，所罗门 2018 年出任 CEO 以来股价上涨逾 300%，在 KBW 银行指数中仅次摩根大通 CEO 戴蒙。沃尔德伦此前据报曾与 Apollo 和 Carlyle 讨论高管职位，高盛已给予其 8000 万美元留任方案，有效期至 2030 年。

**「影响」** 接班若拖延或落空，可能影响高盛管理层稳定和股东对公司治理的评估；所罗门作为董事长对董事会有较大影响力，而财力雄厚的竞争对手仍可能尝试挖走沃尔德伦。

**标签**: `#Goldman Sachs`, `#CEO succession`, `#corporate governance`, `#David Solomon`, `#John Waldron`

---

<a id="item-finance-news-3"></a>
### [盘前异动：Fair Isaac 跌 18%，AMD 宣布 820 亿美元收购 World Labs](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

9 月 29 日盘前，多只个股因重磅消息大幅波动：Fair Isaac 跌约 18%，因美国联邦住房金融局（FHFA）调整房贷定价规则；AMD 宣布以 82 亿美元收购 AI 公司 World Labs 后涨逾 1%；Summit Therapeutics 因获阿斯利康 20 亿美元投资涨约 18%；CarMax 因第二季度每股收益 1.16 美元、远超分析师预期的 0.73 美元而上涨逾 6%。

rss · CNBC Finance · 9月29日 12:03

**「背景」** FHFA 是房利美和房地美的监管机构；新政策把两套独立房贷定价网格合并为一套，并让 VantageScore（另一种信用评分）加入现有的 FICO Classic 定价网格。

**标签**: `#stock movers`, `#FHFA mortgage pricing`, `#M&amp;A`, `#earnings`, `#biotech financing`

---

<a id="item-finance-news-4"></a>
### [中国为人形机器人 IPO 设立三项新标准，多数初创企业或难达标](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据知情人士透露，中国证监会为人形机器人公司上市设置了三项门槛：须有可持续收入和商业订单、亏损收窄并提供三年预测、掌握机器人“大脑”或“手”等核心技术；消息人士预计，目前至少 24 家申请赴港上市的相关公司中，可能只有少数甚至没有一家能达标。

rss · CNBC Finance · 9月29日 07:19

**「背景」** 人形机器人属于中国推动的“具身智能”领域，行业投资今年第二季度达 470.9 亿元人民币，同比增逾六倍；行业标杆宇树科技 8 月上市后股价已较首日收盘价大幅回落。

**「影响」** 新标准可能使尚未稳定盈利的数十家人形机器人初创企业更难公开上市，依赖 IPO 退出的早期投资者也将面临更大不确定性。

**标签**: `#China regulatory policy`, `#humanoid robots`, `#IPO criteria`, `#embodied AI`, `#CSRC`

---

<a id="item-finance-news-5"></a>
### [三部门：10 月 1 日起首套房贷获财政贴息，年化 1%最长 5 年](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 7.0/10

中国财政部、中国人民银行、金融监管总局 9 月 29 日联合宣布，自 2026 年 10 月 1 日起对符合条件的首套住房商业贷款实施财政贴息，贴息标准为年化 1 个百分点，期限最长 5 年，单户贷款本金上限 100 万元，据此计算单户每年最高可获约 1 万元贴息。

telegram · zaihuapd · 9月29日 10:18

**「背景」** 此次贴息适用于新发放的首套房贷（不含存量贷款置换），所购住房面积须在 120 平方米以下、总价 150 万元以下，旨在直接减轻首次购房家庭的利息负担。

**标签**: `#住房贷款`, `#财政贴息`, `#房地产政策`, `#首套住房`, `#宏观政策`

---