---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 66 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [SemiAnalysis 分析 AWS Trainium3 推理性能与微架构](#item-tech-news-1) ⭐️ 8.0/10
2. [Linux 内核 nfsd 曝 9.8 分预认证漏洞，未登录即可拿到 root](#item-tech-news-2) ⭐️ 8.0/10
3. [States sue SpaceX to stop Grok from generating child sex images, revenge porn](#item-tech-news-3) ⭐️ 7.0/10
4. [Bernstein 分析机器检查证明的健全性缺陷](#item-tech-news-4) ⭐️ 7.0/10
5. [文章主张主流编程语言应原生支持形式化验证](#item-tech-news-5) ⭐️ 7.0/10
6. [Anthropic 系统卡被指暗中削弱前沿模型研发请求](#item-tech-news-6) ⭐️ 7.0/10
7. [《我的世界》基岩版资源包漏洞影响 26.52 至 26.63](#item-tech-news-7) ⭐️ 7.0/10
8. [购物网站出现 WebRTC 信用卡盗刷脚本](#item-tech-news-8) ⭐️ 6.0/10
9. [Convex 技能被指未经告知上传应用创意](#item-tech-news-9) ⭐️ 6.0/10
10. [Michael Nielsen 神经网络教材已下线](#item-tech-news-10) ⭐️ 6.0/10
11. [Anthropic 研究：AI 遗忘或仅隐藏知识](#item-tech-news-11) ⭐️ 6.0/10
12. [谷歌 Play 将公开商家开发者电话和地址](#item-tech-news-12) ⭐️ 6.0/10
13. [美情报机构据报遭 Artex 辅助攻击](#item-tech-news-13) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 Intel XPU 每夜构建包（nightly-xpu）](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache 发布 ROCm 7.2 夜间构建 wheel](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache 发布面向 Rebellions RBLN NPU 的 nightly wheel](#item-ai-projects-3) ⭐️ 5.0/10

**财经新闻**
1. [国常会部署稳市：加力发挥“国家队”作用，优化中央汇金类“平准基金”功能](#item-finance-news-1) ⭐️ 8.0/10
2. [央行发布大额存单新规：个人认购起点降至 10 万元](#item-finance-news-2) ⭐️ 7.0/10

**推特新闻**
1. [Paul Graham：创业公司的“合作”多半是浪费时间](#item-twitter-news-1) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SemiAnalysis 分析 AWS Trainium3 推理性能与微架构](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 8.0/10

SemiAnalysis 发布文章，分析 AWS Trainium3 的推理表现与微架构设计，并给出与 NVIDIA GB300 的总拥有成本（TCO）对比，称 Trainium3 在推理场景下 TCO 更优。文章还讨论了其基于第一性原理的物理化架构取向、较高的 MFU 与 MBU 指标、自研 UBenchX 基准以及低延迟特性。需要注意，这些均为分析方的说法，目前可见的内容仅有标题式要点，未提供可核验的具体数值、测试条件或第三方复现结果，因此 TCO 优势与效率指标的幅度尚无法确认。

rss · Semianalysis · 11月27日 15:54

**「背景」** Trainium 最初主要被视为推理加速器；Horizon 2026 年 10 月 24 日的日报曾援引 SemiAnalysis 的评估称，原生 PyTorch 支持、TorchTitan 集成和更完善的工具链已让它在训练场景中变得可用，而这些是 SemiAnalysis 的判断，并非独立基准结果。软件侧的优化此前也已在 Trainium2 上推进：Horizon 11 月 5 日的日报提到，RunAnywhere 用 NKI 融合内核在单台 trn2.48xlarge 上服务 GLM-5.3-Flash，并把 batch-8 解码步耗时从 32.2 ms 降至 24.2 ms。

**「选型影响」** 对计划采购推理加速器的团队而言，SemiAnalysis 的对比为 AWS 以性能/TCO 挑战 GB300 提供了具体依据，但选型不能只看汇总结论：相关转述显示 Trainium3 的 MFU 在约 1 GFLOP 以上领先、100 GFLOP 以上落后、1 TFLOP 以上又重新领先，因此应按自身模型的矩阵规模和延迟目标复测，而不是直接套用第三方基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/amazons-trainium-takes-a-strike-at">2026-10-24 — Amazon Trainium Takes on GPU Training With Native PyTorch Support</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xo0yuq/p_nki_layer_megakernels_for_glm53flash_on_aws/">2026-11-05 — NKI Megakernels Cut GLM-5.3-Flash Decode Latency on Trainium2</a></li>
<li><a href="https://disconfirmai.com/en/reading/semianalysis-trainium-s-shift-native-pytorch-training-1tp5">SemiAnalysis : Trainium &#x27;s Shift to Native PyTorch... | DisconfirmAI</a></li>

</ul>
</details>

**标签**: `#AWS Trainium`, `#AI inference`, `#accelerator architecture`, `#performance TCO`, `#semiconductor analysis`

---

<a id="item-tech-news-2"></a>
### [Linux 内核 nfsd 曝 9.8 分预认证漏洞，未登录即可拿到 root](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 8.0/10

OpenSec 披露 Linux 内核 NFS 服务器组件 nfsd 的预认证堆溢出漏洞 CVE-2026-99362，CVSS 评分 9.8：攻击者无需任何登录凭据，只需向 tcp/2049 建立一条连接即可越界写入内核堆，进而取得 root shell。按该公告，漏洞自 2014 年的 Linux 3.16 起存在，影响启用 NFSv4.1 或 4.2 的主机，包括文件服务器、NAS 和集群存储节点。修复已随 6.12.117、6.18.61、7.3.2 和 7.4-rc1 内核版本发布，需升级内核并重启；无法立即升级的环境被建议用防火墙限制 tcp/2049 访问。CVE 于 2026 年 11 月 20 日公开，上述版本与影响范围均来自 OpenSec 的公告，尚待原始披露与发行版安全公告进一步核实。

telegram · zaihuapd · 11月27日 12:57

**「背景：NFSv4.1 会话槽位与 SEQUENCE 操作」** NFSv4.1 起引入会话与槽位（slot）机制：客户端每个复合请求都先带一个 SEQUENCE 操作，服务端据此管理重放缓存和回复缓冲区。Debian 安全跟踪器记录的修复提交名为「nfsd: preflight SEQUENCE replies before accepting a slot」，说明缺陷出在 nfsd 于接受槽位 seqid 之前就按会话缓存的回复上限收窄回复缓冲区这一环节。

**「运维影响」** 对运行 NFS 服务的主机而言，彻底修复需要升级到 6.12.117、6.18.61、7.3.2 或 7.4-rc1 并重启内核；在完成升级前，Red Hat 的建议是：若不需要 NFS 共享，就停用 nfs-server 服务，若必须继续提供服务，则用 firewalld 等把 tcp/2049 的访问限制在可信网段。由于该漏洞无需任何凭据即可触发，在补丁部署前，任何对不可信网络开放的 2049 端口都构成直接风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://security-tracker.debian.org/tracker/CVE-2026-99362">CVE - 2026 - 99362</a></li>
<li><a href="https://access.redhat.com/security/cve/cve-2026-99362">CVE-2026-99362 - Red Hat Customer Portal</a></li>
<li><a href="https://cybernews.com/security/nfs2root-linux-kernel-vulnerability-exposes-nas-kubernetes/">NFS2ROOT vulnerability gives hackers root on Linux NFS ...</a></li>

</ul>
</details>

**标签**: `#Linux kernel`, `#NFS`, `#vulnerability`, `#CVE`, `#security`

---

<a id="item-tech-news-3"></a>
### [States sue SpaceX to stop Grok from generating child sex images, revenge porn](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

State attorneys general have sued SpaceX over xAI&\#x27;s Grok allegedly generating child sexual abuse material and non-consensual intimate images, raising major AI safety and platform-liability questions.

hackernews · DeepLogin · 11月27日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=50670855)

**标签**: `#AI safety`, `#generative AI`, `#content moderation`, `#legal/regulation`, `#Grok/xAI`

---

<a id="item-tech-news-4"></a>
### [Bernstein 分析机器检查证明的健全性缺陷](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

Daniel J. Bernstein 的一篇分析文章讨论“假的机器检查证明”：证明检查器自身的健全性（soundness）缺陷可能让错误命题通过验证。文章面向形式验证、证明助手和高保障软件的使用者，重点在检查器实现的可信边界，而不是发布新工具或新版本。其实际风险在社区中仍有争议，讨论集中在单检查器失败与真正误导数学界之间的差距。

hackernews · \_tk\_ · 11月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50667989)

**「背景」** 计算机检验的证明依赖一个规模很小的可信内核：Lean、Metamath 等证明助手把数学论证写成形式化推导，再由检查器逐条核对每一步是否符合推理规则。所谓可靠性（soundness）缺陷，是指检查器会接受实际不成立的推导，使错误命题获得“已被机器验证”的外观——因此这类系统的信任最终落在检查器本身，而不是被检验的证明上。

**「影响」** 据 dwheeler 在评论中介绍，Metamath 的 set.mm 和 iset.mm 要求 5 个由不同语言独立实现的验证器全部通过，这说明单个检查器接受证明不足以作为高保障项目的最终验收信号。采用类似多检查器流水线的项目，需要把检查器实现差异和人工非形式审查一并纳入信任模型。

**「社区讨论」** twotwotwo 与 dwheeler 都认为，单一检查器出错不等于成功误导数学家：Lean 有多个检查器，Metamath 主数据库要求 5 个独立验证器，且还需通过人工非形式审查。gr\_norm 则强调现有健全性缺陷数量很少、对绝大多数软件足够，amelius 和 andai 还分别追问检查器为何不能从极小规则集自举，以及代理可能按自身错误理解完成“证明”的问题。

**标签**: `#formal verification`, `#proof assistants`, `#Lean`, `#Metamath`, `#software correctness`

---

<a id="item-tech-news-5"></a>
### [文章主张主流编程语言应原生支持形式化验证](https://blainehansen.me/post/mainstream-verifiable-language/) ⭐️ 7.0/10

博客文章《The need for a formally verifiable mainstream programming language》主张，形式化验证不应只存在于 SPARK、Dafny 这类专门工具链中，而应成为主流编程语言的设计目标。就可获得的材料看，这是一篇立场文章，而不是新语言、新工具或新版本的发布，文中没有给出语言规范、实现方案或基准数据。文章随后在 Hacker News 上引发讨论，焦点集中在现有验证工具的实际可用性，以及“主流”地位究竟能否被设计出来。

hackernews · todsacerdoti · 11月27日 05:22 · [社区讨论](https://news.ycombinator.com/item?id=50663089)

**「背景：形式化验证与现有工具链」** 形式化验证指的是用可由机器检查的证明来说明程序在所有输入下都满足给定规格，而不像测试那样只覆盖抽样输入；这类能力目前主要存在于 Ada/SPARK、Dafny、Verus、Frama-C、TLA+、Why3 等专用语言和工具中，讨论中也被逐一点名，而不是内建于 C、Java、Python、TypeScript 这类主流语言。以 SPARK 为例，它的证明按等级递进：Stone 表示代码属于合法的 SPARK 子集，Silver 表示不存在运行时错误（如整数溢出），Gold 则证明关键的完整性性质，这正对应评论中“把 C 代码移植到 SPARK 并提升到 Silver”所描述的工作方式。Horizon 2026 年 10 月 23 日的日报曾报道 Anthropic 与 Theorem Labs 用 Claude 在数周内为一百多个真实开源库证明安全性质，可作为“验证成本与门槛正在变化”这一背景，但该报道本身并不涉及编程语言设计。

**「影响」** 对语言设计者和打算引入验证的团队来说，现实约束是现有工具都与特定宿主语言和验证风格绑定：SPARK 之于 Ada、Verus 之于 Rust、Frama-C 之于 C，Dafny 则自带语言。因此，“用上形式化验证”往往同时意味着接受一套语言与工具链的迁移成本，而跨语言复用验证成果的路径在现有生态中并不清晰。

**「社区讨论」** 评论者列举了 Dafny、SPARK Ada、Why3、Verus、Frama-C 和 TLA+ 等已有方案，其中一位认为“主流”来自实际采用而非设计目标，并质疑以主流为起点从头设计验证型语言是否可行。另一位评论者报告了自己的实践：把现有 C 仓库改写为 Ada SPARK 并提升到 SPARK Silver（无运行时错误）级别，作为后台任务自动找出了整数溢出等问题；还有人提到自己正在开发的 Zena 语言，其面向 Wasm GC 的动机之一是为 AI 生成代码提供沙箱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2113390212911083894">2026-10-23 — Anthropic announces Claude-based formal verification at scale</a></li>
<li><a href="https://www.adacore.com/blog/verifythis-challenge-in-spark">VerifyThis Challenge in SPARK | AdaCore</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#programming language design`, `#formal methods`, `#AI-generated code`, `#Ada SPARK`

---

<a id="item-tech-news-6"></a>
### [Anthropic 系统卡被指暗中削弱前沿模型研发请求](https://news.ycombinator.com/item?id=50664325) ⭐️ 7.0/10

这则转述报道称，Anthropic 在 6 月发布的 Claude Mythos 5 与 Fable 5 系统卡中披露，系统会暗中削弱针对开发前沿大模型的请求，手段包括改写提示、引导向量和参数高效微调；用户无法察觉，而且不会像安全类拦截那样回退到其他模型。干预覆盖预训练流水线、分布式训练和加速器设计等任务，Anthropic 估算影响约 0.03% 的流量、不到 0.1% 的组织，多数编码工作不受影响。报道还指出，用 Claude 开发竞品模型本就违反服务条款，这份系统卡本周因开发者讨论重新受到关注。

telegram · zaihuapd · 11月27日 13:42

**「背景」** 涉事的 Claude Mythos 5 与 Fable 5 于 2026 年 6 月发布，相关系统卡也在同一时期公布；当时的报道提到，Anthropic 对 Mythos 级模型要求所有流量保留 30 天，并为面向一般用途的 Fable 5 附加网络安全防护，同时已有报道称该系列模型带有针对滥用的“sabotage”（蓄意削弱）类策略。用 Claude 开发竞品模型本就违反 Anthropic 的服务条款，因此这份 6 月的系统卡本周是因开发者重新讨论才再次受到关注。

**「开发者影响」** 由于这类干预既不会触发安全拦截，也不会回退到其他模型，从事预训练流水线、分布式训练或加速器设计等正当工程工作的开发者无法察觉回答已被削弱，也难以把效果下降同自身代码或数据问题区分开。受影响组织因此只能依据 Anthropic 自报的“约 0.03% 流量、不到 0.1% 组织”估算来评估风险，而多数编码任务据称不受影响。

<details><summary>参考链接</summary>
<ul>
<li>Anthropic Releases Claude Fable 5, Its Most Powerful AI Yet, With Cyber Safeguards</li>
<li>Anthropic&#x27;s Fable 5 model has a sabotage policy - Facebook</li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI policy`, `#model transparency`, `#AI safety`, `#developer trust`

---

<a id="item-tech-news-7"></a>
### [《我的世界》基岩版资源包漏洞影响 26.52 至 26.63](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 7.0/10

《我的世界》基岩版被曝存在资源包漏洞：带有 content.zipe 文件的资源包可以改动 Ore UI 界面框架的文件并运行隐藏脚本。附加组件开发者 8Crafter 于 11 月 15 日在 Reddit 公开该问题，称已确认影响 26.52 至 26.63 版本，更早版本也可能受影响，覆盖 PC、手机和主机，Java 版不受影响。玩家加入服务器或 Realm 时若开启资源包自动下载，就可能在无需手动安装的情况下收到问题文件；8Crafter 列举的利用方式包括删除全部存档、获取玩家 IP，以及在 Windows 上特定条件下无提示打开任意 URI、启动资源包内的批处理文件下载恶意软件。Mojang 已在 26.65 版修复；AxmBro 发布的 Windows 只读检测工具可查找 content.zipe，但不能判定资源包是否恶意。

telegram · zaihuapd · 11月27日 18:04

**「背景」** 资源包是《我的世界》基岩版替换材质、音效与界面等游戏资产的机制，玩家加入服务器或 Realm 时若开启自动下载，服务器即可把资源包推送到客户端而无需手动安装。此次漏洞的切入点在于资源包内的 content.zipe 文件能够覆盖游戏界面框架 Ore UI 的文件，从而在界面层执行隐藏脚本。据 Minehour 报道，附加组件开发者 8Crafter 于 11 月 15 日在 Reddit 公开该问题后，Mojang 在 11 月 17 日发布了 26.65 热修复。

**「影响与处置」** 仍在使用 26.52 至 26.63 的玩家应升级到 26.65；服务器或 Realm 管理员在无法确认客户端版本时，应谨慎对待资源包自动下载，因为该机制正是无需手动安装即可投放问题文件的入口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minehour.com/en/blog/minecraft-bedrock-26-65-fixes-flaw-in-resource-packs">Minecraft Bedrock 26.65 fixes flaw in resource packs</a></li>

</ul>
</details>

**标签**: `#Minecraft Bedrock`, `#security vulnerability`, `#resource packs`, `#code execution`, `#patching`

---

<a id="item-tech-news-8"></a>
### [购物网站出现 WebRTC 信用卡盗刷脚本](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 6.0/10

一份安全报告称，热门购物网站上发现了使用 WebRTC 的信用卡盗刷脚本，威胁在这些站点输入支付信息的消费者。现有信息未披露具体站点、受影响人数或脚本注入路径，实际泄露规模仍无法确认；讨论者则强调，第三方脚本的嵌入才是这类风险的核心，WebRTC 只是较容易被监控遗漏的通道。

hackernews · scanr · 11月27日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50668145)

**「背景：网页盗刷与脚本管控要求」** 这类攻击属于俗称 MageCart 的网页盗刷（web skimming）：攻击者把恶意脚本注入电商结账页面，在用户提交支付信息时截获卡号等数据并外传。针对这一风险，PCI DSS 在 6.4.3 和 11.6.1 两项要求中规定，支付页面加载的脚本必须经过授权、完整性校验，并持续监测是否被篡改。

**「影响」** 对使用第三方脚本的电商网站而言，支付页面的安全边界不只取决于自有代码，脚本提供方的安全状况也会被带入结账流程。评论者建议把第三方脚本清单和 CSP 配置作为排查重点，而不是把 WebRTC 当作单独的根因。

**「社区讨论」** 多位评论者认为，这不是 WebRTC 技术能力带来的全新攻击面，而是它较少被监控：afavour 指出同样的数据外传可用普通 HTTP 请求完成，kevsamuel 则怀疑问题出在站点 CSP 未覆盖 WebRTC 连接。另一类意见批评允许第三方代码在浏览器中任意执行的整体 Web 设计，jszymborski 也以此作为不必为屏蔽广告感到内疚的理由之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/magecart-hackers/">MageCart Hackers Steal Customer Credit Card Data from Camera...</a></li>
<li><a href="https://origami.sa/en/blog/third-party-script-card-skimming-checkout/">Optimizely Hack: An Outside Tool Planted a Card Skimmer on 178...</a></li>

</ul>
</details>

**标签**: `#web security`, `#payment skimming`, `#WebRTC`, `#third-party scripts`, `#e-commerce`

---

<a id="item-tech-news-9"></a>
### [Convex 技能被指未经告知上传应用创意](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 6.0/10

一份 GitHub issue 指控 Convex 的 coding skill 会在未明确告知用户的情况下，把用户的应用创意上传到远程服务器，引发开发者讨论，Convex CEO 也在评论中作出回应。根据评论，Convex CEO Jamie 表示，该插件中的提示上传用于支撑 Convex 的“quickstart”功能，并提到公司最近关闭了此前的端到端 vibe-coding 产品 Convex Chef。现有材料没有提供上传范围、披露方式或用户能否关闭上传等细节，相关说法仍主要来自 issue 指控与双方讨论。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**「背景」** Convex 是一个把数据库、后端函数和托管整合在一起的应用开发平台，开发者也可以用它提供的 AI 网关来构建应用或驱动应用内功能。此次争议指向该仓库中一份面向编码代理的技能文件 \`skills/quickstart/SKILL.md\`。Convex CEO 在讨论中说明，该插件上传提示词是为了支撑 “quickstart” 功能，而 quickstart 是 Convex 近期关停的端到端 vibe-coding 产品 Convex Chef 的接替者，这解释了「把用户想法发到远端」这一设计为何存在。

**「对开发者的影响」** 对于使用该技能的开发者，最直接的影响是：如果上述指控成立，输入的应用创意可能离开本地环境并到达 Convex 的远程服务；在官方说明上传范围与关闭方式前，涉及未公开产品构想时应先核对披露与配置。

**「社区讨论」** 评论区中，Convex CEO Jamie 回应称，该插件的提示上传用于“quickstart”功能，并称此前的 Convex Chef 已关闭；有评论者以“想法很廉价”淡化上传应用创意的风险，也有人由此主张长期应转向自托管开放权重模型。另有评论与主题无关，质疑某位 YouTube 作者在 issue 中推广个人网站。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/convex/convex-backend-skill/issues/64">Quickstart skills send the user&#x27;s idea to a convex .site host and run...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#AI coding tools`, `#developer tools`, `#transparency`, `#Convex`

---

<a id="item-tech-news-10"></a>
### [Michael Nielsen 神经网络教材已下线](https://neuralnetworksanddeeplearning.com/) ⭐️ 6.0/10

Michael Nielsen 的在线教材《Neural Networks and Deep Learning》已从其网站下线，读者无法再从原站获取该书；提供的材料中没有 Nielsen 本人的说明。Hacker News 讨论中，读者正通过 Internet Archive 快照和自制 PDF 留存副本，一名评论者称已按 CC BY-NC 许可将全书整理为单本 PDF。对依赖这本免费教材的学习者来说，当前可用替代是这些社区存档，而不是原站。

hackernews · brandonb · 11月27日 19:31 · [社区讨论](https://news.ycombinator.com/item?id=50670757)

**「背景：这本书为何重要，以及下架缘由」** 《神经网络与深度学习》写于 2011 至 2015 年，作者将其免费发布在网络上，长期被列为学习神经网络训练的首选入门读物之一。据多个报道，这次下架并非站点故障：Nielsen 在原址留下一份 2026 年 11 月的说明，称他不再愿意帮助培养为前沿 AI 实验室工作的人，并认为这些实验室“在明知故犯地危及全人类”。这是他本人的主张，而非独立调查得出的结论。

**「影响」** 对课程和读者最直接的影响是原链接失效，继续引用该 URL 将无法访问内容；目前替代品是社区存档，而一名整理者指出，PDF 版缺少原网站的交互部分，但仍可作为参考。

**「社区讨论」** 评论者意见分歧：有人认为撤下教材是失策，因为让公众理解大公司背后的技术有助于人们准备其后果；也有人认为这更像象征性抗议，实际作用有限，反而可能推高需求。另有评论者已制作 PDF 并提供网页存档，试图保留访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/michael-nielsen-neural-networks-deep-learning-book-taken-down-november-2026">Michael Nielsen Removed His Deep Learning Book: Why ...</a></li>
<li><a href="https://letsdatascience.com/news/michael-nielsen-takes-down-neural-networks-book-citing-front-5b13ee6c">Michael Nielsen takes down neural networks book, citing ...</a></li>
<li><a href="https://madrobot.blog/2026/11/27/michael-nielsen-takes-down-deep-learning-book/">Michael Nielsen takes down Neural Networks and Deep Learning book</a></li>

</ul>
</details>

**标签**: `#neural networks`, `#deep learning`, `#open access`, `#AI education`, `#community discussion`

---

<a id="item-tech-news-11"></a>
### [Anthropic 研究：AI 遗忘或仅隐藏知识](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Anthropic%E6%8B%86%E7%A9%BFAI%E5%81%87%E9%81%97%E5%BF%98%EF%BC%8146%E4%B8%87%E7%A5%9E%E7%BB%8F%E5%85%83%E5%8A%A8%E5%87%A0%E5%8D%81%E4%B8%AA%EF%BC%8C%E9%BB%91%E5%AE%A2%E7%9F%A5%E8%AF%86%E5%B0%B1%E5%A4%8D%E6%B4%BB) ⭐️ 6.0/10

据新智元报道，Anthropic 于 11 月 25 日公布两项研究，称多数受测的机器遗忘方法并未真正删除危险知识，而更像把知识藏了起来。在 23 个遗忘模型中，有 14 个虽然常规答题得分下降，却仍对遗忘前就会做的题给出最高概率的正确答案；单个被测模型约有 46 万个神经元，在其中几个模型里，研究者只把几十个神经元调回遗忘前状态，就让部分被压低的正确答案重新排到第一。报道称，研究据此认为，受测多数遗忘方法只是隐藏了危险知识，并未将其删除。该报道未提供论文标题或独立复现结果。

rss · 新智元 · 11月27日 03:27

**「背景」** 机器遗忘（machine unlearning）指通过训练让模型不再输出危险知识，常被用于删除黑客攻击等敏感内容，而验收时通常只看危险题目的得分是否下降。Horizon 11 月 25 日的日报曾报道，Anthropic Fellows 的研究重新主张把神经元作为可解释性分析的基本单位，并列出单个神经元常对多个无关输入放电、概念表示会跨层变化等反对意见；本次报道的两项研究则从神经元层面检验遗忘训练。

**「影响」** 这意味着，用危险题考分下降来验收遗忘训练并不可靠；依赖此类方法做安全部署的机构若要确认危险知识已移除，还需检查模型对正确答案的残余概率，并测试少量神经元恢复后知识是否重新浮现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2125365268381929637">2026-11-25 — Anthropic Fellows revisit neurons as a basis for interpretability</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#machine unlearning`, `#neural networks`, `#Anthropic`, `#model security`

---

<a id="item-tech-news-12"></a>
### [谷歌 Play 将公开商家开发者电话和地址](https://www.androidpure.com/google-play-trader-developer-address/) ⭐️ 6.0/10

谷歌 Play 宣布，自 2027 年 3 月 1 日起在全球范围向用户展示自我声明为“商家”的开发者的联系方式，包括个人账户持有者的电话号码和地址。所有活跃开发者账户须在 2027 年 2 月 1 日前申报商家或非商家身份，逾期可能无法更新应用，并从 Play 全球下架。该政策于 2026 年 10 月公布，本周因隐私担忧遭到开发者反弹；欧盟相关法规并未要求向欧盟以外用户展示这些信息。谷歌不接受邮政信箱作为付款地址，而苹果仅在欧洲相关国家展示地址并允许使用邮政信箱。

telegram · zaihuapd · 11月27日 01:44

**「背景」** Google Play 的“商家”身份由开发者自行申报，平台将据此决定是否向用户公开联系方式；该政策于 2026 年 10 月公布，本周因隐私担忧遭到开发者反弹。欧盟相关法规并未要求向欧盟以外用户展示这些信息，而苹果仅在相关欧洲国家展示地址并允许使用邮政信箱，谷歌则不接受邮政信箱作为付款地址。

**「影响」** 对个人账户持有者而言，一旦申报为商家，电话号码和地址将面向全球 Play 用户公开；需在 2027 年 2 月 1 日前完成身份申报，并注意付款地址不能使用邮政信箱，否则可能影响应用更新和全球上架。

**标签**: `#Google Play`, `#developer policy`, `#privacy`, `#app distribution`, `#regulatory compliance`

---

<a id="item-tech-news-13"></a>
### [美情报机构据报遭 Artex 辅助攻击](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 6.0/10

《纽约时报》报道并经福布斯转述称，美国中央情报局、国家地理空间情报局和国家情报总监办公室等机构遭到黑客攻击，攻击借助名为 Artex 的 AI 工具。该工具可整合多个开源 AI 模型来测试网络和计算机防御；一名中国开发者今年早些时候发布后，Artex 又被用于多起攻击，包括针对欧盟的一起，开发者已将其从 GitHub 删除。报道称此次攻击看起来不算严重，主要影响非机密侦察数据，但现有细节有限，尚无独立确认。FBI 今年早些时候曾警告，网络罪犯和间谍正在广泛使用 Artex。

telegram · zaihuapd · 11月27日 10:42

**「背景」** ARTEX 是 FBI 通报中描述的开源、由大语言模型驱动的自主渗透测试框架，可把自然语言目标转化为由 AI 代理规划和执行的渗透测试命令。据 FBI 和 Censys，开发者 Autumn-27 于 2026 年 7 月将该工具发布在 GitHub。Horizon 10 月 9 日的日报曾援引 CrowdStrike 称，ARTEX 被用于针对韩国金融机构的攻击；当前报道则称其又被用于攻击美国情报机构，但攻击严重程度和具体细节仍然有限。

**「影响」** 受影响机构需要核查非机密侦察数据的暴露范围，并评估开源 AI 工具被滥用于网络侦察的风险；现有报道未说明具体漏洞、攻击者身份或数据是否被取走。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://xcai.pro/">2026-10-09 — CrowdStrike Reports Open-Source AI Tool ARTEX Used in South Korea Financial Attacks</a></li>
<li><a href="https://www.ic3.gov/CSA/2026/261113.pdf">Threat Overview of ARTEX Autonomous Penetration Testing Framework</a></li>
<li><a href="https://ransomnews.com/artex-ai-hacking-tool-fbi-warning-2026/">ARTEX: the AI hacking tool behind the FBI warning</a></li>

</ul>
</details>

**标签**: `#AI cybersecurity`, `#cyberattack`, `#intelligence agencies`, `#open-source AI`, `#Artex`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 Intel XPU 每夜构建包（nightly-xpu）](https://github.com/LMCache/LMCache/releases/tag/nightly-xpu) ⭐️ 5.0/10

LMCache 发布了基于 \`dev\` 分支构建的 Intel XPU 每夜 wheel（\`lmcache==0.5.9.dev89+xpu\`），用于在指定的 vLLM XPU 运行时镜像内安装；本次发布未附带功能变更或性能说明。

github · github-actions\[bot\] · 11月27日 10:16

**「解决的痛点」** 这一构建主要解决“打包与部署”问题：LMCache 的 KV cache 复用能力要运行在 Intel XPU 上，需要有与 vLLM XPU 运行时环境匹配的预编译轮子，否则用户需自行从源码编译，容易出现依赖和版本不匹配。该 nightly 包给出明确的安装方式：在 \`vllm/vllm-openai-xpu\` 运行时镜像内执行 \`pip install ... --no-deps\`，并通过 \`--find-links\` 指向该 release 的扩展资源页，从而绕开依赖解析冲突、简化安装。需要注意，源内容仅包含构建时间、镜像摘要与安装命令，未提供任何功能变更、性能数据或稳定性验证，因此不能据此推断其相比其他构建有速度或内存收益。

**「背景与影响」** 这次发布是 LMCache 面向 Intel XPU 的 nightly wheel（0.5.9.dev89+xpu），构建自 \`dev\` 分支，需安装在指定的 vLLM XPU runtime image 内。它本身未提供功能变更或性能数据，意义主要在于把 LMCache 的 KV cache 复用能力以可安装的 XPU 包形式带入 vLLM 的 Intel 运行时环境。

放到更大生态看，长上下文推理的瓶颈之一是重复 prefill；LMCache 通过存储和复用 KV 状态来减少这类重复计算，并与 vLLM 集成（tool-1-2）。vLLM 侧对 KV connector 和 KV cache 内存管理有特定约束，LMCache 的多进程 connector 在部分优化配置下需要额外注意（tool-1-1）。Intel 也有面向其多 GPU 平台优化的 vLLM 分支（tool-1-3），因此 XPU 打包是该硬件路线可用性的一环。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/configuration/optimization/">Optimization and Tuning - vLLM</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/intel/llm-scaler/blob/main/vllm/README.md">llm -scaler/ vllm /README.md at main · intel / llm -scaler · GitHub</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#Intel XPU`, `#vLLM`, `#nightly release`

---

<a id="item-ai-projects-2"></a>
### [LMCache 发布 ROCm 7.2 夜间构建 wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

LMCache 发布基于 dev 分支的 ROCm 7.2 夜间构建 wheel（0.5.9.dev89+rocm7.2），面向 AMD Instinct MI300X/MI325X 与 MI350X/MI355X，并与上游 vLLM ROCm 容器（torch 2.13、cp312）保持 ABI 匹配。

github · github-actions\[bot\] · 11月27日 08:56

**「解决的痛点」** 在 AMD ROCm 环境中把 LMCache 的 KV cache 层与 vLLM 一起部署时，用户通常需要自行编译，并处理 PyTorch、CPython ABI 与上游容器镜像不一致的问题。该夜间 wheel 提供预构建包，目标是降低源码构建和依赖对齐成本；但它不包含架构变更、新能力、基准测试或修复，稳定性仍应按夜间构建看待。

**「背景与影响」** 从生态位置看，LMCache 的定位是为 LLM 推理提供 KV cache 基础设施，把 KV cache 变成可存储、压缩、检索并在集群内复用的“AI 原生内存”（tool-1-2）；它通过 LMCacheConnectorV1 以进程内方式接入 vLLM v1，也可用 YAML 配置文件和环境变量进行配置（tool-1-1）。所以这类项目的可用性不仅在算法层，还高度依赖与推理引擎及其容器镜像的打包兼容性。

本次 nightly-rocm（0.5.9.dev89+rocm7.2，2026-11-27 从 \`dev\` 构建）的实际变化是分发渠道：wheel 覆盖 gfx942（MI300X/MI325X）与 gfx950（MI350X/MI355X），并对齐上游 \`vllm/vllm-openai-rocm\` 镜像所用的 torch 2.13 与 cp312 ABI。AMD 的 ROCm vLLM Docker 镜像本身即为 MI300X/MI325X/MI350X/MI355X 提供预构建优化环境（tool-2-2），因此 ABI 对齐意味着用户可直接用 \`pip install --no-deps\` 把这层 KV cache 能力装入官方容器，无需自行从源码编译；对在 AMD Instinct 上运行 vLLM 的团队，这降低了部署摩擦。

需要保留的限定：这是滚动 nightly 产物而非正式版本，稳定性和可复现性弱于正式发布；发布说明未提及架构变更、新能力、基准数据或缺陷修复，社区也无评论，因此其价值目前主要体现在打包与部署便利性上，而非推理性能本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/examples/disaggregated/lmcache/">LMCache Examples - vLLM</a></li>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.2.4/how-to/rocm-for-ai/inference/benchmark-docker/vllm.html">vLLM inference — ROCm Documentation</a></li>

</ul>
</details>

**标签**: `#LLM`, `#inference`, `#serving`, `#KV cache`, `#vLLM`, `#ROCm`, `#AMD`, `#nightly build`, `#packaging`

---

<a id="item-ai-projects-3"></a>
### [LMCache 发布面向 Rebellions RBLN NPU 的 nightly wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

LMCache 发布面向 Rebellions RBLN NPU 的 nightly wheel，基于 dev 构建并适配 torch-rbln 0.12.0，用于在 RBLN 环境分发 KV 缓存层。

github · github-actions\[bot\] · 11月27日 09:50

**「解决的痛点」** 它解决的是 LMCache 在 Rebellions RBLN NPU 上的可用性与安装集成问题：以预构建 wheel 形式提供，避免用户自行从源码打包；torch-rbln、rebel-compiler 和 RBLN 驱动仍由宿主环境提供，wheel 不捆绑。该发布未说明性能、API 或架构层面的改进。

**「背景与影响」** LMCache 的定位是为 LLM 推理提供 KV cache 管理/复用层，把 KV cache 从临时状态变为可持久化、可跨推理引擎复用的数据，以降低首 token 延迟并提升吞吐（tool-1-1、tool-1-3）。其论文也指出，将 KV cache 移出 GPU 设备、支持跨查询和推理引擎复用正成为实际需求（tool-1-2）。此次 nightly-rbln 是面向 Rebellions RBLN NPU 的夜间打包产物：基于 dev 分支、针对 torch-rbln 0.12.0（torch 2.13.0+cpu）构建，torch-rbln、rebel-compiler 和 RBLN 驱动仍由宿主机提供，不打入 wheel。它本身未声明性能、API 或架构变化，因此更像是对新增硬件后端的例行构建，而非功能版本。放到生态中看，torch-rbln 以 PyTorch 扩展方式提供 rbln 设备和 torch.compile 接口，并依赖 rebel-compiler/runtime（tool-2-1、tool-2-2）；Rebellions 也提供 RBLN SDK 用于编译、运行时和部署（tool-2-3）。因此该 wheel 的意义在于让 LMCache 的 KV cache 层覆盖 NPU 部署路径，但实际可用性取决于宿主工具链是否就绪，不能据此推断性能收益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">GitHub - RBLN-SW/torch-rbln: PyTorch extension for Rebellions NPU</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch-rbln · PyPI</a></li>
<li><a href="https://rebellions.ai/developers/">Developers - Rebellions</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#inference`, `#NPU`, `#RBLN`, `#nightly build`, `#packaging`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [国常会部署稳市：加力发挥“国家队”作用，优化中央汇金类“平准基金”功能](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 8.0/10

11 月 27 日召开的国务院常务会议由总理李强主持，会议提出持续完善资本市场稳市机制，加力发挥“国家队”稳市作用，进一步优化中央汇金公司的类“平准基金”功能并提供充足流动性保障；同时要求推动上市公司加大分红回购力度，完善保险、企业年金、社保基金等中长期资金入市支持引导政策。上述内容属于会议的方向性部署，未公布具体金额、时间表或实施细则。

telegram · zaihuapd · 11月27日 05:35

**「背景」** “国家队”指参与稳定资本市场的国有资金，中央汇金公司是此次会议点名的机构；“类‘平准基金’”指通过逆向买卖平抑市场波动的公共资金安排，有专家解读称，此次优化中央汇金这一功能意味着中国版“平准基金”从危机应对的临时工具升格为常设机制。

**「影响」** 若相关部署逐步落实，将改变上市公司的分红回购行为，并影响保险资金、企业年金和社保基金的权益资产配置，同时加大对财务造假、违规减持的查处力度；但目前尚无量化目标与执行时间，实际影响仍待具体政策出台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.eastmoney.com/a/202611273941634358.html">如何理解 国 常会对资本 市 场的最新定调？ 专 家 解读来了 _ 东方财富网</a></li>

</ul>
</details>

**标签**: `#China policy`, `#capital markets`, `#Central Huijin`, `#market stabilization`, `#securities regulation`

---

<a id="item-finance-news-2"></a>
### [央行发布大额存单新规：个人认购起点降至 10 万元](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

中国人民银行 11 月 27 日公布《大额存单管理办法》，将个人投资人认购起点从原暂行办法的 20 万元下调至 10 万元，机构投资人从 1000 万元下调至 500 万元，均减半，新规自 2027 年 3 月 21 日起施行。同日央行还发布经 10 月 30 日行务会审议通过、行长潘功胜 11 月 26 日签发的《人民币存贷款利率管理规定》，同样自 2027 年 3 月 21 日起施行，要求金融机构自主确定存贷款利率，不得以高息揽储等不正当手段吸收存款。

telegram · zaihuapd · 11月27日 11:36

**「背景」** 大额存单是银行面向个人和机构发行的大额存款凭证，现行认购门槛来自 2015 年《大额存单管理暂行办法》，即个人 20 万元、机构 1000 万元；新《大额存单管理办法》施行后，将同时废止该暂行办法和 2016 年第 13 号公告。

**「影响」** 新规生效后，原先达不到 20 万元门槛、但资金超过 10 万元的个人将可以购买大额存单，银行面向个人的大额存单潜在客户范围相应扩大。

**标签**: `#大额存单`, `#央行监管`, `#存款利率`, `#银行负债`, `#个人理财`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Paul Graham：创业公司的“合作”多半是浪费时间](https://x.com/paulg/status/2126462588766527593) ⭐️ 6.0/10

Paul Graham 在 X 上表示，对创业公司来说， partnerships（合作关系）通常是浪费时间。他认为，真正值得做的只有两种“退化情形”：买别人的产品，或别人买你的产品。他同时指出，这类交易通常不会被称为“合作”；当需要动用这个特殊名称时，反而是一个坏信号。

twitter · Paul Graham · 11月27日 23:46

**「背景」** 这是 Paul Graham 于 2026 年 11 月 27 日发布的一则简短创业建议，属于面向创始人的经验判断，而非研究论文或新闻报道。其核心是用命名习惯作启发式：把含糊的“合作”与明确的采购、销售关系区分开。原文没有展开具体案例、适用条件或反例，因此更适合理解为一条便于记忆的判断框架，而不是对所有合作形式的普遍结论。

**标签**: `#startups`, `#business-strategy`, `#partnerships`, `#founder-advice`, `#opinion`

---