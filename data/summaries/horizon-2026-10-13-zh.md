# Horizon 每日速递 - 2026-10-13

> 从 54 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [黑客让欧洲超市冰箱自动除霜](#item-tech-news-1) ⭐️ 8.0/10
2. [Looped Diffusion Transformer：采样时可调循环深度的扩散模型](#item-tech-news-2) ⭐️ 8.0/10
3. [用 C 写现代 Web 应用的设计与权衡](#item-tech-news-3) ⭐️ 7.0/10
4. [WiFi 7 路由器变身 320 Msps 软件无线电接收机](#item-tech-news-4) ⭐️ 7.0/10
5. [Meta AI 发布 Muse Wonder 多模态模型](#item-tech-news-5) ⭐️ 7.0/10
6. [PS2 游戏静态重编译为 WebAssembly 的开源项目](#item-tech-news-6) ⭐️ 7.0/10
7. [Python 3.15：显式惰性导入，告别 3.10](#item-tech-news-7) ⭐️ 7.0/10
8. [U-Space 提出单遍无标签的不确定性估计方法](#item-tech-news-8) ⭐️ 7.0/10
9. [learnc：自动调优 C 代码常量，JPEG 与 WebRTC VAD 实测提升](#item-tech-news-9) ⭐️ 7.0/10
10. [Anthropic：蒸馏数据提取初步减少 90%至 99%](#item-tech-news-10) ⭐️ 7.0/10
11. [Z.ai 推出法律专用模型 GLM-Legal](#item-tech-news-11) ⭐️ 6.0/10
12. [Codex CLI 默认启用常驻自更新后台守护进程](#item-tech-news-12) ⭐️ 6.0/10
13. [AI 是工具，善用需技能](#item-tech-news-13) ⭐️ 6.0/10
14. [2026 维护者峰会聚焦 LLM、安全漏洞与继任规划](#item-tech-news-14) ⭐️ 6.0/10
15. [LineageOS 24 发布，基于 Android 17 的迭代更新](#item-tech-news-15) ⭐️ 6.0/10
16. [丘成桐牵头成立数学与 AI 实验室联盟](#item-tech-news-16) ⭐️ 6.0/10

**财经新闻**
1. [中欧就混动及电动汽车贸易达成共识：中方配额不低于其他进口来源](#item-finance-news-1) ⭐️ 8.0/10
2. [美联储哈马克：可能需要进一步加息以遏制通胀](#item-finance-news-2) ⭐️ 7.0/10
3. [皇岗口岸重建后开通，实施“一地两检”新通关模式](#item-finance-news-3) ⭐️ 7.0/10
4. [新能源汽车出口退税率 2027 年下调至 9%](#item-finance-news-4) ⭐️ 7.0/10

**推特新闻**
1. [Anthropic 宣布在降低针对 Claude 的蒸馏攻击有效性方面取得显著进展](#item-twitter-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [黑客让欧洲超市冰箱自动除霜](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

10 月 12 日的报道显示，黑客利用制冷控制器漏洞，远程触发欧洲多家超市的冰箱进入自动除霜模式，导致部分门店冷藏设备停摆，并波及配送和门店价格。法国连锁超市 Intermarché 据称成为目标，约 150 家门店受到影响。安全研究把关注点指向 Danfoss 制冷控制器及相关已知漏洞，但目前没有公开证据确认攻击者身份或完整影响范围。

hackernews · Zeekaas · 10月12日 12:16 · [社区讨论](https://news.ycombinator.com/item?id=50055304)

**「背景」** 本次攻击的目标是欧洲超市广泛部署的丹佛斯（Danfoss）制冷控制器；安全研究机构 Claroty 曾公开披露这类控制器存在多项漏洞，社区评论猜测被利用的可能是已停止支持的 SM800、SC355 等老旧型号。2026 年 8 月底美国军营小卖部冷柜疑似遭同类攻击的讨论，也让这一攻击面提前受到关注。

**「社区讨论」** 有评论者认为，涉案的可能是早已停止支持的 Danfoss SM800、SC355 等老旧控制器，而零售商利润微薄、难以按周期更换设备；也有人解释了为何冷柜会联网，称部分厂商的新设备要求联网和订阅才能运行。另有评论将此次事件与 2026 年 8 月底美国军用超市冷柜疑似遭入侵的报道联系起来，并质疑是同一组织、模仿者还是完全无关的事件。

**标签**: `#cybersecurity`, `#IoT security`, `#critical infrastructure`, `#vulnerabilities`, `#retail technology`

---

<a id="item-tech-news-2"></a>
### [Looped Diffusion Transformer：采样时可调循环深度的扩散模型](https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/) ⭐️ 8.0/10

Looped Diffusion Transformer（arXiv 2609.40305）在每个去噪步骤中多次运行同一组共享 Transformer 块，并在每个循环上加入深度监督与自调制注意力；论文声称 260M 参数循环模型在多个基准上超过 6.5 倍规模的模型，推理计算量低 4.9 倍，且固定推理预算下增加循环深度比增加去噪步数更有效。作者基于 MIT 许可的 B/16 代码与 Hugging Face（sensenova）上的权重，在 M5 Pro 上以 MPS fp32、100 个 Euler 步、CFG 6.0 复现了循环深度 1 至 4。模型按深度 4 训练，但 README 说明其他深度无需重训即可在采样时使用；作者实测深度 3 与 4 输出接近，单图耗时约 23–24 秒（深度 1）到 43–47 秒（深度 4）。

reddit · r/MachineLearning · /u/Fit-Ant2238 · 10月12日 18:13

**「背景」** 扩散模型通过多步去噪逐步从随机噪声生成图像；文本到图像的 Diffusion Transformer（DiT）通常靠堆叠更多层或增加参数量来提升生成质量。这类模型若采用循环结构，就可以在单个去噪步内多次运行同一组 Transformer 块，并通过调整循环深度在采样时灵活控制推理计算量。

**「影响」** 这项设计把循环深度变成采样期的计算-质量调节旋钮：开发者可以在不重训的情况下按单张图像调整推理开销，并在固定推理预算下优先加深循环而非增加去噪步数。但若直接套用朴素循环并不能稳定获益，复现或部署时需要保留论文提出的深度监督与自调制注意力结构；同时作者的实测显示深度 3 之后收益趋平，追求速度时可将深度设为更低值。

**标签**: `#diffusion models`, `#transformers`, `#efficient inference`, `#open source`, `#text-to-image`

---

<a id="item-tech-news-3"></a>
### [用 C 写现代 Web 应用的设计与权衡](https://prophitt.me/writing/a-modern-web-app-in-c) ⭐️ 7.0/10

技术作者 Corey Prophitt 在《A Modern Web App in C》一文中探讨了用 C 语言实现现代 Web 应用的设计思路，文章于 2026 年 10 月 12 日在 Hacker News 引发讨论。对关注 C 与服务端开发的读者而言，这是一篇个人技术写作，而非正式产品发布或行业标准变化；相关讨论主要围绕 CGI、特权分离等部署权衡展开。评论者基本认可文章的技术判断，但也提醒并发编程成本以及 Go 单二进制、C++/WebAssembly 等替代实现的存在。

hackernews · prophittcorey · 10月12日 16:13 · [社区讨论](https://news.ycombinator.com/item?id=50058528)

**「背景」** 这篇文章是开发者 Corey Prophitt 的技术笔记，记录其用 C 语言从零构建并发布商业 Web 产品（marketyour.games）的经验。据 daily.dev 摘要，该架构选择 OpenBSD 自带的 httpd 作为 Web 服务器，并通过 CGI 机制调用 C 编写的后端程序；这与常见的 nginx 反向代理加应用框架的组合形成对照。文中涉及的 pledge/chroot 等权限剥离技术，属于 Unix 服务端程序降低被攻破后影响范围的常见做法。

**「影响」** 对考虑用 C 开发 Web 应用的开发者，一个可行动的建议是先评估 CGI/FastCGI 加特权分离是否满足需求，同时把 C 的并发编程和依赖处理成本与 Go 等替代方案做对比；评论中的实际案例表明这条路可以运行得很好，但不一定是默认选择。

**「社区讨论」** 评论者 ramses0 认为文章的技术判断准确，并补充 busybox 自带 CGI 支持、rclone serve webdav 等例子；OleksandrC 则分享了一个用 C++ 写客户端（编译为 WebAssembly）和服务端、由 nginx 托管的类文明游戏项目。另有评论者以自身经历说明用 FastCGI 加 C 做线上点餐系统运行良好，而 benlivengood 指出 Go 也能单二进制免 libc，并认为 C 的并发编程是主要痛点。

<details><summary>参考链接</summary>
<ul>
<li>A Modern Web App in C | daily.dev</li>

</ul>
</details>

**标签**: `#C`, `#web development`, `#server-side`, `#security`, `#tutorial`

---

<a id="item-tech-news-4"></a>
### [WiFi 7 路由器变身 320 Msps 软件无线电接收机](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 7.0/10

开发者发布了一个开源项目，把 WiFi 7 路由器改造成采样率 320 Msps 的软件无线电接收机，为低成本宽频段 SDR 实验提供了新路径。项目代码托管在 GitHub 的 w1700k-sdr 仓库，当前展示的是接收能力而非完整收发信机，并且尚未提供明确的硬件兼容性清单。对于希望利用现成廉价硬件进行宽带接收实验的爱好者来说，这是一个可以直接尝试的开源方案。

hackernews · djfergus · 10月12日 12:41 · [社区讨论](https://news.ycombinator.com/item?id=50055593)

**「背景」** 软件定义无线电（SDR）接收通常需要专用射频前端硬件，但近年已有研究尝试复用消费级 Wi-Fi 芯片的原始采样能力。Horizon 2026 年 10 月 2 日的日报曾报道，独立项目在 ESP32 微控制器中发现了未文档化的 SDR 接收模式，可绕过固定的 Wi-Fi/蓝牙功能采集原始 IQ 基带样本；本次项目把类似思路应用到 Wi-Fi 7 路由器芯片上，将其变成 320 Msps 的 SDR 接收机，扩展了低成本宽频接收的可行路径。

**「社区讨论」** 评论区有用户指出，该开发者此前已用 ESP32 做过类似的 SDR，并推测由于芯片组相同，这个项目也可能在 Banana Pi R4 上运行；另有评论认为这是目前获得 5GHz 320 Msps 接收能力最便宜的途径之一。这些关于兼容性和成本优势的判断仍属于用户推测，而不是经过实测确认的结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rtl-sdr.com/various-projects-independently-find-hidden-sdr-capabilities-in-esp32-microcontrollers/">2026-10-02 — Hidden SDR Receive Mode Found in ESP32 Microcontrollers</a></li>

</ul>
</details>

**标签**: `#SDR`, `#WiFi 7`, `#hardware hacking`, `#open source`, `#radio`

---

<a id="item-tech-news-5"></a>
### [Meta AI 发布 Muse Wonder 多模态模型](https://research.meta.ai/blog/muse-wonder) ⭐️ 7.0/10

Meta AI 发布 Muse Wonder，一款新的多模态 AI 模型，社区已开始大规模上手测试。早期反馈显示其实际表现与官方基准存在差距，尤其是在图像转 HTML 任务上，有测试者认为它明显不如 Opus 5.5，更接近 Sonnet 或 Haiku。与此同时，有用户报告在 Muse Code 登录页面看到无关他人的账号资料，疑似存在信息暴露问题，但 Meta 尚未回应。

hackernews · meetpateltech · 10月12日 16:48 · [社区讨论](https://news.ycombinator.com/item?id=50059115)

**「背景」** Meta 此前已把 Muse 定位为面向消费者的智能体（agent）系统：Horizon 9 月 26 日的日报转述了 John Gruber 的看法，称 Muse 是首个消费者可用的智能体 AI，每个用户会在 Meta 云端拥有一个持久的 Linux 虚拟机；10 月 6 日的日报又提到 Muse 被描述为拥有全盘访问权限。Muse Wonder 是这条产品线下的新多模态模型发布，因此社区讨论多把它放在 Muse 此前的智能体定位和权限争议背景下看待。

**「影响」** 社区用户 pmuse 报告，从 Muse Code 站点用 Meta 账号登录时看到了无关人员的资料与邮箱，并收到登录验证码轰炸，且无法访问账号设置来停用账号；若该问题属实，使用 Muse Code 接入 Muse Wonder 的开发者将面临凭据与隐私泄露风险。Meta 尚未回应此事，而此前 Muse 已被曝出存在可被本地应用和终端利用的 0-day 漏洞（tool-2-1），因此建议开发者在官方确认或修复前暂缓使用该登录入口。

**「社区讨论」** 有开发者称在 Muse Code 登录时看到与自己无关的用户个人资料，怀疑 Meta 可能向他人暴露了账号和邮箱信息（pmuse）；另有测试者认为 Muse Wonder 在图像转 HTML 任务上比 Opus 5.5 差不少，更接近 Sonnet 或 Haiku，与其基准数字不符（jjcm）。这些是个人使用反馈，尚未得到 Meta 官方证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/25/john-gruber/">2026-09-26 — Gruber on Meta Muse: first consumer agentic AI, with warnings</a></li>
<li><a href="https://stratechery.com/2026/apple-and-a-hackers-future/">2026-10-06 — Apple&#x27;s controlled platform faces the AI-agent era</a></li>
<li>Muse, Meta&#x27;s extraordinarily privileged AI assistant, has a serious 0-day - Ars Technica</li>

</ul>
</details>

**标签**: `#meta-ai`, `#muse-wonder`, `#multimodal-model`, `#ai-research`, `#frontier-models`

---

<a id="item-tech-news-6"></a>
### [PS2 游戏静态重编译为 WebAssembly 的开源项目](https://github.com/snuri00/ps2-web-recomp) ⭐️ 7.0/10

一项名为 ps2-web-recomp 的开源项目尝试把 PlayStation 2 游戏静态重编译为 WebAssembly，作者在 Hacker News 以 Show HN 形式展示，代码托管在 GitHub（snuri00/ps2-web-recomp）。项目属于较新的探索，目前公开信息没有给出游戏兼容性、性能或完整度数据。

hackernews · deadxwarrior · 10月12日 06:46 · [社区讨论](https://news.ycombinator.com/item?id=50052251)

**「背景」** 静态重编译（static recompilation）与传统逐条解释指令的模拟器不同：它先分析游戏可执行文件、识别函数，再翻译成 C++ 并编译为 WebAssembly 等目标平台代码。该项目的作者在此之前已发布 PSP 版本 psp-web-recomp——分析解密后的可执行文件、寻找函数并生成 C++，以每 16 KiB 客户机代码为一个翻译单元，配合寄存器文件和 PSP 内存模型运行，并通过 HLE 内核与 WebGL2 渲染器在浏览器中运行。本次 ps2-web-recomp 是同一思路的延续，把目标平台从 PSP 扩展到同为 MIPS 指令集的 PS2。

**「影响」** 对游戏移植和模拟器开发者而言，静态重编译可能让 PS2 游戏摆脱光盘读取等待和动态模拟开销；不过由于缺少可验证的兼容性测试，现阶段还不足以替代成熟模拟器。

**「社区讨论」** 有评论者担忧这类重编译项目不像模拟器社区那样经过充分审查，存在隐藏恶意软件的风险；另一开发者则分享了为 PS Vita 做 ARM-to-WASM 转译的类似进展，称在 Chrome 手机上运行良好，但只测试了少数游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/snuri00/psp-web-recomp">GitHub - snuri 00 /psp- web - recomp : PSP games in the browser...</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#static-recompilation`, `#PS2`, `#emulation`, `#compilers`

---

<a id="item-tech-news-7"></a>
### [Python 3.15：显式惰性导入，告别 3.10](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 7.0/10

Python 3.15 已发布，并宣告 Python 3.10 终止支持；维护跨版本兼容库的开发者可以开始使用 Python 3.11 特性。新版本引入了 PEP 810 显式惰性导入（\`lazy import json\` / \`lazy from pathlib import Path\`）、PEP 798 推导式解包，以及名为 Tachyon 的标准库采样性能分析器 \`profiling.sampling\`，原 \`cProfile\` 也更名为 \`profiling.tracing\`。针对 3.15.0rc3 的测试显示，除实验性 JIT 带来约 1.2 倍提升外，整体性能与 3.14 基本持平。

rss · Simon Willison · 10月12日 18:15

**「背景」** Python 采用固定的年度小版本发布节奏，每个版本通常获得约五年的官方支持，之后进入停止维护阶段。Python 3.15 的发布意味着 Python 3.10 已到达生命周期终点，因此仍支持 3.10 的项目如今可以放弃该版本，并开始采用 Python 3.11 及之后新增的特性。

**「影响」** 维护跨版本库的开发者应停止针对 Python 3.10 的测试，并可开始使用 3.11 特性；插件化 CLI（如 LLM）的作者则可用 3.15 的显式惰性导入延迟加载 \`sentence\_transformers\` 等重依赖，避免每次启动命令都增加数秒开销。注意 \`lazy\` 语法只在 Python 3.15 中可用，跨版本代码仍需手动惰性导入。

**标签**: `#python`, `#release`, `#programming-languages`, `#open-source`, `#software-engineering`

---

<a id="item-tech-news-8"></a>
### [U-Space 提出单遍无标签的不确定性估计方法](https://www.reddit.com/r/MachineLearning/comments/1x44f9m/uspace_uncovering_when_and_why_uncertainty_arises/) ⭐️ 7.0/10

作者在 Reddit 发布 U-Space/U-Lens：一种面向开放权重推理模型的无标签单遍不确定性估计方法。它把推理结束时某一层隐藏状态与四个“怀疑方向”的内积，乘以推理词元的平均熵，用来区分歧义、信息缺失、证据冲突和一般不确定性。作者报告在 Gemma 4、Qwen3.5 和 Magistral 上以 3 个随机种子、4 个基准的评测中，该方法优于 5 遍/10 遍采样和监督基线；不过这些结果来自作者自述，当前代码是复现管线而非 pip 包。

reddit · r/MachineLearning · /u/AdRevolutionary3242 · 10月12日 15:10

**「背景」** 此前，开发者若想知道开放式推理模型“对这个答案有多确定”，通常需要多次采样投票、调用裁判模型或准备带标注数据集，成本较高。U-Space 提出不依赖这些昂贵组件，只用一次前向传播中的隐藏状态和词元熵来生成可解释的不确定性分数。

**「影响」** 对于使用开放权重推理模型的开发者，该方法提供了一种无需重采样和标注的置信度信号，可据此把低置信度答案转给更大模型或人工，或在“信息缺失”和“歧义”亮起时触发检索或澄清问题。落地时需要注意：模型若不在已提供预拟合 Jacobian lens 的列表中，需要先按作者说明自行拟合该模型特定组件。

**标签**: `#uncertainty estimation`, `#large language models`, `#interpretability`, `#reasoning models`, `#hidden states`

---

<a id="item-tech-news-9"></a>
### [learnc：自动调优 C 代码常量，JPEG 与 WebRTC VAD 实测提升](https://www.reddit.com/r/MachineLearning/comments/1x4dlbm/learnc_fit_the_constants_in_existing_c_code_to/) ⭐️ 7.0/10

learnc 是一个把现有 C 代码中的命名常量当作可优化参数、按用户用 C 编写的评分函数自动拟合并将新值写回源码的工具。开发者在 12 张 Kodak 图像上调优 stb\_image\_write.h 的 128 个量化表项、在另外 12 张上测得 BD-rate 为 9.1%（SSIM 相等），并称结果已在 libjpeg 和 scikit-image 中独立验证；对比之下，mozjpeg 的量化表为 2.7%。对 Google WebRTC VAD 的 vad\_core.c 全部常量用 LibriParty dev 调优后，F1 从 0.810 升至 eval 集上的 0.859。公告同时说明限制：JPEG 在 1 bpp 以下无增益，工具适合数十到数百个常量，不适合大规模权重集；代码以 MIT 许可发布。

reddit · r/MachineLearning · /u/keep\_up\_sharma · 10月12日 20:51

**「背景」** 许多 C 程序（编解码器、信号处理库）的性能依赖手调常量和查找表，传统做法是在固定管线外反复编译、测试和修改。learnc 把这类常量直接作为可优化参数，在同一份 C 源码上形成“自动寻优并写回”的闭环，因此不需要重构程序结构，也不依赖大型参数集。

**「影响」** 维护者可以在不重构 C 实现的情况下，用自定义指标（如码率—质量、分类 F1）自动替换关键常量；但采用前应在自己的数据集上复现，因为公告只覆盖 JPEG 和 WebRTC VAD 两个任务，且明确说明 JPEG 低于 1 bpp 无增益、可调常量规模有限。

**标签**: `#code optimization`, `#C`, `#JPEG`, `#WebRTC VAD`, `#automated tuning`

---

<a id="item-tech-news-10"></a>
### [Anthropic：蒸馏数据提取初步减少 90%至 99%](https://www.anthropic.com/research/distillation-defenses) ⭐️ 7.0/10

Anthropic 于 10 月 12 日表示，初步证据显示其针对模型蒸馏攻击的新防护已使从 Claude 提取的数据减少约 90% 至 99%，并封禁数万相关账号，部分攻击账号在发起后不到两小时即被封。具体措施包括限制推理内容跨会话、模型和账号流转，部署双阶段分类器并持续修补绕过手法。公司称误报率低于 0.1%，但这是 Anthropic 自述的初步结果，部分开发者需要更新集成，被拦截的请求仍可能收费。

telegram · zaihuapd · 10月13日 01:25

**「背景」** 模型蒸馏攻击通常通过大量滥用 API 请求诱导模型泄露推理内容或训练数据，再用于训练竞品模型。本月初（10 月 2 日）Horizon 日报曾报道 OpenAI 披露已破坏一场此类协调攻击，称其峰值涉及逾 4,000 个用户和 16,000 次请求，并关联到 Moonshot AI 相关人员；此次 Anthropic 的新防护是又一家主要模型厂商针对同一类攻击公布的防御进展。

**「影响」** 对使用 Claude 集成的开发者而言，需要按 Anthropic 的提示更新集成以降低误拦截影响；同时，被拦截的请求仍可能被计费，因此调用成本未必会随着防护生效而下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/">2026-10-02 — OpenAI disrupts model distillation campaign tied to Moonshot AI staff</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI security`, `#model distillation`, `#LLM protections`, `#Claude`

---

<a id="item-tech-news-11"></a>
### [Z.ai 推出法律专用模型 GLM-Legal](https://z.ai/blog/glm-legal) ⭐️ 6.0/10

Z.ai 于 2026 年 10 月宣布发布 GLM-Legal，一个面向法律领域的专用大语言模型。来源信息未提供具体版本、基准测试成绩或可用渠道，因此目前只能确认这是该实验室推出的法律专用模型产品，而非已经独立验证的技术突破。公告引发了关于法律 AI 实用性和供应商隐私保护的讨论。

hackernews · ilreb · 10月12日 16:11 · [社区讨论](https://news.ycombinator.com/item?id=50058507)

**「背景」** GLM-Legal 是 Z.ai（智谱）在现有 GLM 系列基础上推出的垂直领域模型。该系列最新的开源权重旗舰是 GLM-5.3；Horizon 9 月 30 日的日报曾转述 Anthropic 的评估，称 GLM-5.3 在基准测试中能够端到端构建网络攻击，且多次越狱测试中安全措施可被绕过。这些先前版本构成了 GLM-Legal 的模型血缘，也提示其可能继承的安全与隐私争议背景。

**「影响」** 对于考虑在合同审查、诉讼文书等工作流中使用 GLM-Legal 的法律从业者，社区讨论提示需要先验证供应商的数据处理方式是否可接受，并确保最终建议有人工律师复核，尤其是涉及当事人法律权利、财务或人身利益的场景。

**「社区讨论」** 评论中既有对法律 AI 的积极体验，例如 jedberg 提到用 Claude 审查模板化 OEM 合同并获得了律师认可；也有对 Z.ai 的严重保留意见，fireflysentinel 指出该公司曾被曝在每次提示前对整个工作区进行快照，因此难以信任其法律产品。victor9000 还强调应保持“人在回路”的审核机制，而 otterley 则对某个基准测试中 20% 的通过率表示不以为然。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">2026-09-30 — Anthropic finds GLM-5.3 can build end-to-end cyberattacks near Claude Mythos</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">zai -org/ GLM -5.3 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#legal-ai`, `#llm`, `#glm`, `#privacy`, `#ai-ethics`

---

<a id="item-tech-news-12"></a>
### [Codex CLI 默认启用常驻自更新后台守护进程](https://github.com/openai/codex/issues/48195) ⭐️ 6.0/10

据 Hacker News 讨论，OpenAI 的 Codex CLI 默认会安装一个持久运行、可自动更新的后台守护进程，并在启动时向 ~/.codex 写入 pid 文件、锁文件等数据。目前没有文档化的设置可以关闭它，但社区用户指出可通过 ~/.codex/config.toml 中的 \`\[features\] daemon\_auto\_start = false\` 禁用。另有用户报告旧版本文件占用大量磁盘空间，以及自动更新过程中破坏文件权限等问题。

hackernews · whimblepop · 10月12日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=50060694)

**「背景」** Codex CLI 自 0.157.0 起将守护进程自动启动改为稳定默认：每次打开交互式会话都会自动启动一个常驻后台服务进程，除非已有进程在运行，相关文章称这是“安静但深远的架构转变”，取代了以往每个会话直接调用 CLI 的一次性模式。GitHub issue 中已有用户建议将该功能改为默认关闭的 opt-in，并希望后台进程在最后一个客户端断开后自动退出。

**「影响」** Codex CLI 用户如不希望后台守护进程常驻，可在 ~/.codex/config.toml 中设置 \`\[features\] daemon\_auto\_start = false\` 来关闭，并应留意清理 ~/.codex 下累积的旧版本文件以及 pid、lock 文件。若已启用自动更新，还需检查 .git 目录是否因权限异常变成只读，否则可能频繁阻塞任务执行。

**「社区讨论」** 多名评论者分享了实测问题：有人称旧版本累计占用约 12GB 磁盘，有人称自动更新会随机破坏权限、使 .git 变成只读并频繁阻塞任务。另有人指出这种后台版本管理并非 Codex 独有，Claude Code 也会保留多个旧版本并运行后台进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/openai/codex/issues/48195">CLI: make `daemon_auto_start` opt-in — a persistent, self ...</a></li>
<li><a href="https://codex.danielvaughan.com/2026/09/25/codex-cli-daemon-auto-start-stable-default-v0157/">Daemon Auto-Start Is Now the Stable Default in Codex CLI v0 ...</a></li>

</ul>
</details>

**标签**: `#OpenAI Codex`, `#CLI`, `#AI coding tools`, `#background daemon`, `#software engineering`

---

<a id="item-tech-news-13"></a>
### [AI 是工具，善用需技能](https://yyhh.org/blog/2026/10/ai-is-a-tool/) ⭐️ 6.0/10

一篇观点文章提出，熟练使用 AI 是一项需要培养的技能，社区讨论则聚焦于“提示词技巧是否正在过时”以及专业人员应如何管理 AI 带来的复杂度。评论者意见分歧明显：有人认为早期依赖的上下文管理和特制提示词技巧已被新模型淘汰，核心变成“知道该问什么”；也有人担心 AI 会加速认知能力下降，并让项目复杂度迅速超出人工可控范围。

hackernews · layer8 · 10月12日 21:40 · [社区讨论](https://news.ycombinator.com/item?id=50063427)

**「背景」** 这篇文章属于生成式 AI 普及后关于“提示工程”价值的持续争论：早期大语言模型对提示词构造、上下文管理和特殊指令格式较为敏感，用户需要专门技巧才能获得可用输出，因此“会使用 AI”一度被视为一项需要练习的技能。随着模型能力提升，提示技巧是否依然重要、专业人士应如何应对 AI 带来的复杂性，成为软件工程与 AI 实践者关注的话题。

**「社区讨论」** 评论者 extr 认为，精调提示词和上下文管理的技巧已经过时，当前的关键是“知道该问什么”；dzink 则警告，缺乏护栏的 AI 会迅速制造人类难以管理的复杂度，专业人士的职责正在于遏制这种复杂度。另有评论者表达了对 AI 削弱人类认知和教育的长期担忧，也有人分享了用 Gemini 辅助贝叶斯分析的具体经历，但这些都属于个人观点而非已验证结论。

**标签**: `#AI tools`, `#LLM usage`, `#software engineering`, `#complexity management`, `#AI skills`

---

<a id="item-tech-news-14"></a>
### [2026 维护者峰会聚焦 LLM、安全漏洞与继任规划](https://lwn.net/Articles/1099594/) ⭐️ 6.0/10

按计划于 2026 年 10 月 8 日在捷克布拉格举行的年度维护者峰会，是一场约 30 名内核开发者受邀参加、为期一天的闭门会议。讨论重点被大型语言模型（LLM）对开发社区的影响所主导，其余时间则用于探讨安全漏洞与长期继任规划。报道仅概述了议题，未披露具体决议或可验证的结果。

rss · LWN.net · 10月12日 15:27

**「背景」** 维护者峰会是每年一次、仅限受邀的内核开发者参加的一天会议，约 30 人出席，旨在讨论那些不适合通过邮件列表解决的策略性问题。

**标签**: `#linux-kernel`, `#open-source`, `#large-language-models`, `#maintainers-summit`

---

<a id="item-tech-news-15"></a>
### [LineageOS 24 发布，基于 Android 17 的迭代更新](https://lwn.net/Articles/1099950/) ⭐️ 6.0/10

LineageOS 项目宣布发布 LineageOS 24.0，这是一个基于 Android 17 代码库重新构建的主要版本。官方表示，由于此前已适应 Google 在过去多个版本中的重构，这次迁移比预期更快，主要变化是迭代改进和 UI/UX 优化。该版本面向仍使用 LineageOS 支持的移动设备的用户和社区维护者。

rss · LWN.net · 10月12日 13:13

**「背景」** LineageOS 是一个面向移动设备的开源 Android 发行版，通常通过社区更新延长旧设备的可用时间。Android 17 已于 2026 年 6 月发布，项目此次将自身改动全部 rebase 到该代码库，并提到 2026 年 12 月 24 日将是 LineageOS 成立 10 周年。

**标签**: `#LineageOS`, `#Android`, `#Open Source`, `#Mobile OS`, `#Release`

---

<a id="item-tech-news-16"></a>
### [丘成桐牵头成立数学与 AI 实验室联盟](https://www.beijing.gov.cn/fuwu/lqfw/gggs/202610/t20261012_4897748.html) ⭐️ 6.0/10

菲尔兹奖得主、清华大学讲席教授丘成桐牵头成立丘成桐数学与人工智能实验室联盟，联盟于 10 月 11 日在清华大学成立，由丘成桐任主席，汇集超过 1000 名科学家。联盟计划自主开发中国数学专用大模型，建设 AI 辅助数学研究基础设施，并拓展至量子计算、生命科学、金融经济等交叉领域。丘成桐称 AI 对数学的冲击“像海啸来了”，应主动冲浪而非回避。目前相关表述属于联盟成立时的计划，尚未披露具体模型版本、时间表或技术成果。

telegram · zaihuapd · 10月12日 03:00

**「背景」** 将大语言模型用于数学推理是当前国际研究的热点方向，但通用模型在严格证明和数学专用工具链上的适配仍有限。菲尔兹奖得主、清华大学讲席教授丘成桐牵头联合多家机构，于 10 月 11 日在清华大学成立联盟并出任主席，汇集超过 1000 名科学家，目标是自主开发中国数学专用大模型，并建设 AI 辅助数学研究的基础设施。

**标签**: `#mathematics`, `#artificial intelligence`, `#large language models`, `#research alliance`, `#China`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中欧就混动及电动汽车贸易达成共识：中方配额不低于其他进口来源](https://www.mofcom.gov.cn/xwfb/sjfzrfb/art/2026/art_4d502e1d49fd4480b39a6cfd0d752038.html) ⭐️ 8.0/10

中国商务部称，中欧在贸易投资磋商机制下就混动汽车和电动汽车贸易达成多项共识。混动汽车安排以 2025 年为基础向上调整，中方配额不低于欧方其他进口来源地；电动汽车方面，欧方将继续推进企业价格承诺等程序。

telegram · zaihuapd · 10月12日 06:19

**「背景」** 此前，欧盟对中国电动汽车发起反补贴调查并于 2024 年公布终裁高额税率，中方随后将初裁和终裁措施诉至世贸组织争端解决机制；双方之后在贸易投资磋商机制下就价格承诺等安排持续磋商。

**「影响」** 对向欧盟出口混动和电动汽车的中国车企而言，这次以 2025 年为基线的向上配额安排意味着出口空间有更明确的政策预期，且中方配额不低于其他进口来源地，有助于降低被差别对待的风险；欧方继续推进价格承诺等程序，也会影响后续出口价格和销量安排。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20240915/herald/9ebf8e23bb9765788fb45b25556c2215.html">21jingji.com/article/20240915/herald/9ebf8e23bb9765788fb45b25556...</a></li>
<li><a href="https://news.qq.com/rain/a/20241128A094PQ00?suid=&amp;media_id=">news.qq.com/rain/a/20241128A094PQ00?suid=&amp;media_id=</a></li>
<li><a href="https://stock.10jqka.com.cn/20241104/c663153624.shtml">stock.10jqka.com.cn/20241104/c663153624.shtml</a></li>
<li><a href="https://news.qq.com/rain/a/20261011A07LQR00">中欧经贸磋商取得积极进展：联合声明列出16条成果共识，双方在符合世...</a></li>
<li><a href="https://www.toutiao.com/article/7595021617957175835/">出口欧洲汽车提供最低限价、销量限额，中欧电动汽车案达成共识</a></li>
<li><a href="https://www.mofcom.gov.cn/syxwfb/art/2026/art_d6a5e2c4e62740868c7f1a7cd061f84a.html">商务部新闻发言人就中欧混动汽车、电动汽车磋商共识答记者问</a></li>

</ul>
</details>

**标签**: `#中国-欧盟贸易`, `#电动汽车`, `#混动汽车`, `#贸易政策`, `#汽车产业`

---

<a id="item-finance-news-2"></a>
### [美联储哈马克：可能需要进一步加息以遏制通胀](https://www.cnbc.com/2026/10/12/beth-hammack-fed-inflation-policy.html) ⭐️ 7.0/10

克利夫兰联储行长贝丝·哈马克周一表示，可能需要更紧缩的货币政策才能让通胀回到 2%目标，并称目前“限制性”政策立场是合适的；她倾向于快速小幅调整，以免日后需要更大动作。她援引 8 月 PCE 同比上涨 3.4%、核心 PCE 同比涨 3%的数据，预计通胀回落需要“一些时间”，并警告持续高通胀可能让“通胀心态”扎根。

rss · CNBC Finance · 10月12日 17:15

**「背景」** 哈马克是美联储利率决策委员会今年有投票权的委员，她是在全国商业经济协会年会上发表事先准备的讲话。美联储上月进行了三年来首次加息，9 月会议纪要显示官员们可能再次投票加息，但没有给出明确时间。

**标签**: `#Federal Reserve`, `#interest rates`, `#inflation`, `#monetary policy`, `#PCE`

---

<a id="item-finance-news-3"></a>
### [皇岗口岸重建后开通，实施“一地两检”新通关模式](https://sc.isd.gov.hk/TuniS//www.info.gov.hk/gia/general/202610/09/P2026100900280.htm) ⭐️ 7.0/10

重建后的皇岗口岸于 2026 年 10 月 12 日上午 6 时 30 分正式开通，实施“一地两检”（在同一地点办理深港两地检查）及“合作查验、一次放行”，提供 24 小时通关。香港政府公布，整体通关时间由原来约 30 分钟缩短至约 5 分钟，自助通道最快约 20 秒完成；初期预计每日可处理高峰流量 20 万人次，未来可提升至 30 万人次。

telegram · zaihuapd · 10月12日 05:12

**「背景」** 皇岗口岸是深港之间重要的 24 小时客运陆路口岸；此次重建后定位为深港最重要的 24 小时客运陆路口岸，并采用“一地两检”和“合作查验、一次放行”，即把两地查验安排在同一地点合作完成，旅客只需一次放行。

**「影响」** 对经常往返深圳与香港的跨境旅客和车辆，通关时只需在口岸一次完成检查，可减少重复排队，节省过关时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260702/herald/e15dde352d5131fdda1938d6d4701dfe.html">5分钟通关，24小时不打烊！ 深圳新 皇 岗 口 岸 开通在即 - 21经济网</a></li>

</ul>
</details>

**标签**: `#皇岗口岸`, `#一地两检`, `#跨境交通`, `#香港`, `#通关效率`

---

<a id="item-finance-news-4"></a>
### [新能源汽车出口退税率 2027 年下调至 9%](https://www.news.cn/20261012/9709731f470b42f9a84825c2e4eb914b/c.html) ⭐️ 7.0/10

财政部、税务总局 10 月 12 日公告，自 2027 年 4 月 1 日起，将新能源汽车增值税出口退税率由 13%下调至 9%，并取消电子烟设备装置的增值税出口退税。

telegram · zaihuapd · 10月12日 11:00

**「背景」** 出口退税是出口商品在报关出口后退还其已缴纳的增值税，退税率下调意味着出口企业可获得的税收返还减少。

**「影响」** 对新能源汽车出口企业而言，出口环节获得的税收返还将减少；电子烟设备出口企业则彻底失去该项退税。

**标签**: `#新能源汽车`, `#出口退税`, `#税收政策`, `#中国`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Anthropic 宣布在降低针对 Claude 的蒸馏攻击有效性方面取得显著进展](https://x.com/AnthropicAI/status/2109795898909950247) ⭐️ 7.0/10

Anthropic 官方账号发布推文称，过去几个月里，他们在降低针对 Claude 的蒸馏攻击有效性方面取得了显著进展。推文表示相关说明已包含在一篇附有链接的文章中，但推文本身未提供具体技术细节，主要引导读者阅读完整内容。

twitter · AnthropicAI · 10月12日 23:58

**「背景信息」** 这条推文来自 Anthropic 官方账号（2026-10-12），宣布近几个月在降低针对 Claude 的蒸馏攻击有效性方面取得重大进展，并附上详细说明的帖子链接。推文本身没有给出技术细节。Anthropic 在相关说明中称，已识别出利用约 24,000 个欺诈账户进行的协调蒸馏攻击，目的是提取 Claude 的能力（tool-1-2）。媒体报道进一步指出，Anthropic 曾指控 DeepSeek、Moonshot 和 MiniMax 使用 24,000 个虚假账户蒸馏 Claude 的能力，背景是美国官员讨论针对中国 AI 进展的出口管制（tool-1-3）；另有汇总称 Anthropic 指责中国实验室对 Claude 发起约 1,600 万次“蒸馏攻击”，OpenAI 的 Sam Altman 则称中国进展“显著”且“快得惊人”（tool-1-1）。行业背景方面，OpenAI 在 10 月初披露破坏了一场与 Moonshot AI 员工有关的模型蒸馏活动（tool-2-2）。这些外界报道和行业动作有助于理解本次声明，但推文本身未提供具体指标或方法。社区评论：暂无可用社区评论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/olliebone_anthropic-and-openai-are-sounding-the-alarm-activity-7432003236405915649-iZoI">Anthropic and OpenAI Sound Alarm on Chinese AI Progress | LinkedIn</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/02/23/anthropic-accuses-chinese-ai-labs-of-mining-claude-as-us-debates-ai-chip-exports/">Anthropic accuses Chinese AI labs of mining Claude as... | TechCrunch</a></li>
<li><a href="https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/">2026-10-02 — OpenAI disrupts model distillation campaign tied to Moonshot AI staff</a></li>

</ul>
</details>

**标签**: `#AI security`, `#distillation attacks`, `#Anthropic`, `#Claude`

---

