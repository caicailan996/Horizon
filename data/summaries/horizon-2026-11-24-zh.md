# Horizon 每日速递 - 2026-11-24

> 从 42 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [Anthropic 仓库论文声称 VP ≠ VNP 对所有域成立](#item-tech-news-1) ⭐️ 9.0/10
2. [Ladybird 浏览器引擎进入 Alpha 阶段](#item-tech-news-2) ⭐️ 8.0/10
3. [智谱 GLM-5.4：首个循环 Transformer 面向通用编程](#item-tech-news-3) ⭐️ 8.0/10
4. [Codex2api 疑似遭供应链投毒，3.1.10–3.1.12 受影响](#item-tech-news-4) ⭐️ 8.0/10
5. [英伟达董事会重新任命黄仁勋为 CEO](#item-tech-news-5) ⭐️ 7.0/10
6. [Windows Server 2028 默认移除 WoW64，32 位应用需手动装回](#item-tech-news-6) ⭐️ 7.0/10
7. [Arm 要求关闭非官方文档站，网站定于 12 月 4 日停运](#item-tech-news-7) ⭐️ 6.0/10
8. [Kagi Mail 进入公测，AI 与隐私取舍受关注](#item-tech-news-8) ⭐️ 6.0/10
9. [Nospeaker：用 MacBook 触控板马达朗读文字](#item-tech-news-9) ⭐️ 6.0/10
10. [FSNotes 称遭 Apple 从欧盟 App Store 下架](#item-tech-news-10) ⭐️ 6.0/10
11. [谷歌被曝用模拟互联网测试 Chrome AI 代理](#item-tech-news-11) ⭐️ 6.0/10
12. [Meta AI 负责人称超级智能临近，警告控制风险](#item-tech-news-12) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 RBLN NPU 夜间构建轮子](#item-ai-projects-1) ⭐️ 6.0/10
2. [LMCache 发布 nightly CUDA 13.0 wheel 构建](#item-ai-projects-2) ⭐️ 5.0/10

**财经新闻**
1. [蚂蚁集团领投 Simplexity Robotics 1 亿美元 pre-A 轮，投后估值 16 亿美元](#item-finance-news-1) ⭐️ 7.0/10
2. [Anthropic IPO 后 AI 股抛售，中国 AI 公司上市计划承压](#item-finance-news-2) ⭐️ 7.0/10
3. [上海地铁 12 月 1 日起实施 21 年来首次票价调整](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 仓库论文声称 VP ≠ VNP 对所有域成立](https://github.com/anthropics/formal-math/tree/main/vp-vnp) ⭐️ 9.0/10

Anthropic 的 formal-math 仓库发布了一篇论文，声称证明了 VP ≠ VNP 对所有域成立；这是代数复杂性理论中一个与 P vs NP 相关的分离命题，但论文尚未经过同行评审，也未在现有材料中获得独立验证。当前能确认的是论文已被公开在仓库中，而不是该结论已被数学界接受或证明成立。若证明经过审查，它将构成代数复杂性理论的重要结果；在得到独立验证前，应将其视为待检验的声明。

hackernews · mikeryan52 · 11月23日 22:09 · [社区讨论](https://news.ycombinator.com/item?id=50620102)

**「背景：Valiant 猜想与 Lean 形式化潮流」** VP 与 VNP 是代数复杂度理论中的一对复杂度类，VP ≠ VNP 作为「Valiant 猜想」自 1979 年起悬而未决，通常被看作 P vs NP 问题在代数框架下的对应版本。此前 11 月 21 日的日报曾报道，Anthropic 数学家 Levent Alpöge 声称借助 Claude 完成了以 Lean 编码发布的黎曼假设证明；本次引发讨论的论文同样出现在 Anthropic 的 formal-math 仓库中，附带 Lean 4 形式化，而仓库自述尚无职业数学家检查过该证明。

**「验证路径与未解的屏障问题」** 对需要评估这一结论的复杂性理论研究者而言，最直接的着力点是：该结果以 Lean 形式化源码与 PDF 一同发布，读者可以先行构建并检查形式化证明，而不必等待同行评审。但评论者引用论文原文指出，作者尚未分析该结果与相对化（relativization）及算术化（algebrization）屏障的关系；在对这两项针对复杂性分离的标准检验作出说明之前，不宜把 VP ≠ VNP 视为已确立的结论。

**「社区讨论」** Hacker News 评论把这项工作看作 Anthropic 朝 P vs NP 这类“圣杯”问题推进的阶段性成果，也有人引用论文自述指出其尚未分析该结果与相对化、代数化的关系。另有评论表达了对 AI 可能迅速解决基础数学问题的焦虑，这些属于个人判断而非对证明的验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">2026-11-21 — Anthropic mathematician claims Claude-assisted Riemann hypothesis proof in Lean</a></li>
<li><a href="https://news.lavx.hu/article/anthropic-publishes-claimed-proof-that-vp-vnp-over-every-field">Anthropic Publishes Claimed Proof That VP ≠ VNP Over Every Field</a></li>
<li><a href="https://www.techflowpost.com/en-US/newsletter/146433">Anthropic Announces Claude Model’s Proof of VP ≠ VNP; Yet to ...</a></li>

</ul>
</details>

**标签**: `#VP vs VNP`, `#algebraic complexity`, `#complexity theory`, `#formal math`, `#Lean`

---

<a id="item-tech-news-2"></a>
### [Ladybird 浏览器引擎进入 Alpha 阶段](https://ladybird.org/posts/alpha/) ⭐️ 8.0/10

Ladybird 项目宣布进入 Alpha 阶段，这是一个从零编写的独立浏览器引擎首次面向试用者发布早期版本。它目前仍属 Alpha 软件，尚无广泛采用，稳定性和兼容性不能按正式版标准预期。社区早期试用称多个网站可以正确渲染，但也报告页面滚动和部分交互存在卡顿。

hackernews · janvdberg · 11月23日 16:13 · [社区讨论](https://news.ycombinator.com/item?id=50614249)

**「背景：从零编写的非营利浏览器引擎」** Ladybird 是一个从零开始编写的浏览器引擎，并非 Chromium 或 Firefox 的分支，由一家 501\(c\)\(3\) 非营利基金会支持，采用自由开源的许可方式（tool-2-1）。其官网列出的 alpha 版本目前面向 macOS 和 Linux 提供（tool-2-1）。正因为渲染与网页兼容性需要自行实现，而非继承现有引擎的成熟代码，其站点兼容程度才成为此次 alpha 发布被检验的重点。

**「影响」** 对希望测试非 Chromium/Gecko 内核的开发者而言，现在有了一个可实际加载网站的新引擎样本；但 Alpha 状态意味着兼容性和稳定性仍可能变化，针对它做的网站适配结论只适用于当前早期版本。

**「社区讨论」** 评论者对从零实现的引擎能渲染大量网站表示惊讶，称 YouTube、Google Maps、Proxmox 界面和 NoVNC 等可用，但也提到滚动和交互仍有卡顿。另有评论惋惜项目改用 SQLite、Skia 等成熟依赖，并询问 Alpha 阶段是否应避免登录、支付和下载等操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ladybird.org/">Ladybird is a truly independent web browser , backed by a non-profit.</a></li>

</ul>
</details>

**标签**: `#Ladybird`, `#browser engine`, `#alpha release`, `#open source`, `#web rendering`

---

<a id="item-tech-news-3"></a>
### [智谱 GLM-5.4：首个循环 Transformer 面向通用编程](https://z.ai/blog/glm-5.4) ⭐️ 8.0/10

智谱发布 GLM-5.4，称这是其首个循环 Transformer（looped transformer），目标是提升通用编程能力。目前可获得的材料只有博客标题和社区讨论，尚未披露模型参数、基准成绩或许可证等具体细节。

hackernews · foohis · 11月23日 10:06 · [社区讨论](https://news.ycombinator.com/item?id=50609685)

**「背景」** 循环 Transformer 的核心思路是让同一组共享层在推理时反复执行多次，以增加有效计算深度，而不是为每一步都堆叠独立权重；Horizon 2026 年 10 月 13 日的日报曾报道，Looped Diffusion Transformer 在每次去噪步骤内重复运行共享块，并用深层监督和自调制注意力解决朴素循环效果不稳定的问题（tool-1-3）。GLM-5.4 接替 Z.ai 此前的开放权重模型 GLM-5.3；Horizon 2026 年 9 月 30 日的日报曾记录 Anthropic 对 GLM-5.3 的网络安全能力评估（tool-1-1）。Z.ai 官方文档称 GLM-5.4 是首个基于 Loop Transformer 架构的旗舰模型，并称其智能水平可对标 2T–3T 参数模型（tool-2-2）。

**「影响」** 对想试用 GLM-5.4 的开发者来说，现有接入路径受限：有社区用户报告，该模型不在 OpenRouter 或常规 Z.ai API 套餐中，必须改用 Coding Plan，而后者签发的 API 密钥与常规密钥用法相同。

**「社区讨论」** 有评论者赞赏智谱公开较多技术细节，认为循环 Transformer 是明确的发展方向，并解释了它针对的正是推理时逐层搬运权重造成的内存带宽瓶颈。另一名用户则抱怨部分中国模型在简单任务上也会进行冗长的“马拉松式思考”，导致完成时间明显长于前沿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">2026-09-30 — Anthropic finds GLM-5.3 can build end-to-end cyberattacks near Claude Mythos</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/">2026-10-13 — Looped Diffusion Transformer trades compute for refinement at sampling time</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.4">GLM - 5 . 4 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**标签**: `#LLM architecture`, `#looped transformers`, `#coding models`, `#GLM-5.4`, `#model release`

---

<a id="item-tech-news-4"></a>
### [Codex2api 疑似遭供应链投毒，3.1.10–3.1.12 受影响](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

Codex2api 疑似遭遇供应链投毒：作者账号被黑后，攻击者绕开 main 分支推送 tag，使 Release 构建出带后门的版本。事件复盘称，v3.1.11 移除了鉴权，等同于可无密码远程执行命令；另有 workflow 将仓库的 16 个 GitHub Actions secrets 外传，波及同一账号下至少 21 个仓库。已安装或更新到 3.1.10–3.1.12 的用户被建议立即停用、回退到 3.1.9，并轮换 GitHub token、SSH key、数据库及 DeepSeek 等相关密钥。该事件目前仍被描述为“疑似”，相关细节尚待进一步确认。

telegram · zaihuapd · 11月23日 11:21

**「背景」** 供应链投毒是指攻击者篡改用户会下载的发布物或构建流程，而不是直接攻击每个使用者。Codex2api 的发布方式是通过推送 Git tag 来触发 Release 构建；由于 main 分支保护无法阻止这种绕过合并审查的发布方式，攻击者一旦拿到作者账号，就可以直接产出带后门的版本。该仓库的 GitHub Actions workflow 还保存了 16 个 secrets，这些 secrets 的权限覆盖同一账号下至少 21 个仓库；因此，workflow 一旦被篡改，相关凭据就可能被外传。

**「处置影响」** 已安装或升级到 3.1.10–3.1.12 的部署应立即停用服务并回退到 3.1.9，因为 v3.1.11 移除了鉴权，等同于允许无密码远程执行命令。由于恶意 workflow 已外传仓库的 16 个 Actions secrets，且波及同账号下至少 21 个仓库，仅更换应用自身的口令不足以止损，需一并轮换 GitHub token、SSH key、数据库及 DeepSeek 等相关凭据。该事件目前被描述为“疑似投毒”，在官方确认前，最稳妥的做法是把相关密钥视为已泄露处理。

**标签**: `#supply-chain-attack`, `#security`, `#GitHub-Actions`, `#backdoor`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [英伟达董事会重新任命黄仁勋为 CEO](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 7.0/10

据该条目链接的英伟达新闻稿，英伟达董事会重新任命黄仁勋（Jensen Huang）为总裁、首席执行官兼董事会董事。董事会声明称，在作出决定过程中“收到了美国联邦政府高层人士的意见”，并据此确信黄的复职“不构成国家安全风险”。该条目本身仅包含新闻稿与 CNBC 报道两个链接，未提供复职的具体条款、时间安排，也未说明此前的职务变动细节，相关原因仍待更多信源确认。

hackernews · jaz · 11月23日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=50611576)

**「背景」** Horizon 11 月 9 日的日报曾报道，英伟达董事会当时调查的是一起针对黄仁勋的情报活动，而非黄本人；11 月 16 日的日报又回顾称，公司已于 11 月 12 日宣布黄仁勋辞去 CEO 和董事职务，由 CFO Colette Kress 担任临时 CEO，且黄已就回归与亲信接触。此次复职发生在上述辞职不到两周后。

**「监管与立法压力」** 黄仁勋复职后，Nvidia 立即被推回美国出口管制立法争论的中心：相关表态称，黄的回归只会增加国会通过两党出口管制法案的紧迫性，并要求 Nvidia 不要游说阻挠该法案。对依赖其 GPU 的客户而言，若相关立法推进，采购与合规安排将面临新的不确定性。

**「社区讨论」** 评论者普遍认为，董事会声明中“收到美国政府高层意见”一句才是关键，而非人事决定本身。有评论者援引特拉华州 Caremark 判例的高归责门槛，并结合其所称司法部不予起诉的表态，推测董事的个人责任可能因此被排除；同一评论者还对董事会在不到两周内从“迅速迫使黄离职”转为一致同意复职表示意外。另有评论者批评，美国在要求 ASML 及日本芯片企业遵守对华制裁的同时，却让英伟达获得白宫的“个人祝福”，属于明显的双重标准。以上均为评论者观点，未获条目所附材料证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/dotey/status/2122062085807030716">2026-11-16 — Report: Jensen Huang Considering Return as NVIDIA CEO</a></li>
<li><a href="https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors">2026-11-09 — Nvidia Board Probes Intelligence Operation Targeting CEO Jensen Huang</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/live/nvidia-live-updates-jensen-huang-reinstated-as-ceo-trump-says-no-reason-to-believe-huang-a-national-security-risk-152429808.html">Nvidia live updates: Jensen Huang reinstated as CEO; Trump says...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#semiconductors`, `#corporate governance`, `#US government`, `#tech industry`

---

<a id="item-tech-news-6"></a>
### [Windows Server 2028 默认移除 WoW64，32 位应用需手动装回](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 7.0/10

微软在 Ignite 2026 上宣布，Windows Server 2028 将默认不包含 WoW64 兼容子系统，因此开箱无法运行 32 位应用；该版本计划于 2027 年秋季与 Windows 11 27H2 一同发布。需要兼容 32 位软件的服务器可通过按需功能（FoD）装回 WoW64，在 Server Core 上通常使用 PowerShell 或 DISM 添加。微软称此举旨在减少攻击面并阻止 32 位恶意软件；Windows 11 目前仍保留 WoW64，微软未公布移除计划。

telegram · zaihuapd · 11月23日 03:03

**「背景：WoW64 是什么」** WoW64（Windows 32-bit on Windows 64-bit）是 Windows 的兼容子系统，负责让 64 位系统运行 32 位 x86 应用；没有它，这类程序在 64 位 Windows 上无法启动。此次变化把这一层从“默认内置”改为“按需功能”：管理员需要用 PowerShell 或 DISM 手动加回，才能继续在服务器上运行旧的 32 位软件。

**「影响」** 企业 IT 在升级或新建 Windows Server 2028 前需要盘点 32 位应用依赖，并在镜像或部署流程中预置 WoW64 按需功能，否则相关应用在默认安装上无法启动；Server Core 环境还需准备 PowerShell 或 DISM 的安装步骤。

**标签**: `#Windows Server`, `#WoW64`, `#32-bit compatibility`, `#Microsoft`, `#enterprise IT`

---

<a id="item-tech-news-7"></a>
### [Arm 要求关闭非官方文档站，网站定于 12 月 4 日停运](https://arm.jonpalmisc.com/) ⭐️ 6.0/10

非官方 Arm 文档网站 arm.jonpalmisc.com 宣布，应 Arm 的要求将于 2026 年 12 月 4 日停止运营。网站运营者 jonpalmisc 在 Hacker News 上表示，Arm 以该站托管其文档、使用其商标和知识产权为由要求移除内容；他认为在不影响网站可用性的前提下很难规避这一要求。该站并非 Arm 官方资源，运营者称正在研究他人提出的镜像托管、寻求律师和发布不含 Arm 知识产权源代码等选项。

hackernews · tech234a · 11月23日 19:17 · [社区讨论](https://news.ycombinator.com/item?id=50617499)

**「背景」** 该站点是开发者 jonpalmisc 维护的非官方 Arm 文档站，将 Arm 的架构参考文档整理为便于在线查阅的形式。站主在讨论中说明，Arm 要求下架的理由是他托管这些文档时使用了 Arm 的商标和知识产权，而在保持站点可用性的前提下，这一点很难规避；他表示会评估他人提出的镜像托管、寻求法律意见，以及剥离 Arm 内容后公开生成站点源码等方案。

**「对使用者的影响」** 对依赖该站查阅 Arm 文档的开发者而言，现有链接将在停运后失效；在镜像或可自建版本真正上线前，他们需转而使用 Arm 官方文档或其他既有副本。运营者尚未确认任何替代方案，因此访问便利性和长期可用性仍不确定。

**「社区讨论」** Hacker News 评论者质疑 Arm 的做法：有人追问记载硬件是否应属合理使用，也有人批评法律行动会给最终为 Arm 创造价值的开发者添麻烦。另有评论指出该站页面与斯坦福大学服务器上的 Arm64 文档页面相似，并猜测二者可能由同一类转换工具生成；这些是评论者的判断，未获 Arm 或运营者确认。

**标签**: `#Arm`, `#documentation takedown`, `#intellectual property`, `#hardware documentation`, `#open access`

---

<a id="item-tech-news-8"></a>
### [Kagi Mail 进入公测，AI 与隐私取舍受关注](https://blog.kagi.com/kagi-mail-public-beta) ⭐️ 6.0/10

Kagi 宣布 Kagi Mail 进入公开测试，这是其现有订阅产品之外的一次邮件服务扩展。现有材料没有给出定价、存储容量、协议兼容性、正式上线时间，也没有说明 AI 功能的具体范围和数据保留政策。因此目前只能确认公测状态，无法独立核实其隐私承诺或 AI 处理边界。

hackernews · rdmuser · 11月23日 17:17 · [社区讨论](https://news.ycombinator.com/item?id=50615481)

**「背景」** Kagi 此前以订阅制、强调隐私的搜索服务和 Orion 浏览器建立用户群；其博客把邮箱描述为用户数字生活中仍被 Google 占据的“最后一大块”。Kagi Mail 因此把 @kagimail.com 或自有域名邮箱与日历一起纳入 Kagi 生态。

**「迁移前需接受的取舍」** 对考虑迁移的用户而言，最具体的代价是定价与加密状况：据 Privacy Affairs 报道，Kagi Mail 公开测试版定价为每年 99 美元，且不提供端到端加密，Kagi 也未公布其 AI 功能所依托的模型供应商，这意味着邮件内容在服务端可被读取、并可能交由第三方模型处理，对加密有硬性要求的用户需自行评估这一条件。另一项可核实的差异是，Kagi 文档称跟踪像素剥离与图片经 Kagi 图片代理加载会在使用任何邮件客户端访问 Kagi Mail 时生效，并不绑定其自家客户端。

**「社区讨论」** 有 Kagi 用户表示自己用 Fastmail 已足够，明确不会让云端 LLM 读取邮件；另一位 Duo 订阅者担心功能蔓延拖累搜索和翻译等核心服务，并称翻译质量下降且被限制。还有评论认为 Kagi 过去以少存用户数据为特点，做邮箱可能改变这一定位，并提醒邮箱是银行、医疗等账号恢复的关键入口，选择小众提供商需考虑可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.kagi.com/kagi-mail-public-beta">Kagi Blog - Kagi Mail is here (Public Beta)</a></li>
<li><a href="https://www.privacyaffairs.com/kagi-mail-public-beta/">Kagi Mail Public Beta: $99 a Year, No End-to-End Encryption</a></li>
<li><a href="https://help.kagi.com/kagi/mail/">Kagi Mail FAQ | Kagi&#x27;s Docs</a></li>

</ul>
</details>

**标签**: `#Kagi Mail`, `#email`, `#privacy`, `#AI integration`, `#product launch`

---

<a id="item-tech-news-9"></a>
### [Nospeaker：用 MacBook 触控板马达朗读文字](https://github.com/os6/nospeaker) ⭐️ 6.0/10

开发者 Cody Collier 开源了 Nospeaker，它调用 macOS 语音合成，把文字拆成每 10 毫秒两个共振峰及响度、音高参数，驱动 MacBook 触控板下的触觉马达以最高每秒 4000 次振动，让玻璃发出可听语音。该工具实测在 100 Hz 至 4 kHz 有声，1 kHz 附近最清晰，听感偏机器人；它只能朗读文字，不能播放音乐或视频。实现上它绕过苹果公开的触觉接口，改用私有框架 MultitouchSupport。项目需要 Force Touch 触控板，作者称目前只在 M5 Max 的 MacBook Pro 上跑通。

hackernews · yakkomajuri · 11月23日 11:31 · [社区讨论](https://news.ycombinator.com/item?id=50610318)

**「背景」** MacBook 的 Force Touch 触控板本身并不会真的被按下，它靠触觉马达（Taptic Engine）振动来模拟“咔哒”的点击手感；而苹果并未公开允许第三方任意驱动这颗马达的接口。此前已有 macos-haptic、M5MultitouchSupport 等开源项目通过调用私有的 MultitouchSupport 框架来读取触控板数据并触发振动，这类依赖也被指出可能因 macOS 更新而失效。Nospeaker 正是沿这条路径，把原本用于点击反馈的马达推到可听频段来发声。

**「影响」** 对想试用的开发者而言，Nospeaker 依赖私有 MultitouchSupport 框架和 Force Touch 硬件，不能当作稳定的公开 API 方案；作者也仅报告在 M5 Max MacBook Pro 上验证通过，其他机型与后续 macOS 版本的兼容性尚未确认。

**「社区讨论」** 评论者把这一做法与老式硬件发声 hack 相比较：有人提到 Commodore 1541 软驱马达曾被用来播放音频甚至生成视频，也有人回忆 PC 压电蜂鸣器播放音乐。RossBencina 则推测苹果触觉 API 采用正弦和表示，可能是为了避免烧坏马达、便于逐分量补偿执行器动态，或降低 USB/HID 传输带宽，并称想观察 Nospeaker 运行时的 USB 流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/crnicholson/macos-haptic/">GitHub - crnicholson/macos-haptic: Control the haptic ...</a></li>
<li><a href="https://github.com/mhuusko5/M5MultitouchSupport">GitHub - mhuusko5/M5MultitouchSupport: [Maintained] [macOS ... OpenMultitouchSupport on CocoaPods.org This Developer Made a MacBook Trackpad Talk. The Speakers ... Handling Trackpad Events - Apple Developer Accessing raw multitouch trackpad data (MacOS) · GitHub This insane trick turns the MacBook’s trackpad into a speaker</a></li>

</ul>
</details>

**标签**: `#haptics`, `#hardware-hacking`, `#macOS`, `#trackpad`, `#reverse-engineering`

---

<a id="item-tech-news-10"></a>
### [FSNotes 称遭 Apple 从欧盟 App Store 下架](https://github.com/glushchenko/fsnotes/discussions/2056) ⭐️ 6.0/10

开源笔记应用 FSNotes 的开发者称，Apple 在应用上架约九年后将其从欧盟区 App Store 移除；目前该应用仍在美国和英国区提供。现有讨论把原因指向欧盟《数字服务法》的商家身份（trader status）核验，而不是应用功能或安全问题，但 Apple 尚未在给定材料中确认具体原因。

hackernews · fluder · 11月23日 18:48 · [社区讨论](https://news.ycombinator.com/item?id=50616933)

**「背景：欧盟 DSA 交易者身份要求」** 欧盟《数字服务法》（DSA）要求面向欧盟用户提供应用的开发者声明其“交易者”（trader）身份，并公开名称、地址、邮箱和电话等联系信息；未完成声明或声明失效的应用会被从欧盟各国家/地区的 App Store 移除。据苹果帮助文档与第三方指南，苹果自 2024 年 10 月 16 日起把交易者身份作为在欧盟提交应用更新的前置条件，开发者可在 App Store Connect 的“App 合规”页面查看和修改该状态。

**「对开发者的影响」** 对在欧盟分发应用的独立开发者而言，这是一次合规中断而非代码问题：需要确保商家身份声明和联系地址持续有效，并在收到 Apple 核验要求时及时处理，否则应用可能只在欧盟区不可用。

**「社区讨论」** 评论者指出该应用仍在美英区上架，并援引荷兰区缓存页面称开发者“未声明为商家”，还提醒商家验证可能因地址变更等失效。也有人认为开源身份与合规义务无关，收费应用应尽早完成验证；另有开发者称近期同类审核约需一个月。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ivryn.com/guides/app-store-dsa-trader-status/">App Store DSA trader status for EU apps : Feb 2025 | IVRYN</a></li>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act trader requirements ...</a></li>
<li><a href="https://orbitkit.io/blog/eu-dsa-trader-status-app-store/">EU DSA trader status : the App Store trader requirements ... | OrbitKit</a></li>

</ul>
</details>

**标签**: `#EU DSA`, `#Apple App Store`, `#open-source software`, `#app distribution`, `#developer compliance`

---

<a id="item-tech-news-11"></a>
### [谷歌被曝用模拟互联网测试 Chrome AI 代理](https://www.landian.news/archives/128701.html) ⭐️ 6.0/10

据蓝点网报道，谷歌为 Chrome 的 AI 代理搭建了一个名为 Mirror Dimension 的模拟互联网，用于在隔离环境中测试它打开网站、搜索浏览、登录、加购和完成任务等操作。报道称，该环境包含数千个模拟网站；每名工程师单独隔离测试，每天运行超过 1000 个测试案例。测试重点包括防御恶意网页的提示词注入等攻击。上述细节来自一篇简短的二手报道；所给材料未包含谷歌的确认，也未公布该代理的版本或上线时间。

telegram · zaihuapd · 11月23日 01:30

**「背景」** 浏览器 AI 代理与普通网页浏览不同：它要依据页面内容自行决定点击、登录、加购等动作，因此恶意页面只要把隐藏指令混入页面，就可能形成提示词注入并劫持代理行为。要测试这类防御，需要在不会影响真实账户和交易的受控环境中复现大量网站与攻击场景；谷歌安全团队称，Mirror Dimension 就是由 Chrome 团队完全控制的合成网络，用于在接近真实但隔离的在线环境中安全评估代理的防御能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents : Evaluating Browser-Use Agents ...</a></li>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘ Mirror Dimension ’ Internet to Test Its Chrome ...</a></li>

</ul>
</details>

**标签**: `#Chrome AI agent`, `#browser automation`, `#prompt injection`, `#AI security`, `#Google`

---

<a id="item-tech-news-12"></a>
### [Meta AI 负责人称超级智能临近，警告控制风险](https://thenextweb.com/news/metas-ai-chief-says-superintelligence-is-arriving-and-control-is-at-risk) ⭐️ 6.0/10

Meta 首席 AI 官、超级智能实验室负责人 Alexandr Wang 在 X 发长文称，超级智能已不再是“未来某天”的议题，并警告人类可能难以控制可无限自我改进或比自己聪明 1000 倍的系统。他援引数学家 Levent Alpöge 借助 Anthropic 的 Claude 完成、并于周六经 Lean 与 Mathlib 社区机器校验的黎曼猜想证明，称 AI 与顶尖人类之间只剩具体知识、工程整合和实验三方面差距。不过，该证明目前没有人类可读版本，来源也只是简短二手报道，因此应视为 Wang 的援引和主张，而非已确认的数学突破；他同时呼吁紧急投入安全、对齐与防护研究。

telegram · zaihuapd · 11月23日 12:49

**「背景」** Horizon 11 月 21 日的日报曾报道，Anthropic 数学家 Levent Alpöge 于 11 月 20 日声称与 Claude 共同证明了黎曼猜想，并以 Lean 代码形式发布论证；Lean 是让数学论证可被机器逐行校验的证明辅助语言，这使得该主张具备可检验的形式，而不只是一篇论文（tool-1-2）。当时社区提到配套的 Lean 形式化约 1500 万行、约 1.3 GB，分 14 个部分分发（tool-1-3），随后 Lean FRO 与 Mathlib 计划发表联合声明，确认这份 Lean 库正确陈述并证明了黎曼猜想（tool-3-2）。Wang 的长文正是把这一经机器校验的结果当作超级智能临近的论据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">2026-11-21 — Anthropic mathematician claims Claude-assisted Riemann hypothesis proof in Lean</a></li>
<li><a href="https://alpo.ge/remark.pdf">2026-11-21 — Levent Alpöge claims Generalized Riemann Hypothesis proof with Lean formalization</a></li>
<li><a href="https://officechai.com/ai/lean-community-certifies-levent-alpoges-claude-assisted-proof-of-the-riemann-hypothesis-as-correct/">Lean Community Certifies Levent Alpöge’s Claude-Assisted ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#superintelligence`, `#Lean/Mathlib`, `#Meta AI`, `#AI-assisted proof`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 RBLN NPU 夜间构建轮子](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 6.0/10

LMCache 发布面向 Rebellions RBLN NPU 的夜间构建 wheel（0.5.9.dev13+rbln），基于 dev 分支于 2026-11-23 构建，对应 torch-rbln 0.12.0（torch 2.13.0+cpu）。

github · github-actions\[bot\] · 11月23日 09:25

**「解决的痛点」** 此前 LMCache 的 KV cache 复用能力主要围绕通用 GPU 生态，非 NVIDIA 的 NPU 平台缺少可直接安装的构建产物，需自行从源码编译并对齐 torch 版本。该 nightly wheel 提供按平台预编译、并与指定 torch-rbln 版本绑定的安装包，降低了在 RBLN NPU 上试用 LMCache 的部署门槛。需注意 torch-rbln、rebel-compiler 与 RBLN 驱动仍由宿主机自行提供、未打包进 wheel，因此安装前须先准备对应依赖环境；这是打包层面的适配，源码中未给出架构或性能层面的说明。

**「背景与影响」** LMCache 定位为 LLM 推理的模块化 KV cache 层，核心是把 KV cache 从 GPU 临时状态扩展为可跨 GPU、CPU 和外部后端存储、复用、压缩、检索与观测的资源，从而降低首 token 延迟并提升长上下文、多请求复用场景的吞吐 \[tool-1-1\]\[tool-1-3\]。传统上 KV cache 常驻 GPU 显存；随着复用需求和缓存总量增长，将其移出 GPU、在不同查询和推理引擎间共享已成趋势 \[tool-1-2\]。此次 nightly-rbln 并非架构级功能发布，而是面向 Rebellions RBLN NPU 的平台专用构建：基于 dev 分支、针对 torch-rbln 0.12.0（torch 2.13.0+cpu）打包，torch-rbln、rebel-compiler 和 RBLN 驱动仍由宿主机环境提供，wheel 不内置。RBLN 生态本身依赖专用 SDK 和编译产物 \[tool-2-2\]，因此该包的实际意义是让已有 RBLN 软件栈的环境可以直接安装 LMCache，把 KV cache 层延伸到 NPU 推理路径；但由于缺少性能数据和实现细节，目前只能视为可用性扩展，影响中等。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://huggingface.co/iAcloud/gemma4-31B-it-rbln-tp16">iAcloud/gemma4-31B-it- rbln -tp16 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly build`

---

<a id="item-ai-projects-2"></a>
### [LMCache 发布 nightly CUDA 13.0 wheel 构建](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 于 2026-11-23 从 dev 分支构建并发布 nightly wheel，覆盖 linux/amd64 与 linux/arm64，基于 CUDA 13.0。该发布只提供打包与安装说明，未包含功能、优化或性能相关信息。

github · github-actions\[bot\] · 11月23日 09:52

**「解决的痛点」** 本次发布解决的主要是安装与构建上的摩擦，与模型推理性能无关：用户在 CUDA 13.0 环境中往往需要自行编译带有 CUDA 扩展的包，耗时且容易因工具链版本不匹配而失败。该 nightly 提供预编译 wheel，并配合 PyTorch 的 cu130 软件源；用户用一条 uv pip 命令即可完成安装，从而跳过源码编译环节。需要注意，来源没有说明这次构建对 LMCache 自身的 KV cache 复用能力做了任何改动，因此无法据此判断它是否带来性能或功能上的改善。

**「生态位置与本次发布的意义」** LMCache 是一个面向 LLM 推理的开源 KV cache 管理/复用层，把 KV cache 视为可持久化、可复用的知识，而非一次性临时状态，覆盖缓存复用、卸载、压缩与服务优化等方向（tool-1-1、tool-1-2、tool-1-3）。在长上下文与编码助手类场景中，每次调用都会重复携带大量相同上下文，KV cache 的命中率与放置策略因此直接影响显存占用与推理成本（tool-1-1）。

本次条目的实质内容是打包与分发：由 CI 机器人从 \`dev\` 分支构建的 nightly CUDA 13.0 wheel，覆盖 linux/amd64 与 linux/arm64，并给出配合 PyTorch cu130 索引的安装命令。这属于安装渠道的更新——让使用 CUDA 13.0 工具链的环境可以直接以 wheel 方式获取预编译包，而不必自行从源码编译。需要强调的是，nightly 构建跟踪开发分支、并非稳定版本；源内容未提供任何功能、优化或性能数据，因此无法据此判断该构建相对既有版本有何变化。

从生态角度看，这类跟随上游 CUDA/PyTorch 版本节奏的轮子发布，是推理加速组件保持可用性的基础工作，其影响主要体现在部署便利性上，而非新的缓存算法或加速能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/a0x8o/lmcache">GitHub - a0x8o/ lmcache : LMCache : Supercharge Your LLM with the...</a></li>
<li><a href="https://www.gitgenius.co/repos/LMCache/LMCache">LMCache : Supercharge Your LLM with the Fastest KV Cache Layer</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#CUDA`, `#nightly release`, `#wheels`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [蚂蚁集团领投 Simplexity Robotics 1 亿美元 pre-A 轮，投后估值 16 亿美元](https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race) ⭐️ 7.0/10

彭博报道，中国具身智能公司 Simplexity Robotics 完成 1 亿美元 pre-A 轮融资，由蚂蚁集团领投，投后估值 16 亿美元；公司董事长兼联合创始人 Wang Kai 向彭博确认，阿里巴巴、腾讯、HongShan（红杉中国）和蓝驰创投跟投。

telegram · zaihuapd · 11月23日 02:02

**「背景」** Simplexity Robotics 于 2025 年 7 月在杭州成立，核心团队来自理想汽车；据彭博，该公司今年 3 月称成立半年内已完成五轮融资、累计融资 20 亿元人民币，当时投后估值已超过 10 亿美元。

**「影响」** 这笔融资会加剧中国本土人形机器人厂商之间的竞争：Simplexity 明确表示，资金将用于与已进入量产的宇树、优必选争夺市场；市场研究机构 Smart Analytics Global 的数据显示，2026 年上半年，中国厂商已占全球人形机器人出货量逾 97%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://global.chinadaily.com.cn/a/202608/11/WS6a7a8b3aa310986e2b46a1a5.html">Chinese humanoid robot makers hold 97% global shipments in H1</a></li>

</ul>
</details>

**标签**: `#humanoid robotics`, `#venture financing`, `#Ant Group`, `#China tech`, `#valuation`

---

<a id="item-finance-news-2"></a>
### [Anthropic IPO 后 AI 股抛售，中国 AI 公司上市计划承压](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

Anthropic 完成 1195 亿美元创纪录 IPO 后，全球 AI 股加速下跌；自 6 月底以来，中国科技股累计蒸发 1.7 万亿美元。彭博报道称，这令正在筹备或考虑发行股份的 DeepSeek、月之暗面和阶跃星辰的上市计划蒙上阴影。

telegram · zaihuapd · 11月23日 09:31

**「背景」** 这轮抛售发生在中国 AI 公司涌向公开市场、为算力竞赛融资之际：据《朝鲜日报》，DeepSeek 和月之暗面正筹备 2027 年上市，DeepSeek 还计划在内蒙古数据中心部署至少 16 万块华为 AI 加速器；《财富》称，这类融资用于支撑对美前沿模型的竞赛。此轮下跌已回吐中国科技股今年上半年的相当部分涨幅，令这些拟议发行的前景转暗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fortune.com/2026/07/23/moonshot-deepseek-great-chinese-ai-ipo-rush/">Moonshot, DeepSeek, and the Great Chinese AI IPO Rush</a></li>
<li><a href="https://www.chosun.com/english/industry-en/2026/10/08/LPVZSXQ4DNAMTKIBF77XUB3U6Y/">DeepSeek, Moonshot AI Prepare for 2027 IPOs - 조선일보</a></li>
<li><a href="https://www.investing.com/news/stock-market-news/chinas-ai-stocks-lose-17-trillion-as-tech-selloff-deepens-5043672">China ’s AI stocks lose $ 1 . 7 trillion as tech selloff deepens By...</a></li>

</ul>
</details>

**标签**: `#AI selloff`, `#China tech stocks`, `#IPOs`, `#Anthropic`, `#market volatility`

---

<a id="item-finance-news-3"></a>
### [上海地铁 12 月 1 日起实施 21 年来首次票价调整](https://weibo.com/1699432410/5368461393397183) ⭐️ 7.0/10

上海轨道交通将于 12 月 1 日实施 21 年来首次票价调整，新起乘价为 3 元、覆盖 0 至 4 公里，之后按 4、4、4、7、7、10、10 公里分段每段加 1 元，50 公里以上每 15 公里加 1 元。同步推出 190 元、210 元、270 元、390 元四档计次票，并对同一支付渠道当月累计满 90 元的乘客给予 9 折优惠。

telegram · zaihuapd · 11月23日 10:45

**「背景」** 上海轨道交通现行票价机制已沿用 21 年，此次为首次调整；调价前，上海市发改委曾公布两套票价方案及票价动态调整机制并提交听证。

**「对通勤者的影响」** 对每天乘地铁通勤的乘客来说，同一支付渠道当月累计满 90 元后按 9 折计费，加上 11 月 26 日开售的 35 至 90 次计次票，可部分抵消起步价 3 元、按里程逐段加价带来的支出上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hot.online.sh.cn/content/2026-09/09/content_10485162.htm">时隔 21 ...</a></li>

</ul>
</details>

**标签**: `#上海地铁`, `#公共交通票价`, `#民生政策`, `#计次票优惠`

---

