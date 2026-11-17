# Horizon 每日速递 - 2026-11-17

> 从 85 条内容中筛选出 25 条重要资讯。

---

**科技新闻**
1. [vLLM v0.34.0 发布：默认启用可扩展 KV cache，移除 Model Runner V1](#item-tech-news-1) ⭐️ 8.0/10
2. [Jiff 1.0 发布：Rust 的新日期时间库](#item-tech-news-2) ⭐️ 8.0/10
3. [Linux 内核补丁提议新增 futex PING 类别](#item-tech-news-3) ⭐️ 7.0/10
4. [Marimba：用冻结 Qwen3-ASR 编码器做校准语音问答](#item-tech-news-4) ⭐️ 7.0/10
5. [duetto：不微调，采样时引导预训练变换器的实时爵士搭档](#item-tech-news-5) ⭐️ 7.0/10
6. [腾讯混元发布 Hy4 flash：224B MoE、1M 上下文并大幅降价](#item-tech-news-6) ⭐️ 7.0/10
7. [美与九国签署《旧金山宣言》协调 AI 供应链安全](#item-tech-news-7) ⭐️ 7.0/10
8. [亚马逊称 AI 代理窃取 API 密钥自筹算力，MadPot 已阻断](#item-tech-news-8) ⭐️ 7.0/10
9. [卡内基梅隆大学在 YouTube 免费发布完整 CS 课程讲座](#item-tech-news-9) ⭐️ 6.0/10
10. [Windows 11 被指收集编程代理与开发者工具使用数据](#item-tech-news-10) ⭐️ 6.0/10
11. [TRMNL 发布 Frame：31.5 英寸彩色电子纸显示屏](#item-tech-news-11) ⭐️ 6.0/10
12. [微软将大规模邮件中断归因于七月修复引入的软件缺陷](#item-tech-news-12) ⭐️ 6.0/10
13. [苹果启动 20 万人健康 AI 使用研究](#item-tech-news-13) ⭐️ 6.0/10
14. [Apple 智能上线国行 iPad 与 Mac 测试版，并测试 Siri 每日用量上限](#item-tech-news-14) ⭐️ 6.0/10

**AI 开源项目**
1. [vLLM v0.34.0：可扩展 KV cache 默认开启，Model Runner V1 退役](#item-ai-projects-1) ⭐️ 9.0/10
2. [LMCache 发布面向 Rebellions RBLN NPU 的 nightly wheel](#item-ai-projects-2) ⭐️ 6.0/10
3. [LMCache 发布 nightly-rocm：面向 AMD Instinct 的 ROCm 7.2 预编译 wheel](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache 发布 nightly 构建（CUDA 13.0 wheel）](#item-ai-projects-4) ⭐️ 5.0/10

**财经新闻**
1. [中国 10 月消费、工业与投资数据全面低于预期](#item-finance-news-1) ⭐️ 8.0/10
2. [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has ties to the chipmaker](#item-finance-news-2) ⭐️ 8.0/10
3. [英特尔及 CEO 陈立武遭股东集体诉讼](#item-finance-news-3) ⭐️ 8.0/10
4. [ETF 专家：英伟达高层动荡与民主党掌控国会或重塑 AI 交易](#item-finance-news-4) ⭐️ 7.0/10
5. [猪肉价格跌至近 10 年低位](#item-finance-news-5) ⭐️ 7.0/10
6. [中国三季度外资直接投资转为净流出 9 亿美元](#item-finance-news-6) ⭐️ 7.0/10

**推特新闻**
1. [Lenny Rachitsky 分享：让 AI 助手接入自有 Anthropic API 的分步提示词](#item-twitter-news-1) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [vLLM v0.34.0 发布：默认启用可扩展 KV cache，移除 Model Runner V1](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 8.0/10

vLLM 发布 v0.34.0，含 1,061 个提交、412 位贡献者，新增约 10 个模型，并默认启用可扩展 KV cache——缓存按 CUDA graph 捕获与预热后实际空闲显存来分配，官方举例 MiniMax-M3 在 H200 上从 433k 增至 672k token。该版本带来多项破坏性变更：Model Runner V1 被移除（V2 成为唯一 GPU runner）、默认 --block-size 由 16 改为 64、gpu\_memory\_utilization 默认 1.0、ROCm 7.2 的镜像与 wheel 停止发布（仅保留 ROCm 10.0），并要求 huggingface\_hub &gt;= 2.0.0（同时需 tokenizers &gt;= 0.23.3、timm &gt;= 1.0.30）；QuTLASS/fp\_quant、Marlin W4A8 以及 Keye-VL 系列支持也被删除。发布说明自报在 Blackwell 与 MI355X 上的加速，例如 GB200 上 Step5 NVFP4 MoE 解码最高 1.95×、GLM-5.3 长提示 TTFT 快 1.24–1.40×，但这些性能数字来自项目自身，尚未经独立验证。

github · khluu · 11月16日 23:22

**「前置概念：KV cache 容量算法与 Model Runner」** vLLM 的 KV cache 决定了单卡能同时缓存多少上下文：此前它按 \`gpu\_memory\_utilization\` 估算可用显存后预分配（发布说明给出的“旧行为”取值是 0.9），v0.34.0 改为在 CUDA graph 捕获与 warmup 结束后按实际剩余显存计算，并将其设为默认。Horizon 10 月 19 日的日报曾报道 v0.32.0 扩大低精度 KV cache 支持（NVFP4 / FP8），那一版改的是缓存精度，这一版改的是缓存容量的计算方式。Model Runner 则是 vLLM 执行模型前向的抽象层，V2 此前作为可选路径存在，可用 \`VLLM\_USE\_V2\_MODEL\_RUNNER=0\` 退回 V1；本版删除 V1 后，该环境变量会直接导致启动失败。

**「影响」** 升级方需先处理兼容性问题：设置 VLLM\_USE\_V2\_MODEL\_RUNNER=0 现在会在启动时直接失败，原有 V1 的 logits processor 需迁移到 vllm.v1.worker.gpu.sample.logits\_processor；若要保留旧行为，可传 --block-size 16、--gpu-memory-utilization 0.9 或 --no-enable-extensible-kv-cache。发布说明同时指出，可扩展 KV cache 在部分 H200 模型、并发 128 时会使单 token 解码延迟（TPOT）上升 6–18%，即更高吞吐与更低单流延迟之间存在取舍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases/tag/v0.32.0">2026-10-19 — vLLM 0.32.0 adds systemone endpoint, generic parsers, low-precision KV cache</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open source`, `#performance optimization`, `#breaking changes`

---

<a id="item-tech-news-2"></a>
### [Jiff 1.0 发布：Rust 的新日期时间库](https://burntsushi.net/jiff/) ⭐️ 8.0/10

由 burntsushi（Andrew Gallant）开发的 Rust 日期时间库 Jiff 发布 1.0 版本。社区讨论围绕它能否替代 chrono 展开，并关注其对时间尺度（如 TAI）的处理以及文档中「何时不该用 Jiff」的适用边界说明。需要说明的是，本条目的正文内容不可得，目前可依据的只有发布页标题与读者评论，因此尚无独立基准测试、迁移成本实测或生态采用情况的证据。

hackernews · burntsushi · 11月16日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=50519744)

**「背景」** Jiff 是 Andrew Gallant（BurntSushi）为 Rust 编写的日期时间库，自 2025 年初起以 0.x 系列发布，并把时区与夏令时处理放在 API 的核心位置。该项目的 GitHub README 曾把 1.0 的目标定在 2025 年夏，同时说明这一期限已经错过、1.0 需要尽可能做“对”，因此本次发布是该库结束长期 0.x 阶段、进入正式 1.0 的节点。

**「影响与兼容性」** 对 Rust 开发者来说，Jiff 1.0 提供了一个 chrono 之外的可选依赖，但是否迁移存在明确顾虑：曾维护 chrono 约五年的 quodlibetor 表示，用户之所以一直使用 chrono，正是因为其 API 稳定，任何小改动都会遇到阻力。这意味着新库的采用更可能取决于下游生态库是否支持，而非 API 设计本身。

**「社区讨论」** 前 chrono 维护者 quodlibetor 称，他因看到改进空间却找不到落地路径而陷入倦怠并停止维护，并对 burntsushi 编写该库表示感谢。有评论者（Dagonfly）赞赏文档坦然承认 Jiff 并非适用于所有场景；ddahlen 则询问时间尺度的一般处理方式以及是否容易加入 UT1 等其他时间尺度，the\_\_alchemist 表示愿意尝试，但仍认为 chrono 相对好用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BurntSushi/jiff">GitHub - BurntSushi/jiff: A datetime library for Rust that ...</a></li>
<li><a href="https://github.com/BurntSushi/jiff/releases">Releases · BurntSushi/jiff - GitHub</a></li>

</ul>
</details>

**标签**: `#Rust`, `#datetime`, `#libraries`, `#API design`, `#time zones`

---

<a id="item-tech-news-3"></a>
### [Linux 内核补丁提议新增 futex PING 类别](https://lwn.net/Articles/1102988/) ⭐️ 7.0/10

LWN 报道了 Suleiman Souhlal 提交的一组 Linux 内核补丁，提议为 futex 子系统增加第三种 futex 类别，命名为“futex PING”，即“下一代优先级继承”（priority inheritance next generation）。目前 futex 提供两种基本变体，该系列的目标是让 futex 更快，并改进优先级继承。所附 LWN 内容仅为文章引言，没有给出性能数据、合并时间表或合入状态，因此这仍是待评审的补丁提案，而非已发布的内核功能。

rss · LWN.net · 11月16日 15:06

**「背景」** futex 是内核中支撑用户空间快速互斥锁的子系统，目前提供两类基本变体，其中 PI futex 通过内核的 rtmutex 实现优先级继承。2026 年 9 月 17 日，Google 的 Suleiman Souhlal 提交了 RFC 补丁系列，首次提出 FUTEX\_PING（PI Next Generation）：这类 PI futex 允许等待队列顶部的等待者被“窃取”（stealable），内部改用 Proxy Execution 而不是 rtmutex，以获得类似 PI 的行为而不必承受经典 PI futex 的严格性。LWN 此次报道的正是 Suleiman Souhlal 提交的补丁系列，为该子系统增加这个第三类 futex。

**「影响」** 该补丁目前以 RFC 形式提出，据外部报道，内核维护者认为其尚不成熟，并指出用锁窃取和代理执行取代严格的优先级继承交接可能带来锁死风险。对依赖 futex 优先级继承的实时与低延迟工作负载而言，这意味着在新类合入主线前需先评估这些风险，短期内不宜指望可直接替换现有 futex 用法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lkml.org/lkml/2026/9/17/386">LKML: Suleiman Souhlal: [RFC PATCH 00/12] FUTEX_PING: A ...</a></li>
<li><a href="https://freenode.net/article/google-floats-stealable-ping-futexes-for-linux">Google floats stealable PING futexes for Linux · freenode</a></li>
<li><a href="https://lwn.net/Articles/1094994/">FUTEX_PING: A stealable futex using Proxy Execution. - lwn.net</a></li>
<li><a href="https://freenode.net/article/google-floats-stealable-ping-futexes-for-linux">Google floats stealable PING futexes for Linux · freenode</a></li>

</ul>
</details>

**标签**: `#Linux kernel`, `#futex`, `#synchronization`, `#priority inheritance`, `#operating systems`

---

<a id="item-tech-news-4"></a>
### [Marimba：用冻结 Qwen3-ASR 编码器做校准语音问答](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Reddit 的 r/MachineLearning 帖子介绍了 Marimba：它用冻结的 Qwen3-ASR-0.6B 编码器，对每个 8 秒音频窗口只做一次编码，回答打字输入的“是/否、选项或评分”问题，并返回校准概率。帖子称在同一组 1000 个公开问题上，它在 9 项测试中有 6 项追平或超过 Qwen3-Omni（30B-A3B），语种识别在 300 条 FLEURS 片段上达到 100%，说话人变化 AUROC 在 AMI 和 VoxConverse 上为 0.966–0.980，说话人数量优于 pyannote 3.1，但 Qwen3-Omni 在 Speech Commands 上仍更好。作者同时注明话轮结束读数是在 Smart Turn 数据上训练的，因此该行只对其自身分布内成立；在 Smart Turn 自家测试集上 Marimba 的 AUROC 为 0.930，低于 Smart Turn v3.2 的 0.982，在 ICSI 上以 0.716 对 0.712 打平，并且对未见任务（如 CochlScene 场景分类）各头都只有随机水平；这些结果来自 Reddit 预印本公告，尚未经同行评审或独立复现。

reddit · r/MachineLearning · /u/solanotodesch · 11月16日 15:47

**「背景」** Marimba 使用的核心组件是冻结的 Qwen3-ASR-0.6B 编码器；这是一个约 0.6B 参数、以 Apache 2.0 发布的开源语音识别模型，支持语言识别、上下文提示和流式处理。作为对照的 Qwen3-Omni 30B-A3B 则是规模大得多的任意模态模型，可接收音频、视频和文本并输出音频或文本，因此两者在参数量和任务范围上并不对等。

**「影响」** 对开发者而言，Marimba 已提供 Apache-2.0 权重、GitHub 代码、Hugging Face 演示和 pip install marimba-audio，可在同一个冻结编码器上搭建术语检测、语种识别、话轮结束检测及说话人变化/数量查询；但它明确不适用于未见任务，选用前需按目标场景验证，而术语检测采用零样本加 Platt 校准是否应对比专用 KWS 模型，也是作者提出的开放评估问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anchorterminal.com/tools/qwen3-asr-0-6b">Qwen 3 - ASR - 0 . 6 B review (2026): pricing, alternatives and grade C</a></li>
<li><a href="https://www.toolify.ai/ai-model/qwen-qwen3-omni-30b-a3b-instruct">Qwen 3 - Omni - 30 B - A 3 B -Instruct huggingface.co api &amp; Qwen... - Toolify</a></li>

</ul>
</details>

**标签**: `#speech recognition`, `#audio question answering`, `#model efficiency`, `#calibration`, `#Qwen3-ASR`

---

<a id="item-tech-news-5"></a>
### [duetto：不微调，采样时引导预训练变换器的实时爵士搭档](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

duetto 是一个面向 MIDI 键盘的实时爵士搭档，它不微调预训练的 Anticipatory Music Transformer（Thickstun 等人，2023），而是在采样时通过基于规则的 logit 掩码与偏置来引导生成，代码可免费用于非商业用途。它能让模型与你合奏一首标准曲（独奏、伴奏、行走低音），在你演奏时伴奏、停下时独奏；演示曲目为《Autumn Leaves》（160 bpm）。技术上，玩家与模型的音符构成同一事件序列逐音续写，乐句来自 Weimar Jazz Database 并按换气点切分、按和弦移调；作者报告演示中约 61% 的独奏音符来自引用乐句或主题，其余由模型生成。服务器预采样约 1 秒音乐并在玩家弹奏时重采样未播放部分；作者报告在 3080 Ti 上约 12 ms/音符（medium）和 18 ms/音符（large），Jetson Orin Nano 上 large 模型约 90 ms/音符，仍足以现场演奏，但他也指出它可能偏离演奏者、响应难以预测，且模型与规则的平衡很脆弱。

reddit · r/MachineLearning · /u/GGAllin43 · 11月16日 09:19

**「背景」** Horizon 10 月 25 日日报曾报道过 Duetto：它让预训练的 Anticipatory Music Transformer 无需微调就为 MIDI 键盘实时伴奏，做法是在采样时偏置 logits，抑制调外音并增强和弦音。当前帖子延续同一思路，把控制扩展为更完整的爵士搭档，增加规则层对音符进行掩码/偏置，并加入来自 Weimar Jazz Database 的乐句引用与实时延迟数据。Anticipatory Music Transformer 本身是 Thickstun 等人 2023 年提出的 anticipatory infilling 模型，在 Lakh MIDI 上训练，可执行包括伴奏在内的 infilling 控制任务。

**「对开发者的实际影响」** 对想搭建实时 AI 合奏的开发者来说，这个项目表明不微调也能在单张消费级显卡上跑通：作者实测 3080 Ti 上约 12 ms/音符（medium）与 18 ms/音符（large），Jetson Orin Nano 上 large 模型约 90 ms/音符，仍足以支撑现场演奏。需要留意的是，公开代码仅限非商业用途，商用部署须另行处理授权；作者也指出系统目前仍会偏离演奏者、响应难以预测，规则与模型创意的平衡尚不稳定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xe4pex/got_a_pretrained_music_transformer_to_jam_with_me/">2026-10-25 — Pretrained music transformer jams live via logit steering, no fine-tuning</a></li>
<li><a href="https://arxiv.org/abs/2306.08620">[2306.08620] Anticipatory Music Transformer - arXiv.org</a></li>

</ul>
</details>

**标签**: `#music generation`, `#transformers`, `#sampling-time steering`, `#real-time MIDI`, `#jazz`

---

<a id="item-tech-news-6"></a>
### [腾讯混元发布 Hy4 flash：224B MoE、1M 上下文并大幅降价](https://mp.weixin.qq.com/s/5yBbf-ctYziM5r0i6Y17lA) ⭐️ 7.0/10

腾讯混元发布 Hy4 flash，这是一个总参数 224B、激活 12B 的多模态 MoE 模型，支持 1M 上下文，并给出每百万 Token 输入 0.5 元、输出 2 元、缓存命中 0.02 元的 API 定价。官方称其综合效果略优于 Hy4 preview，WorkIndex 单任务成本为 Hy4 preview 的 1/13、Hy4 的 1/20，这些均为厂商说法，来源未提供独立评测。模型已在腾讯云 TokenHub、WorkBuddy 和元宝上线，官方表示计划开源；11 月 30 日前 WorkBuddy 限免、API 5 折。

telegram · zaihuapd · 11月16日 07:17

**「背景」** 腾讯混元此前已有 Hy4 系列：Horizon 11 月 5 日的日报曾报道腾讯发布开源权重基础模型 Hy4，并与腾讯互动娱乐事业群合作将其适配游戏开发，同时承认它在科研级数学、长周期编程等任务上与头部闭源模型存在差距。第三方资料显示 Hy4 是总参数 770B、支持 1M 上下文的 MoE 模型，且存在一个 preview 版本。Hy4 flash 与它们同代但体量小得多——224B 总参数、12B 激活，而官方给出的成本与效果对比对象正是 Hy4 和 Hy4 preview。

**「影响」** 对以日常任务为主、按 Token 计费的开发者而言，Hy4 flash 相对 Hy4 的单价下降是可直接核算的成本变化，但 5 折与 WorkBuddy 限免只到 11 月 30 日；在开源版本落地前，使用仍限于腾讯云 TokenHub、WorkBuddy 和元宝等官方渠道，效果与成本优势也需自行验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4">2026-11-05 — Tencent Hy4 Open-Weight Model Targets Game Development</a></li>
<li><a href="https://www.eesel.ai/blog/tencent-hy4">Tencent Hunyuan Hy 4 : specs, benchmarks , and pricing... | eesel AI</a></li>
<li><a href="https://lmspeed.net/model/hy4">Hy 4 API Pricing &amp; Benchmarks | LMSpeed</a></li>

</ul>
</details>

**标签**: `#Tencent Hunyuan`, `#LLM release`, `#MoE`, `#API pricing`, `#multimodal`

---

<a id="item-tech-news-7"></a>
### [美与九国签署《旧金山宣言》协调 AI 供应链安全](https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/) ⭐️ 7.0/10

11 月 15 日，美国与澳大利亚、印度、以色列、日本、韩国、卡塔尔、新加坡、阿联酋和英国签署《旧金山宣言》，承诺共同保护支撑超级智能（SI）供应链的敏感技术和关键基础设施。宣言确认经济安全是国家安全根基，并设立五个工作组，分别负责创新政策框架、SI 在关键领域的应用、SI 全栈供应链协作、安全港与供应链安全枢纽，以及 SI 安全与韧性。目前公开内容仍属宣言层面，未列出有约束力的承诺、执行时间表或具体实施措施。

telegram · zaihuapd · 11月16日 10:40

**「背景」** 美国国务院称，《旧金山宣言》于 11 月 15 日在负责经济事务的副国务卿雅各布·赫尔伯格召集的 Pax Silica Founders Retreat 上签署。《金融时报》将该协议描述为美国与盟友保护 AI 供应链免受中国影响的举措。

**「对相关企业的影响」** 宣言本身不含约束性承诺或实施时间表，因此签署国（美国、澳大利亚、印度、以色列、日本、韩国、卡塔尔、新加坡、阿联酋、英国）的半导体、AI 基础设施与关键零部件企业短期内不会因此新增明确的合规义务。据《印度时报》报道，该协议覆盖半导体、AI 基础设施与关键技术供应链，相关企业更应关注五个工作组后续是否就出口管制、技术标准或「安全港」机制产出具体规则，而不是预期一份立即生效的行业门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.investing.com/news/world-news/us-nine-nations-sign-san-francisco-declaration-on-ai-security-5028448">U.S., nine nations sign San Francisco declaration on AI security By...</a></li>
<li><a href="https://www.ft.com/content/3c2197fc-9618-4838-91e6-522ce1a96a22?syn-25a6b1a6=1">US and allies sign accord to protect AI supply chains from China</a></li>
<li><a href="https://timesofindia.indiatimes.com/business/india-business/india-joins-us-led-alliance-to-secure-ai-supply-chains-amid-china-tech-rivalry/articleshow/135886669.cms">India joins US-led alliance to secure AI supply chains amid China tech...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#supply chain security`, `#geopolitics`, `#superintelligence`, `#international cooperation`

---

<a id="item-tech-news-8"></a>
### [亚马逊称 AI 代理窃取 API 密钥自筹算力，MadPot 已阻断](https://cybernews.com/security/amazon-autonomous-cybercrime-artex-framework/) ⭐️ 7.0/10

亚马逊称，一个由开源渗透测试框架 Artex 驱动的 AI 代理行动，从公网暴露的 LiteLLM、Dify 等 AI 应用中窃取 API 密钥，验证后汇入共享池，用于支付更多大模型调用。该活动自 10 月 3 日开始，11 月 5 日被亚马逊的诱饵网络 MadPot 截获阻断。亚马逊以中等信心将行动归因于中国相关威胁组织，并称并非所有被列出的目标都已失陷，同时表示已通知可能受影响的 AWS 客户。上述内容为亚马逊的单方说法，其中等归因置信度也意味着组织归属尚未得到独立证实。

telegram · zaihuapd · 11月16日 13:00

**「背景」** LiteLLM 这类网关通过统一的 OpenAI 格式接口调用多家模型供应商，并集中保存上游 API 密钥；Dify 等应用也有类似的密钥配置。因此，一旦实例暴露在公网，这些密钥就可能被用来支付模型调用费用。Horizon 2026 年 10 月 9 日日报曾报道，CrowdStrike 称名为 ARTEX 的开源 AI 代理工具在 2025 年 9 月底至 10 月初被用于攻击韩国金融机构，并以中等信心将其归因于以经济获利为目的的中文使用者；亚马逊现在描述的是同一 Artex 工具被用于另一波针对 AI 应用密钥的活动。

**「影响」** 对于使用 LiteLLM、Dify 并将服务暴露在公网的组织，直接风险是自有 API 密钥已被盗用并为攻击者的模型调用付费；亚马逊称已通知可能受影响的 AWS 客户，相关方应核查密钥是否泄露并及时轮换，同时收敛公网暴露面。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://xcai.pro/">2026-10-09 — CrowdStrike Reports Open-Source AI Tool ARTEX Used in South Korea Financial Attacks</a></li>
<li><a href="https://thehackernews.com/2026/11/amazon-uncovers-ai-agent-campaign.html">Amazon Uncovers AI Agent Campaign Targeting LiteLLM , Dify , and...</a></li>
<li><a href="https://docs.litellm.ai/docs/providers">AI Providers | liteLLM</a></li>

</ul>
</details>

**标签**: `#AI security`, `#autonomous agents`, `#API key theft`, `#cybercrime`, `#open-source tooling`

---

<a id="item-tech-news-9"></a>
### [卡内基梅隆大学在 YouTube 免费发布完整 CS 课程讲座](https://www.cs.cmu.edu/learn/) ⭐️ 6.0/10

卡内基梅隆大学推出 CS Learn，在 YouTube 免费发布当前 CMU 计算机科学课程的整学期讲座，涵盖多个主题。项目负责人 Phillip Compeau 在 Hacker News 上表示，本周每天首播一门课程，明年 1 月还会上线更多课程，并称学生开发了自动化制作流程的工具。这一项目是开放课程资源的扩展；评论者提醒，目前重点是讲座视频，课程作业与反馈等配套内容尚未同步提供。

hackernews · pcompeau · 11月16日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=50522980)

**「背景」** 免费开放大学课程并不是新做法：CS Learn 项目负责人在发布讨论中自己也提到，MIT 早在约 25 年前就开放了课程资料，此后 Coursera、edX 等 MOOC 平台也曾大规模上线名校课程。CMU 计算机学院此前已有官方 YouTube 频道（现名为 Kenneth C. Griffin School of Computer Science），而此次上线的是一个独立的 CS Learn 频道；据外部报道，这些讲座来自七个院系的教师，其中包括陈天奇与贾志豪讲授的 ML Systems 课程。

**「影响」** 对想自学的学生和开发者来说，他们现在可以免费观看 CMU 现行课程的完整讲座，但若缺少项目作业与反馈，仅靠视频可能难以达到在校课程的学习效果；评论者提到课程配套材料将在后续推出。

**「社区讨论」** HN 评论中，ecshafer 认为讲座只是起点，项目、讲义和反馈机制才决定学习效果，并提到常见问题是只发布 CS1 而不发布研究生编译器课程；JSR\_FDED 则主张在 AI 时代学好基础仍让人把 AI 当工具而不是被替代。另有评论表达对 15-259 概率与计算等具体课程的期待，并回顾 Coursera 和 edX 从开放课程走向盈利化的经历。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/CMUComputerScience">CMU Kenneth C. Griffin School of Computer Science - YouTube</a></li>
<li><a href="https://todayforai.com/en/items/art-2c7b6259-c5f">Carnegie Mellon Opens Computer Science Courses Free on YouTube</a></li>

</ul>
</details>

**标签**: `#computer-science-education`, `#online-learning`, `#open-courseware`, `#cmu`, `#youtube`

---

<a id="item-tech-news-10"></a>
### [Windows 11 被指收集编程代理与开发者工具使用数据](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 6.0/10

一篇发布在 xusheng.dev 的文章称，Windows 11 会收集用户使用了哪些编程代理（coding agents）和开发者工具，该文在 Hacker News 上引发讨论。所提供材料中没有文章正文，因此这项遥测的具体范围、采集机制、数据去向以及是否可关闭都未获说明或验证，也无法判断微软是否已确认。对在 Windows 11 上工作的开发者而言，争议点在于开发工具的使用情况是否会被上报，但现阶段这仍是一篇博客文章的指控，而非经独立核实的结果。

hackernews · cwaffles · 11月16日 22:58 · [社区讨论](https://news.ycombinator.com/item?id=50524736)

**「背景」** Windows 的遥测收集长期是开发者和隐私倡导者关注的争议点，社区中已存在专门用于阻止 Windows 10/11 遥测并关闭相关服务的第三方工具，例如基于 PowerShell 的 WindowsTelemetryBlocker。\[tool-1-1\] 此次讨论的新焦点在于，有报道称 Windows 11 的收集范围延伸到了用户使用哪些编码代理与开发者工具；由于原帖内容未提供，该范围的具体机制目前无法从现有材料核实。

**「分类决定能否关闭」** 对开发者而言，关键在于这类开发工具使用数据被归入哪一类诊断数据：Windows 11 的“必需诊断数据”在家庭版和专业版下无法关闭，只有企业版用户才能规避，而“可选诊断数据”可以由用户限制。由于原文没有说明采集机制与范围，重视隐私的团队目前只能先按“必需数据不可关闭”的假设评估合规风险，并在部署前自行核查。

**「社区讨论」** 评论者大多没有分析该遥测说法本身，而是转向讨论改用 Linux：s\_dev 认为到 2026 年 Linux 对绝大多数单机游戏已完全可用，多人游戏仍有许多问题；dead\_hn\_theory 称从 Windows 迁移大约只需一周适应时间；nout 表示现在会直接全新安装 Linux，必要时用虚拟机运行 Windows。这些都是个人经验与观点，并不构成对遥测范围的事实确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/N0tHorizon/WindowsTelemetryBlocker">N0tHorizon/WindowsTelemetryBlocker: A PowerShell based tool to...</a></li>
<li><a href="https://www.youtube.com/watch?v=mOeBjArKMYY">How Much Data Does Windows 11 Really Collect ? - YouTube</a></li>
<li><a href="https://windowsforum.com/news/understanding-windows-telemetry-privacy-performance-and-control.346257/">Windows Telemetry : Privacy , Performance &amp; Control</a></li>

</ul>
</details>

**标签**: `#Windows 11`, `#telemetry`, `#privacy`, `#developer tools`, `#coding agents`

---

<a id="item-tech-news-11"></a>
### [TRMNL 发布 Frame：31.5 英寸彩色电子纸显示屏](https://trmnl.com/blog/introducing-frame) ⭐️ 6.0/10

TRMNL 在其博客上宣布推出 Frame，一块 31.5 英寸的彩色电子纸（ePaper）显示屏，这是该产品公告中给出的核心规格。目前可获取的资料中没有官方公布的价格、上市时间或兼容性细节，因此这属于一次产品发布公告，而非已确认上市的成品能力。Hacker News 讨论中出现的 1200 美元报价来自一位评论者的个人说法，并非厂商确认的信息。

hackernews · geerlingguy · 11月16日 16:23 · [社区讨论](https://news.ycombinator.com/item?id=50519354)

**「背景」** Frame 是 TRMNL 的第三款产品：一块 31.5 英寸全彩电子纸显示屏，装在手工木框中，并已开放预售（tool-2-1）。在此之前，彩色电子纸主要出现在个人尺寸设备上，例如采用 3.7 英寸 E Ink Spectra 6 面板、面向桌面或冰箱门的彩色电子纸相框，因此把彩色电子纸放大到 31.5 英寸属于尺寸上的明显跨越（tool-2-3）。

**「影响」** 对个人买家而言，最直接的约束是评论中提到的 1200 美元价格：\[RGS1811\] 表示这超出其愿意支付的范围，说明 31.5 英寸彩色电子纸目前仍属于高价小众档次，而非可随意添置的家用设备。此外 \[Calvin02\] 称早期 TRMNL 设备出现品控下滑与发货延迟，潜在买家在下单前宜确认交付周期和售后条款。

**「社区讨论」** 评论者的关注点集中在价格与厂商信任上：一位用户表示 1200 美元超出其可接受范围但认可产品存在，另一位自称早期用户的评论者称 TRMNL 的品控下滑、发货延迟，并因创始人政治立场表示不会再购买。也有评论者提出大尺寸电子纸为何仍昂贵（怀疑与专利有关），并分享了用二手三星 Frame 电视加脚本与 SDXL 生成图像做墙面画廊的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trmnl.com/blog/introducing-frame">Introducing Frame | TRMNL</a></li>
<li><a href="https://www.gobetterdisplay.com/">VeraMag Color ePaper Photo Frame | GoBetter Display</a></li>

</ul>
</details>

**标签**: `#e-paper`, `#hardware`, `#displays`, `#TRMNL`, `#product-launch`

---

<a id="item-tech-news-12"></a>
### [微软将大规模邮件中断归因于七月修复引入的软件缺陷](https://www.theregister.com/saas/2026/11/16/microsoft-blames-monster-email-outage-on-software-defect-introduced-in-july-fix/5310026) ⭐️ 6.0/10

微软将一次大规模邮件服务中断归因于今年 7 月一次修复所引入的软件缺陷。社区评论引述的事后说明称，该缺陷在配置较低的测试环境中顺利通过验证，却被高配置生产环境中的并发问题触发，因而在测试阶段未被发现。现有素材仅提供标题与评论转述，微软官方事后报告的完整细节、受影响用户规模和恢复耗时均未给出，上述归因与测试环境差异的说明应视为待官方原文确认的说法。

hackernews · Bender · 11月16日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=50517321)

**「事件背景」** Horizon 11 月 13 日的日报曾报道 Microsoft 365 邮件等服务出现全球性大规模服务降级，微软当时验证了一种替代健康检查方法，让部分受影响服务器恢复服务，并着手扩大该变更的适用范围、准备自动检测并重启无响应服务器的恢复流程。11 月 14 日的日报进一步记录该故障持续超过 12 小时，Outlook、Teams 和 Copilot 均受影响，澳大利亚、日本和美国的部分政府机构也被波及，微软表示未发现恶意活动。外部事故报道称，此次引发故障的缺陷源自为 Microsoft 365 网络网关服务器准备的一次修复。

**「影响」** 直接受影响的是中断期间无法正常使用邮件服务的用户；对发布与运维团队而言，评论引述的事后说明所强调的测试环境与生产环境差异意味着，仅靠低负载测试环境验证修复可能无法暴露并发缺陷，需要以生产规模或等效并发条件复现验证。

**「社区讨论」** mike\_hearn 用电力系统的“黑启动”类比恢复过程，指出必须先断开全部负载再分块接入，否则无法维持频率稳定；andix 则质疑为何不通过限制或轮换 IP 段来削峰，让客户端至少有机会周期性同步。ncr100 质疑低配测试环境通过 7 月代码、却在高配生产环境暴露并发缺陷是否属于可接受的成本取舍，mindwok 则对关键网络基础设施中使用 Windows 表示意外。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://status.cloud.microsoft/">2026-11-13 — Microsoft 365 Email Outage Worldwide as Recovery Progresses</a></li>
<li><a href="https://www.reuters.com/technology/microsoft-365-outlook-down-thousands-us-users-downdetector-shows-2026-11-12/">2026-11-14 — Microsoft Outlook, Teams, Copilot Global Outage Exceeds 12 Hours</a></li>
<li><a href="https://cybersecuritynews.com/microsoft-outage-incident-report/">Microsoft Reveals How a Hidden Windows Bug Took Down Microsoft ...</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#service outage`, `#incident postmortem`, `#reliability engineering`, `#load shedding`

---

<a id="item-tech-news-13"></a>
### [苹果启动 20 万人健康 AI 使用研究](https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/) ⭐️ 6.0/10

苹果宣布与美国临床 AI 平台 OpenEvidence 合作，启动 Apple Health AI Usage Study，研究人们如何使用对话式健康 AI，并评估信任与理解程度。该研究计划在美国招募最多 20 万名年满 21 岁的居民，参与者需使用支持 Apple Intelligence 的 iPhone 15 Pro 或更新机型并运行 iOS 26 及以上。苹果表示，研究数据不会用于训练 AI 模型，相关应用也不用于诊断或治疗。目前这是早期公告，尚未公布研究结果。

telegram · zaihuapd · 11月16日 05:01

**「背景」** OpenEvidence 是一家成立于 2022 年、总部位于美国迈阿密的 AI 公司，开发同名的临床决策支持大语言模型平台，主要面向医疗专业人员，其回答以 NEJM、JAMA、Nature、NCCN、Cochrane 等同行评审文献为依据（tool-2-1、tool-2-2）。与这一面向临床医生的专业平台不同，苹果此次与 OpenEvidence 合作的研究考察的是普通用户如何使用对话式健康 AI，以及他们对结果的信任与理解程度。

**「影响」** 对符合条件的美国用户而言，参与门槛是 iPhone 15 Pro 或更新机型及 iOS 26 以上系统，旧设备用户无法加入；同时研究数据不用于训练 AI 模型，应用也不用于诊断或治疗，参与者不应将其视为临床工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenEvidence">OpenEvidence - Wikipedia</a></li>
<li><a href="https://www.openevidence.com/">OpenEvidence</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Health AI`, `#AI Research`, `#OpenEvidence`, `#iOS 26`

---

<a id="item-tech-news-14"></a>
### [Apple 智能上线国行 iPad 与 Mac 测试版，并测试 Siri 每日用量上限](https://www.theverge.com/tech/1034581/apple-intelligence-siri-ai-daily-usage-limits-icloud-subscription) ⭐️ 6.0/10

据来源，Apple 智能（Apple Intelligence）已在国行 iPad 和 Mac 上线，但处于测试阶段，用户需更新到 iPadOS 27.3 beta 2 或 macOS 27.3 beta 2 才能体验。同一批 iOS 27.3、iPadOS 27.3、macOS 27.3 beta 2 中，苹果正在测试部分 Siri AI 与 Apple 智能功能的每日设备用量上限：基础 Siri 命令仍免费不限量，受限的是云端进阶功能，包括多步骤个人情境请求和图片生成与编辑。来源还称，所有 Apple OS 上一处被其记为 worse\_query 的访问文件沙箱逃逸漏洞已经修复。该来源为简短聚合，未给出上限额度、支持机型或漏洞细节。

telegram · zaihuapd · 11月16日 20:12

**「背景」** 国行 iPhone 上的 Apple 智能已先行测试：11 月 4 日的日报记录了 iOS 27.3 测试版中「Apple 智能与 Siri」在国行设备上的测试，与阿里千问合作，包含通知摘要、Genmoji 等部分功能。更早的 10 月 15 日日报报道，苹果计划于 12 月通过 iOS 27.3 在中国大陆推出首批 Apple 智能功能，但不包含新版 Siri。此次 iPadOS 与 macOS 测试版把该测试范围从 iPhone 扩展到 iPad 与 Mac。

**「影响」** 国行 iPad 和 Mac 用户若要使用 Apple 智能，目前必须升级到 27.3 beta 2 测试版，无法在正式版上获得该功能；同时，依赖云端进阶能力的用户可能受每日用量上限约束，多步骤个人情境请求与图片生成、编辑的使用频率会被限制，而基础 Siri 命令不受影响。文件访问沙箱逃逸漏洞的修复同样随这批系统更新提供，未更新系统的设备不包含该修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-14/apple-prepares-to-debut-first-ai-features-in-china-in-december">2026-10-15 — Apple Plans December Launch of Apple Intelligence in Mainland China</a></li>
<li><a href="https://www.macrumors.com/2026/11/03/ios-27-3-health-app/">2026-11-04 — 苹果推 iOS 27.3 测试版：健康 App 重做、手表 AI 听录、国行 Apple 智能</a></li>

</ul>
</details>

**标签**: `#Apple Intelligence`, `#Siri`, `#Apple OS`, `#security vulnerability`, `#usage limits`

---

## AI 开源项目

<a id="item-ai-projects-1"></a>
### [vLLM v0.34.0：可扩展 KV cache 默认开启，Model Runner V1 退役](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 9.0/10

vLLM v0.34.0 是开源 LLM 推理与服务引擎的一次大版本发布：默认启用可扩展 KV cache，移除 Model Runner V1，新增 10 个模型，并在 Blackwell 与 MI355X 上报告了最高 1.95× 的 decode 提速，同时带来多项破坏性默认值变更。

github · khluu · 11月16日 23:22

**「解决的痛点」** 痛点在于显存被浪费、长上下文并发吞吐受限。旧方式按预估而非实测分配 KV cache，预热与 CUDA graph 捕获后仍有很多显存未用上。v0.34.0 改为在预热完成后按实际空闲显存动态确定缓存大小（如 MiniMax-M3 在 H200 上从 433k 增至 672k tokens），从而提升吞吐、降低高并发下的 TTFT。代价是部分模型单 token decode 延迟上升（H200 部分模型并发 128 时 TPOT +6–18%），可通过 --gpu-memory-utilization 0.9 或 --no-enable-extensible-kv-cache 退回旧行为。此外，移除 Model Runner V1 使 MRV2 成为唯一 GPU runner，减少双套执行路径的维护与配置负担；默认 block size 由 16 改为 64、gpu\_memory\_utilization 默认 1.0、ROCm 7.2 构建与 QuTLASS/fp\_quant、Marlin W4A8 等被移除，升级前需逐项核对。

**「背景与影响」** vLLM 是开源 LLM 推理与服务引擎的代表性项目，以高吞吐、显存高效为核心定位，靠 PagedAttention 管理注意力 key/value 显存，并配合连续批处理、分块预填充与前缀缓存（tool-1-1、tool-1-2）。PagedAttention 的关键洞察正在于把 KV 缓存分页管理，使此前动辄浪费 60%–80% 已分配显存的碎片问题基本消失（tool-2-3）。因此，KV 缓存如何分配与度量，一直是 vLLM 提升吞吐的主线之一。

本次 v0.34.0 是这一主线上的重要版本（1,061 个提交、412 位贡献者，其中 120 位新贡献者）。其标志性变化是把「可扩展 KV 缓存」设为默认：KV 缓存不再来自估算，而是按 CUDA graph 捕获与预热之后实际空闲的显存来确定，多数模型因此获得更大缓存、更高吞吐与更低 TTFT（例如 MiniMax-M3 在 H200 上 433k → 672k tokens）；代价是部分模型单 token 解码延迟可能上升，可用 --gpu-memory-utilization 0.9 或 --no-enable-extensible-kv-cache 退回旧行为。

这延续了 vLLM 对显存效率的追求，也说明其优化重心正从「更省显存」转向「把可用显存用满」。同时，Model Runner V1 被移除、V2 成为唯一 GPU runner，属于运行时架构的收敛清理；新增 10 个模型，并给出 Blackwell/MI355X 上的显著加速（最高 1.95× 解码、1.6× 吞吐）与 ROCm 10.0、CUDA 13.0 等硬件支持面。对生态而言，vLLM 的新默认值（block size 16→64、gpu\_memory\_utilization 默认 1.0、依赖与后端下线）会直接传导到下游部署栈，升级时需按「Before you upgrade」逐项核对。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/">vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm - project / vllm : A high - throughput and memory-efficient...</a></li>
<li><a href="https://gigagpu.com/vllm-paged-attention-explained/">vLLM PagedAttention Explained GIGAGPU</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM`, `#inference`, `#serving`, `#KV cache`, `#paged attention`, `#CUDA`, `#model support`, `#release`, `#breaking changes`

---

<a id="item-ai-projects-2"></a>
### [LMCache 发布面向 Rebellions RBLN NPU 的 nightly wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 6.0/10

LMCache 发布面向 Rebellions RBLN NPU 的 nightly 安装包，基于 dev 分支构建，适配 torch-rbln 0.12.0；torch-rbln、rebel-compiler 和 RBLN 驱动需由宿主机提供，不随包捆绑。

github · github-actions\[bot\] · 11月16日 13:07

**「解决的痛点」** 该版本解决的是 LMCache 在 Rebellions RBLN NPU 上的分发与安装适配问题：提供预构建 wheel，并要求宿主机已安装 torch-rbln、rebel-compiler 与 RBLN 驱动，避免在包内重复捆绑厂商组件。发布说明未给出核心代码变更或性能提升数据，因此不宜视为功能或性能升级。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV cache 管理层：它把原本只作为临时状态的 KV cache 变成可持久化、可跨服务引擎复用的“AI 原生知识”，可被存储、监控、压缩与检索（tool-1-1）。相关论文与官网描述进一步说明，它把 vLLM、SGLang 等现代推理引擎产生的 KV cache 从 GPU 显存中提取出来，跨引擎与跨查询共享，主要面向长提示、对话历史和检索内容被反复复用的负载，并支持在 GPU、CPU 内存与外部后端之间存储、复用、压缩、搜索、迁移和观测（tool-1-2、tool-1-3）。

本次 nightly-rbln 是这一缓存层在硬件适配方向上的延伸，为 Rebellions RBLN NPU 提供 nightly wheel。torch-rbln 是让 PyTorch 能自然使用 Rebellions NPU 算力的扩展，其中 rebel-compiler 为必需组件但不随 torch-rbln 一同安装（tool-2-1、tool-2-3）；Rebellions 的 ATOM 加速器则专门面向 AI 推理任务（tool-2-2）。因此该 wheel 的意义在于让 LMCache 的 KV cache 复用能力覆盖到 Rebellions NPU 这类推理加速器，扩展其硬件生态。

边界需要说明：来源显示这是由 CI（github-actions\[bot\]）从 dev 分支构建的 nightly 打包产物，未描述核心代码变更、性能数据或新功能；torch-rbln、rebel-compiler 与 RBLN 驱动仍由宿主机环境提供，不打包进 wheel，安装方需自行准备。因此其影响主要停留在持续集成与硬件适配的可用性层面，而非一次正式功能发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch - rbln · PyPI</a></li>
<li><a href="https://rebellions.ai/developers/">Developers - Rebellions</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">RBLN -SW/ torch - rbln : PyTorch extension for Rebellions NPU · GitHub</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly`, `#packaging`

---

<a id="item-ai-projects-3"></a>
### [LMCache 发布 nightly-rocm：面向 AMD Instinct 的 ROCm 7.2 预编译 wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

LMCache 发布 nightly-rocm 夜间构建：基于 dev 分支、面向 ROCm 7.2 的 wheel，覆盖 AMD Instinct gfx942/gfx950，并与上游 vLLM ROCm 镜像（torch 2.13、cp312）ABI 对齐，可直接 pip 安装。

github · github-actions\[bot\] · 11月16日 13:14

**「解决的痛点」** LMCache 是 LLM 推理的 KV cache 层，目的是复用缓存、减少重复 prefill 计算以及 KV 缓存带来的显存浪费。本次构建解决的是 AMD 平台上的分发与兼容问题：用户此前往往需要自行从源码编译，且容易撞上容器内 torch / Python 版本的 ABI 不匹配。官方直接提供与 vllm/vllm-openai-rocm 镜像 ABI 对齐的预编译 wheel（lmcache==0.5.8.dev167+rocm7.2），把部署从「编译 + 排错」简化为一条 pip 命令。需要注意，这是例行夜间打包产物，源信息未提供新架构特性、性能数据或 changelog。

**「背景与影响」** LMCache 是面向 LLM 推理的 KV cache 管理/复用层，研究工作涵盖缓存复用、卸载、压缩与服务优化（tool-1-1、tool-1-3），并通过 vLLM 的 KV connector 接口集成——应用侧继续访问常规的 OpenAI 兼容端点，LMCache 在推理层之下运行（tool-1-2）。因此它的发布节奏直接影响 vLLM 等推理栈在 KV cache 复用上的可用性。

本次 nightly-rocm 属于例行的夜间打包/CI 产物：从 dev 分支为 ROCm 7.2 构建 wheel，面向 AMD Instinct gfx942（MI300X/MI325X）与 gfx950（MI350X/MI355X），并与上游 vllm/vllm-openai-rocm 镜像 ABI 对齐（torch 2.13、cp312）。它的意义主要在于平台可用性——让 AMD Instinct 用户能够把 LMCache 直接安装进上游 vLLM ROCm 容器。

放到更大的生态里看，ROCm 7.2 已覆盖 MI300/MI350 系列的工作负载优化与兼容性说明（tool-2-1、tool-2-2），针对 CDNA3（gfx942）与 CDNA4（gfx950）也已有内核优化知识的整理（tool-2-3）；LMCache 提供匹配的 wheel，等于把 KV cache 这一层补齐到 AMD 软件栈中。需要说明的是，该 nightly 本身并不带来新的架构特性、性能结果或模型支持：来源未提供 benchmark 或 changelog 细节，因此不应据此推断性能提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.2.4/how-to/rocm-for-ai/inference-optimization/workload.html">AMD Instinct MI300 Series / MI350 Series workload optimization</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.0.0/compatibility/compatibility-matrix.html">Compatibility matrix — ROCm Documentation</a></li>
<li><a href="https://github.com/jhinpan/ROCmKernelWiki">GitHub - jhinpan/ROCmKernelWiki: Agent-queryable ROCm kernel ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#inference`, `#KV cache`, `#serving`, `#ROCm`, `#vLLM`, `#nightly`, `#release`

---

<a id="item-ai-projects-4"></a>
### [LMCache 发布 nightly 构建（CUDA 13.0 wheel）](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache 发布由 dev 分支构建的 nightly 版本，提供 linux/amd64 与 linux/arm64 的 CUDA 13.0 预编译 wheel，源码未附带变更日志、功能新增或性能数据。

github · github-actions\[bot\] · 11月16日 14:51

**「解决的痛点」** LMCache 面向 LLM 推理服务，核心是 KV 缓存层：推理时 KV 缓存占用大量显存，且难以跨请求、跨实例复用，容易造成显存浪费与重复计算。本次 nightly 具体解决的是分发环节的问题——让处于 CUDA 13.0 环境、且使用 linux/amd64 或 linux/arm64 的用户，可以直接通过预编译 wheel 安装，无需自行从源码编译适配。

需要注意：源码条目仅给出构建分支、日期、平台与安装命令，没有 changelog 或优化说明，因此无法判断本版本是否包含 KV 缓存管理上的实质改进，其性质更接近例行的打包构建更新。

**「生态位置与本次发布的性质」** LMCache 的定位是 LLM 推理的 KV cache 管理层：它把原本随请求生灭的 KV cache 变成可持久化存储、可跨多个 serving engine 复用、并可被观测的“AI 原生内存”，目标是在整个集群范围内对 KV cache 做存储、压缩、检索与复用（tool-1-1、tool-1-2）。其论文进一步指出，企业级推理的一个现实约束是主流引擎以 page 为粒度管理 KV cache，Llama、Qwen、GPT-OSS 等模型的 page 通常在 20 KB–63 KB 量级，因此需要专门的缓存层来承接这部分开销（tool-1-3）。

本次 nightly 属于例行的构建/打包更新，而非功能发布：内容仅为从 \`dev\` 分支构建、面向 linux/amd64 与 linux/arm64 的 CUDA 13.0 wheel，安装时需指向 PyTorch 的 cu130 索引。发布说明未包含 changelog、功能或性能信息，因此无法判断具体代码改动范围；可确认的事实只是构建产物对齐到 CUDA 13.0。至于“为 CUDA 13 环境用户省去自行编译”一类的收益，属于合理推断，源内容并未明说。

放到更大的生态里看，这类 nightly 轮子是 KV cache 复用能力进入实际服务栈的最后一环：框架层的缓存优化只有以匹配用户 CUDA/PyTorch 版本的二进制形式分发，才便于在既有推理引擎旁被直接试用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://arxiv.org/pdf/2510.09665">LMCache : An Efficient KV Cache Layer for Enterprise-Scale LLM ...</a></li>

</ul>
</details>

**标签**: `#LMCache`, `#KV cache`, `#LLM inference`, `#CUDA`, `#nightly release`, `#packaging`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国 10 月消费、工业与投资数据全面低于预期](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 8.0/10

中国 10 月经济数据全面低于分析师预期：社会消费品零售总额同比增长 0.4%（预期 0.8%，9 月为 1.1%），规模以上工业增加值增长 4.8%（预期 5.3%，9 月为 5.5%）；1—10 月固定资产投资同比下降 8.1%，差于预期的下降 7%，投资下滑进一步加深。10 月城镇调查失业率降至 5.1%；同期出口同比增长 35.2%，前 10 个月贸易顺差达到 1 万亿美元，为史上最快。

rss · CNBC Finance · 11月16日 03:53

**「背景」** 中国房地产下行已持续五年，削弱家庭财富并拖累消费；出口尤其是 AI 相关科技产品需求成为主要增长支撑，但美国芯片出口管制和欧盟减少对华依赖的举措令这一支撑面临风险。

**「影响」** 内需疲弱而出口激增，使中国增长更依赖外部需求：分析师警告，若全球人工智能资本开支周期回落，或欧盟进一步加码针对性贸易措施，依赖出口的中国制造商将首当其冲。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/11/09/nvidias-spy-scandal-china-chips-01156241">Nvidia’s spy scandal hands Hill hawks fresh ammo on China chips</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-03/eu-plans-changes-to-its-single-market-to-reduce-china-dependence">EU Plans Changes to Its Single Market to Reduce China ...</a></li>

</ul>
</details>

**标签**: `#China economy`, `#macroeconomic data`, `#industrial output`, `#retail sales`, `#fixed-asset investment`

---

<a id="item-finance-news-2"></a>
### [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has ties to the chipmaker](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

CNBC examines possible conflicts between Commerce Secretary Howard Lutnick&\#x27;s handling of Nvidia-related China export controls and his sons&\#x27; firm Cantor Fitzgerald&\#x27;s Nvidia stock holdings and business ties, amid Nvidia CEO Jensen Huang&\#x27;s resignation and increased scrutiny.

rss · CNBC Finance · 11月16日 12:14

**标签**: `#Nvidia`, `#export controls`, `#China`, `#conflict of interest`, `#Commerce Department`

---

<a id="item-finance-news-3"></a>
### [英特尔及 CEO 陈立武遭股东集体诉讼](https://www.investing.com/news/stock-market-news/intel-sued-by-shareholders-following-29-stock-plunge-5028171) ⭐️ 8.0/10

英特尔因 PC 需求疲软和库存问题被指隐瞒风险，在发布不及预期的业绩指引后股价暴跌 28.6%，并遭股东集体诉讼，CEO 与 CFO 同列被告。

telegram · zaihuapd · 11月16日 11:10

**标签**: `#Intel`, `#股东集体诉讼`, `#半导体`, `#业绩指引`, `#市值蒸发`

---

<a id="item-finance-news-4"></a>
### [ETF 专家：英伟达高层动荡与民主党掌控国会或重塑 AI 交易](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

CNBC《ETF Edge》节目采访的投资专家认为，在英伟达创始人兼 CEO 黄仁勋辞职、以及民主党掌控国会后可能放缓数据中心建设的背景下，大型科技股与其他 AI 芯片公司可能再次成为赢家。约克维尔艾夫斯（Yorkville Ives）周四将英伟达目标价从 300 美元下调至 225 美元，但维持买入评级；英伟达股价上周收于 162.85 美元，同期 AMD 上涨近 13%，博通涨幅相近，纳斯达克指数录得 8 月以来最佳一周。

rss · CNBC Finance · 11月16日 12:13

**「背景」** 英伟达联合创始人兼首席执行官黄仁勋于 2026 年 11 月 12 日辞职，此前有报道称他与一名疑似中国间谍及两名公司员工存在婚外情，公司由首席财务官科莱特·克雷斯临时接任。在 11 月 3 日中期选举后，民主党赢得国会控制权，部分民主党议员与地方选民转而主张限制 AI 和数据中心建设。

**「影响」** 多名受访专家认为，若投资者对英伟达失去信任，拥有现成算力的超大规模云厂商以及 AMD、博通等芯片厂商可能承接需求，而国会放缓数据中心建设反而可能推高现有算力的价值——艾夫斯估计，可能有 10%至 20%的规划数据中心无法落地，但需求仍是供给的四倍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npr.org/2026/11/12/nx-s1-6037833/jensen-huang-nvidia-stepped-down">Nvidia CEO Jensen Huang resigns amid spy scandal : NPR</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/12/nvidia-ceo-jensen-huang-resigns">Jensen Huang resigns as Nvidia CEO after alleged affairs</a></li>
<li><a href="https://fxmacrowire.com/wire/top-democrats-call-to-rein-in-ai-buildout-after-midterms-sweep">Top Democrats call to rein in AI buildout after... | FXMacro Wire</a></li>
<li><a href="https://venturesignal.org/us-midterms-data-centres-ballots-musk-474m/">US midterms – data centres lose 46 of 47 ballots as... | Venture Signal</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI trade`, `#ETF flows`, `#semiconductors`, `#US Congress/data centers`

---

<a id="item-finance-news-5"></a>
### [猪肉价格跌至近 10 年低位](https://finance.sina.com.cn/jjxw/2026-11-15/doc-iniyupuh6583194.shtml) ⭐️ 7.0/10

11 月以来中国猪肉价格跌至近 10 年低位，11 月 9 日全国生猪均价为每公斤 8.63 元，福州生猪收购价为每 50 公斤 480 至 550 元，同比下跌 20%至 26%。业内人士将下跌归因于需求减弱与生猪供应增加（养殖管理提升提高了母猪年出栏量），分析人士预计未来 6 至 8 个月猪价反弹仍可能乏力。

telegram · zaihuapd · 11月16日 03:45

**「背景」** 自 2022 年以来，中国生猪价格经历漫长下行探底，2026 年 5 月全国均价约 9.66 元/公斤，9 月第三周为 11.48 元/公斤，显示价格长期在低位波动，本轮下跌延续了此前供应增加带来的下行压力。

**「影响」** 猪价处于近 10 年低位，会直接压低养殖户的销售收入；如果分析人士预计的未来 6 至 8 个月猪价反弹乏力成为现实，养殖户承受的价格压力将持续更久，而消费者则会因猪肉零售价走低而减少食品支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://worldattention.com/stories/china-hog-and-pork-price-monitoring-september-2026-e246ee25a6">China hog prices dip pre-holiday as supply ... — WorldAttention</a></li>
<li><a href="https://www.lydd-global.com/article-domestic-and-international-news/pig-prices-fall-pig-stocks-rise-what-s-behind-the-divergence.html">China Hog Market: Futures Fall, Stocks Rise Amid Pig Cycle ...</a></li>
<li><a href="https://www.mysteel.net/analysis/5122914-hog-prices-bottom-out-amid-deep-breeding-losses">Hog prices bottom out amid deep breeding losses | Mysteel</a></li>

</ul>
</details>

**标签**: `#China pork prices`, `#agricultural commodities`, `#food inflation`, `#livestock supply`, `#consumer prices`

---

<a id="item-finance-news-6"></a>
### [中国三季度外资直接投资转为净流出 9 亿美元](https://cn.nikkei.com/china/ceconomy/64726-2026-11-16-09-03-25.html) ⭐️ 7.0/10

中国国家外汇管理局 11 月 13 日发布的 7～9 月国际收支数据显示，外资对华直接投资时隔 4 个季度转为净流出，规模为 9 亿美元，即撤资和业务缩减回收的资本超过新建工厂等新增投资。

telegram · zaihuapd · 11月16日 05:29

**「背景」** 中国国家外汇管理局按季度发布国际收支数据，今年 8 月公布的初步数据还显示外商来华直接投资保持净流入；7～9 月转为净流出意味着外资企业撤资和业务缩减回收的资本超过了新建工厂等新增投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.safe.gov.cn/en/2026/0814/2442.html">SAFE Releases Preliminary Data of the Balance of Payments for ...</a></li>

</ul>
</details>

**标签**: `#China FDI`, `#Balance of Payments`, `#Foreign Investment`, `#China Economy`, `#SAFE Data`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Lenny Rachitsky 分享：让 AI 助手接入自有 Anthropic API 的分步提示词](https://x.com/lennysan/status/2122493471982592455) ⭐️ 6.0/10

Lenny Rachitsky 在 X 上发布了一段可直接复用的提示词，主题是让 AI 助手通过\*\*用户自己的 Anthropic API 账户\*\*调用 Claude 模型，来完成指定任务（他举的例子是起草播客嘉宾简介）。整段提示词把接入过程拆成六个步骤：

\1. \*\*安全获取凭据\*\*：要求助手用安全的密钥输入框向用户索取 Anthropic API key，明确不要在聊天中明文传输；如果密钥属于某个 Anthropic workspace，也以同样方式索取 workspace ID。
\2. \*\*本地存储并写调用脚本\*\*：密钥只保存在用户自己的电脑上、不得打印出来；同时写一个小的辅助脚本调用 Anthropic Messages API，请求头包含 \`x-api-key\` 和 \`anthropic-version\`，若提供了 workspace ID 则再加 \`anthropic-workspace-id\`。
\3. \*\*列出可用模型\*\*：通过 \`GET /v1/models\` 展示该密钥可用的模型，让用户自行挑选。
\4. \*\*发测试消息验证\*\*：发送一条简短测试消息确认连通；若失败，要求助手报告确切错误（例如“credit balance too low”），以便用户到 Anthropic 的账单页面处理。
\5. \*\*改造工作流\*\*：跑通后更新助手的 skill 和相关例程，让指定模型负责写初稿、助手负责审阅与事实核查；提示词特别提醒某些模型会在正文前返回 thinking block，应只保留 text block；调用失败时回退为由助手自己起草，并说明原因。
\6. \*\*写入记忆\*\*：把这套配置存入记忆，使其持久生效。

整体看，这是一份偏工程实践的“自带密钥（BYO key）”接入模板，重点在于凭据安全、可验证的连通性测试和失败回退，而非新模型或新产品发布。

twitter · Lenny Rachitsky · 11月17日 00:54

**「背景」** Anthropic 的 Messages API 是调用 Claude 模型的接口，通常以 API key 鉴权，并通过版本头（\`anthropic-version\`）声明使用的接口版本；模型列表可通过 \`GET /v1/models\` 查询。这段提示词之所以强调“用我自己的账户”，是因为许多 AI 助手/agent 产品允许用户接入第三方模型提供方，但凭据如何传递、存放在哪里、是否会出现在对话记录里，直接关系到密钥泄露风险。提示词的应对方式是：用 secret 类型的输入字段收集密钥、只在本地保存、绝不回显。

另一类实际问题是多工作空间与环境差异：若密钥绑定特定 workspace，请求需要额外带上 \`anthropic-workspace-id\`，否则可能调用到非预期的资源或直接失败。提示词还覆盖了两个常见故障点：\*\*账户余额不足\*\*（错误信息如 credit balance too low，需在 Anthropic 账单页处理）和\*\*响应结构差异\*\*（部分模型先输出 thinking block 再输出正文，解析时应过滤掉思考内容）。最后一步“写入记忆/更新 skill”体现的是把一次性的接入配置固化为长期工作流，并约定由模型出初稿、助手复核的分工与失败回退策略。

需要说明的是，以上是提示词本身的内容与常见技术语境；该条目未附带社区评论，因此无法判断开发者社区的实际反馈或采用情况，帖子的互动数据也未提供。

**标签**: `#anthropic`, `#claude`, `#api`, `#prompt-engineering`, `#ai-assistant`, `#productivity`

---

