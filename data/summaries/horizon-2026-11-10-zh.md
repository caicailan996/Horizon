# Horizon 每日速递 - 2026-11-10

> 从 83 条内容中筛选出 34 条重要资讯。

---

**科技新闻**
1. [E-means：同等损失下快 10 倍的 k-means 变体](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta 发布最小最高效模型 Muse Ember](#item-tech-news-2) ⭐️ 8.0/10
3. [Anthropic 发布 Claude Fable 5.2 与 Mythos 5.2](#item-tech-news-3) ⭐️ 8.0/10
4. [LingBot-Touch：潜变量预测胜过重建，用于灵巧操作触觉预训练](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Gemini 消费者版个人文件或送人工标注](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Fable 5.2 获 65 分但单任务成本翻倍](#item-tech-news-6) ⭐️ 7.0/10
7. [加拿大推出 Real-Time Rail 实时支付系统](#item-tech-news-7) ⭐️ 7.0/10
8. [Watched.earth 查询一周内拍过某地的卫星及真实影像](#item-tech-news-8) ⭐️ 7.0/10
9. [Atlas 话题页新增 2026 顶会论文基准](#item-tech-news-9) ⭐️ 7.0/10
10. [SwarmEvolve 用潜在智能体群加速数学发现与优化](#item-tech-news-10) ⭐️ 7.0/10
11. [Twindex：可重放证明数据无法区分两组参数的精确证书](#item-tech-news-11) ⭐️ 7.0/10
12. [剑桥团队 AI 设计禽流感候选疫苗，动物试验显示广谱保护](#item-tech-news-12) ⭐️ 7.0/10
13. [谷歌发布 TPU 8tx 与 8i Max 芯片](#item-tech-news-13) ⭐️ 7.0/10
14. [USPS 发布官方 ZIP 编码边界多边形](#item-tech-news-14) ⭐️ 6.0/10
15. [Opus 5.5 被暗中削弱？11 月 3 日变化引争议](#item-tech-news-15) ⭐️ 6.0/10
16. [Simon Willison 用 Claude Code 构建开源蜂鸣定位系统](#item-tech-news-16) ⭐️ 6.0/10
17. [用 &lt;details&gt;&lt;summary&gt; 折叠 AI 生成的 PR 描述](#item-tech-news-17) ⭐️ 6.0/10
18. [Git 拟投票决定 LLM 贡献政策](#item-tech-news-18) ⭐️ 6.0/10
19. [清华开源 OpenMise：两阶段空间编辑减少视频抽卡](#item-tech-news-19) ⭐️ 6.0/10
20. [XGBoost 县级新停电预报：PR-AUC 为 NWS/SPC 基准 2.4 倍](#item-tech-news-20) ⭐️ 6.0/10
21. [彭博：Siri AI 负责人罗克韦尔或明年离职](#item-tech-news-21) ⭐️ 6.0/10
22. [比亚迪闪充机械臂阿联酋首秀：1000kW 自动充电](#item-tech-news-22) ⭐️ 6.0/10
23. [OPPO、vivo、小米、荣耀上线 ADV 开发者验证机制](#item-tech-news-23) ⭐️ 6.0/10
24. [欧盟数字公平法草案限制成瘾设计](#item-tech-news-24) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 ROCm 7.2 夜间版 wheel](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache nightly-rbln：面向 Rebellions RBLN NPU 的每夜构建 wheel](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache 发布 nightly-cu129 轮子](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache 每夜构建版本发布](#item-ai-projects-4) ⭐️ 5.0/10

**财经新闻**
1. [中国继续暂停对美 24%加征关税，保留 10%税率](#item-finance-news-1) ⭐️ 8.0/10

**推特新闻**
1. [OpenAI 推出 Control Room 集中安全系统](#item-twitter-news-1) ⭐️ 8.0/10
2. [Deedy 分享 Fable 5.2 生成照片级蜂蜜 WebGL 模拟](#item-twitter-news-2) ⭐️ 7.0/10
3. [OpenAI dot 新增多电脑连接：可为每个任务指定运行电脑](#item-twitter-news-3) ⭐️ 7.0/10
4. [Fable 5.2：智能提升 10%，成本增加 164%](#item-twitter-news-4) ⭐️ 6.0/10
5. [Ryan Hoover 宣布 AI 智能体现在可以与 Product Hunt 对话](#item-twitter-news-5) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [E-means：同等损失下快 10 倍的 k-means 变体](https://e-means.github.io/) ⭐️ 8.0/10

E-means 项目公布了一种 k-means 变体，宣称在相同聚类损失下只需更少迭代，可将收敛速度提高约 10 倍。社区评论中，有用户报告在 GPU 上用于 IVF 索引时获得 146 倍加速，另一用户则表示将其用于球面等面积网格松弛后并未改善。这些数字来自项目页面宣称和评论者自述，尚未看到独立基准验证。

hackernews · porridgeraisin · 11月9日 18:45 · [社区讨论](https://news.ycombinator.com/item?id=50429734)

**「背景：Lloyd 算法与 e-means 的定位」** 该项目页面说明 e-means 由 Meta FAIR 开发并开源，其对比基线是标准 k-means（通常采用 Lloyd 算法）。Lloyd 算法通过交替进行样本分配和质心更新来收敛，在处理大规模数据时的主要成本来自多轮全量扫描。

**「影响」** 对使用 k-means 做大规模聚类或 IVF 索引的开发者，如果这些社区结果成立，可用更少的数据遍历获得同等损失，从而缩短训练或索引时间；但收益可能依赖数据集规模和访问模式，一名用户在球面网格松弛场景中未观察到改善。

**「社区讨论」** 评论中出现了对照经验：一名用户称其用于球面等面积网格松弛后“肯定没有更好”，而另一名用户称在 IVF 索引的 GPU 实现中获得 146 倍加速。还有评论推测该更新规则可理解为带摩擦项并保持质心在凸包内的期望最大化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://e-means.github.io/">e - means : 10 x faster k - means at equal loss - Blog</a></li>

</ul>
</details>

**标签**: `#clustering`, `#k-means`, `#algorithm-optimization`, `#machine-learning`, `#performance`

---

<a id="item-tech-news-2"></a>
### [Meta 发布最小最高效模型 Muse Ember](https://research.meta.ai/blog/muse-ember) ⭐️ 8.0/10

Meta 发布了 Muse Ember，定位为其最小、最高效的模型，面向复杂推理和智能体任务，支持 100 万 token 上下文窗口，并可处理文本、图像、音频和视频及调用工具。定价为每百万输入 token 0.10 美元、缓存输入 0.004 美元、输出 0.50 美元；社区评论指出该模型未开放权重，最佳智能体基准结果来自 mini-swe-agent 而非 Meta 自有评测套件。

hackernews · dvaplima · 11月9日 17:58 · [社区讨论](https://news.ycombinator.com/item?id=50429024)

**「Muse 系列前作」** Meta 此前已在 Muse 系列中发布过多个模型：Horizon 的 10 月 13 日摘要曾报道 Muse Wonder 多模态模型发布，早期社区测试结果不一；10 月 16 日的摘要报道了 816B 总参数、42B 活跃参数的 Muse Spark Open 开放权重模型。Muse Ember 现在被定位为该系列中最小、最高效的型号，对比这些前作有助于理解其相对定位。

**「影响」** 对需要低成本多模态智能体能力的开发者，Muse Ember 提供了较低的 token 价格和长上下文选项，但社区未找到开放权重，自行部署或微调受限。

**「社区讨论」** 评论中，doodlesdev 指出该模型的最佳基准来自 mini-swe-agent 而非 Meta 自有评测套件；simonw 报告在六个思考级别测试中，更多推理 token 并未让生成的 SVG 明显更好，打破了以往推理量与图像质量的关联。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/muse-wonder">2026-10-13 — Meta AI unveils Muse Wonder multimodal model with mixed early tests</a></li>
<li><a href="https://research.meta.ai/blog/muse-spark-open">2026-10-16 — Meta launches Muse Spark Open, an 816B-parameter open-weight model</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#large language models`, `#model release`, `#meta`, `#agentic AI`

---

<a id="item-tech-news-3"></a>
### [Anthropic 发布 Claude Fable 5.2 与 Mythos 5.2](https://www.anthropic.com/claude-fable-and-mythos-5-2) ⭐️ 8.0/10

Anthropic 宣布推出 Claude Fable 5.2 和 Mythos 5.2，称其具备先进多智能体推理与形式化定理证明能力。公司宣称，1,000 个 Fable 5.2 智能体以最少人工干预在 30 小时内完成费马大定理的形式化，而此前未发布研究版本耗时 11 天。该表述为厂商声明，相关基准和性能尚未经独立验证。

hackernews · meetpateltech · 11月9日 18:56 · [社区讨论](https://news.ycombinator.com/item?id=50429906)

**「背景」** Horizon 10 月 17 日的日报曾报道，Claude Mythos 5 已被用于设计更高效的量子电路，显示该系列面向高难度技术任务。本次费马大定理形式化的对比基准，是此前一个未发布的 Claude 研究模型在人类引导下花费 11 天完成的形式化。

**「影响」** 有用户报告，在普通编码任务中 Fable 5.2 与 Opus 5.5 差异不明显，只有提高提示目标复杂度后才显现优势；因此现有 Opus 5.5 用户未必需要立即迁移，应结合具体工作负载评估。

**「社区讨论」** 讨论中，有用户怀疑 Opus 5.5 被削弱以为新版让路；另有用户批评基准对比选择不合理，例如将 Fable xHigh 与 Carbon Med 对比，且未将定位为网络模型的 Carbon 放入唯一网络基准，认为厂商对比存在选择性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2111152183240511640">2026-10-17 — Anthropic: Claude Mythos 5 Designs More Efficient Quantum Circuits</a></li>
<li><a href="https://aiweekly.co/alerts/anthropics-1000-fable-52-agents-formalize-fermat-in-30-hours">Anthropic&#x27;s 1,000 Fable 5.2 Agents Formalize Fermat in 30 ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#multi-agent-systems`, `#theorem-proving`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [LingBot-Touch：潜变量预测胜过重建，用于灵巧操作触觉预训练](https://www.reddit.com/r/MachineLearning/comments/1xs05uo/latent_prediction_beats_reconstruction_for/) ⭐️ 8.0/10

新论文提出 LingBot-Touch，一个 JEPA 风格的自监督触觉编码器：它预测被遮蔽接触区域的潜在表示，而不是重建原始传感器信号；推理代码和检查点已公开。在相同数据上与同规模 MAE、VAE 重建模型对比，触觉到视频 top-5 召回在 1K 小时为 32.1%（JEPA）对 5.6%（MAE）和 4.4%（VAE）；4K 小时时 JEPA 达 49.3%，MAE 仍低于 9%，VAE 降至 3.1%。Tiny 模型在约 4K 小时后达到平台，Small 仍持续改善。

reddit · r/MachineLearning · /u/Zealousideal-War7154 · 11月9日 18:52

**「背景」** 常见的触觉自监督预训练采用 MAE 或 VAE 等重建原始传感器信号；但触觉片段中大部分是接近零的背景，因此重建损失可能在未学到实际接触信息的情况下下降。LingBot-Touch 的 JEPA 风格训练改为预测被遮蔽接触区域的潜在表示，以避免对稀疏原始信号的重建。

**「影响」** 在 26 个真实机器人任务、4 种策略的 104 个组合中，冻结编码器特征有 89 个组合得分最高；在预训练未见的磁传感器手上，LingBot-VLA 从 57.21 提高到 75.04。研究者可直接用公开检查点复现，作为下游灵巧操作任务的触觉特征基线。

**标签**: `#self-supervised learning`, `#tactile sensing`, `#robotics`, `#representation learning`, `#JEPA`

---

<a id="item-tech-news-5"></a>
### [Google Gemini 消费者版个人文件或送人工标注](https://github.com/thisisme6598/gemini_files/) ⭐️ 7.0/10

消费者版 Google Gemini 在开启“Connected Apps”后，个人 Drive 文件和 Gmail 邮件可能被作为工具加载的数据，并像其他 Gemini 数据一样进入人工标注或审查流程。该说法来自 Hacker News 用户的政策解读与经验描述，并非 Google 的官方产品变更公告。评论同时指出，Workspace 版 Gemini 及 Workspace Intelligence 仍声称不进行人工审查。

hackernews · gf74918 · 11月9日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=50429426)

**「背景」** 2023 年，谷歌曾承诺消费者版 Gemini 中来自 Gmail、Google Docs 和 Drive 的个人内容“不会被人工审核”。但根据“Documentation of Gemini File Leaking Behavior”GitHub 项目及谷歌更新后的帮助文档，2026 年 10 月 16 日对 2023 年博客帖子的编辑显示：当消费者版 Gemini 启用 Connected Apps 时，个人 Gmail 和 Drive 内容可被路由到人工审核管道，推翻了此前的承诺。

**「影响」** 使用消费者版 Gemini 并授权 Gmail/Drive 的用户，其邮件和文件内容可能暴露给第三方人工审核员；注重隐私的用户应避免在个人账户启用 Connected Apps，或切换到声称不进行人工审查的 Workspace 方案。

**「社区讨论」** 多位评论者认为这不是孤立问题：rustyhancock 描述 Gemini 的回答与自己的邮件内容异常吻合，却没有说明读取了邮件；hek2sch 指出所有带人工审核的 Gemini 和 NotebookLM 工具都存在数据被随机人员阅读或用于训练的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://daily.dev/posts/google-gemini-routes-personal-drive-files-and-emails-to-human-annotators-1yiwwc2e8">Google Gemini routes personal Drive files and emails to...</a></li>
<li><a href="https://aiweekly.co/alerts/google-gemini-routes-personal-drive-gmail-to-human-reviewers">Google Gemini Routes Personal Drive, Gmail to Human Reviewers</a></li>

</ul>
</details>

**标签**: `#privacy`, `#google-gemini`, `#ai-ethics`, `#human-annotation`, `#data-practices`

---

<a id="item-tech-news-6"></a>
### [Claude Fable 5.2 获 65 分但单任务成本翻倍](https://artificialanalysis.ai/models/claude-fable-5-2) ⭐️ 7.0/10

Anthropic 的 Claude Fable 5.2 在 Artificial Analysis 上取得 65 分，是当前最高分。根据社区评论，尽管有降价，Fable 5.2 的单任务成本比 5.1 翻倍，输出 token 从约 11.8 万（4.6 万回答/7.1 万推理）增至约 27.4 万（8.1 万回答/19.2 万推理）。

hackernews · theanonymousone · 11月9日 20:04 · [社区讨论](https://news.ycombinator.com/item?id=50431144)

**「背景」** Horizon 的 2026 年 10 月 24 日日报曾报道，Kimi K3.1 Pro 在 Artificial Analysis 上获得 55 分，已超过 Claude Fable 5.1 的 53 分；10 月 30 日的日报则提到由 Fable 5/5.1 驱动的 Spawn 每月 token 成本超过 300 万美元。此次 Fable 5.2 在同一评测中进一步变化，评论区指出其输出 token 数从 5.1 的约 118k 增至 274k，成本对比成为焦点。

**「影响」** 对使用该模型的开发者而言，即使单价下降，实际单任务 API 成本因 token 量增加而显著上升，需重新评估预算或选择更低推理量的配置。

**「社区讨论」** 评论者 rgbrenner 指出 Fable 5.2 的输出 token 数翻倍导致成本激增；brachkow 认为与 DeepSeek-Flash 相比价格高出约 100 倍而性能仅提升几个百分点。oliwary 则补充，低、中配版本在“每任务时间—智能”帕累托前沿上有所改善。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Oct/23/kimi-k31-pro/">2026-10-24 — Kimi K3.1 Pro 上线 API，承诺 11 月 4 日开放权重</a></li>
<li><a href="https://simonwillison.net/2026/Oct/29/how-i-built-the-most-ai-pilled-company-in-the-world/">2026-10-30 — Spawn uses autonomous Fable agents to ship prompt-driven game changes hourly</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#benchmark`, `#cost-efficiency`, `#Anthropic`

---

<a id="item-tech-news-7"></a>
### [加拿大推出 Real-Time Rail 实时支付系统](https://www.payments.ca/canada-launches-real-time-rail-bringing-247-payment-infrastructure-national-economy) ⭐️ 7.0/10

Payments Canada 宣布加拿大 Real-Time Rail（RTR）支付系统已上线，提供 7×24 小时实时支付基础设施。社区评论中引用的初始活跃参与者包括 Wealthsimple、Questbank、Peoples Trust、Paramount Commerce、KOHO、DoBusiness.com、Digital Commerce Bank 和 Bank of America，名单中未包含加拿大主要银行。

hackernews · ocd · 11月9日 16:00 · [社区讨论](https://news.ycombinator.com/item?id=50427362)

**「背景」** 此前加拿大的即时个人转账主要依赖 Interac 的 e-Transfer，这是一个银行共同拥有的专有系统；有评论认为本次发布像是把 Interac 的能力作为公共基础设施向更多机构开放。另外，社区评论指出初始参与名单中未包含加拿大主要大型银行，首批参与者包括 Wealthsimple、KOHO、Peoples Trust 等机构。

**「影响」** 由于初始参与方以金融科技公司和较小银行为主，加拿大主要银行尚未出现在名单中，普通用户能否使用实时转账取决于其开户机构；这将限制 RTR 初期的覆盖范围。

**「社区讨论」** 有加拿大用户对将 Interac 的 e-Transfer 能力开放为公共基础设施表示谨慎乐观，认为邀请 Interac 作为合作伙伴比绕开它更明智；也有人指出美国 FedNow 虽已推出但覆盖银行少且收费，并质疑加拿大主要银行为何缺席。

**标签**: `#fintech`, `#payments`, `#infrastructure`, `#Canada`, `#banking`

---

<a id="item-tech-news-8"></a>
### [Watched.earth 查询一周内拍过某地的卫星及真实影像](https://www.watched.earth/) ⭐️ 7.0/10

作者发布了一个开源浏览器工具 watched.earth，输入任意地点后，会在浏览器中用约半秒时间基于 CelesTrak 目录的 SGP4 模型计算过去 7 天所有过境卫星，并拉取对应的 Sentinel-2、Landsat 和 NASA 真实影像。该工具在 GPU 上绘制约 1.7 万个在轨物体并逐帧求解开普勒方程，仅在实际存在影像时才显示“watched”，且不存储用户位置。代码托管在 github.com/dev-Armaan/satellites。

hackernews · a585gupt · 11月9日 17:51 · [社区讨论](https://news.ycombinator.com/item?id=50428907)

**「背景」** SGP4 是一种广泛使用的卫星轨道传播模型，CelesTrak 提供公开的卫星轨道根数目录；Sentinel-2 和 Landsat 等卫星影像可通过公开数据接口获取。作者将这两者结合，实现了在浏览器端完成过境计算与影像检索。

**「影响」** 普通用户无需安装或注册即可核查自己所在街区过去 7 天被哪些卫星拍摄，并取回对应的真实影像；开发者可以基于开源代码扩展其他影像数据源。

**「社区讨论」** 有 HN 用户称赞这是“风格与内容的最佳结合”，也有用户指责文本由 LLM 生成且故意小写以伪装人工撰写，另有用户反馈输入位置时光标与字符间距错位，影响使用。

**标签**: `#satellite-imagery`, `#open-source`, `#sgp4`, `#webgl`, `#geospatial`

---

<a id="item-tech-news-9"></a>
### [Atlas 话题页新增 2026 顶会论文基准](https://www.reddit.com/r/MachineLearning/comments/1xs6494/followup_2026_papers_are_finally_in_the_topic/) ⭐️ 7.0/10

Atlas.scime.ai 的机器学习话题页已新增 2026 年 ICML/CVPR/ICLR/AAAI 论文的基准记录与消融结果，从约 101k 篇全文抽取约 100 万条“尝试 X，得到 Y”发现，此前为 79k 篇。ICML、CVPR 和 AAAI 几乎全覆盖，ICLR 覆盖约 4.1k/5.4k 篇，NeurIPS 2026 因多数 PDF 尚未公开只完成过半；示例中 Mip-NeRF 360 PSNR 从 2025 年的 29.5 升至今年的 30.1，Deep Blending 约 30.4 和 Tanks&amp;Temples 未变，但论文报道的 3DGS 基线在同一数据集上为 16 至 27.7 PSNR，差异巨大。作者同时发布 ICML/CVPR/ICLR 2026“报纸”并指出：LLM agents 占 ICML 比例从 1.2% 升至 4.4%，CVPR 多模态 LLM 从 5.4% 翻倍至 10.8%，ICLR 可验证奖励的 RL 从几乎零篇增至 110 篇，Qwen 是三者结果表中最常用的基座模型；作者提醒数字由 AI 抽取、未经人工核对，论文过度报告有效结果，应作为起点而非排行榜。

reddit · r/MachineLearning · /u/latenticlabs · 11月9日 22:39

**「前情」** Horizon 11 月 4 日的日报曾报道，Atlas 发布时整理了 2016 年以来 ICML、NeurIPS、ICLR、CVPR、AAAI 的约 1260 个主题页，并从 79k 篇论文全文中提取结果表和消融数据，但当时基准记录和消融停留在 2025 年。此次更新把提取范围扩大到约 101k 篇全文，补入 2026 年 ICML/CVPR/AAAI 及大部分 ICLR 论文，NeurIPS 2026 因大量 PDF 尚未公开仅覆盖一半多一点。

**「影响与注意事项」** Atlas.scime.ai 的免费话题页无需注册即可访问，但完整版 2026“报纸”需免费账号。对需要可靠对比的研究者，当前 AI 抽取且未人工校验的数据只适合用于发现候选论文与复现起点，关键数字应回归原论文核对，尤其要警惕同一 3DGS 基线报告值从 16 到 27.7 PSNR 造成“击败基线 X dB”比较失真。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xmk8rx/we_turned_10_years_of_ml_papers_into_one_page_per/">2026-11-04 — Atlas research map turns 109k ML papers into benchmark topic pages</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#benchmarking`, `#research tools`, `#computer vision`, `#conference papers`

---

<a id="item-tech-news-10"></a>
### [SwarmEvolve 用潜在智能体群加速数学发现与优化](https://www.reddit.com/r/MachineLearning/comments/1xrunu7/using_latentagent_swarms_for_math_discovery_and/) ⭐️ 7.0/10

SwarmEvolve 提出了一种可扩展的潜在智能体群框架，让数百个基于 Qwen3 8B、14B 和 32B 的小型开源模型智能体共享 KV 缓存，在约 5 分钟内达到 OpenEvolve、ShinkaEvolve 和 CodeEvolve 此前需要 1 小时以上的分数；仅用 8B 模型还追平了已知最佳圆形装填结果。作者称该框架已扩展到 Qwen3.5 与 Muse 模型，表现更好。论文地址为 https://www.alphaxiv.org/abs/2611.08483，代码尚未发布，且速度与性能结果是发布者自述、未经独立验证。

reddit · r/MachineLearning · /u/QileHQ · 11月9日 15:30

**「背景」** 理解 SwarmEvolve 需要先了解进化式程序发现：AlphaEvolve 等系统让大语言模型（LLM）编写候选程序、按任务评分并迭代改进，此前已找到 4×4 复矩阵乘法的更快算法。这类方法通常依赖大型模型或运行较慢；SwarmEvolve 旨在用多个开源小模型组成群体，以 KV 缓存共享实现更快、更便宜的探索。

**「影响」** 对尝试复现或评估该框架的研究者，SwarmEvolve 的关键运行配置是每轮 450 个潜在智能体、分成 10 个 swarm（4 个精化、3 个杂交、2 个探索、1 个重置），但作者尚未发布代码（标注为 available soon）。因此目前只能依据论文和补充视频自行实现，并应以 OpenEvolve、ShinkaEvolve、CodeEvolve 以及 Qwen3 8B/14B/32B 作为对照基线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=mA011Yu-lfc">SwarmEvolve : Latent Agent Swarms for Evolutionary Discovery and...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#latent reasoning`, `#evolutionary algorithms`, `#LLM agents`, `#mathematical optimization`

---

<a id="item-tech-news-11"></a>
### [Twindex：可重放证明数据无法区分两组参数的精确证书](https://www.reddit.com/r/MachineLearning/comments/1xryhhg/twindex_exact_replayable_proofs_that_your_data/) ⭐️ 7.0/10

Twindex 发布了一个可重放、精确的参数可辨识性证书工具（pip install twindex），用于证明两组参数在给定数据下无法被区分。它使用有理算术和标准库 Python 编写的小型检查器生成或验证 JSON 证书，支持包含多项式、除法、exp、sin、cos 的 ODE 模型，以及一维/二维椭圆和热方程 PDE；任意 Python 模拟器只能作为数值审计而非证明。作者在 1978 年英国寄宿学校流感爆发数据上演示：观测 5 天计数后，R0=2.5 与 R0=20 的 SIR 模型都拟合所有计数，而 Twindex 找出了一个次日计数可以区分它们，实际计数则同时排除了两者。工具目前假定有界噪声、证明以用户声明的模型与噪声界为条件，且扩展到多个参数仍有困难，尚无独立专家证明审计。

reddit · r/MachineLearning · /u/Longjumping\_Glass852 · 11月9日 17:50

**「背景」** 现有有界误差估计与验证积分已有成熟工作；Twindex 的新增部分是便携的精确证书和一个任何人都能重放的检查器，这填补了参数估计中“数据无法区分不同参数”的可证明性空白。在 PINN、最小二乘和贝叶斯拟合中，通常只返回一个参数，而未说明是否存在差异很大但同样拟合数据的另一个参数。

**「影响」** 对于使用 Twindex 的科研用户，若得到 VALID 双胞胎对，则在有界噪声假设下，没有估计器能从这些数据中把参数恢复得优于间隙的一半，这意味着应追加实验或收集区分性数据，而不是信任单一拟合值。

**标签**: `#parameter identifiability`, `#scientific machine learning`, `#PINNs`, `#uncertainty quantification`, `#formal verification`

---

<a id="item-tech-news-12"></a>
### [剑桥团队 AI 设计禽流感候选疫苗，动物试验显示广谱保护](https://www.cam.ac.uk/stories/ai-developed-vaccines-against-viruses) ⭐️ 7.0/10

剑桥大学等机构在 2026 年 11 月在线发表于《Cell Reports Medicine》的论文中报告，利用 AI 辅助设计的新型禽流感候选疫苗在小鼠和雪貂试验中显示出广谱免疫与保护效果，优于基于 WHO 候选疫苗病毒的对照制剂。研究团队计划推进人体临床试验，但该候选疫苗尚未证实对人类的保护效果。

telegram · zaihuapd · 11月9日 03:00

**「背景」** 此前禽流感疫苗抗原通常基于 WHO 推荐的候选疫苗病毒制备；这项研究用 AI 辅助设计了一种自然界中不存在的人工广谱抗原，并与基于 WHO 候选疫苗病毒的对照制剂进行了动物试验比较。

**「影响」** 如果后续人体试验成功，该候选疫苗可能为禽流感应急应用提供一种广谱抗原设计；但目前仅限动物模型数据，监管或临床使用仍需等待人体验证。

**标签**: `#AI`, `#vaccine design`, `#avian influenza`, `#computational biology`, `#biotech`

---

<a id="item-tech-news-13"></a>
### [谷歌发布 TPU 8tx 与 8i Max 芯片](https://www.bloomberg.com/news/articles/2026-11-09/google-escalates-nvidia-rivalry-with-new-versions-of-its-tpu-systems) ⭐️ 7.0/10

谷歌宣布推出两款新的张量处理单元：TPU 8tx 面向政府机构及受严格监管行业，用于处理安全机密数据，并将与 AMD 芯片协同工作；TPU 8i Max 针对超长上下文窗口 AI 场景，将两颗 TPU 芯片集成在同一封装内，以提供更强算力和更大内存容量。谷歌称今年已连续扩充 TPU 产品线，试图让 TPU 成为英伟达 GPU 之外的重要选择。不过，报道未披露具体性能、功耗或价格数据。

telegram · zaihuapd · 11月9日 13:36

**「背景」** 在此次发布之前，Horizon 11 月 6 日的日报曾报道谷歌 Ironwood TPU 被定位为英伟达 CUDA 的推理替代方案；10 月 21 日的日报曾报道谷歌开源原生 PyTorch 后端 TorchTPU。这些举措为谷歌扩展 TPU 产品线提供了软件生态基础。

**「影响」** 对政府和受监管行业客户，TPU 8tx 提供了与 AMD 协同的安全计算选项；对需要处理超长上下文的 AI 开发者，TPU 8i Max 提供更大内存和算力。但两款产品均未公布可用时间、性能指标或价格，暂无法评估实际竞争力。

**「社区讨论」** 社区评论中，有用户质疑“再次没有人能用上它”，并追问谷歌为何不直接销售这些芯片；另有用户指出报道缺乏每 token 功耗与成本等数据，难以与英伟达同类产品比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/tpu-strikes-the-king">2026-11-06 — Google Ironwood TPU Positions as CUDA Inference Alternative</a></li>
<li><a href="https://github.com/google-pytorch/torch_tpu">2026-10-21 — Google open-sources TorchTPU, native PyTorch backend for TPUs</a></li>

</ul>
</details>

**标签**: `#Google`, `#TPU`, `#AI hardware`, `#Nvidia`, `#cloud computing`

---

<a id="item-tech-news-14"></a>
### [USPS 发布官方 ZIP 编码边界多边形](https://postalpro.usps.com/zcb) ⭐️ 6.0/10

USPS 已在 postalpro.usps.com/zcb 上线官方 ZIP 编码边界多边形数据，面向需要精确邮编地理边界的 GIS 用户和开发者。社区评论指出最低层级定价约 1 万美元，远高于许多用户预期，且美国人口普查局已免费提供 ZCTA 近似边界文件。该产品是付费数据服务，并非免费开放的联邦数据。

hackernews · munro · 11月9日 19:58 · [社区讨论](https://news.ycombinator.com/item?id=50431058)

**「背景」** ZIP 编码传统上代表邮政投递路线而非严格的地理分区，因此长期以来没有官方多边形边界；此前常用的替代方案是美国人口普查局发布的 ZCTA 文件，它是对邮政编码区域的近似表达。这一背景解释了为何官方边界数据的发布值得关注。

**「影响」** 需要官方邮编边界的组织或个人将面对显著成本，最低层级据社区评论约 1 万美元；对于精度要求不高的场景，免费 ZCTA 文件仍是现成的近似替代，因此不一定需要购买该产品。

**「社区讨论」** 社区评论主要争论两点：一是联邦政府生产的数据是否应免费公开，有用户认为收费违背透明原则；二是用户指出 ZIP 编码本质是路线而非地理分区，官方多边形可能仍是抽象近似，并推荐免费的 ZCTA 文件作为替代。

**标签**: `#geospatial`, `#USPS`, `#open-data`, `#government-data`, `#GIS`

---

<a id="item-tech-news-15"></a>
### [Opus 5.5 被暗中削弱？11 月 3 日变化引争议](https://twitter.com/shanemelaugh/status/2119192075505893695) ⭐️ 6.0/10

目前没有官方信息确认 Opus 5.5 在 11 月 3 日被静默更改，Hacker News 用户只提供了相互矛盾的个人感受。一位用户用 9 月的同一基准、prompt 和设置重跑：流式 128K 上限在前后都是 128,000 tokens、2.56 美元、空文件；Batch API 300K 在 9 月为 255,957 tokens/2.56 美元，今天为 243,707 tokens/2.44 美元。另一位用户称其长期评测未显示变化，还有人猜测是 A/B 测试，整体证据仍属推测。

hackernews · rzk · 11月9日 07:04 · [社区讨论](https://news.ycombinator.com/item?id=50422069)

**「背景：Opus 5.5 的发布与既有输出问题」** Claude Opus 5.5 于 2026 年 9 月 22 日由 Anthropic 发布，定位为处理复杂编程和长时运行代理的最强 Opus 模型。Horizon 9 月 29 日的摘要曾报道，Opus 5.5 在最大思考强度下存在一个已知问题：会消耗 128,000 个 token 却无法生成 SVG；这与本次讨论中用户用 SVG 基准复测的上下文直接相关。

**「影响」** 对依赖 Opus 5.5 的开发者而言，目前无法仅凭社区传闻确认模型行为或成本是否改变；由于报告相互矛盾且缺少官方说明，若要判断输出质量是否变化，应使用固定 prompt 和设置自行重跑基准。

**「社区讨论」** PhunkyPhil 怀疑模型在发布周期和账号新旧上被调参，感觉每次新模型先强后弱；ianberdin 用同一基准重跑后认为“这不是真的”，并给出流式和 Batch API 数据；rzk 则称看起来像是 A/B 测试实验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/28/claude-sonnet-5-5/">2026-09-29 — Claude Sonnet 5.5: faster, cheaper, but max thinking fails</a></li>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5.5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#large-language-models`, `#model-evaluation`, `#developer-tools`, `#software-engineering`

---

<a id="item-tech-news-16"></a>
### [Simon Willison 用 Claude Code 构建开源蜂鸣定位系统](https://simonwillison.net/2026/Nov/9/mysterious-beeps/) ⭐️ 6.0/10

Simon Willison 使用 Claude Code（Opus 5.5，Extra thinking 模式）构建并发布了开源系统 Beep Locator，通过 Python Web 服务器和浏览器 WebAudio/WebSocket 协调多台手机、平板和笔记本，利用声波到达时间差定位家中间歇性蜂鸣声来源。系统用 60 秒音频缓冲、FFT 与高通滤波检测蜂鸣，并以校准啁啾对齐各设备录音；设备间自动测距效果不佳，因此加入了 Rough mode 手动摆放后微调。实际部署后，系统将蜂鸣位置锁定在约 40 厘米范围内，最终在一堆箱子里找到需要更换电池的旧一氧化碳探测器。

rss · Simon Willison · 11月9日 23:57

**「背景」** 这种声源定位方法的学术基础是 2007 年 BeepBeep 论文，提出在商用设备上仅用扬声器、麦克风和设备间通信实现高精度声学测距，核心包括双向传感、自录音和样本计数。Claude 在项目启动时找到并参考了这篇论文。

**「影响」** 该仓库以开源形式提供完整实现，其他有类似间歇性声音定位需求的人可以直接部署使用，并依据设备校准获得接近 40 厘米的实际定位精度；不过自动设备定位不可靠，用户可能需要手动标记大致位置。

**标签**: `#AI-assisted development`, `#audio triangulation`, `#Claude Code`, `#open source`, `#software engineering`

---

<a id="item-tech-news-17"></a>
### [用 &lt;details&gt;&lt;summary&gt; 折叠 AI 生成的 PR 描述](https://simonwillison.net/2026/Nov/9/details-summary/) ⭐️ 6.0/10

Simon Willison 建议开发者在 GitHub Markdown 的 PR 描述中使用 HTML \`&lt;details&gt;&lt;summary&gt;\` 元素，把 AI 编码代理生成的长篇描述折叠起来，只留一个人类审定的简短开头。GitHub 支持这些标签，点击摘要文本可展开完整内容；他常用模型名和 effort 级别（如“Claude Opus 5.5 Medium”）作为 summary。该做法并非 GitHub 新功能，而是作者目前的工作流程，所有信息仍保留但首屏只显示要点。

rss · Simon Willison · 11月9日 04:25

**「背景」** AI 编码代理（如 Claude Code、Codex）为 PR 编写描述时往往过于全面准确，导致阅读负担超过人类撰写者；而 GitHub Markdown 原生支持 \`&lt;details&gt;&lt;summary&gt;\` 折叠语法，但编辑器中没有快捷按钮。

**「影响」** 采用该模板的开发者可以在不丢失代理生成细节的前提下，让评审者先读到一个人类编辑过的短引言，降低信息过载。具体操作是在 PR 正文开头写一段简明概述，再把完整代理描述包在 \`&lt;details&gt;\` 中，用模型名作为 \`&lt;summary&gt;\`；需要手动输入标签，移动端输入体验稍差。

**标签**: `#AI coding agents`, `#pull requests`, `#developer workflow`, `#HTML`, `#software engineering`

---

<a id="item-tech-news-18"></a>
### [Git 拟投票决定 LLM 贡献政策](https://lwn.net/Articles/1104195/) ⭐️ 6.0/10

Git 项目正在考虑引入投票程序，以决定是否接受 LLM 撰写的代码贡献。该议题已在近期的 Git 贡献者峰会上讨论，但目前尚无具体决议。Git 项目历来并非以民主方式治理，此次拟议的投票是为了给讨论找到可接受的结论。

rss · LWN.net · 11月9日 15:05

**「背景」** 2026 年各开发项目围绕 LLM 撰写贡献的接受条件展开广泛辩论，Git 项目也未能置身事外。此前该项目没有正式的投票治理机制，因此引入投票本身就是一个治理层面的变化。

**标签**: `#git`, `#open source`, `#llm`, `#software development`, `#governance`

---

<a id="item-tech-news-19"></a>
### [清华开源 OpenMise：两阶段空间编辑减少视频抽卡](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E8%A7%86%E9%A2%91%E7%94%9F%E6%88%90%E4%B8%8D%E5%86%8D%E5%8F%8D%E5%A4%8D%E6%8A%BD%E5%8D%A1%EF%BC%81%E6%B8%85%E5%8D%8E%E5%BC%80%E6%BA%90%EF%BC%8C%E7%BB%99%E6%A8%A1%E5%9E%8B%E8%A3%85%E4%B8%8A%E3%80%8C%E4%B8%89%E7%BB%B4%E7%A9%BA%E9%97%B4%E5%A4%A7%E8%84%91%E3%80%8D) ⭐️ 6.0/10

清华大学与宾夕法尼亚大学团队开源了 OpenMise，一个面向 Agent 的空间场景编辑工具，项目地址为 github.com/Rath-Team/OpenMise。它把视频生成拆成两阶段：先由 Agent 调用 Blender，在三维世界里排布场景、人物、动作、摄影机和灯光并生成可修改草稿；再把草稿交给现有视频生成模型完成写实或特定风格渲染。团队称该设计针对模型难以同时保证细节一致性和画面质量的缺点，但来源未提供对比基准或量化结果。

rss · 新智元 · 11月9日 04:54

**「背景」** Horizon 在 10 月 24 日的日报中曾报道，字节跳动火山引擎发布了 Seedance 2.5 4K，新增 480P 草稿模式并支持 10-bit 色深，但当时只向部分企业客户开放。本次报道进一步指出，这类 SOTA 视频模型在连续棋局等需要精确空间一致性的场景中仍会出现棋子位置漂移，OpenMise 的两阶段「Builder + Render」方案正是针对这一缺陷。

**「影响」** 视频创作者可以把明确的走位、棋局或镜头要求先变成 Blender 三维草稿，再用既有模型渲染；这有望减少棋子错位、穿墙等一致性问题带来的反复生成和时间、算力消耗。但公开文章未给出量化对比，实际效果仍需自行验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mp.weixin.qq.com/s/yUa8oh-IWfl5lDQzGSKWeg">2026-10-24 — ByteDance Releases Seedance 2.5 4K With 480P Draft Mode</a></li>

</ul>
</details>

**标签**: `#video generation`, `#open source`, `#3D spatial understanding`, `#AI`, `#Tsinghua`

---

<a id="item-tech-news-20"></a>
### [XGBoost 县级新停电预报：PR-AUC 为 NWS/SPC 基准 2.4 倍](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 6.0/10

作者发布了一个县级小时级新停电概率预测模型，覆盖密苏里州和伊利诺伊州 216 个县，预测从未来 2 小时开始的 6 小时内该县至少 5%客户新增停电的概率。模型使用 XGBoost，输入 HRRR 风暴相关变量（阵风、风切变、CAPE、结冰等）、县级特征、当前停电和邻县情况；使用 2020–2024 年训练、2025 年测试，测试采用最后 5 次 HRRR 预报的平均值而非观测天气。在 2025 年留出年份上，模型 PR-AUC 为 0.094，对比 NWS 警告+SPC Day 1 展望基线 0.039，比值约 2.4 倍（bootstrap 95%区间 2.0–3.3）；在相同警报量下，新停电捕获率 30%对 17%，精确率 15%对 11%，基准发生率为 0.5%。项目自 11 月 1 日起已上线并保存每次预报供盲测，代码和泄漏审计已公开。

reddit · r/MachineLearning · /u/CarRepresentative843 · 11月9日 21:34

**「背景」** NWS 天气警报和 SPC Day 1 展望是常见的风暴灾害基准，HRRR 是高分辨率数值天气预报模式。该问题中只有 0.5%的县小时发生新停电，属于极不平衡的罕见事件，因此作者用 PR-AUC 比较模型与基线，而不是以总体准确率为主。此前很多停电预测会奖励识别已经发生的停电；该工作明确只预测新增停电，难度更高。

**「影响」** 对密苏里州和伊利诺伊州的电力或应急部门，模型在同等警报量下能把新停电捕获率从 17%提高到 30%，但 15%的精确率意味着仍有较高误报；在爱荷华、印第安纳和密歇根的初步迁移测试中，捕获率为 31%对 19%，提示可能跨区域扩展，但仍需验证。

**标签**: `#machine learning`, `#time series forecasting`, `#power outage prediction`, `#XGBoost`, `#weather forecasting`

---

<a id="item-tech-news-21"></a>
### [彭博：Siri AI 负责人罗克韦尔或明年离职](https://9to5mac.com/2026/11/08/john-ternus-pushing-craig-federighi-to-move-faster-software-engineering/) ⭐️ 6.0/10

彭博社记者古尔曼在《Power On》通讯中爆料，曾主导 Vision Pro 和新版 Siri AI 的迈克·罗克韦尔仍在认真考虑离开，可能于明年卸任 Siri 工程副总裁甚至离开苹果。若他离职，工作预计交给去年从谷歌加入的阿马尔·苏布拉马尼亚和费德里吉副手塞巴斯蒂安·马里诺；有人看好马里诺接任软件工程主管，但费德里吉尚无接班安排。该消息属于未证实的人事变动传闻。

telegram · zaihuapd · 11月9日 04:33

**「背景」** Horizon 10 月 15 日的日报曾报道，苹果计划于 12 月通过 iOS 27.3 在中国大陆推出 Apple Intelligence，但首发功能不含新版 Siri；罗克韦尔正是负责新版 Siri AI 的工程副总裁，这一背景使他的潜在离职更受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-14/apple-prepares-to-debut-first-ai-features-in-china-in-december">2026-10-15 — Apple Plans December Launch of Apple Intelligence in Mainland China</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Siri`, `#AI`, `#leadership`, `#rumor`

---

<a id="item-tech-news-22"></a>
### [比亚迪闪充机械臂阿联酋首秀：1000kW 自动充电](https://m.mydrivers.com/newsview/1164193.html) ⭐️ 6.0/10

比亚迪在阿联酋首次公开演示了闪充机械臂，可自动完成打开充电口、取枪插枪、充电、拔枪和关闭盖板等操作，车主驶入车位后即可离开。现场展示的充电功率可达 1000 kW；配合第二代刀片电池，官方演示称可 5 分钟快速补能、9 分钟充满。该站点还采用光储充一体化方案，并展示“一键泊充”功能，可让车辆自主驶入车位后由机械臂充电。

telegram · zaihuapd · 11月9日 05:20

**「背景」** 该演示的核心前提是车辆具备可自动开闭的充电口，并支持 1000 kW 级直流快充；比亚迪称其第二代刀片电池可承受这一充电倍率，从而在 5 分钟内完成快速补能。机械臂负责自动完成打开充电口、插枪、充电、拔枪和关闭盖板等操作，使车主无需手动干预。

**「影响」** 该演示说明，若此类站点落地，驾驶者可在车辆自动泊入后离开、由机械臂完成充电，省去手动插枪步骤；但来源未给出正式商用时间，目前仍是现场展示。

**标签**: `#electric vehicles`, `#robotic charging`, `#hardware`, `#energy storage`, `#automation`

---

<a id="item-tech-news-23"></a>
### [OPPO、vivo、小米、荣耀上线 ADV 开发者验证机制](https://mp.weixin.qq.com/s/ZiKBASSLzvsZ6WR2AUmFeg) ⭐️ 6.0/10

OPPO、vivo、小米、荣耀在中国大陆联合上线安卓侧载应用开发者身份验证（ADV），支持各方验证结果互认，为开发者与其应用建立可信关联。已在四家开放平台注册上架的 APP 会自动提交验证，无需单独申请；未完成验证的应用在侧载安装时会弹出“未验证”提示，需用户手动确认方可继续安装。该消息来自移动智能终端生态联盟，目前属于上线公告，未披露具体技术实现细节。

telegram · zaihuapd · 11月9日 11:44

**「背景」** 在中国大陆的 Android 生态中，侧载安装允许用户绕过官方应用商店直接安装 APK，但此类应用通常缺少统一的开发者身份核验，用户难以判断应用来源与安全性。

**「影响」** 对已在四家平台注册上架的开发者而言，验证自动完成，无需额外申请；对用户而言，安装未验证侧载应用时新增手动确认步骤，增加了安全溯源和风险提示环节。

**标签**: `#Android`, `#sideloading`, `#app security`, `#developer verification`, `#China tech`

---

<a id="item-tech-news-24"></a>
### [欧盟数字公平法草案限制成瘾设计](https://www.mlex.com/mlex/articles/2546584/digital-businesses-face-addictive-design-controls-under-draft-eu-consumer-law) ⭐️ 6.0/10

一份泄露的欧盟《数字公平法案》草案显示，欧盟拟要求数字企业允许用户关闭自动播放、连续使用奖励等成瘾性功能；在线订阅须提供取消按钮、续费提醒和人工客服，免费试用转付费前获得明确同意。草案还禁止面向未成年人的付费抽奖、付费获胜和画像广告，并要求游戏虚拟货币标明真实币值。违规企业最高可被罚全球营业额 6%。该草案计划于 11 月 11 日提交，但仍须欧洲议会和欧盟各国政府批准才能生效。

telegram · zaihuapd · 11月9日 16:42

**「背景」** Horizon 11 月 7 日的摘要曾报道，欧盟委员会依据《数字服务法》指控 TikTok 推荐算法造成有害的“兔子洞”效应，要求其调整算法，否则最高可处全球年收入 6% 罚款。此次泄露的《数字公平法案》草案把类似的成瘾性设计限制从平台义务扩展到一般数字企业，并新增订阅取消、免费试用同意及虚拟货币真实币值披露等要求。

**「影响」** 若按草案通过，在欧盟提供数字服务的企业需要改造订阅流程、关闭默认成瘾功能，并重新设计游戏内虚拟货币展示，否则面临最高全球营业额 6%的罚款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/06/eu-charges-tiktok-harmful-algorithmic-rabbit-hole-effects.html">2026-11-07 — EU charges TikTok recommendation algorithm with harmful rabbit-hole effects</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#consumer protection`, `#addictive design`, `#subscription`, `#gaming`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 ROCm 7.2 夜间版 wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

LMCache 发布 ROCm 7.2 夜间版 wheel，针对 AMD Instinct GPU，与上游 vLLM ROCm 镜像 ABI 匹配，可 pip 安装到 vLLM ROCm 容器。

github · github-actions\[bot\] · 11月9日 07:57

**「解决的痛点」** 为 AMD Instinct GPU 用户提供与上游 vLLM ROCm 镜像 ABI 匹配的预编译 wheel，避免从源码编译 ROCm 扩展，解决依赖版本冲突和安装部署复杂的问题。夜间版用于测试 dev 分支最新功能。

**「背景与影响」** LMCache 是 LLM 缓存加速项目，此前主要面向 CUDA。此次发布 ROCm 夜间版，扩展了对 AMD GPU 生态的支持。夜间构建来自 dev 分支，并非稳定版本，但可帮助 AMD Instinct 用户在 vLLM ROCm 环境中提前使用和测试 LMCache 新特性。

**标签**: `#llm-cache`, `#rocm`, `#amd`, `#nightly`, `#vllm`

---

<a id="item-ai-projects-2"></a>
### [LMCache nightly-rbln：面向 Rebellions RBLN NPU 的每夜构建 wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

LMCache 面向 Rebellions RBLN NPU 的每夜自动构建 wheel，基于 dev 分支，使用 torch-rbln 0.12.0（torch 2.13.0+cpu），提供可安装的预编译包。

github · github-actions\[bot\] · 11月9日 07:44

**「解决的痛点」** 解决 RBLN NPU 用户需要手动从源码编译 LMCache 或找不到兼容 wheel 的部署痛点。该 wheel 不捆绑 torch-rbln、rebel-compiler 和 RBLN 驱动，要求环境中已有这些依赖，避免重复打包和版本冲突，同时保持安装包轻量。

**「背景与影响」** 这是 LMCache 的自动化每夜预发布版本，属于常规构建而非重大架构更新。LMCache 是 LLM 推理中的 KV 缓存组件，此次发布将其可用性扩展到 Rebellions RBLN NPU 硬件，进一步补充了非 NVIDIA 加速器的推理部署生态。

**标签**: `#LMCache`, `#LLM`, `#inference`, `#KV cache`, `#nightly`, `#RBLN NPU`

---

<a id="item-ai-projects-3"></a>
### [LMCache 发布 nightly-cu129 轮子](https://github.com/LMCache/LMCache/releases/tag/nightly-cu129) ⭐️ 5.0/10

LMCache 发布 nightly-cu129，提供基于 dev 分支构建的 CUDA 12.9 Python 轮子，支持 linux/amd64 和 linux/arm64 平台。

github · github-actions\[bot\] · 11月9日 12:32

**「解决的痛点」** 为使用 CUDA 12.9 环境的用户提供预编译轮子，避免手动编译和依赖版本不匹配的麻烦；同时让用户能更早试用 dev 分支的最新改动。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV 缓存管理层，可将 KV 缓存从临时状态转化为可跨引擎复用、可观测的 AI 原生知识\[^tool-1-2\]。随着其在开源社区中逐渐成为 LLM 推理 KV 缓存管理的实际标准\[^tool-1-1\]，项目会定期从 dev 分支构建 nightly 版本，供用户提前验证最新开发状态。本次 nightly-cu129 针对 CUDA 12.9 提供 linux/amd64 与 linux/arm64 的预编译 wheel，并通过 uv pip 给出安装命令；对于使用 CUDA 12.9 或希望测试最新开发分支的环境，可免于从源码编译，降低了试用门槛。由于是例行 nightly 构建，发布说明中未包含新特性或显著优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#nightly`, `#CUDA`, `#wheels`, `#LLM caching`

---

<a id="item-ai-projects-4"></a>
### [LMCache 每夜构建版本发布](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布基于 dev 分支的每夜构建版本，提供适用于 Linux amd64 和 arm64 的 CUDA 13.0 预编译 wheel 包。

github · github-actions\[bot\] · 11月9日 09:27

**「解决的痛点」** 降低在 CUDA 13.0 环境下安装 LMCache 的门槛。用户无需从源码编译，可直接通过 pip 预发布渠道安装预构建的 wheel 包，简化部署流程。

**「背景与影响」** LMCache 是一个面向 LLM 推理的模块化 KV Cache 管理层，旨在将 KV Cache 从临时状态变为可跨请求、跨引擎复用和持久化的 AI 原生知识。随着长提示、对话历史与检索内容复用场景增多，它帮助团队在 GPU、CPU 内存和外部后端之间存储、复用、压缩与观测 KV Cache。本次为 routine nightly 构建，仅提供从 dev 分支构建的 CUDA 13.0 Linux（amd64/arm64）wheel，未包含具体架构或性能变更说明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**标签**: `#LLM`, `#inference`, `#caching`, `#nightly`, `#CUDA`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国继续暂停对美 24%加征关税，保留 10%税率](https://mp.weixin.qq.com/s/nNxJB3y0YA_2zJvOK6onUQ) ⭐️ 8.0/10

国务院关税税则委员会宣布，自 2026 年 11 月 10 日 13 时 01 分起，在 2 个月内继续暂停对美 24%加征关税税率，保留 10%加征关税税率。

telegram · zaihuapd · 11月9日 04:03

**「背景」** 此前，国务院关税税则委员会曾在 8 月 12 日宣布，对原产于美国的进口商品在 90 天内暂停实施 24%的加征关税税率、保留 10%的税率；本次是两个月的延续措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/K6PK1HVO0514E1NL.html">中 美 发布联合声明： 24 % 对 等 关 税 暂 停 90天，保留 10 ...</a></li>

</ul>
</details>

**标签**: `#tariffs`, `#US-China trade`, `#trade policy`, `#China`, `#economic policy`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [OpenAI 推出 Control Room 集中安全系统](https://x.com/OpenAI/status/2119913172039868579) ⭐️ 8.0/10

OpenAI 宣布构建了 Control Room，一个用于跟踪研究基础设施中模型工作负载的中央系统，并能在出现安全或安保问题时快速停止。它连接所有研究推理工作负载，包括用于模型训练和评估的智能体采样、数据处理等，并与错位监控系统协同，在做出干预决定后 35 秒内停止模型输出。OpenAI 表示这是其安全前沿模型训练与部署整体方法的一部分。

twitter · OpenAI · 11月9日 22:01

**「背景」** 该公告由 OpenAI 官方账号于 2026 年 11 月 9 日在 X（Twitter）上发布。推文介绍了 Control Room 的功能：集中监控模型推理负载，与错位监控系统配合，实现快速暂停或停止任务。推文未提供更多技术实现细节，也未披露特定事件案例。

**标签**: `#AI safety`, `#OpenAI`, `#infrastructure`, `#model monitoring`

---

<a id="item-twitter-news-2"></a>
### [Deedy 分享 Fable 5.2 生成照片级蜂蜜 WebGL 模拟](https://x.com/deedydas/status/2119930300990177509) ⭐️ 7.0/10

Deedy 在推文中展示了一段演示：Fable 5.2 根据提示词“Can you write the most intricate photorealistic simulation of honey in WebGL in the browser”生成了浏览器中的蜂蜜模拟。Deedy 称该视频完全基于物理的实时渲染，并感叹 Fable 5.2 生成照片级场景的能力令人难以置信。推文发布于 2026 年 11 月 9 日。

twitter · Deedy · 11月9日 23:09

**「背景」** 2026 年 11 月 9 日，Deedy 在推特分享了一段演示：他向 Fable 5.2 提问“你能在浏览器中用 WebGL 编写最复杂逼真的蜂蜜模拟吗”，得到的结果是一段完全基于物理的实时渲染视频。该演示展示了 Fable 5.2 从文本提示生成复杂 WebGL 物理模拟的能力，但推文未提供更多技术细节。Anthropic 官方介绍页（tool-1-1）将 Claude Fable 5.2 列为最新模型之一，并提到其在 RoboDojo Sim 基准上的表现；第三方分析（tool-1-3）也收录了该模型的性能与价格对比。此前，Fable 5 与 5.1 已被用于 Spawn 游戏中由提示驱动的实时代码修改（tool-2-1），此次 WebGL 模拟可视为该系列在生成复杂前端/物理代码方向的延续。社区评论暂无。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://artificialanalysis.ai/models/claude-fable-5-2">Claude Fable 5 . 2 (max) - Intelligence, Performance... | Artificial Analysis</a></li>
<li><a href="https://simonwillison.net/2026/Oct/29/how-i-built-the-most-ai-pilled-company-in-the-world/">2026-10-30 — Spawn uses autonomous Fable agents to ship prompt-driven game changes hourly</a></li>

</ul>
</details>

**标签**: `#AI`, `#Fable`, `#WebGL`, `#simulation`, `#generative AI`

---

<a id="item-twitter-news-3"></a>
### [OpenAI dot 新增多电脑连接：可为每个任务指定运行电脑](https://x.com/dotey/status/2119898580131725439) ⭐️ 7.0/10

OpenAI 的常驻 AI 助理 dot 现已支持同时连接多台个人电脑，用户可以把每个任务指定到某台机器上执行。dot 于 9 月底在 DevDay 发布，住在云端，有自己的云电脑和浏览器，可通过 ChatGPT、Slack、Teams 使用；此前只能连接一台个人电脑，本次更新后可将任务派到专门机器，不占用日常电脑。官方开发者账号给出三个例子：在第二台 Mac 的 Xcode 里测试改动并截图；在笔记本和装有旧版 SDK 的机器上运行同一测试以对比复现 Bug；在第二台电脑上执行整套界面操作并记录出错步骤，同时用户仍可继续使用自己的屏幕和鼠标。在已连接的电脑上，dot 会新建 Codex 或 ChatGPT Work 的本地任务，也可继续该电脑上已有的 Codex 任务，任务在云端统一管理并使用那台电脑上的文件和工具。每个线程一次只用一台电脑；要让多台电脑并行工作，需要为每台电脑开设线程，已开始的任务不会随选中电脑切换而迁移。功能正逐步向 ChatGPT Pro 各档和 Business Premium 用户开放；Pro 用户须年满 18 岁，欧洲经济区、英国、瑞士暂不可用；Enterprise、Edu、Healthcare 需管理员开通，11 月 18 日起默认开启，除非企业选择关闭。连接方法是在目标电脑的 ChatGPT 应用中进入 dot 资料页，在 Computers 下选择 Allow 并确认。连接后需保持电脑联网且 ChatGPT 应用开启；Offline 只表示暂时不可用，彻底断开需 Revoke access。该授权独立于 Codex 和 Work Sync。与 dot 聊天不占用 ChatGPT 用量额度，但它派给 Codex、Work 的任务仍按这两个产品额度计费。与竞品相比，Claude Duet 目前未提连接用户电脑，Grok Bot 则支持在本地电脑执行命令；dot 对屏蔽云服务器的网站，会转而在已连接电脑上另开本地任务。

twitter · 宝玉 · 11月9日 21:03

**「背景」** dot 是 OpenAI 在 2026 年 9 月底 DevDay 上发布的云端常驻 AI 助理，定位为可异步执行任务的 agent：它拥有独立的云电脑和浏览器，即使本地设备关机，也能继续工作；用户可通过 ChatGPT、Slack、Teams 向它派活。此前 dot 已经能连接一台个人电脑，使用该电脑上的文件、代码和软件；本次更新把连接能力扩展到多台，并允许在任务/线程层面指定电脑，适合测试、Bug 复现和 UI 检查等场景。同期，Anthropic 的 Claude Duet 于 10 月 21 日以研究预览版发布，也提供云虚拟机与浏览器，但官方未提及连接用户本地电脑；xAI 的 Grok Bot 则具备类似的本地电脑执行能力。dot 的授权机制与 Codex、Work Sync 分开，连接后也需要目标电脑在线并保持 ChatGPT 应用运行。

**标签**: `#OpenAI`, `#AI assistant`, `#multi-device`, `#developer tools`, `#tech news`

---

<a id="item-twitter-news-4"></a>
### [Fable 5.2：智能提升 10%，成本增加 164%](https://x.com/ding_liam/status/2119922378264436741) ⭐️ 6.0/10

丁洪 Liam 在推特上表示，Fable 5.2 的智能水平提升了 10%，但成本增加了 164%。该推文提供了一个关于模型版本成本效益权衡的简洁数据点，但未包含更深入的解释或背景信息。

twitter · 丁洪Liam · 11月9日 22:37

**「背景与上下文」** Anthropic 近期发布了 Claude Fable 5.2（以及 Claude Mythos 5.2）（tool-1-1）。官方介绍称该模型可用于复杂软件工程任务、机器人控制和长周期项目管理，并能同时协调超过 1,000 个 AI 智能体（tool-1-2）。官方文档页面还列出了模型 ID、上下文窗口、输出限制、定价和可用区域等信息（tool-1-3）。

本次推文的核心是 Fable 5.2 的“智能提升 10%、成本上升 164%”。这属于作者给出的数据点，未说明“智能”如何衡量、与哪个基线版本对比，也未说明成本的计算口径。在提供的官方资料片段中，未直接出现这组 +10% / +164% 数字；因此应视为尚未经官方或独立验证的说法。

社区讨论方面：该推文暂无可用评论。上述官方页面可作为了解 Fable 5.2 发布与基本能力的背景，但不能直接证实推文中的成本/智能对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5.2 and Claude Mythos 5.2 \ Anthropic</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-launches-fable-5-2-193609974.html?fr=sycsrp_catchall">Anthropic launches Fable 5.2 and Mythos 5.2 AI models ahead ...</a></li>
<li><a href="https://platform.claude.com/docs/en/models/fable-5-2/overview">Claude Fable 5.2 - Claude Platform Docs</a></li>

</ul>
</details>

**标签**: `#AI`, `#model release`, `#cost efficiency`

---

<a id="item-twitter-news-5"></a>
### [Ryan Hoover 宣布 AI 智能体现在可以与 Product Hunt 对话](https://x.com/rrhoover/status/2119889958593036340) ⭐️ 6.0/10

Product Hunt 创始人 Ryan Hoover 在推文中宣布，AI 智能体现在可以与 Product Hunt 进行对话。推文内容非常简短，未提供技术细节或具体功能说明，仅表明存在某种集成或 API 发布，允许智能体接入 Product Hunt。

twitter · Ryan Hoover · 11月9日 20:28

**「背景」** 2026 年 11 月 9 日，Ryan Hoover 在 X（Twitter）发文称：“Rad. Now your agent can talk to Product Hunt.”（好极了，现在你的智能体可以跟 Product Hunt 对话了。）这则简短公告暗示 Product Hunt 已向 AI 智能体开放某种交互或集成能力，但原帖未披露技术细节、接口形式或发布时间。Product Hunt 是一个每日精选新科技产品的平台，由 Ryan Hoover 创办 \[tool-1-1\]\[tool-1-2\]。Ryan Hoover 近期在 LinkedIn 的动态中提到，大多数时候 AI 智能体需要有人手动提示才能开始工作 \[tool-1-3\]，这可能与此次宣布的产品方向有关。原帖暂无社区评论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.producthunt.com/">Product Hunt – The best new products in tech.</a></li>
<li><a href="https://www.youtube.com/watch?v=p9XOLBKayhM">Triangulation 188: Product Hunt Founder Ryan Hoover - YouTube</a></li>
<li><a href="https://www.linkedin.com/company/producthunt">Product Hunt | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Product Hunt`, `#integration`, `#announcement`

---

