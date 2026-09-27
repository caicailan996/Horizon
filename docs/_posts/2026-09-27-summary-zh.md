---
layout: default
title: "Horizon Summary: 2026-09-27 (ZH)"
date: 2026-09-27
lang: zh
---

> 从 38 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [上诉法院维持 Anthropic 军事合同黑名单](#item-tech-news-1) ⭐️ 8.0/10
2. [Intel Panther Lake 拆解：18A 工艺内部观察](#item-tech-news-2) ⭐️ 7.0/10
3. [NumPy 手写 MLP 训练过程可视化教学工具](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek 弹性计算论文：380k 并发沙盒，131 位作者](#item-tech-news-4) ⭐️ 6.0/10
5. [Reladraw：可手动控制布局的文本式图表语言](#item-tech-news-5) ⭐️ 6.0/10
6. [告别 Google Play：Conversations 应用改为免费](#item-tech-news-6) ⭐️ 6.0/10
7. [GDB 18.1：子进程环境命令、历史保存与 Python API](#item-tech-news-7) ⭐️ 6.0/10
8. [DLR：先分解、看图、再推理](#item-tech-news-8) ⭐️ 6.0/10
9. [Excel 预览版支持单单元格多值存储与数组函数](#item-tech-news-9) ⭐️ 6.0/10
10. [LongCat-2.5-Preview 在 OpenCode 免费开放两周](#item-tech-news-10) ⭐️ 6.0/10

**财经新闻**
1. [10 年期美债收益率升至 19 年新高 5.23%，政府和 AI 相关债券发行激增是主因](#item-finance-news-1) ⭐️ 9.0/10
2. [苹果因 Apple Pay 收费被认证为反垄断集体诉讼](#item-finance-news-2) ⭐️ 7.0/10
3. [香港证监会与普华永道就恒大审计问题达成 10 亿港元和解](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [上诉法院维持 Anthropic 军事合同黑名单](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 8.0/10

美国华盛顿特区联邦上诉法院 9 月 25 日以 2 比 1 的投票维持五角大楼将 Anthropic 列入国家安全供应链风险黑名单的决定，理由是该公司拒绝允许其产品用于自主武器和大规模监控，因此被禁止参与军事合同。Anthropic 表示不同意这一裁决，正在考虑请求全体上诉法院复审；此前旧金山联邦法官曾依据另一部法律推翻列名，并阻止政府对 Anthropic 实施更广泛禁令。本次裁决与下级法院此前的结论相冲突，相关法律状态仍未完全确定。

telegram · zaihuapd · 9月26日 05:19

**「背景」** Anthropic 此前明确承诺，不将自家模型用于自主武器或大规模监控等高风险用途，这是五角大楼将其列入国家安全供应链风险名单的直接原因。此前旧金山联邦法官曾依据另一部法律推翻这一列名，并阻止政府对 Anthropic 实施更广泛的禁令；本次华盛顿特区联邦上诉法院以 2 比 1 维持黑名单，使围绕 AI 军事用途与公司伦理边界的法律争议进一步升级。

**「影响」** 这意味着 Anthropic 目前仍被排除在美国国防部军事合同之外，政府客户和合作方需要面临不一致的司法指令所带来的合规不确定性。Anthropic 下一步只能寻求全体上诉法院复审或继续诉讼，以争取改变这一结果。

**标签**: `#AI regulation`, `#national security`, `#Anthropic`, `#autonomous weapons`, `#supply chain risk`

---

<a id="item-tech-news-2"></a>
### [Intel Panther Lake 拆解：18A 工艺内部观察](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 7.0/10

SemiAnalysis 发布了一份免费的 STEEL 拆解报告，展示了 Intel Panther Lake 处理器及其 18A 工艺节点的内部结构。该分析基于早期硬件，为工程师和行业观察者提供了英特尔最新半导体技术的初步见解。由于具体发现未在公开摘要中详述，读者需查阅完整报告以获取详细技术信息。

rss · Semianalysis · 9月26日 13:36

**「背景」** Panther Lake 是英特尔首款采用 18A 工艺的处理器系列，此前的报道称该系列 SoC 计划于 2025 年底推出，并已有合作伙伴进行测试。SemiAnalysis 的拆解针对 Core Ultra 7 365 样品，检查了 18A 结构、PowerVia 布线以及各 tile 层面的工艺选择。

**「影响」** 该拆解为工程师和行业观察者提供了 Panther Lake 实际芯片的早期物理证据，可用于对照英特尔 18A 工艺宣称的 GAAFET、BSPD 等特性，评估其客户端 SoC 的技术成熟度；鉴于 Panther Lake 被定位为首款基于 18A 的 AI PC 平台，相关发现可能影响后续平台选型与设计决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18 A teardown : what it found | NeoTeo</a></li>
<li><a href="https://wccftech.com/intels-18a-process-shows-great-performance-as-panther-lake-socs-are-finally-up/">Intel &#x27;s 18 A Process Shows &quot;Great Performance&quot; As Initial Panther ....</a></li>
<li><a href="https://www.linkedin.com/posts/enigma-security_intel-pantherlake-pctechnology-activity-7382348178563473408-WJUJ"># intel # pantherlake #pctechnology #advancedchips #aiinhardware...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown, 18 A , BSPD, GAAFET, SemiAnalysis...</a></li>
<li><a href="https://www.linkedin.com/posts/nqobile-predict-maseko-78bbb0249_intel-pantherlake-ai-activity-7382096572819496960-1St8">Intel Unveils Panther Lake : AI PC Platform on 18 A Node | LinkedIn</a></li>

</ul>
</details>

**标签**: `#Intel`, `#Panther Lake`, `#Intel 18A`, `#semiconductor`, `#chip teardown`

---

<a id="item-tech-news-3"></a>
### [NumPy 手写 MLP 训练过程可视化教学工具](https://www.reddit.com/r/MachineLearning/comments/1wqy1qd/p_a_small_mlp_from_scratch_in_numpy_with_a_gui_to/) ⭐️ 7.0/10

作者发布了一个纯 NumPy 实现的 MLP 教学工具（GitHub 项目 neural-network-digits），不使用自动求导，而是靠手动反向传播、带动量的 SGD、L2、Dropout、余弦退火和 4 种激活函数训练；在完整 MNIST 上约达到 98.5% 的准确率。界面会实时展示每个批次和轮次的损失、各层梯度范数、失活神经元比例、初始化前后的权重分布以及首层感受野，并提供逐层 PCA/t-SNE、噪声和旋转鲁棒性曲线，以及单神经元消融、缩放、剪枝、权重加噪和 softmax 温度调整等实验。该工具面向从高中到入门机器学习课程的学生、自学者以及想在课堂上演示神经网络的教师。

reddit · r/MachineLearning · /u/No-Brain-1655 · 9月26日 18:38

**「背景」** 多层感知机（MLP）是最基础的前馈神经网络，但反向传播和权重更新过程通常不可见，容易被当作黑盒。该工具刻意用 NumPy 手写完整训练循环，并把权重分布、激活变化和错误预测等内部状态可视化，便于在教学时对照理论讲解。

**「影响」** 对讲授或自学机器学习的人来说，这个工具可以作为交互式教具：直接修改某个神经元的缩放、剪切权重或调节 softmax 温度，测试准确率会立即更新，从而直观验证单个单元对整体模型的作用。

**标签**: `#machine learning`, `#educational tool`, `#visualization`, `#neural networks`, `#NumPy`

---

<a id="item-tech-news-4"></a>
### [DeepSeek 弹性计算论文：380k 并发沙盒，131 位作者](https://arxiv.org/abs/2609.22978) ⭐️ 6.0/10

DeepSeek 在 arXiv 上发表了一篇弹性计算（DSec）系统论文，据论文声称，该系统能在 160 个 AMD EPYC 服务器节点上支持 380,000 个并发沙盒。论文作者列表长达 131 人（另有 31 人未在页面中显示），引发社区对作者数量的讨论。该论文描述了用于 AI 训练和推理的弹性基础设施能力，但所有性能数据均来自论文自述，尚未经独立验证。

hackernews · shenli3514 · 9月26日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=49859112)

**「背景」** DeepSeek Elastic Compute \(DSec\) 是一个生产级沙箱基础设施，为智能体训练提供弹性执行平台，支持函数调用、容器、微型虚拟机及全虚拟机四种沙箱后端。论文披露其单套生产单元约 160 个节点，每天处理约 300 万个沙箱实例，峰值并发超过 38 万个，每秒可创建 5000 个以上沙箱。这些数字凸显了支撑大规模并行智能体训练所需的系统规模。

**「影响」** 如果 DeepSeek 的弹性计算规模得以复现，对于需要大量隔离沙盒进行分布式 AI 训练或安全测试的团队而言，可能意味着更低的硬件成本和更高的资源利用率。但当前数据仅为论文声明，实际效果需等待第三方基准测试或开源实现确认。

**「社区讨论」** 有评论者指出，DeepSeek 将几乎所有员工列为论文作者（共 131 人），可能是为了防止核心人才被竞争对手挖走，即“人力资产保护”策略。另有评论者关注到 380k 并发沙盒在 160 个节点上的性能数字，猜测该技术可用于构建大规模代理集群。这些观点均为参与者个人推测，并非论文结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>

</ul>
</details>

**标签**: `#elastic-compute`, `#deepseek`, `#ai-infrastructure`, `#distributed-systems`, `#machine-learning`

---

<a id="item-tech-news-5"></a>
### [Reladraw：可手动控制布局的文本式图表语言](https://github.com/reladraw/reladraw) ⭐️ 6.0/10

Reladraw 是一个在 GitHub 上发布的文本式图表语言，目标是让用户（包括人类和 AI 代理）在定义图表时保留对布局的高自由度控制，而不是像 Mermaid 或 Graphviz 那样完全自动排布。项目提供了无需安装的在线 playground、npm install 安装方式，以及用于 Claude 或其他代理的 skill 安装说明。目前项目仍偏早期，社区已报告了曲线箭头等边缘用例还不够完善。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**「背景」** 常见的文本图表 DSL 分两类：Mermaid、Graphviz 这类自动布局语言无法让用户精细决定最终外观；Draw.io 这类手动工具虽然灵活，但耗时且代理难以高效操作。Reladraw 试图用文本 DSL 同时兼顾布局控制和代理可操作性。

**「影响」** 对于在 AI 编码工作流中依赖图表来对齐思路的开发者，Reladraw 提供了一种代理可以直接编辑、同时保留布局控制的方案；可以先在 playground 里验证效果，再通过 npm 集成到现有流程。评论者也指出，若要用于 C4 这类固定架构图，还需要把拓扑定义与布局指令进一步解耦。

**「社区讨论」** 评论整体认可这个方向，HeavyStorm 认为相对定位对流程图已经足够；Garlef 建议将箭头、分组等拓扑部分与 left of、right of 等布局指令解耦；recroad 则报告了“edge parser -&gt; renderer”这类语句无法自动生成曲线箭头的 bug。

**标签**: `#diagramming`, `#DSL`, `#developer tools`, `#AI agents`, `#open source`

---

<a id="item-tech-news-6"></a>
### [告别 Google Play：Conversations 应用改为免费](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 6.0/10

Conversations 开发者宣布该应用现在免费，并解释了与 Google Play 分手的原因。文章把这次变动描述为开发者个人选择，相关讨论集中在 Play Store 抽成与支持体验上；目前没有披露具体分发渠道或附加条件。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**「背景」** Conversations 是一款 Android 上的 XMPP 联邦式即时通讯应用，此前在 Google Play 上为付费应用，开发者 Daniel Gultsch 最初没有在官网直接推广 F-Droid 免费渠道。Horizon 9 月 25 日的日报曾报道 F-Droid 2.0 发布，这是该官方自由软件应用商店客户端十年来最大的一次更新。此后 Conversations 把 F-Droid 作为主要分发渠道，现在开发者宣布该应用免费，并脱离 Google Play 分发。

**「社区讨论」** 评论中，k1w1 报告称，Google 的上架电话验证要求支持号码能接收短信或被人工即时接听，带 IVR 的客服号码无法通过，导致他们的产品一年未能上架。pi-victor 则认为问题主要不是 15% 抽成，而是 Google Play 缺乏支持和快速审核，并因垄断地位不必改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html">2026-09-25 — F-Droid 2.0 launches Android app store overhaul and new UI</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**标签**: `#Android`, `#Google Play`, `#open source`, `#app distribution`, `#developer experience`

---

<a id="item-tech-news-7"></a>
### [GDB 18.1：子进程环境命令、历史保存与 Python API](https://lwn.net/Articles/1096897/) ⭐️ 6.0/10

GDB 18.1 已发布，这是 GNU 交互式调试器的一次小幅更新。新版新增了用于操作子进程环境的命令、将命令历史保存到文件的功能，并加入了对几个新目标的支持和多项 Python API 扩展。完整变更列表见随版本提供的 NEWS 文件。

rss · LWN.net · 9月26日 15:03

**「背景」** GDB（GNU 调试器）是一款用于各类编程语言的命令行调试工具，广泛应用于系统级开发和开源软件调试。此前版本为 GDB 18.0，本次 18.1 是新一轮的小版本更新。

**「影响」** 需要使用这些新功能的 GDB 用户应升级到 18.1，并查阅 NEWS 文件，以确认新增子进程环境命令、目标支持和 Python API 的具体名称与用法。

**标签**: `#gdb`, `#debugger`, `#open-source`, `#software-development`, `#gnu`

---

<a id="item-tech-news-8"></a>
### [DLR：先分解、看图、再推理](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%9D%A2%E5%90%91%E8%A7%86%E8%A7%89%E8%AF%AD%E8%A8%80%E6%A8%A1%E5%9E%8B%E7%9A%84%E5%BC%BA%E5%8C%96%E9%9A%90%E7%A9%BA%E9%97%B4%E6%8E%A8%E7%90%86%EF%BC%9A%E5%85%88%E5%88%86%E8%A7%A3%E3%80%81%E7%9C%8B%EF%BC%8C%E5%86%8D%E6%8E%A8%E7%90%86%7CEMNLP%2726) ⭐️ 6.0/10

美国埃默里大学研究团队提出强化隐空间推理方法 Decompose, Look, and Reason（DLR），论文被 EMNLP 2026 主会议接收，并公开了 arXiv 预印本（2604.07518）。DLR 针对多模态思维链中“文本推理不断拉长、视觉证据逐步变弱”的问题，将推理组织为“先拆解子问题，再针对该子问题查看图像，最后基于刚获得的视觉证据推理”的循环，属于在隐空间反复注入视觉表示的路线。源报道未提供基准测试数字，因此论文的实际效果尚需以全文评测为准。

rss · 新智元 · 9月26日 14:00

**「背景」** 视觉语言模型（VLM）在多模态推理中需要在离散语言序列与高维连续视觉表示之间反复交互。此前方法大致有三条路线：将视觉信息压缩为文本后在语言空间推理，但会产生信息损失；在中间步骤引入图像 patch、bounding box、crop、zoom 或外部视觉工具，能增强显式 grounding，但增加工具调用成本且受预定义操作空间限制；以及把中间视觉信息投影到连续潜在空间，但现有实现常依赖局部 ROI 或只在整条推理链中注入一次视觉 latent。DLR 正是针对“局部 ROI 与当前推理所需语义不一致、单次视觉注入难以支撑多步推理”的局限而提出。

**标签**: `#vision-language models`, `#reinforcement learning`, `#latent space reasoning`, `#EMNLP`, `#AI research`

---

<a id="item-tech-news-9"></a>
### [Excel 预览版支持单单元格多值存储与数组函数](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 6.0/10

微软在 Excel 中引入列表、单元格内数组与嵌套数组功能，率先面向 Windows 和 Mac 的 Beta 通道用户推送。这是 Excel 40 年来首次允许一个单元格存放多个值（例如用 Ctrl+J 或“插入 &gt; 列表”写入逗号或分号分隔的多个项目），并支持按单项筛选与计算。同时新增 FLATTEN、HAS、HASANY、HASALL 四个数组处理函数。所有功能均为预览，正式发布前行为可能调整，官方建议暂不用于重要工作簿。

telegram · zaihuapd · 9月26日 16:26

**「背景」** 传统 Excel 工作表中，每个单元格只能存储单个值（数字、文本或公式结果），多值需分散到多个单元格。这一设计自 Excel 诞生起持续约 40 年，本次更新打破了此限制，使单元格能直接包含列表或数组，并对数组元素进行独立操作。

**「影响」** Beta 通道用户可直接试用新功能，但微软明确提示预览版行为可能变更，因此不建议在生产环境或重要工作簿中依赖该功能。正式发布前，依赖这些新函数或列表公式的工作表可能因后续调整而失效。

**标签**: `#Excel`, `#Microsoft 365`, `#spreadsheet`, `#arrays`, `#productivity tools`

---

<a id="item-tech-news-10"></a>
### [LongCat-2.5-Preview 在 OpenCode 免费开放两周](https://x.com/Meituan_LongCat/status/2103844449550020816) ⭐️ 6.0/10

美团 LongCat 于 2026 年 9 月 26 日开放 LongCat-2.5-Preview，在 OpenCode 平台上提供为期两周的免费试用。该预览模型支持 100 万 token 上下文、多模态输入，并承诺零数据留存。目前这仍是试用性质的发布预告，尚无可依赖的独立基准或详细技术评测。

telegram · zaihuapd · 9月27日 01:41

**「背景」** LongCat 是美团推出的长上下文大模型系列，OpenCode 是提供模型调用的平台之一。本次公告显示，LongCat-2.5-Preview 将在 OpenCode 免费开放两周，支持 1M 上下文、多模态和零数据留存；不过 OpenCode 文档仅将入口标注为“限时免费”，未写明具体截止日期，两周期限目前来自聚合报道和官方推文。

**「影响」** 对需要在 OpenCode 中处理长文档或多模态任务的开发者，这是一次限时免费接入机会，可在两周试用期内实测其 1M 上下文能力及零数据留存承诺是否符合实际使用体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.orcarouter.ai/blog/longcat-2-5-preview-free-opencode">LongCat-2.5-Preview free on OpenCode: 1M tokens, no end date</a></li>
<li><a href="https://x.com/Meituan_LongCat/status/2103844449550020816">Meituan LongCat on X: &quot;LongCat-2.5-Preview is now free to try on @opencode for two weeks! 🐱 Give it a spin and show us what you build.&quot; / X</a></li>
<li><a href="https://x.com/opencode/status/2103841640171614322">OpenCode on X: &quot;LongCat-2.5-Preview is now free on OpenCode for two weeks - 1M Context - Multi-modal - Zero Data Retention&quot; / X</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Model`, `#Multimodal`, `#OpenCode`, `#Model Preview`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [10 年期美债收益率升至 19 年新高 5.23%，政府和 AI 相关债券发行激增是主因](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 9.0/10

本周 10 年期美国国债收益率升至 5.23%，创 2007 年以来最高水平，此前 9 月初该收益率还低于 4.8%。推动因素包括粘性通胀下市场对美联储 10 月加息的预期升温（CME FedWatch 显示概率为 64%），但策略师指出，更主要的原因是联邦政府为弥补赤字大量发债，以及 Alphabet、亚马逊、Meta、微软和甲骨文等公司为 AI 基础设施融资而发行的企业债激增——Vanguard 估算这些公司今年前 7 个月发债 1320 亿美元，远高于 2020-2024 年间约 350 亿美元的年均值。

rss · CNBC Finance · 9月26日 13:30

**「背景」** 债券收益率与价格反向变动；10 年期美债收益率是美国抵押贷款、企业借贷和股市估值的关键基准。此前收益率上行主要受通胀和加息预期驱动，而当前供应端压力来自政府赤字融资与 AI 投资潮叠加，导致债券供给大增。

**「影响」** 美债收益率走高直接推升房贷和企业融资成本，并可能使债券相对股票更具吸引力，从而压制股市表现。Macquarie 策略师警告，若 AI 资本支出计划持续，收益率可能进一步上行。

**标签**: `#Treasury yields`, `#Federal Reserve`, `#Inflation`, `#Bond issuance`, `#AI investment`

---

<a id="item-finance-news-2"></a>
### [苹果因 Apple Pay 收费被认证为反垄断集体诉讼](https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/) ⭐️ 7.0/10

美国联邦法官认证了一项针对苹果的反垄断集体诉讼，原告指控苹果就 Apple Pay 交易向发卡机构（发行银行卡的银行或金融公司）收取过高费用：信用卡交易按 0.15%、借记卡交易每笔按 0.5 美分收费。诉讼称这些费用每年最高可达 10 亿美元，并要求退还费用和寻求禁令。

telegram · zaihuapd · 9月26日 03:32

**「背景」** 原告还称，安卓手机钱包不向发卡机构收取这类费用，且苹果阻止其他公司开发竞争性钱包；集体成员涵盖所有在美国发行支持 Apple Pay 卡片并支付相关费用的机构。

**「影响」** 对美国发卡机构而言，若原告最终胜诉，可能获得费用退还及收费方式改变；但目前法院认证集体诉讼只代表案件可以继续审理，并不等于已认定苹果违法。

**标签**: `#Apple`, `#Apple Pay`, `#class action`, `#antitrust`, `#mobile payments`

---

<a id="item-finance-news-3"></a>
### [香港证监会与普华永道就恒大审计问题达成 10 亿港元和解](https://wallstreetcn.com/articles/3782573) ⭐️ 7.0/10

香港证监会与普华永道（香港）就中国恒大审计失职达成和解，普华永道不承认责任，但同意支付 10 亿港元用于补偿受影响的独立小股东。这笔款项来自普华永道香港自身财产，不影响恒大债权人原有的申索优先次序。

telegram · zaihuapd · 9月26日 07:18

**「背景」** 香港证监会此前指控普华永道（香港称罗兵咸永道）在审计中国恒大集团时存在失职，导致其财务报表虚假。此次达成的 10 亿港元和解协议旨在赔偿受影响的独立小股东，但恒大清盘人已入禀香港高等法院要求撤销该协议，法院预计 10 月底作出判决。

**「影响」** 若和解获法院批准，曾因恒大财务报表造假而遭受损失的独立小股东可获得赔偿，但恒大清盘人已入禀要求撤销和解，最终结果有待香港高等法院预计 10 月底的判决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eu.36kr.com/zh/p/3780065714148610">8点1氪： 华 谊兄弟被申请破产重整， 普 华 永 道 因 恒 大 审 计 赔偿 10 ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260424A01VGD00">普 华 永 道 将支付 10 ...</a></li>

</ul>
</details>

**标签**: `#香港证监会`, `#普华永道`, `#恒大`, `#审计监管`, `#和解`

---