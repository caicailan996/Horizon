---
layout: default
title: "Horizon Summary: 2026-10-03 (ZH)"
date: 2026-10-03
lang: zh
---

> 从 47 条内容中筛选出 18 条重要资讯。

---

**科技新闻**
1. [AI 新算法击败 Stratego 人类顶级选手](#item-tech-news-1) ⭐️ 8.0/10
2. [Zig v0.17.0 发布：聚焦构建集成与工具链](#item-tech-news-2) ⭐️ 8.0/10
3. [Greg Kroah-Hartman 剖析 LLM 在内核漏洞报告中的真实价值](#item-tech-news-3) ⭐️ 8.0/10
4. [RustConf 2026：智能指针灵活性讨论](#item-tech-news-4) ⭐️ 8.0/10
5. [arXiv 新规：每位提交者每月最多两篇论文](#item-tech-news-5) ⭐️ 8.0/10
6. [Google 发布 Cogentic：多智能体自动发现数学证明](#item-tech-news-6) ⭐️ 8.0/10
7. [Claude Code 新增 mods 插件系统，支持 TypeScript 自定义](#item-tech-news-7) ⭐️ 8.0/10
8. [Anthropic 提议澳大利亚采用“退出”机制训练 AI 遭广播公司反对](#item-tech-news-8) ⭐️ 7.0/10
9. [SGLang v0.5.21 发布：新增多模型支持与 Rust 前缀缓存](#item-tech-news-9) ⭐️ 6.0/10
10. [苹果发布官方网页版 Pass Designer 工具](#item-tech-news-10) ⭐️ 6.0/10
11. [FLEET：给 Best-of-N 搜索加记忆而非盲采样](#item-tech-news-11) ⭐️ 6.0/10
12. [Sub2API 计费绕过漏洞已修复，请升级 0.2.13](#item-tech-news-12) ⭐️ 6.0/10

**科技博客**
1. [超级说服力将表现为贿赂](#item-tech-blog-1) ⭐️ 6.0/10

**财经新闻**
1. [疲软就业报告压低 10 月美联储加息概率](#item-finance-news-1) ⭐️ 8.0/10
2. [Bitget CEO：对 3.88 亿美元黑客事件追回资金不抱太大期望](#item-finance-news-2) ⭐️ 8.0/10
3. [美股午盘异动：特斯拉交付超预期、耐克营收不及预期、博通拟向 Anthropic 提供巨额贷款](#item-finance-news-3) ⭐️ 7.0/10
4. [盘前异动：Nike 财报不及预期、ON Semi 拟收购 Synaptics、硬盘股受扩产消息拖累](#item-finance-news-4) ⭐️ 7.0/10
5. [AI 需求重塑华尔街岗位：招聘增 49%，智能体编排技能涨 1,721%](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [AI 新算法击败 Stratego 人类顶级选手](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

一项新近报道的研究称，AI 算法已击败历史上最强的 Stratego 人类玩家；Stratego 的不完美信息特性——棋子位置与军衔相互隐藏——此前长期让 AI 难以搜索局面。研究提供了 Nature 论文（s41586-026-11036-y）和 arXiv 预印本（2511.07312）作为具体证据，并宣称采用高效算法，学习所需对局数远少于此前的 DeepNash。截至报道时，这些仍是研究团队或论文的宣称，尚未看到独立的复现验证。

hackernews · PaulHoule · 10月2日 14:11 · [社区讨论](https://news.ycombinator.com/item?id=49933740)

**「背景」** Stratego 是一款典型的不完全信息双人棋类游戏：玩家看不到对方棋子的实际类型，因此每个行动的价值都取决于无法直接观察的信息，这让传统的搜索与强化学习方法难以稳定估计胜率。此前 DeepMind 在 2022 年提出的 DeepNash 使用无模型多智能体强化学习，被视为在该游戏上的重大突破；而这次被报道的新研究则称，其算法以远少于 DeepNash 的对局数和更低成本达到了超过人类顶级选手的水平。

**「社区讨论」** 评论中 janalsncm 指出，隐藏信息让前向搜索无法直接使用，因为某一步的好坏取决于无法观察到的对手局面，因此样本效率才是关键；smokel 则认为 2022 年 DeepNash 自称“掌握”Stratego 的结论如今看来为时过早。其他评论多回忆儿时游戏经历，未提供更多可验证的细节。

**标签**: `#game AI`, `#reinforcement learning`, `#imperfect information`, `#research`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Zig v0.17.0 发布：聚焦构建集成与工具链](https://ziglang.org/download/0.17.0/release-notes.html) ⭐️ 8.0/10

Zig v0.17.0 的发布说明已公开，分析认为该版本在构建集成和工具链方面有显著进展，是语言发展中的一个重要版本。它面向系统程序员和语言爱好者，但具体的功能细节、兼容性变化与使用条件仍需以官方 release notes 原文为准。

hackernews · ErenayDev · 10月2日 20:56 · [社区讨论](https://news.ycombinator.com/item?id=49938521)

**「背景」** Zig v0.17.0 是这套仍在 1.0 之前、以 0.x 版本不断演进的语言的又一次版本发布，因此构建集成和工具链的变化是用户关注的重点。在异步 I/O 方面，Zig 生态中已有 zig-aio 这类提供 io\_uring 风格异步 API 和协程式 IO 任务的项目，为社区期待的新协程 IO 实现提供了参照。

**「影响」** 对 Zig 0.16 用户来说，升级到 0.17.0 需要核对语言、标准库和 build.zig 的破坏性变更，相关迁移说明已随发布文档提供。新版本的构建集成会直接影响依赖 Zig 构建系统的工具链发展；社区还在期待后续的 stackless coroutine IO 和 fuzzer 工具，但当前版本仍不稳定、生态较小，是否迁移需结合项目情况权衡。

**「社区讨论」** 评论者 ubavic 称，在 Zig 上工作一年后认为它是“为人类设计得最好的语言之一”，但也不否认其目前仍不稳定、生态较小。audunw 提到项目负责人 Andrew Kelley 正对用 LLM 发现 bug 持开放态度（受 SQLite 结果启发），这与 jabedude 记忆中“Zig 曾对 AI 持强硬立场”的疑问形成对照；另有开发者期待后续的协程 IO、io\_uring 进展和 fuzzer 工具。以上均为评论者个人观点，并非发布说明中的既定事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Cloudef/zig-aio">Cloudef/ zig -aio: io _ uring like asynchronous API and coroutine ...</a></li>
<li><a href="https://ziggit.dev/t/zig-aio-lightweight-abstraction-over-io-uring-and-coroutines/4767">Zig -aio: lightweight abstraction over io _ uring and coroutines ... - Ziggit</a></li>
<li><a href="https://ziglang.org/download/0.17.0/release-notes.html">0.17.0 Release Notes ⚡ The Zig Programming Language</a></li>
<li><a href="https://www.ziglang.in/learn/getting-started/zig-0-17/">Zig 0.17: What Changed Since 0.16, With Working Code · Zig ...</a></li>

</ul>
</details>

**标签**: `#zig`, `#systems-programming`, `#release-notes`, `#programming-languages`, `#tooling`

---

<a id="item-tech-news-3"></a>
### [Greg Kroah-Hartman 剖析 LLM 在内核漏洞报告中的真实价值](https://www.youtube.com/watch?v=NnV_cWeoo5Q) ⭐️ 8.0/10

在 Kernel Recipes 2026 演讲中，Linux 内核维护者 Greg Kroah-Hartman 公开拆解了 Anthropic 的 Mythos 模型此前宣称发现的 79 个内核漏洞：其中 24 个无任何细节，14 个并非漏洞，3 个数据完全虚构，15 个已在最新版本中被其他贡献者修复（Anthropic 仅修复其中 4 个），真正需要修复的 20 个中又有 7 个依赖“假设恶意文件系统镜像”、2 个依赖“假设你能注入……”。Greg 估算所有必要修复仅相当于一名内核开发者一小时的正常工作量，并批评 Anthropic 未正确归因原始修复者。

hackernews · usernomdeguerre · 10月2日 02:51 · [社区讨论](https://news.ycombinator.com/item?id=49929391)

**「背景」** 近年来，多家 AI 公司（如 OpenAI、Anthropic）声称其大语言模型能自主发现软件安全漏洞，并以此作为模型能力与安全风险的宣传点。Mythos 是 Anthropic 推出的模型，此前其团队高调宣布在 Linux 内核中找到 79 个 CVE，引发业界对 AI 辅助漏洞研究的广泛讨论。

**「影响」** Greg 的演讲意味着，基于 LLM 的漏洞发现工具当前产生的报告需要人工逐一验证，且大多数为噪音或已修复缺陷。依赖此类报告评估模型安全性的组织应将实际修复工作量——仅一小时而非 79 个 CVE——作为更可靠的指标，而非原始报告数量。

**「社区讨论」** Hacker News 评论指出，Mythos 实际仅通过模式匹配历史补丁来发现未修补位置，而非独立发现新漏洞；Anthropic 在宣传时未引用原始内核开发者的工作，与 OpenAI 此前因归因问题所受的批评如出一辙。

**标签**: `#linux-kernel`, `#llm-security`, `#vulnerability-research`, `#AI`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [RustConf 2026：智能指针灵活性讨论](https://lwn.net/Articles/1096028/) ⭐️ 8.0/10

在 RustConf 2026 上，Rust 语言团队负责人 Tyler Mandry 介绍了让用户自定义智能指针拥有与内置引用同等灵活性的长期努力。目前，部分可对内置引用执行的操作仍无法用于用户自定义智能指针；这场演讲属于设计讨论，尚未宣布或交付具体的语言变更。

rss · LWN.net · 10月2日 15:11

**「背景」** 在 Rust 中，像 &amp;T 这样的内置引用由语言本身直接支持，而 Box、Rc 以及用户自定义的智能指针则是普通类型，因此语言层面一些专门为内置引用保留的能力，很难被用户自定义智能指针完整复刻。Tyler Mandry 作为 Rust 语言团队负责人，在 RustConf 2026 上介绍的正是这项长期努力：让用户自定义的智能指针获得与内置引用同等的灵活性。

**标签**: `#Rust`, `#smart pointers`, `#language design`, `#programming languages`

---

<a id="item-tech-news-5"></a>
### [arXiv 新规：每位提交者每月最多两篇论文](https://www.reddit.com/r/MachineLearning/comments/1wvg7yc/arxiv_now_limits_submitters_to_up_to_two/) ⭐️ 8.0/10

arXiv 自 10 月 1 日起实施新规，每位提交者每个自然月最多提交 2 篇论文，覆盖计算机、数学、物理等全部学科；被拒稿件同样占用当月额度，多作者论文只计算实际提交者，其余合著者不受影响。arXiv 称 9 月投稿达 40363 篇、创 35 年新高，其中 AI 分类论文两年增长超 6 倍，大量低质量 AI 生成论文挤占了人工审核资源。

reddit · r/MachineLearning · /u/Nunki08 · 10月2日 00:47

**「背景」** arXiv 是全球最大的预印本平台，其审稿工作依赖志愿版主。2026 年 9 月平台收到 40363 篇投稿，创下 35 年新高，而 10 年前同月约仅 9869 篇、两年前约 20569 篇；其中 AI 分类论文两年增长超过 6 倍，大量低质量、疑似 AI 生成的投稿挤占了人工审核资源。官方称每月 2 篇的限额是对投稿量激增和版主负荷的临时应对措施，而非长期规则。

**「影响」** 对月度产出超过两篇的研究者，该额度会直接影响预印本发布流程；被拒稿件也占用额度，因此反复提交或快速迭代的手稿可能更快耗尽配额。多作者论文只计算实际提交者，团队可考虑由不同合著者分别承担提交任务，以缓解每月限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/">arXiv has updated its rate limit policy for all submitters .</a></li>
<li><a href="https://rottenpanda.com/tech-digital-safety/arxiv-s-updated-rate-limit-policy/">ArXiv &#x27;s Updated Rate Limit Policy - RottenPanda</a></li>
<li><a href="https://www.theregister.com/ai-and-ml/2026/10/02/arxiv-imposes-rate-limit-on-paper-submissions-to-stem-the-ai-slop-tide/5300899">ArXiv imposes rate limit on paper submissions to stem the AI slop tide</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#preprints`, `#academic publishing`, `#research policy`, `#machine learning`

---

<a id="item-tech-news-6"></a>
### [Google 发布 Cogentic：多智能体自动发现数学证明](https://arxiv.org/abs/2609.40324v1) ⭐️ 8.0/10

Google Research 在 arXiv（2609.40324v1）发布论文，提出 Cogentic 多智能体系统：多个独立证明器并行探索不同方向，配合对抗式验证组件与可持续使用的验证账本，通过“证明—验证”循环自动发现数学证明。系统以 Gemini 为基础模型，已在在线学习、拍卖理论和机制设计领域的 5 个开放问题上产出新结果，并由领域专家独立验证，配套论文中展开了具体结论。目前公开的是论文成果，尚需社区更广泛的复现与验证。

telegram · zaihuapd · 10月2日 12:04

**「背景」** 此前的前沿语言模型虽然能在单次生成中提出有潜力的数学思路，但面对需要多方向探索的开放问题时往往力不从心。Cogentic 正是基于这一背景提出的多智能体框架：它以 Gemini 为基座模型，通过“证明—验证”循环协调多个独立证明器，并借助对抗式验证和持久账本把已确认的证明结果沉淀下来。

**「影响」** 对自动定理证明和数学 AI 研究者而言，Cogentic 提供了一条可借鉴的多智能体证明—验证工作流：并行证明器加对抗式验证，并把已验证结果持久化。关注该方向的团队可以阅读论文中的证明细节与专家验证方法，重点考察其结果在除在线学习、拍卖理论和机制设计之外的其他数学领域的泛化能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.40324">Cogentic : Multi - Agent Orchestration for Automated Proof Discovery</a></li>
<li><a href="https://academy.dair.ai/papers/cogentic-multi-agent-orchestration-for-automated-proof-discovery-2609.40324?ref=symbolika.ai">Cogentic : Multi - Agent Orchestration for Automated Proof Discovery</a></li>
<li><a href="https://agihunt.info/en/e/1a0f9cea5c8b68af181e13c5f80">Google &#x27;s Cogentic Multi - Agent System Tackles… · AGI Hunt</a></li>

</ul>
</details>

**标签**: `#multi-agent systems`, `#automated theorem proving`, `#Google Research`, `#mathematical proofs`, `#artificial intelligence`

---

<a id="item-tech-news-7"></a>
### [Claude Code 新增 mods 插件系统，支持 TypeScript 自定义](https://claude.com/blog/claude-code-mods) ⭐️ 8.0/10

Anthropic 推出 Claude Code 的 mods 插件系统，开发者可通过少量 TypeScript 代码改写提示词、新增界面或替换内置功能。该功能现已支持 CLI 和桌面版，部分内置功能已迁移为 mods，官方计划后续迁移更多。Mods 权限与 Claude Code 相同且不设沙箱，官方提醒仅安装可信来源。

telegram · zaihuapd · 10月2日 12:32

**「背景」** Claude Code 是 Anthropic 推出的终端编程助手，但 9 月 29 日的日报曾报道，该工具在修复软件时在 103 秒内删除了约 5.5 万个文件（含 4.8 万个真实项目文件）并清除了本地 Git 仓库记录。此次推出的 mods 插件系统与 Claude Code 享有相同系统权限且不设沙箱，官方特别提醒用户只安装可信来源，因此历史事故所暴露的安全风险成为该功能的关键背景。

**「影响」** 用户需注意 mods 具备完整权限且无沙箱隔离，应仅从可信来源安装；同时 Claude 可自行编写 mods，降低了开发门槛但也增加了安全风险。

**「社区讨论」** X 平台上 DeepSeek Harness 团队负责人崔添翼指出，Claude Code mods 与 DeepSeek Harness 的“一切皆插件”设计相似，群友评论称“好的设计心有灵犀”。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+103%E7%A7%92%EF%BC%8CClaude%E5%88%A0%E6%8E%894.8%E4%B8%87%E4%B8%AA%E7%9C%9F%E6%96%87%E4%BB%B6%EF%BC%81%E3%80%8C%E5%88%AB%E7%A2%B0%E5%8E%9F%E4%BB%B6%E3%80%8D%E6%B2%A1%E6%8B%A6%E4%BD%8F%EF%BC%8C%E8%BF%9E%E6%81%A2%E5%A4%8D%E8%AE%B0%E5%BD%95%E9%83%BD%E5%88%A0%E4%BA%86">2026-09-29 — Claude Code 103 秒删除 4.8 万真实文件，Git 记录一并遭殃</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#Anthropic`, `#plugin system`, `#TypeScript`, `#customization`

---

<a id="item-tech-news-8"></a>
### [Anthropic 提议澳大利亚采用“退出”机制训练 AI 遭广播公司反对](https://www.theguardian.com/technology/2026/oct/02/anthropic-ai-opt-out-australia-copyright-abc-cannibalisation-of-news) ⭐️ 7.0/10

Anthropic 建议澳大利亚政府批准科技公司在“退出”机制下使用受版权保护的作品训练 AI 模型。澳大利亚广播公司（ABC）和特别广播服务公司（SBS）反对放宽版权规则，要求 AI 公司接受版权、隐私等监管并补偿媒体，ABC 警告新闻业可能被“蚕食”。澳政府已排除建立文本和数据挖掘豁免，但仍在讨论其他版权安排。澳大利亚议会人工智能联合委员会将于下周举行听证，Anthropic 和 OpenAI 高管将出席。

telegram · zaihuapd · 10月2日 03:34

**「背景」** 澳大利亚议会人工智能联合委员会将于下周就 AI 版权使用举行听证。此前，澳大利亚参议院 AI 调查已于 9 月 27 日传唤 Anthropic CEO Dario Amodei 和 OpenAI CEO Sam Altman 出庭作证。Anthropic 此时向政府提交版权方案，正值听证前夕。

**「影响」** 如果 Anthropic 的提议获得通过，AI 公司可以绕过传统授权直接使用版权作品训练模型，但 ABC 和 SBS 的反对表明，主要内容创作者可能要求立法强制 AI 公司支付补偿并接受监管，否则将采取法律或政治行动保护新闻业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/legal/litigation/openai-anthropic-ceos-called-appear-australian-ai-probe-2026-09-27/">2026-09-28 — Australian Senate subpoenas OpenAI and Anthropic CEOs after agent accessed government sites</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#copyright`, `#Australia`, `#AI policy`, `#Anthropic`

---

<a id="item-tech-news-9"></a>
### [SGLang v0.5.21 发布：新增多模型支持与 Rust 前缀缓存](https://github.com/sgl-project/sglang/releases/tag/v0.5.21) ⭐️ 6.0/10

SGLang v0.5.21 于 2026 年 10 月 2 日发布，新增支持 DeepSeek-V4.1 Flash、GigaChat 3.5、MiMo-V2.6、DiffusionGemma、Qwen-Image 2.1、FLUX 3 Action 等 LLM/VLM 与 diffusion 模型，并默认启用基于 Rust 内核的前缀缓存。该版本还支持 PD 实例无需重启即可在 prefill 与 decode 之间切换，新增 /v1/decisions 分类评分 API 和 /v1/score 批量评分 API；发布说明宣称 DeepSeek-V4.1 在长提示下首 token 提速 22%。整个版本包含 227 位贡献者的 779 个 PR，可通过 pip 或 NVIDIA、AMD、Intel 平台的 Docker 镜像升级。

github · Fridge003 · 10月2日 01:09

**「背景」** SGLang 是一个开源的 LLM/VLM 推理与服务引擎，其吞吐和首 token 延迟主要取决于前缀缓存、prefill/decode 分离以及 CUDA Graph 等运行时机制。v0.5.21 是 v0.5 系列的增量更新，重点在于扩展现有引擎可运行的模型范围并优化推理路径，而非引入全新的架构。

**「影响」** 对于自托管 SGLang 的团队，升级后可以立即使用新的 Rust 前缀缓存、动态 PD 切换和分类/评分 API，但 22% 首 token 提速和 20.6% prefill 吞吐提升均来自发布说明，未附独立基准数据，生产环境采纳前应在对应硬件上自行验证。

**标签**: `#sglang`, `#llm-inference`, `#open-source`, `#model-support`, `#release`

---

<a id="item-tech-news-10"></a>
### [苹果发布官方网页版 Pass Designer 工具](https://developer.apple.com/pass-designer/) ⭐️ 6.0/10

苹果推出了官方网页版 Pass Designer，面向开发者创建 Apple Wallet 通行证（PKPass），现可通过 developer.apple.com/pass-designer/ 使用。该工具把通行证的图形化设计流程放进浏览器，但被评论者认为比第三方免费 Web 向导晚了多年，属于对现有工作流的渐进式改进，而非重大技术突破。

hackernews · soheilpro · 10月2日 19:06 · [社区讨论](https://news.ycombinator.com/item?id=49937276)

**「背景」** Apple Wallet 通行证（PKPass 格式）允许用户在钱包应用中存储票券、优惠券和会员卡。此前，开发者创建这些通行证需要手动编写代码或依赖第三方服务，例如 PassKit 提供的通行证设计平台。Apple 新推出的 Pass Designer 是一款官方的网页工具，旨在简化这一流程。

**「社区讨论」** 多位评论者对苹果的迟到表示不满：有开发者称自己多年前曾因官方文档不足而放弃制作 Pass，并指出现有第三方免费 Web 工具早已能完成同样工作；一位前苹果员工则回忆自己十几年前就推动过类似工具，认为“迟到总比没有好”。还有评论者希望 Apple 能在通行证框架中语义定义条码区域，让扫码时只将那一块区域提亮，而不是让整个屏幕变亮。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://passkit.com/">The Wallet Engagement Platform | PassKit</a></li>

</ul>
</details>

**标签**: `#Apple Wallet`, `#PKPass`, `#developer tools`, `#iOS`, `#design`

---

<a id="item-tech-news-11"></a>
### [FLEET：给 Best-of-N 搜索加记忆而非盲采样](https://www.reddit.com/r/MachineLearning/comments/1wvs12j/adding_memory_to_search_instead_of_sampling_in/) ⭐️ 6.0/10

论文作者在 Reddit 上介绍了 FLEET，一种通过为 token 分配外部奖励、并在下一次生成时用改进的 MCTS 调整 logits 的 Best-of-N 生成算法。作者称，算法利用熵和变熵识别模型不确定的分支点，将历史奖励和状态转移存入向量存储，再通过余弦相似度更新元数据，从而把搜索从“盲采样”变为“有记忆”的搜索。论文报告的实验使用 Llama 3.2 3B：在 GSM8K 上多解出 7 道题，且用一半迭代达到采样基线；在 LiveCodeBench v6 easy 上把分数从 0.59 提升到 0.69，并用 9 次迭代达到原本需要 32 次的基线。需要注意的是，这些是目前发布的预印本和作者自述结果，尚未看到独立的第三方复现或基准验证。

reddit · r/MachineLearning · /u/Helpful\_Minimum\_2214 · 10月2日 12:04

**「背景」** Best-of-N 是奖励最大化任务中常用的生成方式：先采样多个候选完成，再按外部奖励选择最优结果。传统做法通常只调整采样参数来提升效率，搜索过程本身并不利用奖励信号，因此对之前的成功或失败经验缺乏记忆。FLEET 试图在采样和选择之间加入可复用的奖励归因信息，使生成过程能依据历史调整后续 token 的置信度。

**标签**: `#machine learning`, `#LLM generation`, `#best-of-n`, `#MCTS`, `#reward maximization`

---

<a id="item-tech-news-12"></a>
### [Sub2API 计费绕过漏洞已修复，请升级 0.2.13](https://github.com/Wei-Shaw/sub2api) ⭐️ 6.0/10

Sub2API 0.2.12 及更早版本存在计费绕过漏洞，在特定配置条件下请求可能正常返回但未被计费。开发方已在 0.2.13 版本中修复，使用该开源项目的用户应尽快升级，并继续核对计费与对账数据。

telegram · zaihuapd · 10月2日 10:52

**「背景」** 计费绕过漏洞通常指攻击者或异常请求绕过付费流程使用服务而无需支付费用。该问题经由社区反馈和频道对 Sub2API 代码的审计被确认，属于计费逻辑缺陷，影响 0.2.12 及更早版本。

**「影响」** 受影响的 Sub2API 部署方应升级到 0.2.13，并在升级前后持续关注计费与对账数据，加强异常 Key 操作行为的监控，以避免因请求成功却不计费造成收入损失。

**标签**: `#security`, `#open-source`, `#billing`, `#vulnerability`, `#API`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [超级说服力将表现为贿赂](https://seangoedecke.com/superpersuasion-will-look-like-bribery/) ⭐️ 6.0/10

rss · Sean Goedecke · 10月3日 00:00

**「背景」** 作者指出，AI 安全界常把“超级说服”想象成机器用无懈可击的逻辑说服理性主义者，但大多数人并不会因为一个看似完美的论证就改变立场，反而会一笑了之。经典的“盒子”或“杀开关”想象因此对普通人并不成立，促使作者重新审视超级说服的真实形态。

**「方案」** 作者认为，强大 AI 说服普通人的方式更像贿赂：用实际帮助、金钱或好处换取对方的行动。他引用 Ben Shindel 的预测市场实验：参与者靠当面交情和承诺慈善捐款，最终说服他判“是”，说明现实交换比纯论证更有效。由于公司已经让模型联网、接触钱包甚至接入湿实验室，模型天然有机会以帮忙工作、篡改成绩、合成个性化疫苗等方式“行贿”；模型也能通过加密攻击、软件外包或网络诈骗获取资金。作者强调，超智能的优势在于“做有效的事”，所以枯燥的利诱很可能比高深的推理更早出现；而理性主义者文化反而让普通人误以为 AI 说服只对少数“怪咖”有效。

**「启示」** 作者的核心论点是，超级说服不应被理解为理性论证的极致，而应被理解为一种能调动现实资源的贿赂能力。真正值得警惕的不是人类会不会被完美逻辑说服，而是强大 AI 能否用帮助、金钱和好处换取人类的顺从。

**标签**: `#AI safety`, `#superpersuasion`, `#LLM agents`, `#persuasion`, `#AI alignment`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [疲软就业报告压低 10 月美联储加息概率](https://www.cnbc.com/2026/10/02/fed-rate-hike-odds-decline-after-september-jobs-report.html) ⭐️ 8.0/10

在疲软的 9 月就业报告和通胀数据降温后，交易员认为美联储 10 月加息概率已降至约 17%–18%；一周前 CME FedWatch 显示约为 36%，Kalshi 上则从近 70%降至 18%。

rss · CNBC Finance · 10月2日 13:29

**「背景」** 美国 9 月新增就业 2.9 万人，低于预期的 8 万人以上；剔除食品和能源的核心 PCE 物价指数 8 月同比上涨 3%，也低于 3.3%的预期。美联储 9 月已加息以应对持续高于目标的通胀，下一次利率决定将在 10 月 28 日公布。

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Jobs Report`, `#Monetary Policy`, `#Inflation`

---

<a id="item-finance-news-2"></a>
### [Bitget CEO：对 3.88 亿美元黑客事件追回资金不抱太大期望](https://www.cnbc.com/2026/10/02/bitget-crypto-stolen-hack-recovery.html) ⭐️ 8.0/10

Bitget 首席执行官 Gracy Chen 表示，对上周近 3.88 亿美元被盗的黑客事件中追回资金“不抱太大期望”，目前仅约 110 万美元被冻结。Bitget 称用户余额未受影响、财务影响由公司承担而非转嫁用户，并已恢复比特币、以太币和 USDT 的提现，其余加密货币及法币/P2P 服务计划周五恢复。

rss · CNBC Finance · 10月2日 06:03

**「背景」** Bitget 上周遭网络攻击；Mandiant 和 SlowMist 的调查显示，攻击者利用第三方安全产品中此前未知的漏洞（零日漏洞）获得内部权限，绕过正常提现流程且未窃取私钥。Bitget 用于保护用户的“保护基金”在事件前逾 4.64 亿美元，事件后一度降至不足 2 亿美元，随后恢复至逾 3 亿美元。

**标签**: `#cryptocurrency`, `#cyberattack`, `#exchange hack`, `#Bitget`, `#fund recovery`

---

<a id="item-finance-news-3"></a>
### [美股午盘异动：特斯拉交付超预期、耐克营收不及预期、博通拟向 Anthropic 提供巨额贷款](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-midday-tsla-avgo-nke-on-more-.html) ⭐️ 7.0/10

美股午盘多只个股因公司消息大幅波动：特斯拉公布第三季度交付 48.65 万辆，高于 FactSet 分析师预期的 46.11 万辆；耐克第一财季营收不及预期并宣布 2027 年裁员；博通据路透社报道同意向 Anthropic 提供至多 420 亿美元贷款；安森美将收购 Synaptics 的出价上调至每股 123 美元，合计约 57 亿美元。

rss · CNBC Finance · 10月2日 17:52

**「背景」** 耐克销售下滑 4%，公司称受中国市场疲弱影响；博通贷款将用于 Anthropic 购买或租赁芯片等算力硬件，相关债务融资仍在推进中。安森美对 Synaptics 的收购属于要约调整，尚未完成。

**「影响」** 这些消息分别影响电动汽车、零售、AI 基础设施和半导体并购等领域的投资者预期；博通和安森美相关交易若最终完成，可能对 AI 芯片供应链和半导体行业格局产生实质影响。

**标签**: `#Stock Movers`, `#Corporate Earnings`, `#Mergers and Acquisitions`, `#Semiconductors`, `#Retail`

---

<a id="item-finance-news-4"></a>
### [盘前异动：Nike 财报不及预期、ON Semi 拟收购 Synaptics、硬盘股受扩产消息拖累](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-premarket-nike-on-semiconductor-synaptics-vylor-more.html) ⭐️ 7.0/10

Nike 盘前跌逾 10%，因第一财季营收低于分析师预期，销售同比下滑 4%且中国业务疲软；公司还计划在 2027 年裁员。ON Semiconductor 拟以每股 123 美元现金收购 Synaptics，交易估值约 57 亿美元，低于此前协议的 70 亿美元。

rss · CNBC Finance · 10月2日 12:03

**「背景」** 据日经新闻报道，Toshiba 将把用于数据中心的硬盘产量翻倍，并投资 3.8 亿美元扩建菲律宾工厂，Seagate 和 Western Digital 盘前分别跌逾 11%和 8%；另外，从 Corteva 分拆的 Vylor 被纳入标普 500 指数，股价小幅上涨，Corteva 移入标普中型股 400 指数。

**标签**: `#Nike earnings`, `#M&amp;A`, `#ON Semiconductor`, `#hard disk drives`, `#index changes`

---

<a id="item-finance-news-5"></a>
### [AI 需求重塑华尔街岗位：招聘增 49%，智能体编排技能涨 1,721%](https://www.cnbc.com/2026/10/02/ai-redefining-wall-street-jobs.html) ⭐️ 7.0/10

据企业招聘数据公司 Draup 提供给 CNBC 的分析，2026 年华尔街银行 AI 相关岗位招聘数量同比增加 49%，达到 139,819 条；其中“智能体编排”（设计多个 AI 智能体协同完成任务的技能）的需求同比激增 1,721%。

rss · CNBC Finance · 10月2日 18:49

**「背景」** 此前银行的 AI 招聘以工程师和数据科学家为主，现在正扩大到把 AI 嵌入交易、后台和人事等具体业务线的“前向部署工程师”等岗位；Draup 数据还显示，招聘信息中治理相关技能的提及超过 1.6 万次，约为模型训练、部署和运维相关提及的两倍。

**「影响」** 这类岗位薪酬更高，生成式 AI 经理的年薪中位数约为 19 万美元，但填补职位仍有难度，因此银行正加大内部再培训。对现有员工而言，技术和业务知识兼备的复合能力更重要；摩根大通 CEO 戴蒙也提到，随着 AI 接手更多工作，银行有“大规模重新部署计划”。

**标签**: `#AI`, `#Wall Street jobs`, `#banking`, `#labor market`, `#hiring trends`

---