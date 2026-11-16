---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 65 条内容中筛选出 25 条重要资讯。

---

**科技新闻**
1. [现代大语言模型位置嵌入方法解析](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta FAIR 与 NYU 训练 200+ 多模态模型：预训练可选，专用视觉参数不可少](#item-tech-news-2) ⭐️ 8.0/10
3. [MacBook Pro OLED PWM 调光闪烁问题分析](#item-tech-news-3) ⭐️ 7.0/10
4. [微软 365 中断致酒店 15 人氯气中毒](#item-tech-news-4) ⭐️ 7.0/10
5. [观点：所有 AI 生成代码都应开源](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Meetings 测试：加入 Google Meet 边听边写方案画白板](#item-tech-news-6) ⭐️ 7.0/10
7. [免训练梯度引导离散扩散序列设计](#item-tech-news-7) ⭐️ 7.0/10
8. [B300 上 cudaMemcpy 可分页传输提速 5 倍](#item-tech-news-8) ⭐️ 7.0/10
9. [FAA 全国停飞起因：换铜线升级引发路由故障](#item-tech-news-9) ⭐️ 7.0/10
10. [鲁比奥与 Anthropic 疑为黄仁勋风波推手](#item-tech-news-10) ⭐️ 7.0/10
11. [美团开源 LongCat-2.5：未用英伟达 GPU 训练](#item-tech-news-11) ⭐️ 7.0/10
12. [Emacs 作为浏览器：个人工作流与社区讨论](#item-tech-news-12) ⭐️ 6.0/10
13. [训练无关早停：把线性探针折入&lt;/think&gt;输出行](#item-tech-news-13) ⭐️ 6.0/10
14. [特斯拉 Cybercab 月租 299 美元订阅协议](#item-tech-news-14) ⭐️ 6.0/10
15. [华为云 MaaS 上线开源盘古模型 openPangu-2.1-Pro](#item-tech-news-15) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache 发布 nightly ROCm 构建](#item-ai-projects-1) ⭐️ 6.0/10
2. [LMCache nightly-rbln 预发布版本](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache nightly 发布：CUDA 13.0 Linux wheel 自动构建](#item-ai-projects-3) ⭐️ 5.0/10

**财经新闻**
1. [卢特尼克因英伟达间谍担忧面临质询，其子经营公司与英伟达有关联](#item-finance-news-1) ⭐️ 7.0/10
2. [美法官驳回美光、三星、SK 海力士 DRAM 价格操纵案撤诉动议](#item-finance-news-2) ⭐️ 7.0/10

**推特新闻**
1. [Paul Graham 澄清令人困惑的创业建议列表](#item-twitter-news-1) ⭐️ 7.0/10
2. [四个神经元，怎么学会追光](#item-twitter-news-2) ⭐️ 7.0/10
3. [黄仁勋据报考虑重返英伟达 CEO，多方公开支持](#item-twitter-news-3) ⭐️ 7.0/10
4. [@venturetwins 关于 Gemini 4 Carbon /swarm 功能的推文](#item-twitter-news-4) ⭐️ 7.0/10
5. [@paulg 关于福特三发飞机航程的说明](#item-twitter-news-5) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [现代大语言模型位置嵌入方法解析](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 8.0/10

这篇文章详细解释了现代大语言模型如何表示词元位置，涵盖不同位置嵌入方法，并将它们与底层理论联系起来。文章属于技术说明，不涉及新发布或突破性成果。

hackernews · Ahead of AI · 11月15日 12:14 · [社区讨论](https://news.ycombinator.com/item?id=50506376)

**「背景」** 在基于 Transformer 的大语言模型中，自注意力机制本身不区分 token 顺序，因此通常需要显式的位置编码；例如 GPT-2 采用可学习的绝对位置嵌入，在进入第一个 Transformer 块之前把位置向量加到 token 嵌入上，并受限于固定的上下文长度（原始为 1024 个位置）。

**「社区讨论」** 评论者 programjames 认为，要真正理解位置嵌入，需要理解群表示理论；旋转位置嵌入（RoPE）是平移群的表示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://daily.dev/posts/understanding-positional-embeddings-in-modern-llms-415mglzuo">Understanding Positional Embeddings in Modern LLMs</a></li>
<li><a href="https://sebastianraschka.com/blog/">Blog and Notes - Sebastian Raschka, PhD Positional embeddings in modern LLMs: from GPT-2 to RoPE and ... RoPE vs NoPE: Modern LLM Position Encoding (2026 ... No Positional Embeddings (NoPE) | Sebastian Raschka, PhD Sebastian Raschka Explains Positional Embeddings… · AGI Hunt</a></li>

</ul>
</details>

**标签**: `#positional-embeddings`, `#LLMs`, `#transformers`, `#deep-learning`, `#NLP`

---

<a id="item-tech-news-2"></a>
### [Meta FAIR 与 NYU 训练 200+ 多模态模型：预训练可选，专用视觉参数不可少](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR 与纽约大学的研究人员训练了 200 多个多模态 LLM（LLM 也从零训练），用同一数据和匹配的计算预算分别检验视觉编码器的三个捆绑选择。结果显示：单独的编码器预训练最多与从零训练的编码器持平，即使免费预训练也没有带来 VQA 提升；完全没有视觉专用参数的模型在 0.6B 到 6.4B 的各个规模都落后，需要约 3 倍计算才能追平；把零初始化的视觉专用权重作为“in-fusion”分支加入 LLM 前 8 层，与前置编码器性能相当，且首 token 延迟降低约 13%。主要对比使用 Qwen3-1.7B 和 4B 配置、0.4B 视觉容量，并在 16 个 VQA 基准和 12 个语言基准上评估。

reddit · r/MachineLearning · /u/trungh98 · 11月15日 17:38

**「背景」** 当前各家实验室对视觉编码器做法不一：Gemma 4 12B 去掉了编码器，Kimi K3 从零训练编码器，Inkling 2 Small 又恢复了编码器；而已发布模型因数据和计算量不同、很少单独控制编码器预训练，无法回答该问题。一个标准编码器实际上捆绑了三个独立选择——单独预训练、仅视觉 token 使用的参数、以及放在 LLM 之前的位置。该研究将这三个选择拆开分别测试。

**「影响」** 对多模态 LLM 设计者而言，可以在匹配计算预算下跳过视觉编码器的单独预训练，但必须保留仅视觉 token 使用的专用参数；将这类参数作为零初始化的 in-fusion 分支放进 LLM 前 8 层，可在不损失 VQA 的情况下降低约 13% 的首 token 时间。

**标签**: `#multimodal learning`, `#vision encoders`, `#model pretraining`, `#empirical study`, `#MLLMs`

---

<a id="item-tech-news-3"></a>
### [MacBook Pro OLED PWM 调光闪烁问题分析](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

MacAnorak 发布的技术分析指出，MacBook Pro OLED 显示屏采用 PWM 调光，可能引发部分用户的闪烁敏感和不适；文章未给出已证实的统一调光频率，具体数值在评论中存在争议。

hackernews · MacAnorak · 11月15日 13:15 · [社区讨论](https://news.ycombinator.com/item?id=50506719)

**「背景」** OLED 屏幕常采用 PWM（脉冲宽度调制）调光，通过快速开关光源来控制亮度；低频率闪烁可能引起部分用户头痛或眼疲劳。此前 Horizon 10 月 28 日摘要曾报道，Apple 计划发布首款触屏 MacBook Pro，配备 OLED XDR 显示屏和 Dynamic Island，起售价约 2,899 美元；当前讨论针对的正是该 OLED 面板的 PWM 行为。

**「影响」** 对 PWM 闪烁敏感的用户在选购 MacBook Pro OLED 版时，需注意可能的不适风险，实际体验前难以仅凭文章确定安全频率。

**「社区讨论」** legitronics 质疑文章提到的 240Hz，认为串联 OLED 双面板以 480Hz 反向 PWM 可等效为 960Hz；另有评论描述了个人因屏幕或灯光闪烁而头痛、恶心等经历。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=uVtylIuB_zQ">Thank you, Xiaomi! No More OLED PWM Headaches... - YouTube</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-27/apple-14-inch-16-inch-macbook-pro-touch-price-is-likely-2-899-laptop-details">2026-10-28 — Apple Reported to Launch Touchscreen MacBook Pro From $2,899</a></li>

</ul>
</details>

**标签**: `#hardware`, `#display`, `#pwm`, `#macbook`, `#flicker`

---

<a id="item-tech-news-4"></a>
### [微软 365 中断致酒店 15 人氯气中毒](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

德国 Phantasialand 酒店发生氯气泄漏，15 名客人受伤。运营方告诉 WDR，由于微软 365 服务中断，维护安全系统发出的电子邮件报警未被收到，因此自动加氯系统泵入过多氯气无人知晓。不过，多位技术人员指出，根本问题在于将安全警报完全依赖云邮件，而非微软故障本身。

hackernews · DeepLogin · 11月15日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=50509411)

**「背景」** Horizon 在 2026-11-14 的日报中曾报道，微软 Outlook、Teams 和 Copilot 于 11 月 13 日发生全球中断，持续超过 12 小时，导致邮件服务不可用。根据 WDR 报道，布吕尔 Phantasialand 的 Hotel Ling Bao 泳池自动加药系统存在缺陷并过量加氯，其维护安全系统本应通过 Outlook 邮件发出警报，但因该中断未被接收，造成 15 名客人受伤。

**「影响」** 对使用自动加氯系统的酒店和水疗设施，此事件表明仅靠云邮件作为安全警报通道会导致现场无人知晓危险。相关运营方应考虑增加本地声光报警或冗余传感器等独立于云服务的机制。

**「社区讨论」** Hacker News 评论大多认为责任在酒店的设计而非微软；用户 amluto 自称运营高级闭环氯化系统，指出此类系统容易在测量低氯或零氯时失效并过量加氯，因此必须有真人或完全不同的传感器设计作为后备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsforum.com/news/outlook-outage-blocked-phantasialand-pool-alerts-before-chlorine-incident-injured-15.452435/">Outlook Outage Blocked Phantasialand Pool Alerts Before ...</a></li>
<li><a href="https://www.reuters.com/technology/microsoft-365-outlook-down-thousands-us-users-downdetector-shows-2026-11-12/">2026-11-14 — Microsoft Outlook, Teams, Copilot Global Outage Exceeds 12 Hours</a></li>

</ul>
</details>

**标签**: `#safety-critical-systems`, `#cloud-dependency`, `#incident-report`, `#system-design`, `#microsoft-365`

---

<a id="item-tech-news-5"></a>
### [观点：所有 AI 生成代码都应开源](https://jakub.jankiewicz.org/blog/ai-code-open-source/) ⭐️ 7.0/10

这是一篇观点文章，主张所有 AI 生成代码应当开源，但并未提出具体法律修改或已实施的技术方案。文章作者认为 AI 生成代码在版权归属上应受到开源要求的约束；评论区则引用美国版权局指引，指出现有法律即可处理 AI 辅助作品的版权问题，AI 辅助创作不一定导致输出无法获得版权保护。

hackernews · jcubic · 11月15日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=50507303)

**「背景」** 软件版权保护取决于作品中是否存在足够的人类创作贡献，而开源是一种许可选择，与作品进入公有领域不是同一概念。讨论中提到的美国版权局指引强调，使用 AI 辅助而非替代人类创作并不自动影响版权保护资格，这为争论提供了关键的法律背景。

**「影响」** 开发者不应默认 AI 生成代码可以自由复制或必须开源：当前该主张没有强制力，且根据评论中引用的版权局指引，含有充分人类指导的 AI 辅助代码仍可能受版权保护。

**「社区讨论」** 评论区出现对立观点：一方认为 AI 只是像编译器一样的工具，人类的工程指导和产品决策应使代码继续受版权保护；另一方报告自己的 AGPL 开源代码曾被模型几乎逐字输出，还遇到公司先侵权后又用大语言模型克隆其系统的经历，反映出训练数据来源与许可证执行之间的紧张关系。

**标签**: `#AI`, `#open source`, `#copyright`, `#software licensing`, `#policy`

---

<a id="item-tech-news-6"></a>
### [Claude Meetings 测试：加入 Google Meet 边听边写方案画白板](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Claude%E8%83%BD%E8%BF%9B%E8%A7%86%E9%A2%91%E4%BC%9A%E8%AE%AE%E4%BA%86%EF%BC%81%E8%BE%B9%E5%90%AC%E8%BE%B9%E5%86%99%E6%96%B9%E6%A1%88%EF%BC%8C%E7%99%BD%E6%9D%BF%E5%BD%93%E5%9C%BA%E7%94%BB) ⭐️ 7.0/10

Anthropic 于 11 月 12 日宣布 Claude Meetings 进入测试，团队可以把 Claude 直接拉进 Google Meet，让它在会议进行中整理讨论、起草方案并更新白板。该功能目前为测试性质，来源未披露正式上线时间和完整的支持范围。

rss · 新智元 · 11月15日 08:35

**「背景」** Horizon 11 月 13 日的日报曾报道，Anthropic 已推出 Claude Meetings 测试版，Claude 以参会者身份加入 Google Meet，负责会议纪要、回答问题、起草文档和画白板，并逐步向 Team 和 Enterprise 套餐开放，当时仅支持 Google Meet。Horizon 11 月 11 日的日报还报道过 Anthropic 发布 Claude Whiteboards、Sheets 和 Data，允许用户在 Claude 内部创建与编辑白板、表格和仪表盘；会议中的白板功能延续了这类实时协作能力。当前文章进一步展示了在“客户活动筹备”会议中，Claude 将讨论实时整理成结构化文档并辅助现场修改的过程。

**「影响」** 对于使用 Google Meet 的团队，Claude 可以在会议进行中把口头讨论转为结构化文档和白板内容，减少会后补记和确认的工作；但当前仅为测试功能，正式可用性尚未公布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/dotey/status/2120979951599931793">2026-11-13 — Claude Meetings 测试版：Claude 加入 Google Meet 会议</a></li>
<li><a href="https://claude.com/resources/articles/sheets-whiteboards-data">2026-11-11 — Anthropic Introduces Claude Whiteboards, Sheets, and Data</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#Anthropic`, `#video conferencing`, `#productivity`

---

<a id="item-tech-news-7"></a>
### [免训练梯度引导离散扩散序列设计](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+NeurIPS%2726%EF%BD%9C%E6%97%A0%E9%9C%80%E8%AE%AD%E7%BB%83%2B%E6%A2%AF%E5%BA%A6%EF%BC%9A%E5%BC%95%E5%AF%BC%E7%A6%BB%E6%95%A3%E6%89%A9%E6%95%A3%E6%A8%A1%E5%9E%8B%E8%AE%BE%E8%AE%A1DNA/%E8%9B%8B%E7%99%BD%E8%B4%A8) ⭐️ 7.0/10

新智元报道的一篇发表于 NeurIPS 2026 的工作提出 D-DOIT，一种针对掩码离散扩散模型的免训练、免奖励梯度推理时采样器，通过 Doob h-变换将冻结模型适配到任意黑盒奖励。论文报告在 HepG2 增强子设计上，高预算 D-DOIT-Q 预测活性为 6.19，超过需要微调的 DRAKES（5.61）；在蛋白质逆折叠上，结构–稳定性联合成功率为 68.1%，高于免微调的 SMC（63.6%）和 TDS（62.9%）。代码和项目主页已公开，论文预印本为 arXiv:2610.04938。

rss · 新智元 · 11月15日 05:50

**「背景」** 掩码离散扩散从全掩码序列开始逐步揭示每个位置的碱基或氨基酸，天然适合 DNA、蛋白质等有限字母表数据；但将预训练模型引向特定任务奖励通常需要微调、可微奖励或高成本粒子/搜索过程，而许多生物学奖励（如 Enformer、结构打分）是黑盒，难以反传梯度。

**「影响」** 研究人员可在不修改模型参数、不获取奖励梯度的条件下，仅通过推理阶段修改采样规则，将冻结的离散扩散模型用于增强子设计、蛋白质逆折叠等黑盒奖励任务；公开代码（github.com/WeiminWu2000/D-DOIT）便于复现与进一步验证。

**标签**: `#discrete diffusion models`, `#protein design`, `#DNA synthesis`, `#generative models`, `#bioinformatics`

---

<a id="item-tech-news-8"></a>
### [B300 上 cudaMemcpy 可分页传输提速 5 倍](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

一位开发者发布了开源工具 cudamemcpy-tuner，用于加速 cudaMemcpy 的可分页（pageable）传输。在 B300 GPU 上，该工具将 1GB 张量从 CPU 复制到 GPU 的带宽从作者基准测试中的 10.2 GB/s 提升到 51.5 GB/s，约为 5 倍。工具可通过 \`cmt tune -- python bench.py\` 形式使用，代码公布在 GitHub。该性能数据来自作者自己的测试，尚未经第三方独立验证。

reddit · r/MachineLearning · /u/makneeee · 11月15日 18:20

**「背景」** 在 CUDA 中，当 cudaMemcpy 使用可分页（pageable）主机内存时，通常无法利用直接内存访问，需要额外的中间复制，因此带宽往往低于固定（pinned）内存；本次提交的工具正是针对这种默认的可分页传输进行调优。

**「影响」** 在 B300 上使用 PyTorch 进行 CPU-GPU 数据传输的开发者可以尝试该工具，但需在自己的工作负载上验证，因为提速结果仅基于作者单一基准测试。

**标签**: `#cuda`, `#gpu`, `#performance`, `#machine-learning`, `#data-transfer`

---

<a id="item-tech-news-9"></a>
### [FAA 全国停飞起因：换铜线升级引发路由故障](https://www.theverge.com/transportation/1033898/faa-ground-stop-sean-duffy-faa-copper-wire) ⭐️ 7.0/10

美国交通部长 Sean Duffy 于 11 月 14 日表示，FAA 全国停飞源于一处偏远设施在将老旧铜线换成光纤的例行维护后，新安装的路由器出现问题。该路由器以每 4 到 5 秒逾千次连接请求冲击其他路由器，干扰雷达信号和飞机通信，导致数千航班停飞。目前根因尚不明确，可能是硬件故障、配置错误或承包商 L3Harris 失误；Duffy 呼吁国会追加空管现代化资金。

telegram · zaihuapd · 11月15日 02:10

**「背景」** Horizon 11 月 14 日的摘要曾报道，FAA 因空管通信中断发布全国地面停飞令，事件疑似涉及 L3Harris 运营的电信网络，并有软件更新导致系统重启崩溃的说法。本次报道更新了原因：一处偏远设施将老旧铜线更换为光纤后，新装路由器异常，并以高频率连接请求冲击其他路由器，导致雷达信号和飞机通信受干扰。

**「影响」** 此次故障已导致数千航班停飞，影响旅客和航空公司运营；美国交通部长据此呼吁国会为空管现代化追加资金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247">2026-11-14 — FAA issues nationwide ground stop after communications outage</a></li>

</ul>
</details>

**标签**: `#networking`, `#infrastructure`, `#aviation`, `#outage`, `#routing`

---

<a id="item-tech-news-10"></a>
### [鲁比奥与 Anthropic 疑为黄仁勋风波推手](https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/) ⭐️ 7.0/10

据《华盛顿邮报》11 月 13 日报道，英伟达创始人黄仁勋疑遭一场协调行动：他此前借与特朗普私交游说放宽对华芯片出口，并公开批评对华鹰派“是一种耻辱，根本不爱国”，引发国安官员不满；国务卿鲁比奥据称利用 CIA 情报撰写强硬备忘录向总统施压。报道还称，科技圈怀疑 Anthropic 高管向《纽约时报》记者提供了关于新加坡 Megaspeed 公司的最初调查线索，记者和 Anthropic 均未回应；Anthropic 一直游说严格限制对华芯片出口并主张给西方 GPU 加装固件级锁或追踪机制，与黄仁勋反对芯片追踪和后门的立场直接冲突。受此影响，众议院中国问题特别委员会主席等人正推动在年底重大国防法案中加入三项条款：进一步限制高端 AI 芯片出口、强制芯片内置防走私追踪技术、限制中国获取芯片制造设备。

telegram · zaihuapd · 11月15日 08:08

**「背景」** Horizon 11 月 13 日日报曾转引美联社报道，黄仁勋已辞去 NVIDIA 首席执行官职务；11 月 14 日日报进一步报道，他承认与一名涉嫌中国间谍的女子有染，并同意在 11 月 26 日前赴国会作证。CNBC 分析认为该丑闻增加了美国国会在年底前收紧对华先进芯片出口限制的可能性。

**「国防法案或收紧芯片出口与追踪要求」** 如果这些条款被纳入年底国防法案，英伟达及其他高端 AI 芯片出口商将面临更严格的出口许可审查、强制内置防走私追踪技术，以及对中国获取芯片制造设备的进一步限制。相关议案已出现在参议院版国防法案中，但仍处立法阶段，尚未成为法律。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/13/jensen-huang-nvidia-us-china-relations.html">2026-11-14 — Nvidia CEO&#x27;s resignation amid spy allegations raises risk of tighter U.S.-China tech controls</a></li>
<li><a href="https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f">2026-11-13 — Jensen Huang Resigns as NVIDIA CEO</a></li>
<li><a href="https://www.zerohedge.com/ai/who-whacked-jensen-huang-cia-wasnt-convinced-so-rubio-reworked-their-memo">Who Whacked Jensen Huang ? The CIA... | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#export controls`, `#Nvidia`, `#Anthropic`, `#semiconductors`

---

<a id="item-tech-news-11"></a>
### [美团开源 LongCat-2.5：未用英伟达 GPU 训练](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 7.0/10

美团旗下的 LongCat 团队开源了 LongCat-2.5 的权重：该模型总参数约 1.6 万亿、每个 token 激活约 480 亿，支持文本、图像和视频输入，以 MIT 许可证发布且可商用。官方称训练全程使用华为升腾加速卡而非英伟达 GPU；在 Terminal Bench v2.1 上得分为 88.4，略低于 Claude Opus 5 的 89.1，这是目前公开的主要基准结果。

telegram · zaihuapd · 11月15日 11:08

**「背景」** 2026 年 11 月 2 日的日报曾报道，LongCat-2.5 作为 1.6 万亿总参数（约 480 亿激活参数）的原生多模态模型发布，面向长时程智能体任务，当时已提供试用和 API。更早的 LongCat-2.0 也声称在约 5 万卡的中国国产芯片集群上训练，未使用英伟达 GPU，因此本次公布的权重和 MIT 许可证是对该系列非英伟达训练路线的延续。

**「影响」** 开发者和企业现在可以下载权重并在 MIT 许可下商用；其宣称的华为升腾训练路线为无法获得英伟达 GPU 的团队提供了一个可参考的替代方案，但基准表现目前仅由 Terminal Bench v2.1 单一结果支撑，需在实际任务中进一步验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://longcat.ai/blog/longcat-2.5/">2026-11-02 — LongCat-2.5: 1.6T-Parameter Native Multimodal Model Released</a></li>
<li><a href="https://braindetox.kr/en/posts/longcat_2_open_model_2026.html">LongCat - 2 .0: A 1.6-Trillion-Parameter Open Model Trained Without ...</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#large language models`, `#AI agents`, `#non-Nvidia hardware`, `#coding models`

---

<a id="item-tech-news-12"></a>
### [Emacs 作为浏览器：个人工作流与社区讨论](https://joshblais.com/blog/emacs-as-my-browser/) ⭐️ 6.0/10

一篇个人博客介绍了在 Emacs 内浏览网页的工作流，使用 eww 并配合 follow-mode 的列布局技巧以增加同屏文本量。作者和评论者指出，静态 HTML、博客和 Wikipedia 等页面体验尚可，但 Reddit 及多数现代商业网站通常无法正常使用。社区还提到 xwidget 嵌入式 WebKit 和 w3m-mode 的标签与会话管理可作为替代或补充。

hackernews · nyc111 · 11月15日 15:21 · [社区讨论](https://news.ycombinator.com/item?id=50507553)

**「背景」** 在 Emacs 中浏览网页通常依赖 eww 或 w3m-mode 等文本模式工具，它们能渲染静态 HTML 并保留键盘操作，但对现代复杂 Web 应用支持有限。Joshua Blais 的这篇博文在此基础上展示了个人配置和取舍。

**「影响」** 对于想尝试这一工作流的用户，应预期现代商业网站兼容性差；若需更完整的浏览功能，可评估 xwidget 嵌入式 WebKit，或在资源受限设备上使用 w3m-mode 获得标签与会话管理。

**「社区讨论」** 评论区中，有用户认为现代商业网站与该工作流不兼容，既可能是限制也可能是特性；另有用户指出，真正需要的是内容寻址的 HTTP\(S\) 替代层，单纯复古浏览器设置无法解决更根本的协议采用问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://joshblais.com/blog/emacs-as-my-browser/">Emacs is my browser - The Universe of Joshua Blais</a></li>

</ul>
</details>

**标签**: `#emacs`, `#web-browsing`, `#productivity`, `#open-source`, `#text-mode`

---

<a id="item-tech-news-13"></a>
### [训练无关早停：把线性探针折入&lt;/think&gt;输出行](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 6.0/10

作者在 Reddit 上描述了一种无需训练和额外推理代码的推理模型早停方法：对 24 道数学题记录隐藏状态，用线性判别分析得到区分“仍在求解”和“已得出答案但反复检查”的方向，并将该方向乘以强度 14 加到输出层 &lt;/think&gt; 标记所在行。修改后的模型是普通权重文件；作者称在 Qwen3.5-4B 的 8 道未见 MATH-500 题上准确率不变且 token 减少 54%，在 3 道 AIME 2025 题中从原模型 32k token 超限全部未完成变为编辑模型解出 2 道，DeepSeek V4.1 Flash 上数学题 7/7 对 6/7 且 token 减少 40%。但这些结果是极小样本、每个设置单次运行，探针仅用数学样本拟合。

reddit · r/MachineLearning · /u/Good-Presentation-23 · 11月15日 17:52

**「背景」** 推理模型在最终回答前会在草稿中“思考”，并以特殊标记 &lt;/think&gt; 结束；输出层为每个词表 token 存一行权重，某 token 的得分等于该行与当前隐藏状态的内积。因此修改 &lt;/think&gt; 这一行的权重可以直接改变模型决定停止思考的概率，而不需要运行额外分类器或修改推理代码。

**「影响」** 使用该方法的 GGUF 权重已发布在 Hugging Face，作者称可在 llama.cpp 中直接运行；对同类数学题或可用它减少约一半推理 token 且不损失小样本准确率，但探针只在数学数据上拟合，其他任务存在过早停止的风险。

**标签**: `#reasoning-models`, `#early-exit`, `#llm-inference`, `#weight-editing`, `#machine-learning`

---

<a id="item-tech-news-14"></a>
### [特斯拉 Cybercab 月租 299 美元订阅协议](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 6.0/10

特斯拉已发布 Cybercab 订阅协议：消费者需先以 29,990 美元购车，并每月支付 299 美元订阅费，否则车辆无法运行；特斯拉可提前一个月通知调整价格。欠费或违规使用可能导致订阅被暂停或取消，累计三次警告则自动驾驶功能停用一周，且车辆只能在指定区域行驶，未经授权不得接入网约车、配送或租赁平台。Electrek 指出，Cybercab 与 Robotaxi 版 Model Y 均采用 AI4 硬件并运行相同的自动驾驶软件，但面向普通车主的 FSD 仍需人类监督。

telegram · zaihuapd · 11月15日 01:10

**「背景」** Horizon 10 月 23 日的日报曾报道，特斯拉在第三季度财报电话会上称将在年底前开始向客户销售 Cybercab，但当时的产量优先分配给自有 Robotaxi 车队，且无监督 FSD 已延至明年第二季度；该报道还提到这款无方向盘双座车正接受 NHTSA 安全标准调查。在此之前，购车后是否需要持续订阅以及使用限制并未披露，本次订阅协议条款补上了这些条件。

**「影响」** 潜在买家需将每月 299 美元订阅作为长期固定成本，且一旦欠费或违反区域/平台限制，可能失去车辆运行或自动驾驶能力，购车前须评估其使用范围和合规风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/10/21/tesla-says-it-will-start-selling-cybercabs-by-end-of-year/">2026-10-23 — Tesla says Cybercab sales start by end of year; FSD slips to Q2</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#autonomous vehicles`, `#subscription pricing`, `#AI4 hardware`, `#robotaxi`

---

<a id="item-tech-news-15"></a>
### [华为云 MaaS 上线开源盘古模型 openPangu-2.1-Pro](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 6.0/10

华为云 MaaS 模型即服务平台于 11 月 15 日正式上线开源盘古模型 openPangu-2.1-Pro，官方称其基于 10 万余条专项数据优化 Agent 的 Skills 触发与工具调用，并重点适配鸿蒙 ArkTS 开发、升腾算子生成，接入智果 AgentArts、码道 CodeArts、果办 OfficeAce 等产品。该模型在 MaaS 平台按量计费：推理输入 0.8 元/百万 tokens，推理输出 3.2 元/百万 tokens，缓存命中输入 0.016 元/百万 tokens。公告未披露基准测试或与上一版本的对比数据。

telegram · zaihuapd · 11月15日 16:03

**「背景」** 华为云的模型即服务（MaaS）平台以 API 形式对外提供大模型调用能力，而开源模型通常公开权重、允许用户自行部署或微调。此次华为云将 openPangu-2.1-Pro 上线该平台并同时公布输入、输出和缓存命中三级 token 价格，说明这一开源盘古模型以托管 API 方式开放调用。

**「影响」** 使用华为云 MaaS 的开发者可立即调用该开源模型进行 Agent 开发和 AI 编码，并按上述 token 价格付费；对鸿蒙 ArkTS 和升腾算子的重点适配意味着其优化更偏向华为自研软件与硬件栈。

**标签**: `#AI`, `#large language model`, `#Huawei Cloud`, `#open source`, `#MaaS`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache 发布 nightly ROCm 构建](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 6.0/10

LMCache 发布面向 AMD Instinct GPU 的 nightly ROCm 7.2 预编译 wheel，支持 gfx942 与 gfx950，ABI 与上游 vLLM ROCm 镜像匹配，可直接在 vLLM 容器中安装使用。

github · github-actions\[bot\] · 11月15日 07:46

**「解决的痛点」** AMD Instinct 用户此前在 ROCm 环境安装 LMCache 常需自行编译或面临 Python ABI 不匹配问题。该构建提供与 vLLM ROCm 容器（torch 2.13, cp312）匹配的二进制 wheel，简化部署，降低 AMD GPU 上使用 LMCache 的门槛，避免手动编译和依赖冲突。

**「背景与影响」** LMCache 是一个 LLM 推理的 KV 缓存管理层，能够将 KV 缓存从临时状态转为可复用知识，从而降低首 token 延迟并提高吞吐量（tool-1-1, tool-1-2）。该 nightly-rocm 版本是针对 AMD Instinct GPU 的每日自动构建，提供 ROCm 7.2 环境的 wheel 包，支持 MI300X/MI325X（gfx942）和 MI350X/MI355X（gfx950），并与上游 vLLM ROCm 容器 ABI 匹配。这使得 AMD GPU 用户可以在 vLLM ROCm 容器中安装 LMCache，扩展了 LMCache 的硬件平台覆盖。该版本本身不包含新的功能特性或架构突破，属于常规的自动化构建发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#ROCm`, `#AMD`, `#LLM`, `#inference`, `#nightly-build`

---

<a id="item-ai-projects-2"></a>
### [LMCache nightly-rbln 预发布版本](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

LMCache 为 Rebellions RBLN NPU 发布的每日开发版预构建轮子，提供 KV 缓存管理，基于 torch-rbln 0.12.0（torch 2.13.0+cpu）。

github · github-actions\[bot\] · 11月15日 07:35

**「解决的痛点」** 提供与 RBLN NPU 软件栈（torch-rbln、rebel-compiler）兼容的预编译安装包，避免用户在专用加速器环境中从源码构建 LMCache，降低部署复杂度，使 KV 缓存优化可以更便捷地应用于 RBLN NPU 上的 LLM 推理。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV 缓存管理项目，用于减少显存占用和提高吞吐。随着 Rebellions RBLN NPU 等专用 AI 加速器生态发展，需要持续集成的每日构建来跟踪 dev 分支的最新改动。此 nightly 轮子让 RBLN NPU 用户能提前测试 LMCache 开发版功能，但本版本未描述架构性突破或新优化。

**标签**: `#LMCache`, `#nightly-release`, `#RBLN-NPU`, `#KV-cache`

---

<a id="item-ai-projects-3"></a>
### [LMCache nightly 发布：CUDA 13.0 Linux wheel 自动构建](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布 nightly 版本，提供基于 dev 分支构建的 CUDA 13.0 Linux amd64/arm64 预编译 wheel，便于用户通过 pip 安装最新开发版。

github · github-actions\[bot\] · 11月15日 09:32

**「解决的痛点」** 解决用户在 CUDA 13.0 环境下缺乏现成编译包的问题，避免从源码手动构建 LMCache 扩展，简化 Linux amd64/arm64 上的安装流程。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV 缓存管理项目；nightly 构建让用户提前使用 dev 分支的最新改动。该发布属于自动化持续集成产物，未提供功能或性能细节。

**标签**: `#llm`, `#kv-cache`, `#cuda`, `#nightly`, `#inference`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [卢特尼克因英伟达间谍担忧面临质询，其子经营公司与英伟达有关联](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

美国商务部长霍华德·卢特尼克因英伟达相关间谍担忧及其前公司关联受到质询。据 CNBC 对证券申报文件的分析，坎托·菲茨杰拉德报告的英伟达持股数量在 2025 年 9 月至 2026 年 3 月间下降近 50%，从逾 350 万股降至 178 万股。

rss · CNBC Finance · 11月15日 19:58

**「背景」** 此前，白宫和美国情报官员曾敦促卢特尼克打击涉嫌向中国转运英伟达先进 AI 芯片的新加坡公司 Megaspeed，但 Axios 报道称卢特尼克多次抵制；其子布兰登和凯尔目前管理坎托·菲茨杰拉德。

**标签**: `#Nvidia`, `#Howard Lutnick`, `#Cantor Fitzgerald`, `#export controls`, `#conflict of interest`

---

<a id="item-finance-news-2"></a>
### [美法官驳回美光、三星、SK 海力士 DRAM 价格操纵案撤诉动议](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

美国法官 Noël Wise 驳回美光、三星和 SK 海力士要求撤销 DRAM 价格操纵集体诉讼的动议，认为原告举出的证据使这三家公司在一年内四次同步限制供应、价格最多上涨 500% 的共谋指控具有合理性。

telegram · zaihuapd · 11月15日 16:39

**「背景」** 这是针对美光、三星和 SK 海力士的 DRAM 价格操纵集体诉讼；原告指控三家公司自 2022 年起四次同步限制供应，导致 DRAM 价格最高上涨 500%。11 月 14 日，加州北区联邦地区法官 Noël Wise 驳回被告的撤诉动议，认为原告已合理主张违反《谢尔曼法》第 1 条的共谋，案件将继续推进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techpowerup.com/354863/samsung-sk-hynix-and-micron-fail-to-get-dram-antitrust-suit-dismissed">Samsung, SK hynix, and Micron Fail to Get DRAM Antitrust Suit ...</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#price fixing`, `#antitrust`, `#semiconductors`, `#litigation`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Paul Graham 澄清令人困惑的创业建议列表](https://x.com/paulg/status/2122108050584592765) ⭐️ 7.0/10

Paul Graham 在回复 @romanbuildsaas 和 @ycombinator 时表示，他自己也对列表中的部分内容感到困惑。他认为“避免大交易”和“远离大公司”是同一个观点：初期最好卖给创业公司，尽管它们资金较少，但决策快。所谓“谋杀”应为“自杀”，即更多创业公司是因执行不力而失败，而非被竞争对手杀死；但他也强调不应完全忽视竞争对手，只是应该更关注用户。此外，他也不理解“大多数公司不会因为没钱而死”这句话的含义。

twitter · Paul Graham · 11月15日 23:22

**「背景」** 这条推文是 Paul Graham 对 @romanbuildsaas 转述其 2009 年文章《Startups in 13 Sentences》中若干建议的澄清。@romanbuildsaas 提到在 YC 录取后重读这些建议，并贴出清单；YC 官方 Library 也收录了 Paul Graham 的多篇随笔。Graham 在回应中解释了自己对其中部分条目也感到困惑，说明“避免大交易”和“远离大公司”其实是同一点：创业初期通常卖给初创公司更好，尽管初创公司钱少，但决策快；将“谋杀”更正为“自杀”，指更多创业公司死于执行不力而非被竞争对手杀死，但不应完全忽略竞争对手，只是应更多关注用户而非竞争者；并对“大多数公司不是因没钱而死”这一条表示完全不理解。该推文当前没有社区评论数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ycombinator.com/library/carousel/Essays+by+Paul+Graham">Essays by Paul Graham - YC Library | Y Combinator</a></li>
<li><a href="https://x.com/romanbuildsaas/status/2069492465338548714">Paul Graham published “Startups in 13 sentences” back in 2009 ...</a></li>
<li><a href="https://paulgraham.com/13sentences.html">Startups in 13 Sentences - Paul Graham</a></li>

</ul>
</details>

**标签**: `#startup advice`, `#Paul Graham`, `#Y Combinator`, `#entrepreneurship`

---

<a id="item-twitter-news-2"></a>
### [四个神经元，怎么学会追光](https://x.com/dotey/status/2122106906814935475) ⭐️ 7.0/10

这条推文介绍了一个教育性演示：Myriad 系列第二章《Watch a Brain Learn》由科学记者 Aatish Bhatia 与神经科学家 Arkarup Banerjee 制作，模拟一个只有四个神经元的小生物如何学会追光。推文用原文数据重绘动画，说明三个数字决定它怕光、冲撞还是爱上光；把三个数字映射为立方体后，学习过程变成立方体中的一条路径。它不依赖直接指令，只靠奖励与惩罚，从两千多种连接方式中找到不到 2% 的好方案。改变奖励后，它还能学会逃跑、装死和战斗，最后回到鸣禽、AI 和人类大脑的讨论。推文将神经科学与机器学习联系起来，属于对已有工作的科普总结，而非原创研究。

twitter · 宝玉 · 11月15日 23:18

**「背景与社区讨论」** 这条推文是宝玉对 Myriad 系列第二章《Watch a Brain Learn》的科普总结：一个只有四个神经元的虚拟生物，如何只靠奖励和惩罚学会追光等行为。该交互文章由神经科学家 Arkarup Banerjee 和物理学家出身的科学记者 Aatish Bhatia 合作完成，发表于 Myriad。\[tool-1-1\]\[tool-1-2\] 项目借鉴了 Valentino Braitenberg 1984 年《合成心理学》的思路，展示吸引力、恐惧、攻击和偏好等复杂行为可以从四个神经元的连接方式中自下而上涌现，而非来自隐藏机制。\[tool-1-2\] 在 Hacker News 上，该文章以“强化学习的可视化解释”被讨论，获得 17 点。\[tool-1-3\]

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aatishb.com/myriad/how-brains-learn/">Watch a Brain Learn - aatishb.com</a></li>
<li><a href="https://news.lavx.hu/article/four-neurons-four-behaviors-how-a-virtual-spark-reveals-the-roots-of-intelligence">Four Neurons, Four Behaviors: How a Virtual Spark Reveals the ...</a></li>
<li><a href="https://zeli.app/story/50496885">Watch a four-neuron brain teach itself · Hacker News | Zeli</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#machine-learning`, `#educational`, `#simulation`, `#AI`

---

<a id="item-twitter-news-3"></a>
### [黄仁勋据报考虑重返英伟达 CEO，多方公开支持](https://x.com/dotey/status/2122062085807030716) ⭐️ 7.0/10

英国《金融时报》11 月 15 日报道，黄仁勋正在考虑重新出任英伟达 CEO，并已与多名亲信讨论回归可能。此前 11 月 12 日，英伟达宣布黄仁勋辞去 CEO 和董事职务，由 CFO Colette Kress 任临时 CEO；报道称董事会对其独立调查尚未结束。

支持者正在行动：黄仁勋的一名未具名盟友称正召集硅谷高管组成“作战室”，游说董事会让其复职并争取白宫支持。网上公开信“Stand with Jensen”要求董事会在调查期间先让其回归、公布调查范围和时间表，截至 11 月 14 日上午已有超 10 万人签名，其中 5000 多人自称英伟达在职员工，马斯克、Tim Sweeney、Garry Tan、Amjad Masad 等也在名单上。Altimeter Capital 的 Brad Gerstner 和 Atreides Management 的 Gavin Baker 则公开致信董事会，希望谨慎处理交接，并把黄仁勋回归留作选项，但未要求立即复职。

twitter · 宝玉 · 11月15日 20:20

**「背景」** 该推文引用英国《金融时报》报道称黄仁勋在辞去英伟达 CEO 后正考虑回归。此前相关背景如下：根据检索到的 Horizon 存档摘要，11 月 13 日已出现黄仁勋辞职的报道；CNBC 后续报道提到其辞职涉及与一名被指为中国间谍的人士存在婚外情，并称他同意在 11 月 26 日前到国会作证，分析师认为该事件可能促使美国在年内收紧对华先进芯片出口限制。另据 CNBC 报道，美国商务部长卢特尼克因 Cantor Fitzgerald 与英伟达的关系面临伦理质疑，该公司报道的英伟达持股数量在 2025 年 9 月至 2026 年 3 月间下降 49%。社区评论部分目前没有提供内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f">2026-11-13 — Jensen Huang Resigns as NVIDIA CEO</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html">2026-11-14 — Lutnick faces ethics questions over Cantor Fitzgerald&#x27;s Nvidia ties after Huang resignation</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/jensen-huang-nvidia-us-china-relations.html">2026-11-14 — Nvidia CEO&#x27;s resignation amid spy allegations raises risk of tighter U.S.-China tech controls</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Jensen Huang`, `#AI industry`, `#leadership`, `#news`

---

<a id="item-twitter-news-4"></a>
### [@venturetwins 关于 Gemini 4 Carbon /swarm 功能的推文](https://x.com/venturetwins/status/2122043781507948954) ⭐️ 7.0/10

Justine Moore 于 2026 年 11 月 15 日发布推文，称 Gemini 4 Carbon 的 /swarm 功能被低估。她请求生成旧金山渡轮大厦的 3D 模型，该功能协调了 12 个并行代理进行研究、规划、编写 Blender Python 脚本，并在共享留言板上互相评审工作。推文认为这是多代理编排的高价值演示，但缺乏深层技术细节或可验证的新颖性。

twitter · Justine Moore · 11月15日 19:07

**「背景」** 2026 年 11 月 15 日，Justine Moore 发推称 Gemini 4 Carbon 的 /swarm 功能被低估。她要求生成渡轮大厦（Ferry Building）的 3D 模型，该功能协调了 12 个并行智能体，分别进行研究、规划、编写 Blender Python 脚本，并在共享留言板上相互评审。这一演示提供了多智能体编排的具体案例。背景：谷歌于 2026 年 11 月 11 日发布 Gemini 4 Carbon，强调其面向长周期智能体工作流，并随 Antigravity 推出 /swarm 功能（tool-1-2）。该模型被定位为面向编码、智能体与复杂推理的前沿模型，支持多模态输入与长输出（tool-1-3）。网络视频也展示了 Gemini 4 Swarm 的自主运行能力（tool-1-1）。截至抓取时间，原帖暂无可用社区评论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=Sc6TriRAGnI">Gemini 4 Swarm is out of control... - YouTube</a></li>
<li><a href="https://agihunt.info/en/e/1a1c635d7ef6f674fcbda38ded0">Google launches Gemini 4 Carbon , its strongest… · AGI Hunt</a></li>
<li><a href="https://openrouter.ai/google/gemini-4-carbon">Gemini 4 Carbon - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#multi-agent`, `#AI`, `#3D modeling`, `#Blender`

---

<a id="item-twitter-news-5"></a>
### [@paulg 关于福特三发飞机航程的说明](https://x.com/paulg/status/2122080094264995922) ⭐️ 6.0/10

Paul Graham 表示，杰克逊维尔到萨凡纳（125 英里）大约是他们所驾驶的福特三发飞机有效航程的一半，因此他们最多只能减少大约一半的停靠次数，不可能更多。

twitter · Paul Graham · 11月15日 21:31

**「背景」** 保罗·格雷厄姆在回复中解释，杰克逊维尔至萨凡纳的航线距离约 125 英里，大约是当时所飞福特三发机（Ford Trimotor）有效航程的一半。这意味着即便减少经停，最多也只能砍掉约一半的站点。福特三发机是美国三发动机运输机，1926 年 6 月 11 日首飞，早期多用于客运航线；其 4-AT-E 型号的技术参数可见 Holcomb&\#x27;s Aerodrome 的资料，军事工厂网站则提供了其开发与运营历史。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ford_Trimotor">Ford Trimotor - Wikipedia</a></li>
<li><a href="https://www.airminded.net/ford3m/ford3m.html">Ford Tri-Motor - Holcomb&#x27;s Aerodrome</a></li>
<li><a href="https://www.militaryfactory.com/aircraft/detail.php?aircraft_id=1374">Ford Trimotor Transport Aircraft / Passenger Airliner</a></li>

</ul>
</details>

**标签**: `#aviation`, `#history`, `#Ford Trimotor`, `#fact-check`

---