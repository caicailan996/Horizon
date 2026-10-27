# Horizon 每日速递 - 2026-10-27

> 从 50 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [OpenAI 公布数学、计算机科学与物理学三项新发现](#item-tech-news-1) ⭐️ 10.0/10
2. [Anthropic 公开提交 S-1，披露财务与战略细节](#item-tech-news-2) ⭐️ 8.0/10
3. [CorridorKey 2.0 发布：为视频制作提供低价绿幕抠像](#item-tech-news-3) ⭐️ 7.0/10
4. [Sebastian Raschka 的从零构建推理模型视频课程](#item-tech-news-4) ⭐️ 7.0/10
5. [微软提出 Type Server Protocol，尝试规范 Python 类型检查通信](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI 发布 GPT-6.1 Terra，引发定位与定价讨论](#item-tech-news-6) ⭐️ 7.0/10
7. [微软大规模买断四分之一员工](#item-tech-news-7) ⭐️ 7.0/10
8. [美国将氦列为关键材料](#item-tech-news-8) ⭐️ 7.0/10
9. [CPython 实验性 JIT 编译器将被移除](#item-tech-news-9) ⭐️ 7.0/10
10. [systemd 新增 Rust 叶组件支持](#item-tech-news-10) ⭐️ 7.0/10
11. [iFixit 拆解苹果折叠机 iPhone Duo：纳米纹理掩盖折痕，可维修性 5/10](#item-tech-news-11) ⭐️ 7.0/10
12. [CSS-Tricks 宣布新所有者，结束 DigitalOcean 时期的不确定](#item-tech-news-12) ⭐️ 6.0/10
13. [Windows 11 上仍在运行的最老 GUI 程序](#item-tech-news-13) ⭐️ 6.0/10
14. [Pharo 14 发布公告公开](#item-tech-news-14) ⭐️ 6.0/10
15. [Flock CEO 称公众反弹不是真的](#item-tech-news-15) ⭐️ 6.0/10
16. [EPA 悄然移除网络档案，政府数据保存引关注](#item-tech-news-16) ⭐️ 6.0/10
17. [Deepity：C++/CUDA 预测编码库发布，CPU MNIST 基准领先](#item-tech-news-17) ⭐️ 6.0/10
18. [PBT 不加速 grokking，但可从超参数死区逃逸](#item-tech-news-18) ⭐️ 6.0/10
19. [小米开源 HachimoDock：150 元自制语音 AI 硬件](#item-tech-news-19) ⭐️ 6.0/10
20. [传 C-V2X 强标制定启动，乘用车或将强制装载](#item-tech-news-20) ⭐️ 6.0/10
21. [即梦 AI 短剧工作室上线：一站式剧本到分镜工具](#item-tech-news-21) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 公布数学、计算机科学与物理学三项新发现](https://openai.com/index/building-scientific-understanding-with-academic-communities/) ⭐️ 10.0/10

10 月 26 日，OpenAI 与多个学术共同体宣布，在数学、计算机科学和物理学各取得一项新结果，并称已将关键证明形式化。最受关注的是，一项确定性精确计数算法对任意固定 k ≥ 2 的 k-CNF 公式，用 poly\_k\(n, m\) 空间在 \(n+m\)^\{O\_k\(1\)\} 2^\(n/\(log n\)^\(1/2+o\(1\)\)\) 时间内计数可满足赋值；按公告解读，这一上界与指数时间假说（ETH）相矛盾。团队还称已于 9 月 9 日和 9 月 18 日分别获得杨-米尔斯存在性和 QCD 的自然语言证明，并于 10 月 16 日完成 Lean 形式化。需要强调的是，ETH 为假并不等于 P=NP，也不表明 NP 有亚指数算法。

hackernews · jonluca · 10月26日 21:35 · [社区讨论](https://news.ycombinator.com/item?id=50251344)

**「背景」** 指数时间假说（ETH）是计算复杂度理论中被广泛用于推导 NP 难问题下界的长期假设；Yang–Mills 存在性与质量间隙则是克莱数学研究所列出的千禧年大奖难题之一。了解这两项背景，有助于理解本次公告的分量。

**「影响」** 若该结果通过验证，依赖 ETH 的下界证明将失去一个常用前提：大量参数复杂度论文用 ETH 作为难解性或下界证明的假设。研究者在引用相关结论前应等待论文与 Lean 形式化的独立核验，并关注后续是否出现清理证明或修正。

**「社区讨论」** 社区讨论中最有用的辨析是：ETH 为假并不自动意味着 P=NP；cochne 提醒，新算法的时间上界仍为超多项式，不能推出 NP 有亚指数算法。abetusk 表示原本不会相信 ETH 为假，martinhath 则指出大量参数复杂度论文曾把 ETH 当作下界证明的基础。

**标签**: `#OpenAI`, `#complexity theory`, `#mathematics`, `#physics`, `#AI research`

---

<a id="item-tech-news-2"></a>
### [Anthropic 公开提交 S-1，披露财务与战略细节](https://www.sec.gov/Archives/edgar/data/2130357/000162828026067168/anthropicpbc-sx1.htm) ⭐️ 8.0/10

Anthropic 已向美国证券交易委员会公开提交 S-1 文件，为其可能的公开上市提供详细的财务与战略信息。文件涉及风险因素、长期基础设施采购承诺以及 AI 商业化路径等关键披露；本次条目未提供文件原文，具体数据应以 SEC 原始文件为准。

hackernews · SiNTEx · 10月26日 13:04 · [社区讨论](https://news.ycombinator.com/item?id=50242939)

**「背景」** 这份 S-1 是 Anthropic 上市筹备的正式公开文件。10 月 16 日的日报记载，Anthropic 向投资者披露 2026 年第三季度营收达 168 亿美元、环比增长近 50%，并计划在近期推进 IPO；10 月 17 日的日报记载，部分投资者因增长放缓和算力成本高昂，把 IPO 估值预期从约 2 万亿美元下调至约 1.5 万亿美元；10 月 20 日的日报则称，该公司被市场视为 2026 年最后一个重大 IPO 希望，但增速正在放缓。这些先前的财务披露与市场预期，为理解这份 S-1 中的营收数据、估值讨论和风险因素提供了直接背景。

**「实际影响」** S-1 披露首次让外界同时看到 Anthropic 的收入和算力合同：2026 年上半年约 48% 的收入（约 78 亿美元）来自亚马逊、谷歌和微软的云市场渠道，而公司已锁定总额约 5180 亿美元的多年算力承诺，其中仅博通就占约 1612 亿美元。对客户和投资者而言，Claude 的定价、可用性和交付因此高度绑定在这些超大规模云厂商及算力供应商的合同执行上；依赖 Claude 的企业在扩展或续约时应把这些集中度视为实际商业风险。

**「社区讨论」** 评论者主要围绕需求能否支撑巨额支出展开辩论：有观点称 Anthropic 已承诺对 Google、AWS、Broadcom、SpaceX 等合计超过 5000 亿美元的长期采购，若收入能从约 500 亿美元增长到 5000 亿美元则可消化，否则压力巨大；另一些评论则强调 AI 编码（Claude Code）是增长引擎，但也指出技术快速扩散可能让增速难以外推。还有评论提到文件的风险因素涵盖开源与开放权重模型（尤其是中国实验室）以及模型被滥用或护栏失效带来的声誉与财务风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Oct/15/anthropic-tells-investors/">2026-10-16 — Anthropic tells investors Q3 revenue up nearly 50% to $16.8bn</a></li>
<li><a href="https://www.reuters.com/business/finance/investors-temper-anthropic-ipo-valuation-expectations-over-revenue-growth-2026-10-15/">2026-10-17 — Investors temper Anthropic IPO valuation expectations to $1.5 trillion</a></li>
<li><a href="https://www.cnbc.com/2026/10/19/anthropic-ipo-ai-trade.html">2026-10-20 — Anthropic is the last big IPO hope for 2026, but growth is slowing</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-1-518-billion-commitment-165731037.html?fr=sycsrp_catchall">Anthropic’s S-1 Is Here. The $518 Billion Commitment Is the ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-1-shows-cloud-marketplaces-140304486.html?fr=sycsrp_catchall">Anthropic S-1 shows cloud marketplaces carried 48% of first ... Anthropic&#x27;s Public S-1 Sets Stage for Massive IPO Debut ... Anthropic&#x27;s IPO filing reveals $16.3B revenue, $80.7B loss ... Anthropic&#x27;s Draft S-1 Reveals 15x Revenue Surge and $600B ... Broadcom to lend Anthropic up to $42 billion to lease its ... Anthropic Locks In Up to $517 Billion of AI Compute: 14.8 GW ...</a></li>

</ul>
</details>

**标签**: `#anthropic`, `#s-1`, `#ipo`, `#ai-industry`, `#financial-disclosures`

---

<a id="item-tech-news-3"></a>
### [CorridorKey 2.0 发布：为视频制作提供低价绿幕抠像](https://corridorkey.com/) ⭐️ 7.0/10

CorridorKey 2.0 已作为一款视频抠像/绿幕合成工具发布，并在 Hacker News 上因质量与定价受到关注。根据分析摘要和评论区信息，其测试版定价为 50 美元、正式版为 100 美元，且对年收入不超过 2000 万美元的组织之外的用户免费；但当前信息是发布动态而非独立测评，也未提供实时性能证据。

hackernews · ravenical · 10月26日 21:18 · [社区讨论](https://news.ycombinator.com/item?id=50251127)

**「背景」** 绿幕抠像（keying）是把前景人物或物体从纯色背景中分离出来以便合成到新画面的常见视频制作步骤；传统工具往往需要精细的边缘、发丝和半透明遮罩处理。

**「影响」** 如果评论区披露的许可条件属实，独立创作者和小型团队可能以极低成本获得接近专业工具的抠像能力。使用该工具的组织应检查自身年收入是否超过 2000 万美元，因为超过该门槛的组织需要付费购买。

**「社区讨论」** 评论区认为 50/100 美元的定价极具性价比，并指出对年收入不超过 2000 万美元的组织之外的用户免费；ShakataGaNai 将其与 Final Cut 的 Magnet Mask 类比，但表示尚未亲自对比。多位用户询问是否能用于 OBS 或实时视频合成，wongarsu 和 keyle 都表达了实时处理需求。

**标签**: `#CorridorKey`, `#video-production`, `#green-screen`, `#keying`, `#visual-effects`

---

<a id="item-tech-news-4"></a>
### [Sebastian Raschka 的从零构建推理模型视频课程](https://magazine.sebastianraschka.com/p/building-reasoning-models) ⭐️ 7.0/10

Sebastian Raschka 的从零开始构建推理模型视频课程已在 Hacker News 引发大量正面讨论。课程面向希望亲手搭建推理模型的开发者和学习者；资料中未提供平台、价格或所需算力等细节。

hackernews · sgiannopoulos · 10月26日 15:11 · [社区讨论](https://news.ycombinator.com/item?id=50245138)

**「背景」** 推理模型指的是在给出最终答案前先生成思考过程的 LLM；从零构建这类模型能让学习者理解其内部机制，而不仅仅是调用现成 API。对于已经熟悉基础 LLM 训练的开发者和研究者，这类课程提供了一条更贴近实现细节的学习路径。

**「社区讨论」** libraryofbabel 认为，这类从零教程的目的不是让学员最终训练出可用的 LLM，而是理解原理；darrelld 评价作者同主题书籍《Build Your Own LLM From Scratch》可读性强，能一步步引导读者。flakiness 则提出了实际算力问题，询问课程或书籍需要云 GPU 还是可以在本地运行，以及需要多强的电脑。

**标签**: `#machine-learning`, `#LLM`, `#reasoning-models`, `#education`, `#AI`

---

<a id="item-tech-news-5"></a>
### [微软提出 Type Server Protocol，尝试规范 Python 类型检查通信](https://github.com/microsoft/pylance-release/blob/main/docs/tsp/type-server-protocol.md) ⭐️ 7.0/10

微软在 pylance-release 仓库发布了 Type Server Protocol（TSP）文档，提议为 Python 类型检查服务器之间的通信建立新的标准协议。该协议目前仍是提案，而非已可实际使用的功能；它面向 Python 语言服务器、类型检查器及 IDE 工具链的开发者和维护者，目的是改善不同实现之间的互操作性。提案已引发社区讨论，但各方尚未形成一致支持。

hackernews · adamnemecek · 10月26日 18:14 · [社区讨论](https://news.ycombinator.com/item?id=50248371)

**「背景」** Python 类型检查器（如微软的 Pyright、Astral 的 Ty）依赖由 PEP 标准化的类型提示体系工作；此前编辑器与这些检查器之间的通信通常走微软提出的通用 Language Server Protocol（LSP）。TSP 是微软在 pylance-release 仓库中提出的新协议标准，专门规范 Python 类型检查服务器与编辑器之间的通信。

**「影响」** 该提案对 Python 类型检查工具链的实际影响仍不确定：评论区显示 basedpyright 维护者曾公开批评 TSP，而 Astral 的 Ty 据称将支持该协议，说明主流实现之间已经出现路线分歧。工具链维护者在决定是否采用 TSP 时，需要同时考虑这些实现方的兼容性立场。

**「社区讨论」** 有评论者认为该协议应改名为 Python Type Server Protocol，因为它只支持 Python，却占用了通用协议命名空间；也有评论者引用 basedpyright 维护者的批评和 Astral Ty 可能支持的信息，指出实现方之间的分歧。另一些用户则以 Pyright、Pylance、basedpyright 等碎片化为例，担心跨 IDE 无法获得一致的类型检查结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.python.org/3/library/typing.html">typing — Support for type hints — Python 3.14.8 documentation</a></li>
<li><a href="https://python.plainenglish.io/ty-2-0-python-type-checker-tutorial-the-30-faster-mypy-killer-for-modern-django-projects-43256d120e39">Ty 2.0 Python Type Checker Tutorial: The 30× Faster Mypy Killer for...</a></li>

</ul>
</details>

**标签**: `#python`, `#type-server-protocol`, `#developer-tools`, `#microsoft`, `#type-checking`

---

<a id="item-tech-news-6"></a>
### [OpenAI 发布 GPT-6.1 Terra，引发定位与定价讨论](https://openai.com/index/introducing-gpt-6-1-terra/) ⭐️ 7.0/10

OpenAI 于 2026 年 10 月 26 日发布 GPT-6.1 Terra，为 GPT-6.x 系列新增一个模型版本，面向使用 OpenAI API 的开发者。此次发布本身是一个增量更新，官方公告并未在现有材料中提供详细基准或完整定价信息，但已引发社区对模型命名体系、推理级别设置以及成本取舍的集中讨论。

hackernews · meetpateltech · 10月26日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=50248124)

**「背景」** OpenAI 的 GPT-6.1 是 GPT-6 之后的增量版本系列；9 月 30 日的日报曾报道该系列的首个型号 GPT-6.1 Sol 以约五分之一的价格提供接近 GPT-6 Astra 的性能。Terra 是本次新增的更小、更便宜的型号：OpenAI 官方页面称，在中等推理强度下，GPT-6.1 Terra 比 GPT-5.6 Terra 的得分高 15 个百分点，成本约为后者的三分之一，并以仅为 GPT-6 Astra 十分之一的每 token 价格达到与其相当的表现；这些数字来自厂商自述，尚未经独立评测验证。

**「影响」** 对正在选择 OpenAI 模型的开发者而言，Terra 的加入并不自动解决选型难题：多位评论者认为，通过切换相邻模型层级或调整推理级别，往往能获得更低成本或更高性能的结果，因此选择 Terra 前应与邻近型号的价格和单任务成本进行对比。

**「社区讨论」** 评论中，Silagi 认为 Terra 缺少不可替代的用途，几乎所有任务都能通过调整层级或推理级别获得更便宜或更优的结果；minimaxir 也质疑在 TerminalBench 4.0 的单任务成本数据下选择 Terra 而非 Sol 的理由。simonw 则报告称“none”与“low”推理级别几乎不消耗推理 token，且“low”的 token 和费用甚至低于“none”；另有评论者对 Luna、Terra、Sol、Astra 的命名混乱表示困惑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/OpenAI/status/2104986129686741046">2026-09-30 — OpenAI Announces GPT-6.1 Sol with Cost-Efficiency Claims</a></li>
<li><a href="https://openai.com/index/introducing-gpt-6-1-terra/">Introducing GPT-6.1 Terra | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT`, `#large language models`, `#AI industry`, `#model releases`

---

<a id="item-tech-news-7"></a>
### [微软大规模买断四分之一员工](https://www.seattletimes.com/business/microsoft/microsoft-offers-mass-buyouts-for-roughly-a-quarter-of-its-workforce/) ⭐️ 7.0/10

微软据报向约占四分之一的员工提供大规模买断方案，用于缩减人力规模。报道尚未给出官方确认，也没有披露补偿条款、接受期限或如果接受人数不足是否会转为强制裁员。受影响员工需要在接受买断和等待后续安排之间做出选择。

hackernews · doctorzook · 10月26日 15:35 · [社区讨论](https://news.ycombinator.com/item?id=50245524)

**「背景」** 微软已向约 6 万名员工（约占其 22.3 万全球员工总数的四分之一，涉及美国、英国、加拿大和印度）提供自愿买断方案；据 TechCrunch 报道，公司确认这是为控制成本并面向 AI 调整人力结构的最新举措。此前 Horizon 在 10 月 9 日的日报中曾报道，美方因指控微软涉嫌欺诈而暂停其参与外国工人绿卡项目，当时副总统 Vance 称微软去年裁减了 6000 个美国岗位；如今的自愿买断延续了微软缩减人力的走向，但最终接受人数尚不确定。

**「影响」** 受影响员工需要决定是否接受买断，而选择接受的人将进入就业市场，并可能与大量同时离职的微软员工竞争同类岗位。

**「社区讨论」** 多位评论者讨论买断方案的两难处境：ecshafer 认为接受者将面对与大量前同事竞争，拒绝者则需承担后续强制裁员风险；christophilus 引述前上司观点称此类方案常先带走最有外部就业能力的员工。tandr 提醒接受率可能远超管理层预期，theodpHN 则指出该消息距 Brad Smith 发布“我们始终支持员工”的表态不到一周。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/h1b-visa-program-vance-microsoft-e7b3a407f822702b269ee277d21343ea">2026-10-09 — US suspends Microsoft from foreign-worker green card program over alleged fraud</a></li>
<li><a href="https://techcrunch.com/2026/10/26/microsoft-offers-buyouts-to-around-60000-employees-reports-say/">Microsoft offers buyouts to around 60,000 employees | TechCrunch</a></li>

</ul>
</details>

**标签**: `#microsoft`, `#tech-industry`, `#layoffs`, `#workforce`, `#business`

---

<a id="item-tech-news-8"></a>
### [美国将氦列为关键材料](https://apnews.com/article/energy-critical-materials-minerals-helium-43da160adc1bad389fba0b9ffbd14c3c) ⭐️ 7.0/10

美国已正式将氦列为一种关键材料，承认其在半导体制造、低温设备和工业供应链中的战略重要性。这是一项政策认定，具体执行措施和后续监管影响尚未公布，但可能影响相关行业的供应保障安排。

hackernews · rbanffy · 10月26日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=50248665)

**「背景」** 氦通常作为天然气开采的副产品回收，而非单独开采。美国政府依据《2020 年能源法案》建立了关键材料认定框架；本次将氦列为关键材料，意味着它进入能源部开发、示范和商业化关键材料技术的政策框架，理由是它在半导体制造和先进能源技术中不可或缺、且面临日益增长的供应链风险。

**「社区讨论」** 评论者对认定的实际效果存在分歧：有评论称美国约 95%的提取氦仍作为废气排空，认为该认定更像是在为少数提取公司抬高价格；也有人批评过去出售国家氦储备的做法，认为把氦用于气球是浪费。另有评论补充了同位素背景，指出低温应用涉及氦-3 与氦-4 的组合，并认为加拿大因重水反应堆和天然气生产可成为相关供应来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.energy.gov/articles/energy-department-designates-helium-critical-material-strengthen-american-manufacturing">Energy Department Designates Helium as Critical Material to...</a></li>
<li><a href="https://www.alexjoneslive.com/2026/10/24/us-designates-helium-a-critical-material-in-reindustrialization-push-to-avoid-single-point-of-failure/">US Designates Helium a Critical Material in... - Alex Jones Live</a></li>
<li><a href="https://www.theepochtimes.com/us/us-designates-helium-as-critical-material-amid-global-supply-risks-6108399">US Designates Helium as Critical Material Amid... | The Epoch Times</a></li>

</ul>
</details>

**标签**: `#helium`, `#critical materials`, `#semiconductors`, `#supply chain`, `#policy`

---

<a id="item-tech-news-9"></a>
### [CPython 实验性 JIT 编译器将被移除](https://lwn.net/Articles/1102102/) ⭐️ 7.0/10

CPython 的实验性即时编译器（JIT）即将被移除。该编译器在 2024 年随 Python 3.13 加入，但在 Python 指导委员会于今年 6 月暂停该项目后，JIT 维护者已撤回 PEP 836（“JIT Go Brrr: The Path to a Supported JIT Compiler for CPython”），理由是 PEP 未能充分解决维护、兼容性、成功指标和完成时间表方面的担忧。这意味着 CPython 主分支上这一一度颇具前景的性能优化开发暂时告终。

rss · LWN.net · 10月26日 15:45

**「背景」** CPython 3.13 于 2024 年首次以实验特性引入 JIT 编译器，目标是通过将部分字节码转换为机器码来提升解释器性能。2026 年 6 月，Python 指导委员会要求任何继续推进 JIT 的提案必须先通过正式 PEP，明确维护责任、兼容性影响、可衡量的成功标准以及明确的完成时间线。

**「影响」** 依赖 CPython 解释器性能的开发者短期内不会得到由 JIT 带来的加速，Python 性能提升路线将回到其他优化手段。关注 Python 3.13 实验性 JIT 的用户也不应将其用于生产环境，因为该功能正在被移除且不会再得到官方支持。

**标签**: `#python`, `#cpython`, `#jit`, `#performance`, `#open source`

---

<a id="item-tech-news-10"></a>
### [systemd 新增 Rust 叶组件支持](https://lwn.net/Articles/1102970/) ⭐️ 7.0/10

Christian Brauner 已合并 systemd 对“新叶组件”使用 Rust 编写的支持；现有代码不会移植到 Rust，其他组件依赖的部分也仍用 C 实现。Brauner 表示项目希望未来在核心 systemd 中推进 Rust，但 Rust 的动态库支持仍存在阻塞问题，可能导致二进制体积显著膨胀。该工作很可能随预计 12 月发布的 systemd v263 版本一起出现。

rss · LWN.net · 10月26日 15:13

**「背景」** systemd 是 Linux 下负责初始化、服务管理等核心功能的软件套件。这里的“叶组件”（leaf component）指不会被其他组件依赖的独立程序或工具，因此允许用 Rust 编写新叶组件不会影响既有代码的构建和接口。

**「影响」** 对希望为 systemd 贡献新组件的开发者，Rust 现已成为可进入主线代码库的编写语言，并可能出现在 v263 中；但动态库支持瓶颈意味着不应期待核心 systemd 会很快迁移到 Rust。现有组件的 C 实现和依赖关系保持不变，因此既有 systemd 部署无需因本次合并调整配置。

**标签**: `#systemd`, `#rust`, `#systems-programming`, `#linux`, `#open-source`

---

<a id="item-tech-news-11"></a>
### [iFixit 拆解苹果折叠机 iPhone Duo：纳米纹理掩盖折痕，可维修性 5/10](https://www.ifixit.com/News/119895/iphone-duo-teardown) ⭐️ 7.0/10

iFixit 拆解了苹果首款折叠机 iPhone Duo，给出 5/10 的可维修性评分，称这是其拆过的折叠手机中最高分；拆解发现屏幕表面的纳米纹理层通过散射反射来掩盖折痕，子像素呈椭圆且朝向各异。iFixit 还推测部分用户遇到的屏幕开裂与铰链某部分下沉不到位、挤压附近排线有关。内屏一旦损坏，保修外更换需 999 美元。

telegram · zaihuapd · 10月26日 04:15

**「背景」** iPhone Duo 在 10 月 23 日开售前，苹果已开放针对该折叠机的 App Store 提交，10 月 7 日的 Horizon 日报曾报道只有基于 iOS 27.1 SDK 或更高版本构建的 App 才能动态适配内屏宽度。10 月 25 日的日报则记录了首批用户在铰链处出现屏幕开裂的反馈，有设备使用不足 20 次开合即故障；本次 iFixit 拆解正是在这一背景下，对开裂原因给出了自己的推测。

**「影响」** 对潜在买家或维修用户而言，iPhone Duo 的内屏维修成本高达 999 美元，且开裂原因目前只是 iFixit 的推测而非确认结论；在苹果官方说明或更多拆解验证前，不应将铰链问题视为定论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/10/05/apple-opens-iphone-duo-app-submissions/">2026-10-07 — Apple Opens iPhone Duo App Submissions Ahead of October 23 Launch</a></li>
<li><a href="https://www.macrumors.com/2026/10/23/iphone-duo-screen-cracks/">2026-10-25 — iPhone Duo Users Report Screen Cracks Along Hinge</a></li>

</ul>
</details>

**标签**: `#hardware`, `#teardown`, `#foldable phones`, `#Apple`, `#repairability`

---

<a id="item-tech-news-12"></a>
### [CSS-Tricks 宣布新所有者，结束 DigitalOcean 时期的不确定](https://css-tricks.com/css-tricks-has-a-new-owner/) ⭐️ 6.0/10

CSS-Tricks 在公告中确认站点已更换所有者，结束了此前被 DigitalOcean 收购后一度陷入前景不明状态的局面。当前信息只表明控制权易主，未披露新所有者身份、交易条件或后续编辑与运营安排，也没有涉及任何技术性更新。

hackernews · edent · 10月26日 15:51 · [社区讨论](https://news.ycombinator.com/item?id=50245831)

**「背景」** CSS-Tricks 是运营多年的知名前端开发资源网站，此前被 DigitalOcean 收购；收购之后网站曾一度处于前景不明的“搁置”状态，社区也有相关讨论。现在该网站宣布有了新所有者，标志着其所有权再次发生变更。

**「影响」** 对长期把 CSS-Tricks 当作参考资料的前端开发者而言，实际变化是站点所有权从 DigitalOcean 转入长期参与编辑的 Geoff Graham 手中，结束了此前的悬置状态。读者应留意新独立所有权下内容更新、广告或付费服务等运营方式是否会调整，以判断这一资源能否继续稳定提供教程。

**「社区讨论」** 评论区的分歧集中在 CSS-Tricks 的未来：sikozu 不看好新东家能在当前前端生态下长期维持，认为当初卖给 DigitalOcean 是错误，并以 Tailwind CSS 团队缩小并加入 Shopify 为例；willio58 则猜测 DigitalOcean 此前似乎忘记了自己拥有该站点。grahamburger 分享的类似运营经历是：广告和课程都难赚钱，最终靠直接提供付费服务谋生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dzen.ru/a/at-SfXadql3iIysi">Джефф Грэм стал владельцем CSS - Tricks после четырёх... | Дзен</a></li>

</ul>
</details>

**标签**: `#css-tricks`, `#web-development`, `#industry-news`, `#frontend`, `#digitalocean`

---

<a id="item-tech-news-13"></a>
### [Windows 11 上仍在运行的最老 GUI 程序](https://blog.enlyth.com/posts/oldest-windows-gui-app-win-11/) ⭐️ 6.0/10

这篇博客文章探寻了仍能在 Windows 11 上运行的年代最久远的 GUI 应用程序，并以此讨论 Windows 的向后兼容性。评论者根据文章内容估算该程序已有 33 年 8 个月历史，同时提供的亲历案例显示，老程序能启动并不等于一切正常：Windows 11 对 8 位/256 色 DirectDraw 调色板的解析方式与旧系统不同，部分 Win3.1 游戏需要补丁才能正确显示。

hackernews · enlyth · 10月26日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=50248055)

**「背景」** Windows 长期坚持 Win32 API 的二进制向后兼容，使几十年前为老版本编译的图形界面程序仍能在新系统上启动；评论中有人据此称 Win32 是“唯一稳定的 ABI”。这篇博客正是在测试这条兼容路线的实际边界：寻找 Windows 11 上仍能运行的最老 GUI 应用。有评论者实测发现，兼容并非无缝——例如一款 Windows 3.1 时代的儿童 CD-ROM 游戏因依赖早期 DirectDraw 的 8 位调色板行为，需要补丁才能在 Windows 11 上正常显示。

**「影响」** 对依赖旧版 Win32 API 或 DirectDraw 调色板技巧的遗留软件，一个现实后果是：程序仍能在 Windows 11 启动，但显示行为可能已改变；评论者 mattbee 就为一部 Windows 3.1 游戏编写补丁 DLL，来恢复 256 色下的调色板淡入淡出效果。

**「社区讨论」** 讨论中最有信息量的内容是具体兼容性案例：anticorporate 记录了把 FreeCell 最高分（保存在注册表中）逐代迁移到新电脑的过程，并保留用户熟悉的 Win32 版本；mattbee 则为 Windows 3.1 儿童游戏写了补丁 DLL，因为 Windows 11 对 256 色调色板的处理与旧系统不同。另有评论者 drnick1 批评现代 UI 抛弃菜单栏和原生 Win32 框架，认为 Windows 95 时代的桌面界面已经足够成熟。

**标签**: `#windows`, `#backward-compatibility`, `#win32`, `#software-history`, `#gui`

---

<a id="item-tech-news-14"></a>
### [Pharo 14 发布公告公开](https://pharo.org/news/2026-10-26-Pharo14Release.html) ⭐️ 6.0/10

Pharo 项目于 2026 年 10 月 26 日在其官网发布了 Pharo 14 的版本公告，面向现有 Smalltalk/Pharo 用户与开发者。由于手头资料未包含发布说明的具体内容，本摘要无法确认该版本的新特性、兼容性变化或下载渠道；应以官方公告原文为准。

hackernews · xkriva11 · 10月26日 11:15 · [社区讨论](https://news.ycombinator.com/item?id=50241925)

**「背景」** Pharo 是 Smalltalk-80 编程语言与运行时系统的开源跨平台实现。此前 Pharo 项目曾宣布接近 Pharo 13 发布阶段，冻结 13 分支的新功能开发，并已为 Pharo 14 打开新的开发分支；因此 Pharo 14 的发布是该项目既定版本迭代中的下一步。

**「社区讨论」** 在 Hacker News 讨论中，ElevenLathe 询问代理辅助 Smalltalk 的现状，认为智能体直接操控运行中的程序听起来很契合，但担心 Smalltalk 缺少足够的训练数据；adius 则推荐 Cuis Smalltalk，称其更地道、且基于矢量图形的渲染效果更好。这些都是评论者的个人观点，并非来自官方发布公告的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pharo">Pharo - Wikipedia</a></li>
<li><a href="https://www.pharo.org/news/">Pharo - Pharo News</a></li>

</ul>
</details>

**标签**: `#Pharo`, `#Smalltalk`, `#programming languages`, `#open source`, `#developer tools`

---

<a id="item-tech-news-15"></a>
### [Flock CEO 称公众反弹不是真的](https://www.404media.co/in-leaked-audio-flock-ceo-tells-cops-backlash-to-the-company-isnt-real/) ⭐️ 6.0/10

据 404 Media 报道，一段泄露音频显示 Flock Safety 首席执行官在面向警方的场合称，针对该公司的反弹“并非真实”。该说法目前仍只是媒体报道的“据称泄露”内容，尚未获得公司回应或完整录音的独立证实。

hackernews · Frieren · 10月26日 17:54 · [社区讨论](https://news.ycombinator.com/item?id=50248005)

**「背景」** 10 月 25 日的日报曾报道，安全研究员从 Flock 自身系统获取的设备清单被 Proton 制成公开地图，显示美国有超过 30 万台 Flock 监控设备；10 月 4 日的日报还曾报道，一名联邦法官在相关诉讼中将 Flock 的车牌自动识别系统称为“无差别的大规模监控”。这些报道分别涉及 Flock 装置的规模和法律定性，是理解当前 CEO 否认反弹声音真实存在的直接前史。

**「社区讨论」** 有评论者以自己约 6000 人的低犯罪率小镇为例，质疑当地政府安装多台 Flock 摄像头的必要性，并表示每次驾车经过都因行踪可能被记录而感到不安。另有评论批评 CEO 既承认犯错又坚持“永不道歉”的态度自相矛盾，还有评论讽刺称“既然反弹不是真的，就不应起诉剪断摄像头的人”，并将“这些人不是真的”的说法与历史上的迫害话语相类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/proton-flock-map/">2026-10-25 — Proton Maps 300,000+ US Flock Surveillance Devices</a></li>
<li><a href="https://techcrunch.com/2026/10/03/federal-judge-calls-flock-indiscriminate-mass-surveillance/">2026-10-04 — Federal Judge Labels Flock ALPR System &#x27;Indiscriminate Mass Surveillance&#x27;</a></li>

</ul>
</details>

**标签**: `#surveillance`, `#privacy`, `#flock-safety`, `#tech-industry`, `#ethics`

---

<a id="item-tech-news-16"></a>
### [EPA 悄然移除网络档案，政府数据保存引关注](https://www.motherjones.com/environment/2026/10/epa-online-archive-deletion-zeldin-camp-lejeune-trump-clean-power/) ⭐️ 6.0/10

Mother Jones 于 2026 年 10 月 26 日报道，美国环保署（EPA）正在悄悄关闭其在线网络档案，可能导致历史环境数据对公众不再可访问。报道聚焦于这一政策动作，但没有公布具体删除范围、时间表或技术细节。Hacker News 的讨论指出，这类页面仍可能通过 Internet Archive 的 Wayback Machine 和 End of Term Web Archive 等既有工具找到存档。

hackernews · robtherobber · 10月26日 19:05 · [社区讨论](https://news.ycombinator.com/item?id=50249275)

**「背景」** EPA 的在线档案长期收集该机构发布的报告、监管文件和历史数据，被视为外界回溯美国环境监管变化的重要入口。由于政府网站清理或改版容易造成链接失效，专门的网页存档项目通常会在政府换届等时间点批量保存联邦网站内容。

**「影响」** 依赖 EPA 原始档案的研究者、记者和公益组织应尽快通过第三方存档服务查找并保存所需页面，因为仅靠政府官网无法保证长期可访问。目前评论中有人在询问是否已有全站离线抓取，但尚未看到有人给出明确可用的抓取结果。

**「社区讨论」** 用户 toomuchtodo 给出了 Wayback Machine 针对 archive.epa.gov 的存档入口，并提醒 EPA 在 2022 年 3 月就已计划淘汰在线档案；dannyobrien 则认为 End of Term Web Archive 可能已保存相关内容，但表示让这些存档更容易访问仍是值得做的项目。另有用户询问是否已经有人抓取过 EPA 档案供离线使用，但没有得到确定答复。

**标签**: `#web archiving`, `#open data`, `#data preservation`, `#government transparency`, `#climate data`

---

<a id="item-tech-news-17"></a>
### [Deepity：C++/CUDA 预测编码库发布，CPU MNIST 基准领先](https://www.reddit.com/r/MachineLearning/comments/1xg6sqa/deepity_a_handtuned_ccuda_predictive_coding/) ⭐️ 6.0/10

Deepity 0.1.0a3（MIT 许可）已发布到 PyPI，这是一个由 C++20 手写 AVX2/AVX-512 SIMD 内核、OpenBLAS/MKL 与 CUDA 后端组成、并通过 nanobind 提供 Python 接口的预测编码库。作者报告在 12 代 i7-12700H 笔记本 CPU、784-512-512-10 sigmoid 网络、T=20 步、batch 250、100 epoch 的匹配配置下，Deepity 的 MNIST 准确率为 98.21%（487.5 秒），高于 jpc \(JAX\) 的 97.55%（531.4 秒）和 ngc-learn 的 98%（1707.7 秒）；同架构 PyTorch 反向传播参考结果为 97.51%（627.8 秒）。这些是开发者自报的 CPU 基准，CUDA 后端仍在调优，尚无经过验证的大规模训练数据。

reddit · r/MachineLearning · /u/Important-Home4431 · 10月26日 19:34

**「背景」** 预测编码（PC）与反向传播不同：它不再沿存储的计算图反向传播单一全局误差，而是让每层维护局部状态，并与上一层的自上而下预测比较，经过若干步“settling”减少自身预测误差后再只更新本层权重，因此无需保存另一层权重的转置或反向图。Deepity 是这种模型的从零实现，当前 CPU 路径是最成熟、有基准的部分；CUDA 后端使用 cuBLAS、CUTLASS 和 CUDA Graph 捕获来加速 settling 循环，但尚未面向大规模训练开放。

**「影响」** 对想尝试预测编码的研究者，现在可以直接执行 pip install pydeepity 并复现作者公布的 CPU 基准；但应把它视为 alpha 软件，CUDA 后端和卷积路径（目前为 im2col+cuBLAS，而非 cuDNN）仍不适合大批量训练，且基准未经独立验证。

**标签**: `#predictive coding`, `#C++`, `#CUDA`, `#machine learning`, `#open source`

---

<a id="item-tech-news-18"></a>
### [PBT 不加速 grokking，但可从超参数死区逃逸](https://www.reddit.com/r/MachineLearning/comments/1xfqhfc/pbt_doesnt_make_grokking_faster_but_it_can_escape/) ⭐️ 6.0/10

一项针对 grokking 的实证实验显示，在 mod 97 模加法、35%训练集、小型 MLP、20 个成员的设置下，Population Based Training（PBT）并不比固定网格更快：最优固定网格单元约 317±29 步达到 95%验证准确率，而 PBT 约 2667±2244 步，且每个种子都更慢。但在固定设置无法 grokking 的死区（学习率 1e-4 到 1e-3、权重衰减 0.01 到 0.08），固定网格 0/3 成功，慢速 PBT 0/3 成功，快速 PBT（每 100 步，×0.5/×2）3/3 成功，约 6850 步逃逸；宽随机搜索从同样的死区出发则以中位数 300 步达成 95%，远快于 PBT 的 6650 步。作者重放获胜超参数调度（不复制权重）在新初始化上 55/60 次达到 95%，而固定为调度几何均值的常参数为 0/60，说明逃逸主要来自调度本身。作者强调这是单任务、单模型、单数据划分的小规模实验，每个测试仅 3 到 10 个种子，多数 p 值高于 0.05，且重放调度属于事后挑选。

reddit · r/MachineLearning · /u/Virtual-Message-9739 · 10月26日 07:48

**「背景」** “Grokking”指的是模型在训练集上先出现过拟合、随后在某个时刻突然泛化到验证集的现象；Population-Based Training（PBT）则是一种在训练过程中动态调整超参数（如学习率、权重衰减）的群体式超参数优化方法。所谓“dead zone”，是指给定的超参数网格内没有任何固定配置能够实现 grokking 的区域。

**「影响」** 在这项实验范围内，PBT 应被视为超参数坏区间的救援工具而非加速手段：如果固定网格已包含可用区域，直接使用固定网格更快；如果固定网格落入死区，宽随机搜索在该任务上比 PBT 更早达到同样效果。研究者不应默认 PBT 能加快 grokking，而应先检查是否存在能工作的固定超参数区间，并警惕 PBT 可能塌缩到学习率下界、权重衰减上界的角落而无法离开。

**标签**: `#grokking`, `#population-based training`, `#hyperparameter optimization`, `#deep learning`, `#ML research`

---

<a id="item-tech-news-19"></a>
### [小米开源 HachimoDock：150 元自制语音 AI 硬件](https://weibo.com/1642634100/Ror200cVb) ⭐️ 6.0/10

小米技术委创新产品团队在 2026 观猹大会上亮相了开源 AI 硬件 HachimoDock，硬件自制成本约 150 元。该设备集桌宠、语音操控电脑 Agent 和智能家居联动于一体：用户可通过语音向电脑端 Codex、WorkBuddy 等 Agent 派发任务，也能联动小米 Miloco 控制家居；软件源码、物料清单、结构件模型及装配教程已在 GitHub 公开。需要留意的是，目前公开信息主要是产品发布和开源资料，尚未提供第三方实测数据或详细性能指标。

telegram · zaihuapd · 10月26日 05:31

**「背景」** 开源硬件通常以低成本、可复现的方式提供设备设计方案，而 AI Agent 和智能家居联动近年正从云端服务走向本地边缘设备。HachimoDock 是小米在开源硬件与 Agent 结合方向上的一个具体项目，其特点是用户可自行采购元件组装，并通过语音将任务交给电脑端 Agent 执行。

**「影响」** 对于 DIY 开发者和智能家居用户，HachimoDock 提供了一个约 150 元成本、可自行组装验证的语音控制入口，可以把现有电脑端 Agent 与小米 Miloco 家居生态连接起来。动手能力较强的用户可以按 GitHub 上的物料清单和装配教程复现，但实际效果仍取决于 Codex、WorkBuddy 等 Agent 的兼容性和 Miloco 生态的开放程度。

**标签**: `#open-source hardware`, `#AI agents`, `#Xiaomi`, `#smart home`, `#voice control`

---

<a id="item-tech-news-20"></a>
### [传 C-V2X 强标制定启动，乘用车或将强制装载](https://m.nbd.com.cn/articles/2026-10-26/4617416.html) ⭐️ 6.0/10

据每日经济新闻报道，知情人士称相关部门已启动 C-V2X（蜂窝车联网）强制性国家标准制定工作，相关工作组已成立，数十家单位参与；营运客车、货车已率先推进强制安装，未来有望扩大至乘用车。报道引述数据称，2026 年上半年中国乘用车前装标配 C-V2X 交付量为 34.4 万辆，同比增长 13.63%，但搭载率仅 4.03%。目前该消息仍属知情人士透露的初步监管动态，尚待官方正式确认。

telegram · zaihuapd · 10月26日 08:24

**「背景」** C-V2X（蜂窝车联网）是一种让汽车与其他车辆、道路设施及云端交换信息的技术，可实现盲区碰撞预警、事故提醒和智能信号灯提示，弥补摄像头、雷达的感知局限。报道称，营运客车、货车等已率先推进强制安装要求；截至 2026 年上半年，中国乘用车前装标配 C-V2X 交付量为 34.4 万辆，同比增长 13.63%，但搭载率仅为 4.03%。

**「影响」** 若强制标准未来从营运客车、货车扩大至乘用车，目前在售车型中约 96% 未前装 C-V2X 的车企将需要新增车联网硬件，并相应调整整车成本与产线配置；以 2026 年上半年乘用车前装交付 34.4 万辆、搭载率仅 4.03% 计算，改造覆盖面将远大于已先行推进强制安装的商用车领域。对已量产 C-V2X 功能的厂商而言，该功能可能从差异化卖点转变为进入中国乘用车市场的准入门槛。

**标签**: `#C-V2X`, `#Connected Vehicles`, `#China Regulation`, `#Intelligent Transportation`, `#Automotive Technology`

---

<a id="item-tech-news-21"></a>
### [即梦 AI 短剧工作室上线：一站式剧本到分镜工具](https://mp.weixin.qq.com/s/F--NRueOTrucjnJT_7Du6w) ⭐️ 6.0/10

字节跳动旗下即梦 AI 短剧工作室正式上线，覆盖剧本、分镜到后期制作的完整流程。工作室提供自研剧本模型 DreamScript、图片模型 Anycook 与分镜模型 DreamShot：DreamScript 支持多题材剧本生成和爆款诊断，可解析 10 万字长篇；Anycook 面向短剧角色与场景生成；DreamShot 支持画布与故事板双模式，并具备 3D 导演台动态预演能力。后期功能包括片段重拍、声音重构、智能切镜，以及原片智能解构与本地化重制转绘。

telegram · zaihuapd · 10月26日 10:16

**「背景」** 10 月 24 日的日报曾报道，字节跳动发布 Seedance 2.5 4K 视频生成模型，其 Draft 模式支持先用 480P 样片验证分镜、满意后再生成 4K 正片。即梦 AI 短剧工作室此次上线，可看作把这类分镜验证思路进一步扩展为从剧本、分镜到后期的一体化产品流程。

**「影响」** 对短剧创作者和制作机构而言，这套工作室把此前分散在多个工具中的剧本、分镜和后期环节集中到同一流程中。不过来源并未提供定价、开放范围或生成质量实测数据，实际效率和生成效果仍需进一步验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mp.weixin.qq.com/s/yUa8oh-IWfl5lDQzGSKWeg">2026-10-24 — 字节发布 Seedance 2.5 4K 模型，面向大荧幕</a></li>

</ul>
</details>

**标签**: `#AI tools`, `#generative media`, `#ByteDance`, `#content creation`, `#storyboarding`

---

