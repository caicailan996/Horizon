---
layout: default
title: "Horizon Summary: 2026-10-29 (ZH)"
date: 2026-10-29
lang: zh
---

> 从 49 条内容中筛选出 26 条重要资讯。

---

**科技新闻**
1. [指纹脚本以混淆与蜜罐反制 AI 爬虫](#item-tech-news-1) ⭐️ 8.0/10
2. [MacBook Pro 推出 ProLED XDR 显示屏与触控支持](#item-tech-news-2) ⭐️ 8.0/10
3. [macOS 系统 git 仍信任已泄露的 eMudhra 证书](#item-tech-news-3) ⭐️ 8.0/10
4. [零训练注入空空间使 EmbeddingGemma-2 登顶 MAEB 音频](#item-tech-news-4) ⭐️ 8.0/10
5. [Anthropic 招聘经理停用编程面试](#item-tech-news-5) ⭐️ 8.0/10
6. [Google 提出睡眠框架防遗忘](#item-tech-news-6) ⭐️ 8.0/10
7. [Google 发布 Gemini 4 Carbon：面向长时程工程与网络安全](#item-tech-news-7) ⭐️ 8.0/10
8. [肯塔基人文主义者首次获 AI 宗教豁免](#item-tech-news-8) ⭐️ 7.0/10
9. [2026 年 10 月：用 vibe coding 做游戏迎来拐点](#item-tech-news-9) ⭐️ 7.0/10
10. [sched\_ext 微会议：聚焦优先级反转与跨虚拟机调度](#item-tech-news-10) ⭐️ 7.0/10
11. [将 LLM 编写的 Nordstjernen 浏览器引入 Linux 发行版的争议](#item-tech-news-11) ⭐️ 7.0/10
12. [企业 GPU 闲置过半仍计划采购 AI 平台](#item-tech-news-12) ⭐️ 7.0/10
13. [长鑫存储拟限量产 HBM3E，良率仅两三成](#item-tech-news-13) ⭐️ 7.0/10
14. [CNC 石材雕刻助力哥特式修道院建造](#item-tech-news-14) ⭐️ 6.0/10
15. [AI 代理税务评测：50 项专业任务](#item-tech-news-15) ⭐️ 6.0/10
16. [Emacs 迎来 50 周年：经典编辑器回顾](#item-tech-news-16) ⭐️ 6.0/10
17. [archive.today 被指重定向到可疑克隆站点，说法尚未证实](#item-tech-news-17) ⭐️ 6.0/10
18. [Ted Sanders 谈 LLM 规模与 OpenAI 版本号含义](#item-tech-news-18) ⭐️ 6.0/10
19. [GitHub Octoverse 2026：代理工程推动合并 PR 与提交量创新高](#item-tech-news-19) ⭐️ 6.0/10
20. [亚马逊工程领导：AI 工具帮不上忙也是发现，应记录并上报](#item-tech-news-20) ⭐️ 6.0/10
21. [Redox OS 完成 io\_uring 风格环形缓冲区支持](#item-tech-news-21) ⭐️ 6.0/10
22. [MIDA 基准：狼人杀测出多模态大模型社交盲区](#item-tech-news-22) ⭐️ 6.0/10
23. [通用反馈行与自写批评效果相当，缩减后见蒸馏所需特权信息](#item-tech-news-23) ⭐️ 6.0/10
24. [人机在鸡尾酒会语音上差距过小](#item-tech-news-24) ⭐️ 6.0/10
25. [Discord 公开服务器对话将被网络搜索](#item-tech-news-25) ⭐️ 6.0/10
26. [韩国以支付违规为由对苹果和谷歌合计罚款 4750 万美元](#item-tech-news-26) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [指纹脚本以混淆与蜜罐反制 AI 爬虫](https://nullpt.rs/fingerprinting-bioweapons) ⭐️ 8.0/10

hazebooth 于 2026 年 10 月 28 日在 nullpt.rs 发表技术深度分析，标题以“为什么这个指纹脚本会制造生物武器？”为切入点，拆解一个针对 AI 爬虫的指纹识别脚本。按分析摘要，该脚本疑似通过动态 JavaScript 混淆和蜜罐载荷识别、诱捕或反制 LLM 机器人，并引发关于反 AI 抓取军备竞赛的讨论；具体算法细节在当前材料中无法进一步核实。

hackernews · hazebooth · 10月28日 17:13 · [社区讨论](https://news.ycombinator.com/item?id=50276998)

**「背景」** 为应对 LLM 爬虫的自动抓取，许多网站会使用浏览器指纹识别、JavaScript 混淆和蜜罐脚本来识别非人类流量，并让这些爬虫在抓取过程中被诱导或阻断。这篇分析针对的正是这样一个混淆过的指纹识别脚本，它被设计用来检测和反制 AI 爬虫，属于当前反 LLM 抓取对抗中的典型做法。

**「社群讨论」** 评论中，jacquesm 分享了一次因文档水印未移除导致客户文件被系统长期隔离的真实经历，提醒这类标记机制可能误伤正常流程；ghm2199 则将动态混淆与蜜罐描述为“疯狂的军备竞赛”，并质疑 LLM 是否真的会在上下文窗口中大规模执行此类抓取，从而让这种对抗值得投入。

**标签**: `#anti-crawler`, `#LLM bots`, `#obfuscation`, `#fingerprinting`, `#web security`

---

<a id="item-tech-news-2"></a>
### [MacBook Pro 推出 ProLED XDR 显示屏与触控支持](https://www.apple.com/macbook-pro/proled-xdr-display/) ⭐️ 8.0/10

苹果于 2026 年 10 月 28 日发布新一代 MacBook Pro，核心变化是配备 ProLED XDR 显示屏并加入触控支持。官方将其称为突破性更新，但这一发布目前仍属于厂商宣布，尚未看到独立评测验证实际显示效果与触控体验。具体机型规格、价格和上市时间仍需以官方后续信息为准。

hackernews · etothet · 10月28日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=50276940)

**「背景」** 苹果此前的 MacBook 一直不提供触控屏，部分原因是高管多年来基于人体工学的反对。10 月 26 日的日报曾收录彭博社的报道，称苹果计划推出首款触控屏 MacBook Pro，配备 OLED 显示屏与灵动岛，提供 14 英寸和 16 英寸两种尺寸，且起售价将高于当时的 2,499 美元。苹果官方新闻稿随后正式确认了这一发布，并将新屏幕命名为 PROLED XDR，说明其基于串联 OLED 技术。

**「社区讨论」** 有评论认为触控 Mac 是“糟糕的发展”，因为 macOS 现有界面控件对手指来说太小且不适配，可能带来误触和 bug；也有评论更关注硬件改进，称 14 英寸和 16 英寸机型重量分别降至约 3.0 磅和 4.0 磅，OLED 面板取消背光层是减重原因之一。另有用户质疑笔记本触控的实际需求，并担心屏幕容易沾上指纹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/newsletters/2026-10-25/apple-to-unveil-touch-screen-macbook-pro-executive-promotions-in-box-checker">2026-10-26 — Apple to Unveil First Touchscreen MacBook Pro With OLED, Dynamic Island</a></li>
<li><a href="https://www.apple.com/newsroom/2026/10/apple-unveils-groundbreaking-macbook-pro-with-proled-xdr-display/">Apple unveils groundbreaking MacBook Pro with PROLED XDR Display</a></li>

</ul>
</details>

**标签**: `#Apple`, `#MacBook Pro`, `#hardware`, `#display technology`, `#touchscreen`

---

<a id="item-tech-news-3"></a>
### [macOS 系统 git 仍信任已泄露的 eMudhra 证书](https://emudhra.we-have-a-problem.com/apple.html) ⭐️ 8.0/10

Apple 在 macOS 中随系统安装的 git 目前仍信任已泄露/吊销的 eMudhra 证书。官方缓解手段是手工编辑证书链，但这种修改可能被后续 macOS 系统更新还原，从而重新引入漏洞；受影响者主要是依赖系统 git 或系统证书库的 macOS 开发者。

hackernews · galadran · 10月28日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=50271640)

**「背景」** eMudhra 的八个中级 CA 私钥此前被泄露，其中六个用于签发 TLS 证书，攻击者可能借此伪造看似有效的任意网站证书；eMudhra 与 Sectigo 已吊销受影响证书。Apple 的支持文档确认，macOS 自带的 curl、git、python3、ruby、perl、openssl 等命令行工具使用 /etc/ssl/cert.pem 检查证书链，因此会信任指向该文件中根 CA 的证书，而不检查 Apple 的封锁列表或吊销状态。这意味着除非用户手动修改证书链，系统 git 等工具仍会信任已泄密的 eMudhra 证书，而后续系统更新可能还原修改。

**「影响」** 受影响的开发者应主动应用 Apple 的修补措施，并在每次 macOS 系统更新后确认修补没有被回滚；否则系统自带 git 及相关命令行工具仍可能暴露于针对已泄露 eMudhra 证书的攻击。

**「社区讨论」** 评论者 chrisweekly 指出受影响的不仅是 git，而是所有信任 macOS 系统证书库的工具；jrochkind1 批评操作系统级证书管理长期混乱。truelson 和 qaz\_plm 转贴了 Apple 官方修补说明，faxmeyourcode 则猜测弱密钥可能是情报机构有意促成，但他也承认目前没有证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/149555">About the compromised eMudhra intermediate CAs - Apple Support</a></li>
<li><a href="https://github.com/Steff81/apple_eMudhra_removeScript">GitHub - Steff81/apple_eMudhra_removeScript: Removes and ...</a></li>

</ul>
</details>

**标签**: `#security`, `#certificates`, `#macOS`, `#git`, `#PKI`

---

<a id="item-tech-news-4"></a>
### [零训练注入空空间使 EmbeddingGemma-2 登顶 MAEB 音频](https://www.reddit.com/r/MachineLearning/comments/1xho7pr/r_taking_embeddinggemma2_577m_from_rank_26_to_1/) ⭐️ 8.0/10

一项零训练方法通过 PCA 将中间 Conformer 层的特征压缩至 256 维，并注入 EmbeddingGemma-2（577M）最终投影矩阵的 256 维零空间中，使该模型在 MAEB 音频基准上的宏平均得分从 49.3%升至 54.4%（+5.1 分），排名从第 26 位升至第 1 位，超过了 8B-9B 多模态模型。文本嵌入保持不变，文本到音频检索分数变化在 0.05 分以内；但该方案无法继续使用 Matryoshka 式截断，且以语义为主的任务会出现下降，例如口语句子主题分类从 57.2%降至 21.3%，口语意图识别从 97.6%降至 88.3%。权重已发布在 Hugging Face 上。

reddit · r/MachineLearning · /u/JeanMichelRanu · 10月28日 13:34

**「背景」** Google 于 2026 年 10 月上旬发布开源多模态嵌入模型 EmbeddingGemma 2，采用 Apache 2.0 许可，将文本、图像、视频帧和音频映射到统一向量空间用于本地检索（10 月 7 日的日报曾报道）。10 月 14 日的日报记载，一位开发者曾利用该共享文本/音频向量空间把 EmbeddingGemma 2 改造成实验性的本地语音转文字模型；本贴用 PCA 向该音频模型的 256 维零空间注入中间层特征，属于对这一向量空间的进一步挖掘。

**「影响」** 使用音频嵌入的开发者可以在不重新训练的情况下获得性别聚类、艺术家检索、情感识别和环境声音分类等副语言与声学任务的显著提升；但对于需要忽略说话人音色的语义型音频任务，应避免直接采用该权重，或需要额外权衡语义分量被缩放带来的损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eg2.haku.sh/">2026-10-14 — EmbeddingGemma 2 turned into an experimental local speech-to-text model</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/">2026-10-07 — EmbeddingGemma 2: Google&#x27;s open multimodal embedding model</a></li>

</ul>
</details>

**标签**: `#audio embeddings`, `#MAEB`, `#null space`, `#PCA`, `#representation learning`

---

<a id="item-tech-news-5"></a>
### [Anthropic 招聘经理停用编程面试](https://felixrieseberg.com/hunger-beats-tenure-advice-for-junior-engineers/) ⭐️ 8.0/10

Anthropic 招聘经理 Felix Rieseberg 本月停止在面试中考核编程题。他表示，Claude 对这类题目的表现已经超过候选人，写代码不再是有效的筛选标准；他还举出两名新人在一个周末为 Claude Code 的图形界面做出原型、约八天后发布首个公开版本的例子，以此说明执行力比资历更影响实际产出。该说法属于招聘经理的个人判断，并不代表 Anthropic 的全公司政策。

telegram · zaihuapd · 10月28日 01:46

**「背景」** 编程面试是科技行业长期使用的候选人筛选方式，通常通过算法题或白板题考核候选人的代码能力。随着 Claude 等 AI 编程工具的性能提升，业界开始重新评估这类面试是否仍能有效筛选工程能力，而本文正是这一讨论中的具体案例。Anthropic 的 Claude Code 是该公司面向开发者的编程代理产品，文中提到的图形界面原型由初级工程师在短期内完成，也是公司内部对 AI 辅助开发效能的一种验证。

**「影响」** 在 Felix Rieseberg 负责的招聘流程中，候选人将不再被要求现场写代码；软件工程师求职者应准备好展示利用 AI 工具快速做出可演示原型的能力，而非只展示算法或编程题表现。

**标签**: `#Anthropic`, `#hiring practices`, `#AI-assisted development`, `#Claude`, `#software engineering`

---

<a id="item-tech-news-6"></a>
### [Google 提出睡眠框架防遗忘](https://research.google/blog/the-sleep-framework-a-new-way-for-llms-to-retain-knowledge-in-continual-learning/) ⭐️ 8.0/10

Google Research 提出“睡眠框架”（Sleep Framework），在持续学习中让大语言模型交替进行主动交互和离线巩固，将短期上下文固化为长期参数，以缓解灾难性遗忘。研究博客称，该框架在 1000 万 token 长上下文、持续翻译和数学推理等任务上超过 GPT-4、SFT 等基线；这些属于研究报告中的实验结果，并非独立验证或已发布的产品能力。

telegram · zaihuapd · 10月28日 01:46

**「背景」** 持续学习要求模型在接收新任务或新数据后仍保留此前学到的能力；若只做普通微调，新知识往往会覆盖旧参数，导致旧任务表现下降，即“灾难性遗忘”。睡眠框架的做法是在主动学习阶段之外加入离线巩固阶段，把短期积累的信息整理进模型长期参数，对应了来源中“短期上下文巩固为长期参数”的描述。

**标签**: `#continual learning`, `#LLM`, `#catastrophic forgetting`, `#Google Research`, `#AI research`

---

<a id="item-tech-news-7"></a>
### [Google 发布 Gemini 4 Carbon：面向长时程工程与网络安全](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) ⭐️ 8.0/10

Google 发布新一代前沿模型 Gemini 4 Carbon，宣称其在长时程自主工程与网络安全任务上明显提升：与前代 Argon 相比，安全代码生成成功率提高超过 2 倍，高严重性错位警报下降近 80%，并在 SEC-bench Pro 上取得 88.2%。该模型以 introductory 价格提供（输入 $2/百万 token、输出 $10/百万 token，与 Argon 相同，后续将翻倍），但目前仅向部分网络安全防御者和可信合作伙伴（含美国政府预发布测试）开放，尚未面向开发者、企业与消费者广泛提供；上述性能均为官方口径，尚未独立验证。

telegram · zaihuapd · 10月28日 17:09

**「背景」** Horizon 10 月 1 日的日报曾报道 Google 推出 Gemini 4 Argon，称其具备代理能力并已在内部协助将 C/C++ 代码迁移至 Rust，但当时尚未向开发者、企业和消费者广泛开放；10 月 14 日的日报则记载 Argon 正式发布后，早期 API 用户给出积极评价，同时免费层级访问存在摩擦，部分用户被重定向到旧版本而无法升级。此次发布的 Gemini 4 Carbon 正是 Argon 的直接后继，并在安全代码生成等指标上以前代作为对照。

**「社区讨论」** 评论区对“先展示基准、再逐步开放”的策略提出质疑，有用户认为等到模型广泛可用时竞争对手可能更强，基准意义有限；也有用户抱怨命名与获取路径混乱，例如在 Gemini 应用中仍未看到 Argon，且 Argon 此前发布后延迟开放。另有评论建议前沿模型采用统一的 Ultra/Pro/Flash/Lite 分层命名，以减少选择困惑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">2026-10-01 — Google introduces Gemini 4 Argon with Rust migration agents</a></li>
<li><a href="https://deepmind.google/models/gemini/">2026-10-14 — Gemini 4 Argon draws early praise but access friction</a></li>

</ul>
</details>

**标签**: `#google`, `#gemini`, `#ai-models`, `#cybersecurity`, `#agentic-ai`

---

<a id="item-tech-news-8"></a>
### [肯塔基人文主义者首次获 AI 宗教豁免](https://religionnews.com/2026/10/26/in-a-first-a-humanist-granted-a-religious-exemption-from-using-ai/) ⭐️ 7.0/10

据 Religion News 10 月 26 日报道，肯塔基州一名人文主义者成为已知首位以宗教豁免为由获准不使用人工智能的人，这被视为把世俗人文主义信仰认定为拒绝使用 AI 之合法依据的首例。报道未披露作出豁免的雇主、处理机构或具体程序，也未说明该结果是行政协商还是法院裁定，因此该先例的实际适用范围仍不明确。

hackernews · danso · 10月28日 13:41 · [社区讨论](https://news.ycombinator.com/item?id=50273396)

**「背景」** 此前已有类似的先例：2025 年，一位一神论普救派软件工程师 Erin Maus 以宗教理由反对在工作中使用 AI，并于当年 5 月获得雇主的宗教豁免。本次肯塔基州的案例则是人文主义者首次因信仰获得 AI 使用豁免，其所属大学于 9 月同意给予宗教便利。

**「影响」** 依据工具检索结果，软件工程师 Erin Maus 成为已知首位依据《民权法》第七章（Title VII）获得宗教便利、免于在工作中使用 AI 的美国员工，这为同类宗教或信念异议提供了可引用的先例。与此同时，美国最高法院已降低宗教便利请求的举证门槛，雇主要对员工的宗教实践作出合理通融，而非仅简单拒绝；因此，要求员工使用 AI 的企业可能需要评估这类请求，并准备不依赖 AI 的替代工作流程。

**「社区讨论」** 评论中的主要分歧在于这件事的分量：有评论者认为该请求“小而合理”，人力资源部门经常处理类似通融，因此算不上重大事件；另一些评论则担心这可能催生“类阿米什”式的技术拒绝群体，并质疑法律如何界定受保护的核心信仰与一般偏好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/maureen-pritchard-phd-106b7234_she-won-an-exemption-from-using-ai-at-her-activity-7469026315183009792-6_Sb">Unitarian Universalist Secures Religious Exemption from AI Use at...</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/now-religious-exemption-using-ai-200105422.html?guccounter=1">You Can Now Get a Religious Exemption From Using AI at Work</a></li>
<li><a href="https://www.linkedin.com/posts/alexisdufresne_erin-maus-secures-title-vii-ai-exemption-activity-7472699930638315520-KBeh">US Worker Wins Religious Exemption from AI Use at Work | LinkedIn</a></li>
<li><a href="https://www.troutman.com/insights/scotus-overturns-title-vii-precedent-lowering-bar-for-religious-accommodations/">SCOTUS Overturns Title VII Precedent , Lowering Bar for Religious ...</a></li>

</ul>
</details>

**标签**: `#ai policy`, `#law`, `#humanism`, `#society`, `#ethics`

---

<a id="item-tech-news-9"></a>
### [2026 年 10 月：用 vibe coding 做游戏迎来拐点](https://simonwillison.net/2026/Oct/28/vibe-game-development/) ⭐️ 7.0/10

Simon Willison 在 2026 年 10 月 28 日的文章中提出，vibe coding（完全不看代码地让人工智能开发软件）制作电脑游戏已到达新的拐点，尤其是 Claude Opus 5.5 在 3D 建模、音乐生成和游戏设计上的明显进步。他称自己近几周用这一方式完成了四款真正玩起来有趣的浏览器游戏（HTML/JavaScript），其中《Tree Appreciator》仅靠一段提示、未加迭代就生成了基于 three.js 的找不同游戏，《Emberwick》则是一个可探索的俯视 RPG 原型。他也说明这只是个人印象，认为 GPT-6 Astra 尚不能达到 Opus 5.5 的“手感”，预计 OpenAI 年内会追上。

rss · Simon Willison · 10月28日 13:55

**「背景」** 在 Horizon 9 月 28 日的日报中，Willison 曾把 2025 年 11 月视为编码代理的拐点：Claude Opus 4.5 与 GPT-5.1 配合代理框架后，已成为软件工程师日常可用的可靠工具。本文延续这一判断，宣称 2026 年 10 月是“vibe coding”游戏开发的新拐点。

**「影响」** 对独立开发者或有兴趣的工程师而言，制作可玩、有美感的 3D 网页小游戏的门槛已经明显降低：这类作品可以直接在浏览器中运行、不需要专门游戏引擎，甚至普通 Claude 聊天界面也能完成单轮生成。若想复现类似结果，可优先尝试 Opus 5.5 与 three.js，并在提示中明确要求“更有趣”；但仍需把结果视为作者的主观体验，而非独立基准测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/">2026-09-28 — Simon Willison&#x27;s 2026 LLM keynote: coding agents reached daily-use reliability</a></li>

</ul>
</details>

**标签**: `#vibe coding`, `#AI coding agents`, `#game development`, `#AI-assisted software engineering`, `#Simon Willison`

---

<a id="item-tech-news-10"></a>
### [sched\_ext 微会议：聚焦优先级反转与跨虚拟机调度](https://lwn.net/Articles/1103426/) ⭐️ 7.0/10

Linux Plumbers Conference 在布拉格举行的 sched\_ext 微会议报告显示，讨论集中在三个主题：优先级反转处理，包括锁持有者与锁等待者的抢占、时间片延长，以及让代理执行与 BPF 调度器协同；跨虚拟机边界的半虚拟化调度，以 sched\_ext 作为宿主机上的策略引擎；以及利用 Intel HFI、设备或加速器局部性和缓存拓扑进行硬件与拓扑感知的任务放置。该内容来自会议报告，属于讨论方向而非已经合入内核的实现。

rss · LWN.net · 10月28日 22:11

**「背景」** sched\_ext 是 Linux 内核中一个可扩展的调度框架，允许开发者用 BPF 程序定义和替换 CPU 调度策略。据 Horizon 10 月 19 日的日报，Linux 7.3 内核发布时已完成了 sched\_ext 子调度器（subscheduler）特性。本次在布拉格举行的 Linux Plumbers Conference sched\_ext 微会议在此基础上，讨论了三个主题：优先级反转的处理（包括代理执行与 BPF 调度器的结合）、让宿主机与虚拟机调度器协作的半虚拟化调度，以及利用硬件反馈（如 Intel HFI）和设备/缓存拓扑来驱动任务放置。

**「影响」** 内核与 BPF 调度器开发者可以把代理执行、半虚拟化调度协作和硬件反馈机制纳入后续开发路线图；若要跟进实际进展，应关注相关的补丁和邮件列表讨论，而不是仅依据此次会议报告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1101143/">2026-10-19 — Linux 7.3 kernel released with record commit count</a></li>

</ul>
</details>

**标签**: `#linux-kernel`, `#sched\_ext`, `#BPF`, `#scheduling`, `#conference-report`

---

<a id="item-tech-news-11"></a>
### [将 LLM 编写的 Nordstjernen 浏览器引入 Linux 发行版的争议](https://lwn.net/Articles/1102738/) ⭐️ 7.0/10

LWN 报道称，一项试图将 LLM 编写的 Nordstjernen 浏览器纳入 Debian 和 Arch Linux 发行版的推广活动，引发了外界对项目开发与安全流程的质疑。Nordstjernen 被视为主流 Blink、Gecko 或 WebKit 之外的新兴开源浏览器引擎候选，但围绕其如何通过发行版审查的问题尚无明确结论。

rss · LWN.net · 10月28日 14:26

**「背景」** Nordstjernen 是一个用 C 语言从零编写的开源浏览器，采用 GPL-3 许可、无 JIT 设计，主打对 HTML 和 CSS 标准的支持，并被视为 Chromium 和 Firefox 之外的独立替代品。其作者 Andreas Røsdal 已向 Debian 提交软件包引入申请，而 Debian 此前就曾质疑这个由 LLM 构建的浏览器的版权问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://freenode.net/article/debian-questions-copyright-of-llm-built-northstar-browser">Debian questions copyright of LLM -built Northstar browser · freenode</a></li>
<li><a href="https://nordstjernen.org/">Nordstjernen Web Browser</a></li>

</ul>
</details>

**标签**: `#Linux`, `#open source`, `#web browsers`, `#LLM code generation`, `#software security`

---

<a id="item-tech-news-12"></a>
### [企业 GPU 闲置过半仍计划采购 AI 平台](https://venturebeat.com/infrastructure/ai-bubble-update-79-of-companies-say-their-gpus-sit-idle-at-least-half-the-time-yet-most-plan-new-ai-platforms) ⭐️ 7.0/10

VentureBeat 发布的企业调研显示，79% 受访企业的 GPU 平均利用率不足 50%，91% 的 AI 基础设施投入从未经过财务部门的正式 ROI 审计；尽管如此，70% 处于低利用率状态的企业仍计划在未来 12 个月内继续采购并部署新的 AI 计算平台。该结果反映企业 AI 算力采购与回报管理之间存在明显脱节，但属于调研披露而非独立测量结果。

telegram · zaihuapd · 10月28日 02:37

**「背景」** 这份调研讨论的是企业 AI 基础设施投入中算力采购与回报审计脱节的问题。可供参照的近期市场变化是 GPU 租赁价格的普遍上行：Horizon 10 月 26 日的日报曾报道 a16z 的租赁价格指数显示，自 2026 年初以来 H200 租金累计上涨约 160%、B200 约 120%、RTX PRO 6000 约 65%，价格压力为企业继续采购算力提供了现实动机。本次调研则从利用率与财务审计角度量化了这一采购行为的效率代价。

**「影响」** 对计划继续扩容 AI 算力的企业而言，调研结果意味着应先把 GPU 利用率和投资回报纳入财务审计流程，避免在现有算力大量闲置的情况下重复采购；缺乏审计机制会使资本开支的真实回报难以核实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/a16z/status/2113741008550990191">2026-10-26 — GPU Rental Prices Rise Broadly, Including Older A100, per a16z Index</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#GPU utilization`, `#enterprise AI`, `#ROI`, `#AI spending`

---

<a id="item-tech-news-13"></a>
### [长鑫存储拟限量产 HBM3E，良率仅两三成](https://www.reuters.com/world/china/chinas-cxmt-start-advanced-ai-memory-production-despite-poor-yields-sources-say-2026-10-28/) ⭐️ 7.0/10

路透社援引两名知情人士称，长鑫存储（CXMT）已向多家国内 AI 芯片设计公司送样 HBM3E，并计划未来两个月内限量生产；其良率仅 20% 至 30%，明显低于 SK 海力士约 70% 的水平。测试显示该产品性能更接近 SK 海力士上一代 HBM3，预计售价也高于海外同类产品。这是媒体报道的企业计划，尚不代表已量产或达到同级性能。

telegram · zaihuapd · 10月28日 06:19

**「背景」** HBM3E 是高带宽内存（HBM）的新一代规格，AI 加速器在高强度训练与推理中依赖这类器件提供大容量、高带宽的存储。在美国出口管制导致国内 AI 内存供应短缺的背景下，国产 DRAM 厂商长鑫存储计划以自研 HBM 限量生产来填补这一缺口。

**「影响」** 对美国出口管制下难以获得海外高端 HBM 的国内 AI 芯片设计公司而言，这提供了一个性能折中、价格更高的国产替代选项；但两至三成良率表明首批可供应量有限，实际交付规模仍待验证。

**标签**: `#HBM`, `#semiconductors`, `#AI hardware`, `#China`, `#memory`

---

<a id="item-tech-news-14"></a>
### [CNC 石材雕刻助力哥特式修道院建造](https://carmelitegothic.com/cnc-stone-carving/) ⭐️ 6.0/10

10 月 28 日发表的一篇文章介绍了 CNC 石材雕刻技术在哥特式修道院建造中的应用。文章展示了一座现代哥特式修道院如何借助数控加工完成石材切割与雕刻，并说明这种技术如何与手工石雕传统结合。受文章启发的评论还提到，类似做法在巴塞罗那圣家堂的建造中已实践多年。

hackernews · bschne · 10月28日 14:38 · [社区讨论](https://news.ycombinator.com/item?id=50274409)

**「背景」** 新芒特卡梅尔基金会（New Mount Carmel Foundation）正在怀俄明州建造一座哥特式修道院，其中使用数控加工设备将多吨重的花岗岩板材雕刻成哥特式建筑构件。项目方解释称，选择花岗岩正是因为这种坚硬耐久的石材历来难以手工实现哥特式风格的精细雕饰，而 CNC 加工让这种细节成为可能；该项目也曾被制造行业刊物《Modern Machine Shop》报道。

**「社区讨论」** 评论中最有价值的背景来自 soci：圣家堂的石匠自 1990 年代初就开始使用 CNC 进行石料粗加工，再以手工精修，并非完全自动化。wolframhempel 则指出，雕塑家从古埃及的网格放样、罗马时代的模具翻制到 18 世纪的刻点机，一直试图用工具节省工时，因此不能简单认为 CNC 削弱了艺术的人性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newmountcarmelfoundation.org/the-chapel-carving-granite/">The Chapel: Carving Granite - New Mount Carmel Foundation</a></li>
<li><a href="https://newmountcarmelfoundation.org/monastery-stone-carving-article/">Monastery featured in Modern Machine Shop - New Mount Carmel ...</a></li>

</ul>
</details>

**标签**: `#CNC`, `#stone carving`, `#hardware`, `#manufacturing`, `#gothic architecture`

---

<a id="item-tech-news-15"></a>
### [AI 代理税务评测：50 项专业任务](https://surgehq.ai/blog/dayjob-tax) ⭐️ 6.0/10

SurgeHQ 于 2026 年 10 月 28 日发布博客《Dayjob: Tax》，介绍一个用 50 项专业税务任务衡量 AI 代理的评测基准，面向关心 AI 报税可靠性的开发者与纳税人。该内容是第三方基准评估，而不是可直接使用的税务软件，评论区的反应也表明实际可靠性仍有争议。

hackernews · landonxi · 10月28日 15:46 · [社区讨论](https://news.ycombinator.com/item?id=50275626)

**「背景」** DAYJOB 是 SurgeHQ 评估 AI 智能体在专业任务中表现的一系列基准，此前已覆盖医疗和金融领域；本次 Tax 版把相同方法扩展到税务准备、合规与咨询服务。据公开介绍，该基准包含 50 个环境、横跨八个税务实务领域，并提供 1,789 个工作区文件（如 PDF、Excel 工作簿和手写收据）；排行榜按 pass@1 且 95% 评分阈值计分，目前领先的 Claude Sonnet 5.5 通过率也仅约 10.8%。

**「影响」** 对有复杂税表的纳税人而言，社区实例显示 AI 能帮助发现错误，也会在字段填写和退税计算上出错，因此在未经税务专业人士复核前不宜直接提交 AI 生成的申报结果。

**「社区讨论」** 评论者提供了相反的真实体验：有人称用 AI 辅助报税后发现了自身错误，也有人报告 AI 生成的申报表曾被会计师退回并低估退税近 2000 美元；另有网友质疑该评测是否只是把文档交给通用代理后观察结果，缺少方法学细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://surgehq.ai/blog/dayjob-tax">DAYJOB: Tax — Benchmarking AI Agents on Professional Tax Work</a></li>
<li><a href="https://daily.dev/posts/dayjob-tax-evaluating-ai-agents-on-50-professional-tax-assignments-tknynvr2r">Dayjob: Tax – evaluating AI agents on 50 professional tax ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#benchmarking`, `#LLM evaluation`, `#tax software`

---

<a id="item-tech-news-16"></a>
### [Emacs 迎来 50 周年：经典编辑器回顾](https://www.technologyreview.com/2026/10/20/1145399/emacs-turns-50/) ⭐️ 6.0/10

2026 年 10 月 20 日，MIT Technology Review 刊发回顾文章，纪念开源编辑器 Emacs 诞生 50 周年。文章属纪念性盘点而非新版本或新功能发布；Hacker News 讨论中，多名长期用户分享了数十年使用经历，并强调 Emacs 仍在活跃开发，Magit、ghostel 等外部包已成为日常工作流的一部分。

hackernews · internet\_points · 10月28日 13:25 · [社区讨论](https://news.ycombinator.com/item?id=50273171)

**「背景」** Emacs 是软件史上仍在活跃使用的古老文本编辑器之一，其历史可追溯到 1970 年代中期，以高度可扩展性和内置 Lisp 扩展机制著称。本篇文章在 Emacs 诞生 50 周年之际回顾其数十年来的发展历程。

**「社区讨论」** 评论里有长期用户把 Emacs 当作个人与职业生活的中枢，也有用户提出是否应刻意保持配置精简的疑问；后一类用户表示扩展和 org-mode 的全能性反而造成复杂性负担，并提到更喜欢 Plan 9 的 Sam 和 Acme。另有观点认为，Evil 模式、LSP 支持和终端模拟包没有削弱 Emacs，反而让它保持现代感。

**标签**: `#emacs`, `#open source`, `#software history`, `#editors`

---

<a id="item-tech-news-17"></a>
### [archive.today 被指重定向到可疑克隆站点，说法尚未证实](https://www.reddit.com/r/Seattle/comments/1xhf6qp/archivetoday_links_going_forward/) ⭐️ 6.0/10

10 月 28 日，Reddit r/Seattle 的一则帖子称 archive.today（即 archive.is）会把用户重定向到可疑甚至恶意站点；发帖者 consumer451 随后澄清这只是“声称发现”，没有外部验证，也没有技术分析。讨论中，社区成员 surround 报告了一次复现：在 archive.ph/jXv3A 页面点击 “Filed on Tuesday” 链接后，被重定向到 stolidityseashellshotter\[.\]com，再进入仿冒 RT 新闻的 rurtnews\[.\]com，但未进入恶意软件站点。该说法在 Hacker News 上引发谨慎讨论，目前没有官方确认。

hackernews · consumer451 · 10月28日 15:31 · [社区讨论](https://news.ycombinator.com/item?id=50275373)

**「背景」** archive.today（又称 archive.is）是一种常用的网页存档服务，用户点击存档快照时通常会被导向该服务自身域名下的页面。此前已有 Reddit 社区报告称，在特定来源头（referer）指向 removepaywall.com 的情况下，访问 archive.is 会被重定向到 RT 新闻网站；这次有关 archive.today 可能重定向到可疑或恶意站点的说法，因此并非完全没有先例，但仍缺少技术细节与独立验证。

**「影响」** 由于 Reddit 版主和发帖者都未提供可核验的细节，用户暂时无法判断风险范围；已有讨论者表示不会再使用 archive.today。在 archive.today 方面或独立安全团队给出说明前，点击归档链接时应保持谨慎。

**「社区讨论」** surround 给出了上述复现路径，认为至少会出现跳转到仿冒 RT 网站的情况；avidruntime 猜测问题可能来自被归档页面嵌入的 JavaScript，在 archive 的渲染过程中让用户看到与原始页面不同的内容，而不是 archive 本身主动投放恶意软件。lxe 则提到此前有过类似事件，并附上了旧报道和 HN 讨论链接；efficax 认为缺少证据，并表示不会再使用该服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.redditmedia.com/r/cybersecurity/comments/1jlqyyi/is_archiveis_archivetoday_compromised_redirect_to/">Is Archive.is / Archive.today Compromised? Redirect to Russia ...</a></li>

</ul>
</details>

**标签**: `#security`, `#archive.today`, `#web archiving`, `#malware`, `#community discussion`

---

<a id="item-tech-news-18"></a>
### [Ted Sanders 谈 LLM 规模与 OpenAI 版本号含义](https://simonwillison.net/2026/Oct/28/ted-sanders/) ⭐️ 6.0/10

Simon Willison 引述 OpenAI 的 Ted Sanders 在 Hacker News 上的解释：LLM 性能虽然高度多维，但模型规模是主要变量，更大的模型通常更可靠、每 token 成本更高，并对冷门事实有更好的回忆。他还说明 OpenAI 的版本号同时承载发布顺序、与同系列版本的关系以及改进幅度，例如 6.1 代表在 5.6 之后发布、与同类 6.1 模型共享训练数据和性格，但改进幅度还不足以命名为 7。

rss · Simon Willison · 10月28日 23:23

**「背景」** 大型语言模型厂商通常以系列名加版本号来标识模型代际，但版本数字究竟表示能力排序还是发布顺序，外界并不总是清楚。Ted Sanders 的这段表态是对 OpenAI 模型命名惯例的一次公开说明。

**「影响」** 对 AI 开发者而言，选型时宜把版本号和模型规模视为相对信号而非绝对能力排序：更大、更新的模型往往更可靠但成本更高，而不同任务维度上的表现可能并不一致，仍需按具体场景实测。

**标签**: `#llm`, `#model-scaling`, `#ai-versioning`, `#machine-learning`

---

<a id="item-tech-news-19"></a>
### [GitHub Octoverse 2026：代理工程推动合并 PR 与提交量创新高](https://simonwillison.net/2026/Oct/28/github-octoverse-2026/) ⭐️ 6.0/10

GitHub 在 2026 年 GitHub Universe 上发布了 Octoverse 年度报告，EVP Jay Parikh 宣布的数据显示，目前每月合并约 2.2 亿个 PR、产生 73.8 亿次提交，并新建 3030 万个仓库。报告将增长主要归因于代理式工程：合并 PR 在不到一年内增至三倍，提交量增至三倍以上，且大部分增幅发生在 2026 年下半年；这些是 GitHub 官方发布的平台指标，而非独立测量结果。

rss · Simon Willison · 10月28日 16:45

**「背景」** GitHub Octoverse 是 GitHub 每年发布的开发者活动年度报告，通常在 GitHub Universe 大会上公布，用于观察跨年度的开发趋势。今年的报告以 agentic engineering 为主线，新增了按行业以及按“互操作性或逆向工程”相关关键词划分的公共仓库统计，并说明其采用了 LLM 分类与嵌入模型等方法来识别地区、行业和互操作性相关仓库。

**标签**: `#GitHub`, `#Octoverse`, `#Developer Metrics`, `#AI Agents`, `#Open Source`

---

<a id="item-tech-news-20"></a>
### [亚马逊工程领导：AI 工具帮不上忙也是发现，应记录并上报](https://simonwillison.net/2026/Oct/28/terk-terkowitz/) ⭐️ 6.0/10

亚马逊工程领导 Terk Terkowitz 在一份关于开发者在 AI 时代角色的更新中告诉工程师：如果当前 AI 工具没有让你的工作受益，这是一个“发现”而不是“失败”。工程师应记录原因、与同行分享、向经理反馈，并共同寻找解决方案；能够解释 AI 尚不能帮助之处，被视为展示了公司要求的判断力。这属于一份面向亚马逊工程师的指导性说明，并非某个产品功能或可验证的技术成果。

rss · Simon Willison · 10月28日 10:09

**「背景」** Terk Terkowitz 在亚马逊工程领导层面向开发者的 AI 角色指南中，将“AI 工具尚未帮助到当前工作”定义为一种需要记录、分享并上报的发现，而不是工程师的个人失败。这项表述来自亚马逊官方公告《An update from Amazon engineering leadership on the role of the developer in the age of AI》，属于对工程师预期和工作方式的正式说明。

**「影响」** 对亚马逊软件工程师而言，这项指导把“指出 AI 工具的局限”纳入期望行为：工程师需要把工具帮不上忙的实际案例主动上报给同事和管理者，而不是回避或隐藏。这也意味着在内部讨论和评估中，说明“哪里无法使用 AI”可能被视为判断力的一部分，而不仅仅是抱怨或负面反馈。

**标签**: `#amazon`, `#generative-ai`, `#software-engineering`, `#ai-tooling`, `#agentic-engineering`

---

<a id="item-tech-news-21"></a>
### [Redox OS 完成 io\_uring 风格环形缓冲区支持](https://lwn.net/Articles/1103359/) ⭐️ 6.0/10

Redox OS 项目发布报告，称其获得 NLnet 资助、为期一年的 io\_uring 风格环形缓冲区工作已于九月完成：在系统任务层实现了环形缓冲区机制，并完成了可供应用使用的 io\_uring/liburing 风格 API。项目还补充了驱动异步执行器等支持 crate，并改善了应用与系统服务之间的切换性能。该结论来自项目自述，尚缺少独立验证。

rss · LWN.net · 10月28日 14:05

**「背景」** io\_uring 是 Linux 上的异步 I/O 接口，通过应用与内核之间的环形缓冲区提交和完成请求，从而减少系统调用开销。Redox OS 是用 Rust 编写的类 Unix 微内核操作系统，本次工作是“应用与多数系统服务之间环形缓冲通信”的第一步，即在系统任务层提供类似机制，并给出配套的应用层 API。

**「影响」** 对 Redox OS 的应用和驱动开发者而言，现在可以使用类似 liburing 的 API 发起异步 I/O，并由新增的驱动异步执行器承担配套调度。需要注意的是，这是 Redox 自己的兼容实现而非 Linux io\_uring 的直接移植，具体 API 命名和行为可能存在差异；能否使用取决于所对接的系统服务或驱动是否已支持环形缓冲区。

**标签**: `#Redox OS`, `#Rust`, `#io\_uring`, `#operating systems`, `#microkernel`

---

<a id="item-tech-news-22"></a>
### [MIDA 基准：狼人杀测出多模态大模型社交盲区](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+EMNLP%2726%EF%BD%9CGPT%E4%B9%9F%E4%B8%8D%E4%BC%9A%E3%80%8C%E8%AF%BB%E7%A9%BA%E6%B0%94%E3%80%8D%EF%BC%8C%E7%8B%BC%E4%BA%BA%E6%9D%80%E5%9F%BA%E5%87%86%E6%B5%8B%E5%87%BA%E7%A4%BE%E4%BA%A4%E7%9B%B2%E5%8C%BA) ⭐️ 6.0/10

东京大学研究团队提出多模态交互式欺骗评估基准 MIDA，以「一夜终极狼人」为实验场景，系统测试 GPT、Gemini、Claude、Qwen、DeepSeek 等开源和闭源模型在多人互动中的欺骗判断能力。结果显示，这些多模态大模型能够理解图像、声音和文本，却难以可靠地区分真话与谎言，无法准确把握说话者当时“知道什么、相信什么、又试图让别人相信什么”。该研究已被 EMNLP 2026 主会接收，论文、项目主页、代码和数据集均已公开。

rss · 新智元 · 10月28日 11:48

**「背景」** 此前欺骗检测研究大多围绕单人陈述或两人对话展开，难以处理带有追问、站队和群体压力的多人互动，而且现实中一句话是否构成谎言往往缺乏可核实、可统一判定的标准答案。MIDA 选择“一夜终极狼人”作为实验环境，正是因为游戏中的角色、夜间行动和规则都可追溯，研究者能够依据玩家当时实际掌握的信息判断其发言是否属于欺骗。

**「影响」** 对计划在涉及多人互动、话术博弈或安全审查场景中部署多模态大模型的开发者来说，这项基准给出了可复用的评估方法：研究团队已公开代码、数据集和项目主页，可以自行复现测试。同时，论文结果显示，包括 GPT、Gemini、Claude、Qwen、DeepSeek 在内的 12 个主流多模态模型在 MIDA 上仍有明显性能差距，且普遍存在心智理论不足、难以对齐多模态社交线索的问题。因此，在实际产品中不应依赖当前多模态模型可靠识别谎言或隐含社交意图，至少需要先在该类任务上做针对性验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.16221">Can MLLMs Read the Room ? A Multimodal Benchmark for...</a></li>
<li><a href="https://huggingface.co/papers/2510.27195">Paper page - Can MLLMs Read the Room ? A Multimodal Benchmark ...</a></li>
<li><a href="https://www.academia.edu/145120659/Can_MLLMs_Read_the_Room_A_Multimodal_Benchmark_for_Assessing_Deception_in_Multi_Party_Social_Interactions">(PDF) Can MLLMs Read the Room ? A Multimodal Benchmark for...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#social reasoning`, `#EMNLP`, `#AI evaluation`

---

<a id="item-tech-news-23"></a>
### [通用反馈行与自写批评效果相当，缩减后见蒸馏所需特权信息](https://www.reddit.com/r/MachineLearning/comments/1xhv8yp/how_much_does_the_hint_matter_a_generic_feedback/) ⭐️ 6.0/10

一项针对 GPT-OSS-20B 多步金融推理的研究发现，在后见自蒸馏中把模型自写的批评替换成一句固定的通用反馈，仍能保留约 3 个百分点的全部性能提升；来自 6 倍规模模型的批评也没有带来实质性改善。作者由此认为，后见蒸馏提供的位置信息大幅降低了有效训练所需的特权信息量。该研究还报告，Fin-SD 在全参考解蒸馏 OPSD 的基础上实现了匹配性能，同时少用 9.5% 的 token。

reddit · r/MachineLearning · /u/jhzyu · 10月28日 17:52

**「背景」** 后见自蒸馏指学生模型先找出自己的第一步错误并写出批评，再用冻结的模型副本在给定前缀和批评的条件下，通过反向 KL 散度把知识蒸馏回学生自身。这项研究专门检验了批评内容本身的作用，以判断显式批评文本是否真的必要。

**「影响」** 对从事推理模型蒸馏的研究者和开发者而言，该结果意味着可以不再依赖逐样本生成高质量批评或更大教师模型，而用固定反馈提示来获得相近收益，从而降低训练时的特权信息需求和计算开销。

**标签**: `#hindsight self-distillation`, `#financial reasoning`, `#large language models`, `#knowledge distillation`, `#research`

---

<a id="item-tech-news-24"></a>
### [人机在鸡尾酒会语音上差距过小](https://www.reddit.com/r/MachineLearning/comments/1xhuado/cocktailparty_audio_as_a_reverse_turing_test/) ⭐️ 6.0/10

一项小规模研究报告，在 40 段合成鸡尾酒会语音中（目标句混有多名背景说话人，4 dB 衰减），人类转写均值词准确率为 0.71，而指令增强的 Gemini 3.8 Flash 为 0.54、Qwen3-ASR 为 0.55；以词准确率≥0.5 为通过线，人类通过率 77%，Gemini 为 55%。作者认为这一差距太窄，无法构成可靠音频 CAPTCHA，且实验仅覆盖 18 个听写会话、单一合成设置，未做声源分离。

reddit · r/MachineLearning · /u/cloud\_kj · 10月28日 17:17

**「背景」** 鸡尾酒会效应指人耳能从嘈杂多人声中集中听清一个说话人；音频 CAPTCHA 想利用这种人类能力，让机器在分离语音时失败而人类成功。作者用合成语音混合背景语声构造了这种测试，并比较多套 ASR 配置。

**「影响」** 对考虑用语音分离做验证码的系统，这一结果表明当前通用 ASR 已接近人类水平，不能仅凭“选出一路说话人”区分人机；需要继续寻找对人类容易、对模型稳定困难的音频条件。

**标签**: `#speech recognition`, `#audio captcha`, `#ASR benchmark`, `#cocktail party effect`, `#machine learning`

---

<a id="item-tech-news-25"></a>
### [Discord 公开服务器对话将被网络搜索](https://techcrunch.com/2026/10/27/discord-is-making-its-public-communities-more-searchable-and-people-have-concerns/) ⭐️ 6.0/10

Discord 于 10 月 27 日宣布，公开的「可发现服务器」中的对话将被网络搜索引擎收录。11 月 16 日起，每个此类服务器将获得独立网页，并可能包含自动生成的讨论摘要；12 月中旬起，部分公开频道的消息将出现在搜索结果中。管理员可以选定参与频道，成员可以自行退出，且发布内容不显示用户名与头像。因法律限制，该功能在欧盟、英国等地默认关闭，青少年账号不参与。

telegram · zaihuapd · 10月28日 03:21

**「背景」** Discord 平台以服务器（Server）为组织单位，其中可被搜索和加入的公开服务器即「可发现服务器」。此前这些服务器内的对话通常需要登录并进入具体频道才能查看，本次变化相当于把部分公开内容向 Web 搜索开放。

**标签**: `#Discord`, `#privacy`, `#search`, `#social media`, `#tech industry`

---

<a id="item-tech-news-26"></a>
### [韩国以支付违规为由对苹果和谷歌合计罚款 4750 万美元](https://appleinsider.com/articles/26/10/28/south-korea-becomes-the-latest-to-fine-apple-and-google-millions-over-their-app-stores) ⭐️ 6.0/10

韩国媒体与通信委员会对苹果处以 1550 万美元、对谷歌处以 3200 万美元罚款，认定两家公司虽然名义上允许第三方支付，却通过高收费实际阻碍开发者使用，违反韩国 2021 年相关法律。监管机构还指其疑似拖延应用审核，要求两家公司允许应用内接入外部支付链接，并改进应用审核流程。

telegram · zaihuapd · 10月28日 12:30

**「背景」** 2021 年，韩国修订《电信业务法》，要求苹果、谷歌等应用商店运营商允许开发者接入第三方支付，不得强制使用自家支付系统。此次罚款针对的就是两家公司在名义上开放第三方支付后，仍通过高额费用等方式实际阻碍开发者使用该渠道的做法。

**「影响」** 对在韩国 App Store 和 Google Play 上架的开发者而言，外部支付链接可能因此获得更明确的合规空间，应用审核流程也可能调整；开发者应留意苹果和谷歌是否落实监管要求，以及由此带来的支付分成和审核时限变化。

**标签**: `#app-store`, `#regulation`, `#antitrust`, `#Apple`, `#Google`

---