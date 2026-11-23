---
layout: default
title: "Horizon Summary: 2026-11-23 (ZH)"
date: 2026-11-23
lang: zh
---

> 从 61 条内容中筛选出 18 条重要资讯。

---

**科技新闻**
1. [OpenAI 讨论困惑度与模型智能的关系](#item-tech-news-1) ⭐️ 7.0/10
2. [硅谷反思：机制设计与 AI 目标](#item-tech-news-2) ⭐️ 7.0/10
3. [Anthropic 2028 年电力结构预测：天然气 87%、煤炭 11%](#item-tech-news-3) ⭐️ 7.0/10
4. [英媒指英伟达芯片经柬埔寨相关网络流入中国](#item-tech-news-4) ⭐️ 7.0/10

**科技博客**
1. [不确定时，不妨主动“乱撞”](#item-tech-blog-1) ⭐️ 6.0/10

**AI 开源项目**
1. [LMCache v0.5.8 发布：强化多进程 KV 缓存与生产可用性](#item-ai-projects-1) ⭐️ 8.0/10
2. [LMCache v0.5.8 发布 ROCm 7.2 预编译 wheel，适配 AMD Instinct](#item-ai-projects-2) ⭐️ 7.0/10
3. [LMCache v0.5.8 Intel XPU 平台轮子发布](#item-ai-projects-3) ⭐️ 6.0/10
4. [LMCache v0.5.8-rbln：面向 Rebellions RBLN NPU 的专用发行版](#item-ai-projects-4) ⭐️ 6.0/10
5. [LMCache 发布 ROCm 7.2 nightly 构建](#item-ai-projects-5) ⭐️ 5.0/10
6. [LMCache 发布面向 Rebellions RBLN NPU 的 nightly 构建](#item-ai-projects-6) ⭐️ 5.0/10
7. [LMCache 发布 nightly 构建：CUDA 13.0 wheel（linux/amd64 与 linux/arm64）](#item-ai-projects-7) ⭐️ 5.0/10
8. [LMCache v0.5.8 ROCm 预编译 Wheel 发布](#item-ai-projects-8) ⭐️ 5.0/10

**财经新闻**
1. [美股科技股暴跌，亚洲多市场出台应急交易措施](#item-finance-news-1) ⭐️ 9.0/10
2. [中国要求美国撤销 FCC 电话号段接入限制](#item-finance-news-2) ⭐️ 7.0/10
3. [超级厄尔尼诺海温创纪录，世界粮食计划署警告或新增 4900 万急性粮食不安全人口](#item-finance-news-3) ⭐️ 7.0/10

**推特新闻**
1. [Agent 说“验证完了”，怎样才真的可信？](#item-twitter-news-1) ⭐️ 7.0/10
2. [东锡 NLP：从困惑度曲线读出 OpenAI 训练范式由预训练转向后训练](#item-twitter-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 讨论困惑度与模型智能的关系](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 7.0/10

OpenAI 刊出一篇题为《Perplexity and Intelligence》的文章，讨论语言模型的困惑度（perplexity）与智能之间的关系。提供的源内容为空，因此文章的具体论证、数据和结论无法核实；现有讨论主要围绕困惑度作为交叉熵指标的定义、其与模型能力的对应关系，以及“能力在特定困惑度上涌现”的说法是否成立。

hackernews · acossta · 11月22日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=50601525)

**「背景：困惑度是什么」** 困惑度（perplexity）是语言模型预训练目标交叉熵损失的指数形式，用来衡量模型预测序列中下一个 token 时的“惊讶”程度：如果模型对每个 token 都给出概率 1，困惑度就是 1；如果模型完全随机预测，困惑度则接近词表大小，因此数值越低越好。OpenAI 首席科学家 Jakub Pachocki 在 11 月 22 日发布的这篇文章属于立场性论述，而非新模型或新工具的发布；他主张把困惑度（等价地，交叉熵损失）作为模型开发者之间可横向比较的指标，并以此支撑共同的安全标准。

**「影响」** 对使用困惑度评估模型的开发者来说，不能把单一交叉熵或困惑度数值直接当作跨任务能力的证据；在数学等专门任务上，训练数据分布不同，模型表现可能无法由通用困惑度反映。

**「社区讨论」** 评论中，hazrmard 补充了困惑度的定义：它衡量模型对下一 token 的“惊讶”程度，最好为 1、最差为词表大小；d\_burfoot 则认为预测或压缩率与智能的对应关系在逻辑上成立。tensor 对“特定能力在给定困惑度上涌现”的说法表示怀疑，指出专门训练数学的小模型在其他任务上的通用困惑度可能更高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#perplexity`, `#language models`, `#cross-entropy`, `#AI benchmarks`, `#OpenAI`

---

<a id="item-tech-news-2"></a>
### [硅谷反思：机制设计与 AI 目标](https://www.oreilly.com/radar/what-happened-to-silicon-valley/) ⭐️ 7.0/10

O&\#x27;Reilly Radar 刊出一篇反思硅谷演变的长文，面向科技从业者讨论资本主义、激励机制设计以及行业向 AI 的转向；它不是产品发布或技术突破，而是评论文章。文章的核心主张是：与其只接受当前市场游戏的规则，不如用“逆向博弈论”式的机制设计追问“我们应当玩什么游戏”，并把“人类繁荣”作为优化目标。这个框架把讨论从单纯的技术或公司成败，转到谁在设计激励、系统实际奖励什么，以及 AI 时代这些目标是否需要重新设定。

hackernews · greenyouse · 11月22日 19:20 · [社区讨论](https://news.ycombinator.com/item?id=50602947)

**「背景：机制设计视角」** 这场论述源自 Tim O&\#x27;Reilly 2026 年 10 月 16 日在约翰斯·霍普金斯大学的一次演讲，他把硅谷的发展轨迹描述为从以客户为中心的创新转向由股东资本主义、垄断野心和炒作驱动的“榨取”。其分析框架是机制设计，即他所说的“逆向博弈论”：与其接受现有游戏规则，不如追问“我们本应该玩什么游戏”，因为技术的价值取决于围绕它的规则、激励与接口设计。

**「社区讨论」** HN 评论围绕“机制设计”展开：有人认同资本主义是被设定目标的优化机器，主张让机制设计者对结果负责，并把目标改为人类繁荣；也有人把当前局面归因于 ZIRP 时代催生的过度扩张，质疑利率回归后市场是否会约束科技公司借 AI 进行的鲁莽支出。另有评论批评“VC 网红”文化，认为硅谷的诚信比过去更稀薄。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.oreilly.com/radar/what-happened-to-silicon-valley/">What Happened to Silicon Valley? – O’Reilly</a></li>
<li><a href="https://oreillyradar.substack.com/p/what-happened-to-silicon-valley">What Happened to Silicon Valley? - oreillyradar.substack.com</a></li>
<li><a href="https://news.lavx.hu/article/tim-o-reilly-traces-silicon-valley-s-shift-from-value-creation-to-extraction">Tim O&#x27;Reilly Traces Silicon Valley&#x27;s Shift From Value ...</a></li>

</ul>
</details>

**标签**: `#Silicon Valley`, `#tech industry`, `#mechanism design`, `#venture capital`, `#AI`

---

<a id="item-tech-news-3"></a>
### [Anthropic 2028 年电力结构预测：天然气 87%、煤炭 11%](https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/) ⭐️ 7.0/10

Better Data Center Project 的一篇分析预测，到 2028 年 Anthropic 的电力结构中约 87%来自天然气、11%来自煤炭，并讨论了 AI 数据中心用电带来的环境成本。该结果是分析性预测，并非已确认的运营数据；现有材料没有交代预测方法、地理范围或是否计入备用电源等条件。

hackernews · happosai · 11月22日 08:57 · [社区讨论](https://news.ycombinator.com/item?id=50597612)

**「背景」** Colossus 是 xAI 在孟菲斯—南哈文地区建设的数据中心集群；Anthropic 于 2026 年 5 月宣布与 xAI 母公司 SpaceX 达成协议，使用 Colossus 1 的全部算力。2026 年 8 月的一篇调查报道称，Anthropic 未直接回应孟菲斯居民对污染和水使用的担忧，尽管其在当年 6 月加入了资助碳移除技术的 Frontier 联盟。

**「影响」** 该分析预测，Anthropic 在 2028 年的算力用电将有 87% 来自天然气、11% 来自煤电。对采购其模型服务的企业而言，若要把 AI 工作负载纳入低碳采购或排放核算，这种电力结构意味着需要额外购买绿电、进行抵消，或在供应商选择上作替代安排。

**「社区讨论」** 有评论者批评 Anthropic 在孟菲斯租用 Colossus 1 造成当地污染，且未在美国作出可再生能源承诺，并主张用监管把环境外部性内部化。另有评论者强调 AI 数据中心的能耗规模难以直观想象，并提到美国页岩油伴生天然气常被放空燃烧的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_%28data_center%29">Colossus (data center) - Wikipedia</a></li>
<li><a href="https://www.eenews.net/articles/anthropic-moves-into-musks-memphis-data-center/">Anthropic moves into Musk’s Memphis data center</a></li>
<li><a href="https://www.thebureauinvestigates.com/stories/2026-08-14/misaligned-colossus-musks-data-empire-anthropic">How Musk’s toxic data empire is powering Anthropic’s ...</a></li>
<li><a href="https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/">How AI is powered : a breakdown of BYOP and grid power</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#energy`, `#sustainability`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [英媒指英伟达芯片经柬埔寨相关网络流入中国](https://www.ft.com/content/f3ad8a81-3890-4a8a-8853-ff0a94b08ba9?syn-25a6b1a6=1) ⭐️ 7.0/10

英国《金融时报》援引知情人士称，被美国财政部指为柬埔寨太子集团“二号人物”的胡小伟涉嫌参与将英伟达芯片运入中国，相关网络涉及空壳公司、地下融资和私人飞机运输。该报援引的贸易数据显示，2024 年 12 月至 2025 年 12 月，Megaspeed 马来西亚子公司进口货物申报价值约 46 亿美元，部分芯片据称流入中国黑市。太子集团否认胡小伟曾为其工作，并称有关非法网络和私人飞机走私的指控缺乏事实依据。

telegram · zaihuapd · 11月22日 04:34

**「背景」** 美国商务部与司法部 2026 年 11 月 16 日曾发表联合声明，说明对新加坡公司 Megaspeed 的出口管制与刑事调查时间线：商务部于 2024 年立案，2025 年 5 月要求英伟达提供对 Megaspeed 的销售记录，同年 6 月英伟达将该公司列入禁售名单。另据《纽约时报》报道，中方相关小组承担“反封锁”工作，其中包括帮助中国企业获取并走私先进芯片，以绕开美国及其盟友的出口管制。

**「影响」** 对涉及第三地转口的芯片交易而言，这一报道的直接影响是最终用途与进口申报将受到更严格审视；但相关走私规模和流向目前仍为《金融时报》援引的未证实指控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.commerce.gov/sites/default/files/2026-11/DOC-DOJ-Joint-Statement.pdf">2026-11-18 — US Commerce and DOJ issue joint statement on Megaspeed export-control investigation</a></li>
<li><a href="https://www.nytimes.com/2026/11/21/world/asia/china-nvidia-spy-chips-state-security.html">China’s Spies Set Sights on A.I. Chips Years Before Nvidia Scandal</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#chip smuggling`, `#export controls`, `#semiconductor supply chain`, `#Cambodia`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [不确定时，不妨主动“乱撞”](https://seangoedecke.com/when-in-doubt-flail-about/) ⭐️ 6.0/10

rss · Sean Goedecke · 11月23日 00:00

**「背景」** 当工作缺乏明确指引，或系统复杂到不知从何改起时，谨慎等待、先彻底理解往往并不可行。作者提出，此时更有效的做法是有反馈意识地“乱撞”（flail）：主动尝试，而不是把不确定误当成需要更多分析的信号。

**「方案」** 作者把“乱撞”拆成三条原则：大量尝试不同方案、密切观察来自人和现实的反馈、毫不留情地砍掉没有正反馈的方案。因为不确定时多数想法注定平庸，只有尝试足够多才可能撞上有效方向，也才不会对单一计划过度投入。产品上，他在 GitHub Models 做过多个不成功的功能，但“用 GitHub Actions token 运行 AI 推理”意外受欢迎，后来成为 Continuous AI 的种子；工程上，面对过于庞大纠缠的系统，他不建议先通读全貌，而是做若干试探性改动，有效再深挖；组织上，面对团队不沟通或主管部门说不清的问题，可以自动化杂活、主动接手、提出长期方案，但此时最需要对反馈敏感，失败计划不立刻放弃会把不满引向自己。作者提醒，这样做有损害声誉的风险，且从内部感受像反复失败；但若及时止损，上级看到的会是主动实验的工程师。

**「启示」** 作者的核心论点是：在高度不确定的情境中，带反馈的“乱撞”比等到完全理解后再行动更快，也更容易找到真正有牵引力的方向。其更大意义在于，有效工程师需要穿过“自己像在瞎折腾”的心理不适，把及时放弃失败方案当作一种可训练的判断力。

**标签**: `#engineering judgment`, `#experimentation`, `#feedback loops`, `#organizational dynamics`, `#uncertainty`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [LMCache v0.5.8 发布：强化多进程 KV 缓存与生产可用性](https://github.com/LMCache/LMCache/releases/tag/v0.5.8) ⭐️ 8.0/10

LMCache v0.5.8 升级多进程缓存架构、KV 缓存一致性、RDMA 点对点传输、推理服务兼容性与安全边界，目标是让 LLM 推理缓存更模块化、更可靠、更接近生产可用。

github · travisVux · 11月22日 15:39

**「解决的痛点」** LLM 推理缓存需在多进程、多请求、模型修订、LoRA 适配器和张量并行副本间复用；缓存身份不一致会造成错误命中或重复存储，旧的多进程实现和阻塞式通信也会影响服务稳定性。v0.5.8 通过重构共享客户端与传输边界、强化缓存身份、扩展 RDMA 传输，并为 gRPC/ZMQ 增加 API Key 认证和默认回环绑定，降低误用与运维风险。

**「背景与影响」** LMCache 是面向 LLM 推理的模块化 KV cache 管理层，目标是在 GPU、CPU 内存及磁盘/远程后端之间组织多级缓存，让长提示、对话历史和检索内容对应的 KV cache 可被跨请求、跨服务引擎复用 \[tool-1-1\]\[tool-1-2\]\[tool-1-3\]。在这一背景下，v0.5.8 属于一次面向生产环境的增量强化：发布说明显示其重点围绕多进程架构重构、跨请求/模型版本/LoRA/张量并行驻留的缓存身份一致性、RDMA 点对点传输，以及 vLLM、SGLang 等 serving 兼容性和 gRPC/ZMQ 安全边界展开。它并非基础性突破，而是针对分布式推理缓存运行时在可靠性、可运维性和部署兼容性上的持续补强。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li><a href="https://docs.lmcache.ai/developer_guide/architecture.html">Architecture Overview | LMCache</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**标签**: `#LLM`, `#KV cache`, `#inference`, `#distributed`, `#RDMA`, `#serving`, `#multiprocess`, `#CUDA`, `#security`

---

<a id="item-ai-projects-2"></a>
### [LMCache v0.5.8 发布 ROCm 7.2 预编译 wheel，适配 AMD Instinct](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rocm) ⭐️ 7.0/10

LMCache 发布 v0.5.8 的 ROCm 7.2 预编译 wheel，面向 AMD Instinct gfx942（MI300X/MI325X）与 gfx950（MI350X/MI355X），并与上游 vLLM ROCm 镜像（torch 2.13、cp312）保持 ABI 匹配。

github · github-actions\[bot\] · 11月22日 17:35

**「解决的痛点」** 在 AMD ROCm 环境里部署 LMCache 时，用户往往需要自行从源码编译，或面对 wheel 与 vLLM 容器之间 Python 版本（cp312）、PyTorch 版本（torch 2.13）不一致导致的 ABI 不兼容问题。该版本提供与上游 vllm/vllm-openai-rocm 镜像对齐的预编译包，可通过 pip 直接装入容器，减少编译与依赖排查成本，降低因二进制不匹配引发的运行期故障风险。

**「生态定位与发布意义」** LMCache 处在 vLLM 服务栈的 KV 缓存层：vLLM 自带的 prefix caching 只在单节点内复用 KV 状态，而 LMCache 在其上叠加分布式缓存层，让不同机器上的多个 vLLM worker 通过以太网、RDMA 或 NVLink 共享同一份 KV 缓存，从而消除多副本集群中重复的 prefill 计算（tool-1-2）。它也能以 MP 模式脱离 vLLM 独立运行，实现缓存层自身的独立扩缩容（tool-1-1）；接入成本被官方作为卖点，曾以“改一行代码”来宣传可显著扩大可用 KV 缓存空间（tool-1-3）。

放到这个背景下，v0.5.8-rocm 的价值主要是平台可用性而非架构演进：它把 v0.5.8 这一版本以 ROCm 7.2 wheel 的形式带到 AMD Instinct gfx942（MI300X/MI325X）与 gfx950（MI350X/MI355X），并与上游 \`vllm/vllm-openai-rocm\` 镜像做 ABI 对齐（torch 2.13、cp312），使使用者可以直接把预编译包 \`--no-deps\` 装进上游 vLLM ROCm 容器，而不必自行针对该平台编译。对在 AMD 加速卡上跑 KV 缓存共享/多副本推理的团队来说，这降低的是部署摩擦；就项目本身而言，它仍是一次打包与硬件适配发布，未涉及核心机制变更。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for... | DataCamp</a></li>
<li><a href="https://www.spheron.network/blog/deploy-lmcache-vllm-kv-cache-sharing-gpu-cloud/">Deploy LMCache on GPU Cloud: Share KV Cache Across vLLM ...</a></li>
<li><a href="https://blog.lmcache.ai/2024-09-23-pip-install/">Are you a vLLM user? Change just ONE line of code to unlock...</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#ROCm`, `#vLLM`, `#KV cache`, `#AMD Instinct`, `#wheel`, `#inference serving`

---

<a id="item-ai-projects-3"></a>
### [LMCache v0.5.8 Intel XPU 平台轮子发布](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-xpu) ⭐️ 6.0/10

LMCache v0.5.8 的 Intel XPU/SYCL 平台轮子，面向 Intel vLLM XPU 容器分发现有 KV-cache 库，基于固定版本的 torch-xpu 与 oneAPI 工具链构建，未引入新的核心功能或架构变更。

github · github-actions\[bot\] · 11月22日 17:35

**「解决的痛点」** 它主要降低 Intel XPU 环境下的分发与安装门槛：用户无需自行从源码编译，可直接在上游 Intel vLLM XPU 容器中通过指定 wheel 源安装预构建包；运行时仍需绑定宿主机的 oneAPI/SYCL 库。该发布属于平台适配，未提供性能数据或功能增强。

**「背景与影响」** 该版本属于平台适配型发布：LMCache 将既有的 KV 缓存能力以 Intel XPU/SYCL wheel 形式提供给 Intel vLLM XPU 容器，构建时固定 torch-xpu 与 oneAPI 工具链，运行时依赖宿主机的 oneAPI/SYCL 库。它没有引入新的核心功能、架构或性能数据，主要意义是把 KV 缓存复用与卸载层扩展到 Intel 硬件生态。vLLM 文档已将 LMCache 列为 KV connector 之一，但部分 KV 缓存配置与连接器存在兼容限制；Intel llm-scaler 的 vLLM 文档也包含启动 LMCache 的流程，说明这一打包面向已有的 Intel 推理服务集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/configuration/optimization/">Optimization and Tuning - vLLM</a></li>
<li><a href="https://github.com/intel/llm-scaler/blob/main/vllm/README.md">llm-scaler/ vllm /README.md at main · intel /llm-scaler · GitHub</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#Intel XPU`, `#SYCL`, `#vLLM`, `#inference serving`, `#packaging`, `#release`

---

<a id="item-ai-projects-4"></a>
### [LMCache v0.5.8-rbln：面向 Rebellions RBLN NPU 的专用发行版](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rbln) ⭐️ 6.0/10

LMCache 发布 v0.5.8-rbln 平台专用 wheel，面向 Rebellions RBLN NPU，基于 torch-rbln 0.12.0（torch 2.13.0+cpu）构建，用于在已有 RBLN 软件栈的环境中安装 LMCache v0.5.8。

github · github-actions\[bot\] · 11月22日 17:35

**「解决的痛点」** 它解决的是在 Rebellions RBLN NPU 环境中安装 LMCache 的适配问题：提供针对 torch-rbln 0.12.0 构建的专用 wheel，并避免打包由宿主环境管理的 torch-rbln、rebel-compiler 和 RBLN 驱动，从而减少依赖冲突和部署负担。

**「背景与影响」** LMCache 在 LLM 推理栈中的定位是 KV 缓存层：通过复用重复文本（不限于前缀）的 KV 状态，减少重复 prefill 计算、降低首 token 时延，并把缓存铺到 GPU 显存之外的多级存储中（工具结果 tool-1-2、tool-1-3）。其公开材料也强调面向网络与存储的 KV 缓存扩展（tool-1-1）。这意味着它的部署形态长期围绕 GPU 生态展开。

本次 v0.5.8-rbln 的意义在于把这条缓存路径延伸到非 NVIDIA 加速器：发布的是面向 Rebellions RBLN NPU 的平台专用 wheel，基于 torch-rbln 0.12.0（torch 2.13.0+cpu）构建。对使用 Rebellions 硬件的团队而言，这是一个可直接 pip 安装的接入方式，而不必自行从源码适配。

打包策略同样值得注意：torch-rbln、rebel-compiler 与 RBLN 驱动保持由宿主机持有、不随 wheel 一起分发，安装前需环境中已具备 torch-rbln 和 rebel-compiler。这样做避免了与厂商侧运行时/编译器版本产生冲突，但也把环境准备的责任留给部署方。

需要说明的是，随附内容未显示核心架构改动、性能数据或重大功能变化，因此这是一次以分发与硬件覆盖为主的更新，而非能力层面的跃迁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=rINy7mFyRAU">Introducing LMCache - YouTube</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for... | DataCamp</a></li>
<li><a href="https://github.com/neeltom92/lmcache">neeltom92/ lmcache : Supercharge Your LLM with the Fastest KV ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#KV cache`, `#inference`, `#NPU`, `#Rebellions`, `#release`, `#hardware acceleration`

---

<a id="item-ai-projects-5"></a>
### [LMCache 发布 ROCm 7.2 nightly 构建](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

LMCache 发布面向 ROCm 7.2 的 nightly wheel，支持 AMD Instinct gfx942/gfx950，由 dev 分支构建，并与上游 vLLM ROCm 容器（torch 2.13、cp312）ABI 匹配。

github · github-actions\[bot\] · 11月22日 07:45

**「解决的痛点」** 解决 AMD ROCm 平台上部署 LMCache 的兼容与打包问题：提供预编译 wheel，并与 vLLM ROCm 镜像的 ABI 对齐，减少用户从源码编译、处理依赖和版本不匹配的成本。LMCache 本身用于 LLM 服务中的 KV 缓存复用与显存压力缓解，但该发布是例行 nightly 构建，未声明性能提升。

**「背景与影响」** LMCache 的定位是 LLM 推理中的 KV 缓存层：把 KV tensor 从 GPU 显存卸载到分层存储，并在 vLLM 等推理框架中复用，减少重复 prefill。此前其主要部署路径围绕 NVIDIA 生态，ROCm 版本以 nightly 形式从 \`dev\` 分支构建，属于打包与 CI 产物而非功能发布——本次发布本身没有给出任何性能或能力声明，可确认的事实仅限于平台与 ABI 兼容性（gfx942/gfx950、torch 2.13、cp312，对齐 \`vllm/vllm-openai-rocm\` 镜像）。

放到更大的图景看，这是 AMD 推理栈逐步补齐的一环。AMD 官方博客称，LMCache 与 vLLM 集成后在 MI300X 上对 Qwen3、Llama3、Qwen-VL 等社区模型带来 3–10x 提升，并降低长文档问答、多轮问答等场景的 GPU 周期消耗（tool-1-1）；AMD 同期还推出了面向 Instinct GPU 的解耦式 KV cache 推理栈 ROCm AIC，从 MI300X/MI350 系列起步并延伸至 MI450/Helios 平台（tool-1-3）。在这样的生态中，持续产出与上游 vLLM ROCm 容器 ABI 对齐的 wheel，意味着 AMD 用户可以用一条 pip 命令获得与 NVIDIA 路径对等的 KV 缓存能力，而不必自行编译；但 nightly 标签也说明其稳定性与验证程度低于正式版本，且缺少社区反馈可供参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.lmcache.ai/en/2026/01/09/amd-x-lmcache-amd-gpu-acceleration-with-lmcache/">AMD × LMcache: AMD GPU Acceleration with LMcache</a></li>
<li><a href="https://rocm.blogs.amd.com/software-tools-optimization/amd-infinity-context/README.html">Introducing ROCm™ AMD Infinity Context: A Purpose-Built KV ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#KV cache`, `#serving`, `#vLLM`, `#ROCm`, `#AMD Instinct`, `#nightly build`, `#packaging`

---

<a id="item-ai-projects-6"></a>
### [LMCache 发布面向 Rebellions RBLN NPU 的 nightly 构建](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

LMCache 发布 nightly 版 RBLN NPU wheel，基于 dev 分支构建，面向 torch-rbln 0.12.0（torch 2.13.0+cpu），用于在 Rebellions RBLN 环境安装 LMCache。

github · github-actions\[bot\] · 11月22日 07:39

**「解决的痛点」** 该构建提供平台专用的预编译 wheel，减少用户在 RBLN NPU 环境中从源码打包 LMCache 的步骤。它将 torch-rbln、rebel-compiler 和 RBLN 驱动保留为宿主机自有依赖，不随 wheel 捆绑，需在已具备这些依赖的环境中安装。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV cache 管理层，把原本临时的 KV cache 变成可持久化、可跨多个服务引擎复用的“AI 原生知识”，并在 GPU 显存、CPU 内存与磁盘/远程后端之间做多级缓存调度（tool-1-1、tool-1-2、tool-1-3）。本次 nightly-rbln 属于平台适配型打包产物：它把 LMCache 的 wheel 构建到 Rebellions RBLN NPU 生态上，对应 torch-rbln 0.12.0（torch 2.13.0+cpu）。torch-rbln 是让 PyTorch 自然调用 Rebellions NPU 算力的扩展，而 rebel-compiler 需要单独从 RBLN 包索引安装、并不随 torch-rbln 一起提供（tool-2-1、tool-2-3），因此该 wheel 明确将 torch-rbln、rebel-compiler 与 RBLN 驱动保留为宿主机自有依赖、不打入包内。其意义在于让 LMCache 的 KV cache 分层能力从 GPU 进一步覆盖到非 GPU 的 NPU 推理硬件；但源内容未描述任何功能、性能或架构层面的变更，应视为常规夜间构建而非特性发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li><a href="https://docs.lmcache.ai/developer_guide/architecture.html">Architecture Overview | LMCache</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch - rbln · PyPI</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">RBLN -SW/ torch - rbln : PyTorch extension for Rebellions NPU · GitHub</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly build`, `#packaging`, `#torch-rbln`

---

<a id="item-ai-projects-7"></a>
### [LMCache 发布 nightly 构建：CUDA 13.0 wheel（linux/amd64 与 linux/arm64）](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布 nightly 版本，提供由 \`dev\` 分支构建、面向 CUDA 13.0 的预编译 wheel，覆盖 linux/amd64 与 linux/arm64 两个平台，可通过 \`uv pip install lmcache --pre\` 配合 PyTorch cu130 索引安装。

github · github-actions\[bot\] · 11月22日 09:28

**「解决的痛点」** 对使用 CUDA 13.0 环境的团队来说，稳定版渠道未必提供对应 CUDA 版本与 CPU 架构的预编译包，往往需要自行从源码编译，耗时且容易在依赖和工具链上出错。该 nightly 直接给出 amd64 与 arm64 的现成 wheel，并说明需搭配 \`--extra-index-url https://download.pytorch.org/whl/cu130\`、\`--find-links\` 指向该 release 资源页以及 \`--index-strategy unsafe-best-match\` 才能正确解析依赖，降低了在新 CUDA 环境（尤其是 arm64 服务器）上试用 LMCache 的安装门槛。

需要注意，这是 \`--pre\` 渠道的 dev 构建，源内容未列出任何功能变更、性能数据或稳定性保证，因此更适合作为验证与尝鲜用途，而非生产默认选择。

**「背景与生态位置」** LMCache 是面向 LLM 推理的 KV cache 管理层，目标是在多个推理 worker 之间复用缓存的 KV 状态，并将缓存扩展到 GPU、CPU DRAM 和本地磁盘，而不是绑定在单一模型进程内（tool-1-1、tool-1-2、tool-1-3）。这次 nightly 没有披露功能或性能变化，核心信息是从 dev 分支构建的 CUDA 13.0 轮子覆盖 linux/amd64 与 linux/arm64；安装命令使用 PyTorch 的 cu130 索引，表明该构建面向 CUDA 13 软件栈。对生态而言，这是持续集成与打包层面的跟进，便于开发者在 CUDA 13 环境试用最新代码；nightly 的稳定性与具体改动仍需以实际测试为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/a0x8o/lmcache">GitHub - a0x8o/ lmcache : LMCache : Supercharge Your LLM with the...</a></li>
<li><a href="https://landscape.jimmysong.io/projects/lmcache/">LMCache | AI Native Landscape</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#LLM inference`, `#KV cache`, `#CUDA`, `#nightly release`, `#packaging`

---

<a id="item-ai-projects-8"></a>
### [LMCache v0.5.8 ROCm 预编译 Wheel 发布](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rocm-torch210) ⭐️ 5.0/10

这是 LMCache v0.5.8 的 AMD ROCm 预编译 wheel，在 rocm/pytorch 容器（ROCm 7.2.4 + torch 2.10.0）中构建并测试，锁定精确的 torch/ROCm ABI，方便 AMD GPU 用户直接 pip 安装，无需从源码编译。

github · github-actions\[bot\] · 11月22日 17:35

**「解决的痛点」** LMCache 包含需要编译的 C++/HIP 扩展，在 AMD 平台上从源码安装时必须让 ROCm 版本、torch 的 ROCm 构建、Python 版本和 C++ ABI 完全对齐；稍有偏差就会出现 ABI 不匹配、链接失败或运行时崩溃。这个 wheel 固定了整条工具链（ROCm 7.2.4、torch 2.10.0+rocm7.2.4.git3d3aa833、cp312-cp312-manylinux\_2\_39\_x86\_64、\_GLIBCXX\_USE\_CXX11\_ABI=1，并包含 gfx942/gfx950 代码对象），用户只需在匹配的容器里用一条带 --no-deps 的 pip 命令安装即可，从而把“环境拼装 + 编译排错”换成确定性的二进制分发。代价是适用范围极窄：只有 ABI 精确吻合的环境才可用。

**「背景与影响」** 这次发布不是功能更新，而是既有 LMCache v0.5.8 的 AMD ROCm 预编译 wheel：把构建/测试环境钉在 \`rocm/pytorch:rocm7.2.4\_ubuntu24.04\_py3.12\_pytorch\_release\_2.10.0\`（digest \`sha256:4449...179e\`），并给出精确 ABI 组合——torch \`2.10.0+rocm7.2.4.git3d3aa833\`、ROCm \`7.2.4\`（HIP \`7.2.53211\`）、\`cp312-cp312-manylinux\_2\_39\_x86\_64\`、\`\_GLIBCXX\_USE\_CXX11\_ABI=1\`，内含 gfx942/gfx950 的 GPU code object。核心增量是“AMD 上可 pip 直装”，而非新特性或性能提升。

放到更大的推理栈里看，KV cache 复用层长期以 CUDA 为主路径。LMCache 的思路是缓存所有可复用文本的 KV，从而跨请求、甚至跨 vLLM 实例复用（社区仓库 LMCache-ROCm 描述了用 lmcache.server 模块共享 KV 的方式，见 tool-1-3）。AMD 侧本已有 vLLM 的 ROCm 安装路径（tool-1-2），并出现过 MI300X 上 vLLM + LMCache、走 ROCm 与 LMCacheConnector V1 的长文档与多轮 QA 基准（tool-1-1）。因此这个 wheel 的实际意义是补齐 LMCache 接入 AMD 推理栈的最后一段——构建与 ABI 对齐——把“能不能装”的问题前置解决，降低 AMD GPU 上的部署门槛。

边界需保留：源内容只说明打包与 ABI 细节，未给出性能数字或新功能；“包含对应版本全部集成”的说法来自发布说明本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/upto-107x-speedup-llm-inference-lmcache-rohan-paul-ibxkf">Upto 10.7X speedup on LLM inference with LMCache</a></li>
<li><a href="https://docs.vllm.ai/en/latest/getting_started/installation/gpu/">GPU - vLLM</a></li>
<li><a href="https://github.com/EmbeddedLLM/LMCache-ROCm">GitHub - EmbeddedLLM/ LMCache - ROCm : ROCm support of...</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#ROCm`, `#AMD GPU`, `#release packaging`, `#wheel`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美股科技股暴跌，亚洲多市场出台应急交易措施](https://news.bjd.com.cn/2026/11/22/12039852.shtml) ⭐️ 9.0/10

周五美国 AI 科技股遭大规模抛售，纳斯达克指数单日下跌 5.28%，费城半导体指数重挫近 11%。亚洲多个市场随即推出应急措施，其中中国台湾地区自 11 月 23 日起全面禁止平盘以下卖空，中国内地则将融资保证金最低比例下调至 80%。

telegram · zaihuapd · 11月22日 13:24

**「背景」** 11 月 20 日，对人工智能投资热潮放缓的担忧已在华尔街引发抛售，纳斯达克 100 指数单日下跌 5.6%，费城半导体指数较 6 月高点累计下跌 43%，这轮以科技股为主的回撤随后波及亚洲市场。

**「影响」** 对中国台湾地区投资者而言，平盘以下禁止卖空和融券保证金比例由 130%上调至 150%，将直接提高做空成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guancha.cn/GuoJi%C2%B7ZhanLue/2026_11_21_909399.shtml">AI 恐慌爆发，华尔街震荡，美国 科 技 股 跌 入熊市</a></li>

</ul>
</details>

**标签**: `#US tech stocks`, `#market disruption`, `#Asian markets`, `#regulatory response`, `#short-selling rules`

---

<a id="item-finance-news-2"></a>
### [中国要求美国撤销 FCC 电话号段接入限制](https://www.bloomberg.com/news/articles/2026-11-22/china-objects-to-us-curbs-on-telecoms-access-to-phone-numbers) ⭐️ 7.0/10

中国商务部 11 月 22 日敦促美国撤销一项限制中国移动、中国电信和中国联通直接接入美国电话号码的措施；美国联邦通信委员会（FCC）在 11 月 19 日投票收紧互联网语音服务商的安全认证，以阻止其“Covered List”上的实体、设备和服务接入美国网络。商务部称该措施违反非歧视与公平竞争原则、缺乏事实依据，并警告将采取必要行动。

telegram · zaihuapd · 11月22日 06:44

**「背景」** 美国电话号码的接入授权由联邦通信委员会（FCC）管理，互联网语音服务商（VoIP）须获授权才能直接取得号码资源。FCC 在 11 月 19 日通过的规则中，在这一授权框架上加入国家安全认证，以阻止“涵盖清单”（Covered List，即美方认定构成国家安全风险的设备和服务名单）上的实体、设备或服务接入美国网络。

**「影响」** 该措施直接限制中国移动、中国电信和中国联通直接接入美国电话号段的业务，并使中美跨境电信互联新增一道安全认证合规门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fcc.gov/document/fcc-cracks-down-bad-actors-access-us-phone-numbers-0">FCC Cracks Down on Bad Actors&#x27; Access to U.S. Phone Numbers</a></li>
<li><a href="https://fccid.io/news/fcc-voip-direct-number-access-covered-list-certifications-fcc-26-82">FCC 26-82: New National Security Rules for VoIP Number Access</a></li>
<li><a href="https://www.globaltimes.cn/page/202611/1374802.shtml">China urges US to revoke proposed telecom restrictions , warns of...</a></li>
<li><a href="https://www.foxbusiness.com/politics/fcc-bans-chinese-firms-direct-access-us-phone-numbers-bid-curb-robocalls">FCC regulators bar Chinese telecom giants from direct number access</a></li>

</ul>
</details>

**标签**: `#美中关系`, `#电信监管`, `#FCC`, `#中国商务部`, `#国家安全`

---

<a id="item-finance-news-3"></a>
### [超级厄尔尼诺海温创纪录，世界粮食计划署警告或新增 4900 万急性粮食不安全人口](https://www.wired.com/story/how-this-years-super-el-nino-will-worsen-global-hunger/) ⭐️ 7.0/10

据伯克利地球气候学家 Zeke Hausfather，截至 10 月，衡量厄尔尼诺强度的中热带太平洋升温已达 3.5℃，打破此前约 2.75℃的纪录，并预计在初冬升至约 4℃的峰值；世界粮食计划署 8 月警告，这可能到 2027 年底把额外 4900 万人推入急性粮食不安全，使总数达到 2.74 亿。

telegram · zaihuapd · 11月22日 14:09

**「背景」** 厄尔尼诺指中热带太平洋海水异常升温、进而扰乱全球天气的现象；世界气象组织已于 2026 年 6 月宣布本轮事件开始，并称其可能是有记录以来最强的一次。

**「影响」** 援助资金减少会直接削弱粮食救济覆盖：全球援助资金 2025 年较 2022 年峰值下降 30%，而在索马里遭遇类似旱情时，世界粮食计划署能覆盖的人数从 1000 万降至不足 100 万。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026%E2%80%932027_El_Ni%C3%B1o_event">2026–2027 El Niño event - Wikipedia</a></li>

</ul>
</details>

**标签**: `#厄尔尼诺`, `#粮食安全`, `#人道援助`, `#气候风险`, `#经济影响`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Agent 说“验证完了”，怎样才真的可信？](https://x.com/dotey/status/2124603209394078089) ⭐️ 7.0/10

宝玉在 X 上分享了一套让 AI Agent 的“验证”变得可检查、可信任的实务经验。背景是：随着 Vibe Coding 普及，生成代码的成本大幅下降，越来越多人直接把 Agent 的“做好了、验证完了”当成结论，直到上线后才发现问题；瓶颈也从写代码转移到了验证与代码审查。

文章的核心主张是：不要依赖 Agent 的自述，而要提前定义“什么叫做好”，并让结果变成人可以低成本检查的证据。具体包括五条经验：

\1. 不要依赖对抗式验证。让另一个或多个 Agent 反复检查、执行 Agent 反复修改，听起来合理，但常常无法收敛；尤其是不够强的模型可能越改越糟，还浪费 Token。根本原因是缺少统一验收标准，检查方未必掌握完整上下文和准确标准，容易自行提出一堆意见，执行方照单全收后越改越偏。

\2. 给出清晰验收标准，再提供能验收的环境。例如把设计稿交给 Agent 时，不只说“做成页面”，而是要求完成后截图、与设计稿对比，直到像素一致。重点不一定是每个项目都要像素级一致，而是让 Agent 知道标准是什么，并且手里有工具自行验证。

\3. 越早验证，返工成本越低。文章回顾传统软件工程中的三道关：可行性分析，判断项目是否值得做；原型开发，用模拟数据低成本验证方向；系统设计，包括技术选型、模块划分、数据结构、数据库和 API Schema。文章建议在动手实现前先让 Agent 写技术方案文档，既帮助人理解实现方式，也能及时纠正潜在问题。

\4. 让 Agent 提供证据，降低人的验收成本。人仍然必须在 Loop 中，否则容易得到 AI Slop；但人的验收能力是瓶颈。可让 Agent 提供截图、录屏、可视化 HTML 报告，或修 bug 时提供修改前后对比截图，也可模拟 API 响应生成不同场景截图。截图的价值是让人一眼看出问题，Agent 在截图过程中也可能自己发现问题。文中还提到，使用 Antigravity 时跨 Workspace 每读一个文件都要手工确认，体验很痛苦，说明应尽量减少人工确认成本。

\5. 代码审查聚焦真正的问题。Agent 生成代码太快，瓶颈已转向审查和验证。建议 PR 尽可能小，让 Agent 审查但不要全信结论，对结果分级，人只重点看 P0、P1，尤其是安全和性能问题；代码规范、最佳实践等细枝末节可以放过。

文章最后把这五条归纳为一句话：Agent 说的“做好了”不能直接当结论，要变成你能检查的东西——动手前告诉它标准，先用原型和方案文档验证方向，做完后让它用截图和对比证明，人的精力只花在最要紧的问题上。这是一则面向 Agent 工作流的实践经验分享，而非研究论文或产品发布。

twitter · 宝玉 · 11月22日 20:37

**「背景」** 这条帖子的背景是：AI Agent 已能快速生成代码和页面，但“完成”与“验证通过”往往只是模型自述，缺少可复核的证据。宝玉据此把问题归结为验收标准和验收环境的缺失，并提出五条做法：不要依赖对抗式验证；先定义清晰的验收标准，再给 Agent 一个能自行执行验证的环境；在可行性、原型和系统设计阶段尽早验证；用截图、录屏、HTML 报告降低人的验收成本；代码审查聚焦小 PR 与 P0、P1 问题。这些属于作者基于实践的评论，并非对照实验结论。

更广的讨论也在往类似方向走：Horizon 收录的 Hacker News 讨论中，开发者提出自己设计架构、让 LLM 补实现、把模型当初级工程师，并把省下的编码时间投入测试（tool-1-2）；另一个产品与 UX 评审提示词让 AI 按验收步骤走查页面和交互细节（tool-1-3）；Sphinx 则在推送生产前用理解问卷卡住 AI 生成代码，要求开发者先证明自己理解代码（tool-1-1）。这些例子可作为旁证，说明关注点正从“让 Agent 说它做完了”转向设置检查点、要求证据和保留人工判断。

该条目未附带社区评论，因此无法呈现针对该帖的直接反馈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sphinx-six-theta.vercel.app/">2026-10-19 — Sphinx: open-source hook quizzes developers on AI-generated code before deployment</a></li>
<li><a href="https://news.ycombinator.com/item?id=50151036">2026-10-20 — Engineers Share How to Ship AI-Written Code Safely</a></li>
<li><a href="https://x.com/vista8/status/2119574943021371755">2026-11-09 — AI Walkthrough Prompt for Product &amp; UX Review</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#verification`, `#agent workflows`, `#software engineering`, `#Vibe Coding`, `#practitioner insights`

---

<a id="item-twitter-news-2"></a>
### [东锡 NLP：从困惑度曲线读出 OpenAI 训练范式由预训练转向后训练](https://x.com/dongxi_nlp/status/2124602615543595393) ⭐️ 7.0/10

Dongxi 东锡 NLP 发布了一条技术长帖，对 OpenAI 公布的困惑度（perplexity）曲线提出一种解读：曲线形态的变化反映的是一次训练范式的迁移，即从「把基座模型做大」的预训练路线，转向「在更小基座上做大规模强化学习」的后训练路线。

帖中给出的关键观察是：GPT‑4.5 的困惑度约 0.877，被作者视为「预训练做大 base model」这条路的终点；其后的 o3 困惑度反而回升到约 0.90 附近。作者对这一「倒退」给出的解释是算力配置的改变：RL 需要跑大量 rollout，其成本与基座规模成正比，因此用更小的基座做大量 RL 更划算，算力便从预训练流向了后训练。

第二个论点涉及机制层面：RL 本身并不降低困惑度。它把输出分布收窄到高奖励的模式上，提升的是任务能力，牺牲的是对整体文本分布的拟合程度，所以困惑度回升并不等于模型变差。

第三个论点是一个反馈回路：后训练会间接反哺基座。经过 RL 的强模型可以生成合成数据、推理轨迹和干净的代码，用于下一代模型的预训练或 mid‑training。作者据此认为，后训练虽不直接降低困惑度，但通过「造数据」的循环间接让基座变强，这也对应他所称的 2026 年困惑度骤降。

需要注意的证据边界：帖中的具体困惑度数值（约 0.877、约 0.90）以及对 2026 年曲线走势的判断，均未附可核验的来源或口径说明，属于作者基于公开曲线的解读与推演，而非 OpenAI 的官方表述。因此这条内容更适合作为理解 LLM 训练趋势的一个分析框架，其中的定量细节和前瞻性结论应保留不确定性看待。

背景上，这类讨论处在「预训练 scaling law 收益递减、后训练与 RL 算力占比上升、合成数据回流预训练」这一近年反复出现的行业话题脉络中；该帖的价值在于把这些线索统一到一条可观察的指标（困惑度曲线）上加以叙述。

twitter · Dongxi 东锡 NLP · 11月22日 20:35

**「背景：困惑度曲线与训练重心迁移」** 这条讨论针对 OpenAI 公开的困惑度（perplexity）曲线，以及如何用它解读训练重心的迁移。困惑度长期被视为语言模型预训练的核心指标；OpenAI 首席科学家 Jakub Pachocki 曾在《Perplexity and Intelligence》一文中用对数困惑度回顾模型代际，例如 GPT‑3.5 在其当时的主评估集上约为 ~0.99。这说明 OpenAI 确实会公开使用该指标比较不同代模型。

但困惑度衡量的是模型对文本整体分布的拟合程度，并不直接等同于下游任务能力。随着 o 系列等推理模型把强化学习放到训练流程的核心，评测叙事逐渐从“基座拟合更好”转向推理与任务表现更强，“困惑度回升是否等于退步”也因此成为需要解释的问题。同期还有两类相关动向：前沿实验室开始把 RL 训练运行本身当作需要专门防护的对象；工程教育内容则把 RL、蒸馏与推理时扩展作为构建推理模型的标准手段来讲授。两者都指向后训练已成为主要的算力与工程投入方向。

原帖给出的具体数值（GPT‑4.5 ~0.877、o3 ~0.90、2026 年的骤降）来自作者对曲线的读图，并未提供可核验出处，该条内容下也没有社区回复。因此下面梳理的因果链条——RL rollout 成本随基座规模增长、算力从预训练转向后训练、RL 收窄输出分布、合成数据反哺下一代基座——应视为一种有技术依据的解读框架，而非已被证实或官方确认的结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/OpenAI/status/2104815409522483470">2026-09-30 — OpenAI: How we think about securing frontier RL training runs</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/building-reasoning-models">2026-10-25 — Building Reasoning Models From the Ground Up: 11-Hour Video Course</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#LLM training`, `#perplexity`, `#post-training`, `#reinforcement learning`, `#scaling laws`, `#synthetic data`, `#OpenAI`

---