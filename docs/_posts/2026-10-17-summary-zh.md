---
layout: default
title: "Horizon Summary: 2026-10-17 (ZH)"
date: 2026-10-17
lang: zh
---

> 从 52 条内容中筛选出 25 条重要资讯。

---

**科技新闻**
1. [Claude 破解 NIST ECDSA 曲线种子来源之谜](#item-tech-news-1) ⭐️ 8.0/10
2. [越狱 PS5 原生运行 llama.cpp，执行 GGUF 模型](#item-tech-news-2) ⭐️ 8.0/10
3. [Big Fish：OpenBSD 一个存在 37 年的内核漏洞被利用并公开分析](#item-tech-news-3) ⭐️ 8.0/10
4. [ORL 开源扩散模型推理方案：单张 RTX 5090 宣称达 2,788 tokens/s](#item-tech-news-4) ⭐️ 8.0/10
5. [特斯拉展示 Roadster 冷气推进器与火箭发动机选项](#item-tech-news-5) ⭐️ 7.0/10
6. [Apple 用 MLX 在 Mac Studio 集群运行近万亿参数 Muse Spark Open](#item-tech-news-6) ⭐️ 7.0/10
7. [JPEG XL 与 AVIF 网页应用场景对比评测](#item-tech-news-7) ⭐️ 7.0/10
8. [Claude Code 团队公开 AI 代码审查流程](#item-tech-news-8) ⭐️ 7.0/10
9. [Mercor 报告：现有 AI 基准未覆盖约九成美国工作时长](#item-tech-news-9) ⭐️ 7.0/10
10. [StarSkirmish Bench v0.2：大模型写代码打星际争霸](#item-tech-news-10) ⭐️ 7.0/10
11. [Kangrejos 2026 提出 pin\_init 安全自引用结构方案](#item-tech-news-11) ⭐️ 7.0/10
12. [阶跃星辰发布 Step 5 Preview 智能体旗舰模型](#item-tech-news-12) ⭐️ 7.0/10
13. [Telegram 向美政府提供用户数据细节曝光](#item-tech-news-13) ⭐️ 7.0/10
14. [Waymo 宣布将在多伦多推出自动驾驶网约车服务](#item-tech-news-14) ⭐️ 6.0/10
15. [Home Assistant 泄露扫描未征得同意，维护者道歉并给出关闭方法](#item-tech-news-15) ⭐️ 6.0/10
16. [软件渲染的独特画风引发 GPU 差异讨论](#item-tech-news-16) ⭐️ 6.0/10
17. [GNOME OS 推出面向非开发者的 Preview 版本](#item-tech-news-17) ⭐️ 6.0/10
18. [Linux NFS 服务器近期与未来变化综述](#item-tech-news-18) ⭐️ 6.0/10
19. [Rust 框架 DenseCore 逐位对齐 PyTorch 的 nanoGPT](#item-tech-news-19) ⭐️ 6.0/10
20. [可灵 Kling 4.0 全量上线，API 近期开放](#item-tech-news-20) ⭐️ 6.0/10

**财经新闻**
1. [市场回调与利率上升考验 AI 数据中心交易潮，多宗上市被撤回](#item-finance-news-1) ⭐️ 7.0/10
2. [商务部拟对 AI、生物医药、光伏相关 40 项技术出口实施临时登记](#item-finance-news-2) ⭐️ 7.0/10
3. [Anthropic IPO 估值预期下调至 1.5 万亿美元](#item-finance-news-3) ⭐️ 7.0/10

**推特新闻**
1. [Anthropic：Claude Mythos 5 可设计出比已发表最佳结果更高效的量子电路](#item-twitter-news-1) ⭐️ 8.0/10
2. [OpenAI 宣布 GPT-6 Astra Pro 升级：更快响应与并行多智能体任务](#item-twitter-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude 破解 NIST ECDSA 曲线种子来源之谜](https://www.anthropic.com/research/ecdsa-curve-origins) ⭐️ 8.0/10

Anthropic 的研究称，Claude 已经解开了 NIST ECDSA 曲线种子来源的长期谜团：P-192、P-224、P-256、P-384 和 P-521 的种子并非哈希算法的输出，而是 C 库的 lrand48 随机数生成器以 Unix 时间戳为种子生成的结果。这意味着这些种子可以用实际生成路径进行复现验证，但二进制曲线 B-163 的种子仍然未被解释。

hackernews · ahlCVA · 10月16日 18:55 · [社区讨论](https://news.ycombinator.com/item?id=50122800)

**「背景」** NIST 在 FIPS 186 中为 P-192、P-224、P-256、P-384、P-521 等椭圆曲线给出的参数种子，长期来源不明，密码学界一直无法解释它们是如何生成的。Anthropic 的研究显示，这些种子实际上是 C 库伪随机函数 lrand48\(\) 以 Unix 时间戳为种子后输出结果右移 23 位的产物，而不是某个哈希函数的输出。

**「影响」** 对信任或审查 NIST 曲线的密码学界而言，这一发现让种子来源从黑箱猜测变成可复现的实验对象；但正如评论者所指出的，确认生成方式并不等于证明曲线在选定过程中没有经过特定属性筛选，因为无法看到生成后未被采用的候选种子。

**「社区讨论」** 评论中 fidotron 提醒，确认生成方法并不能说明曲线的选择过程，被生成后丢弃的候选种子不可见，因此仍不能完全排除按特定属性搜索时间戳后选曲线的可能性；teddyh 则猜测 B-163 无法复现可能只是公布过程中打错了一位数字。tptacek 称这一发现对 NIST 密码学阴谋论是“毁灭性消息”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/ecdsa-curve-origins">Claude reveals ECDSA curve origins \ Anthropic</a></li>
<li><a href="https://man.openbsd.org/lrand48.3">rand48(3) - OpenBSD manual pages</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#NIST curves`, `#Claude`, `#random number generation`, `#security research`

---

<a id="item-tech-news-2"></a>
### [越狱 PS5 原生运行 llama.cpp，执行 GGUF 模型](https://github.com/cobanov/PS5LM) ⭐️ 8.0/10

GitHub 项目 cobanov/PS5LM 让越狱版 PlayStation 5 原生运行 llama.cpp，可直接加载并执行 GGUF 格式模型，把游戏主机改造成低功耗的本地 LLM 推理设备。该能力面向已经越狱主机的玩家和硬件黑客，目前项目以 GitHub 为主要托管地。

hackernews · Anon84 · 10月16日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=50122431)

**「背景」** PS5LM 把 llama.cpp 移植到已越狱的 PlayStation 5，使其能原生运行 GGUF 模型，上游 llama.cpp 以子模块固定版本，并为 PS5 补齐所缺的少量 libc 函数。Horizon 9 月 30 日的日报曾报道一个代号 Relapse 的 PS5 漏洞，据称针对 WebKit/JavaScriptCore，但当时尚无完整越狱被独立证实；这类越狱路径若能成立，正是 PS5LM 在本机运行的前提条件。

**「影响」** 对想用低价硬件长时间运行本地 LLM 的用户来说，这项移植指明了一个更便宜的载体：社区用户推测，采用与 PS5 同源“Cyan Skillfish”APU 的二手 BC-250 矿卡（二手价约 60–100 美元）也可能运行同一套 llama.cpp 移植，从而把本地推理硬件成本压到远低于整机 PS5 的水平。不过 BC-250 的标准 Windows 驱动并不提供常规 GPU 加速，实际性能和驱动适配仍需单独验证。

**「社区讨论」** Rabbit504030201 担心项目托管在 GitHub 容易被索尼要求下架，建议改用自定义域名；shiftpgdn 认为同样基于 PS5 定制硅片的二手 BC250 显卡（Cyan Skillfish APU）也应能运行，eBay 价格约 150 至 200 美元。另有评论者 jjcm 称目前只能以 2-bit 量化运行约 27B 的 Qwen 模型，但认为它适合长时间低强度文本生成任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">2026-09-30 — PS5 Relapse exploit reportedly targets WebKit JavaScriptCore bug</a></li>
<li><a href="https://github.com/cobanov/PS5LM">cobanov / PS 5 LM : llama . cpp on a jailbroken PS 5 : run any GGUF ...</a></li>
<li><a href="https://www.ebay.com/itm/327403530900">ASRock AMD BC-250 PS5 APU Board RDNA2 16GB GDDR6- - eBay</a></li>
<li><a href="https://pithwire.com/en/articles/the-60-gaming-pc-amd-bc-250-2025/">AMD BC-250: The $60-$100 PS5-Chip Gaming PC | PithWire</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#PS5`, `#GGUF`, `#LLM inference`, `#hardware hacking`

---

<a id="item-tech-news-3"></a>
### [Big Fish：OpenBSD 一个存在 37 年的内核漏洞被利用并公开分析](https://calif.io/research/big-fish) ⭐️ 8.0/10

安全研究报告《Big Fish》公开了如何在 OpenBSD 中利用一个存在 37 年的内核漏洞，并以此说明，即便是像 OpenBSD 这样长时间受到严格审计的代码库，单靠人工代码审查也可能长期漏掉某些内核级缺陷。报告由 calif.io 发布，但其中未提供可验证的漏洞版本号或修复补丁，安全影响仍需以原始报告为准。

hackernews · rs\_rs\_rs\_rs\_rs · 10月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50118977)

**「背景」** 该漏洞涉及一个共享内存附件计数器字段。根据 Calif 的研究报告，这个字段在约 37 年前的原始 BSD 源码中就被定义为有符号 16 位短整型，并被后来各 BSD 分支继承至今；报告同时澄清，37 年指的是这项继承设计的年龄，而不是说现代 OpenBSD 本身已经存在了这么久。

**「影响」** 该研究把一个存在约 37 年的内核缺陷做成了可利用漏洞，说明即便是 OpenBSD 这类以安全为核心、长期被密集审计的系统，仅靠人工代码审查也难以发现此类问题。OpenBSD 用户应关注官方 errata 和后续补丁发布并及时评估升级；在官方修复落地前，不应假设默认内核配置对此漏洞天然免疫，具体受影响版本和利用条件应以研究报告的完整内容为准。

**「社区讨论」** 有评论者提到，NetBSD 曾在 1999 年 8 月重写相关代码时意外修复了这个 bug；另一名评论者则认为，这类缺陷很难靠 fuzzing 或静态分析发现，可能必须由人从利用原语入手思考才能找到。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://calif.io/research/big-fish">Big Fish : Exploiting a 37 - Year - Old Kernel Bug in OpenBSD | Calif</a></li>
<li><a href="https://dzen.ru/a/atJi8f5wA2igUvxy">Calif получила root в OpenBSD через 37 -летнюю ошибку ядра | Дзен</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenBSD">OpenBSD - Wikipedia</a></li>
<li><a href="https://calif.io/research/big-fish">Big Fish : Exploiting a 37-Year-Old Kernel Bug in OpenBSD | Calif</a></li>

</ul>
</details>

**标签**: `#openbsd`, `#kernel-security`, `#exploitation`, `#operating-systems`, `#security-research`

---

<a id="item-tech-news-4"></a>
### [ORL 开源扩散模型推理方案：单张 RTX 5090 宣称达 2,788 tokens/s](https://www.reddit.com/r/MachineLearning/comments/1x7qgr0/research_2788_tokenss_on_a_single_rtx_5090_with_a/) ⭐️ 8.0/10

研究团队发布 ORL（On-Policy Residual Learning）与自研推理引擎 dlmrt，宣称在单张 RTX 5090 上对 LLaDA-2.1-mini 达到 2,788 tokens/s 的峰值单请求解码速度，并在 8×B200 上对 DiffusionGemma 26B MoE 达到 7,708 tokens/s。模型、训练代码、评测流程与推理引擎均已开源。作者强调这些数字来自特定基准的峰值结果且为 batch size 1 的单请求解码，并非任意提示词的平均值。

reddit · r/MachineLearning · /u/arty\_photography · 10月16日 20:03

**「背景」** 扩散语言模型不同于逐个生成 token 的自回归模型，可以在一次前向中并行精化多个 token。ORL 通过在训练中回放模型自身生成的残差状态，并引入 Adjacent Entropy Contraction 鼓励每步去噪更快降低不确定性，从而让模型用更少前向完成更多 token；dlmrt 则通过 CUDA graph 捕获整个去噪循环，避免 CPU 逐步骤启动和同步。作者还将 ORL 与 DFlash、EAGLE3 等投机解码方法做了端到端对比。

**「影响」** 对拥有 RTX 5090 的本地推理用户，可以直接用 dlmrt 运行 LLaDA-2.1-mini ORL NVFP4 检查点来验证宣称的速度；对研究者，完整的开源代码和模型使得在自身负载上复现结果、比较其他推理路径或评估单请求延迟之外的真实瓶颈成为可能。

**标签**: `#diffusion LLMs`, `#inference optimization`, `#open source`, `#efficient decoding`, `#GPU performance`

---

<a id="item-tech-news-5"></a>
### [特斯拉展示 Roadster 冷气推进器与火箭发动机选项](https://www.tesla.com/roadster) ⭐️ 7.0/10

特斯拉发布了一段 Roadster 宣传视频，展示这款纯电超级跑车配备冷气推进器，并提供燃烧式火箭发动机选装，火箭版标注为“仅限邀请”。目前这仍是发布前的营销演示，尚无量产交付产品，具体性能、价格和上市时间也尚未公布。

hackernews · shekhar101 · 10月16日 01:32 · [社区讨论](https://news.ycombinator.com/item?id=50112657)

**「背景」** 冷气推进器依靠高压气体高速喷出产生反作用力，通常用于航天器姿态控制，本身不涉及燃烧。特斯拉此次展示的 Roadster 提供两种版本：一种仅用冷气为额外向前加速提供推力，另一种配备真正的燃烧火箭发动机，并采用邀请制销售。

**「影响」** 对潜在买家而言，这是一次营销展示而非已交付能力：基础版 Roadster 的预订需先支付 5,000 美元，并在 10 天内再付 45,000 美元，而冷气推进器和空气吸入系统均属额外选装。外媒按约 4,000 磅车重反推，纯电基础版即可提供约 2.5 G 的起步加速度；视频中的飞行或垂直机动依赖高可选配推力系统，购车决策应把演示效果与标准版规格及选装成本明确区分。

**「社区讨论」** 有评论者称这是极酷的营销演示，但质疑冷气推进器对车辆周围人员的安全风险，并指出特斯拉无法保证 Roadster 预订单最终交付；另一些评论则聚焦垂直或贴顶飞行在千公斤级车重和有限储气条件下的技术可行性，并批评长期收取订金相当于向用户获取无息贷款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.engadget.com/2288437/teslas-redesigned-roadster-cold-gas-thruster-option-reservation/">Tesla &#x27;s Redesigned Roadster Has A Cold - Gas Thruster Option, But...</a></li>
<li><a href="https://www.motorbiscuit.com/insane-tesla-roadster-0-60-mph-in-1-1-seconds-uses-gas-thruster-option/">Insane: Tesla Roadster 0-60 MPH in 1.1 Seconds Uses Gas Thruster ...</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#electric vehicles`, `#rocket propulsion`, `#automotive engineering`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [Apple 用 MLX 在 Mac Studio 集群运行近万亿参数 Muse Spark Open](https://machinelearning.apple.com/research/mlx-distributed-inference) ⭐️ 7.0/10

Apple ML Research 发布了一项分布式推理演示：通过最新版本的 MLX，将接近一万亿参数的 Muse Spark Open 开放模型运行在四台 Mac Studio 组成的集群上，生成速度超过每秒 36 个 token。该演示还覆盖了从单台最高 512GB 统一内存的 Mac Studio 起步、再扩展到多机集群的路径，但这是 Apple 自家的展示，不等同于独立第三方基准。

hackernews · antipaul · 10月16日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=50118320)

**「背景」** Muse Spark Open 是 Meta 与 Apple 联合发布的开放权重模型，约 8160 亿参数，The Verge 报道称 Meta 形容其为“迄今最强的美国开放权重模型”，并针对 Apple 硬件与 MLX 框架优化。更早，Apple ML Research 还发布过把闲置 Apple Silicon 设备动态池化为虚拟 GPU 集群的研究概念。本次博客正是沿这条路径，演示用新版 MLX 把 Muse Spark Open 分布到多台 Mac Studio 上进行推理，属于研究展示而非已上市产品。

**「社区讨论」** 评论区对演示的可比性提出质疑：有读者认为用 4-bit 量化运行 Meta 模型、却让 Qwen 以原生 BF16 对比并不公平，并指出 8,192 token 的上下文长度对实际用途偏短。另有一位开发者分享了自己的实测经验，称单台 M5 Ultra 可以约 45 tok/s 运行 DeepSeek 4.1 Flash，但这属于个人测试而非 Apple 的基准数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://machinelearning.apple.com/research/distributed-gpu-cloud">2026-10-14 — Apple Research Details Virtual GPU Cloud from Idle Apple Silicon</a></li>
<li><a href="https://www.theverge.com/news/1012293/meta-apple-muse-spark-open-ai-model-mlx">Meta and Apple team up to make Muse AI models run... | The Verge</a></li>

</ul>
</details>

**标签**: `#MLX`, `#distributed inference`, `#Apple`, `#large language models`, `#Mac Studio`

---

<a id="item-tech-news-7"></a>
### [JPEG XL 与 AVIF 网页应用场景对比评测](https://jakearchibald.com/2026/jpeg-xl-vs-avif/) ⭐️ 7.0/10

Jake Archibald 在 2026 年 10 月发布了一篇深度技术评测，系统比较 JPEG XL 与 AVIF 在网页场景下的压缩效率、画质与实际取舍。文章面向正在选择图片格式的开发者，属于技术评估而非新版本发布或标准变更；它同时讨论了两种格式各自的优势场景和现实限制。

hackernews · farlight · 10月16日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=50120224)

**「背景」** 10 月 8 日的日报曾报道，Chrome 已重新启用 JPEG XL 支持，加上 Safari 与 Firefox 后，该格式在 2026 年获得了大多数浏览器的覆盖；相比之下，AVIF 的浏览器覆盖率约为 93.4%（2026 年 7 月数据）。Jake Archibald 的这篇文章正是在这一格式支持格局变化后，对 JPEG XL 与 AVIF 在网页场景中的压缩效率、质量和实际取舍进行了实测比较。

**「社区讨论」** 评论区对 AVIF 的画质存在明显分歧：PaulHoule 认为示例 F1 图片中高光细节被 AVIF 抹掉并替换成“看似合理”的内容，不适合需要仔细查看的图片；Metricon 则分享了自己在生产环境使用的 ffmpeg 参数，称可让 AVIF 体积缩小 10 倍以上并保留 PNG 透明通道。另有开发者指出，libjxl 当前编码器仍偏弱，改用更优编码器可让无损 JXL 文件再缩小约 30–39%，因此评测中的 JPEG XL 数据未必代表格式本身的上限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/blog/jpeg-xl-in-chrome">2026-10-08 — Chrome ships JPEG XL support, joining Safari and Firefox</a></li>
<li><a href="https://www.inverity.ai/posts/avif-vs-webp-vs-jpeg-xl-2026">AVIF vs WebP vs JPEG XL in 2026: Which Format Wins?</a></li>

</ul>
</details>

**标签**: `#jpeg-xl`, `#avif`, `#image-compression`, `#web-performance`, `#codecs`

---

<a id="item-tech-news-8"></a>
### [Claude Code 团队公开 AI 代码审查流程](https://claude.dev/blog/solving-code-review-at-anthropic/) ⭐️ 7.0/10

Anthropic 的 Claude Code 团队发布博文，详细介绍其 AI 辅助代码审查流水线：绝大多数拉取请求先经过自动化审查路径，人工注意力只投放在高风险变更上，而评估集（evals）会随每次事故增长，并用来为评审器的每次改动打分。文中称这一流程每天处理约 3 万个拉取请求，但这是团队对内部实践的自我描述，并非独立测量的基准或新产品发布。

hackernews · pretext · 10月16日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=50122951)

**「背景」** LLM 辅助代码审查指的是在合并变更前用大模型自动检查，筛出高风险部分再交由人工处理。10 月 14 日的日报曾报道，PostgreSQL 19 beta 期间大量功能回退被归因于这类审查更早暴露边缘案例缺陷，导致维护者积压过多而无法按时修复；正是在这一背景下，Anthropic 文章介绍了 Claude Code 团队将类似流程用于内部每日海量 PR 的做法。

**「影响」** 考虑采用类似流程的工程团队应把“每天 3 万 PR”视为自报的运营规模，而不是可直接复制的普遍指标；在引入风险分级和事故驱动评估机制前，需要自行测量成本、返工率以及 LLM 生成内容的实际质量。

**「社区讨论」** Hacker News 评论者对该文章的严谨性提出质疑：有评论认为每日大量 PR 可能更多反映返工和低效，而非真实工程产出，并希望看到返工率和每行代码成本；还有评论批评允许 LLM 写文档且无人阅读的做法是“疯狂”。这些是评论者的观点，并非已证实的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1100182/">2026-10-14 — PostgreSQL 19 beta reverts traced to LLM-assisted code review</a></li>

</ul>
</details>

**标签**: `#ai-code-review`, `#anthropic`, `#claude-code`, `#software-engineering`, `#developer-tools`

---

<a id="item-tech-news-9"></a>
### [Mercor 报告：现有 AI 基准未覆盖约九成美国工作时长](https://www.mercor.com/research/labor-index/benchmark-map/) ⭐️ 7.0/10

Mercor 的一份研究报告声称，约 90% 的美国工作时长花在现有 AI 基准很少或未覆盖的任务上，因此当前基准分数难以反映模型在美国真实劳动市场中的表现。报告认为，现有评估更偏向某些类型的工作，而大量需要复杂判断和人际互动的任务缺乏足够覆盖，这使企业很难根据基准判断 AI 能否胜任实际岗位。

hackernews · speckx · 10月16日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=50121179)

**「背景」** 现有 AI 能力基准通常以编码、数学等可自动评分的任务为主，而劳动力研究常借助美国 O\*NET 职业数据库将岗位拆解为具体工作任务；Mercor 此前也发布过 APEX 基准系列，试图衡量模型能否完成具有经济价值的专业工作。这份劳动指数报告正是在这一框架下，对照基准提示与 O\*NET 任务的覆盖范围，评估 AI 在真实工作场景中的可用性。

**「影响」** 对于考虑依据基准分数选型或部署 AI 的企业，报告提示这些分数不能直接等同于真实岗位产出；评估时应尽量采用贴近具体工作任务的测试，否则可能高估模型在日常工作中的可用性。

**「社区讨论」** 有评论者指出，报告似乎把“有基准覆盖”当成了“覆盖得好”，例如用 13 个提示词代表社会工作者“育儿咨询”这类任务，显然不足；另一条评论则用“门房谬误”类比，警告自动化方案可能忽略原有岗位承担的隐性职能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.everydev.ai/tools/mercor">Mercor - AI Expert Workforce Platform | EveryDev. ai</a></li>

</ul>
</details>

**标签**: `#AI benchmarks`, `#labor market`, `#AI evaluation`, `#O\*NET`, `#AI adoption`

---

<a id="item-tech-news-10"></a>
### [StarSkirmish Bench v0.2：大模型写代码打星际争霸](https://starskirmish.com/bench/v0-2/) ⭐️ 7.0/10

StarSkirmish Bench v0.2 更新了让大模型通过编写代码游玩《星际争霸：血战》的基准测试，作者于 2026 年 10 月 16 日发布，并纳入 OpenAI、Anthropic、Google 和 Muse 旗舰模型的对比结果。帖子本身没有给出详细的技术指标或排名表格，因此该项目仍属于自建基准，结果需要独立复现和验证。

hackernews · \_\_cayenne\_\_ · 10月16日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=50118688)

**「背景」** StarSkirmish Bench 是一种让大语言模型通过编写代码来游玩《星际争霸：母巢之战》的基准测试。v0.2 版要求各家模型在 OpenAI Codex、Claude Code、Antigravity CLI、Muse Code 等第一方命令行代理中被评测，默认关闭联网搜索与抓取工具，CLI 在计时开始前才安装，并限定在一小时内完成。此类测评不仅考察模型写代码的能力，也考察其在真实代理环境中的规划、调试与自我修正表现。

**「社区讨论」** 评论区最有价值的交叉印证来自 GodelNumbering：他指出该基准的模型排名（GPT-6 Astra &gt; GPT-6.1 Sol &gt; Gemini 4 Argon &gt; Claude Opus 5.5 &gt; Claude Fable 5.1 &gt; Claude Sonnet 5.5）与他朋友创建的 9×9 围棋基准排名完全一致，尽管两者表面任务不同；这属于个人观察，并非独立验证。cgearhart 则追问这些 agent 生成的机器人是否只是顶尖人工 bot 的劣化版本、是否学会了需要实验反馈或领域经验的功能，以及是否每次都在套用固定策略；这些问题尚未由作者回应。

**标签**: `#AI agents`, `#LLM benchmarks`, `#StarCraft`, `#machine learning`, `#software engineering`

---

<a id="item-tech-news-11"></a>
### [Kangrejos 2026 提出 pin\_init 安全自引用结构方案](https://lwn.net/Articles/1099224/) ⭐️ 7.0/10

在 Kangrejos 2026 上，Gary Guo 提出了一种让内核 Rust 安全实现自引用数据结构的方法，该方案基于 pin\_init crate。这目前仍是方案展示而非已合入的功能，但可能移除 Nova 驱动中大部分与生命周期相关的 unsafe 代码，并最终惠及其他内核 Rust 组件。

rss · LWN.net · 10月16日 18:30

**「背景」** Kangrejos 是 Rust for Linux 项目的年度开发者会议。内核中的 pin\_init crate 用于创建不可移动（immovable）的数据结构，通常是为了与 C 代码互操作；而 Rust 的所有权与借用规则长期以来使得自引用数据结构难以在没有 unsafe 代码的情况下实现。Gary Guo 在 Kangrejos 2026 上提出的方案正是针对这一难题。

**「影响」** 对 Nova 驱动及其他内核 Rust 组件的开发者而言，如果该方案落地，可显著减少为绕过 Rust 生命周期规则而编写的 unsafe 代码；现阶段仍应将其视为提案，尚未表明实现已合并或可直接使用。

**标签**: `#rust`, `#linux-kernel`, `#self-referential-structures`, `#unsafe-code`, `#systems-programming`

---

<a id="item-tech-news-12"></a>
### [阶跃星辰发布 Step 5 Preview 智能体旗舰模型](https://huggingface.co/stepfun-ai/Step-5-Preview) ⭐️ 7.0/10

阶跃星辰在 Hugging Face 发布旗舰模型 Step 5 Preview，面向软件工程与金融场景的智能体任务。这是一款稀疏 MoE 模型，总参数 6000 亿、激活参数 270 亿，支持最高 100 万 token 的多模态上下文，可接收文本、图像和视频输入。官方称其在软件工程、长周期智能体执行和专业知识任务上表现领先，但这是厂商声明，尚缺乏独立基准验证；模型处于 Preview 阶段，可通过 OpenAI 兼容 API 配合 vLLM 或 SGLang 部署，并采用 StepFun Model License 1.0 许可。

telegram · zaihuapd · 10月16日 06:36

**「背景」** 稀疏 MoE（专家混合）架构意味着模型每次推理只激活一小部分参数——Step 5 Preview 总参数为 6000 亿，而激活参数仅 270 亿——这使训练规模远大于单次推理开销，是当前旗舰大模型控制推理成本的主流做法。智能体（agentic）场景要求模型在软件工程或金融分析中自主规划并长周期执行任务，因而需要百万级 token 上下文来容纳完整代码仓库或长篇业务文档。该模型为预览版本，现有能力表述来自厂商发布，尚无独立基准或实际部署数据加以验证。

**「影响」** 开发者现在可以直接从 Hugging Face 下载 Step 5 Preview，并通过 OpenAI 兼容 API 配合 vLLM 或 SGLang 自主部署，从而在软件工程和金融场景的智能体任务中接入这一模型。不过该模型为预览版，实际性能仍需独立基准验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stepfun.com/step-5-preview">Step 5 Preview: Advancing the Pareto Frontier - stepfun.com</a></li>
<li><a href="https://github.com/stepfun-ai/Step-5-Preview">GitHub - stepfun-ai/Step-5-Preview: StepFun&#x27;s flagship model ...</a></li>

</ul>
</details>

**标签**: `#AI models`, `#sparse MoE`, `#agentic AI`, `#software engineering`, `#long context`

---

<a id="item-tech-news-13"></a>
### [Telegram 向美政府提供用户数据细节曝光](https://www.404media.co/heres-what-telegram-giving-data-to-the-u-s-government-looks-like/) ⭐️ 7.0/10

新公开的法院文件显示，Telegram 在回应美国法院命令时向美方提供了一名用户的手机号、用户 ID 和 IP 地址，并称此举为“自愿”，同时不承认受美国司法管辖。涉案人为被控参与 2023 年 10 月 7 日袭击以色列事件的 Mahmoud Al-Muhtadi；截至今年 1 月，Telegram 已向美方提供 2253 名用户的数据。

telegram · zaihuapd · 10月16日 14:57

**「背景」** 此事源于一起具体刑事案件：Mahmoud Al-Muhtadi 被控参与 2023 年 10 月 7 日针对以色列的袭击，美国执法部门据此向 Telegram 索取其账户信息。Telegram 在回函中称提供数据系“自愿”，同时不承认受美国司法管辖。

**「影响」** 对依赖 Telegram 隐私保护的用户而言，此次披露表明美国法院命令可能促使 Telegram 交出可直接关联到账户和网络位置的手机号、用户 ID 与 IP 地址。有关用户应意识到，Telegram 的隐私承诺并不等同于对司法数据请求免疫。

**标签**: `#privacy`, `#telegram`, `#government-data-requests`, `#surveillance`, `#tech-policy`

---

<a id="item-tech-news-14"></a>
### [Waymo 宣布将在多伦多推出自动驾驶网约车服务](https://waymo.com/blog/2026/10/waymo-in-toronto/) ⭐️ 6.0/10

Waymo 于 2026 年 10 月 16 日通过官方博客宣布，其自动驾驶网约车服务将进入多伦多。该消息目前属于公司公告，尚未披露具体上线时间、覆盖区域或车队规模等细节；因此还不能视为服务已在当地实际运营。

hackernews · ChrisArchitect · 10月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50118981)

**「背景」** 此前多家加拿大媒体曾报道，Waymo 有意将自动驾驶出行服务扩展至多伦多和卑诗省，并可能成为加拿大首个无人驾驶出租车车队，但仍需安大略省政府批准。相关报道还提示，多伦多的冬季道路环境和监管阻力是落地的不确定因素。此次 Waymo 官方博客宣布在多伦多启动服务，是对这一计划的重要推进。

**「影响」** Waymo 官方公告称，将在多伦多建设本地设施和岗位，目标 2028 年迎来首批乘客，因此多伦多可能成为加拿大首个提供完全无人驾驶网约车的城市。对当地居民而言，近期可见的变化主要是自动驾驶测试车开始上路以及本地投资和就业机会，而非立刻就能使用的无人驾驶出行服务。

**「社区讨论」** 评论中的乘客体验呈现差异：tcoop25 报告在奥斯汀的首次乘车本应只需 9 分钟，却突然被延长到 45 分钟，客服将其放在餐厅后道歉，最终只能改乘人工 Uber；tpurves 和 joshuat 则表示在旧金山等地的体验良好或正常。ilamont 还提到多伦多公告以就业为开篇，并称波士顿因担心就业损失而出现针对 Waymo 的立法阻力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://driveteslacanada.ca/news/waymo-eyes-canadian-launch-in-toronto-and-b-c/">Waymo eyes Canadian launch in Toronto and B.C. - Drive Tesla</a></li>
<li><a href="https://www.cbc.ca/news/canada/toronto/waymo-self-driving-taxis-toronto-9.7023379">Could Torontonians soon ride self-driving taxis? That’s Waymo ’s plan</a></li>
<li><a href="https://www.readthepeak.com/p/take-the-wheel">Waymo eyes Toronto expansion, Discount grocery stores are...</a></li>
<li><a href="https://waymo.com/blog/2026/10/waymo-in-toronto/">Hello Toronto! Waymo is En Route</a></li>
<li><a href="https://toronto.citynews.ca/2026/10/16/waymo-cars-autonomous-toronto-2028-launch/">Waymo eyes Toronto launch in 2028 - CityNews Toronto</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#waymo`, `#ride-hailing`, `#AI-transportation`, `#expansion`

---

<a id="item-tech-news-15"></a>
### [Home Assistant 泄露扫描未征得同意，维护者道歉并给出关闭方法](https://github.com/home-assistant/home-assistant.io/issues/49314) ⭐️ 6.0/10

Home Assistant 用户报告称，Supervisor 的密码泄露检查会在未明确选择加入的情况下，把应用选项中密码哈希的前 5 个字符发送给第三方服务。维护者 Frenck 为此致歉，并说明该检查已存在多年，可用 \`ha security options --pwned=false\` 关闭，只是近期版本修复了相关提示，用户才开始注意到这一行为。

hackernews · trvrprkr · 10月16日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=50124251)

**「背景」** 这类密码泄露检查通常采用“Have I Been Pwned”式的 k-匿名模型：客户端只发送密码哈希的前 5 个字符，服务端返回匹配的完整哈希后缀，以便在不暴露完整密码的情况下判断密码是否出现在已知泄露中。Home Assistant 的 Supervisor 很早就将该检查用于标记为密码的应用选项，但直到最近的修复让警告可见，用户才意识到存在此行为。

**「社区讨论」** 多名用户质疑，无论哈希前缀在数学上多么“安全”，未获明确同意就把任何数据发送给第三方都不可接受；维护者 Frenck 在后续回复中致歉，并指出该检查可用 \`--pwned=false\` 关闭。另有评论者说明这是与许多密码管理器相同的泄露扫描机制，也有人借此批评项目维护者的沟通态度。

**标签**: `#home-assistant`, `#privacy`, `#security`, `#open-source`

---

<a id="item-tech-news-16"></a>
### [软件渲染的独特画风引发 GPU 差异讨论](https://www.jamesfmackenzie.com/2026/10/13/i-love-software-rendering/) ⭐️ 6.0/10

《I Love Software Rendering》是一篇回顾软件渲染视觉特色的文章；它把低分辨率下的像素化纹理、阴影和光照查找表等表现归因于 CPU 逐像素软件渲染，并对比了当时 GPU 固定功能管线的不同。评论者对此提出两点保留：部分效果其实只是关闭了空间抗锯齿，现代游戏仍可做到；但 GPU 只在三角形覆盖像素中心时才绘制三角形，与旧软件渲染的三角形覆盖规则不同，低分辨率下画面会有差异。

hackernews · speckx · 10月16日 12:52 · [社区讨论](https://news.ycombinator.com/item?id=50117746)

**「背景」** 软件渲染指使用 CPU 逐像素完成三角形填充、纹理映射和光照计算；在可编程着色器普及前，GPU 路径受固定功能限制，而 CPU 软件代码理论上可以实现任意效果。评论者提到，可编程着色管线要到 GeForce 3（2001 年）才出现。

**「影响」** 对希望复现这种复古画面的开发者，一个直接可行的手段是在现代游戏中关闭空间抗锯齿；但若想完全复刻旧软件渲染的低分辨率观感，还需要处理 GPU 的像素中心覆盖规则，并考虑 CPU 渲染的开销——评论提醒 CPU 还要承担游戏逻辑，不能只做矩阵乘法。

**「社区讨论」** 评论中最主要的争论是：这种画面究竟属于软件渲染的本质，还是仅仅关闭抗锯齿的结果；delta\_p\_delta\_x 认为它只是关闭空间抗锯齿，现代游戏仍可做到，buffportion 则强调旧 CPU 渲染不使用重心坐标逐像素判断，与 GPU 的三角形覆盖方式不同。BugsJustFindMe 甚至认为标题应改为“我喜爱像素化纹理”，bob1029 补充说可编程着色器出现前 CPU 软件渲染能实现 GPU 路径无法实现的效果，这成为讨论中的主要分歧线。

**标签**: `#software rendering`, `#computer graphics`, `#GPU rasterization`, `#retro gaming`, `#game development`

---

<a id="item-tech-news-17"></a>
### [GNOME OS 推出面向非开发者的 Preview 版本](https://lwn.net/Articles/1101057/) ⭐️ 6.0/10

GNOME 项目宣布发布 GNOME OS Preview。该版本不再像 Nightly 那样基于最新提交构建，而是基于当前最新稳定版 GNOME 51.1 构建，面向非开发者爱好者。Preview 仅推出数周、实际测试有限，项目方预计初期会暴露出一些问题，但认为它比 Nightly 稳定得多，足以供爱好者日常使用。项目尚未宣称 GNOME OS 已适合大众用户，部分功能仍未实现；愿意在未来稳定版发布后重装系统的用户，现在就可以下载试用。

rss · LWN.net · 10月16日 19:05

**「背景」** 在此之前，GNOME 项目只提供 GNOME OS 的“Nightly”版本，该版本由最新代码提交构建，目标用户是 GNOME 开发者。GNOME OS Preview 则改为基于最新稳定版 GNOME 构建，并明确面向非开发者受众。

**「影响」** 喜欢尝鲜的非开发者现在可以体验比 Nightly 更稳定的 GNOME OS 日常版本，但需要接受初期可能遇到问题，并准备好重新安装系统。由于 Preview 仍缺少一些计划中的功能，追求完整稳定体验的用户应继续等待项目宣布“ready for prime time”的正式版本。

**标签**: `#GNOME`, `#Open Source`, `#Linux`, `#Desktop`, `#Operating Systems`

---

<a id="item-tech-news-18"></a>
### [Linux NFS 服务器近期与未来变化综述](https://lwn.net/Articles/1098611/) ⭐️ 6.0/10

LWN 报道称，在 2026 年 Linux Plumbers Conference 上，NFS 开发者 Jeff Layton 对 Linux NFS 服务器的近期增强进行了综述，并透露了未来实现方向的一些线索。文章目前只概述了会议内容，没有给出具体特性、版本号或时间表，因此尚不能确认任何已落地的改动。

rss · LWN.net · 10月16日 14:26

**「背景」** NFS 是 Unix 类系统上历史悠久的网络文件系统协议，但仍在持续演进，内核实现需要跟上协议变化。本文基于 NFS 开发者 Jeff Layton 在 2026 年 Linux Plumbers Conference 上的演讲，综述 Linux 内核中 NFS 服务器近期已完成的增强以及即将到来的改动。

**标签**: `#Linux`, `#NFS`, `#kernel`, `#filesystems`, `#conference`

---

<a id="item-tech-news-19"></a>
### [Rust 框架 DenseCore 逐位对齐 PyTorch 的 nanoGPT](https://www.reddit.com/r/MachineLearning/comments/1x7ojxo/p_my_rust_framework_trains_nanogpt_with_the_exact/) ⭐️ 6.0/10

计算机科学专业学生作者发布了 DenseCore，一个用 Rust 编写、提供 PyTorch 风格 Python API 的小型深度学习框架。作者声称，在 Apple Silicon Mac 上让 Karpathy 的 nanoGPT 不加修改地运行，50 个训练步骤内的初始权重、损失、梯度和权重都能与 PyTorch 逐位一致，即使开启 dropout 也是如此。该框架体积约 2 MB，而 PyTorch 约 580 MB；但作者也发现，PyTorch 在不同机器上并不总是与自己一致，因此 DenseCore 目前只在 Apple Silicon 上匹配。项目仓库已公开，并附带运行 nanoGPT 对比的演示脚本。

reddit · r/MachineLearning · /u/Mental-Feature-2377 · 10月16日 18:49

**「背景」** nanoGPT 是 Karpathy 发布的一个小型 GPT 训练示例，常用于演示和验证深度学习框架的正确性。PyTorch 是最常用的深度学习框架之一，但其 CPU 实现包含许多非教科书式细节，例如注意力机制使用类似 Flash Attention 的路径、dropout 会切换不同实现，以及 Adam 和梯度裁剪在数值处理上的特殊细节，这些都会影响逐位复现的难度。

**「影响」** 目前该项目的实际影响有限，主要对需要在 Apple Silicon 上复现 PyTorch 数值结果的开发者有参考价值，也为小体积 CPU 场景（如 serverless 或 CI）提供了一个约 2 MB 的轻量候选。不过作者仍在征求方向：是继续兼容 PyTorch，还是做成轻量替代品，或是做成分析 PyTorch 两次运行结果差异的工具，因此现阶段不宜把它当作可用的 PyTorch 替代品。

**标签**: `#rust`, `#deep learning framework`, `#pytorch compatibility`, `#nanogpt`, `#bit-exactness`

---

<a id="item-tech-news-20"></a>
### [可灵 Kling 4.0 全量上线，API 近期开放](https://mp.weixin.qq.com/s/Dn2jAxV0m6kpt7y4edRvdg) ⭐️ 6.0/10

10 月 15 日，可灵 Kling 4.0 正式全量上线 klingai.com，创作页面同步升级，提供更灵活自由的创作体验。本次上线的能力已接入 MCP/CLI，可供开发者直接使用；4K、1080p 的 10-bit HDR 格式输出和面向企业与开发者的 API 服务则属于后续规划，官方称将于近期开放。

telegram · zaihuapd · 10月16日 04:30

**「背景」** 此前 9 月 29 日的 Horizon 日报曾报道，快手宣布 Kling 4.0 将于 10 月正式上线，并已从 9 月 28 日起限量预览 Kling 4.0 Flash 模型；当时预告的能力包括 4K 和 1080p 10-bit HDR 输出、最多 10 张图片、5 段视频和 7 个主体的输入，以及最长 30 秒的视频生成。该报道仍属厂商公布的计划时间线，而非已交付的能力。

**「影响」** 开发者现在可通过 MCP/CLI 将 Kling 4.0 能力接入现有工作流，但在 API 服务正式开放前，生产环境的自动化集成仍需等待官方后续发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.sina.com.cn/stock/t/2026-09-28/doc-initmeau2827369.shtml">2026-09-29 — Kuaishou&#x27;s Kling 4.0 Arrives in October with 4K and HDR Upgrades</a></li>

</ul>
</details>

**标签**: `#AI video generation`, `#Kling 4.0`, `#MCP`, `#API`, `#HDR`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [市场回调与利率上升考验 AI 数据中心交易潮，多宗上市被撤回](https://www.kitco.com/news/off-the-wire/2026-10-15/market-selloff-rising-rates-test-ai-data-centre-deal-boom) ⭐️ 7.0/10

受市场抛售和利率上升影响，过去一周 AirTrunk 的 REIT（房地产投资信托）上市计划、英伟达支持的 Firmus 及软银支持的 SB Energy 的上市安排均被撤回或暂停，投资者要求企业证明能消化升高的利率与算力成本。Dealogic 数据显示，亚洲数据中心并购交易今年已达 213 亿美元，约为 2025 年全年 100 亿美元的两倍，但股权融资同比下降 4.6%。

telegram · zaihuapd · 10月16日 05:10

**「背景」** AirTrunk 原计划在新加坡发行 REIT（房地产投资信托）上市，募资约 15 亿美元；英伟达支持的澳大利亚数据中心运营商 Firmus 则在 10 月 8 日撤回募资额最高 50 亿美元的 IPO，理由包括市场波动导致投资者兴趣不足。软银支持的 SB Energy 的上市安排也被暂停；这些融资原本用于数据中心建设，但在利率上升和算力成本压力下，投资者要求企业先证明能消化这些成本。

**「影响」** 这意味着依赖公开市场融资的数据中心开发商今年面临更紧的股权融资环境；亚洲该行业股权融资已同比下降 4.6%，撤回和暂停上市可能进一步收紧融资窗口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.freemalaysiatoday.com/category/business/2026/09/11/blackstone-s-airtrunk-seeks-us-1-6bil-loan-for-singapore-ipo">Blackstone’s AirTrunk seeks US$1.6bil loan for Singapore IPO | FMT</a></li>
<li><a href="https://au.finance.yahoo.com/news/stock-sinks-23-australia-30bn-034730756.html">A stock sinks 23% as Australia’s $30bn Firmus AI data - centre IPO ...</a></li>

</ul>
</details>

**标签**: `#AI数据中心`, `#IPO撤回`, `#利率上升`, `#并购`, `#资本市场`

---

<a id="item-finance-news-2"></a>
### [商务部拟对 AI、生物医药、光伏相关 40 项技术出口实施临时登记](https://aqygzj.mofcom.gov.cn/flzc/gzjgfxwj/art/2026/art_c99f95ca0cd043829ac9991495fc283c.html) ⭐️ 7.0/10

商务部拟修订《中国禁止出口限制出口技术目录》，对人工智能、生物医药、光伏三个领域的 40 项技术出口实施临时登记，并公开征求意见；该措施目前仍为草案，尚未生效。

telegram · zaihuapd · 10月16日 09:12

**「背景」** 商务部根据《中国禁止出口限制出口技术目录》管理技术出口；此次修订的公开征求意见于 10 月 16 日启动，拟对人工智能、生物医药、光伏三个领域的 40 项技术采取临时出口登记，即相关技术出口前须先向主管部门登记，目前仍属草案阶段。

**「影响」** 若正式实施，中国相关企业向境外出口或授权人工智能、生物医药、光伏技术以及承载这些技术的关键设备时，将需要先办理临时登记或出口许可，从而影响跨境技术转让和设备供应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chinadaily.com.cn/a/202610/16/WS6ad1fcece4b06d4aa05633ae.html">China mulls banning, restricting export of some AI ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/china-proposes-adding-40-ai-biotech-solar-technologies-export-control-list-2026-10-16/">China proposes adding 40 AI, biotech, solar technologies to ...</a></li>
<li><a href="https://www.independent.co.uk/asia/china/china-export-controls-ai-solar-biotech-us-trade-war-b3068046.html">China proposes export controls on AI, solar and biopharma ...</a></li>
<li><a href="https://www.chinadaily.com.cn/a/202610/16/WS6ad1fcece4b06d4aa05633ae.html">China mulls banning, restricting export of some AI ...</a></li>
<li><a href="https://www.wsj.com/economy/trade/china-proposes-export-controls-on-ai-technologies-75ac2030">China Proposes Export Controls on AI Technologies - WSJ</a></li>

</ul>
</details>

**标签**: `#export-controls`, `#artificial-intelligence`, `#biotechnology`, `#photovoltaics`, `#china-regulation`

---

<a id="item-finance-news-3"></a>
### [Anthropic IPO 估值预期下调至 1.5 万亿美元](https://www.reuters.com/business/finance/investors-temper-anthropic-ipo-valuation-expectations-over-revenue-growth-2026-10-15/) ⭐️ 7.0/10

Anthropic 第三季度营收 168 亿美元，环比增长 45%，经调整后盈利并实现季度现金流转正；但部分投资者将其 IPO 估值预期从 2 万亿美元下调至约 1.5 万亿美元，理由是增速放缓、模型价格竞争加剧及算力投入压力。

telegram · zaihuapd · 10月16日 15:46

**「背景」** 此前报道显示，Anthropic 正在筹备上市，联合创始人寻求在 IPO 前获得 50.1% 的投票控制权；其估值在 2026 年从约 9650 亿美元升至 1.5 万亿美元，二级市场报价也一度达到这一水平，但硅谷和华尔街对 IPO 定价的看法已出现分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lteHJYZUVSRTZGVGJVRWRwSnJ5Z0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Anthropic prepares for potential initial public offering ...</a></li>
<li><a href="https://www.bitget.com/news/detail/12560605896083">AI valuation divergence intensifies! Anthropic IPO ... | Bitget News</a></li>
<li><a href="https://techbeat.co/story/anthropic-founders-seek-50-1-voting-control-ahead-of-expected-1-5-trillion-ipo">Anthropic Founders Seek 50.1% Voting Control Ahead of Expected ...</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#IPO估值`, `#AI行业`, `#财报`, `#估值预期`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Anthropic：Claude Mythos 5 可设计出比已发表最佳结果更高效的量子电路](https://x.com/AnthropicAI/status/2111152183240511640) ⭐️ 8.0/10

Anthropic 于 2026 年 10 月 16 日在 X 平台发布推文，介绍其 STEM Fellows Program 的最新成果：让 Claude Mythos 5 根据自然语言指令设计量子电路。推文称，该模型设计的量子电路有时能比已发表的最佳电路提升一个数量级甚至更多；更高效的电路可减少量子算法所需资源，从而可能让化学与材料科学中的量子计算应用更快成为现实。推文为简要公告，并附有“Read more”链接，但未在推文中提供可核实的技术细节或独立验证；上述表述均来自 Anthropic 官方账号的说明。

twitter · AnthropicAI · 10月16日 17:47

**「背景：Claude 设计更高效量子电路」** Anthropic 官方账号于 2026 年 10 月 16 日发布推文，宣布其 STEM Fellows Program 的新成果：使用 Claude Mythos 5 设计更高效的量子电路。推文称，在给出自然语言指令后，Claude Mythos 5 设计出的量子电路可以改进已发表的最佳电路，有时改进幅度达一个数量级或更多；更高效的电路能减少量子算法所需资源，或有助于更快实现化学、材料科学等领域中的量子计算应用。Anthropic 的研究页面进一步说明，这项工作中 Claude 基本自主运行，设计出优于已发表最佳版本的量子电路。第三方媒体 unite.ai 在报道中也指出，Anthropic 于 2026 年 10 月 16 日发布研究文章，称 Claude Mythos 5 在与自动化评估器构成闭环的情况下基本自主工作，设计出优于已发表最佳量子电路的结果。该推文为官方简要预告，并附有研究文章链接，更多技术细节需以完整研究内容为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/designing-efficient-quantum-circuits">Designing more efficient quantum circuits with Claude \ Anthropic</a></li>
<li><a href="https://x.com/AnthropicAI/status/2111152183240511640">Anthropic on X: &quot;New from our STEM Fellows Program: Designing ...</a></li>
<li><a href="https://www.unite.ai/anthropic-says-claude-beat-best-published-quantum-circuit-designs/">Anthropic Says Claude Beat Best Published Quantum Circuit ...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#AI research`, `#Claude`, `#Anthropic`, `#circuit design`

---

<a id="item-twitter-news-2"></a>
### [OpenAI 宣布 GPT-6 Astra Pro 升级：更快响应与并行多智能体任务](https://x.com/OpenAI/status/2111192259073094035) ⭐️ 7.0/10

OpenAI 在官方 X 账号宣布，ChatGPT 中的 GPT-6 Astra Pro 获得升级：响应速度更快，插件和工具的使用能力有所改进。此外，现在多个智能体可以并行处理同一任务的不同部分，用户能够跟踪每个智能体的进度，并打开已完成的任务查看其工作成果。该更新已面向 Pro 用户开放，位于 Chat 标签页中。

twitter · OpenAI · 10月16日 20:27

**「背景」** 这是 OpenAI 在 X（原 Twitter）上发布的官方产品更新，介绍 GPT-6 Astra Pro 在 ChatGPT 中的一次增量升级：响应更快，插件与工具的使用体验更完善，并且新增了多智能体并行处理能力——不同智能体可同时处理任务的各个部分，用户能跟踪每个智能体的进度，并打开已完成的任务查看其工作成果。该功能现已面向 Pro 用户在 Chat 标签页中提供。

在此之前，OpenAI 已于 2026 年 9 月底公布多项相关产品动态：发布由 GPT-6 Astra 驱动的常驻智能体“dots”，覆盖 ChatGPT 网页端、移动端和桌面端，面向 Pro、Business Premium 和 Enterprise 用户\[工具结果 tool-1-1\]；发布 GPT-6.1 Sol，声称以五分之一的价格提供接近 Astra 的智能水平，并称其为当前最具成本效益的模型\[工具结果 tool-1-2\]；推出 Ultrafast 高级速度档位，宣称在 Codex 中最高可将 token 生成速度提升 8 倍，在 API 中最高提升 6 倍\[工具结果 tool-1-3\]。这些动态共同勾勒出 OpenAI 在 GPT-6 系列上围绕性能、成本与智能体能力持续迭代的脉络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/OpenAI/status/2104984504133918973">2026-09-30 — OpenAI Introduces “dots,” Powered by GPT-6 Astra</a></li>
<li><a href="https://x.com/OpenAI/status/2104986129686741046">2026-09-30 — OpenAI Announces GPT-6.1 Sol with Cost-Efficiency Claims</a></li>
<li><a href="https://x.com/OpenAI/status/2104993966043320759">2026-09-30 — OpenAI announces Ultrafast premium speed tier</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6 Astra Pro`, `#AI product update`, `#multi-agent`, `#ChatGPT`

---