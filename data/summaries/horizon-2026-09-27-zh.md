# Horizon 每日速递 - 2026-09-27

> 从 36 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [DeepSeek 弹性计算论文 DSec 引热议](#item-tech-news-1) ⭐️ 8.0/10
2. [Reladraw：让用户决定元素位置的图表 DSL](#item-tech-news-2) ⭐️ 7.0/10
3. [SemiAnalysis 免费拆解 Intel 18A 与 Panther Lake](#item-tech-news-3) ⭐️ 7.0/10
4. [AI 门萨智商测试满分 151，碾压 99.97% 人类](#item-tech-news-4) ⭐️ 7.0/10
5. [美国法院维持将 Anthropic 列入黑名单](#item-tech-news-5) ⭐️ 7.0/10
6. [Excel 首次支持单元格内多值及四个新数组函数](#item-tech-news-6) ⭐️ 7.0/10
7. [Conversations 离开 Google Play，免费开放](#item-tech-news-7) ⭐️ 6.0/10
8. [GDB 18.1 发布：新增子进程环境与命令历史功能](#item-tech-news-8) ⭐️ 6.0/10
9. [纯 NumPy MLP 教育工具：实时可视化训练内部过程](#item-tech-news-9) ⭐️ 6.0/10
10. [分布式算法学习指南：LLM 训练与推理的论文与开源实现](#item-tech-news-10) ⭐️ 6.0/10
11. [LongCat-2.5-Preview 在 OpenCode 免费两周](#item-tech-news-11) ⭐️ 6.0/10
12. [OpenAI 计划扩大 Ultrafast API 访问范围](#item-tech-news-12) ⭐️ 6.0/10

**财经新闻**
1. [10 年期美债收益率升至 5.23%，为 2007 年以来最高](#item-finance-news-1) ⭐️ 8.0/10
2. [苹果因 Apple Pay 收费面临美国反垄断集体诉讼](#item-finance-news-2) ⭐️ 7.0/10
3. [中行万事达卡被指疑似遭境外盗刷 用户紧急锁卡](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DeepSeek 弹性计算论文 DSec 引热议](https://arxiv.org/abs/2609.22978) ⭐️ 8.0/10

DeepSeek 在 arXiv 发布了弹性计算系统 DSec 的论文预印本。据 Hacker News 讨论，该系统能在约 160 个 Epyc 服务器节点上运行 38 万并发沙箱，被评论者拿来与 Google 的 ax 项目比较。目前该消息仅基于论文列表页和社区讨论，相关规模与性能数据尚未得到独立验证。

hackernews · shenli3514 · 9月26日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=49859112)

**「背景」** DeepSeek 在 arXiv 发表的论文介绍了 DSec，称其为用于大规模智能体（agentic）训练的生产级沙箱平台，通过统一的 SDK 暴露 FnCall、容器、microVM 和完整虚拟机等多种沙箱后端。这篇论文的背景是大规模智能体训练需要弹性执行平台，而非单一的沙箱运行时。

**「对开发者与基础设施的影响」** 根据 DeepSeek 在 arXiv 上发布的 DSec 论文及 Pandaily 的报道，该系统声称在仅 160 个 AMD Epyc 服务器节点上即可达成超过 38 万个并发沙箱、每秒超过 5,000 个沙箱创建速率以及每日约 300 万沙箱的处理能力。这意味着，对于从事 Agent 强化学习训练的团队而言，DSec 展示了一种在相对紧凑的集群规模下实现极高隔离任务并发的可能路径，从而大幅降低大规模 Agent 训练的基础设施成本或节点密度需求。不过，这些数字来自预印本论文的自我声明，尚未经过第三方独立复现或验证，在实际部署前应审慎评估其可靠性。

**「社区讨论」** 评论中既有对规模的惊讶，也有对作者名单的讨论：有评论认为列出大量作者可能是防止核心员工被挖角的人才资产保护策略，另有评论者好奇 131 名作者如何协作完成论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://pandaily.com/deepseek-dsec-elastic-compute-agentic-training-sandbox-3m-day">DeepSeek Details DSec Elastic Compute : Agentic-Training... - Pandaily</a></li>
<li><a href="https://arxiv.org/abs/2609.22978v1">[2609.22978v1] DeepSeek Elastic Compute (DSec): A Sandbox ...</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#elastic-compute`, `#ai-infrastructure`, `#sandboxing`

---

<a id="item-tech-news-2"></a>
### [Reladraw：让用户决定元素位置的图表 DSL](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw 是一个新的开源图表描述语言（DSL），在文本定义图表的同时允许用户通过相对位置控制布局，兼顾人类和 AI agent 的使用需求。项目已在 GitHub 发布，提供无需安装的在线 playground、npm install 安装方式，以及适用于 Claude 或其他 agent 的 skill 安装说明。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**「背景」** 此前的文本图表语言如 Mermaid 或 Graphviz 采用自动布局，用户难以决定最终外观；而以 Draw.io 为代表的手工绘图工具虽然灵活，但操作耗时，也不方便 agent 直接操作。Reladraw 试图填补这两类工具之间的空白。

**「影响」** 需要精确控制图表外观的开发者，以及需要以文本方式驱动图表生成的 AI agent 工作流，可以直接在 playground 中试用 Reladraw，或通过 npm 将其集成到现有工具链中。

**「社区讨论」** 有评论者认为相对定位对大多数流程图已经够用，Mermaid 在处理固定布局（如时序图）时很好，但流程图需要位置控制；也有人报告 Reladraw 在解析“edge parser -&gt; renderer”这类带方向描述时仍不够智能，未能生成弯曲箭头。另有用户建议将拓扑关系与布局关注点分离，使其更适合作为 C4 模型的布局层。

**标签**: `#diagramming`, `#domain-specific-language`, `#developer-tools`, `#ai-agents`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [SemiAnalysis 免费拆解 Intel 18A 与 Panther Lake](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 7.0/10

SemiAnalysis 发布了一篇免费的拆解分析报告，面向公众开放，重点检查 Intel 18A 工艺节点以及 Intel 的 Panther Lake 处理器。该报告归属其 STEEL 拆解系列，但当前公开摘要未披露具体测量数据、性能结果或发售细节等更深层次的技术结论。

rss · Semianalysis · 9月26日 13:36

**「背景」** Intel 18A 是英特尔采用 PowerVia 背面供电等关键结构的先进制程节点，Panther Lake 是其首批应用该节点的客户端处理器产品。SemiAnalysis 的这篇拆解针对 Core Ultra 7 365 样品，用于观察 18A 的实际结构、布线路径以及模块级工艺选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown , 18A, BSPD, GAAFET, SemiAnalysis ...</a></li>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18A teardown : what it found | NeoTeo</a></li>

</ul>
</details>

**标签**: `#Intel`, `#semiconductors`, `#hardware`, `#process technology`, `#teardown`

---

<a id="item-tech-news-4"></a>
### [AI 门萨智商测试满分 151，碾压 99.97% 人类](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%97%A8%E8%90%A8%E6%99%BA%E5%95%86%E6%B5%8B%E8%AF%95%E8%A2%ABAI%E8%80%83%E7%88%86%E4%BA%86%EF%BC%81151%E6%BB%A1%E5%88%86%E7%99%BB%E9%A1%B6%EF%BC%8C99.97%25%E4%BA%BA%E7%B1%BB%E8%A2%AB%E7%A2%BE%E5%8E%8B) ⭐️ 7.0/10

Claude Fable 5.1 与 GPT-6 Astra 在门萨挪威智商测试（35 道图形推理题，限时 25 分钟）中连续 7 次获得理论满分 151 分，超越 99.97% 人类得分者。该测试仅考察流体智力，不依赖知识储备，此前人类最高只能测到 145 分。目前尚不清楚这些 AI 模型的能力上限。

rss · 新智元 · 9月26日 08:06

**「背景」** 门萨挪威智商测试由 35 道图形推理题组成，限时 25 分钟，不依赖知识储备，侧重考察“流体智力”，即面对陌生图形临场找规律的能力。此类测试也常用于检验视觉模型的视觉推理表现，测评平台 tracking AI 便注明视觉模型需要直接查看测试图片作答。

**「影响」** 这一结果意味着在纯粹图形推理的流体智力维度上，当前最强 AI 已完全超越人类基准。对于依赖此类测试的人才筛选或认知研究，AI 的满分表现可能促使重新评估智商测试的有效性；对于 AI 开发者，这展示了多模态推理能力的重大进步，但需注意该成就不等同于通用智能或现实世界的问题解决能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trackingai.org/">IQ Test | Tracking AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#IQ test`, `#Mensa`, `#benchmarking`, `#artificial intelligence`

---

<a id="item-tech-news-5"></a>
### [美国法院维持将 Anthropic 列入黑名单](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 7.0/10

美国华盛顿特区联邦上诉法院 9 月 25 日以 2 比 1 裁决，维持五角大楼将 Anthropic 列为国家安全供应链风险并禁止其参与军事合同的决定。多数法官认为，Anthropic 拒绝允许其产品用于自主武器和大规模监控，五角大楼的担忧合理。Anthropic 表示不同意裁决，正考虑请求全体上诉法院复审；此前旧金山联邦法官曾依据另一部法律推翻相关列名。

telegram · zaihuapd · 9月26日 05:19

**「背景」** 五角大楼的“黑名单”指其依据国家安全供应链风险将企业列为受限制实体，禁止其参与军事合同；Anthropic 因拒绝允许产品用于自主武器和大规模监控而被列入。此前，旧金山联邦法官曾依据另一部法律推翻该列名，并阻止政府对 Anthropic 实施更广泛禁令，但本次华盛顿特区上诉法院以 2 比 1 裁决维持了列名。

**「影响」** 在列名维持期间，Anthropic 无法获得美国国防部军事合同；Anthropic 若成功推动全体上诉法院复审，这一准入限制可能被推翻。

**标签**: `#Anthropic`, `#AI policy`, `#national security`, `#military contracts`, `#regulation`

---

<a id="item-tech-news-6"></a>
### [Excel 首次支持单元格内多值及四个新数组函数](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

微软在 Excel 中推出列表、单元格内数组与嵌套数组，率先面向 Windows 和 Mac 的 Beta 通道提供，这是 Excel 40 年来首次允许一个单元格存放多个值。用户可通过 Ctrl+J 或“插入 &gt; 列表”输入以逗号或分号分隔的多个项目，并可按单项进行筛选与计算。同时新增 FLATTEN、HAS、HASANY、HASALL 四个数组函数。所有功能目前均为预览，正式发布前行为可能调整，官方建议暂不用于重要工作簿。

telegram · zaihuapd · 9月26日 16:26

**「背景」** 自 1985 年发布以来，Excel 一直以每个单元格只保存一个值为基本设计，这使得同一位置无法直接存放多个项目。微软于 2026 年 9 月 24 日通过 Microsoft 365 Insider 博客宣布，向 Windows 和 Mac 的 Beta 通道推出列表、单元格内数组与嵌套数组，并附带兼容性版本 3；微软强调该功能仍是预览性质，不建议用于重要的生产工作簿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>
<li><a href="https://windowsforum.com/news/excel-beta-adds-lists-and-nested-arrays-with-compatibility-version-3.445888/">Excel Beta Adds Lists and Nested Arrays With Compatibility Version 3</a></li>
<li><a href="https://windowsforum.com/news/excel-beta-adds-lists-and-nested-arrays-with-compatibility-version-3.445888/?amp=1">Excel Beta Adds Lists and Nested Arrays With Compatibility Version 3 | Windows Forum</a></li>

</ul>
</details>

**标签**: `#Excel`, `#Microsoft 365`, `#spreadsheet`, `#data management`, `#arrays`

---

<a id="item-tech-news-7"></a>
### [Conversations 离开 Google Play，免费开放](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 6.0/10

开源 XMPP 聊天应用 Conversations 的开发者 Daniel Gultsch 宣布退出 Google Play，原因是对 Google 的支持和审核政策感到失望。该应用现已免费提供，用户可通过 F-Droid 或 GitHub 获取。此前 Conversations 在 Play Store 上售价 4.99 美元，但开发者认为 15% 的分成并未换来应有的支持。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**「背景」** Conversations 是由 Daniel Gultsch 于 2014 年开发的基于 XMPP 的开源 Android 即时通讯客户端。此前，它在 Google Play 上以付费形式提供，同时在 F-Droid 上也有免费版本，但开发者并未主动宣传 F-Droid 版本。如今，由于对 Google Play 的支持和政策不满，作者决定完全退出该平台，并将 Conversations 免费开放。

**「影响」** 现有用户若此前通过 Play Store 购买，将无法再获得自动更新，需手动迁移至其他分发渠道。其他开发者则需重新评估对单一平台的依赖风险。

**「社区讨论」** 多位用户指出 Google Play 存在严重支持问题，例如电话号码验证流程对机构不友好、侧载警告日益强化。有评论认为，Google 作为垄断平台，糟糕的支持却未受到市场惩罚。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conversations_%28software%29">Conversations (software) - Wikipedia</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**标签**: `#android`, `#google play`, `#open source`, `#app distribution`, `#developer experience`

---

<a id="item-tech-news-8"></a>
### [GDB 18.1 发布：新增子进程环境与命令历史功能](https://lwn.net/Articles/1096897/) ⭐️ 6.0/10

GDB 18.1 交互式调试器已正式发布。本次版本新增用于操纵子进程环境的命令、将命令历史保存到文件的功能，并增加对若干新目标的支持及多项 Python API 增强；完整变更列表见 NEWS 文件。

rss · LWN.net · 9月26日 15:03

**「背景」** GDB（GNU Debugger）是 GNU 项目维护的交互式调试器，代码托管在 binutils-gdb 仓库中；借助它，开发者可以在程序运行时设置断点、检查变量并跟踪执行流。18.1 是该项目的常规版本号更新，完整改动清单由仓库内的 NEWS 文件公布。

**标签**: `#gdb`, `#debugging`, `#developer-tools`, `#release`, `#python-api`

---

<a id="item-tech-news-9"></a>
### [纯 NumPy MLP 教育工具：实时可视化训练内部过程](https://www.reddit.com/r/MachineLearning/comments/1wqy1qd/p_a_small_mlp_from_scratch_in_numpy_with_a_gui_to/) ⭐️ 6.0/10

这是一个用纯 NumPy 从头构建的多层感知器（MLP）教育工具，无需自动求导，通过手动反向传播、带动量的 SGD、L2 正则化、Dropout、余弦退火和四种激活函数，在 MNIST 上达到约 98.5%的测试准确率。其 GUI 在训练过程中实时显示损失、逐层梯度范数与失活神经元比例、权重分布变化以及第一层感受野。此外，还提供逐层 PCA/t-SNE 可视化、噪声与旋转鲁棒性曲线、以及神经元消融和缩放等交互式实验功能，适合从高中生到机器学习入门课程的自学者和教师使用。

reddit · r/MachineLearning · /u/No-Brain-1655 · 9月26日 18:38

**「背景」** 多层感知器（MLP）是神经网络的基础架构，通常依赖 PyTorch 或 TensorFlow 等框架的自动求导机制。该工具完全基于 NumPy 手动实现反向传播，让学习者能够观察并操控梯度流动、权重演化及神经元活动，从而更直观地理解训练过程的内部原理。

**「影响」** 该工具为机器学习教育提供了直观且可交互的演示平台，学生可以通过消融单个神经元、调整噪声强度或改变 softmax 温度，即刻观察到准确率的变化，将抽象概念具象化，有助于从高中到高等教育的不同层次学习者掌握神经网络的训练机制。

**标签**: `#educational tool`, `#NumPy`, `#MLP`, `#visualization`, `#neural network training`

---

<a id="item-tech-news-10"></a>
### [分布式算法学习指南：LLM 训练与推理的论文与开源实现](https://www.reddit.com/r/MachineLearning/comments/1wqk0x2/a_little_guide_to_learning_distributed_algorithms/) ⭐️ 6.0/10

一位 Reddit 用户在 r/MachineLearning 发布了一份入门指南，列出其过去三个月阅读的若干分布式算法基础论文，并附上 AlphaXiv 共享文件夹链接和 GitHub 仓库 smolcluster（含基础级参考实现）。该资源面向想了解分布式并行、张量并行、流水线并行与模型并行，但不知从何开始的 LLM 训练/推理学习者。帖子未给出具体论文清单或技术细节，属于个人经验分享，而非权威教程。

reddit · r/MachineLearning · /u/East-Muffin-6472 · 9月26日 07:10

**「背景」** 分布式训练与推理一般需要理解分布式系统及其并行方式，包括数据并行、张量并行、流水线并行和模型并行。这些概念是阅读和实现相关论文的前提。

**「影响」** 对刚入门的 LLM 训练/推理学习者，这份帖子把常见的学习路径压缩为约三个月的论文阅读清单，并提供一个基础实现作为对照，降低“不知道从哪开始”的门槛。使用时应把帖子当作路标，最终以论文原文和仓库现状为准。

**标签**: `#distributed systems`, `#LLM training`, `#LLM inference`, `#distributed parallelism`, `#machine learning education`

---

<a id="item-tech-news-11"></a>
### [LongCat-2.5-Preview 在 OpenCode 免费两周](https://x.com/Meituan_LongCat/status/2103844449550020816) ⭐️ 6.0/10

据 Meituan LongCat 官方社交账号宣布，LongCat-2.5-Preview 将于 2026 年 9 月 26 日起在 OpenCode 上免费试用两周。该模型支持 1M 上下文、多模态能力，并承诺零数据留存。目前该消息仅来自单一官方帖子，尚未提供更多技术细节或第三方独立确认。

telegram · zaihuapd · 9月27日 01:41

**「背景」** LongCat 是美团的多模态模型系列；第三方安装指南和对比页面显示，LongCat-2.5-Preview 于 2026 年 9 月 25 日上线美团 LongCat API 平台，提供 100 万 token 上下文、图片输入和可选思考模式，并公布了缓存输入等定价，其输出上限为 131,072 token。此次在 OpenCode 免费试用两周，是该模型在 API 上架后的限时试用安排，而非长期免费计划。

**「影响」** 开发者现在可在 OpenCode 上免费试用 LongCat-2.5-Preview，获得 1M 上下文、多模态支持和零数据留存能力；OpenCode 官方称免费期约两周，但第三方报道称该试用“免费且不限量、未公布截止日期”，因此实际开放时间应以官方页面为准。该模型被描述为面向浏览器等长时 agent 场景，若需评估长上下文工作负载，可借此机会直接测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ahmetbalaman.com/en/blog/how-to-install-longcat-2-5-preview-en/">How to Install LongCat 2 . 5 Preview (Guide)</a></li>
<li><a href="https://www.orcarouter.ai/blog/longcat-2-5-preview-vs-minimax-m3">LongCat - 2 . 5 - Preview vs MiniMax M3: identical rate cards</a></li>
<li><a href="https://x.com/opencode/status/2103841640171614322">OpenCode on X: &quot;LongCat-2.5-Preview is now free on OpenCode for two weeks - 1M Context - Multi-modal - Zero Data Retention&quot; / X</a></li>
<li><a href="https://huggingnews.com/ai/update-opencode-makes-meituan-16t-parameter-longcat-25-free-for-2-weeks-85004eb5">OpenCode Makes Meituan 1.6T Parameter LongCat 2.5 Free for 2 Weeks | HuggingNews</a></li>
<li><a href="https://www.orcarouter.ai/blog/longcat-2-5-preview-free-opencode">LongCat-2.5-Preview free on OpenCode: 1M tokens, no end date</a></li>

</ul>
</details>

**标签**: `#AI models`, `#multimodal`, `#long context`, `#Meituan`, `#OpenCode`

---

<a id="item-tech-news-12"></a>
### [OpenAI 计划扩大 Ultrafast API 访问范围](https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/) ⭐️ 6.0/10

据第三方消息源 TestingCatalog 报道，OpenAI 准备在 9 月 29 日 DevDay 前后扩大 Ultrafast API 的开放范围。该模式随 GPT-5.6 Sol 预览推出，输出速度最高可达 750 tokens/秒，据称推理速度比 Standard 模式快 14 倍，但目前仅限受邀客户使用。开发者未来或可在 Playground 中选择 Standard、Fast、Ultrafast 三档，GPT-6 是否支持尚待确认。需要注意的是，这些细节尚未获得官方证实，且原始信源为聚合平台。

telegram · zaihuapd · 9月27日 02:06

**「背景」** OpenAI 于 2026 年 8 月 13 日随 GPT-5.6 Sol 预览推出了 Ultrafast API 模式，该模式输出速度最高可达 750 token/秒，推理速度比 Standard 快 14 倍，最初仅限受邀客户使用。当前报道的扩大开放范围计划正是基于这一已发布的预览版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.progressiverobot.com/2026/09/26/openai-ultrafast-api-playground-speed-selector/">Ultrafast API: OpenAI&#x27;s Quick, Powerful Playground Upgrade</a></li>
<li><a href="https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/">OpenAI prepares to expand Ultrafast API to more users</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#API`, `#performance`, `#GPT`, `#AI infrastructure`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [10 年期美债收益率升至 5.23%，为 2007 年以来最高](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 8.0/10

10 年期美国国债收益率周五升至 5.23%，为 2007 年以来最高；此前本月早些时候还在 4.8%下方。驱动因素包括通胀黏性、市场预期的美联储加息，以及政府和企业为人工智能基础设施大规模发债带来的供给压力。

rss · CNBC Finance · 9月26日 13:30

**「背景」** 债券收益率与价格反向变动。密歇根大学 9 月一年期通胀预期升至 4.6%，高于 8 月的 4%；芝商所 FedWatch 工具显示，市场认为美联储 10 月加息概率为 64%。

**「影响」** 收益率上升会推高抵押贷款等借贷成本，也可能让债券相对股票更具吸引力，从而对股市构成压力。

**标签**: `#Treasury yields`, `#Federal Reserve`, `#bond issuance`, `#inflation`, `#AI investment`

---

<a id="item-finance-news-2"></a>
### [苹果因 Apple Pay 收费面临美国反垄断集体诉讼](https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/) ⭐️ 7.0/10

美国联邦法官认证了一起针对苹果的反垄断集体诉讼：发行支持 Apple Pay 卡片的发卡机构指控，苹果对信用卡交易按 0.15%、对借记卡交易按 0.5 美分收费，并称这些费用每年最高可达 10 亿美元，而安卓手机钱包不向发卡机构收费。原告要求退还费用并申请禁令，但这些数字目前只是原告指控，并非法院最终认定的事实。

telegram · zaihuapd · 9月26日 03:32

**「背景」** 苹果的移动支付服务 Apple Pay 每笔交易会向发卡机构收取费用（信用卡 0.15%、借记卡 0.5 美分），而安卓手机上的钱包通常不向发卡机构收费；美国一位联邦法官近日认证了由发卡机构提起的反垄断集体诉讼，该诉讼指控苹果滥用 iPhone 的 NFC 芯片控制权，阻止竞争对手开发与 Apple Pay 竞争的钱包并收取过高费用。

**「影响」** 若原告最终胜诉，美国相关发卡机构可能获得费用退还，苹果对 Apple Pay 的收费做法也可能被禁止；目前诉讼仍处于集体诉讼认证后的早期阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://macdailynews.com/2026/09/25/federal-judge-certifies-class-in-apple-pay-fee-antitrust-case-brought-by-credit-union/">Federal judge certifies class in Apple Pay fee antitrust case brought...</a></li>
<li><a href="https://www.macrumors.com/2026/09/25/apple-pay-antitrust-lawsuit-advances/">Banks and Credit Unions to Team Up Against Apple Pay Fees</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Apple Pay`, `#antitrust`, `#class action`, `#payment fees`

---

<a id="item-finance-news-3"></a>
### [中行万事达卡被指疑似遭境外盗刷 用户紧急锁卡](https://finance.sina.com.cn/jryx/2026-09-26/doc-initcyza0450311.shtml) ⭐️ 7.0/10

9 月 26 日，多名用户在社交媒体反映，中国银行万事达卡疑似遭大规模境外盗刷：有用户半夜收到 Apple Pay 主卡失效通知、卡片被锁并出现一笔巴西账单，实体卡从未带出使用。据用户称，信息泄露以英镑卡较多，也有美元卡；目前仅为用户指控，尚未见银行官方确认。

telegram · zaihuapd · 9月26日 12:27

**「背景」** 用户怀疑事件与发卡行发卡逻辑和万事网联（万事达卡在华清算机构）的鉴权问题有关。去年 9 月，浦发银行万事达卡也曾发生类似事件，同样涉及 Apple Pay 绑卡和巴西等拉美货币。

**标签**: `#Bank of China`, `#Mastercard fraud`, `#cybersecurity`, `#card security`, `#China`

---

