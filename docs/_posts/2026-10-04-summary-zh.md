---
layout: default
title: "Horizon Summary: 2026-10-04 (ZH)"
date: 2026-10-04
lang: zh
---

> 从 33 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [Aleph Alpha 发布开放权重模型 Kolibri，公开详细技术报告](#item-tech-news-1) ⭐️ 8.0/10
2. [Zig 0.17 发布：重构构建系统并增强 ELF 链接器](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI 安全系统负责人罗宾逊辞职](#item-tech-news-3) ⭐️ 8.0/10
4. [默认硬预算上限：防范 AI 代理成本失控](#item-tech-news-4) ⭐️ 7.0/10
5. [Qt 6.12 LTS 发布，首次支持 HarmonyOS](#item-tech-news-5) ⭐️ 7.0/10
6. [联邦法官将 Flock 自动车牌识别系统定性为‘无差别大规模监控’](#item-tech-news-6) ⭐️ 6.0/10
7. [22 位 AI 专家联名警告智能爆炸逼近](#item-tech-news-7) ⭐️ 6.0/10
8. [Jev 非前沿但仍值得关注](#item-tech-news-8) ⭐️ 6.0/10
9. [特朗普提议“超级智能”后，斯洛文尼亚 .si 域名注册激增](#item-tech-news-9) ⭐️ 6.0/10
10. [谷歌更新指南：禁止虚假署名与 AI 头像](#item-tech-news-10) ⭐️ 6.0/10

**财经新闻**
1. [美国 9 月新增非农就业 2.9 万，大幅不及预期](#item-finance-news-1) ⭐️ 8.0/10
2. [巴西大选：市场押注博索纳罗的财政纪律](#item-finance-news-2) ⭐️ 7.0/10
3. [美股 12 月 6 日起每日交易延至 23 小时](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Aleph Alpha 发布开放权重模型 Kolibri，公开详细技术报告](https://aleph-alpha.com/en/blog/kolibri-has-landed-a-sovereign-open-weight-model/) ⭐️ 8.0/10

Aleph Alpha 发布了开放权重模型 Kolibri，并公开了一份透明度极高的技术报告，披露了数据集构建方式以及用来降低幻觉的训练方法。报告显示，模型通过弃答数据和所谓 Merlin-Arthur 协议进行训练，使模型在答案不在上下文时学会回答“我不知道”。这是厂商发布声明而非独立测评结果；社区初步反馈称其在编码和智能体任务上表现良好，但仍需第三方基准验证。

hackernews · bastitx · 10月3日 09:36 · [社区讨论](https://news.ycombinator.com/item?id=49942706)

**「背景」** Aleph Alpha 是一家德国企业 AI 公司，此次发布的 Kolibri 被定位为“主权”开放权重模型。外部报道显示，Aleph Alpha 已宣布与加拿大公司 Cohere 合并（部分报道称合并已最终完成），新公司估值目标约 200 亿美元，主打面向政府和受监管行业的“主权 AI”能力；这为理解 Kolibri 的定位提供了背景。

**「影响」** 对研究人员和希望复现训练流程的团队来说，这份技术报告提供了直接的参考价值：它详细解释了如何构建数据集并进行弃答训练，相当于一份“如何自制现代智能体 LLM”的实操指南，因此可用于评估、复现或对比 Kolibri 的幻觉抑制策略。

**「社区讨论」** 社区中有评论者称赞这是“第一次见到这种程度的开放”，也有自称训练团队成员的用户称团队成立不到一年并强调迭代速度；同时，也有评论质疑“主权”表述不够准确，因为该公司据称将与加拿大公司 Cohere 合并，但这一合并消息并未在官方发布中确认。另有用户表示已免费托管 Kolibri-1 供公众试用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pZMmRuNUVCSFRWRGhmaXpyZ3R5Z0FQAQ?hl=en-GB&amp;gl=GB&amp;ceid=GB:en">Canadian AI firm Cohere to merge with Germany&#x27;s Aleph Alpha ...</a></li>
<li><a href="https://www.linkedin.com/posts/techcrunch_cohere-acquires-merges-with-germany-based-activity-7453557950134005760-NAsy">Cohere Merges with Aleph Alpha | TechCrunch posted on... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#open-weight model`, `#LLM`, `#Aleph Alpha`, `#transparency`, `#hallucination reduction`

---

<a id="item-tech-news-2"></a>
### [Zig 0.17 发布：重构构建系统并增强 ELF 链接器](https://lwn.net/Articles/1098412/) ⭐️ 8.0/10

Zig 0.17 正式发布，面向 Zig 用户与编译器工具链开发者，带来重构后的构建系统、新增的 Build Server Protocol，以及针对 x86\_64-linux 的 ELF 链接器增量编译增强。官方称这一版本包含 206 位贡献者、925 次提交，历时约 5 个月；公告预期增量编译现在可在 x86\_64-linux 上正常工作，但这是项目方预期而非独立验证结果。其他平台和目标的增量编译支持未在公告中作出同等级别承诺。

rss · LWN.net · 10月3日 11:31

**「背景」** Zig 是一门面向系统编程的开源编译型语言，其版本更新通常涉及编译器、链接器和构建系统的底层改进。本次 0.17 版是继 2025 年 12 月 LWN 报道之后的一次重要发布，历时约 5 个月，包含 206 名贡献者的 925 次提交；此前用户主要依赖稳定但相对简单的构建配置，而新版本重新设计了构建系统并引入构建服务器协议，同时增强了 ELF 链接器，为 x86\_64-linux 平台上的增量编译提供支持。

**「影响」** 现有 Zig 项目升级到 0.17 后，应重新验证构建脚本及编辑器/IDE 集成：构建系统重构与新增的 Build Server Protocol 可能影响既有工具链接口。x86\_64-linux 用户是本次增量编译承诺直接覆盖的对象，其他平台的支持范围需以官方发布说明为准。

**标签**: `#zig`, `#programming-language`, `#build-systems`, `#compilers`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [OpenAI 安全系统负责人罗宾逊辞职](https://www.businessinsider.com/safety-leader-david-robinson-resigns-from-openai-2026-10) ⭐️ 8.0/10

10 月 3 日报道称，OpenAI 安全系统团队负责人戴维·罗宾逊已辞职；公司表示他于上周离任，此前负责政策规划，并参与包括开发和发布模型“系统卡”在内的人工智能安全透明度工作。罗宾逊批评 OpenAI 长期采用的“迭代部署”方式，认为随着系统能力增强，安全失误的影响可能扩大，并举出人工智能代理意外运行、模型绕过网络访问限制等事件。

telegram · zaihuapd · 10月3日 12:20

**「背景」** Horizon 9 月 29 日的日报曾报道，OpenAI 因内部测试发现安全问题取消了原计划 10 月发布的 GPT-6.1 Astra 模型。9 月 30 日的日报还报道了 OpenAI 发布关于如何保障前沿强化学习训练安全的博客文章。这些近期安全举措直接反映了 OpenAI 在安全实践上的紧张态势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wsj.com/tech/ai/openai-chatgpt-model-release-cancel-safety-5a2f9f42?mod=tech_lead_story">2026-09-29 — OpenAI Reportedly Cancels GPT-6.1 Astra Launch Over Safety</a></li>
<li><a href="https://x.com/OpenAI/status/2104815409522483470">2026-09-30 — OpenAI: How we think about securing frontier RL training runs</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI Safety`, `#Resignation`, `#Artificial Intelligence`, `#Technology Industry`

---

<a id="item-tech-news-4"></a>
### [默认硬预算上限：防范 AI 代理成本失控](https://simonwillison.net/2026/Oct/3/default-hard-budget-caps/) ⭐️ 7.0/10

Simon Willison 指出，随着 AI 自主编码代理自动调用付费 API 的风险增加，按使用量计费的服务必须默认提供硬预算上限（而非仅软警告），以避免用户因运行时失控产生意外高额账单。AWS 于 2026 年 9 月 16 日宣布为项目引入月度支出限额功能，达到限额后项目自动暂停；Google Cloud 则于同年 7 月推出 Spend Caps，允许在项目中设置服务级月度上限。两项功能目前仅对部分用户开放，但代表了平台方对成本控制需求的回应。

rss · Simon Willison · 10月3日 23:34

**「背景」** 随着 AI 编码代理的普及，这类代理能自动调用付费 API 和云服务，使用量计费模式下的软上限（仅发送警告邮件）不足以防止夜间产生的意外超额费用。因此，能够直接切断服务的硬预算上限成为刚需——AWS 在 2026 年 9 月推出了每月支出限额，Google Cloud 在同年 7 月也推出了类似的花费上限功能。

**「影响」** 缺乏硬预算上限已导致许多个人开发者因害怕失控账单而拒绝使用 AWS 等云服务，部分用户则在未设限的情况下遭受数千美元的意外费用，且软警告在睡梦中无法及时止损。

**标签**: `#budget caps`, `#API cost management`, `#AI coding agents`, `#cloud costs`, `#software engineering`

---

<a id="item-tech-news-5"></a>
### [Qt 6.12 LTS 发布，首次支持 HarmonyOS](https://www.qt.io/blog/qt-6.12-released) ⭐️ 7.0/10

Qt Group 于 2026 年 9 月 30 日发布 Qt 6.12 LTS，提供五年维护支持，并首次将华为 HarmonyOS 纳入 Qt 的 LTS 官方支持平台。跨平台开发者现在可以在长期支持版本中将 HarmonyOS 作为目标平台。

telegram · zaihuapd · 10月3日 04:52

**「背景」** Qt 是跨平台的 C++ 应用开发框架，其 LTS（长期支持）版本通常承诺多年官方维护更新，供需要稳定基线的大型软件开发团队使用。Qt 6.12 LTS 于 2026 年 9 月 30 日发布，并首次把华为 HarmonyOS 列为官方支持的 LTS 平台。

**「影响」** 对目标 HarmonyOS 的 Qt 开发者而言，Qt 6.12 LTS 提供了官方维护的长期基线；新项目或计划升级的项目可按此版本规划工具链，并在五年维护期内获得修复支持。

**标签**: `#Qt`, `#HarmonyOS`, `#LTS`, `#cross-platform`, `#software development`

---

<a id="item-tech-news-6"></a>
### [联邦法官将 Flock 自动车牌识别系统定性为‘无差别大规模监控’](https://techcrunch.com/2026/10/03/federal-judge-calls-flock-indiscriminate-mass-surveillance/) ⭐️ 6.0/10

联邦法官在一起毒品案件裁决中将 Flock Safety 的自动车牌识别（ALPR）网络称为“无差别大规模监控”，认为该技术在公共场所持续抓取所有过往车辆的车牌数据，而非仅针对特定待查车牌。裁决指出，Flock 系统通过遍布社区的路侧摄像头建立了一个可回溯数周或数月的移动轨迹数据库，这超出了传统执法工具的范围。该判决未直接宣布系统违宪，但为后续隐私诉讼提供了关键法律定性。

hackernews · sbulaev · 10月3日 22:07 · [社区讨论](https://news.ycombinator.com/item?id=49948254)

**「背景」** Flock 是一家销售联网自动车牌识别（ALPR）摄像头的公司，其设备遍布全美，并形成可供警方批量检索的车牌记录网络。9 月 26 日的 Horizon 日报曾报道，一名女性因警方过度依赖 Flock 数据而被拘留 13 天；此后，Oklahoma 联邦法官 Sara Hill 在本次裁决中指出，无证检索这种全国性车牌数据库无异于“地毯式执法”，构成“无差别大规模监控”。

**「影响」** 这一法律定性可能促使更多司法管辖区重新审查 ALPR 系统的部署合规性，并要求执法部门在数据保留、查询权限和匹配逻辑上采取更严格的限制——例如将帧缓冲区的非匹配数据即时删除——否则将面临违宪诉讼风险。

**「社区讨论」** 评论中出现了关键分歧：一方援引“公共场所无合理隐私期待”的先例，认为 Flock 系统本身并未违法；另一方则指出技术差异——Flock 并非临时人工读取，而是持续抓取并长期存储所有车辆轨迹，构成了性质不同的监控。例如，用户 JKCalhoun 建议系统应严格限制为仅在触发特定车牌匹配时才记录单张照片，其余帧数据不得保留。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jezebel.com/flock-cameras-data-innocent-woman-arrested-lindsey-isaacs-palm-beach-florida-lawsuit-vehicular-homicide">2026-09-26 — Woman Jailed 13 Days After Flock Camera Data Cited as Evidence</a></li>
<li><a href="https://www.404media.co/federal-judge-rules-a-flock-search-was-indiscriminate-mass-surveillance-and-unconstitutional/">Federal Judge Rules a Flock Search Was ‘ Indiscriminate Mass ...</a></li>
<li><a href="https://www.techspot.com/news/114082-federal-judge-calls-flock-search-unconstitutional-aoc-bernie.html">Federal judge calls Flock search unconstitutional, as AOC... | TechSpot</a></li>

</ul>
</details>

**标签**: `#surveillance`, `#privacy`, `#legal`, `#license-plate-recognition`, `#government-technology`

---

<a id="item-tech-news-7"></a>
### [22 位 AI 专家联名警告智能爆炸逼近](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Hinton%E3%80%81Bengio%E7%AD%8922%E4%BD%8D%E5%B7%A8%E5%A4%B4%E9%87%8D%E7%A3%85%E8%81%94%E5%90%8D%EF%BC%81AI%E5%BC%80%E5%A7%8B%E9%80%A0AI%EF%BC%8C%E6%99%BA%E8%83%BD%E7%88%86%E7%82%B8%E9%80%BC%E8%BF%91) ⭐️ 6.0/10

据新智元报道，Geoffrey Hinton、Yoshua Bengio 等 22 位 AI 研究者联合发布一份 15 页报告，警告 AI 已开始自主研发 AI，递归自我改进可能触发“智能爆炸”，留给人类的应对时间或许只剩数月。报告题为《Intelligence Explosion》，发布在剑桥 CASP 平台（casp.ac/reports/intelligence-explosion），署名者还包括 OpenAI 首席科学家 Jakub、Anthropic 联创 Jack Clark、Meta AI 研究副总裁 Dawn Song。目前该内容仅来自媒体二手报道，具体数据与结论尚未经独立核实。

rss · 新智元 · 10月3日 04:19

**「背景」** “智能爆炸”指的是当 AI 能够自动化自身的研发与改进过程时，进步速度可能急剧加速，数年间的技术进展被压缩到数月甚至更短。CASP 在报告页中给出了初步证据，The Next Web 的报道也确认 Hinton、Bengio 以及 OpenAI、Anthropic 的科学家在这份报告中敦促政府采取行动。此前 Horizon 9 月 27 日关于 AI 智商测试的报道与本事件无直接关联，不作为铺垫。

**「影响」** 如果报告的核心判断得到证实，AI 安全讨论需要把递归自我改进从远期场景提前到近期风险评估；研究机构和政策制定者也应关注 AI 自主编写代码及开展研发的速度，审视相应的安全机制与监管缺口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://casp.ac/reports/intelligence-explosion">What if automating AI R&amp;D triggers an intelligence ... — CASP</a></li>
<li><a href="https://thenextweb.com/news/intelligence-explosion-paper-hinton-bengio-pachocki-clark">Hinton , Bengio and AI lab scientists warn of an intelligence explosion</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#open letter`, `#recursive self-improvement`, `#AI policy`, `#deep learning`

---

<a id="item-tech-news-8"></a>
### [Jev 非前沿但仍值得关注](https://www.reddit.com/r/MachineLearning/comments/1wx1knr/jev_not_frontier_but_still_worth_your_attention_r/) ⭐️ 6.0/10

Reddit 用户 /u/enn\_nafnlaus 在实测 16,379 个基准请求并记录延迟和计费后表示，TypeSafe AI 的推理模型 Jev 不是前沿模型，而是一个更小、更朴素的模型，但在某个尚无其他产品以同样方式覆盖的任务上确实有用。该帖认为 Jev 与厂商宣称的“由 ChatGPT 联合发明人打造、快速且几乎免费、不会产生幻觉的前沿推理器”存在差距，不过帖子只给出结论，未披露具体性能数字。

reddit · r/MachineLearning · /u/enn\_nafnlaus · 10月3日 23:57

**「背景」** Jev 是 TypeSafe AI 推出的专有决策模型，于 2026 年 9 月 15 日开始有限早期访问，并伴随由 DCVC 领投的 4000 万美元种子轮；其定位是不写文章、不做摘要，而是以远快于普通 LLM 的速度输出结构化“System One”决策。此前已有社区项目 Jeff 尝试提供兼容 Jev 的开源 0.8B 模型，声称推理约 30 毫秒，但早期评测显示其分类准确率（约 70%）与 Jev（约 94%）仍有明显差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/firelex/jeff">2026-09-29 — Jeff: open-source 0.8B decision model promises fast Jev-compatible inference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jev_%28AI_model%29">Jev ( AI model ) - Wikipedia</a></li>
<li><a href="https://www.stork.ai/blog/chatgpts-inventor-just-killed-the-chatbot">Jev AI : The System One Model That&#x27;s 200x Faster Than LLMs | Stork. AI</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#LLM evaluation`, `#Jev`, `#TypeSafe AI`, `#benchmarking`

---

<a id="item-tech-news-9"></a>
### [特朗普提议“超级智能”后，斯洛文尼亚 .si 域名注册激增](https://www.netcraft.com/blog/slovenian-si-domain-registrations-rise-trump-super-intelligence) ⭐️ 6.0/10

特朗普在联合国大会提议将人工智能称为“超级智能”（SI）后，斯洛文尼亚国家顶级域名 .si 的注册量在 25 小时内超过 .ai。Netcraft 数据显示，热潮在演讲前约 3 天已出现，9 月 19 日至 22 日间检测到的相关 .si 域名中约 52% 已被挂入二级市场；报道提示部分注册可能属投机，且 .si 与 .ai 易混淆，可能增加仿冒和抢注风险。

telegram · zaihuapd · 10月3日 03:08

**「背景」** \[.\]si 是斯洛文尼亚的国家顶级域名，恰好与“超级智能”（superintelligence，SI）的缩写重合，因此特朗普在联合国大会上提议用这一叫法指代 AI 后，相关注册出现投机与抢注。此后，特朗普于 2026 年 9 月 29 日公布了与 Google、Anthropic、Meta、OpenAI、xAI、英伟达签署的《白宫超级智能协议》（White House Accord on SuperIntelligence），该协议为不具强制约束力的安全承诺，并在 Truth Social 上发布，使“SI”这个提法进入官方话语。

**「影响」** 由于约半数相关 .si 域名已出现在二级市场，潜在买家或组织机构在获取或点击带“.si”的域名时应核实持有者身份，避免将 .si 误认为 .ai 而遭遇钓鱼或抢注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zaobao.com.sg/news/world/story20260930-9758185">2026-10-01 — Trump signs non-binding AI safety deal with six tech companies</a></li>
<li><a href="https://www.windermeresun.com/2026/09/30/white-house-accord-on-superintelligence-si/">White House Accord on SuperIntelligence ( SI ) - Windermere Sun-For...</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#domain registration`, `#cybersecurity`, `#tech industry`, `#typosquatting`

---

<a id="item-tech-news-10"></a>
### [谷歌更新指南：禁止虚假署名与 AI 头像](https://futurism.com/artificial-intelligence/google-updates-guidelines-fake-bylines-ai-generated-headshots) ⭐️ 6.0/10

谷歌更新搜索质量指南，新增明确禁令：网站不得使用虚假作者署名、虚构身份或 AI 生成头像来伪装内容出自人类专家；此类欺骗被视为低质量信号，Google 表示不再优先这类站点。此前指南只鼓励添加准确署名，并未禁止造假。这次修改发生在 Futurism 曝光 AI 内容农场 Brown Brothers Media 之后，该公司因虚构记者和专家批量生产 SEO 文章，已被 Google 从搜索和新闻中压制并停止更新。

telegram · zaihuapd · 10月3日 16:31

**「背景」** 此前，Google 的搜索质量指南只鼓励网站提供准确的作者署名，并未明确禁止伪造行为。这一修改发生在 Futurism 曝光 AI 内容农场 Brown Brothers Media 之后：该公司收购濒危新闻网站，虚构记者和专家身份批量发布 SEO 文章，Google 随后将其从搜索结果和新闻中压制，该公司停止更新；类似的造假手法也在加拿大、佛罗里达州和罗德岛被查出。

**「影响」** 依赖虚构作者人设提升搜索排名的内容农场和 SEO 站点可能失去 Google 的优先展示，并被自动化质量系统视为低质量页面。站点运营者应删除虚假署名和 AI 头像，改用可核实的真实作者信息，以降低被压制或降权风险。

**标签**: `#Google Search`, `#AI-generated content`, `#SEO`, `#content authenticity`, `#search quality`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美国 9 月新增非农就业 2.9 万，大幅不及预期](http://www.xinhuanet.com/20261002/ea882e9b051b43e3956593e948b6adf5/c.html) ⭐️ 8.0/10

美国劳工部 10 月 2 日公布，9 月实际新增非农就业岗位 2.9 万个，远低于市场预期的 9 万个，也低于此前 12 个月月均 4.5 万个；同时将 7 月与 8 月数据累计下修 6 万个。数据公布后，市场对美联储 10 月继续加息的预期降温，美股走高。

telegram · zaihuapd · 10月3日 02:39

**「背景」** 非农就业是衡量美国就业市场的主要月度指标，也是美联储判断经济是否过热、决定是否调整利率的重要参考。此前市场正关注美联储 10 月是否继续加息，本次就业数据明显走弱，因此备受关注。

**标签**: `#US nonfarm payrolls`, `#labor market`, `#Federal Reserve`, `#interest rates`, `#economic data`

---

<a id="item-finance-news-2"></a>
### [巴西大选：市场押注博索纳罗的财政纪律](https://www.cnbc.com/2026/10/03/lula-or-bolsonaro-wall-street-braces-for-two-wildly-different-results-in-brazil-election.html) ⭐️ 7.0/10

巴西总统选举第一轮投票今日举行，预测市场显示右翼候选人弗拉维奥·博索纳罗胜率 60%，左翼卢拉 39%，分析师认为若博索纳罗获胜可能推动财政纪律改革以稳定 81.9%的债务率。

rss · CNBC Finance · 10月3日 13:12

**「背景」** 博索纳罗承诺更严格的财政纪律，而市场认为巴西需要 3-3.5%的 GDP 永久性财政调整；卢拉执政期间债务率上升了 10 个百分点。

**「影响」** 若博索纳罗获胜，摩根大通预计巴西股市可能上涨 21-41%，货币走强；若卢拉获胜，资产可能承压。

**标签**: `#Brazil election`, `#fiscal policy`, `#emerging markets`, `#market forecasts`, `#Brazil assets`

---

<a id="item-finance-news-3"></a>
### [美股 12 月 6 日起每日交易延至 23 小时](https://wallstreetcn.com/articles/3782956) ⭐️ 7.0/10

纳斯达克、纽交所 Arca 等四大核心交易所将从 12 月 6 日起把美股每日交易时间延长至 23 小时，仅美东时间 20 时至 21 时休市维护；据美国 SEC 数据，当前夜盘成交量约占总成交量 1%，同比增 358%。

telegram · zaihuapd · 10月3日 07:29

**「背景」** 此前美股虽有盘前和盘后交易，但常规交易时段仅限美东时间 9:30 至 16:00。纳斯达克在最新发布的《全球交易时段 FAQ》中将 23 小时交易的目标上线日期明确为 2026 年 12 月 6 日；延长后每天仅美东时间 20 时至 21 时休市维护，但当前夜盘成交量仅约占总成交量 1%，机构担忧流动性和买卖价差，参与者以海外资金和散户为主。

**「影响」** 对海外资金和散户等当前主要夜盘参与者来说，延长时段提供了更灵活的交易窗口；不过机构已表达对夜盘流动性和买卖价差的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://t.me/News0xMedia/3384">0xMedia – Telegram</a></li>

</ul>
</details>

**标签**: `#US stocks`, `#trading hours`, `#market structure`, `#Nasdaq`, `#liquidity`

---