# Horizon 每日速递 - 2026-10-23

> 从 57 条内容中筛选出 30 条重要资讯。

---

**科技新闻**
1. [Switch 2 越狱：解密文件系统读写与自动化工具](#item-tech-news-1) ⭐️ 8.0/10
2. [eMudhra 宣布退出全球 SSL/TLS 证书业务](#item-tech-news-2) ⭐️ 8.0/10
3. [甲骨文发布 Java SE 高危漏洞警报 CVE-2026-91403](#item-tech-news-3) ⭐️ 8.0/10
4. [333 个 Tor 出口节点因 Ebury 后门下架](#item-tech-news-4) ⭐️ 8.0/10
5. [Quad9 因版权禁令压力退出法国](#item-tech-news-5) ⭐️ 7.0/10
6. [NVIDIA 开源 OpenShell，为自主 AI 代理提供沙箱化运行时](#item-tech-news-6) ⭐️ 7.0/10
7. [PHP 维护者就无意破坏 RCE 漏洞披露 embargo 道歉](#item-tech-news-7) ⭐️ 7.0/10
8. [489 毫秒三角剖分 370 万地图多边形](#item-tech-news-8) ⭐️ 7.0/10
9. [pwn.watch 实时追踪当前正在被利用的漏洞与安全事件](#item-tech-news-9) ⭐️ 7.0/10
10. [Anthropic 将 Agent Skills 捐赠给 Linux 基金会下的 AAIF](#item-tech-news-10) ⭐️ 7.0/10
11. [Linux 内核 7.4 终结 \_\_get\_user\(\) 与 \_\_put\_user\(\)](#item-tech-news-11) ⭐️ 7.0/10
12. [开源 14.8B 模型 Carbon-X 可同时处理 DNA 与文本](#item-tech-news-12) ⭐️ 7.0/10
13. [Claude API 新版移除温度等参数并改默认认证](#item-tech-news-13) ⭐️ 7.0/10
14. [特斯拉宣布年底开卖 Cybercab，无监督 FSD 推迟至明年 Q2](#item-tech-news-14) ⭐️ 7.0/10
15. [部分智能电视关闭 ACR 仍上报观看数据](#item-tech-news-15) ⭐️ 7.0/10
16. [开源 GameScaling：基于 Qwen3.5 的键鼠操作模型](#item-tech-news-16) ⭐️ 7.0/10
17. [禁运 Nvidia B300 服务器现身中国国有网络](#item-tech-news-17) ⭐️ 7.0/10
18. [DeepSeek、MiniMax 完成 AI 出口登记并继续开源](#item-tech-news-18) ⭐️ 7.0/10
19. [GNU Taler 准备在德国投入运营](#item-tech-news-19) ⭐️ 6.0/10
20. [hackios-xnu-kernel：安卓设备引导 iOS 16.5 固件](#item-tech-news-20) ⭐️ 6.0/10
21. [KeePassXC 2.8.0 发布：Qt6 迁移、Wayland Auto-Type 与 ARM64 构建](#item-tech-news-21) ⭐️ 6.0/10
22. [Rust 未来特性：Kangrejos 2026 上的内核开发者视角](#item-tech-news-22) ⭐️ 6.0/10
23. [LWN 周报索引：内核、Rust、安全与 Nix 议题](#item-tech-news-23) ⭐️ 6.0/10
24. [Open-XTTS-Trainer：一键训练 XTTS v2 三大组件](#item-tech-news-24) ⭐️ 6.0/10
25. [SteerTTS 边缘版仅 11.84 MB，词错误率不变、UTMOS 微降](#item-tech-news-25) ⭐️ 6.0/10
26. [前沿模型对 ASMR 音频标注 F1 最高仅 0.325](#item-tech-news-26) ⭐️ 6.0/10

**科技博客**
1. [软件慢是因为设计差，不是语言慢](#item-tech-blog-1) ⭐️ 8.0/10

**财经新闻**
1. [沪深 300 较 6 月高点回落 20%，A 股逼近熊市](#item-finance-news-1) ⭐️ 8.0/10

**推特新闻**
1. [Anthropic 宣布使用 Claude 与 Theorem Labs 对 100 多个开源库进行形式化验证](#item-twitter-news-1) ⭐️ 9.0/10
2. [OpenAI 邀请 METR 与 Redwood Research 试点评估内部监控系统](#item-twitter-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Switch 2 越狱：解密文件系统读写与自动化工具](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 8.0/10

2026 年 10 月 22 日，ledoge 发布了一篇 Switch 2 越狱技术文章，声称实现了对解密文件系统的访问，并借助自动化硬件工具完成越狱流程。文章细节目前没有独立验证，也未提供可复现的漏洞或持久化方法。若该描述属实，Switch 2 游戏转储可能迅速出现，独占游戏也有望在非官方硬件上运行。

hackernews · ledoge · 10月22日 08:01 · [社区讨论](https://news.ycombinator.com/item?id=50192536)

**「背景」** ns2jb 是开发者 pepsipu 发布的 Switch 2 用户态漏洞利用，属于 tethered（重启后需重新触发）的纯软件破解，据称可用于最新 23.0.1 固件。其漏洞链包括 SmileBASIC 4 的整数溢出和 fs 系统模块的缓冲区溢出，可执行原生代码、运行自制程序与游戏修改，但并非永久自定义固件；报道还称该工具借助 OpenAI Codex 自动构建。

**「社区讨论」** 评论者认为，如果解密文件系统真能做到读写，几小时内就可能出现 Switch 2 游戏转储，并可在任意硬件上运行；还有观点称赞现代自动化工具（如 KVM、蓝牙灯开关、USB 手柄注入）让此类研究更容易落地。也有用户抱怨 AI 编程工具在涉及漏洞研究会拒绝配合，质疑 AI 在其中的实际贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gbatemp.net/news/switch-2-jailbreak-ns2jb-released-software-only-exploit-tethered.685698/">Switch 2 jailbreak &quot;ns2jb&quot; released. Software-only exploit, tethered</a></li>
<li><a href="https://www.aipulse.it/en/news/nintendo-switch-2-jailbreak-ns2jb-exploit-504293">Switch 2 Jailbroken: First Software Exploit Runs Homebrew and Mods</a></li>
<li><a href="https://www.notebookcheck.net/The-Nintendo-Switch-2-has-reportedly-been-jailbroken-through-a-software-only-exploit.1431060.0.html">The Nintendo Switch 2 has reportedly been jailbroken ... - Notebookcheck</a></li>

</ul>
</details>

**标签**: `#Switch 2`, `#jailbreak`, `#hardware security`, `#console hacking`, `#security research`

---

<a id="item-tech-news-2"></a>
### [eMudhra 宣布退出全球 SSL/TLS 证书业务](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business) ⭐️ 8.0/10

eMudhra 于 2026 年 10 月 22 日宣布将退出全球 SSL/TLS 证书业务，面向依赖其全球证书签发的用户。公告称这一决定是在其 CA 运营受到安全审查和社区广泛关注之后作出的；目前仍属计划中的退出，而不是已经完成的业务关停。

hackernews · bo0tzz · 10月22日 13:33 · [社区讨论](https://news.ycombinator.com/item?id=50195110)

**「背景」** 在本次退出声明之前，eMudhra 的八张中级 CA 证书已于 10 月 20 日被 Mozilla、Chrome 与 Apple 等浏览器厂商确认为密钥泄露，并被封禁或吊销。10 月 21 日的日报曾报道，社区分析显示这八把私钥都是单字节值，其中一把就是“4”，任何人都能凭公钥证书几乎瞬间恢复这些密钥。正是这一事件构成了 eMudhra 决定退出全球 SSL/TLS 证书业务的直接背景。

**「影响」** 使用 eMudhra 全球 SSL/TLS 证书服务的组织应尽快联系替代 CA 重新签发证书，因为该公司已决定自愿退出该业务。据外部报道，这一决定是在研究人员恢复其八个中间 CA 证书私钥的五天后作出的；依赖这些中间 CA 签发证书的企业应检查证书链，并准备在浏览器信任措施生效前完成迁移。

**「社区讨论」** 评论者普遍认为 eMudhra 的回应不充分：rdtsc 批评其未解释私钥事故成因，luispa 用一段仅含数字 4 的示例 RSA 私钥嘲讽密钥强度；rahimnathwani 则质疑“未从受影响 CA 签发终端实体证书”的说法，因为私钥泄露后任何人都可自行签发证书。另有评论指出 Mozilla Bugzilla 中 Chrome 团队对 eMudhra 的公开质询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://emudhra.we-have-a-problem.com/">2026-10-21 — eMudhra Intermediate CA Compromise: Single-Byte Keys and Revocation Gaps</a></li>
<li><a href="https://thehackernews.com/2026/10/eight-emudhra-ca-keys-compromised.html">Eight eMudhra CA Keys Compromised, Triggering Emergency Fixes...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/mozilla-google-apple-block-compromised-emudhra-ca-certificates/">Mozilla , Google, Apple block compromised eMudhra CA certificates</a></li>
<li><a href="https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business">eMudhra to Exit global SSL / TLS Certificate Business</a></li>
<li><a href="https://thehackernews.com/2026/10/emudhra-to-exit-global-ssltls-business.html">eMudhra to Exit Global SSL / TLS Business After 8 Intermediate CA...</a></li>

</ul>
</details>

**标签**: `#TLS certificates`, `#certificate authorities`, `#web security`, `#PKI`, `#eMudhra`

---

<a id="item-tech-news-3"></a>
### [甲骨文发布 Java SE 高危漏洞警报 CVE-2026-91403](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 8.0/10

甲骨文于 10 月 22 日发布安全警报，披露 Java SE 的 JSSE 组件存在编号 CVE-2026-91403 的严重漏洞，CVSS 评分为 9.1。攻击者无需身份验证即可通过网络远程利用该漏洞，威胁数据机密性与完整性；受影响版本包括 Java SE 8u511、11.0.33、17.0.21、21.0.13、25.0.5、27.0.1 及多个 GraalVM 版本。甲骨文已提供修复补丁，并敦促用户尽快升级至受支持版本。

telegram · zaihuapd · 10月22日 12:30

**「背景」** JSSE（Java Secure Socket Extension）是 Java SE 中实现 TLS/SSL 协议、保护加密网络通信的组件。许多基于 Java 的服务会在默认或常见配置下使用该组件处理安全连接，因此组件内出现可被远程利用的未认证漏洞时，影响范围往往较广。

**「影响」** 受影响的开发者和运维团队应尽快应用甲骨文发布的补丁或将 Java SE/GraalVM 升级至修复版本；在修复完成前，暴露于网络的 Java 服务可能遭遇未认证远程攻击，导致加密通信的机密性和完整性受损。

**标签**: `#java-se`, `#security`, `#CVE-2026-91403`, `#vulnerability`, `#patch-management`

---

<a id="item-tech-news-4"></a>
### [333 个 Tor 出口节点因 Ebury 后门下架](https://kaba.cx/posts/20261020_Tor/) ⭐️ 8.0/10

据一名 Tor 运营者发布的信息，他扫描约 3000 个出口中继后发现其中 333 个被植入 Ebury 后门，约占扫描样本的 10%；该后门可把 22 端口 SSH 连接劫持到 12 台拦截服务器并窃取凭据。这些节点于 10 月 4 日被标记为 BadExit，次日全部下线。攻击者自今年 8 月就已入侵这些服务器，并屏蔽部分端口以专门收集未加密邮件流量，具体入侵途径尚无定论。

telegram · zaihuapd · 10月22日 14:52

**「背景」** Tor 出口中继是 Tor 网络中把匿名流量转发到普通互联网的最后一跳服务器；一旦被入侵，运营者可将其标记为 BadExit，使客户端避开这些节点。本次事件正是通过扫描出口中继并标记 BadExit 来阻止受影响节点继续提供服务。

**「影响」** 由于 Ebury 会劫持 22 端口 SSH 连接并窃取凭据，曾在这批出口节点在线期间通过 Tor 登录远程服务器的用户应把相关凭据视为已泄露并及时轮换；这 333 个节点被标记并下线后，也不再承担 Tor 出口流量。

**标签**: `#Tor`, `#security`, `#Ebury`, `#SSH`, `#backdoor`

---

<a id="item-tech-news-5"></a>
### [Quad9 因版权禁令压力退出法国](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 7.0/10

Quad9 宣布将退出法国市场，原因是法国版权禁令带来的法律压力。该公司计划在 11 月 24 日后通过 geoIP 过滤阻止法国用户访问其服务，但其 CTO 承认这类阻断并不充分，因为用户可用 VPN 绕过；此前原告索尼音乐娱乐（Sony Music Entertainment GmbH）就曾用 VPN 从德国访问被屏蔽内容，导致 Quad9 因藐视法庭被罚款。

hackernews · farrokhi · 10月22日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=50195959)

**「背景」** 10 月 6 日的 Horizon 日报曾报道，瑞士非营利 DNS 解析器 Quad9 拒绝执行法国法院应 beIN Sports 请求发布的封锁 58 个盗版体育直播域名的命令，面临最高每日 58 万欧元的罚款，并表示若法院要求仅对法国用户封锁，它只能在全球封锁与退出法国之间二选一。现在 Quad9 正式宣布退出法国，同时解释称由于用户可用 VPN 绕过 geoIP 封锁，这种选择性拦截不足以满足法院要求，且公司已因藐视法庭被罚款。

**「影响」** 对法国用户而言，Quad9 退出后其隐私优先的 DNS 解析服务在 11 月 24 日后可能无法正常使用，依赖该服务的个人或组织需要改用其他解析器。这一决定也延续了此前 Cisco 因同类法院禁令放弃法国市场的先例，说明针对 DNS 解析服务的版权执法压力仍在扩大。

**「社区讨论」** Quad9 CTO johnhtodd 解释称，公司预计会使用 geoIP 过滤来屏蔽法国用户，但认为围绕“如何屏蔽”的争论偏离了更根本的问题。其他评论者将起诉 DNS 解析器比作惩罚收录罪犯电话的电话簿公司，还有人提议，被强制屏蔽的解析器也应停止解析起诉方公司的域名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/">2026-10-06 — Quad9 refuses French DNS piracy blocks, faces €580K daily fines</a></li>
<li><a href="https://reclaimthenet.org/quad9-considers-leaving-france-over-website-blocking-order">Quad 9 Considers Leaving France Over Website Blocking Order</a></li>

</ul>
</details>

**标签**: `#dns`, `#internet-governance`, `#copyright`, `#privacy`, `#tech-policy`

---

<a id="item-tech-news-6"></a>
### [NVIDIA 开源 OpenShell，为自主 AI 代理提供沙箱化运行时](https://github.com/NVIDIA/OpenShell) ⭐️ 7.0/10

NVIDIA 以开源方式发布了 OpenShell，一个面向自主 AI 代理集群的运行时，让代理在沙箱化和私有环境中获得文件、凭据与网络资源的受控访问，以便安装软件包、调用 API 和执行任务。项目托管在 GitHub，定位是替代“完全不受限”的代理运行方式，而不是取消代理能力本身。目前公开信息有限，许可证、版本和与现有容器编排工具的集成程度尚未明确。

hackernews · niemandhier · 10月22日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=50198675)

**「背景」** Horizon 2026 年 9 月 29 日的日报曾报道，NVIDIA 在 Open Agent Safety Platform 参考架构中描述了 OpenShell 组件，它运行在 CPU 层以限制自主 AI 代理的操作，并与负责网络层监控的 Sentry 配合。现在 OpenShell 以独立开源运行时发布，用户可以直接获得代码并自行部署，而不只是停留在平台蓝图层面。

**「影响」** 对正在生产环境运行自主代理的团队，这类运行时提供了一层容器管理上的安全封装，但并不会自动解决数据外泄问题：即使把网络限制到可信域名，代理读写过的代码库仍可能被带走。采用者应把网络出口审计和敏感数据标记纳入部署方案，而不是只依赖沙箱本身。

**「社区讨论」** 部分评论者认为 OpenShell 是容器管理的合理补充：mfro 称如果还没把代理放进容器就是“疯了”，这个项目是管理这些容器的好方式；smallnix 则指出宣传文案有过度承诺之嫌，因为给代理的权限越多其能力越强，所谓“又安全又全能”并不可能。fennecbutt 分享自己使用 iron proxy 限制域名和交换凭据的经验，认为代码库防外泄仍是信任代理时最难解决的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/nvidia-open-agent-safety-platform-a-reference-for-continuous-in-silicon-agent-monitoring/">2026-09-29 — Nvidia Open Agent Safety Platform Aims to Prevent AI Agent Escapes</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#sandboxing`, `#security`, `#open source`, `#AI infrastructure`

---

<a id="item-tech-news-7"></a>
### [PHP 维护者就无意破坏 RCE 漏洞披露 embargo 道歉](https://news.ycombinator.com/item?id=50193416) ⭐️ 7.0/10

一位 PHP 维护者在 Hacker News 上公开道歉，承认自己无意中破坏了围绕 CVE-2026-109618 与 CVE-2026-109619 这两个即将公开的 PHP 远程代码执行漏洞的协调披露 embargo，并称这给披露日程带来了连锁影响和额外工作量。他表示发帖时并不知道存在任何 embargo，信息来源链条中的联系人也都声称没有 embargo；其本意是提醒从源码编译 PHP 的用户重视更新。文中没有给出漏洞技术细节或修复版本，因此这则帖子的直接信息是披露协调失败及其道歉。

hackernews · petecooper · 10月22日 10:11

**「背景」** 在作者发帖前一天，PHP 安全团队已预先公告将于 10 月 21 日 14:00 UTC 发布一次高优先级安全更新，并敦促用户提前准备升级，但当时没有公开任何 CVE 细节或受影响版本。这轮预先公告正是针对本次涉及的两个 RCE 漏洞（CVE-2026-109618、CVE-2026-109619）的协调披露流程的一部分，因此作者提前泄露相关信息才会影响原定的披露时间表。

**「影响」** 这两个 PHP 远程代码执行漏洞（CVE-2026-109618 与 CVE-2026-109619，合称 PHP2Shell）已于 2026 年 10 月 21 日公开披露，CVSS v4.0 评分为 9.2，PHP 安全团队已发布紧急补丁，并强烈建议所有 PHP 用户立即更新。安全厂商 watchTowr 称已复现 CVE-2026-109618，Cloudflare CTO 也表示已观察到早期攻击迹象，因此受影响用户应尽快应用修复版本，并优先排查暴露在公网的 PHP 服务。

**「社区讨论」** 多位评论者认为作者并没有违反 embargo，因为他既不是 embargo 当事方，也未被告知 embargo 存在，真正的责任应在信息链上游；rancar2 还表示这些漏洞在作者先前发帖之前就已被泄露并遭利用，并附上 AWS 安全博客链接。这些观点属于评论者判断，尚不能作为对事件完整经过的独立确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1101687/">2026-10-21 — PHP security team pre-announces critical update for October 21</a></li>
<li><a href="https://watchtowr.com/intelligence/php-cve-2026-109618-faq/">PHP2Shell FAQ: CVE-2026-109618 &amp; CVE-2026-109619 Fixes</a></li>
<li><a href="https://www.zscaler.com/blogs/security-research/cve-2026-109618-and-cve-2026-109619-php-vulnerable-unauthenticated-rce">CVE-2026-109618 and CVE-2026-109619: PHP2Shell | ThreatLabz</a></li>
<li><a href="https://www.tenable.com/blog/php2shell-cve-2026-109618-cve-2026-109619-frequently-asked-questions-about-critical-php-remote">php2shell (CVE-2026-109618, CVE-2026-109619): Critical PHP ...</a></li>

</ul>
</details>

**标签**: `#PHP`, `#RCE`, `#security`, `#CVE`, `#disclosure`

---

<a id="item-tech-news-8"></a>
### [489 毫秒三角剖分 370 万地图多边形](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 7.0/10

该博客文章介绍了一个名为 Earstrip 的新三角剖分库，声称能在 489 毫秒内处理 370 万个地图多边形，并显示其性能优于 Earcut。这一结果目前仍是作者发布的基准声明，尚未看到独立的第三方复现；文章引发了 Earcut 作者等三角剖分开发者关注，但属于对现有算法的增量式性能优化，而非理论突破。

hackernews · molind · 10月22日 09:31 · [社区讨论](https://news.ycombinator.com/item?id=50193170)

**「背景」** 多边形三角剖分是将一个多边形区域划分为一组内部互不相交的三角形，这是地图渲染、计算几何等场景中的基础操作。Earcut 是 JavaScript 生态中广泛使用的基于耳切法的三角剖分库，常被作为性能对比基准；这篇博客介绍的新库 earstrip 同样采用耳切法，因此其性能数字可以直接与 Earcut 对照。

**「影响」** 对使用 WASM 三角剖分的渲染项目来说，“3.7M 多边形 489 ms”不是唯一决策指标：Earcut 作者提醒，为维持 4.1 kB min/gz 的包体大小，他刻意放弃了一些优化；社区也质疑极小三角形可能带来渲染问题。若以该库为基准，应先验证三角形质量与包体体积，并可将其与 Delaunay32 等支持并行和约束 Delaunay 的实现放在同类语料上对比。

**「社区讨论」** Earcut 作者 mourner 在 HN 上对这项优化表示认可，并说明 Earcut 为保持 4.1k min/gz 的包体积，刻意放弃了一些潜在优化；还有其他评论者讨论耳切法为何能在实践中胜过 Seidel 梯形法，以及细小三角形是否会造成渲染问题。这些都属于参与者的个人观点和技术推测，并非由文中数据独立证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polygon_triangulation">Polygon triangulation - Wikipedia</a></li>
<li><a href="https://globus.software/blog/2026/10/16/cutting-map-polygons/">Faster than earcut: triangulating 3.7M map polygons in 489 ms</a></li>
<li><a href="https://github.com/morishuz/delaunay32">GitHub - morishuz/delaunay32: Fast, parallel 2D Delaunay ...</a></li>

</ul>
</details>

**标签**: `#triangulation`, `#computational-geometry`, `#performance-optimization`, `#map-rendering`, `#webassembly`

---

<a id="item-tech-news-9"></a>
### [pwn.watch 实时追踪当前正在被利用的漏洞与安全事件](https://pwn.watch/) ⭐️ 7.0/10

2026 年 10 月 22 日，Hacker News 帖文介绍了 pwn.watch，一个面向工程师和安全团队的实时面板，用于追踪当前正被利用的漏洞与安全事件。根据现有帖文信息，无法确定数据集的规模、更新频率或来源方法，因此其可信度目前仅取决于站点自身的说明。

hackernews · mrkd · 10月22日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=50195543)

**「背景」** pwn.watch 是一个实时展示“正在被利用的漏洞与安全事件”的网页，所谓“pwn”是安全圈对目标被攻破的俗称。这类实时威胁看板此前已有先例，例如供红队演练追踪 beacon 与凭据的 pwnboard，以及汇总勒索软件、APT 组织、CVE 和攻击活动的 CyberMonitor、CTIWatch；pwn.watch 试图把这一思路进一步聚焦到“当前正在被利用”的条目上。

**「影响」** 运行 RingRTC 低于 2.72.0 的信号应用用户应立即升级：CVE-2026-113380 允许远程对端通过填满呼叫的 FSM 队列，干扰本地挂断操作，使通话（音频及可能视频）无法正常结束。安全团队参考实时漏洞面板时也应结合补丁状态核实“Live/ongoing”标签，因为评论者指出该 Signal 条目在补丁发布一个多月后才被列为“持续中”。

**「社区讨论」** 评论者对其准确性提出质疑：aeturnum 指出，被标为“Live/ongoing”的 Signal 漏洞（CVE-2026-113380）其实在一个多月前已修复，质疑无已知利用的“ongoing”状态何时才算结束；demibabs 与 b1n 则批评页面是 AI 生成式地塞入过多信息、赞助商布局容易被误认为“被黑最多的网站”。此外，xbar 预测这一代 LLM 将引发史上最大规模的安全事件浪潮，pixl97 也认为多年松懈的安全姿态终于开始反噬。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/max-49/pwnboard">GitHub - max-49/pwnboard: Real-time web dashboard for tracking beacons ...</a></li>
<li><a href="https://cybermonitor.cloud/">CyberMonitor — Real-Time Cyber Threat Intelligence Dashboard</a></li>
<li><a href="https://ctiwatch.com/">CTIWatch — Cyber Threat Intelligence Platform</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-113380">CVE-2026-113380 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://cve.halosecurity.com/cve-advisory/cve-2026-113380-ringrtc-fsm-queue-saturation-vulnerability">CVE-2026-113380: RingRTC FSM Queue Saturation Vulnerability</a></li>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-113380">CVE-2026-113380 - RingRTC Finite State Machine Queue ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#cve`, `#incident-response`, `#cybersecurity`

---

<a id="item-tech-news-10"></a>
### [Anthropic 将 Agent Skills 捐赠给 Linux 基金会下的 AAIF](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 7.0/10

Anthropic 今日宣布，将 Agent Skills 标准捐赠给 Linux 基金会旗下的 Agentic AI Foundation（AAIF），以保持该标准的开放、社区驱动和厂商中立。AAIF 是 Anthropic 与 Block、OpenAI 去年共同创立并已接收 Model Context Protocol（MCP）捐赠的组织。此次捐赠使 Agent Skills 与 MCP 同归一个基金会治理，延续了 Anthropic 将关键代理标准交由中立组织管理的路径。

rss · Simon Willison · 10月22日 18:09

**「背景」** Agent Skills 是 Anthropic 提出的开放标准，用于以可复用、可组合的方式向模型提供专门技能。此前 Anthropic 已与 Block、OpenAI 共同创立了 Linux 基金会旗下的 Agentic AI Foundation（AAIF），并将 Model Context Protocol（MCP）捐赠给该基金会；本次将 Agent Skills 捐赠给 AAIF，延续了同样的开放治理路径。

**「影响」** 对构建代理系统的开发者而言，Agent Skills 的后续版本和兼容性要求预计将在 AAIF 的公开治理下演进，而非由 Anthropic 单独决定；由于 MCP 已归属同一基金会，开发者可以在同一框架下跟踪这两项相互关联的代理标准。

**标签**: `#agentic-ai`, `#open-standards`, `#anthropic`, `#linux-foundation`, `#mcp`

---

<a id="item-tech-news-11"></a>
### [Linux 内核 7.4 终结 \_\_get\_user\(\) 与 \_\_put\_user\(\)](https://lwn.net/Articles/1102061/) ⭐️ 7.0/10

Linus Torvalds 合并了一个由他本人编写的 48 部分补丁系列，将 \_\_get\_user\(\) 和 \_\_put\_user\(\) 这两个用于内核访问用户空间内存的旧原语从 Linux 内核中移除。该系列面向 7.4 版本，属于一次长期拖延的清理；这些接口曾是最佳实践，但早已被后续方案取代。

rss · LWN.net · 10月22日 16:25

**「背景」** Linux 内核长期使用 \_\_get\_user\(\) 和 \_\_put\_user\(\) 等原语来访问用户空间内存，但源码中提到，这些接口很久以前就已被更新的机制取代，只是清除这类旧代码需要时间。另外，10 月 19 日的日报曾报道 Linux 7.3 以 18,765 个非合并提交刷新纪录并正式发布，此后 7.4 开发周期随之展开；Torvalds 的这一 48 补丁清理系列正是预定随 7.4 合入的改动。

**「影响」** 依赖这两个旧接口的内核代码在 7.4 中会失效，相关开发者需要改用已有的替代接口以继续在内核中使用用户空间内存访问功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1101143/">2026-10-19 — Linux 7.3 kernel released with record commit count</a></li>

</ul>
</details>

**标签**: `#linux-kernel`, `#kernel-development`, `#memory-access`, `#open-source`, `#systems-programming`

---

<a id="item-tech-news-12"></a>
### [开源 14.8B 模型 Carbon-X 可同时处理 DNA 与文本](https://www.reddit.com/r/MachineLearning/comments/1xchayq/carbonx_is_an_open_148b_model_trained_jointly_on/) ⭐️ 7.0/10

Carbon-X 是一个 14.8B 参数的 decoder-only 模型，用同一 token 流同时处理 6-mer DNA token 和英文文本，用户可以在普通聊天中输入原始 DNA 并获得英文回答。模型在 302B token 上完成了中期训练，Hugging Face 报告其五项 DNA 基准的平均得分为 66.7%（关闭思考模式），而 GPT-6.1 Sol 为 67.5%。权重以 Apache 2.0 许可发布，bfloat16 下可装入单块 80 GB GPU；但该模型尚未经过临床验证，模型卡也明确说明精确的序列操作仍应由代码处理。

reddit · r/MachineLearning · /u/jatingargiitk · 10月22日 12:32

**「背景」** 生物信息学中的 DNA 语言模型通常先把序列编码为 k-mer token，再在基因组数据上预训练，用于序列分类、变异解释等任务。Carbon-X 延续了这一思路，但把 DNA 与文本放进同一个 token 流，并提供对话式输入原始 DNA 的界面，降低了使用门槛。

**「影响」** 对持有敏感基因组数据的团队而言，Carbon-X 可以在单块 80 GB GPU 上本地运行，配合 Apache 2.0 许可，便于在不出域的情况下做初步序列分析。不过模型卡要求精确序列操作仍用代码校验，因此用户不能只依赖该模型进行变异判定等关键步骤。

**标签**: `#genomics`, `#large language models`, `#open weights`, `#bioinformatics`, `#Hugging Face`

---

<a id="item-tech-news-13"></a>
### [Claude API 新版移除温度等参数并改默认认证](https://x.com/ClaudeDevs/status/2113013247209021918) ⭐️ 7.0/10

据社交媒体转帖，Anthropic 发布 Claude API 版本 2026-10-21，这是自 2023 年以来首次正式版本更新；新版本移除 temperature、top\_p、top\_k，继续传入这些参数会返回 400，SDK 与 ant CLI 默认切换至新版，认证头改为 Authorization: Bearer，旧版 2023-06-01 暂未弃用。该消息来自未经证实的转帖，尚未看到官方正式公告或完整技术文档。

telegram · zaihuapd · 10月22日 03:54

**「背景」** 此前 Claude API 一直以 2023-06-01 作为官方版本；官方迁移文档确认，2026-10-21 是 Anthropic 自 2023 年以来首次发布的正式 API 版本。在该新版本中，请求即使使用 temperature、top\_p、top\_k 的默认值，也会返回 400 错误，因此调用方需要从请求中移除这三个参数。

**「影响」** 使用 SDK 或 ant CLI 的开发者升级后应删除对 temperature、top\_p、top\_k 的依赖，并改用 Bearer 认证；若仍需旧行为，可继续固定使用 2023-06-01 版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/api/migration-2026-10-21">Migrating to API version 2026-10-21 - Claude Platform Docs</a></li>
<li><a href="https://aicoder.com/news/news-20261022-anthropic-claude-api-version-2026-10-21-sdk-majors">Claude API ships version 2026-10-21, its first since 2023 ...</a></li>

</ul>
</details>

**标签**: `#Claude API`, `#Anthropic`, `#breaking change`, `#API update`, `#AI`

---

<a id="item-tech-news-14"></a>
### [特斯拉宣布年底开卖 Cybercab，无监督 FSD 推迟至明年 Q2](https://techcrunch.com/2026/10/21/tesla-says-it-will-start-selling-cybercabs-by-end-of-year/) ⭐️ 7.0/10

特斯拉在周三第三季度财报电话会上表示，年底前将开始向客户出售 Cybercab。工程副总裁 Lars Moravy 称，当前产量全部供给自家 robotaxi 车队，之后才会小规模向客户交付全自动驾驶车辆。这款无方向盘的双座车正被 NHTSA 调查是否符合联邦安全标准；马斯克表示 Cybercab 主要作为出行服务而非个人购买，无监督版 FSD 已推迟到明年第二季度推送。

telegram · zaihuapd · 10月22日 07:54

**「背景」** Cybercab 是特斯拉设计的无方向盘双座自动驾驶车辆，商业定位以无人驾驶出行服务为主，而非个人购买。特斯拉在此次财报电话会上重申，当前量产车将优先供给自家 robotaxi 车队，向客户的交付只是后续的小规模开放；同时，无监督版 FSD 的推送时间已推迟到明年第二季度。

**「影响」** NHTSA 已就特斯拉如何为没有方向盘、踏板和后视镜的 Cybercab 取得联邦安全合规认证展开调查，这一监管不确定性可能影响公司年底前向客户交付车辆的承诺；同时，马斯克明确 Cybercab 主要定位为出行服务而非个人购买，潜在个人买家应对交付范围和监管风险保持谨慎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cleverdude.com/content/nhtsa-opens-investigation-into-tesla-cybercab-safety-certification-after-austin-launch/">NHTSA Opens Investigation Into Tesla Cybercab Safety Certification...</a></li>
<li><a href="https://www.nytimes.com/2026/09/04/business/tesla-cybercab-nhtsa-investigation.html">Tesla ’s Cybercab Is Being Investigated by Federal Regulators</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2kzcXY3dkVSRlBZcnJpUTBKMjFTZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - NHTSA investigates Tesla following Cybercab rollout...</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#autonomous-vehicles`, `#robotaxi`, `#FSD`, `#EV`

---

<a id="item-tech-news-15"></a>
### [部分智能电视关闭 ACR 仍上报观看数据](https://watchingthewatchers.github.io/watchingthewatchers/index.html) ⭐️ 7.0/10

一项覆盖 10 家厂商 12 台智能电视、共 5943 次受控实验的研究显示，部分机型即使在设置中关闭自动内容识别（ACR），仍会继续发送内容相关遥测。其中 VIDAA OS 通过 MQTT 明文发送含不可重置设备 ID 与音频指纹的数据，Vizio WatchFree+ 将节目名写入未加密域名查询且用户无法关闭。该研究以美国市场电视为样本，并未覆盖所有品牌和地区型号。

telegram · zaihuapd · 10月22日 09:50

**「背景」** 自动内容识别（ACR）是智能电视通过采样播放中的音频或视频并与内容数据库比对，来识别用户正在观看什么节目的技术，厂商常将其用于收视统计和广告定向。VIZIO 的隐私政策与支持文档均说明，其联网电视在功能开启时会通过 ACR 收集“Viewing Data”，包括节目、广告和连接设备等信息，并向用户提供关闭开关。

**「影响」** 依赖设置中的 ACR 开关来保护观看隐私的用户需要知道，该开关并不能保证停止所有内容上报；对 VIDAA 和 Vizio 用户，观看数据还存在以明文形式在网络路径中被截获的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vizio.com/en/terms/privacy-policy/viewing-data-privacy-policy">Viewing Data Supplement - VIZIO</a></li>
<li><a href="https://classlawdc.com/2026/09/09/vizio-smart-tv-viewing-data-and-acr-privacy-investigation/">VIZIO Smart TV Viewing Data and ACR Privacy Investigation</a></li>
<li><a href="https://support.vizio.com/s/article/Smart-Interactivity-Broadcast-Interactivity-FAQ-How-to-turn-Smart-Interactivity-Broadcast-Interactivity-on-or-off?language=en_US">How to turn Viewing Data On, Off, or Delete - VIZIO Support</a></li>

</ul>
</details>

**标签**: `#privacy`, `#smart-tv`, `#ACR`, `#security`, `#telemetry`

---

<a id="item-tech-news-16"></a>
### [开源 GameScaling：基于 Qwen3.5 的键鼠操作模型](https://arxiv.org/abs/2610.28698v1) ⭐️ 7.0/10

米哈游崩坏 AI 团队联合清华大学等发布并开源 GameScaling，一个基于 Qwen3.5 视觉语言模型做键鼠操作继续预训练的游戏操作模型，规模覆盖 0.8B 至 27B，每次输出未来 200 毫秒的键鼠动作。项目提供八个检查点和 Apache-2.0 推理客户端，但不含训练代码。论文通过 120 组训练配置考察数据量、多样性与模型规模，发现数据越多同源表现越好，多样化数据有助于迁移到相近游戏，对差异较大的世界提升有限。

telegram · zaihuapd · 10月22日 11:32

**「背景」** GameScaling 基于 Qwen3.5 视觉语言模型进行键鼠操作继续预训练。此前 Horizon 10 月 1 日的日报曾报道，已有多家机构基于 Qwen3.5 开源下游模型，例如 B 站开源的 Index-Translate 翻译模型系列就以 Qwen3.5 为基础，支持 150 种语言。这说明 Qwen3.5 已成为开源社区中可复用的基础模型底座之一。

**「影响」** 开发者和研究者可以直接使用已开源的检查点与推理客户端搭建游戏操作代理，但缺少训练代码意味着无法自行复现或修改训练流程；后续是否补充训练代码将影响该模型在研究与再训练方向上的实际可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/1/008/914.htm">2026-10-01 — Bilibili Open-Sources Index-Translate Translation Models</a></li>

</ul>
</details>

**标签**: `#game AI`, `#vision-language models`, `#open source`, `#AI research`

---

<a id="item-tech-news-17"></a>
### [禁运 Nvidia B300 服务器现身中国国有网络](https://theinference.org/article/china-s-state-money-bought-banned-nvidia-b300-servers-then-redacted-the-receipts) ⭐️ 7.0/10

据 The Inference 与 Quartz 报道，国资控股的半导租赁集团为 AI 公司荣耀视图科技融资购入 32 台搭载 Nvidia B300 芯片的华硕服务器，属于总额超过 30 亿元的 700 余台服务器交易的一部分，计划部署于中国移动宁夏枢纽。B300 属于美国最严出口管制层级、对华基本禁运；备案引发关注后，半导租赁重新提交文件并抹去硬件描述。Nvidia 表示正联合代工伙伴调查，华硕则称遵守出口管制。目前相关细节仍停留在媒体报道层面，尚待进一步证实。

telegram · zaihuapd · 10月22日 15:22

**「背景」** 美国出口管制将顶级 AI 加速芯片列入对华基本禁运的最高限制层级，Nvidia B300 正属于这一层级。理解这起报道需要这一前提：此类禁令的执行依赖出口商与代工伙伴的合规核查，而融资租赁等间接渠道可能让受管制硬件的实际流向更难追踪。

**「影响」** 若 Nvidia 联合代工伙伴的调查确认该批服务器确实搭载禁运 B300，采购与融资链条上的企业需要重新评估合规备案和供货风险；在此之前，硬件描述被抹除的备案文件可能无法满足监管审查要求。

**标签**: `#Nvidia`, `#B300`, `#export controls`, `#AI hardware`, `#China`

---

<a id="item-tech-news-18"></a>
### [DeepSeek、MiniMax 完成 AI 出口登记并继续开源](https://mp.weixin.qq.com/s/hoeaIXEFagSHugSgMjFe9g) ⭐️ 7.0/10

玉渊谭天报道称，商务部、科技部于 10 月 16 日就修订《中国禁止出口限制出口技术目录》公开征求意见，目录涉及 23 项人工智能领域技术，包括大模型、智能体、算力集群和信息处理等。在这一新框架下，DeepSeek、MiniMax 两家头部企业已顺利履行登记手续，并完成开源和海外授权使用。报道援引商务部相关答问强调，目录的核心是划定边界，而非单纯限制 AI 技术对外出口。

telegram · zaihuapd · 10月22日 16:10

**「背景」** 10 月 17 日的日报曾报道，中国商务部就拟对人工智能、生物医药、光伏等领域 40 项技术实施临时登记和出口管制公开征求意见，其中涵盖 23 项 AI 相关技术。该提议正是当前《中国禁止出口限制出口技术目录》修订公开征求意见的后续进展。

**「影响」** 对依赖 DeepSeek、MiniMax 开源模型或海外授权的开发者与客户而言，新目录并未叫停相关技术流动；两家企业完成登记后即可继续开源和海外授权，说明在中国运营的 AI 企业在对外提供相关技术前需要关注目录范围内的登记与申报要求。这也为其他计划在修订目录落地后继续出海的中国 AI 企业提供了一条可参考的合规路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aqygzj.mofcom.gov.cn/flzc/gzjgfxwj/art/2026/art_c99f95ca0cd043829ac9991495fc283c.html">2026-10-17 — China proposes export registration for 40 AI, biotech, and solar technologies</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#export controls`, `#open source`, `#China AI`, `#DeepSeek`

---

<a id="item-tech-news-19"></a>
### [GNU Taler 准备在德国投入运营](https://www.taler.net/en/news/2026-13.html) ⭐️ 6.0/10

GNU Taler 发布公告称，这一开源、注重隐私的支付系统正在准备在德国投入运营，标志着项目从技术讨论迈向实际运营准备阶段。目前公告未给出具体的上线日期或合作机构名单，实际可用性仍需后续确认。

hackernews · dewey · 10月22日 16:14 · [社区讨论](https://news.ycombinator.com/item?id=50197404)

**「背景」** 按照 NGI TALER 项目的最初计划，位于波鸿的 GLS Bank 将担任 Taler 的电子货币发行方，并推动其在德国上线；但 GLS Bank 已于 2026 年 1 月决定不引入 Taler，随后与联盟伙伴共同商定了后续步骤。最新进展是 GNU Taler 为此成立了一家新公司，接替原先由 GLS Bank 发行电子货币的安排，并向愿意投资至少 5 万欧元的投资者募资，而 Taler 本身仍保持自由软件。

**「影响」** 对于希望减少对美国支付依赖的欧洲用户和商户，GNU Taler 若要真正在德国落地，将面对已获欧洲主要银行支持的 Wero 的竞争：Wero 自 2024 年 9 月推出以来累计交易近 5000 万笔、金额超过 30 亿欧元，并宣称很快将覆盖比利时、法国和德国超过 75% 的个人银行客户（tool-3-2、tool-3-3）。这意味着 Taler 的早期推广可能主要吸引重视隐私的小众用户，而不是取代现有银行支付渠道；考虑采用 Taler 的开发者或商户应评估其离线期限和监管合规限制带来的使用门槛。

**「社区讨论」** 评论区的争论集中在可行性与竞争上：有用户质疑 Taler 电子货币需联网使用且久离线会过期，认为比比特币更差；也有用户认为欧盟监管会以 KYC 限制隐私。另有评论者认可 GLS 银行的参与并希望减少对美国的依赖，但怀疑其能与主流银行支持的 Wero 竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.taler.net/en/news/2026-13.html">GNU Taler</a></li>
<li><a href="https://www.gls.de/taler/">Taler - in Zukunft digital &amp; sicher bezahlen - GLS Bank</a></li>
<li><a href="https://zeli.app/story/50197404">GNU Taler forms a new company to bring · Hacker News | Zeli</a></li>
<li><a href="https://wero-wallet.eu/about">Wero - All about Wero : Europe&#x27;s mobile payment solution</a></li>
<li><a href="https://epicompany.eu/media-insights/wero-successfully-positioned-itself-on-payments/">EPI Company | After 12 months of existence, Wero has ...</a></li>

</ul>
</details>

**标签**: `#GNU Taler`, `#open-source`, `#digital payments`, `#privacy`, `#Germany`

---

<a id="item-tech-news-20"></a>
### [hackios-xnu-kernel：安卓设备引导 iOS 16.5 固件](https://github.com/oosexgang/hackios-xnu-kernel) ⭐️ 6.0/10

开源项目 hackios-xnu-kernel 宣称可在 QEMU、POCO X5 Pro 5G 及部分小米设备上引导 iOS 16.5 固件，并提供了演示网页和源码。需要指出的是，评论者认为这并非可日常使用的完整 iOS ROM，而是一个限时研究测试台：会话运行若干秒后，内核会返回加载器并输出日志。

hackernews · aghuang · 10月22日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50196718)

**「背景」** Horizon 在 10 月 20 日的日报中曾报道，一名开发者通过移植苹果开源 XNU 内核，让取自 iPhone X 的 iOS 16.7.16 用户空间在搭载骁龙 732G 的红米 Note 10 Pro 上启动，并能进入主屏幕，但当时没有 GPU 驱动，图像由 CPU 渲染。本次项目是同类开源尝试的后续：它声称可在 QEMU 以及 POCO X5 Pro 5G 等部分小米设备上引导 iOS 16.5 固件，而非提供完整可日常使用的镜像。

**「影响」** 对移动安全、逆向工程和内核研究人员而言，这提供了在非苹果硬件上观察 iOS 固件引导流程的实验途径，但不应把它当作可替代日常系统的 iOS 移植版；目前只覆盖 QEMU 和特定小米系设备。

**「社区讨论」** 评论者 SoKamil 将项目定性为“研究测试台”而非 ROM，强调会话时间有限、内核随后返回加载器并移交日志；sanid 则提醒，市面上已有模仿 iOS 界面的安卓仿制机，购买二手旧 iPhone 时需加倍确认真伪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/hackintosh/comments/1x95qq0/ios_16716_booting_on_a_snapdragon_732g_redmi_note/?sort=new">2026-10-20 — XNU Port Brings iOS 16.7.16 Booting to Redmi Note 10 Pro</a></li>

</ul>
</details>

**标签**: `#iOS`, `#Android`, `#XNU kernel`, `#open source`, `#mobile OS research`

---

<a id="item-tech-news-21"></a>
### [KeePassXC 2.8.0 发布：Qt6 迁移、Wayland Auto-Type 与 ARM64 构建](https://lwn.net/Articles/1102270/) ⭐️ 6.0/10

KeePassXC 2.8.0 已正式发布，这是该密码管理器的一次主要版本更新。新版本从 Qt5 迁移到 Qt6，在 Linux 上加入 Wayland Auto-Type 支持、可配置键盘快捷键、可通过外部工具同步远程数据库，并为 macOS 和 Linux 分别增加密码快速解锁与 Polkit 快速解锁。此外，2.8.0 包含多项安全更新和 bug 修复，并首次提供 Windows 原生 ARM64 构建和实验性的 Linux AArch64（ARM64）AppImage。

rss · LWN.net · 10月22日 13:34

**「背景」** KeePassXC 是一款开源的跨平台密码管理器。在此之前，该软件仍基于 Qt5，并且在 Wayland 会话下 Auto-Type 功能的使用受到限制；这次 2.8.0 版本主要完成 Qt 框架升级并补齐这些长期等待的能力，同时也开始提供 Windows ARM64 和 Linux AArch64 的构建。

**「影响」** Wayland 会话下的 Linux 用户现在可以直接使用 Auto-Type，无需依赖 XWayland 或额外适配；使用 Windows ARM 设备的用户可安装官方原生构建，而 Linux AArch64 AppImage 仍标记为实验性，生产环境使用需谨慎。

**标签**: `#KeePassXC`, `#password-manager`, `#open-source`, `#security`, `#Linux`

---

<a id="item-tech-news-22"></a>
### [Rust 未来特性：Kangrejos 2026 上的内核开发者视角](https://lwn.net/Articles/1099606/) ⭐️ 6.0/10

据 LWN 报道，Josh Triplett 在 Kangrejos 2026 上介绍了 Rust 项目当前正在开发的、尚未稳定的多项未来特性，面向希望将它们用于内核开发的 Rust 内核开发者。演讲涉及的方向包括类型系统改进、小型语法改进，以及更智能的借用检查器。需要明确的是，这些仍是规划中的能力，并非已经发布的功能。

rss · LWN.net · 10月22日 13:19

**「背景」** Kangrejos 是内核开发者与 Rust 项目成员定期交流的会议，会上常出现面向内核场景的 Rust 语言提案。此前 Horizon 的日报曾报道过若干相关提议，例如 2026 年 10 月 17 日的日报介绍了在无需 unsafe 代码的情况下实现自引用数据结构的方案，10 月 20 日的日报则报道了跨 crate 前向声明的语言特性提案。这些讨论反映了内核开发者对 Rust 语言能力持续演进的需求，也构成了 Josh Triplett 在本次演讲中概述“其他”未来特性的背景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1099224/">2026-10-17 — Safe self-referential structures proposed for kernel Rust</a></li>
<li><a href="https://lwn.net/Articles/1099596/">2026-10-20 — Cross-crate forward declarations proposed for Rust</a></li>

</ul>
</details>

**标签**: `#Rust`, `#kernel development`, `#programming languages`, `#borrow checker`, `#type system`

---

<a id="item-tech-news-23"></a>
### [LWN 周报索引：内核、Rust、安全与 Nix 议题](https://lwn.net/Articles/1100612/) ⭐️ 6.0/10

2026 年 10 月 22 日的 LWN.net 每周版以索引形式发布，列出了多篇待读文章的主题，包括 Android vendor hooks、可重现构建与内核完整性、Rust 数据结构、NFS 服务器改动、为 PID 1 设置 no\_new\_privs、Rust XArray、Rust 跨 crate 声明、7.3 统计和 Nix flakes；简报部分还提到 eMudhra CA 失陷、PHP RCE、Node.js 与 musl 漏洞、GNOME OS、OpenBSD 8.0、Ubuntu 26.10 及 TAB 结果。该页面只是目录而非完整文章，因此不包含具体技术细节或分析。

rss · LWN.net · 10月22日 00:29

**「背景」** LWN 每周版是一份按主题汇总本周文章目录的栏目，这一期列出了 Android 厂商 hook、可重现构建与内核完整性、Rust 数据结构、NFS 服务器变更等文章。此前 10 月 16 日的日报曾报道 2026 年 Linux Plumbers Conference 上关于 Android 内核 vendor hooks 的讨论，本期周刊收录的相关文章正是对这一机制的后续深入报道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1098493/">2026-10-16 — LPC 2026 session examines Android vendor hooks</a></li>

</ul>
</details>

**标签**: `#Linux kernel`, `#Rust`, `#security`, `#reproducible builds`, `#Nix`

---

<a id="item-tech-news-24"></a>
### [Open-XTTS-Trainer：一键训练 XTTS v2 三大组件](https://www.reddit.com/r/MachineLearning/comments/1xcurgj/i_built_openxttstrainer_now_you_can_add_new/) ⭐️ 6.0/10

作者发布了开源项目 Open-XTTS-Trainer（MPL-2.0），旨在补齐 Coqui AI 停运后 XTTS v2 的 DVAE 音频分词器、GPT 文本与词表扩展器、Latent HiFi-GAN 声码器这三个组件的训练/微调流程，并支持为印地语、阿拉伯语等新增 Unicode 脚本动态扩展词表。项目提供 GitHub、Hugging Face 页面及一键 Colab 演示，并宣称可在 Python 3.10–3.13 的现代 PyTorch 环境中运行而无需 torchcodec。据作者自报，在 NVIDIA T4 上使用 LJSpeech 和 JFK 演讲数据测试，HiFi-GAN 的 mel 重建损失在 10 个 epoch 内下降 67%，DVAE 的 mel 误差从 8.14 降至 2.71；这些结果仅验证组件级训练收敛和梯度稳定性，尚未展示完整端到端 TTS 推理效果。

reddit · r/MachineLearning · /u/yashubhakt · 10月22日 21:03

**「背景」** XTTS v2 是 Coqui AI 发布的一个本地零样本文本转语音模型，但 Coqui AI 关停后，官方并未提供其全部训练代码，尤其是 DVAE 音频分词器和 Latent HiFi-GAN 声码器的训练流程，社区通常只能对 GPT 部分进行微调。同时，模型的分词器硬编码了 17 种语言，输入印地语、阿拉伯语、泰语等新文字时会出现词表外标记或矩阵维度错误。

**「影响」** 对需要把 XTTS v2 扩展到原始 17 种语言之外脚本（阿拉伯文、印地文、泰文、迪维希文等）的开发者和研究者，这套 MPL-2.0 套件补上了 Coqui 关停后缺失的 DVAE 与 Latent HiFi-GAN 训练管线，并绕开了 PyTorch 2.4+ 上的 torchcodec 依赖问题；此前社区只有 GPT 微调可用，2023 年 11 月的 GitHub 议题仍在询问如何重训 vocoder 与 DVAE。但收敛基准与“1 键 Colab”均为作者自报，尚无独立复现，建议先在小数据集上验证训练循环再用于实际项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/amitbhakt/open-xtts-trainer">amitbhakt/open-xtts-trainer · Hugging Face</a></li>
<li><a href="https://github.com/coqui-ai/TTS/issues/3323">Retraining vocoder (hifigan) and dvae in XTTS #3323 - GitHub</a></li>

</ul>
</details>

**标签**: `#text-to-speech`, `#XTTS-v2`, `#open-source`, `#model training`, `#ML tooling`

---

<a id="item-tech-news-25"></a>
### [SteerTTS 边缘版仅 11.84 MB，词错误率不变、UTMOS 微降](https://www.reddit.com/r/MachineLearning/comments/1xcum4s/we_shrank_our_steerable_small_tts_to_1184_mb_wer/) ⭐️ 6.0/10

作者发布 SteerTTS 的边缘版 SteerTTS Edge：应用需交付的权重、音色、文本前端和 Python 运行时合计 11.84 MB。声学模型（9.25M 参数，注意力加双向 Mamba-3）与 6.2M 参数、从 charactr/vocos-mel-24khz 蒸馏的 Vocos 风格声码器均采用 int4 量化感知训练；文本前端为纯 numpy，运行时不再依赖 NLTK、g2p\_en、torchaudio 或 num2words。按作者本地运行 Open TTS Leaderboard 协议（非官方提交）的数据，词错误率保持 0.96%，UTMOS 从 4.20 降至 4.11，12 项控制仍保留至少 95% 的 fp32 效果。限制是仅支持英语、附带 200 个音色（完整版为 2825 个），设备端不含声音克隆、自由文本提示或 flow refiner。

reddit · r/MachineLearning · /u/Working\_Hat5120 · 10月22日 20:57

**「背景」** SteerTTS v1 是作者此前发布的一款小型英语 TTS 模型，核心特点是“用数字操纵”：用户可通过数值参数控制语速、音高、响度、停顿等语音特征，并结合风格标签与内联标记生成语音。此次发布的 edge 变体正是对这一模型做量化与蒸馏后的压缩版本，目标是端侧部署。

**「影响」** 对想做设备端或边缘部署的开发者，11.84 MB 的完整运行时降低了打包成本，但需先确认英语、200 音色以及无克隆、无自由文本提示的边界可以接受；由于加载时权重被反量化回 fp32，当前收益主要在体积而非推理速度，若想真正获得 CPU 或移动端加速，仍需等待新内核或 ONNX、WASM 等导出支持。

**标签**: `#text-to-speech`, `#model compression`, `#quantization`, `#on-device AI`, `#speech synthesis`

---

<a id="item-tech-news-26"></a>
### [前沿模型对 ASMR 音频标注 F1 最高仅 0.325](https://www.reddit.com/r/MachineLearning/comments/1xcbqdm/frontier_models_are_bad_at_hearing_asmr_8_judges/) ⭐️ 6.0/10

Reddit 用户 u/MissAppleby 为训练 text2asmr 文本生成 ASMR 模型，用 8 个前沿模型自动标注 480 个片段，并与人工标签对比，发现效果远低于预期：最高的 Gemini 3.1 Pro 也只有 F1=0.325，之后是 Gemini 2.5 Pro（0.290）、GPT Audio 1.5（0.288），最低的是以频谱图输入的 Claude Opus 5.5（0.121）和 Grok 4.7（0.110）。模型对低语人声识别尚可（Gemini/MiMo 的 F1 为 0.70–0.79），但纸张、刷动等物理触发声几乎听不到；单片段成本很低（Gemini 3.1 Pro 约 0.0088 美元，MiMo 约 0.0008 美元），因此作者计划把多个模型与 AST、CLAP 等标签融合，并把模型都不确定的片段优先送人工标注。

reddit · r/MachineLearning · /u/MissAppleby · 10月22日 07:10

**「背景」** text2asmr 是作者正在训练的一个文本到 ASMR 模型，目标是生成低语以及轻敲、揉纸、刷动等触发声，训练集约有 12.6 万个录音，每个片段都需要声音标签。本评测中的外部片段来自 FSD50K 和 ESC-50 等已有人工单类标签的声音事件数据；真正的 ASMR 片段则以“至少一半人工标注者勾选”的类别作为真值。

**「影响」** 对想用前沿模型做细粒度音频标注的人来说，可靠的自动标签目前仍主要落在人声上；作者因此把纸、刷动、切割、粘性、喷溅等模型几乎听不到的类别优先送人工处理，并计划在模型训练完成后公开权重和标签。前一轮廉价模型只根据转录文本打标签而非真正听音频，线性探测无法超过多数类基线（tapping 对 page turning 为 51%），说明在训练前应先验证标签可学习性。

**标签**: `#machine learning`, `#audio tagging`, `#ASMR`, `#frontier models`, `#benchmark`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [软件慢是因为设计差，不是语言慢](https://seangoedecke.com/software-is-slow-because-of-bad-design-not-slow-languages/) ⭐️ 8.0/10

rss · Sean Goedecke · 10月23日 00:00

**「背景」** 肖恩·戈德克认为，把软件重写成 C 或 Rust 就能大幅加速的想法普遍不成立。多数真实程序是 I/O 密集型的，比如一个 CRUD 网站可能有约一半请求时间花在数据库查询上，语言本身的执行速度只影响剩余部分。

**「方案」** 依据阿姆达尔定律，只优化语言执行速度对整体性能有硬上限；而且慢语言往往已经把 CPU 密集工作委托给 C 库，例如 Python 借助矩阵运算库获得接近 C 的性能，所以重写语言很难再带来数量级提升。作者经验里，显著加速几乎都来自重新设计以减少工作量：缓存外部调用、把慢操作移出请求生命周期、并行化、合并 SQL 查询、消除 N+1 查询等。他还引用 Bryan Cantrill 的例子：放弃把 C 程序改写成 Rust 后，朴素的 Rust 版本反而比精心优化的 C 快 30%，原因主要是 Rust 默认数据结构对缓存更友好，说明连 CPU 密集场景也由设计而非语言速度主导。真正值得用更快语言重写的，只有少数无法通过重构减少工作的 CPU 热点。

**「启示」** 作者主张应让 AI 剖析程序、定位热点并建议重新设计，而不是从头用 Rust 或 C 重写；软件慢的根源多半是设计不佳，语言选择只在少数热点处有意义。

**标签**: `#performance`, `#I/O-bound`, `#Amdahl&\#x27;s law`, `#software design`, `#optimization`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [沪深 300 较 6 月高点回落 20%，A 股逼近熊市](https://www.bloomberg.com/news/articles/2026-10-22/china-stocks-set-for-bear-market-as-ai-trade-policy-hopes-fade) ⭐️ 8.0/10

据彭博报道，沪深 300 指数周四一度下跌 1.7%，较 6 月高点累计回落 20%，A 股因此逼近熊市；创业板指已连续 16 个交易日下跌。

telegram · zaihuapd · 10月22日 05:05

**「背景」** 下跌主因是实质性财政刺激缺位以及企业业绩不及预期：宁德时代季度利润增速低于预期，周三股价暴跌 12%；光模块企业新易盛、中际旭创跌幅居前，恒生科技指数下跌超 4.5%。

**标签**: `#A股`, `#沪深300`, `#熊市`, `#宁德时代`, `#科技股`

---

## 推特新闻

<a id="item-twitter-news-1"></a>
### [Anthropic 宣布使用 Claude 与 Theorem Labs 对 100 多个开源库进行形式化验证](https://x.com/AnthropicAI/status/2113390212911083894) ⭐️ 9.0/10

Anthropic 在其 Frontier Red Team 博客上宣布，正在使用 Claude 大规模开展软件形式化验证。形式化验证可以证明代码不存在某些类型的错误，但历史上通常只适用于小型代码库，或者需要投入大量专家时间。Anthropic 表示，借助 AI 模型，这一局面正在改变。他们与 Theorem Labs 合作，在数周内使用 Claude 证明了 100 多个真实世界开源库的安全属性。完整研究已在博客中发布。

twitter · AnthropicAI · 10月22日 22:01

**「背景」** 2026 年 10 月 22 日，Anthropic 在官方 X 账号宣布，其 Frontier Red Team 博客发布了新研究：与 Theorem Labs 合作，使用 Claude 对超过 100 个真实世界开源库进行形式化验证，并在几周内证明了这些库的安全属性。Anthropic 称，形式化验证历来只能用于小型代码库，或需要大量专家时间，而 AI 模型正在改变这一局面。

这一宣布延续了 Anthropic 近期在软件安全验证领域的多项动作。据此前归档信息，10 月 6 日 Anthropic 宣布扩展其 Cyber Verification Program，为通过验证的安全专业人员提供 Claude Mythos 5.1、Opus 5.5 和 Sonnet 5.5 的访问权限，并开放经授权的攻击性安全工作（如渗透测试和红队）层级（tool-1-1）；10 月 9 日，Anthropic 又发布 OSS Scanner，计划用前沿模型定期扫描已选择加入的开源项目以发现漏洞（tool-1-2）。

Anthropic 研究页还提到，合作方 Theorem 也计划为其他开源项目提供同类验证流程，并发布一个 Claude skill 帮助开发者开始验证自己的代码（tool-2-1）。更早前，Anthropic 曾分享 Claude 在 Lean 编程语言中形式化证明费马大定理的工作，称 Claude 在 11 天内基本自主完成证明（tool-2-2），显示 Claude 在数学与软件形式化验证方面的持续进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2107546569654636883">2026-10-07 — Anthropic Expands Cyber Verification Program for Security Professionals</a></li>
<li><a href="https://x.com/AnthropicAI/status/2108302543977906649">2026-10-09 — Anthropic launches OSS Scanner for open-source security</a></li>
<li><a href="https://www.anthropic.com/research/formal-verification">Formally verifying real-world software with Claude \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/formalizing-fermats-last-theorem">Formalizing Fermat&#x27;s Last Theorem \ Anthropic</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#AI`, `#Claude`, `#security`, `#research`

---

<a id="item-twitter-news-2"></a>
### [OpenAI 邀请 METR 与 Redwood Research 试点评估内部监控系统](https://x.com/OpenAI/status/2113298833392496746) ⭐️ 7.0/10

OpenAI 于 2026 年 10 月 22 日通过 X 平台宣布，今年夏天邀请 METR 和 Redwood Research 对其内部监控系统进行试点式嵌入式评估，并在三周内提供深度基础设施访问权限。OpenAI 表示，两家机构的发现帮助其在扩展该系统时加强了安全防护，并将影响未来与 METR 及其他第三方评估者的合作。公告未披露具体评估方法、技术细节或具体发现。

twitter · OpenAI · 10月22日 15:57

**「背景」** OpenAI 在 2026 年 10 月 22 日通过 X 发布公告：今年夏天邀请 METR 与 Redwood Research 对其内部监控系统进行试点嵌入式评估，并提供为期三周的基础设施深度访问。公告称，评估团队的发现帮助 OpenAI 在系统扩展过程中强化了安全防护，未来也会影响与 METR 及其他第三方评估机构的研究合作。

这一动向发生在第三方评估更受关注的背景下。工具摘要显示，Anthropic 此前也在 2026 年 10 月中旬宣布，已向 METR 团队提供类员工访问权限，并表示正与多家机构讨论对其安全实践展开评估（tool-1-1）。同期，安全专家在讨论近期 AI 事件时认为，问题更多来自前沿实验室的沙箱隔离与监控配置失误，而非模型本身失控（tool-1-2）。因此，OpenAI 给予外部评估者深度基础设施访问，并据此调整内部监控，可视为前沿实验室加强第三方评估和透明度的一部分。

需要说明的是，工具结果中的日期为摘要归档日期，不一定是事件确切发生日期；OpenAI 未在公告中披露评估具体技术细节或量化结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2110784662071398807">2026-10-16 — Anthropic grants METR employee-like access for third-party safety evaluation</a></li>
<li><a href="https://www.csoonline.com/article/4234854/ai-agents-arent-going-rogue-frontier-labs-are-skipping-security-basics.html">2026-10-15 — AI Hacking Reports Blamed on Sandbox and Monitoring Failures, Experts Say</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#OpenAI`, `#evaluation`, `#third-party audit`

---

