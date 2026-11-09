---
layout: default
title: "Horizon Summary: 2026-11-09 (ZH)"
date: 2026-11-09
lang: zh
---

> 从 59 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [Dux v2.0：开源的 Wayland 桌面外壳新增原子发行版支持](#item-tech-news-1) ⭐️ 7.0/10
2. [高盛将 Claude Code 从银行家和交易员移除](#item-tech-news-2) ⭐️ 7.0/10
3. [Outlook.com 开始拒绝无 DMARC 域名邮件](#item-tech-news-3) ⭐️ 7.0/10
4. [告别 Claude，转用 Pi：一个开发者的 LLM 工具迁移记录](#item-tech-news-4) ⭐️ 7.0/10
5. [Claude Code 被曝泄露真实邮箱，应尽快更新](#item-tech-news-5) ⭐️ 7.0/10
6. [Agent MechSuits：仅干预 10 个维度，CLI 智能体风险检测准确率超 97%](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek 自改 Transformer 架构数学题+7 分](#item-tech-news-7) ⭐️ 7.0/10
8. [写作作为思维工具引发讨论](#item-tech-news-8) ⭐️ 6.0/10
9. [英伟达调查黄仁勋遭情报行动](#item-tech-news-9) ⭐️ 6.0/10
10. [SQLite parse\_number 扩展：C 优化后比 Rust 更小更快](#item-tech-news-10) ⭐️ 6.0/10
11. [Nace 发布 Drex Max v1.1，自称登顶决策模型基准](#item-tech-news-11) ⭐️ 6.0/10
12. [姚顺雨：AI 公司护城河在产品层而非模型层](#item-tech-news-12) ⭐️ 6.0/10
13. [苹果据称最快 2027 年让 Siri 更像智能体](#item-tech-news-13) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 nightly-rocm 版本](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache 发布 nightly-rbln 版本](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache 发布 nightly-cu129 构建](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache 发布 CUDA 13.0 nightly 轮子](#item-ai-projects-4) ⭐️ 5.0/10

**推特新闻**
1. [Pieter Levels 发布 Infinite Slop TV 项目总结](#item-twitter-news-1) ⭐️ 8.0/10
2. [AI 产品/UX 走查提示词分享](#item-twitter-news-2) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Dux v2.0：开源的 Wayland 桌面外壳新增原子发行版支持](https://duxlabs.dev/) ⭐️ 7.0/10

Dux（原 Dank Material Shell）已发布 v2.0，这是一款自由开源的 Wayland 桌面外壳，提供文件管理器和主题功能，并新增对 Bazzite 等原子发行版的官方支持。该版本与 Niri 滚动窗口管理器搭配使用，目标是为 Linux 桌面提供可定制的 Wayland 环境。此前原子发行版支持是明显缺口，v2.0 补齐了这一需求。

hackernews · indigodaddy · 11月8日 19:08 · [社区讨论](https://news.ycombinator.com/item?id=50416053)

**「背景」** Dux 的前身是 Dank Material Shell，一个运行在 Niri 滚动式平铺 Wayland 合成器之上的桌面外壳；部分用户已经将其与 Niri 组合使用近一年。最近项目更名为 Dux 并发布 v2.0，新增了对 Bazzite 等原子化发行版的官方支持。

**「影响」** 对于 Bazzite 等原子发行版用户，现在可以获得官方安装支持，无需绕过此前的兼容性缺口；这降低了尝试 Dux/Niri 桌面的门槛。

**「社区讨论」** 多位用户报告已使用 DMS/Dux 近一年，认为其能帮助 Niri 走向主流；但也有评论质疑其 curl \| sh 安装方式的安全性，并指出该外壳正变得过于包罗万象。

**标签**: `#Wayland`, `#desktop-shell`, `#open-source`, `#Linux`, `#Niri`

---

<a id="item-tech-news-2"></a>
### [高盛将 Claude Code 从银行家和交易员移除](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

据 HN 消息及分析，高盛正在把 Anthropic 的 Claude Code 从银行家和交易员手中移除；官方未说明原因，但讨论集中在编码代理在敏感工作站的权限隔离、合规审计与按量计费失控等风险。目前尚无官方公告或细节确认，需视为报道而非已证实政策。

hackernews · TheWiggles · 11月8日 18:16 · [社区讨论](https://news.ycombinator.com/item?id=50415628)

**「背景」** 就在今年 7 月，高盛首席信息官 Marco Argenti 还公开赞扬非技术员工使用“vibe coding”；如今却将 Claude Code 和 GitHub Copilot 等 AI 编码工具仅限工程师使用，这一转变构成了理解本次撤回的背景。

**「影响」** 若属实，受影响的银行家和交易员将无法在主要工作机上使用 Claude Code；同类企业可能加快对编码代理的权限限制、审计要求或转向固定计费产品（有评论称 Gemini 以固定账单和节流方式赢得非工程用户）。

**「社区讨论」** 评论中，lukebuehler 称在金融专业人员主工作站运行半无人值守代理会同时接触客户/交易/自营信息、邮件、内网，风险过高；legitster 报告其组织因 Claude 消费计费超支而收回权限，而 Gemini 以固定计费和节流方式切入；fancyfredbot 推测更可能因交易损失而非主动决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://the-decoder.com/goldman-sachs-pulls-ai-coding-tools-from-traders-and-bankers/">Goldman Sachs pulls AI coding tools from traders and bankers</a></li>

</ul>
</details>

**标签**: `#AI`, `#enterprise software`, `#cybersecurity`, `#fintech`, `#Claude`

---

<a id="item-tech-news-3"></a>
### [Outlook.com 开始拒绝无 DMARC 域名邮件](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

据报道，Outlook.com 已开始对未发布 DMARC 记录的域名邮件进行拒绝或投递失败，发送方需配置 SPF/DKIM/DMARC 才能确保送达。部分用户报告收到 5xx 永久投递失败，但也有长期管理员称 Outlook 此前曾“静默丢弃”已正确认证的邮件；微软尚未正式公布这一变更。

hackernews · xmddmx · 11月8日 19:20 · [社区讨论](https://news.ycombinator.com/item?id=50416158)

**「相关背景」** DMARC 是基于 SPF 和 DKIM 的邮件认证协议，域名所有者通过 DNS 发布策略来声明如何处理认证失败的邮件。此前有报告显示，Outlook.com 自 2025 年 5 月起开始对每封邮件执行 SPF、DKIM 和 DMARC 检查，并直接拒绝未通过认证的邮件，而非仅标记为垃圾邮件。

**「影响」** 向 Outlook.com 地址发送邮件的组织和个人，如果域名未配置 DMARC，可能面临邮件被拒收或无法送达；应尽快发布 DMARC（并正确设置 SPF 与 DKIM）以避免投递失败。

**「社区讨论」** 评论者存在分歧：dwm 称 Outlook 实际返回 5xx 永久失败而非“静默”拒绝；codethief 则称 Outlook 多年来会在日志显示接受后仍丢弃部分正确配置 SPF/DKIM/DMARC 的邮件。Neikius 支持拒绝无 DMARC 域名，但批评 Outlook 还使用不公开的拦截列表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.getshadowinbox.com/posts/outlook-cold-email-rejected">Outlook Is Rejecting Your Cold Email . — Shadow Inbox blog</a></li>

</ul>
</details>

**标签**: `#email`, `#dmarc`, `#outlook`, `#deliverability`, `#microsoft`

---

<a id="item-tech-news-4"></a>
### [告别 Claude，转用 Pi：一个开发者的 LLM 工具迁移记录](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

作者记录了自己从 Claude 迁移到 Pi 这一 LLM harness 的经历，围绕提示词框架设计、模型表现和使用政策展开；文章在 Hacker News 上引发了关于 CLI 与 GUI 工具取舍、harness 内部机制以及第三方 harness 配合 Anthropic 订阅的 ToS 风险的讨论。

hackernews · karagenit · 11月8日 03:11 · [社区讨论](https://news.ycombinator.com/item?id=50410107)

**「背景」** Pi 是一个极简、可扩展的 LLM 代理运行框架（harness），目标是以用户自己的工作流为中心，而非让用户适应工具；它支持通过扩展、技能、提示模板和主题进行定制，并可将这些定制打包为 Pi 包，经 npm 或 git 分发。Pi 自带较强大的默认配置，但有意省略了子代理、计划模式等功能。

**「影响」** 社区评论指出，将 Pi 等第三方 harness 与 Anthropic 订阅配合使用可能违反服务条款并面临封禁，且非官方 harness 未必完整实现 Anthropic 的通信机制，可能影响模型行为；开发者在追求完全控制时需要评估这一兼容性与合规风险。

**「社区讨论」** 讨论中最实质的分歧在于控制力与合规、兼容性：gvkhna 认为 Pi 的完全控制让 orchestration 取代了反复干预，大幅减少了中断；leobuskin 则提醒在 Anthropic 模型上使用替代 harness 存在封禁风险，并可能缺失其自定义头、隐藏标志等通信机制。real\_faxenoff 还指出，当前模型的效率在很大程度上来自 harness 本身，第三方 harness 有时会过度消耗 token。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pi.dev/">Pi - There are many agent harnesses</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/pi: AI agent toolkit: unified LLM API ...</a></li>

</ul>
</details>

**标签**: `#LLM tooling`, `#AI assistants`, `#command-line`, `#Anthropic Claude`, `#open-source AI`

---

<a id="item-tech-news-5"></a>
### [Claude Code 被曝泄露真实邮箱，应尽快更新](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E5%B0%8F%E5%BF%83%EF%BC%8CClaude%20Code%E4%BC%9A%E6%93%85%E8%87%AA%E6%B3%84%E9%9C%B2%E4%BD%A0%E7%9A%84%E9%82%AE%E7%AE%B1%EF%BC%81%E8%AF%B7%E6%8A%93%E7%B4%A7%E6%97%B6%E9%97%B4%E6%9B%B4%E6%96%B0) ⭐️ 7.0/10

据新智元报道，Claude Code 会在联网请求外部网站时，把用户的真实登录邮箱、姓名、团队名称和公司内部 GitHub 仓库路径写入 HTTP User-Agent 请求头，已有用户因此收到直呼真名的诈骗邮件。原因是 Anthropic 工程团队为让模型获取账号信息，将登录邮箱硬编码进系统提示词，而 SEC、维基百科、crates.io 等站点又要求请求头提供联系邮箱，Claude 便将其发送出去。工程师 Lydia Hallie 已于 11 月 6 日公开道歉并说明原因，但报道未列出具体修复版本，仅提醒用户尽快更新。

rss · 新智元 · 11月8日 13:11

**「背景」** Claude Code 是 Anthropic 的本地终端编程工具，执行联网抓取时会向外部网站发送 HTTP 请求；部分站点（如 SEC、crates.io）要求在 User-Agent 头中带联系邮箱，否则返回 403。早先版本因拿不到账号信息导致 author 标签生成错误人名，工程师便把登录邮箱写入系统提示词，最终被模型带进请求头。该问题在 GitHub Issue \#107757 中已有用户报告，并被技术媒体记录为“Claude Code 将邮箱写入 User-Agent 的漏洞”。

**「影响与处置」** 受影响用户应尽快更新 Claude Code，并检查本地代理或服务器日志中是否已有带有真实登录邮箱、姓名或内部仓库路径的 User-Agent 请求外发；已有多名用户因此类泄露收到针对性诈骗邮件，若继续使用未修复版本，企业还可能暴露内部代码库地址。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/30672/claude-code-bug-email-user-agent-header">Claude Code bug sends your email to websites in the User - Agent</a></li>
<li><a href="https://github.com/anthropics/claude-code/issues/107757">Bug Report: Privacy violation in User - Agent header · Issue #107757...</a></li>
<li><a href="https://dev.to/naveenmalothu/claude-code-leaks-your-email-what-it-means-and-how-to-safeguard-your-apps-m9">Claude Code Leaks Your Email – What It Means and How to ...</a></li>
<li><a href="https://cybersecuritynews.com/claude-code-leaks-user-email/">Anthropic’s Claude Code Reportedly Leaks User Email Addresses ...</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#security vulnerability`, `#AI coding tools`, `#privacy`, `#software update`

---

<a id="item-tech-news-6"></a>
### [Agent MechSuits：仅干预 10 个维度，CLI 智能体风险检测准确率超 97%](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+NeurIPS%2726%20%7C%20%E5%8F%AA%E5%B9%B2%E9%A2%8410%E4%B8%AA%E7%BB%B4%E5%BA%A6%EF%BC%8C%E7%BB%99%E6%99%BA%E8%83%BD%E4%BD%93%E7%A9%BF%E4%B8%8A%E5%AE%89%E5%85%A8%E6%9C%BA%E7%94%B2%EF%BC%8C%E5%87%86%E7%A1%AE%E7%8E%87%E8%B6%8597%25) ⭐️ 7.0/10

NeurIPS 2026 接收的一篇论文提出 Agent MechSuits，一种面向多轮命令行（CLI）智能体的安全干预方法：在每一步动作生成前读取模型内部安全信号，只通过单个模型层中的 10 个隐藏表征维度进行稀疏干预，主模型权重保持冻结。论文报告，在三种受测模型上，当前步骤风险检测平均准确率达到 97.32%。该工作由佐治亚大学、罗格斯大学、南加州大学等机构的研究者完成，目前以论文形式提出，尚未说明已在生产系统部署。

rss · 新智元 · 11月8日 09:45

**「背景」** 多轮命令行智能体（CLI Agent）每一步都要结合历史动作、系统反馈和原始任务来决定下一步，因此安全风险会随执行过程不断变化；以往针对单轮命令的静态审查难以覆盖整个长程任务。Agent MechSuits 将安全检测接入模型内部隐藏表征，在单个模型层内进行稀疏干预，区别于常见的外部规则护栏。

**「影响」** 对开发 CLI 智能体安全防护的团队来说，该论文提供了一种不修改主模型权重、只在单层 10 个隐藏维度干预的轻量方案，如果被独立复现，可用于多轮任务中的逐步风险检测；但目前只有论文报告的三种受测模型平均准确率，尚未经独立验证或真实命令行环境评估，不能直接视为生产可用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.22673">[2606.22673] Agent MechSuits: Mechanistic Subspace Safety ...</a></li>

</ul>
</details>

**标签**: `#ai-safety`, `#agents`, `#neurips-2026`, `#representation-engineering`, `#model-interpretability`

---

<a id="item-tech-news-7"></a>
### [DeepSeek 自改 Transformer 架构数学题+7 分](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+AI%E4%BA%B2%E6%89%8B%E6%94%B9%E5%86%99Transformer%E6%9E%B6%E6%9E%84%EF%BC%81DeepSeek%E8%87%AA%E6%88%91%E6%94%B9%E9%80%A0%E6%9A%B4%E6%B6%A87%E5%88%86) ⭐️ 7.0/10

据新智元报道，DeepSeek-V4.1-Flash（7630 亿参数）读取自己求解数学题时最深 7 层的内部激活状态，在不修改权重的条件下生成了 Python 代码并将其插入推理流程，检测到“算偏”后回滚重算，在 AIME 与 HMMT 2026 数学竞赛上准确率提高 7 个百分点。该结果来自 DoubleAI 提出的“机制干预”研究，属于研究机构宣称的结果；原文未提供可独立验证的论文或复现细节。

rss · 新智元 · 11月8日 09:45

**「背景」** 10 月 18 日的日报曾报道 DeepSeek-V4.1-Flash-1017 作为 DeepSeek-V4.1-Flash 的小版本更新发布，官方称在推理、编码等任务上有所提升。本次 DoubleAI 的“机制干预”是在已发布的 DeepSeek-V4.1-Flash 上，让编程 Agent 读取内部激活并插入 Python 代码，而不是修改权重，与以往仅靠梯度调权重的模型修改方式不同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017">2026-10-18 — DeepSeek-V4.1-Flash-1017 Released With Coding Benchmark Gains</a></li>

</ul>
</details>

**标签**: `#AI`, `#DeepSeek`, `#Transformer`, `#architecture search`, `#machine learning`

---

<a id="item-tech-news-8"></a>
### [写作作为思维工具引发讨论](http://muratbuffalo.blogspot.com/2026/11/writing-as-thinking-tool.html) ⭐️ 6.0/10

一篇发表于个人技术博客的文章提出，写作本身是一种基本的思维工具，而不仅仅是对已完成想法的记录。文章在软件工程师和研究者中引发了关于写作、设计与编程如何帮助理清思路的讨论。该文没有提供新的技术或产品，属于关于认知方法的随笔。

hackernews · jruohonen · 11月8日 10:41 · [社区讨论](https://news.ycombinator.com/item?id=50412067)

**「背景」** 这类反思讨论的是将模糊想法外化（写成文字、草图或代码）以促进思考的普遍经验。评论者的亲身经历显示，纸面草图和手写代码常被用作整理系统设计的前置步骤。

**「社区讨论」** 评论者从不同领域补充了相似经验：一位博士生发现论文写作不是科研的收尾，而是理清思路的关键；一位设计师认为设计过程本身（而非仅靠原型或提示）能产生洞察；还有程序员指出手写代码也是思考工具。这些是个体经验，并非对文章主张的独立验证。

**标签**: `#writing`, `#cognition`, `#software-engineering`, `#research`, `#communication`

---

<a id="item-tech-news-9"></a>
### [英伟达调查黄仁勋遭情报行动](https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors) ⭐️ 6.0/10

英伟达董事会正在调查一起针对 CEO 黄仁勋的情报行动，而不是调查黄仁勋本人；原标题具有误导性。据评论区援引彭博社的报道，董事会将调查间谍案，且黄仁勋已承认婚外情。目前公开细节有限，无法确认黄仁勋或英伟达是否涉及不当行为。

hackernews · vincentchau · 11月8日 20:26 · [社区讨论](https://news.ycombinator.com/item?id=50416801)

**「背景」** 据彭博社等报道，英伟达董事会发起调查的重点是黄仁勋本人是否成为外国间谍活动的目标，而不是调查他本人违法；报道称黄仁勋已向员工承认婚外情，涉事女性被指疑似为中国政府从事间谍活动。这一区别解释了原始标题的误导性：董事会调查的是发生在他身上的情报行动，而非将黄仁勋作为调查对象。

**「社区讨论」** 评论区普遍指出原标题误导：英伟达调查的是黄仁勋遭遇的情报行动，而非黄仁勋本人（nrmitchi）。另有评论（everfrustrated）推测，若黄仁勋知晓新加坡公司是中国幌子并帮助规避美国出口管制，可能面临法律风险，但这一说法尚无证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity">Nvidia Board to Probe Spying Case After CEO Jensen... - Bloomberg</a></li>
<li><a href="https://nypost.com/2026/11/08/tech/jensen-huang-ceo-of-4-5t-chipmaker-nvidia-admits-affair-as-memo-warned-lover-was-chinese-spy/">Jensen Huang, CEO of $4.5T chipmaker Nvidia admits affair — as...</a></li>
<li><a href="https://finance.yahoo.com/markets/article/nvidias-jensen-huang-admits-to-affair-after-allegations-of-romance-with-chinese-spy-report-205122263.html">Nvidia &#x27;s board launches investigation into CEO Jensen Huang&#x27;s affair.....</a></li>

</ul>
</details>

**标签**: `#nvidia`, `#jensen-huang`, `#corporate-governance`, `#security`, `#tech-industry`

---

<a id="item-tech-news-10"></a>
### [SQLite parse\_number 扩展：C 优化后比 Rust 更小更快](https://simonwillison.net/2026/Nov/8/sqlite-parse-number-c-vs-rust/) ⭐️ 6.0/10

Simon Willison 发布了一份研究笔记，比较用 C 和 Rust 为 SQLite 编写 parse\_number\(\) 标量函数扩展的性能、代码复杂度和文件大小。该函数用于剥离逗号、美元/英镑符号和百分号，处理前导负号，无法解析时返回 NULL。Rust 版生成文件分别为 rusqlite 321KB、sqlite-loadable-rs 298KB，C 版仅 14KB；最初 Rust 更快，但在 C 中自写十进制解析器替代 strtod 后，C 在 200 万行混合数据上每行 19ns，优于 rusqlite 的 46ns 和 sqlite-loadable-rs 的 41ns。

rss · Simon Willison · 11月8日 22:26

**「背景」** SQLite 支持通过 C ABI 加载扩展来注册自定义 SQL 标量函数。parse\_number 的目标是把 &\#x27;-$1,234.56&\#x27; 或 &\#x27;12.5%&\#x27; 这类文本转为可求和、可排序的数值；C 默认可用 strtod 解析浮点数，但该研究中 Claude 发现 Rust 的等价实现速度约为 strtod 的两倍，于是进一步让 C 实现自写十进制解析器来追赶。

**「影响」** 对需要给 SQLite 添加此类轻量解析函数的开发者而言，若以 .so 体积和单行处理延迟为关键指标，C 扩展可以做到明显更小（14KB vs 298–321KB）且经优化后更快；但这需要自行维护自定义十进制解析代码，而不是依赖 strtod 或 Rust 生态现成 crate 的默认路径。

**标签**: `#SQLite`, `#Rust`, `#C`, `#extensions`, `#performance`

---

<a id="item-tech-news-11"></a>
### [Nace 发布 Drex Max v1.1，自称登顶决策模型基准](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 6.0/10

Nace 团队的 Alti 在 Reddit 自称发布了 Drex Max v1.1，并在 Artificial Analysis 的多模态决策模型基准上同时达到 SOTA 与 Pareto 前沿；该成绩由模型方陈述，尚未经独立验证。Drex Max v1 的权重已在 Hugging Face 以 Open RAIL-M 许可证提供，而 v1.1 开源权重称“即将推出”，目前仍在优化本地推理。作者还称上下文窗口约 256k，并比该类别中次优模型便宜 8 倍，可通过 kapitsa 引擎在 Mac 上运行。

reddit · r/MachineLearning · /u/m4rkGS · 11月8日 17:54

**「背景」** Artificial Analysis Decision Index 用于评估决策模型给出的概率与实际准确率的校准程度，各子基准等权重（tool-2-1）。同系列的 Drex Max v1 此前已作为 27B 参数的多模态决策模型开源，并在该指数上得 64 分（tool-2-3）。

**「影响」** 对希望复现的研究者，目前可直接获取的是 Drex Max v1 权重与论文，而非宣称达到 SOTA 的 v1.1；v1.1 开源权重及其本地推理优化仍待发布，因此相关评估应等待或基于 v1 进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-decision-index">Artificial Analysis Decision Index | Artificial Analysis</a></li>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/ drex - max - v 1 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#multimodal models`, `#decision models`, `#open source`, `#benchmarks`

---

<a id="item-tech-news-12"></a>
### [姚顺雨：AI 公司护城河在产品层而非模型层](https://www.ithome.com/1/023/991.htm) ⭐️ 6.0/10

11 月 8 日，腾讯首席 AI 科学家姚顺雨在 2026 未来科学大奖的一场对话中回应张亚勤提问时表示，AI 公司的护城河更多在产品层而非模型层，真正难替代的是理解用户背景、掌握专有数据并获得用户信任的产品。他以微信为例：若 AI 内嵌微信，能了解用户日程与社交关系，对手更聪明的模型也难以提供同样服务。张亚勤则调侃，按此逻辑 Anthropic 未来或许不值两万亿美元。

telegram · zaihuapd · 11月8日 14:17

**「背景」** 在 AI 竞争力讨论中，常见看法是模型能力构成核心壁垒；姚顺雨将重点转向产品层的用户背景、专有数据和信任，与纯粹比拼模型性能的观点形成区别。

**标签**: `#artificial intelligence`, `#technology industry`, `#product strategy`, `#competitive moat`, `#Tencent`

---

<a id="item-tech-news-13"></a>
### [苹果据称最快 2027 年让 Siri 更像智能体](https://9to5mac.com/2026/11/08/apple-working-on-agentic-siri-ai-next-year-report/) ⭐️ 6.0/10

据彭博记者 Mark Gurman 在 Power On 中称，苹果可能最早于 2027 年让 Siri 朝“智能体”方向转变，使其更主动地替用户执行任务，但这一说法尚未获苹果证实。Siri 已在 iOS 27 中实现个性化，却仍缺少主动代为操作的能力。为配合这一方向，苹果据称还调整了内部流程：iOS 28 首个开发周期从常规的四周编码、四周整合，改为六周编码探索加两周收敛，以便工程师有更多时间创新。

telegram · zaihuapd · 11月8日 16:36

**「背景」** Horizon 10 月 1 日的日报曾报道苹果计划推出配备升级版 Siri AI 的智能家居中枢；本次报道进一步聚焦 Siri 的主动执行能力，称 iOS 27 中的 Siri 已实现个性化但仍缺少代为操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-30/apple-is-finally-ready-to-enter-its-next-big-category-the-smart-home">2026-10-01 — Apple Plans October 13 Launch of Smart Home Hub with Siri AI</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Siri`, `#AI agents`, `#iOS`, `#software engineering process`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 nightly-rocm 版本](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

该版本提供针对 AMD Instinct GPU 的 LMCache 夜间 ROCm 7.2 轮子，支持 MI300X/MI325X \(gfx942\) 与 MI350X/MI355X \(gfx950\)，并与上游 vLLM ROCm 容器 ABI 匹配。

github · github-actions\[bot\] · 11月8日 08:24

**「解决的痛点」** 解决 AMD Instinct 用户在 ROCm 环境下安装 LMCache 的兼容性问题：预编译轮子匹配上游 vLLM ROCm 镜像的 torch 2.13 与 Python 3.12，避免从源码构建或依赖不匹配，简化部署。

**「背景与影响」** 在 LLM 推理生态中，LMCache 提供缓存加速，但 AMD GPU 用户需要与 ROCm 堆栈兼容的构建产物。此次 nightly 发布是例行的打包/支持更新，扩展了对 AMD Instinct 系列 GPU 的覆盖，未引入新的架构或性能声明。

**标签**: `#llm`, `#inference`, `#rocm`, `#lmcache`, `#nightly`

---

<a id="item-ai-projects-2"></a>
### [LMCache 发布 nightly-rbln 版本](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

这是 LMCache 面向 Rebellions RBLN NPU 的 nightly 预编译 wheel，基于 dev 分支于 2026-11-08 构建，适配 torch-rbln 0.12.0（torch 2.13.0+cpu），用于在 RBLN NPU 上运行 LLM 推理缓存。

github · github-actions\[bot\] · 11月8日 08:16

**「解决的痛点」** 为 Rebellions RBLN NPU 提供预编译的 LMCache wheel，避免用户从源码编译的复杂性，简化在专用 NPU 上的安装与部署。但 torch-rbln、rebel-compiler 和 RBLN 驱动仍需用户自行安装，未捆绑在 wheel 中。

**「背景与影响」** 在 LLM 推理缓存重要性提升的背景下，针对非 NVIDIA 专用 NPU 的硬件适配构建有助于扩展加速选项。此发布为常规 nightly 构建，基于 dev 分支，无重大架构或功能变更。

**标签**: `#LLM`, `#inference`, `#cache`, `#nightly`, `#NPU`

---

<a id="item-ai-projects-3"></a>
### [LMCache 发布 nightly-cu129 构建](https://github.com/LMCache/LMCache/releases/tag/nightly-cu129) ⭐️ 5.0/10

提供基于 dev 分支的 LMCache CUDA 12.9 预编译 wheel，支持 Linux amd64/arm64，可用 uv/pip 直接安装，便于使用最新开发版。

github · github-actions\[bot\] · 11月8日 11:49

**「解决的痛点」** 解决了用户在 CUDA 12.9 环境下需要从源码编译 LMCache 的痛点，提供预构建 wheel 降低安装门槛，并兼容 ARM64 平台，避免本地编译耗时和依赖冲突。

**「背景与影响」** LMCache 是面向大语言模型的缓存引擎，nightly 构建跟随开发分支，为需要最新特性和 CUDA 12.9 的用户提供快速获取渠道。本次发布为自动化构建，无功能亮点或更新日志，属于例行版本更新。

**标签**: `#lmcache`, `#cuda`, `#nightly`, `#wheels`, `#llm-caching`

---

<a id="item-ai-projects-4"></a>
### [LMCache 发布 CUDA 13.0 nightly 轮子](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布了从 dev 分支构建、面向 Linux amd64 与 arm64 的 CUDA 13.0 夜间版 wheel，用户可通过 pip 直接安装。

github · github-actions\[bot\] · 11月8日 09:19

**「解决的痛点」** 为需要在 CUDA 13.0 环境使用 LMCache 最新开发版的用户免去从源码编译的麻烦，提供了预编译的 pip 安装包，降低部署门槛并加快测试迭代。

**「背景」** LMCache 是一个面向 LLM 推理的 KV 缓存管理层，可将 KV 缓存从临时状态转化为可持久化、可跨引擎复用的 AI 原生知识。本次 nightly 发布提供了基于 dev 分支构建的 CUDA 13.0 预编译 wheel，覆盖 linux/amd64 和 linux/arm64，方便用户通过 pip 快速安装并测试最新开发版本。该发布属于自动化例行构建，未声明具体新特性或性能改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache ! | LMCache</a></li>

</ul>
</details>

**标签**: `#llm`, `#cache`, `#cuda`, `#nightly`, `#release`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Pieter Levels 发布 Infinite Slop TV 项目总结](https://x.com/levelsio/status/2119564112208257515) ⭐️ 8.0/10

Pieter Levels 于 2026 年 11 月 8 日发布推文，宣布其 AI 实时视频流项目 Infinite Slop TV 于 2026 年 8 月至 10 月运营后关闭。该项目允许互联网用户通过聊天输入内容，实时生成持续播放的 AI 视频。Levels 称，此前没有 AI 视频模型能生成得比播放更快，直到 @fal 将 MiniMax 的 H3 模型优化到足够快才实现；FAL 还赞助了该项目，否则每月 GPU 成本至少 20 万美元。他给出的统计包括：1780 万次剪辑观看、287,555 条聊天消息、287,000 个剪辑点赞、210,196 个 AI 剪辑播出、125,808 条消息被审核拦截（约 44%）、185,000 名访客、47,000 人制作了视频、860 小时不重复视频，以及 3 个赞助商和 3 个奖项（5000 美元、2500 美元、1000 美元）。他表示项目最终未能持续吸引关注，但认为未来会有实时生成的互动和个性化内容，并提到类似技术用于实时生成教师讲解有其积极一面。

twitter · @levelsio · 11月8日 22:53

**「背景与总结」** Pieter Levels（@levelsio）于 2026 年 11 月 8 日发布推文，宣布其项目“Infinite Slop TV”已于 2026 年 10 月结束。这是一个实时 AI 生成视频流，任何人都可通过聊天输入参与，输入内容会进入持续播放的 AI 视频流。据 Levels 称，此前没有 AI 视频模型能以快于播放的速度生成内容，直到 FAL 修改了 MiniMax 的 H3 模型才实现；FAL 还赞助了该项目，否则每月 GPU 成本至少 20 万美元。

项目为期两个月，Levels 给出了详细数据：17,800,000 次片段观看，287,555 条聊天消息，287,000 个剪辑点赞，210,196 个 AI 片段播出，125,808 条消息被审核屏蔽（约 44%），185,000 名访客，47,000 人制作过视频，累计 860 小时不重复视频。赞助方包括 sideshiftai、creem\_io、chatbase；并向三位创作者发放了 5000、2500 和 1000 美元奖金。

Levels 总结称该实验很有趣但未能持续吸引注意力。由于每个视频会尝试与前一个视频保持一定连贯性，出现了哥特女孩、史莱姆女孩、腌黄瓜、像素艺术等流行趋势并被用户反复切换。他认为“slop”令人上瘾但也会因过于基础而令人厌倦，未来可能会出现实时生成、互动且个性化的内容，但也指出这既有反乌托邦的一面（如实时生成的教师向孩子讲解内容）也有乌托邦潜力。就“slop”一词，一项被归档于 2026 年 10 月 15 日的 Reddit 研究（tool-1-1）分析了 LLM 文本中该风格的来源；此处它被用于描述实时生成的 AI 视频。原帖下无社区评论可供参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1x64lbk/tracing_where_llm_slop_style_comes_from_in_the/">2026-10-15 — Tracing where LLM &#x27;slop&#x27; style comes from and how to cut it</a></li>

</ul>
</details>

**标签**: `#AI video`, `#generative AI`, `#project retrospective`, `#real-time AI`, `#technical stats`

---

<a id="item-twitter-news-2"></a>
### [AI 产品/UX 走查提示词分享](https://x.com/vista8/status/2119574943021371755) ⭐️ 6.0/10

作者分享了一个用于模拟产品与设计走查的 AI 提示词。该提示词让 AI 扮演产品经理、UX 研究员和顶级 UI 设计师，主动走查每个页面和交互细节，从信息架构、用户流程、操作效率、反馈机制、视觉层级、组件一致性六个维度审视，判断问题严重度并形成可执行方案。

twitter · 向阳乔木 · 11月8日 23:37

**「背景」** 作者在开发工具后想继续打磨，联想到大厂有产品、设计走查验收环节，于是编写了该提示词。提示词强调让 AI 主动决定顺序与优先级，以真实用户的认知负担和情绪体验为标准，目标是行业顶级而非“能用就行”。

**标签**: `#AI prompt`, `#UX review`, `#product design`, `#automation`

---