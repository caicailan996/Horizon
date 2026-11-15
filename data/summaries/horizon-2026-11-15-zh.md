# Horizon 每日速递 - 2026-11-15

> 从 66 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [SpaceX 星舰第 15 次试飞成功捕获飞船上级](#item-tech-news-1) ⭐️ 8.0/10
2. [Lovable 应用泄露护照信息和逾 20 万私信](#item-tech-news-2) ⭐️ 8.0/10
3. [PyPI 项目页改版上线：更清晰的安全与来源信号](#item-tech-news-3) ⭐️ 7.0/10
4. [科技公司再次试图重新定义隐私概念](#item-tech-news-4) ⭐️ 7.0/10
5. [意大利对 Meta 罚款 8.05 亿欧元，涉 Android 相册默认访问](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI 解散独立机器人团队，改由通用模型驱动](#item-tech-news-6) ⭐️ 7.0/10
7. [W5000 无人货机完成技术验证试飞](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare 开源 AI 代理浏览器 Kitesurf](#item-tech-news-8) ⭐️ 7.0/10
9. [软件职位名称家族树](#item-tech-news-9) ⭐️ 6.0/10
10. [KDE 纪录片：桌面环境历史与社区回顾](#item-tech-news-10) ⭐️ 6.0/10
11. [AI4AI 综述：三项研究决策与 L0-L3 控制来源框架](#item-tech-news-11) ⭐️ 6.0/10
12. [Reddit 讨论：短期价格预测论文是否应对比市场隐含预测？](#item-tech-news-12) ⭐️ 6.0/10
13. [谷歌高管用 Gemini 在折叠 iPhone 上运行 Windows 11](#item-tech-news-13) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 nightly-rocm：AMD ROCm 7.2 支持](#item-ai-projects-1) ⭐️ 7.0/10
2. [LMCache Nightly CUDA 13.0 构建发布](#item-ai-projects-2) ⭐️ 5.0/10

**财经新闻**
1. [Nvidia CEO 辞职后 AI 交易或转向其他芯片商和云公司](#item-finance-news-1) ⭐️ 8.0/10
2. [Anthropic IPO 被曝拒绝中国内地及香港投资者下单](#item-finance-news-2) ⭐️ 8.0/10

**推特新闻**
1. [SpaceX 首次用机械臂夹住回收二级飞船](#item-twitter-news-1) ⭐️ 7.0/10
2. [Pieter Levels：让用户上传家具照片生成 3D 物体](#item-twitter-news-2) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SpaceX 星舰第 15 次试飞成功捕获飞船上级](https://www.spacex.com/launches/starship-flight-15) ⭐️ 8.0/10

在 11 月 13 日的星舰第 15 次试飞中，助推器因技术问题未返场塔捕，改在墨西哥湾受控溅落后爆炸，原因未公布；飞船则成功入轨，部署 26 颗 Starlink V3 卫星（其中 3 颗带摄像头检查隔热瓦），绕地球约 14 圈后返回。11 月 14 日，飞船完成约 22.5 小时飞行后首次被发射塔机械臂捕获，实现轨道级飞船塔捕。这是星舰上二级首次成功回收，向完全可复用迈出关键一步，但双回收尚未实现。

hackernews · ls612 · 11月14日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=50500963)

**「背景」** 此前，星舰第 14 次试飞已实现首次入轨并部署 26 颗 Starlink 卫星，但上面级回收尚未验证。第 15 次试飞则是首次尝试用发射塔机械臂捕获飞船上面级。

**「影响」** 对回收复用目标而言，本次成功仅覆盖飞船一级；评论指出下一步的双捕获和复飞同一飞船才是轨道载荷成本显著下降的关键，而助推器爆炸意味着该闭环尚未打通。

**「社区讨论」** 评论区将星舰与航天飞机对比，认为无固体助推器且飞船叠于顶部避开了挑战者号和哥伦比亚号的事故模式；同时有评论强调，只有完成双捕获并复飞同一飞船，发射成本才会显著下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/spacex-starship-orbit-262d3c58d56bf7a525b49115d6c5dfe8">2026-09-29 — SpaceX Starship Reaches Orbit, Deploys Starlink Satellites</a></li>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/spacex-says-starship-flight-15-booster-aborted-chopsticks-landing-catch-after-launch-due-to-guidance-issue-video">SpaceX still investigating why Starship Flight 15 booster ... | Space</a></li>

</ul>
</details>

**标签**: `#spacex`, `#starship`, `#reusable-rockets`, `#space-hardware`, `#aerospace`

---

<a id="item-tech-news-2"></a>
### [Lovable 应用泄露护照信息和逾 20 万私信](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

安全研究人员披露，Lovable 平台生成的 AI 应用因行级安全（RLS）配置不足，泄露了护照信息和超过 20 万条私人消息。Lovable 安全负责人确认根因是 RLS 不足，并表示平台会在发布前自动扫描每个应用，同时提供免费的深度 SAST 扫描和修复选项。评论者提到的 Supabase 宽松默认设置责任尚未得到独立确认。

hackernews · armcat · 11月14日 17:43 · [社区讨论](https://news.ycombinator.com/item?id=50499017)

**「背景」** Lovable 平台生成的应用程序在 Supabase 上运行时，依靠行级安全（Row-Level Security, RLS）来限制对数据库行的访问；如果未正确启用或配置，匿名或已认证用户就可能读取本应私密的数据。有社区评论称，Supabase 为了降低上手门槛，多年来默认采用宽松的 RLS 设置，且虽报道称 10 月 30 日已修复，但现有项目可能仍沿用旧默认值，这解释了为何 Lovable 应用会暴露护照信息和超过 20 万条私信。

**「影响」** 研究人员扫描了 159,041 个 Lovable 生成的应用，发现其中 24,664 个应用可被任何人在无认证情况下直接读取数据库记录，泄露了护照号码、支付信息和超过 20 万条私人聊天消息；这意味着相关应用的用户数据可能已被未授权访问，开发者需要立即检查 Supabase 的行级安全（RLS）设置并启用 Lovable 提供的自动修复或发布拦截。

**「社区讨论」** 评论中一个主要分歧是责任归属：SOLAR\_FIELDS 认为 Supabase 多年为降低上手门槛而选择宽松的行级安全默认值，且 10 月 30 日的修复对现有项目可能仍不生效；其他评论则强调平台应默认拒绝数据库访问、采用最小权限 API。Lovable 安全负责人表示其自动扫描正是用于发现这类 RLS 问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/security/lovable-ai-apps-expose-personal-information/">Lovable AI apps exposed sensitive data in open databases ...</a></li>
<li><a href="https://startupfortune.com/lovable-ai-apps-left-passport-and-payment-data-open-to-anyone/">Lovable AI Apps Left Passport and Payment Data Open to ...</a></li>
<li><a href="https://dailysecurityreview.com/cyber-security/24664-lovable-built-apps-leak-passports-and-chat-messages/">24,664 Lovable-Built Apps Leak Passports and Chat Messages</a></li>

</ul>
</details>

**标签**: `#security`, `#AI code generation`, `#Supabase`, `#Row-Level Security`, `#data exposure`

---

<a id="item-tech-news-3"></a>
### [PyPI 项目页改版上线：更清晰的安全与来源信号](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI 的项目页面现已上线改版，为访问者提供更清晰的安全与来源（provenance）信号，帮助用户评估软件包可信度。该更新主要是界面重设计，集中展示已有的信任数据，而不是新增安全机制。

hackernews · rbanffy · 11月14日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50497892)

**「背景」** PyPI 用 attestations 提供可验证的 provenance（来源证明）记录。此前 Horizon 10 月 22 日日报曾报道 LiteLLM 1.107.0 在 PyPI 被植入凭据窃取器与后门，这类事件凸显了在项目页直接展示来源与安全信息的必要性。

**「影响」** 用户在浏览 PyPI 项目页时可以更直观地看到哪些包具备有效来源证明，从而在安装前降低遭篡改包的风险；但该更新不新增恶意包检测能力，且来源信息依赖集中式云服务，存在锁定担忧。

**「社区讨论」** 有用户欢迎对来源信息的强调，并希望密钥无关签名和可信发布支持可复用工作流。也有用户担心信任机制依赖“大云”和锁定，另有用户指出该功能只能识别原本良性项目被入侵，无法识别恶意项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/">2026-10-22 — Compromised LiteLLM 1.107.0 on PyPI Ships Credential Stealer and Backdoor</a></li>
<li><a href="https://pypi.org/project/amoorion-blogger/">amoorion-blogger · PyPI</a></li>

</ul>
</details>

**标签**: `#python`, `#pypi`, `#security`, `#supply-chain`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [科技公司再次试图重新定义隐私概念](https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again) ⭐️ 7.0/10

EFF 在 2026 年 11 月 14 日发布的文章中提出，科技公司正试图再次改变隐私的定义，方向可能削弱用户保护；分析摘要指出，争议集中在 AI 驱动的监控和难以退出的隐私选择上。

hackernews · gslin · 11月14日 12:45 · [社区讨论](https://news.ycombinator.com/item?id=50496602)

**「背景」** Horizon 在 10 月 24 日的日报中曾报道，Google 更新隐私政策，可能将 Gmail 和 Google Photos 数据用于广告定向，这已反映出企业将用户数据默认纳入商业用途的做法。EFF 这篇文章则把这一变化放在更长的脉络里，认为科技公司正在把隐私负担转嫁给个人：用户需要自行了解市面上各种设备的录音能力和信号，才能避免自己的对话被记录和上传。

**「影响」** 对普通员工而言，这意味着专业会议甚至一对一对话可能在未明确同意的情况下被 AI 记录并上传，拒绝参与记录可能与维持就业产生冲突；有评论建议在会议开始时明确要求关闭 AI 转录，但这尚未成为可执行的普遍规范。

**「社区讨论」** 一位用户报告称，如今几乎所有工作会议都被可见或不可见的 AI 访客记录，甚至包括直属管理者与同事的一对一交谈；另一评论引用《世界人权宣言》第十二条，认为技术公司无权任意干涉个人隐私。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/tech/1017600/google-personal-intelligence-privacy-policy-ads-update">2026-10-24 — Gmail and Google Photos data may target ads under updated Google policy</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again">Tech Companies Are Trying to Shift the Entire Concept of ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#technology-policy`, `#AI`, `#surveillance`, `#EFF`

---

<a id="item-tech-news-5"></a>
### [意大利对 Meta 罚款 8.05 亿欧元，涉 Android 相册默认访问](https://www.reuters.com/world/italy-fines-meta-887-million-over-android-users-data-access-2026-11-14/) ⭐️ 7.0/10

意大利隐私监管机构对 Meta 处以 8.05 亿欧元（约合 8.87 亿美元）罚款，原因是 Facebook Android 应用在未经用户具体同意或明确告知的情况下，访问了约 2000 万意大利用户的相册照片、视频及元数据。涉事功能为 2023 年上线的相册推荐功能，默认开启且授权提示笼统。Meta 须在 60 天内将该功能改为默认关闭并单独征得用户同意。

hackernews · giuliomagnifico · 11月14日 13:48 · [社区讨论](https://news.ycombinator.com/item?id=50497009)

**「背景」** 意大利数据保护机构 Garante 依据 GDPR 和《隐私法典》执法，近年来对大型科技公司采取过多项高调行动，例如 2023 年短暂禁用 ChatGPT、禁用 Replika，并在 2022 年对 Clearview AI 罚款 2000 万欧元。这一背景有助于理解此次对 Meta 的罚款并非孤立事件，而是该机构持续监管大型平台数据行为的体现。

**「社区讨论」** 在 Hacker News 讨论中，有用户质疑为何 iOS 版未被同样处罚、以及 Android 与 iOS 的授权机制有何不同；也有用户认为用户此前已授权，不清楚监管机构保护的具体内容，并指出报道缺少技术细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gdprfine.com/dpa/italy-garante">Italian Garante GDPR Fines : Enforcement Record &amp; AI Cases</a></li>
<li><a href="https://www.recordinglaw.com/world-laws/world-data-privacy-laws/italy-data-privacy-laws/">Italy Data Privacy Laws: GDPR, Privacy Code &amp; Garante Guide (2026)</a></li>

</ul>
</details>

**标签**: `#Meta`, `#privacy`, `#Android`, `#data access`, `#regulation`

---

<a id="item-tech-news-6"></a>
### [OpenAI 解散独立机器人团队，改由通用模型驱动](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/) ⭐️ 7.0/10

OpenAI 解散了独立机器人团队，将研究员重新分配到更通用的研究团队。公司称，原因是 GPT-6 Astra 等通用前沿模型已能直接操控机器人执行任务，不再需要专门机器人团队。OpenAI 仍在继续自研人形机器人，CEO 的目标是 2027 年首次公开展示。此前其早期机器人团队于 2020 年解散，2024 年重建并与 Figure 合作，该合作已于 2025 年 2 月终止。

telegram · zaihuapd · 11月14日 04:00

**「背景」** OpenAI 曾在 2020 年解散早期机器人团队，2024 年重建并与 Figure 合作，但该合作于 2025 年 2 月终止；此次调整前，OpenAI 称其通用模型 GPT-6 Astra 在模拟操作任务上达到 74.8% 成功率，超过专用机器人模型的 51.0%（Nvidia 研究），这为用通用模型直接控制机器人提供了依据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://theroboticsmedia.com/article/openai-disbands-robotics-team-gpt-6-astra">OpenAI Disbands Robotics Team, Bets on GPT-6 Astra Instead</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#robotics`, `#general AI models`, `#AI strategy`, `#humanoid robots`

---

<a id="item-tech-news-7"></a>
### [W5000 无人货机完成技术验证试飞](https://www.ithome.com/1/027/068.htm) ⭐️ 7.0/10

白鲸航线于 11 月 14 日宣布，W5000 大型无人货运飞机在内蒙古鄂托克前旗完成技术验证试飞，爬升、平飞、转弯、下降、进近着陆全部科目按计划完成。该机标称最大起飞重量 10.8 吨、最大业载 5 吨、设计航程 2600 公里，采用涡桨动力和自主驾驶、地面监控模式，按设计一个机组可同时监控 6 至 7 架。企业预计 2027 年上半年完成适航取证，此次试飞仅是技术验证，尚未取得适航认证。

telegram · zaihuapd · 11月14日 05:00

**「背景」** 技术验证试飞是大型无人货机进入适航审定前的关键环节，用于验证爬升、平飞、转弯、下降、进近着陆等基本飞行科目能否按设计完成。白鲸航线此次公布的是这一前置阶段的进展，企业预计 2027 年上半年完成适航取证，目前尚未取得适航证书。

**「影响」** 对潜在货运运营方而言，该机若按计划于 2027 年上半年取证，可提供 5 吨业载、2600 公里航程的无人货运能力，并可能以一名地面机组同时监控 6 至 7 架的方式降低远程航线人力成本；但在取证前不能投入商业运营。

**标签**: `#autonomous-cargo-aircraft`, `#unmanned-aerial-vehicle`, `#aviation`, `#logistics`, `#autonomous-systems`

---

<a id="item-tech-news-8"></a>
### [Cloudflare 开源 AI 代理浏览器 Kitesurf](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) ⭐️ 7.0/10

Cloudflare 以 Apache 2.0 许可证开源了 Kitesurf，这是一款面向 AI 代理的无状态浏览器，基于 Cloudflare Workers 构建，无需浏览器容器即可解析 HTML、处理 CSS 并执行 JavaScript。Cloudflare 称其比 Chromium 占用更少 CPU 和内存，并可在全球 Workers 网络上按需扩展；相关代码已发布在 GitHub。

telegram · zaihuapd · 11月14日 09:33

**「背景」** 在 Kitesurf 之前，Cloudflare 已陆续推出面向 AI 代理的开发与数据接口：9 月 30 日摘要曾报道其发布 cf CLI 开放测试版，让开发者和 AI 代理通过命令行访问 3000 多个 Cloudflare API 操作；10 月 6 日摘要曾报道其发布面向 AI 代理工作流的 Web Search API。Kitesurf 是在这些接口基础上补上可解析 HTML/CSS/JS 的浏览器层，使代理无需自建 Chromium 容器即可完成页面渲染。

**「影响」** 开发者可以在 Apache 2.0 许可下将 Kitesurf 集成到 AI 代理工作流中，并利用 Cloudflare Workers 按需扩展，避免维护浏览器容器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-cf-cli-launch/">2026-09-30 — Cloudflare cf CLI targets agents with 3,000 API operations</a></li>
<li><a href="https://developers.cloudflare.com/changelog/post/2026-10-02-introducing-web-search-api/">2026-10-06 — Cloudflare Introduces Web Search API for AI Agent Workflows</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#browser`, `#Cloudflare`, `#open source`, `#edge computing`

---

<a id="item-tech-news-9"></a>
### [软件职位名称家族树](https://zwischenzugs.com/2026/11/03/a-family-tree-of-software-job-titles/) ⭐️ 6.0/10

这篇博客文章以图谱形式梳理软件职位名称的演变与相互关系，展示不同头衔之间的沿革和重叠。文章引发了关于头衔通胀和角色含义模糊的讨论，评论者结合自身经历指出 DevOps、SRE、Scrum/Agile 等头衔在不同组织中的实际含义差异很大。

hackernews · umerf · 11月14日 17:45 · [社区讨论](https://news.ycombinator.com/item?id=50499038)

**「背景：同一职衔的语义漂移」** 这篇关于软件职位名称谱系的文章指出，许多职衔并非稳定含义，而是会在不同时期被重新定义。例如，“系统工程师”在 1960 年代 IBM 是面向客户的售前安装设计角色，而在 1990 年代受微软 MCSE 认证影响，则指更资深、偏设计的系统管理员。

**「影响」** 对求职者和招聘方而言，这些讨论表明仅凭职位头衔无法可靠判断实际技能与职责；多名评论者称自己在不同公司担任 DevOps 或 SRE 时的实际工作内容相差甚远，求职时需结合具体职责描述而非头衔。

**「社区讨论」** 一位评论者（probably\_wrong）提到有人未正式学习软件开发却想用“软件工程师”头衔申请相关岗位，并认为软件工程师应能区分代码好坏；评论者 siva7 则认为 Scrum、Agile、DevOps 等头衔的含义已像 90 年代中期的“webmaster”一样过时，不同组织甚至同一组织内部都相差很大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zwischenzugs.com/2026/11/03/a-family-tree-of-software-job-titles/">A Family Tree of Software Job Titles – zwischenzugs.com</a></li>

</ul>
</details>

**标签**: `#software-engineering`, `#careers`, `#job-titles`, `#technology-industry`, `#devops`

---

<a id="item-tech-news-10"></a>
### [KDE 纪录片：桌面环境历史与社区回顾](https://tube.kockatoo.org/w/fFinNHfanLT7aBEb2B8y4c) ⭐️ 6.0/10

一段关于 KDE 桌面环境的纪录片在 tube.kockatoo.org 发布，回顾了该项目的历史、技术挑战与社区协作。视频内容属于历史叙述，不涉及新的软件版本、功能发布或兼容性变更。

hackernews · mrkn1 · 11月14日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=50496976)

**「背景」** 这部纪录片所回顾的 KDE 历史始于 1996 年 Matthias Ettrich 在 Usenet 上呼吁为 Linux 打造更好的桌面环境，随后项目经历了 Qt 许可证争议、KDE 4 发布初期的严重不稳定与社区分裂，最终逐渐恢复并延续至今。

**「社区讨论」** 多位评论者从个人使用经历出发回顾 KDE：有人称 KDE3 时代 Amarok 1.4、k3b 和 Konqueror 的集成体验曾让自己选择 Mandrake 而非 Windows XP；也有人提到 KDE 4 初期不稳定和缺陷导致其一度疏远，直到后续版本才重新关注。这些是用户个人体验，不代表项目官方说明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m-zone.cc/details/movie/1777637">KDE : The Documentary Movie Details - M-Zone</a></li>

</ul>
</details>

**标签**: `#KDE`, `#open source`, `#desktop environment`, `#documentary`, `#software history`

---

<a id="item-tech-news-11"></a>
### [AI4AI 综述：三项研究决策与 L0-L3 控制来源框架](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E3%80%8C%E8%AE%A9AI%E7%A0%94%E7%A9%B6AI%E3%80%8D%E6%9C%80%E6%96%B0%E7%BB%BC%E8%BF%B0%EF%BC%9A%E4%B8%89%E9%A1%B9%E5%85%B3%E9%94%AE%E5%86%B3%E7%AD%96%E6%A1%86%E6%9E%B6%EF%BC%8C%E9%87%8D%E6%96%B0%E5%AE%A1%E8%A7%86%E7%A0%94%E7%A9%B6%E8%87%AA%E4%B8%BB%E6%80%A7) ⭐️ 6.0/10

南开大学与中关村学院团队在一篇 AI 研究自主性综述中，将 AI 驱动的研究拆解为搜索方向、搜索空间和评价信号三项决策，并提出 L0-L3 控制来源框架，用于判断研究控制权在人类与 AI 之间的分布。文章指出，让 AI 读论文、写代码、跑实验并不等同于把研究决策交给 AI；研究问题、允许修改范围和成功标准仍常由人类设定。该综述以预印本形式发布（preprints.org 编号 202610.2999，项目主页 ai4ai-research.github.io），是对现有系统的分类框架，不是新系统的实测结果。

rss · 新智元 · 11月14日 09:03

**「背景」** 该综述以预印本形式发布在 Preprints.org 上（手稿编号 202610.2999），未经同行评议；因此文中提出的 L0–L3 控制来源框架属于作者提出的分析方案，而非已被独立验证的研究结论。

**「影响」** 开发或评估 AI 研究智能体的团队可以按搜索方向、搜索空间、评价信号分别检查控制权，避免把流程自动化误判为研究决策自动化；但该框架不提供新的实验性能数据，主要作用是分类与评估工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.preprints.org/">Preprints .org - The Multidisciplinary Preprint Platform</a></li>

</ul>
</details>

**标签**: `#AI research`, `#research autonomy`, `#survey`, `#machine learning`, `#AI agents`

---

<a id="item-tech-news-12"></a>
### [Reddit 讨论：短期价格预测论文是否应对比市场隐含预测？](https://www.reddit.com/r/MachineLearning/comments/1xw6fk9/should_shorthorizon_price_forecasting_papers/) ⭐️ 6.0/10

Reddit 用户 happypeanut-t 提出一个方法论问题：许多加密货币和大宗商品短期价格预测论文只用 ARIMA、随机游走或简单 LSTM 作为基线并报告更好的 RMSE，却很少对比市场隐含预测（如期权隐含波动率区间、真金白银的群体预测），也很少评估点预测之外的区间覆盖率。该用户认为，市场隐含预测已包含大量公开信息，仅击败随机游走说明不了什么，对 BTC 等资产区间覆盖率比 RMSE 更有信息量。帖子询问这一做法未成为标准的原因是数据获取困难还是自己漏看了相关论文。

reddit · r/MachineLearning · /u/happypeanut-t · 11月14日 16:23

**「研究背景」** 在短周期加密货币和大宗商品价格预测文献中，常见做法是与 ARIMA、随机游走和简单 LSTM 等基准比较并报告 RMSE；而市场隐含预测（如期权隐含波动率区间或参与者下注的群体预测）很少被作为对照，因为这些预测已整合大量公开信息，仅跑赢随机游走不能说明跑赢了市场自身预期。此外，多数论文只评估点预测，对 BTC 等波动资产而言 80% 区间的覆盖率比 RMSE 更有信息量。

**标签**: `#machine learning`, `#forecasting`, `#model evaluation`, `#finance`, `#benchmarking`

---

<a id="item-tech-news-13"></a>
### [谷歌高管用 Gemini 在折叠 iPhone 上运行 Windows 11](https://www.windowslatest.com/2026/11/14/windows-11-can-run-on-apples-foldable-iphone-and-googles-ai-boss-proved-it-using-gemini-years-after-microsoft-gave-up-on-windows-phones/) ⭐️ 6.0/10

Google AI Studio 产品设计负责人 Ammaar Reshi 用 Gemini 4 Carbon 在一台苹果折叠手机 iPhone Duo 上本地运行 Windows 11 24H2，并公开了操作视频；这目前是一次技术演示，而非面向普通用户的产品。该方案基于开源项目 WindowsiOS，无需越狱，通过 JIT 翻译运行 ARM64 代码，并支持 Microsoft Prism 运行部分传统应用；镜像约 12 GB，需 Apple Silicon Mac 与开发工具。

telegram · zaihuapd · 11月14日 06:52

**「背景」** WindowsiOS 是一个开源项目，允许在未越狱的 iPhone 上通过 JIT（即时编译）翻译运行 Windows 11 ARM64 代码；其镜像约 12 GB，需要 Apple Silicon Mac 和开发工具配合，并可借助微软 Prism 兼容层运行部分传统 x86 应用。此次演示正是基于这一技术路径，由 Gemini 4 Carbon 辅助完成操作。

**标签**: `#Windows 11`, `#iOS`, `#JIT emulation`, `#Gemini AI`, `#Open source`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 nightly-rocm：AMD ROCm 7.2 支持](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 7.0/10

LMCache 的 nightly 版本提供了针对 AMD Instinct MI300X/MI325X/MI350X/MI355X 的 ROCm 7.2 预编译 wheel，ABI 与上游 vLLM ROCm 容器匹配，可直接安装使用。

github · github-actions\[bot\] · 11月14日 07:47

**「解决的痛点」** 此前 LMCache 在 AMD GPU 上缺少与 vLLM ROCm 环境匹配的官方构建，用户需自行编译或面临 ABI 不兼容问题。该 nightly 版本提供了针对 gfx942/gfx950 架构的 ROCm 7.2 wheel，并确保与上游 vLLM ROCm 镜像（torch 2.13, cp312）一致，简化了在 AMD Instinct GPU 上的部署流程。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV 缓存管理层，可将 KV 缓存从临时状态转变为可复用知识，支持跨推理引擎复用与监控（tool-1-2）。本次 nightly 发布提供 ROCm 7.2 wheels，适配 AMD Instinct gfx942（MI300X/MI325X）与 gfx950（MI350X/MI355X），ABI 与上游 vLLM ROCm 容器（torch 2.13, cp312）匹配，使 LMCache 得以部署在 AMD GPU 上，扩大了其非 CUDA 生态覆盖。由于是 nightly 构建，属于平台支持路径的前瞻性更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#ROCm`, `#LLM inference`, `#AMD`, `#nightly`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly CUDA 13.0 构建发布](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布 nightly 构建，提供基于 dev 分支的 CUDA 13.0 预编译 wheel，支持 Linux amd64 和 arm64。

github · github-actions\[bot\] · 11月14日 09:48

**「解决的痛点」** 用户无需从源码编译即可在 CUDA 13.0 环境下安装并测试 LMCache 最新开发版本，尤其覆盖 ARM64 平台，简化了早期验证和部署流程。

**「背景与影响」** 该 nightly 版本属于 LMCache 项目的日常自动化构建，主要提供基于 dev 分支、面向 CUDA 13.0 的预发布 wheel，支持 linux/amd64 和 linux/arm64。LMCache 本身是一个面向大语言模型推理的 KV 缓存管理层，旨在将 KV 缓存从临时状态转化为可持久复用的知识，从而减少重复计算、降低延迟。此次发布未提及任何功能或性能变更，更像是一次基础设施/构建产物更新，为使用 CUDA 13.0 环境的开发者提供更便捷的安装渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache ! | LMCache</a></li>

</ul>
</details>

**标签**: `#llm-infrastructure`, `#cuda`, `#nightly`, `#release`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Nvidia CEO 辞职后 AI 交易或转向其他芯片商和云公司](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 8.0/10

Nvidia CEO 黄仁勋辞职后，ETF 专家认为 AI 投资可能转向其他芯片商和云公司。Yorkville Ives 将 Nvidia 目标价从 300 美元下调至 225 美元但维持买入，该股本周收于 162.85 美元。

rss · CNBC Finance · 11月14日 15:50

**「背景」** 民主党在 11 月 3 日中期选举后控制国会，可能放缓数据中心建设；Nvidia 临时 CEO 科莱特·克雷斯下周二将首次公布财报并安抚市场。

**标签**: `#Nvidia`, `#AI trade`, `#ETFs`, `#data centers`, `#semiconductors`

---

<a id="item-finance-news-2"></a>
### [Anthropic IPO 被曝拒绝中国内地及香港投资者下单](https://m.economictimes.com/markets/us-stocks/news/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed/articleshow/135809948.cms) ⭐️ 8.0/10

据知情人士称，Anthropic 的 IPO 不接受中国内地和香港投资者下单，限制与 ITAR（国际武器贸易条例）出口管制有关；该发行据报拟以 1.4 万亿美元估值募资至多 904 亿美元，定价日为 11 月 18 日，代码 ANT。

telegram · zaihuapd · 11月14日 10:18

**「背景」** 类似限制并非首次：SpaceX 在此前 IPO 中也曾以美国出口规则为由拒绝中国内地和香港投资者下单；Anthropic 此次限制被知情人士归因于 ITAR（国际武器贸易条例）。

**「影响」** 中国内地和香港投资者被排除在认购之外，部分资金据称转向英属维尔京群岛信托、SPV 和掉期结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thedailybugle.bartlettpublications.com/p/26-0616-tuesday-s-export-import-daily-bugle">26-0616: Tuesday&#x27;s &quot; Export /Import Daily Bugle&quot;</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#IPO`, `#export controls`, `#China`, `#valuation`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [SpaceX 首次用机械臂夹住回收二级飞船](https://x.com/op7418/status/2121756191495954772) ⭐️ 7.0/10

推文作者 @op7418 发布消息称，SpaceX 首次使用机械臂夹住并回收了二级飞船，并附上链接。推文原文为“🐂🍺 SpaceX 第一次用机械臂夹住回收了二级飞船”。除此之外，推文没有提供技术细节、任务编号或独立分析，仅作为该事件的简单公告。

twitter · 归藏\(guizang.ai\) · 11月15日 00:04

**「背景」** 这条推文称 SpaceX 首次使用机械臂夹住并回收了二级飞船。此前，SpaceX 已展示过用发射塔上的“筷子”机械臂（Mechazilla）回收第一级超重型助推器，例如在试飞中利用机械臂在空中接住返回的助推器（\[tool-1-1\]\[tool-1-2\]\[tool-1-3\]）。Starship 系统由超重型助推器和二级航天器组成，设计目标是完全可重复使用；机械臂回收是实现该目标的关键技术。推文未提供更多技术细节，社区评论暂无。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/roderick-beck-94868948_spacex-catches-starship-rocket-booster-in-activity-7253027931701080064-WUgI">SpaceX catches Starship rocket booster in historic test launch</a></li>
<li><a href="https://satfleetlive.com/blogs/spacex-starship/">SpaceX Starship : Next Flight, Full History &amp; Everything... | SatFleet Live</a></li>
<li><a href="https://www.france24.com/en/live-news/20241013-spacex-will-try-to-catch-giant-starship-rocket-shortly-before-landing">SpaceX successfully catches returning Starship booster... - France 24</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Starship`, `#space technology`, `#engineering`, `#news`

---

<a id="item-twitter-news-2"></a>
### [Pieter Levels：让用户上传家具照片生成 3D 物体](https://x.com/levelsio/status/2121712181125525706) ⭐️ 6.0/10

Pieter Levels \(@levelsio\) 在推特上提出，与其构建一个庞大的家具库，不如让用户上传自己想要的家具照片，然后使用图像转 3D 模型在 30 秒内生成 3D 物体。

twitter · @levelsio · 11月14日 21:09

**「背景」** 该推文发布于 2026 年 11 月 14 日，作者为 @levelsio。推文展示了将图像转 3D 生成技术用于用户上传内容的实际应用思路。

**标签**: `#AI`, `#3D generation`, `#user-generated content`, `#product design`

---

