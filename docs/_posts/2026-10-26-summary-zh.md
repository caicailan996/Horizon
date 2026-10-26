---
layout: default
title: "Horizon Summary: 2026-10-26 (ZH)"
date: 2026-10-26
lang: zh
---

> 从 34 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Brotli 高危漏洞波及 Python 与 Node.js HTTP 组件](#item-tech-news-1) ⭐️ 8.0/10
2. [Cerebras 详解万亿参数模型部署](#item-tech-news-2) ⭐️ 7.0/10
3. [苹果周三发布首款触屏 MacBook Pro](#item-tech-news-3) ⭐️ 7.0/10
4. [10 年前的 CNN 在皮肤癌诊断上胜过前沿 LLM](#item-tech-news-4) ⭐️ 6.0/10
5. [Borcherds 称 AI 使批改作业失去意义](#item-tech-news-5) ⭐️ 6.0/10
6. [Nanbeige 开源 33B 教师模型 Nanbeige4.3-33B](#item-tech-news-6) ⭐️ 6.0/10
7. [memt-1.0 记忆原生架构：门控 DeltaNet-2 与混合存储](#item-tech-news-7) ⭐️ 6.0/10

**财经新闻**
1. [a16z 指数：GPU 租赁价格全面上涨，H200 较年初涨 160%](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Brotli 高危漏洞波及 Python 与 Node.js HTTP 组件](https://www.aikido.dev/blog/python-packages-vulnerable-node2shell-brotli-cve-2026-111497) ⭐️ 8.0/10

谷歌 Brotli 解码器漏洞 CVE-2026-111497（CVSS 4.0 评分为 9.2）影响 1.0.3 至 1.2.0 版本，并波及 Python 与 Node.js 的 HTTP 组件。远程未认证攻击者可发送特制压缩流，导致内存损坏、敏感数据泄露、进程崩溃，甚至可能执行任意代码。修复版本为 Python brotli 1.2.1、brotlicffi 1.2.1.0，以及 Node.js 22.23.4、24.22.1 或 26.12.1。

telegram · zaihuapd · 10月25日 02:42

**「背景」** Brotli 是 HTTP 内容编码中常用的压缩格式，语言绑定和运行时通常直接依赖其 C 解码器来解析不可信的压缩流。据披露，该漏洞最初以 Node2Shell 名称公开，后被称为 HTTP2Shell；OpenAI 表示于今年 2 月发现该问题。

**「影响」** 使用受影响版本的 Python 或 Node.js 服务应尽快升级到对应修复版本，否则处理来自不可信来源的 Brotli 压缩流可能被远程未认证攻击者利用，造成内存破坏甚至任意代码执行。

**标签**: `#Brotli`, `#CVE-2026-111497`, `#security`, `#Python`, `#Node.js`

---

<a id="item-tech-news-2"></a>
### [Cerebras 详解万亿参数模型部署](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

Cerebras 在官方博客中介绍其如何在晶圆级系统上部署万亿参数级前沿 AI 模型，称这体现了系统工程能力的进展。该内容属于厂商自述，尚不构成独立验证；社区评论普遍质疑其实际可访问模型的时效性、输出质量，以及硬件供应能否跟上需求。

hackernews · gmays · 10月25日 01:33 · [社区讨论](https://news.ycombinator.com/item?id=50227356)

**「背景」** Cerebras 的晶圆级引擎 WSE-3T 单颗晶圆只有 44GB 片上内存，而万亿参数模型的权重通常需要 TB 级存储，因此部署时必须将模型拆分并映射到多块晶圆上。该公司在公开介绍中称，其方案能在推理时实现每秒 1000–2000+ token 的吞吐量，这正是理解其部署方式所需的关键前提。

**「影响」** 对于考虑用 Cerebras 做 AI 推理的开发者来说，社区实测显示部分可访问模型速度很快但结果并不可靠，因此在上线生产前应核实目标模型版本是否可用、质量是否达标，而不能仅凭宣传速度做选择。

**「社区讨论」** 评论者围绕模型新鲜度展开讨论：piterrro 认为如果 Cerebras 平均比前沿模型晚 6 到 9 个月，那么未来几个月应能看到更接近前沿的模型；keyle 则表示实际可用的大多是“GPT OSS 120b、Qwen 3.8 27B”这类模型，速度虽快但错误率较高。ilaksh 还指出，Cerebras 的硬件制造能力和资金规模限制了其满足爆发式需求的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras">How we deploy Trillion-parameter frontier models on Cerebras</a></li>
<li><a href="https://x.com/cerebras/article/2113315017714246003">How we deploy Trillion-parameter frontier models on Cerebras</a></li>
<li><a href="https://dev48.org/en/articles/how-cerebras-deploys-trillion-parameter-ai-models">How Cerebras Deploys Trillion-Parameter AI Models</a></li>

</ul>
</details>

**标签**: `#cerebras`, `#ai inference`, `#trillion-parameter models`, `#wafer-scale hardware`, `#ai infrastructure`

---

<a id="item-tech-news-3"></a>
### [苹果周三发布首款触屏 MacBook Pro](https://www.bloomberg.com/news/newsletters/2026-10-25/apple-to-unveil-touch-screen-macbook-pro-executive-promotions-in-box-checker) ⭐️ 7.0/10

据彭博社报道，苹果计划于本周三推出首款触屏 MacBook Pro，这也是 Mac 首次支持触摸和 OLED 屏幕，并加入灵动岛设计。新机提供 14 英寸与 16 英寸版本，起售价预计高于现款 2499 美元。此为该报道中的发布计划，尚未经官方公布或实际开售证实。

telegram · zaihuapd · 10月25日 14:25

**「背景」** 多年来，苹果高管一直以人体工学为由否定触屏笔记本，认为触控不适合 Mac。本次发布将是这一立场的首次逆转，报道将转变归因于营收与营销考量，并指出触控将作为键盘、触控板的补充，而非替代。

**「影响」** 计划近期购买 MacBook Pro 的用户可以暂缓下单，等待周三官方公布具体配置与价格后再做决定；触屏和 OLED 将改变 Mac 笔记本的交互与显示体验，但新机价格预计比现款有所提高。

**标签**: `#Apple`, `#MacBook Pro`, `#Touchscreen`, `#OLED`, `#Hardware`

---

<a id="item-tech-news-4"></a>
### [10 年前的 CNN 在皮肤癌诊断上胜过前沿 LLM](https://lynchlab.net/llm-skin-cancer) ⭐️ 6.0/10

一项实证对比显示，10 年前的 Inception v3 CNN 在微调后，皮肤癌（皮肤病变）图像诊断表现优于前沿 LLM。作者在单块 H100 GPU 上，用 ISIC Archive 中 68,011 张皮肤镜和临床图像微调了网络全部层，并用与训练数据完全隔离的 200 个病变图像测试；结果表明专用小模型在窄任务上仍可超过通用大模型。该结果属于特定基准上的比较，并非已上线的临床诊断系统。

hackernews · sungam · 10月25日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=50233779)

**「背景知识」** 皮肤病变图像识别通常使用专门的深度卷积网络，而 ISIC Archive 是该领域常用的公开数据源，提供大量皮肤镜与临床图像用于训练和评估。相比之下，前沿 LLM 是面向多种任务训练的通用模型，因此其能否在皮肤癌分类这一窄任务上胜过针对此类图像微调的老式 CNN，需要实际测试而非假设。

**「影响」** 对构建医疗影像诊断流程的开发者，这项对比说明应把微调后的专用 CNN 纳入基线评估，不能默认前沿 LLM 会在窄分类任务上更准确；在相关基准上选用模型时，需要先验证专用模型与通用模型的实际差距。

**「社区讨论」** 多名评论者认为这个结果并不意外：专用小模型在特定任务上超过通用大模型，类似围棋中专用网络远超通用 LLM 的情况。也有评论者提醒，这可能是针对基准优化的“benchmaxxing”，而 LLM 的潜在价值或许在于结合病历文本、追问患者或处理纹身等分布外图像，而非直接替代专用图像分类器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lynchlab.net/llm-skin-cancer">A 10-year-old CNN outperforms frontier LLMs for skin ... | Lynch Lab</a></li>
<li><a href="https://www.isic-archive.com/">ISIC | International Skin Imaging Collaboration</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#LLMs`, `#computer vision`, `#medical AI`, `#benchmarking`

---

<a id="item-tech-news-5"></a>
### [Borcherds 称 AI 使批改作业失去意义](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 6.0/10

加州大学伯克利分校数学教授 Richard Borcherds 表示，在学生普遍使用 AI 的情况下，批改作业已没有意义，因为教师无法判断作业是否由学生本人完成。这是一位知名数学家对教学实践的个人判断，并非已实施的政策变化或独立测量结果；报道未说明他是否已因此调整课程评分或停止布置作业。

hackernews · romanhn · 10月25日 16:28 · [社区讨论](https://news.ycombinator.com/item?id=50233304)

**「背景」** 理查德·博尔彻兹（Richard Borcherds）是加州大学伯克利分校的数学教授，也是菲尔兹奖得主。此前他已不再亲自批改作业，而是花钱请阅卷人为作业正确性打分。据《每日加州人》等报道，在看到大量学生借助 AI 稳定获得满分后，他认为继续为作业正确性评分已“没有意义”。

**「影响」** 对大学数学教学而言，这一表态将“AI 是否让作业失去评分价值”的讨论带入公开议程，促使教师重新考虑作业在总成绩中的权重，并可能更多依赖考试、口试或课堂表现来评估学生。不过，报道中没有提供任何课程调整、政策变化或替代考核方案，读者不应据此认为伯克利已改变教学政策。

**「社区讨论」** 有评论者指出其中的讽刺之处：Borcherds 本人早已不亲自批改作业，而是由助教完成，因此他的表态更像是对作业目的的质疑；另一些评论认为，作业即使被抄袭或相互参考，也能迫使学生接触和思考课程内容，完全取消批改可能削弱学习动力并影响考试成绩。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html">AI use leads UC Berkeley math professor to see ‘no point’ in ...</a></li>
<li><a href="https://newsscore.com/story/197972">UC Berkeley Fields medalist math professor stops grading ...</a></li>

</ul>
</details>

**标签**: `#AI in education`, `#mathematics`, `#academia`, `#LLMs`, `#Richard Borcherds`

---

<a id="item-tech-news-6"></a>
### [Nanbeige 开源 33B 教师模型 Nanbeige4.3-33B](https://www.reddit.com/r/MachineLearning/comments/1xf6x35/nanbeige_releases_nanbeige4333b_an_apache_20/) ⭐️ 6.0/10

Nanbeige 发布 Nanbeige4.3-33B，权重以 Apache 2.0 开源，定位为即将推出的 3B 等小型智能体模型的教师模型。模型卡标注 512K 上下文窗口；团队称在 Terminal-Bench 2.1 上取得 80.9 分，高于 Qwen3.8-27B 的 73.0 分，但在 SWE-Bench Pro 上为 60.3 分，略低于后者的 61.7 分。这些基准结果为发布方自测，未经独立复现；复现智能体评测需保留 preserve\_thinking=true，该设置官方仅推荐用于多轮工具调用，而非普通对话。

reddit · r/MachineLearning · /u/jatingargiitk · 10月25日 16:32

**「背景」** Nanbeige LLM Lab 在 Hugging Face 上以 Apache 2.0 许可证发布了 Nanbeige4.3-33B，模型卡片标注 524,288 token 的上下文窗口，并默认启用推理。根据外部分发报道，该模型 330 亿参数、为稠密文本模型，厂商自报在 Terminal-Bench 2.1 上达到 80.9、在 DeepSWE 上达到 65.5，而对比的 Qwen3.8-27B 分别为 73.0 和 42.5；这些数字属于发布方自报评测，尚未经独立复现。

**「影响」** 对打算基于该模型构建或蒸馏小型智能体的开发者，Apache 2.0 许可降低了使用门槛，但应把榜单分数视为厂商报告而非部署排名，并用固定 preserve\_thinking=true 的完整工具调用测试自行验证。若用于通用聊天，官方并不建议开启该设置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/nanbeige-opens-33b-model-under-apache-20-with-512k-context">Nanbeige Opens 33 B Model Under Apache 2 . 0 With... | AI Weekly</a></li>
<li><a href="https://www.marktechpost.com/2026/10/25/nanbeige-releases-nanbeige4-3-33b-open-agentic-coding-model/">Nanbeige Releases Nanbeige 4 . 3 - 33 B , a 33 B Open... - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#large language models`, `#open source models`, `#AI agents`, `#benchmarks`, `#model release`

---

<a id="item-tech-news-7"></a>
### [memt-1.0 记忆原生架构：门控 DeltaNet-2 与混合存储](https://www.reddit.com/r/MachineLearning/comments/1xeu0ht/memt10_architecture_breakdown_gated_deltanet2/) ⭐️ 6.0/10

据 Reddit 上的一篇技术总结，memt-1.0 采用记忆原生架构，将智能体过去的执行经验持续内化为模型权重或状态，而非依赖追加式提示堆叠或外部 RAG。帖子称，在 128k token 历史长度下，memt-1.0-nano 相比全上下文 KV 缓存可实现约 1.86 倍端到端推理加速和 66 倍持久化存储缩减，通过门控 DeltaNet-2 的 token 级记忆更新机制与 mixture-of-storage 层扩展容量，并用 34B token 的两阶段训练保持通用推理能力。需注意，这些数字来自该 Reddit 帖子的转述，目前没有附带原始论文、基准代码或独立验证。

reddit · r/MachineLearning · /u/Mrs-Grumpy23 · 10月25日 05:31

**「背景」** MemT-1.0 由 MemTensor 提出，官方 arXiv 摘要称其为构建在 Metis 之上的记忆基础模型架构：记忆被内化为模型计算的一部分，采用 Gated DeltaNet-2 的稳定 token 级更新机制，并新增 Mixture-of-Storage 以扩展原生记忆容量。本 Reddit 帖子围绕该架构做非正式技术拆解，帖中提到的推理加速与存储缩减等效率数据源自项目发布方的表述，尚未见第三方独立验证。

**「影响」** 如果这些宣称得到验证，长期任务智能体的开发者将多出一种把记忆压入模型计算层、减少 KV 缓存与外部检索依赖的架构选择；但在原始论文或可复现基准公布之前，不应直接依据 1.86 倍和 66 倍的数字做工程决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.26825">[2610.26825] MemT-1.0: Towards Memory-Native Evolution</a></li>
<li><a href="https://github.com/MemTensor/MemT-1.0/">GitHub - MemTensor/MemT-1.0: Official repository for MemT-1.0</a></li>

</ul>
</details>

**标签**: `#AI memory`, `#LLM inference`, `#agentic AI`, `#model architecture`, `#storage efficiency`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [a16z 指数：GPU 租赁价格全面上涨，H200 较年初涨 160%](https://x.com/a16z/status/2113741008550990191) ⭐️ 7.0/10

以 2026 年 1 月 1 日为基准 100 的 a16z GPU 租价七日移动平均指数显示，截至 10 月 19 日 H200 升至约 265（累计+160%），B200 约 225（+120%）。RTX PRO 6000 约 165（+65%）、H100 约 137（+35%），连 2020 年发布的 A100 也略高于年初水平。

telegram · zaihuapd · 10月25日 06:39

**「背景」** 该指数由 a16z 编制，以 2026 年 1 月 1 日为基准 100，追踪主流 GPU 云租赁的小时价格；除该指数外，Runpod 等云平台也公开按小时报价，但实际价格会因供需和租用方式而明显不同。

**「影响」** 依赖云端 GPU 进行 AI 训练和推理的企业将面临更高的算力成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.runpod.io/pricing">GPU Cloud Pricing | Per-Second H100, A100, RTX | Runpod</a></li>

</ul>
</details>

**标签**: `#GPU rental prices`, `#AI infrastructure`, `#compute demand`, `#H200/B200`, `#price index`

---