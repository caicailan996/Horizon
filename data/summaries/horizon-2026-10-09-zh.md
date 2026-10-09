# Horizon 每日速递 - 2026-10-09

> 从 55 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [清华团队率先研制成功钍-229 核光钟](#item-tech-news-1) ⭐️ 9.0/10
2. [LWN 每周版汇总内核与开源项目更新](#item-tech-news-2) ⭐️ 8.0/10
3. [Ecosia 弃用 Mistral 转向中国开源 AI 模型](#item-tech-news-3) ⭐️ 7.0/10
4. [不明攻击者用中国开源工具 ARTEX 攻击韩国金融机构](#item-tech-news-4) ⭐️ 7.0/10
5. [OpenAI 封禁俄伊两起 ChatGPT 影响行动](#item-tech-news-5) ⭐️ 7.0/10
6. [Whistle：仅 16.9 MB 的本地语音转文本模型](#item-tech-news-6) ⭐️ 6.0/10
7. [特朗普政府暂停微软绿卡项目参与](#item-tech-news-7) ⭐️ 6.0/10
8. [两个竞争补丁争夺 swap 缓存槽解耦方案](#item-tech-news-8) ⭐️ 6.0/10
9. [LWN 汇总多发行版安全更新：内核、Firefox、Chromium 等](#item-tech-news-9) ⭐️ 6.0/10
10. [马斯克宣布 Grok Bot 接入 Claude](#item-tech-news-10) ⭐️ 6.0/10
11. [Lunara：主动学习训练的次百亿参数图像生成模型](#item-tech-news-11) ⭐️ 6.0/10

**财经新闻**
1. [盘前主要公司动态：Wolfspeed 获国防部贷款，Broadcom 与 OpenAI 融资谈判](#item-finance-news-1) ⭐️ 7.0/10
2. [标普预测中国房价 2028 年三季度触底，大城市或明年反弹](#item-finance-news-2) ⭐️ 7.0/10
3. [华为重新押注自研芯片手机，汽车业务交付下滑](#item-finance-news-3) ⭐️ 7.0/10
4. [Manus 母公司完成超 5 亿美元融资](#item-finance-news-4) ⭐️ 7.0/10
5. [人社部就新就业形态劳动者权益保障办法公开征求意见](#item-finance-news-5) ⭐️ 7.0/10
6. [OpenAI 被曝年化收入比市场普遍报道少约 200 亿美元](#item-finance-news-6) ⭐️ 7.0/10
7. [美政府以欺诈为由暂停微软绿卡申请资格](#item-finance-news-7) ⭐️ 7.0/10

**推特新闻**
1. [Anthropic 推出 Cyber Mission，聚焦关键基础设施与开源软件安全](#item-twitter-news-1) ⭐️ 7.0/10
2. [Anthropic 发布 OSS Scanner：免费为开源项目扫描漏洞并提供修复建议](#item-twitter-news-2) ⭐️ 7.0/10
3. [天体物理学家借助 Claude Science 创建首张完整紫外天空地图](#item-twitter-news-3) ⭐️ 7.0/10
4. [Anthropic 深化对科学研究的承诺：投入 1.5 亿美元于创世纪使命，并向 15 个以上联邦机构开放 Claude](#item-twitter-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [清华团队率先研制成功钍-229 核光钟](https://www.nature.com/articles/s41586-026-11122-1) ⭐️ 9.0/10

清华大学研究团队利用自主研制的 148 纳米连续波真空紫外激光和掺钍-229 氟化钙晶体，在国际上率先研制出核光钟并实现稳定运行，成果发表于《自然》。核光钟以钍-229 原子核能级跃迁为计时基准，有望成为新一代时间频率基准，并服务于卫星导航、深空探测等高精度计时场景。

telegram · zaihuapd · 10月8日 05:19

**「背景」** 传统光钟以原子外层电子的能级跃迁作为计时基准，而核光钟改用原子核内部的能级跃迁。钍-229 的原子核存在能量极低的同核异能态，可用真空紫外激光直接驱动，因此被视为实现新一代时间频率基准的关键候选体系。

**「影响」** 对依赖高精度时间同步的卫星导航、深空探测等领域，这一成果首次展示了可稳定运行的核光钟，为下一代时间频率基准提供了以原子核跃迁为核心的新技术路线。不过，其应用前景目前仍以“有望”表述，要替代现有原子钟或光钟，还需要进一步验证长期稳定度并推进工程化。

**标签**: `#nuclear clock`, `#time-frequency standard`, `#thorium-229`, `#quantum physics`, `#precision measurement`

---

<a id="item-tech-news-2"></a>
### [LWN 每周版汇总内核与开源项目更新](https://lwn.net/Articles/1097859/) ⭐️ 8.0/10

LWN.net 于 2026 年 10 月 8 日发布每周版，以目录形式汇集了 Linux 内核缺陷、Rust 智能指针、Gentoo 的 Chromium 打包、LAVD 调度器、Python 随机数模块，以及 OpenSSH 10.6、Rust 1.99.0、Picard 3.0、Zig 0.17 等报道入口。该条目本身仅提供链接列表，未包含各项目的具体细节，完整文章面向 LWN 读者提供。

rss · LWN.net · 10月8日 00:22

**「背景」** 本期 LWN 周刊是围绕近期开源发布的综述。外部资料确认其中多项已于本周正式推出：OpenSSH 10.6 于 10 月 6 日发布，重点增强后量子加密，并提到团队收到大量 AI 辅助的安全漏洞报告（tool-1-1；tool-1-2；tool-1-3）；Rust 1.99.0 稳定版可通过 rustup 更新（tool-2-1）；Zig 0.17.0 在时隔五个月后发布（tool-3-1；tool-3-3）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.tuxmachines.org/n/2026/10/07/OpenSSH_10_6_released.shtml">Tux Machines — OpenSSH 10 . 6 released</a></li>
<li><a href="https://trashbox.ru/link/2026-10-06-openssh-10-6-post-quantum-security">Вышел OpenSSH 10 . 6 с усилением пост-квантового шифрования...</a></li>
<li><a href="https://habr.com/ru/news/1091226/">Вышел OpenSSH 10 . 6 / Хабр</a></li>
<li><a href="https://alestaweb.com/haber/rust-1-99-yenilikleri-c-variadic-fonksiyon-size-of-val-raw-rehberi">Rust 1 . 99 Yenilikleri: C Variadic Fonksiyonlar ve Yeni API | Alesta WEB</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>
<li><a href="https://www.opennet.ru/opennews/art.shtml?num=66391">Выпуск языка программирования Zig 0 . 17 .0 | Новости</a></li>

</ul>
</details>

**标签**: `#linux-kernel`, `#open-source`, `#software-engineering`, `#development-news`, `#systems-programming`

---

<a id="item-tech-news-3"></a>
### [Ecosia 弃用 Mistral 转向中国开源 AI 模型](https://www.politico.eu/article/germany-ecosia-search-engine-mistral-china-open-source-ai/) ⭐️ 7.0/10

总部位于柏林的搜索引擎 Ecosia 已放弃法国 AI 实验室 Mistral，转而采用包括中国模型在内的开源 AI 模型。CEO 克里斯蒂安·克罗尔表示，团队对 Mistral 的质量感到失望，认为其模型已落后竞争对手一年。Ecosia 被德国联邦环境部和英国国家医疗服务体系等机构使用，该切换将影响这些用户。目前尚不清楚 Ecosia 具体集成了哪些中国开源模型。

telegram · zaihuapd · 10月8日 10:08

**「背景」** 此前 Ecosia 已在 AI 搜索功能中使用 Mistral 的模型。10 月 7 日的日报曾报道，Mistral 发布了从零训练的大型语言模型 Mistral Large 4，称其在视觉、网络安全和编程等基准上的得分接近 Kimi K3、Claude Sonnet 5.5 等顶尖模型。现在 Ecosia 首席执行官公开表示对 Mistral 的模型质量失望，认为其已落后竞争对手约一年，因此决定改用包括中国模型在内的开源模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/mistral-large-4//">2026-10-07 — Mistral Large 4: New LLM Trained on 3,800 Grace Blackwell GPUs</a></li>

</ul>
</details>

**标签**: `#AI`, `#open source`, `#Ecosia`, `#Mistral`, `#search engine`

---

<a id="item-tech-news-4"></a>
### [不明攻击者用中国开源工具 ARTEX 攻击韩国金融机构](http://xcai.pro/) ⭐️ 7.0/10

CrowdStrike 在 10 月 7 日的报告中称，一名身份不明的攻击者在 9 月底至 10 月初针对韩国金融机构实施攻击并窃取数据，行动使用了中国开发的开源智能体渗透工具 ARTEX，并通过中转站 xcai.pro 调用 DeepSeek v4.1-flash，同时辅以智谱 GLM-5.3 与 Grok 4.6。公司以中等置信度判断对方为中文使用者、动机偏财务，但尚未归因到已知组织。报告还披露了攻击者控制目录中的 Claude Code 会话记录及 ARTEX 配置，并称会话中出现的年龄、华南理工大学及广东茂名等细节可能属于攻击者本人。身份、泄露规模均未证实，疑似使用的中转站目前已经关闭。

telegram · zaihuapd · 10月8日 10:32

**「背景」** Horizon 10 月 5 日的日报曾报道，Shinhan、Kookmin、Hana、BNK Busan 四家韩国银行报告员工或外包供应商系统发生数据泄露，其中新韩银行的贷款代理查询系统遭攻击三天、涉及约 25,729 名客户，金融监管机构随后扩大对员工业务系统和外部合作伙伴的 IT 安全检查。CrowdStrike 10 月 7 日的最新报告进一步将攻击工具指向中国开发的开源智能体渗透工具 ARTEX 及中转站 xcai.pro，但攻击者身份和泄露规模仍未被证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thelec.net/news/articleView.html?idxno=14402">2026-10-05 — South Korean Regulators Expand IT Checks After Four Banks Report Data Breaches</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#cybersecurity`, `#open-source`, `#llm-agents`, `#crowdstrike`

---

<a id="item-tech-news-5"></a>
### [OpenAI 封禁俄伊两起 ChatGPT 影响行动](https://openai.com/index/disrupting-ai-enabled-false-front-operations/) ⭐️ 7.0/10

OpenAI 封禁了来自俄罗斯和伊朗的两个隐蔽影响行动，二者均滥用 ChatGPT 生成虚假内容。俄罗斯行动疑似冒用身份控制拉美一个研究平台，传播损害乌克兰声誉及影响当地政治的虚假信息，被 OpenAI 评为影响行动突破量表第 5 类，这是其开始报告以来首次达到该级别。伊朗行动以 7 个“记者”人设向全球中小网络媒体投稿并批量生成社交媒体评论，被定为第 4 类，产出近 100 篇署名文章。两起行动均结合传统手段与 AI 生成内容，部分内容已进入主流媒体。

telegram · zaihuapd · 10月8日 15:52

**「背景」** OpenAI 所称“虚假前台”（false-front）行动，是指以伪造记者署名、智库等合法身份包装 AI 生成内容，以增强其可信度并进入主流媒体的隐蔽影响操作。OpenAI 用影响行动突破量表为这类行动定级，此次俄罗斯行动获第 5 类、伊朗行动获第 4 类，其中第 5 类是该量表开始报告以来首次启用的最高级别。

**「影响」** 这些行动的部分 AI 生成内容已进入主流媒体，表明现有审核机制难以完全阻断 AI 辅助的虚假信息传播，平台和媒体需加强内容溯源与身份验证能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/disrupting-ai-enabled-false-front-operations/">Disrupting AI - enabled “ false front ” operations | OpenAI</a></li>
<li><a href="https://cellcog.ai/blog/openai-false-front-operations/">OpenAI &#x27;s False - Front Report: Its First Category 5 Takedown | CellCog</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI safety`, `#disinformation`, `#influence operations`, `#cybersecurity`

---

<a id="item-tech-news-6"></a>
### [Whistle：仅 16.9 MB 的本地语音转文本模型](https://cactuscompute.com/blog/whistle) ⭐️ 6.0/10

Whistle 是一个大小仅 16.9 MB 的语音转文本模型，专为本地设备处理设计。实际测试显示，其准确率远低于大型模型：在 170 条消息的测试中，Qwen ASR（1.7B 参数）正确识别了 168 条，而 Whistle 仅正确识别 70 条。该模型不支持流式输出，但已开源并提供代码和模型权重。其核心优势是超小体积，适合资源受限的边缘场景，但精度取舍限制了通用用途。

hackernews · gmays · 10月8日 16:59 · [社区讨论](https://news.ycombinator.com/item?id=50008427)

**「背景」** 大多数高精度语音转文本模型体积庞大（如 Qwen ASR 的 1.7B 参数），需要 GPU 加速。Cactus Compute 推出的 Whistle 使用 Needle 运行时，将多语言转录模型压缩至 16.9 MB，可完全在本地 CPU 上运行。

**「影响」** 对于需要完全本地化、低功耗语音识别的用户（如 Home Assistant 集成），Whistle 的 16.9 MB 体积使得它能在老旧或低性能设备上运行。但用户必须接受约 41% 的识别准确率（对比大型模型约 99%），且无法用于需要逐字流式输出的实时转录场景。开发者需自行评估任务对精度的容忍度。

**「社区讨论」** 社区用户对比测试指出 Whistle 准确率显著低于 Qwen ASR（70/170 vs 168/170），但通过改用“JEV”模式（类似结巴分词）可改善实用性。另有用户报告模型在转录 TV 剧集时，会反复输出“Thank you.”长达 60 秒，表明存在静音或语种切换时的退化行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cactuscompute.com/blog/whistle">Whistle : Speech to Text in 16 . 9 MB | Cactus</a></li>
<li><a href="https://runtimewire.com/article/cactus-whistle-16-9mb-local-speech-model">Cactus Compute releases a 16 . 9 MB speech model for local CPUs</a></li>

</ul>
</details>

**标签**: `#speech-to-text`, `#machine learning`, `#edge computing`, `#open source`, `#AI tools`

---

<a id="item-tech-news-7"></a>
### [特朗普政府暂停微软绿卡项目参与](https://apnews.com/article/h1b-visa-program-vance-microsoft-e7b3a407f822702b269ee277d21343ea) ⭐️ 6.0/10

据美联社 2026 年 10 月 8 日报道，特朗普政府已暂停微软参与一项绿卡项目。该决定与围绕 H-1B 签证招聘外国劳工的争议相关，并引发对执法是否具有选择性的讨论。目前细节有限，暂停期限、涉及的签证类别以及微软的回应均未披露。

hackernews · alephnerd · 10月8日 15:15 · [社区讨论](https://news.ycombinator.com/item?id=50006832)

**「背景」** H-1B 绿卡项目是雇主为持 H-1B 签证的外籍员工申请美国永久居留的通道。在此次暂停微软之前，特朗普政府已着手整改该项目并加收签证费用，还曾中止包括塔塔咨询在内的八家 IT 公司的参与资格，理由是这些企业利用该程序绕过美国本土员工、大量聘用外籍劳工。

**「影响」** 对微软而言，暂停参与意味着其通过该绿卡项目为外籍员工申请永久居留的渠道暂时受阻，可能影响相关人才的在美留任与后续招聘。评论者提醒，其他科技公司也应重新审查自身的 H-1B 招聘和绿卡申请操作，避免因同类问题成为执法目标。

**「社区讨论」** 评论中，最集中的争论是执法公平性：有用户引述万斯关于企业以“无人应聘”为由替换美国工人的说法，认为这类操作普遍存在，现在却不对称地用于盟友；也有用户以微软与 Wipro 为例，担心暂停资格成为可选择性使用的武器，并呼吁立法统一处理所有滥用者。另一名用户分享亲身经历，称其前雇主通过 OPT、H-1B 与 L1 的渠道聘用外籍毕业生，并随即启动 PERM 劳工证申请。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.etvbharat.com/en/international/vance-says-microsoft-is-being-suspended-from-program-to-apply-for-green-cards-for-h-1b-visa-workers-enn26100807880">Trump Administration Suspends Eight IT Firms Including Tata...</a></li>
<li><a href="https://www.nytimes.com/2026/10/08/us/politics/microsoft-visas-green-cards.html">Trump Administration Suspends Microsoft From Green Card ...</a></li>

</ul>
</details>

**标签**: `#policy`, `#Microsoft`, `#immigration`, `#H-1B`, `#tech industry`

---

<a id="item-tech-news-8"></a>
### [两个竞争补丁争夺 swap 缓存槽解耦方案](https://lwn.net/Articles/1098399/) ⭐️ 6.0/10

LWN 报道称，Linux 内核的 swap 层在过去一年经历了显著改动，但尚未解决 swap 缓存槽与持久 swap 文件空间直接绑定所带来的低效资源利用问题。目前有两个竞争补丁方案试图解耦这种绑定关系，但两者都还没有达到可合并状态，相关讨论也显示社区对最佳路径仍存在明显分歧。

rss · LWN.net · 10月8日 13:43

**「背景」** Linux 内核的交换层过去一年经历了多项改动，但主线尚未解决一个长期问题：交换缓存的槽位（slot）与持久交换文件中的空间直接绑定。这种绑定导致当缓存槽被占用时，即使对应页面已回收，也无法释放交换文件中的相应空间，造成低效的资源使用。

**「影响」** 在方案合并之前，依赖 swap 文件的内核用户无法获得解耦带来的资源利用优化，swap 文件场景下的低效占用问题仍会持续。内核开发者需要关注两个方案的后续进展，因为最终选择将影响 swap 层的兼容性和长期接口设计。

**标签**: `#linux-kernel`, `#memory-management`, `#swap`, `#kernel-development`, `#open-source`

---

<a id="item-tech-news-9"></a>
### [LWN 汇总多发行版安全更新：内核、Firefox、Chromium 等](https://lwn.net/Articles/1099388/) ⭐️ 6.0/10

LWN 于 10 月 8 日汇总了多个 Linux 发行版当天发布的安全更新，包括 AlmaLinux、Debian、Fedora、Mageia、Oracle、Slackware、SUSE 和 Ubuntu 等。受影响软件覆盖内核、Firefox、Chromium、curl、sudo、xz-utils 等，具体涉及 bind、gst-plugins-base1.0、xorg-server、wireshark、poppler 等软件包。该列表是发行版公告的集中汇总，未包含个别软件包的具体版本号与漏洞编号。

rss · LWN.net · 10月8日 13:11

**「背景」** Linux 发行版通常通过各自的安全公告渠道向用户推送软件包补丁，以修复已公开漏洞；LWN 的“Security updates”栏目会定期将各发行版发布的这类更新集中列成清单，便于管理员在同一处核对。

**「影响」** 使用上述发行版的系统管理员应核对本机安装的软件包并尽快应用对应更新，尤其是 Firefox、Chromium、内核等攻击面较大的组件；重启受影响服务或系统前，需查阅各发行版公告确认具体版本和漏洞影响。

**标签**: `#security`, `#linux`, `#patch management`, `#vulnerabilities`, `#distributions`

---

<a id="item-tech-news-10"></a>
### [马斯克宣布 Grok Bot 接入 Claude](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%A9%AC%E6%96%AF%E5%85%8B%E8%AE%A9Grok%20Bot%E6%8E%A5%E5%85%A5Claude%EF%BC%81%E8%B0%81%E5%A5%BD%E7%94%A8%EF%BC%8C%E5%B0%B1%E7%94%A8%E8%B0%81) ⭐️ 6.0/10

10 月 7 日，马斯克在 X 上宣布，Grok Bot 将根据具体任务自动选择最合适的后端模型，并点名 Claude Opus 5.5、Midjourney 和 Suno，理由是“哪个最有可能给你带来最好的结果，就用哪个”。据 9to5Mac 同日报道，Grok Bot 已可以使用 Claude Opus 5.5。马斯克列出的名单还包括“其他领先的 API”，OpenAI 虽未被点名，但并未明确排除，因此 Grok Bot 是否会调用 OpenAI 模型仍是悬念。

rss · 新智元 · 10月8日 11:55

**「背景」** Grok Bot 是马斯克旗下 xAI 推出的 AI 助手，过去主要依赖 xAI 自家的 Grok 系列模型驱动。Anthropic 的 Claude 则是与之竞争的另一前沿模型系列，通常只能通过 Anthropic 官方产品或第三方集成使用。此次马斯克宣布 Grok Bot 将按具体任务动态选用最合适的后端模型，并点名 Claude Opus 5.5，意味着 xAI 开始直接调用竞品模型来支撑自家助手。

**「影响」** 对 Grok Bot 用户而言，部分任务的实际输出可能由 Anthropic 等第三方模型生成，而非 xAI 自家模型；在 OpenAI 是否加入名单得到确认前，用户不应默认 Grok Bot 完全基于单一模型。

**标签**: `#AI industry`, `#Grok`, `#Claude`, `#Anthropic`, `#xAI`

---

<a id="item-tech-news-11"></a>
### [Lunara：主动学习训练的次百亿参数图像生成模型](https://www.reddit.com/r/MachineLearning/comments/1x13zf7/moonworks_lunara_modeling_artistic_intelligence_r/) ⭐️ 6.0/10

Moonworks 发布了 Lunara，一个参数少于 100 亿的扩散混合 Transformer 图像生成模型，并公开了论文与评测集。其 CAT 训练算法通过主动学习式地挑选样本、细化图像并纳入人类艺术作品来迭代更新训练分布。在 1000 个共享提示词生成 8000 张图片的评测中，Lunara 在 GPT-5.6 Sol 评价下美学得分为 8.473，略高于 GPT-Image-1 Mini 的 8.457 和 Qwen-Image 的 8.366；但 GPT-Image-1 Mini 在情绪共鸣与内容完整性上仍领先。作者还报告了 6 名评估者的盲评中 Lunara 三项指标均值最高；这些结果均为自报，需独立验证。

reddit · r/MachineLearning · /u/paper-crow · 10月8日 21:54

**「背景」** 扩散 Transformer 把扩散模型的去噪过程与 Transformer 结构结合，是当前图像生成的重要技术路线。主动学习通常通过挑选最有信息量的样本提高训练效率；Lunara 把这类样本选择和数据改写机制引入扩散图像模型，属于该思路的一次应用尝试。

**「影响」** 对研究者而言，Lunara 显示不足 100 亿参数的扩散混合 Transformer 可能在美学评分上接近主流闭源与开源基线，但 0.016 分的优势处于边际范围，且情绪与内容指标仍落后。由于评估为自报结果，更稳妥的做法是等待权重开放或独立复现后再作为技术选型或研究基线。

**标签**: `#image generation`, `#diffusion models`, `#transformer architecture`, `#active learning`, `#model evaluation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [盘前主要公司动态：Wolfspeed 获国防部贷款，Broadcom 与 OpenAI 融资谈判](https://www.cnbc.com/2026/10/08/stocks-making-the-biggest-moves-premarket-hae-avgo-lulu-wolf.html) ⭐️ 7.0/10

芯片制造商 Wolfspeed 获得国防部有条件 1.5 亿美元贷款，股价盘前上涨超过 15%；Broadcom 据《华尔街日报》报道正为与 OpenAI 开发的 AI 芯片安排超过 500 亿美元的融资，盘前下跌近 2%。

rss · CNBC Finance · 10月8日 12:28

**「背景」** 这笔贷款是国防部 30 年的融资承诺，将支持美国国内芯片生产，国防部还将获得 Wolfspeed 最多 7.5%的认股权证。Broadcom 的融资谈判仍处于早期阶段。其他公司中，台积电第三季度营收达 160.3 亿美元、同比增长 54.6%且超预期，Lululemon 任命新高管以重振北美业务，Levi Strauss 营收略低于预期，Applied Digital 营收同比大增 322%。

**标签**: `#premarket movers`, `#semiconductors`, `#AI infrastructure`, `#corporate financing`, `#earnings`

---

<a id="item-finance-news-2"></a>
### [标普预测中国房价 2028 年三季度触底，大城市或明年反弹](https://www.cnbc.com/2026/10/08/chinas-real-estate-market-may-be-set-for-a-turnaround-sp-says.html) ⭐️ 7.0/10

标普全球评级 10 月 8 日报告预测，中国住宅价格可能在 2028 年第三季度触底，而北京、上海等大城市的房价有望最早在 2027 年回升。报告指出政府限制开发商预售未完工房产、以及对首套房提供按揭补贴等政策，正在推动市场供应减少，这是调升预期的关键原因。

rss · CNBC Finance · 10月8日 09:27

**「背景」** 今年 2 月标普曾认为高库存使中国房地产市场难以复苏。此后，政府于 8 月限制开发商预售未完工项目，9 月启动对总价低于 150 万元、面积小于 120 平方米的首套住房的按揭利率补贴。标普表示，这些政策将引导开发商减少购地和新建项目，加速去库存，而 2026 年是本轮下行中首次出现实际库存下降的年份。

**「影响」** 若房价如期触底，持有房产的中国家庭资产缩水压力将减轻，同时降低银行对开发贷款和按揭贷款的坏账风险。不过摩根士丹利分析师认为，按揭补贴更多是将购房需求提前释放，而非创造大量新增需求，市场长期可持续性仍存不确定性。

**标签**: `#China real estate`, `#S&amp;P Global Ratings`, `#property market forecast`, `#economic recovery`, `#housing policy`

---

<a id="item-finance-news-3"></a>
### [华为重新押注自研芯片手机，汽车业务交付下滑](https://www.cnbc.com/2026/10/08/huawei-china-smartphone-ev-slow.html) ⭐️ 7.0/10

面对中国智能手机和电动汽车市场放缓，华为于 10 月 1 日发布搭载自研 LogicFolding 芯片的 Mate 90 系列，并重新聚焦国产芯片手机；其消费者业务收入 2025 年已回升至约 510 亿美元，占华为总收入的约 39%。同期，华为与车企合作的汽车技术软件体系 HIMA 在 9 月的交付量约为 3.75 万辆，同比下降 29%。

rss · CNBC Finance · 10月8日 08:04

**「背景」** 2019 年美国限制华为使用谷歌安卓系统和台积电芯片后，华为消费者业务收入曾减半至 2021 年约 340 亿美元；该公司表示，计划未来 1 至 3 年把鸿蒙系统推向海外，并希望中国芯片制造能力最终能支持自研芯片手机在海外销售。

**标签**: `#Huawei`, `#smartphones`, `#China EV market`, `#consumer business`, `#semiconductors`

---

<a id="item-finance-news-4"></a>
### [Manus 母公司完成超 5 亿美元融资](https://www.cls.cn/detail/2499126) ⭐️ 7.0/10

Manus 母公司蝴蝶效应近日完成新一轮融资，金额超过 5 亿美元。本轮由博裕投资、IDG 资本领投，腾讯、红杉中国、真格基金等老股东继续参与；报道未披露具体估值和资金用途。

telegram · zaihuapd · 10月8日 06:43

**「背景」** Manus 是一家 AI 代理（能自主执行任务的 AI 程序）初创公司，其母公司蝴蝶效应今年早些时候以接近 5 亿美元估值完成一轮融资，由美国风投 Benchmark 领投。2025 年底，Meta 已达成收购 Manus 的协议。

**「行业影响」** 据彭博社此前报道，本轮融资预计使 Manus 母公司估值翻倍至 40 亿美元，有望成为中国估值最高的 AI agent 初创公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deeplearning.ai/the-batch/meta-strikes-a-deal-to-acquire-manus-a-singapore-based-agentic-ai-startup-with-chinese-origins">Meta Strikes a Deal to Acquire Manus , a Singapore-Based Agentic AI...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2025-12-29/meta-acquires-startup-manus-to-bolster-ai-business?ref=spyglass.org">Meta to Buy Manus , an AI Startup With Chinese Roots - Bloomberg</a></li>
<li><a href="https://www.cnbc.com/2026/10/08/manus-fund-raise-meta-muse-tencent.html">Manus raises $500 million in first funding round since Meta breakup</a></li>

</ul>
</details>

**标签**: `#AI`, `#venture capital`, `#financing`, `#China`, `#startups`

---

<a id="item-finance-news-5"></a>
### [人社部就新就业形态劳动者权益保障办法公开征求意见](https://mp.weixin.qq.com/s/saqkOXlhe0wX7qD83vdkRw) ⭐️ 7.0/10

人社部 10 月 8 日发布《新就业形态劳动者权益保障办法（征求意见稿）》，公开征求意见至 11 月 8 日。草案要求正常劳动报酬不得低于当地最低工资标准，连续工作 4 小时应保障休息，并规定停止派单、封禁账号等重大决定不得由算法自动作出，须经人工审核。

telegram · zaihuapd · 10月8日 09:23

**「背景」** 此前人社部曾于 2024 年发布针对新就业形态劳动者的休息报酬、劳动规则公示等指引文件，并自 2025 年起通过座谈、调研等方式多轮征求意见。此次公开的《办法（征求意见稿）》仍处于征求意见阶段，尚未正式生效。

**「影响」** 若正式施行，该办法可能通过最低工资、休息保障和人工审核等要求，影响外卖平台、网约车平台及直播平台对骑手、司机和主播等劳动者的用工与算法管理方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jiemian.com/article/15168747.html">jiemian.com/article/15168747.html</a></li>
<li><a href="https://www.yicai.com/news/103386701.html">让数千万 人 走出算 法 之困， 新 就 业 形 态 迎首 部 专属规章</a></li>

</ul>
</details>

**标签**: `#China`, `#labor regulation`, `#gig economy`, `#algorithmic governance`, `#workers&\#x27; rights`

---

<a id="item-finance-news-6"></a>
### [OpenAI 被曝年化收入比市场普遍报道少约 200 亿美元](https://www.ft.com/content/b66a9858-f8fb-46cb-b506-44bfe26fca2a?syn-25a6b1a6=1) ⭐️ 7.0/10

英国《金融时报》援引投资者看到的财务文件称，OpenAI 截至 9 月底的年化收入接近 500 亿美元，比此前广泛报道的 700 亿美元少约 200 亿美元。差距部分源于统计口径不同：OpenAI 未计入通过 AWS、谷歌云等云伙伴销售的收入，OpenAI 拒绝置评。

telegram · zaihuapd · 10月8日 17:22

**「背景」** 年化收入是按近期收入趋势推算的全年收入估算值，常用于评估未上市科技公司；这次数据来自投资者获得的文件，并非 OpenAI 官方披露。

**标签**: `#OpenAI`, `#artificial intelligence`, `#revenue`, `#financial disclosure`, `#market sentiment`

---

<a id="item-finance-news-7"></a>
### [美政府以欺诈为由暂停微软绿卡申请资格](https://apnews.com/article/h1b-visa-program-vance-microsoft-e7b3a407f822702b269ee277d21343ea) ⭐️ 7.0/10

特朗普政府以涉嫌欺诈为由，暂停微软参与外籍劳工绿卡申请项目。副总统万斯称，微软去年裁员约 6000 名美国员工，却获得 6300 份 H-1B 签证和近 3000 张绿卡，并指责其以虚假招聘广告用外籍劳工替代美国员工；微软尚未回应。

telegram · zaihuapd · 10月9日 00:00

**「背景」** H-1B 是发给外国专业人才的临时工作签证；企业要帮这类员工申请绿卡，通常需要先通过“劳工证”（PERM）程序证明招不到合格的美国工人。被暂停参与该项目意味着微软在调查期间不能再为外籍员工启动绿卡申请。美方称这是针对多家科技公司的签证操作暂停之一，同时也在调查包括哈佛、耶鲁在内的九所大学涉嫌滥用 J-1（交流访问学者）签证。

**「影响」** 此次暂停直接导致微软数千名持 H-1B 签证的外籍员工无法通过公司申请绿卡，其职业发展和留美身份面临不确定性；同时，其他高度依赖 H-1B 的科技公司（如亚马逊、谷歌）可能因担忧类似指控而收紧外籍员工招聘或调整签证使用策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tampafp.com/white-house-bars-microsoft-from-foreign-worker-green-card-program-over-fraud-allegations/">White House Bars Microsoft From Foreign Worker Green Card ...</a></li>
<li><a href="https://www.nytimes.com/2026/10/08/us/politics/microsoft-visas-green-cards.html">Trump Administration Suspends Microsoft From Green Card Program...</a></li>
<li><a href="https://www.foxbusiness.com/politics/vance-suspends-microsoft-others-from-foreign-workers-applying-green-cards-accuses-company-visa-abuse">Vance accuses Microsoft of abusing visa system... | Fox Business</a></li>
<li><a href="https://grandgoldman.com/blogs/business/microsoft-h-1b-green-card-suspension-impact-on-tech-workers">Microsoft H - 1 B Green Card Suspension : Impact on Tech Workers</a></li>
<li><a href="https://www.theguardian.com/technology/2026/oct/08/jd-vance-microsoft-visa-workers-green-card-suspension">Microsoft suspended from applying for green cards ... | The Guardian</a></li>

</ul>
</details>

**标签**: `#微软`, `#H-1B签证`, `#移民政策`, `#特朗普政府`, `#科技行业`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Anthropic 推出 Cyber Mission，聚焦关键基础设施与开源软件安全](https://x.com/AnthropicAI/status/2108302539498414208) ⭐️ 7.0/10

Anthropic 官方账号于 2026 年 10 月 8 日通过推文宣布启动“Anthropic Cyber Mission”，将其描述为一项保护关键基础设施和开源软件的新努力。公告本身没有提供具体技术方案、合作方或实施细节，仅附有进一步信息的链接。

twitter · AnthropicAI · 10月8日 21:04

**「背景」** Anthropic 于 2026 年 10 月 8 日通过官方 X 账号宣布启动 Anthropic Cyber Mission，称这是一项保障关键基础设施和开源软件安全的新计划。根据 Anthropic 官方页面，Cyber Mission 是一项长期承诺，旨在通过工具、研究和资源支持防御者保护其软件和系统。相关报道提到，该计划以两个项目起步，其中一个与关键基础设施防御有关。此次发布属于官方层面的行业公告，未包含具体技术细节或新的研究内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/anthropic-cyber-mission">Introducing the Anthropic Cyber Mission \ Anthropic</a></li>
<li><a href="https://www.unite.ai/anthropic-launches-cyber-mission-for-critical-infrastructure-open-source/">Anthropic Launches Cyber Mission for Critical Infrastructure , Open ...</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#cybersecurity`, `#critical infrastructure`, `#open-source`

---

<a id="item-twitter-news-2"></a>
### [Anthropic 发布 OSS Scanner：免费为开源项目扫描漏洞并提供修复建议](https://x.com/AnthropicAI/status/2108302543977906649) ⭐️ 7.0/10

Anthropic 于 2026 年 10 月 8 日通过其官方 X 账号宣布推出 OSS Scanner。该工具旨在保护开源软件安全，将利用 Anthropic 的前沿模型，定期扫描选择加入（opt-in）的开源项目，且不收取费用。根据官方消息，扫描报告会提供概念验证（proof-of-concept）、漏洞解释以及建议修复方案。推文中还附带了项目相关链接。

twitter · AnthropicAI · 10月8日 21:04

**「背景」** Anthropic 于 2026 年 10 月 8 日宣布推出 OSS Scanner，这是一款免费的漏洞扫描工具，将使用其前沿模型定期扫描“选择加入”的开源项目，并在报告中提供概念验证（PoC）、漏洞解释和修复建议。这一举措延续了 Anthropic 近期在安全领域的一系列动作：此前该公司刚宣布扩大网络验证计划（Cyber Verification Program），向经过验证的安全专业人员开放更强大的模型访问权限，并新增授权进攻性安全工作的层级，例如渗透测试和红队演练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2107546569654636883">2026-10-07 — Anthropic Expands Cyber Verification Program for Security Professionals</a></li>

</ul>
</details>

**标签**: `#security`, `#open-source`, `#AI`, `#vulnerability scanning`, `#Anthropic`

---

<a id="item-twitter-news-3"></a>
### [天体物理学家借助 Claude Science 创建首张完整紫外天空地图](https://x.com/AnthropicAI/status/2108290395599667700) ⭐️ 7.0/10

Anthropic 发布消息称，一位天体物理学家利用 Claude Science 创建了首张完整的紫外波段天空地图。虽然天文学家此前已经制作了从射电波到伽马射线的完整天空图，但大部分紫外线观测区域仍属空白。

在这篇科学博客中，天体物理学家 Brice Ménard 解释了他如何指导 Claude 发现现有数据集、整合它们，并通过统计推断填补缺失区域。这项工作若由人类完成需要数周时间，但在 Claude 的协助下，Ménard 在几天内完成，且同时可以处理其他项目。

这张地图不仅是一份有用的教学工具，也展示了人工智能如何使过去被搁置、优先级较低的科研工作成为可能——科学家往往无暇完成这类缓慢且非紧迫的任务，而 AI 现在使之变为现实。

twitter · AnthropicAI · 10月8日 20:16

**「背景信息」** 天文学家此前已在从射电到伽马射线的几乎所有波段完成了完整的天空巡天，但紫外波段一直存在大片空白——大面积天空区域从未被观测过。天体物理学家 Brice Ménard 利用 Anthropic 的 Claude Science 工具，从现有数据集入手，通过统计推断填补了缺失区域，首次绘制出完整的紫外天图（结合远紫外 154 nm 和近紫外 232 nm）。据 Anthropic 介绍，这项工作若由人工完成需数周，而借助 Claude 仅用数天即可完成，且 Ménard 在此期间还能并行处理其他项目。该地图约三分之一（包括大量银道面区域）由 Claude 预测生成，成为 AI 加速低优先级、耗时型科研工作的典型范例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/the-missing-map-of-the-sky">Using Claude Science to produce the first complete map of the sky ...</a></li>
<li><a href="https://twiscan.com/en/x/AnthropicAI/2108290395599667700">Anthropic(@AnthropicAI):An astrophysicist worked with Claude ...</a></li>
<li><a href="https://cryptobriefing.com/claude-science-complete-ultraviolet-sky-map/">Anthropic says scientist used Claude Science to build first complete ...</a></li>

</ul>
</details>

**标签**: `#AI in science`, `#Anthropic`, `#Claude Science`, `#astronomy`, `#ultraviolet mapping`

---

<a id="item-twitter-news-4"></a>
### [Anthropic 深化对科学研究的承诺：投入 1.5 亿美元于创世纪使命，并向 15 个以上联邦机构开放 Claude](https://x.com/AnthropicAI/status/2108226292235809081) ⭐️ 7.0/10

Anthropic 宣布将向“创世纪使命”（Genesis Mission）投入 1.5 亿美元，以深化在科学发现和技术研究方面的承诺。同时，该公司将向超过 15 个联邦机构提供其 AI 助手 Claude 及相关技术支持。这一举措标志着 Anthropic 在推动 AI 赋能科学研究及政府应用方面迈出了重要一步。

twitter · AnthropicAI · 10月8日 16:01

**「背景」** Anthropic 于 2026 年 10 月 8 日通过推文宣布，将向“创世纪使命”（Genesis Mission）承诺投入 1.5 亿美元，用于深化科学研究和科技发现。根据 Anthropic 官方新闻稿和相关报道，这笔资金将在三年内到位，主要以 Claude、Claude Code 和 API 积分形式支持科研项目，并包含工程支持和科学家培训。Genesis Mission 是一项联邦倡议，旨在借助 AI 加速科学与技术发现。Anthropic 还表示，将向超过 15 个联邦机构提供 Claude 及技术支持。截至本条目整理时，暂无社区评论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/genesis-mission-commitment">Building on our commitment to American scientific discovery</a></li>
<li><a href="https://cellcog.ai/blog/anthropic-genesis-mission/">Genesis Mission : Anthropic Pledges $ 150 M, Industry $2.4B | CellCog</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI for Science`, `#Government`, `#Claude`, `#Funding`

---

