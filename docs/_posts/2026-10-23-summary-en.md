---
layout: default
title: "Horizon Summary: 2026-10-23 (EN)"
date: 2026-10-23
lang: en
---

> From 57 items, 30 important content pieces were selected

---

**Technology News**
1. [Switch 2 jailbreak write-up details decrypted filesystem access](#item-tech-news-1) ⭐️ 8.0/10
2. [eMudhra exits global SSL/TLS certificate business after CA scrutiny](#item-tech-news-2) ⭐️ 8.0/10
3. [Oracle Flags Critical Java SE JSSE Vulnerability CVE-2026-91403](#item-tech-news-3) ⭐️ 8.0/10
4. [333 Ebury-Backdoored Tor Exit Relays Taken Down](#item-tech-news-4) ⭐️ 8.0/10
5. [Quad9 DNS Resolver Exits France Over Piracy Injunctions](#item-tech-news-5) ⭐️ 7.0/10
6. [NVIDIA OpenShell: open-source sandboxed runtime for autonomous AI agents](#item-tech-news-6) ⭐️ 7.0/10
7. [PHP maintainer apologizes for breaking RCE embargo](#item-tech-news-7) ⭐️ 7.0/10
8. [Earstrip: 3.7M map polygons triangulated in 489 ms](#item-tech-news-8) ⭐️ 7.0/10
9. [pwn.watch: live dashboard of active vulnerabilities and incidents](#item-tech-news-9) ⭐️ 7.0/10
10. [Anthropic Donates Agent Skills Standard to Linux Foundation&\#x27;s Agentic AI Foundation](#item-tech-news-10) ⭐️ 7.0/10
11. [Linux kernel 7.4 drops \_\_get\_user\(\) and \_\_put\_user\(\)](#item-tech-news-11) ⭐️ 7.0/10
12. [Carbon-X: open 14.8B DNA-text model with Apache 2.0 weights](#item-tech-news-12) ⭐️ 7.0/10
13. [Claude API 2026-10-21 reportedly drops temperature and changes auth](#item-tech-news-13) ⭐️ 7.0/10
14. [Tesla says Cybercab sales start by end of year; FSD slips to Q2](#item-tech-news-14) ⭐️ 7.0/10
15. [Study: Some Smart TVs Still Send Telemetry After ACR Is Disabled](#item-tech-news-15) ⭐️ 7.0/10
16. [miHoYo and Tsinghua Open Source GameScaling Game-Operation Model](#item-tech-news-16) ⭐️ 7.0/10
17. [Report: Banned Nvidia B300 Servers Reached China Via State-Backed Lease](#item-tech-news-17) ⭐️ 7.0/10
18. [DeepSeek and MiniMax Complete Filing for Open Source and Overseas Licensing](#item-tech-news-18) ⭐️ 7.0/10
19. [GNU Taler prepares to operate in Germany](#item-tech-news-19) ⭐️ 6.0/10
20. [hackios-xnu-kernel boots iOS 16.5 firmware on Android devices and QEMU](#item-tech-news-20) ⭐️ 6.0/10
21. [KeePassXC 2.8.0 adds Qt6, Wayland Auto-Type, ARM64 builds](#item-tech-news-21) ⭐️ 6.0/10
22. [Upcoming Rust features for kernel developers at Kangrejos 2026](#item-tech-news-22) ⭐️ 6.0/10
23. [LWN Weekly Edition for October 22, 2026 Lists Kernel and Security Stories](#item-tech-news-23) ⭐️ 6.0/10
24. [Open-XTTS-Trainer brings XTTS v2 training to new language scripts](#item-tech-news-24) ⭐️ 6.0/10
25. [SteerTTS Edge Shrinks to 11.84 MB with Unchanged WER](#item-tech-news-25) ⭐️ 6.0/10
26. [Frontier models struggle to label ASMR trigger sounds in benchmark](#item-tech-news-26) ⭐️ 6.0/10

**Technology Blog**
1. [Software is slow because of design, not language choice](#item-tech-blog-1) ⭐️ 8.0/10

**Financial News**
1. [China’s CSI 300 Nears Bear Market After 20% Drop From June Peak](#item-finance-news-1) ⭐️ 8.0/10

**Twitter News**
1. [Anthropic announces Claude-based formal verification at scale](#item-twitter-news-1) ⭐️ 9.0/10
2. [OpenAI announces METR and Redwood Research embedded evaluation](#item-twitter-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Switch 2 jailbreak write-up details decrypted filesystem access](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 8.0/10

Security researchers have shared a Switch 2 jailbreak write-up describing decrypted filesystem read/write access, combined with automated hardware tooling. The claims are not independently confirmed, but the write-up appears substantive enough to draw significant community discussion about practical exploit implications.

hackernews · ledoge · Oct 22, 08:01 · [Discussion](https://news.ycombinator.com/item?id=50192536)

**「Background」** The ns2jb jailbreak is described as a tethered, software-only exploit rather than a hardware modchip: the reported chain chains an integer overflow in SmileBASIC 4 with a buffer overflow in the Switch 2&\#x27;s fs sysmodule to reach userland code execution, and it reportedly works on firmware 23.0.1. Because it is tethered, the exploit must be re-applied after each reboot, so it enables homebrew, game mods, and save access without installing permanent custom firmware.

**「Community discussion」** Commenters focused on the automation rig — KVMs, USB controller input, and a SwitchBot to press the power button — and on the possible fallout of decrypted filesystem access, including dumped games becoming playable on other hardware. One user questioned how such research is done with Codex, reporting that it refused similar Android security work on their account.

<details><summary>References</summary>
<ul>
<li><a href="https://gbatemp.net/news/switch-2-jailbreak-ns2jb-released-software-only-exploit-tethered.685698/">Switch 2 jailbreak &quot;ns2jb&quot; released. Software-only exploit, tethered</a></li>
<li><a href="https://www.aipulse.it/en/news/nintendo-switch-2-jailbreak-ns2jb-exploit-504293">Switch 2 Jailbroken: First Software Exploit Runs Homebrew and Mods</a></li>

</ul>
</details>

**Tags**: `#Switch 2`, `#jailbreak`, `#hardware security`, `#console hacking`, `#security research`

---

<a id="item-tech-news-2"></a>
### [eMudhra exits global SSL/TLS certificate business after CA scrutiny](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business) ⭐️ 8.0/10

eMudhra announced it will exit its global SSL/TLS certificate business following security scrutiny and community concern over its certificate authority operations. The decision is stated as an announced exit rather than a completed shutdown, and no remediation plan or explanation of how the underlying problems occurred is included in the supplied information. The scrutiny centered on CA private-key concerns and public questioning from browser vendors.

hackernews · bo0tzz · Oct 22, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50195110)

**「Background」** Days before this announcement, Mozilla, Google, and Apple blocked eight eMudhra intermediate CA certificates after analysis showed their private keys were single-byte values—one literally &\#x27;4&\#x27;—that anyone could recover from the public certificates and abuse to forge trusted certificates. Horizon&\#x27;s October 21 digest reported that eMudhra&\#x27;s preliminary assessment in a Mozilla bug report attributed the weak keys to a flaw in the key-generation script used that day, and that Mozilla&\#x27;s OneCRL removed the compromised certificates from Firefox automatically within hours. That compromise, and the ensuing browser-vendor scrutiny, is the context for eMudhra&\#x27;s exit from the global SSL/TLS certificate business.

**「Impact」** Organizations relying on SSL/TLS certificates issued by eMudhra&\#x27;s global CA must plan to migrate to another certificate authority before the business winds down, since the board has decided to voluntarily withdraw from the global SSL/TLS business. The pressure to move quickly is heightened because, five days before the announcement, a researcher reported recovering the private keys of eight of eMudhra&\#x27;s intermediate CAs, which could make certificates chained to those intermediates untrustworthy in practice.

**「Community Discussion」** In the comments, rdtsc argued the scrutiny matched the apparent weakness of the affected private keys and criticized the lack of an apology or explanation of whether the issue was a human or process mistake. ieie3366 linked to a Mozilla Bugzilla thread where the Chrome team publicly questioned eMudhra, and rahimnathwani pushed back on the statement that no end-entity certificates were issued, noting that anyone can issue certificates from the affected CAs.

<details><summary>References</summary>
<ul>
<li><a href="https://emudhra.we-have-a-problem.com/">2026-10-21 — eMudhra Intermediate CA Compromise: Single-Byte Keys and Revocation Gaps</a></li>
<li><a href="https://thehackernews.com/2026/10/eight-emudhra-ca-keys-compromised.html">Eight eMudhra CA Keys Compromised, Triggering Emergency Fixes...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/mozilla-google-apple-block-compromised-emudhra-ca-certificates/">Mozilla , Google, Apple block compromised eMudhra CA certificates</a></li>
<li><a href="https://thehackernews.com/2026/10/emudhra-to-exit-global-ssltls-business.html">eMudhra to Exit Global SSL / TLS Business After 8 Intermediate CA...</a></li>

</ul>
</details>

**Tags**: `#TLS certificates`, `#certificate authorities`, `#web security`, `#PKI`, `#eMudhra`

---

<a id="item-tech-news-3"></a>
### [Oracle Flags Critical Java SE JSSE Vulnerability CVE-2026-91403](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 8.0/10

Oracle has released a security alert for CVE-2026-91403, a critical Java SE vulnerability in the JSSE component with a CVSS score of 9.1. The flaw is remotely exploitable without authentication and could compromise data confidentiality and integrity. It affects Java SE 8u511, 11.0.33, 17.0.21, 21.0.13, 25.0.5, 27.0.1, and multiple GraalVM versions. Patches are available, and Oracle is urging users to upgrade to supported versions.

telegram · zaihuapd · Oct 22, 12:30

**「Background」** JSSE, the Java Secure Socket Extension, is the Java component that implements TLS/SSL for encrypted network communications. A vulnerability in this component can expose secure connections to interception or tampering, making patching important for any Java-based service that relies on network encryption.

**「Impact」** Developers and operations teams running any of the listed Java SE or GraalVM versions should prioritize applying the available patches or upgrading to supported releases, since the vulnerability can be exploited remotely without authentication. Unpatched environments that expose SSL/TLS endpoints face a heightened risk of data exposure or modification.

**Tags**: `#java-se`, `#security`, `#CVE-2026-91403`, `#vulnerability`, `#patch-management`

---

<a id="item-tech-news-4"></a>
### [333 Ebury-Backdoored Tor Exit Relays Taken Down](https://kaba.cx/posts/20261020_Tor/) ⭐️ 8.0/10

A Tor operator scanned about 3,000 exit relays and found 333 running the Ebury backdoor, roughly 10%, which redirected SSH connections on port 22 to 12 interception servers and stole credentials. The affected relays were marked BadExit on October 4 and taken offline the next day. The attacker had compromised the servers since August and blocked some ports to collect unencrypted mail traffic; the original intrusion method has not been confirmed.

telegram · zaihuapd · Oct 22, 14:52

**「Background」** Tor exit relays are the last hop between a user&\#x27;s traffic and the public internet, giving them visibility into plaintext connections; a relay suspected of tampering can be flagged &quot;BadExit&quot; so clients stop using it. The Ebury backdoor in this case works by hijacking SSH connections on port 22 and routing them through attacker-controlled interception servers to harvest credentials.

**「Impact」** Tor users who authenticated to SSH services through these relays should treat credentials entered during the compromise window as potentially exposed and rotate them. Operators running exit infrastructure should audit their relays for signs of Ebury or similar SSH hijacking.

**Tags**: `#Tor`, `#security`, `#Ebury`, `#SSH`, `#backdoor`

---

<a id="item-tech-news-5"></a>
### [Quad9 DNS Resolver Exits France Over Piracy Injunctions](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 7.0/10

Quad9 is exiting France rather than comply with copyright injunctions that require blocking piracy-related domain names, saying geoIP blocking cannot reliably enforce the orders because users can evade it with VPNs. The nonprofit resolver says it will probably use geoIP filters to block French users from its services after November 24, a step it considers inadequate; the pressure follows a contempt-of-court fine after Sony Music accessed blocked content from Germany via a VPN.

hackernews · farrokhi · Oct 22, 14:32 · [Discussion](https://news.ycombinator.com/item?id=50195959)

**「Background」** Horizon&\#x27;s October 6 digest reported that Quad9 was refusing a French court-ordered block of 58 pirate sports-streaming domains requested by beIN Sports, even while facing fines of up to €580,000 per day. Quad9 said it does not collect user data and therefore could not block domains only for French users, leaving it to choose between a global block and leaving France. The current news is the outcome of that dispute: Quad9 is now exiting France.

**「Impact」** French users of the Quad9 DNS resolver will lose access to the service after November 24, when Quad9&\#x27;s CTO says it will geoIP-block French IPs rather than selectively block the domains named in a French copyright injunction. Users in France who rely on Quad9 for privacy-respecting DNS should switch to an alternative resolver before that cutoff, since the blocking follows a contempt fine after a plaintiff circumvented geoIP filtering with a VPN.

**「Community Discussion」** Quad9 CTO johnhtodd acknowledges the apparent contradiction between saying geoIP blocking is insufficient and planning to use geoIP filters after November 24, arguing that concern is misplaced. Commenter euio757 notes the move follows Cisco&\#x27;s exit from the same French market about two years ago, after Canal+ won blocking injunctions against Google, Cloudflare, and Cisco; another commenter compares punishing a DNS resolver for a listed domain to punishing a phone book company for a criminal&\#x27;s number.

<details><summary>References</summary>
<ul>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/">2026-10-06 — Quad9 refuses French DNS piracy blocks, faces €580K daily fines</a></li>
<li><a href="https://reclaimthenet.org/quad9-considers-leaving-france-over-website-blocking-order">Quad 9 Considers Leaving France Over Website Blocking Order</a></li>

</ul>
</details>

**Tags**: `#dns`, `#internet-governance`, `#copyright`, `#privacy`, `#tech-policy`

---

<a id="item-tech-news-6"></a>
### [NVIDIA OpenShell: open-source sandboxed runtime for autonomous AI agents](https://github.com/NVIDIA/OpenShell) ⭐️ 7.0/10

NVIDIA has released OpenShell, an open-source runtime for running fleets of autonomous AI agents in sandboxed containers while giving them controlled access to files, credentials, and network resources. It is positioned as a privacy-preserving layer for agent deployments, but detailed implementation information and real-world adoption evidence are still limited. The project is available on GitHub.

hackernews · niemandhier · Oct 22, 17:44 · [Discussion](https://news.ycombinator.com/item?id=50198675)

**「Background」** Horizon&\#x27;s September 29 digest reported on Nvidia&\#x27;s Open Agent Safety Platform, describing OpenShell as the CPU-side component that restricts agent operations, alongside the Sentry network monitoring layer. That announcement framed the platform as a reference system with open-sourcing planned and cited recent sandbox escape incidents as motivation.

**「Impact」** For teams building agent fleets, OpenShell offers a concrete open-source option for constraining agent access to data, secrets, and the network. Community reviewers caution that network restrictions alone do not fully prevent data exfiltration, so organizations should treat OpenShell as a risk-reduction layer and combine it with separate data-loss controls.

**「Community discussion」** Commenters generally saw OpenShell as a useful container-management layer, but several challenged its security framing. smallnix argued that the pitch obscures a tradeoff between agent capability and safety, while fennecbutt noted that restricting traffic to trusted domains still leaves data exfiltration, such as agent-accessed codebases, unsolved and referenced the HF incident; mfro said containers should already be mandatory for agents and described OpenShell as a good way to manage them.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/nvidia-open-agent-safety-platform-a-reference-for-continuous-in-silicon-agent-monitoring/">2026-09-29 — Nvidia Open Agent Safety Platform Aims to Prevent AI Agent Escapes</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#sandboxing`, `#security`, `#open source`, `#AI infrastructure`

---

<a id="item-tech-news-7"></a>
### [PHP maintainer apologizes for breaking RCE embargo](https://news.ycombinator.com/item?id=50193416) ⭐️ 7.0/10

A Hacker News user who said he inadvertently disclosed two upcoming PHP remote code execution vulnerabilities, CVE-2026-109618 and CVE-2026-109619, has publicly apologized for disrupting the coordinated disclosure schedule and adding workload for the parties involved. He says he did not know an embargo existed because his contact, and her contact, had told him there was none, and that he posted to alert people who compile PHP from source in the four-week release cycle to update urgently. The post is an apology and explanation, not a technical advisory; it confirms the embargo coordination failure but does not include technical details.

hackernews · petecooper · Oct 22, 10:11

**「Background」** Horizon&\#x27;s October 21 digest reported that the PHP security team had pre-announced a critical security update for release at 14:00 UTC that day, urging users to prepare to upgrade, without disclosing the vulnerability details or affected versions. The current item clarifies that the upcoming update concerned two PHP remote code execution vulnerabilities, CVE-2026-109618 and CVE-2026-109619, and that a maintainer&\#x27;s earlier public posting disrupted their coordinated disclosure schedule.

**「Impact」** PHP users should apply the emergency patches for CVE-2026-109618 and CVE-2026-109619 immediately: the PHP security team rated both as critical at CVSS v4.0 9.2, public disclosure occurred on October 21, 2026, and security researchers already report early attacks emerging, so delaying the update noticeably increases exposure.

**「Community discussion」** Several commenters push back on the apology, arguing that someone who is not a party to an embargo and was not told about it cannot have broken it, and that responsibility lies earlier in the disclosure chain. One commenter additionally claims the vulnerabilities had already been leaked and exploited before the Hacker News post, citing an Amazon Web Services security blog, though this is not verified by the post itself.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1101687/">2026-10-21 — PHP security team pre-announces critical update for October 21</a></li>
<li><a href="https://www.zscaler.com/blogs/security-research/cve-2026-109618-and-cve-2026-109619-php-vulnerable-unauthenticated-rce">CVE-2026-109618 and CVE-2026-109619: PHP2Shell | ThreatLabz</a></li>
<li><a href="https://www.tenable.com/blog/php2shell-cve-2026-109618-cve-2026-109619-frequently-asked-questions-about-critical-php-remote">php2shell (CVE-2026-109618, CVE-2026-109619): Critical PHP ...</a></li>

</ul>
</details>

**Tags**: `#PHP`, `#RCE`, `#security`, `#CVE`, `#disclosure`

---

<a id="item-tech-news-8"></a>
### [Earstrip: 3.7M map polygons triangulated in 489 ms](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 7.0/10

A blog post introduces Earstrip, an ear-clipping polygon triangulation approach that reports triangulating 3.7 million map polygons in 489 ms, claiming to be faster than Earcut. The benchmark is presented as the author&\#x27;s own result rather than an independently measured comparison, and the item does not provide release or compatibility details.

hackernews · molind · Oct 22, 09:31 · [Discussion](https://news.ycombinator.com/item?id=50193170)

**「Background」** Polygon triangulation is a fundamental computational-geometry step that partitions a polygonal area into non-overlapping triangles, a core operation for rendering map polygons. Earcut is the widely used JavaScript ear-clipping triangulator that the new library is benchmarked against, and ear clipping remains a common technique in this space. The challenger, earstrip, is an ISC-licensed C++ and WebAssembly ear-clipping triangulator published by Globus Software from its map engine.

**「Impact」** For developers choosing a triangulation library, the 489 ms benchmark does not automatically justify switching: Earcut&\#x27;s author says he deliberately rejected such optimizations to keep the JS version at 4.1 kB min/gz and fast enough for typical map clients, so WASM users should weigh bundle size and API suitability. Independent comparison is also pending—the Delaunay32 author noted his polygon API currently requires simple rings with non-touching holes and has not benchmarked this corpus.

**「Community Discussion」** The Earcut author praised the work but said he deliberately rejected some optimizations to keep Earcut&\#x27;s JavaScript bundle small, and asked about the size of Earstrip&\#x27;s WebAssembly build. The Delaunay32 author asked for a benchmark against his divide-and-conquer triangulator, while another commenter questioned why ear clipping remains common compared with Seidel&\#x27;s O\(n log\* n\) trapezoidal method.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polygon_triangulation">Polygon triangulation - Wikipedia</a></li>
<li><a href="https://globus.software/blog/2026/10/16/cutting-map-polygons/">Faster than earcut: triangulating 3.7M map polygons in 489 ms</a></li>
<li><a href="https://zeli.app/story/50193170">A new triangulator beats earcut on 3.7 · Hacker News | Zeli</a></li>

</ul>
</details>

**Tags**: `#triangulation`, `#computational-geometry`, `#performance-optimization`, `#map-rendering`, `#webassembly`

---

<a id="item-tech-news-9"></a>
### [pwn.watch: live dashboard of active vulnerabilities and incidents](https://pwn.watch/) ⭐️ 7.0/10

pwn.watch is a live dashboard that tracks vulnerabilities and security incidents currently being exploited, available at pwn.watch. It gives engineers and security teams a real-time view of active threats, though the submission does not describe how the data is collected or verified.

hackernews · mrkd · Oct 22, 14:08 · [Discussion](https://news.ycombinator.com/item?id=50195543)

**「Background」** Real-time vulnerability dashboards have become a common way for security teams to monitor active threats, aggregating public CVE feeds, exploit databases, and incident reports into a single live view. Comparable tools already exist: pwnboard tracks beacons and credentials from offensive security tools during red-team operations, while services such as CyberMonitor and CTIWatch monitor ransomware, APT groups, zero-days, CVEs, and attack campaigns in real time. pwn.watch applies this pattern to currently exploited vulnerabilities and security incidents, presenting them on a continuously updated public page.

**「Impact」** Signal deployments using RingRTC versions before 2.72.0 should upgrade, since a remote peer can saturate a call&\#x27;s FSM queue and prevent a local hang-up from tearing down the call. Watch-dashboard users should also verify patch dates before treating an entry as an active incident: CVE-2026-113380, which is described as live and ongoing on pwn.watch, was patched over a month before the advisory was announced and has no known exploits.

**「Community Discussion」** In the comments, aeturnum questioned the site&\#x27;s categorization, pointing to a Signal vulnerability listed as &quot;Live&quot; and &quot;ongoing&quot; even though it was patched over a month ago and has no known exploits. Other commenters raised presentation concerns, with demibabs saying AI-generated pages cram too much information into a small space and b1n noting the Sponsors layout could be mistaken for a list of hacked sites.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/max-49/pwnboard">GitHub - max-49/pwnboard: Real-time web dashboard for tracking beacons ...</a></li>
<li><a href="https://cybermonitor.cloud/">CyberMonitor — Real-Time Cyber Threat Intelligence Dashboard</a></li>
<li><a href="https://ctiwatch.com/">CTIWatch — Cyber Threat Intelligence Platform</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-113380">CVE-2026-113380 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://cve.halosecurity.com/cve-advisory/cve-2026-113380-ringrtc-fsm-queue-saturation-vulnerability">CVE-2026-113380: RingRTC FSM Queue Saturation Vulnerability</a></li>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-113380">CVE-2026-113380 - RingRTC Finite State Machine Queue ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerabilities`, `#cve`, `#incident-response`, `#cybersecurity`

---

<a id="item-tech-news-10"></a>
### [Anthropic Donates Agent Skills Standard to Linux Foundation&\#x27;s Agentic AI Foundation](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 7.0/10

Today, Anthropic announced that it is donating the Agent Skills standard to the Agentic AI Foundation \(AAIF\) under the Linux Foundation, the body it co-founded with Block and OpenAI and to which it already donated the Model Context Protocol \(MCP\). The stated goal is to keep Agent Skills open, community-driven, and vendor-neutral. This is a governance change rather than a new technical capability: developers and vendors building agentic systems can expect the skills specification to be stewarded by the multi-vendor foundation.

rss · Simon Willison · Oct 22, 18:09

**「Background」** The Agentic AI Foundation \(AAIF\) under the Linux Foundation was established last year by Anthropic, Block, and OpenAI, and already hosts the Model Context Protocol \(MCP\) after Anthropic donated it. Agent Skills, which Anthropic first described as an open standard in December 2025, now follows the same vendor-neutral governance path.

**「Impact」** For developers and platform vendors standardizing on agent tooling, the donation means Agent Skills will be governed alongside MCP by a neutral foundation, reducing the risk that the skills format becomes locked to Anthropic as the ecosystem matures.

**Tags**: `#agentic-ai`, `#open-standards`, `#anthropic`, `#linux-foundation`, `#mcp`

---

<a id="item-tech-news-11"></a>
### [Linux kernel 7.4 drops \_\_get\_user\(\) and \_\_put\_user\(\)](https://lwn.net/Articles/1102061/) ⭐️ 7.0/10

Linus Torvalds merged a 48-part patch series that removes the \_\_get\_user\(\) and \_\_put\_user\(\) macros from the Linux kernel, ahead of the 7.4 release. The two primitives, long used to access user-space memory from kernel code, had already been superseded and are now being cleaned out. The series is notable because Torvalds rarely contributes large amounts of kernel code himself.

rss · LWN.net · Oct 22, 16:25

**「Background」** \_\_get\_user\(\) and \_\_put\_user\(\) are low-level kernel macros for accessing user-space memory from the kernel; the primitives were once best practice but have long been superseded by safer user-access APIs. The removal lands in the 7.4 development cycle, which follows the 7.3 release that Horizon&\#x27;s October 19 digest reported as a record-breaking kernel with 18,765 non-merge commits.

**「Impact」** Any remaining in-tree users of \_\_get\_user\(\) or \_\_put\_user\(\) must be converted to the newer accessor interfaces before the 7.4 release, since these legacy primitives will no longer be available.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1101143/">2026-10-19 — Linux 7.3 kernel released with record commit count</a></li>

</ul>
</details>

**Tags**: `#linux-kernel`, `#kernel-development`, `#memory-access`, `#open-source`, `#systems-programming`

---

<a id="item-tech-news-12"></a>
### [Carbon-X: open 14.8B DNA-text model with Apache 2.0 weights](https://www.reddit.com/r/MachineLearning/comments/1xchayq/carbonx_is_an_open_148b_model_trained_jointly_on/) ⭐️ 7.0/10

Carbon-X is now available as an open 14.8B decoder-only model that processes raw DNA in chat and answers in English, sharing one token stream for text and 6-mer DNA tokens after mid-training on 302B tokens. The Apache 2.0 weights fit on a single 80 GB GPU in bfloat16. Hugging Face reports a 66.7% average across five DNA benchmarks with thinking disabled, compared with 67.5% for GPT-6.1 Sol, but the model is not clinically validated and its model card says exact sequence operations should still be handled by code.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 22, 12:32

**「Background」** Genomic language models usually require domain-specific preprocessing and fine-tuning before they can answer questions about DNA. Carbon-X instead builds one shared token stream for English and DNA using 6-mer tokens, so the same autoregressive model can be prompted with raw sequence in a normal chat interface.

**「Impact」** For genomics and ML practitioners, the local bfloat16 footprint and open weights make it feasible to analyze sensitive sequence data on-premises, but the lack of clinical validation and the model card&\#x27;s warning mean it should supplement code-based exact sequence analysis rather than replace it.

**Tags**: `#genomics`, `#large language models`, `#open weights`, `#bioinformatics`, `#Hugging Face`

---

<a id="item-tech-news-13"></a>
### [Claude API 2026-10-21 reportedly drops temperature and changes auth](https://x.com/ClaudeDevs/status/2113013247209021918) ⭐️ 7.0/10

A Telegram/X repost of a ClaudeDevs post claims Anthropic has released Claude API version 2026-10-21, described as the first formal API version update since 2023. The version reportedly removes the temperature, top\_p, and top\_k parameters, returning HTTP 400 if they are still passed, and switches SDK and ant CLI defaults to the new version while changing authentication to an Authorization: Bearer header; the older 2023-06-01 version is said to remain available. These details have not been independently confirmed.

telegram · zaihuapd · Oct 22, 03:54

**「Background」** Anthropic&\#x27;s Claude Messages API has been versioned with dated releases since 2023, with 2023-06-01 as the stable version and temperature, top\_p, and top\_k as standard sampling parameters. The 2026-10-21 version is the first dated API version released since then; Anthropic&\#x27;s migration guide confirms that requests still sending those three parameters get a 400 error and that 2023-06-01 is not deprecated.

**「Impact」** AI developers who rely on temperature, top\_p, or top\_k should remove those parameters or continue pinning the 2023-06-01 API version, because the new version is reported to reject them with HTTP 400 and the SDK and CLI defaults will move to the new version.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/api/migration-2026-10-21">Migrating to API version 2026-10-21 - Claude Platform Docs</a></li>
<li><a href="https://aicoder.com/news/news-20261022-anthropic-claude-api-version-2026-10-21-sdk-majors">Claude API ships version 2026-10-21, its first since 2023 ...</a></li>

</ul>
</details>

**Tags**: `#Claude API`, `#Anthropic`, `#breaking change`, `#API update`, `#AI`

---

<a id="item-tech-news-14"></a>
### [Tesla says Cybercab sales start by end of year; FSD slips to Q2](https://techcrunch.com/2026/10/21/tesla-says-it-will-start-selling-cybercabs-by-end-of-year/) ⭐️ 7.0/10

Tesla said on its third-quarter earnings call that it will begin selling Cybercabs to customers by the end of the year. Engineering VP Lars Moravy said current production is going entirely to Tesla&\#x27;s own robotaxi fleet, with small-scale customer deliveries of the fully autonomous vehicles to follow. The steering-wheel-less two-seater is under NHTSA investigation over federal safety standards, and Elon Musk said the unsupervised FSD rollout is delayed to the second quarter of next year, with Cybercab mainly positioned as a ride-hail service rather than a personal purchase.

telegram · zaihuapd · Oct 22, 07:54

**「Background」** Tesla&\#x27;s Cybercab is a purpose-built autonomous vehicle with no steering wheel, designed as a robotaxi rather than a conventional passenger car. The company has said it expects the vehicle to be used mainly for ride-hailing services rather than personal ownership, which is why current production is being directed to Tesla&\#x27;s own robotaxi fleet.

**「Impact」** For would-be buyers, the immediate practical consequence is limited availability: Tesla says all current Cybercab production is going to its own robotaxi fleet, with only small-scale customer deliveries to follow, and federal regulators are investigating whether the no-steering-wheel, no-pedal, no-mirror vehicle was properly certified under U.S. safety standards. That investigation, opened after commercial deployment in Austin, could affect the planned end-of-year sales, while customers waiting for unsupervised FSD now face a delay to the second quarter of next year.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cleverdude.com/content/nhtsa-opens-investigation-into-tesla-cybercab-safety-certification-after-austin-launch/">NHTSA Opens Investigation Into Tesla Cybercab Safety Certification...</a></li>
<li><a href="https://www.nytimes.com/2026/09/04/business/tesla-cybercab-nhtsa-investigation.html">Tesla ’s Cybercab Is Being Investigated by Federal Regulators</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#autonomous-vehicles`, `#robotaxi`, `#FSD`, `#EV`

---

<a id="item-tech-news-15"></a>
### [Study: Some Smart TVs Still Send Telemetry After ACR Is Disabled](https://watchingthewatchers.github.io/watchingthewatchers/index.html) ⭐️ 7.0/10

A study of 12 smart TVs from 10 vendors in the US ran 5,943 controlled experiments and found that some models continued sending content-related telemetry after users disabled automatic content recognition \(ACR\). VIDAA OS transmitted data over plaintext MQTT, including a non-resettable device ID and audio fingerprints, while Vizio&\#x27;s WatchFree+ sent show titles in unencrypted DNS queries that users cannot turn off. The findings indicate that the ACR setting alone is not a reliable privacy control on these platforms.

telegram · zaihuapd · Oct 22, 09:50

**「Background」** Automatic content recognition \(ACR\) is a smart TV feature that identifies what is playing on screen and reports it for analytics and advertising. Vizio&\#x27;s privacy policy and support documentation describe this as &\#x27;Viewing Data&\#x27; and say users can turn it off on supported models and that no viewing data is collected in Canada or when the TV is offline. The study tests whether that official setting actually stops content-related traffic.

**「Impact」** Users concerned about viewing privacy on smart TVs should not assume that turning off ACR stops content reporting; on VIDAA- and Vizio-based sets, viewing data may still be exposed in cleartext, so network-level blocking or using a separate streaming device may be necessary.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vizio.com/en/terms/privacy-policy/viewing-data-privacy-policy">Viewing Data Supplement - VIZIO</a></li>
<li><a href="https://classlawdc.com/2026/09/09/vizio-smart-tv-viewing-data-and-acr-privacy-investigation/">VIZIO Smart TV Viewing Data and ACR Privacy Investigation</a></li>
<li><a href="https://support.vizio.com/s/article/Smart-Interactivity-Broadcast-Interactivity-FAQ-How-to-turn-Smart-Interactivity-Broadcast-Interactivity-on-or-off?language=en_US">How to turn Viewing Data On, Off, or Delete - VIZIO Support</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#smart-tv`, `#ACR`, `#security`, `#telemetry`

---

<a id="item-tech-news-16"></a>
### [miHoYo and Tsinghua Open Source GameScaling Game-Operation Model](https://arxiv.org/abs/2610.28698v1) ⭐️ 7.0/10

miHoYo&\#x27;s Honkai AI team, together with Tsinghua University, open-sourced GameScaling, a game-operation model built by continued pretraining of the Qwen3.5 vision-language model on keyboard/mouse actions. It releases eight checkpoints from 0.8B to 27B parameters plus an Apache-2.0 inference client, and each output predicts 200 milliseconds of future actions. The accompanying paper evaluates 120 training configurations, but training code is not included.

telegram · zaihuapd · Oct 22, 11:32

**「Background」** GameScaling belongs to the emerging category of game-operation models: neural networks that take game-screen visual input and predict the next keyboard and mouse actions, instead of producing text or images. It is built by taking Qwen3.5, a vision-language model family, and applying continued pre-training for game control, so the model learns to map visual game states directly to input actions. This specialization approach lets a general multimodal model act as a game agent for desktop-style games.

**「Impact」** Game-agent developers can now run the 0.8B-to-27B checkpoints locally through the Apache-2.0 inference client and use the 200 ms action-prediction capability outside miHoYo, but the missing training code means the reported 120-configuration scaling study cannot be reproduced or extended by others.

**Tags**: `#game AI`, `#vision-language models`, `#open source`, `#AI research`

---

<a id="item-tech-news-17"></a>
### [Report: Banned Nvidia B300 Servers Reached China Via State-Backed Lease](https://theinference.org/article/china-s-state-money-bought-banned-nvidia-b300-servers-then-redacted-the-receipts) ⭐️ 7.0/10

A report alleges that Chinese state-controlled leasing firm Semiconductor Leasing financed 32 ASUS servers carrying banned Nvidia B300 accelerators for AI company Rongyao Shitu Technology, part of a 700-plus-server deal worth over 3 billion yuan planned for China Mobile&\#x27;s Ningxia hub. The B300 falls under the strictest US export-control tier and is effectively prohibited for China. After the filing drew attention, Semiconductor Leasing resubmitted its paperwork with the hardware description redacted. Nvidia said it is investigating with its manufacturing partners, while ASUS said it complies with export controls.

telegram · zaihuapd · Oct 22, 15:22

**「Background」** The B300 is Nvidia&\#x27;s latest AI accelerator and sits in the most restrictive tier of US export controls, making sales to China effectively banned. That embargo is the prerequisite for this report: the claimed purchase and financing of B300-equipped ASUS servers through a Chinese state-linked leasing company would, if confirmed, route embargoed hardware toward Chinese state-adjacent infrastructure.

**「Impact」** If the report is confirmed, it would show restricted US AI hardware reaching Chinese state-linked infrastructure through a leasing structure rather than a direct sale, potentially intensifying US scrutiny of financing arrangements in export-control enforcement. Nvidia and ASUS now face public compliance questions over the B300 supply chain.

**Tags**: `#Nvidia`, `#B300`, `#export controls`, `#AI hardware`, `#China`

---

<a id="item-tech-news-18"></a>
### [DeepSeek and MiniMax Complete Filing for Open Source and Overseas Licensing](https://mp.weixin.qq.com/s/hoeaIXEFagSHugSgMjFe9g) ⭐️ 7.0/10

China&\#x27;s Ministry of Commerce and Ministry of Science and Technology opened public consultation on Oct 16 on revising the export-control catalog, which covers 23 AI technology areas including large models, intelligent agents, computing clusters, and information processing. According to the report, DeepSeek and MiniMax have already completed registration and have continued open-source releases and overseas licensing under the new framework. The ministry&\#x27;s Q&amp;A emphasizes what is not subject to control, and the report frames the catalog as drawing boundaries rather than imposing a blanket export ban.

telegram · zaihuapd · Oct 22, 16:10

**「Context」** Horizon&\#x27;s October 17 digest reported that China&\#x27;s Ministry of Commerce proposed temporary registration and export controls on 40 technologies — including 23 AI-related categories such as large models, intelligent agents, and computing clusters — when the revised export-control catalog was opened for public comment on October 16. The current item is the first implementation follow-up: DeepSeek and MiniMax have completed registration and continued open-sourcing and overseas licensing, which the Commerce Ministry frames as boundary-setting rather than a blanket export ban.

**「Impact」** For Chinese AI vendors developing these technologies, the concrete implication is a compliance path: open-sourcing and overseas licensing remain permitted after registration under the current draft. Overseas users and developers relying on Chinese open-weight models should track the final catalog, since the 23 enumerated AI areas define where future export controls can apply.

<details><summary>References</summary>
<ul>
<li><a href="https://aqygzj.mofcom.gov.cn/flzc/gzjgfxwj/art/2026/art_c99f95ca0cd043829ac9991495fc283c.html">2026-10-17 — China proposes export registration for 40 AI, biotech, and solar technologies</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#export controls`, `#open source`, `#China AI`, `#DeepSeek`

---

<a id="item-tech-news-19"></a>
### [GNU Taler prepares to operate in Germany](https://www.taler.net/en/news/2026-13.html) ⭐️ 6.0/10

GNU Taler, the open-source, privacy-preserving payment system, has announced that it is getting ready to operate in Germany, signaling a step toward practical deployment rather than a live service. The announcement does not specify a launch date, availability conditions, or regulatory approvals, so users should treat this as a preparatory status update from the project.

hackernews · dewey · Oct 22, 16:14 · [Discussion](https://news.ycombinator.com/item?id=50197404)

**「Background」** GNU Taler is a free-software payment system whose electronic-cash model is designed to preserve payer privacy. In the original NGI TALER project plan, Bochum-based GLS Bank was assigned the role of e-money issuer for Taler in Germany, but GLS says it decided in January 2026 not to introduce Taler, prompting the consortium to work out alternative next steps and leading GNU Taler to form a new company. This history frames why the project is now preparing its own operations in Germany rather than relying on the originally planned bank issuer.

**「Impact」** German users interested in a privacy-preserving, open-source payment system now have a concrete alternative to watch, but Taler enters a market where Wero is already backed by major Western European banks and reportedly available to over 75% of personal bank customers in Belgium, France, and Germany. Wero has also accumulated nearly 50 million transactions worth more than €3 billion since its September 2024 launch, so Taler&\#x27;s adoption will depend on distribution, merchant acceptance, and whether it can differentiate on privacy despite Wero&\#x27;s existing bank integrations.

**「Community discussion」** Commenters disagreed about whether Taler&\#x27;s design can deliver real privacy, with one user criticizing its internet requirement and expiring e-money compared with Bitcoin and another predicting EU regulators will impose KYC at key junctions. Others debated its prospects against bank-backed Wero, while one commenter noted GLS Bank&\#x27;s involvement in both projects and hoped European payment independence improves.

<details><summary>References</summary>
<ul>
<li><a href="https://www.taler.net/en/news/2026-13.html">GNU Taler</a></li>
<li><a href="https://www.gls.de/taler/">Taler - in Zukunft digital &amp; sicher bezahlen - GLS Bank</a></li>
<li><a href="https://zeli.app/story/50197404">GNU Taler forms a new company to bring · Hacker News | Zeli</a></li>
<li><a href="https://www.werotracker.eu/">Wero Tracker - European Payment Adoption Progress</a></li>
<li><a href="https://wero-wallet.eu/about">Wero - All about Wero : Europe&#x27;s mobile payment solution</a></li>
<li><a href="https://epicompany.eu/media-insights/wero-successfully-positioned-itself-on-payments/">EPI Company | After 12 months of existence, Wero has ...</a></li>

</ul>
</details>

**Tags**: `#GNU Taler`, `#open-source`, `#digital payments`, `#privacy`, `#Germany`

---

<a id="item-tech-news-20"></a>
### [hackios-xnu-kernel boots iOS 16.5 firmware on Android devices and QEMU](https://github.com/oosexgang/hackios-xnu-kernel) ⭐️ 6.0/10

An open-source project, oosexgang/hackios-xnu-kernel, demonstrates booting iOS 16.5 firmware under QEMU and on select Android hardware, including the POCO X5 Pro 5G and some Xiaomi devices. The accompanying website frames the work as a research bench rather than a full ROM: each session lasts only a limited number of seconds, after which the kernel returns to the loader and hands over its log. So &quot;Run full iOS 16.5 firmware&quot; is best understood as an XNU/firmware bring-up demo, not a usable iOS replacement.

hackernews · aghuang · Oct 22, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50196718)

**「Background」** Horizon&\#x27;s October 20 digest reported a related community project that booted an unmodified iOS 16.7.16 userspace from an iPhone X on a Redmi Note 10 Pro by porting Apple&\#x27;s open-source XNU kernel to the Snapdragon 732G, reaching the home screen with CPU-only graphics at roughly 20–30 FPS and no Wi-Fi or camera support. That earlier bring-up demonstrates the approach of running iOS firmware on non-Apple hardware by adapting XNU rather than emulating the full system; the current GitHub project extends this kind of work to iOS 16.5 on QEMU and selected Android devices.

**「Impact」** Firmware researchers get a low-cost way to exercise the iOS 16.5 XNU kernel outside Apple hardware and inspect its boot logs, but the time-limited session design means it cannot serve as a persistent or app-usable iOS environment.

**「Community discussion」** Commenters clarified the demo&\#x27;s limits: SoKamil described it as a research bench where a session runs for a fixed number of seconds, then the kernel returns to the loader with its log, and speculated that AI guardrails may have encouraged that design. sanid separately warned that buyers of used iPhones should be careful about Android devices customized to look like iOS; these are community opinions, not independent confirmation of the project&\#x27;s claims.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/hackintosh/comments/1x95qq0/ios_16716_booting_on_a_snapdragon_732g_redmi_note/?sort=new">2026-10-20 — XNU Port Brings iOS 16.7.16 Booting to Redmi Note 10 Pro</a></li>

</ul>
</details>

**Tags**: `#iOS`, `#Android`, `#XNU kernel`, `#open source`, `#mobile OS research`

---

<a id="item-tech-news-21"></a>
### [KeePassXC 2.8.0 adds Qt6, Wayland Auto-Type, ARM64 builds](https://lwn.net/Articles/1102270/) ⭐️ 6.0/10

KeePassXC 2.8.0 has been released as a major update to the open-source password manager. The release migrates from Qt5 to Qt6, adds Auto-Type support on Wayland, configurable keyboard shortcuts, remote database synchronization with external tools, and quick unlock via password on macOS and via Polkit on Linux. It also ships the first native ARM64 builds for Windows and an experimental AArch64 AppImage for Linux, along with bug fixes and security updates.

rss · LWN.net · Oct 22, 13:34

**「Background」** Wayland&\#x27;s security model restricts global keyboard shortcuts and synthetic input events, which made features such as Auto-Type difficult for desktop password managers under Wayland sessions. The relevance of that limitation has grown as Wayland becomes the default for Linux desktops; Horizon&\#x27;s October 15 digest reported that KDE Plasma 6.8 dropped support for Plasma X11 sessions, while keeping X11 applications usable through XWayland. KeePassXC&\#x27;s new Wayland Auto-Type support therefore addresses a gap that matters more as Wayland-only desktop sessions spread.

**「Impact」** Wayland users gain Auto-Type support in this release, and Windows on ARM users receive a native build instead of relying on emulation. Existing users must upgrade to 2.8.0 to get these features and the accompanying security fixes.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1100429/">2026-10-15 — KDE Plasma 6.8 released with accessibility, Kup, and Wayland-only sessions</a></li>

</ul>
</details>

**Tags**: `#KeePassXC`, `#password-manager`, `#open-source`, `#security`, `#Linux`

---

<a id="item-tech-news-22"></a>
### [Upcoming Rust features for kernel developers at Kangrejos 2026](https://lwn.net/Articles/1099606/) ⭐️ 6.0/10

Josh Triplett&\#x27;s Kangrejos 2026 talk, reported by LWN, outlined Rust features under active development that kernel developers have been hoping for, including type-system refinements, syntax improvements, and a smarter borrow checker. The talk gave kernel developers ideas for how to use these upcoming features in the kernel, but none are stabilized yet, so they remain plans rather than shipped capabilities.

rss · LWN.net · Oct 22, 13:19

**「Background」** Kangrejos is an annual conference focused on using Rust in the Linux kernel, and Horizon&\#x27;s earlier coverage of the 2026 event reported two other proposed language and kernel improvements: self-referential data structures implemented without unsafe code, and checked cross-crate forward declarations. Against that backdrop, Josh Triplett&\#x27;s talk surveyed the broader Rust feature roadmap that kernel developers might eventually rely on, rather than any single shipped capability.

**「Impact」** Kernel developers now have an early roadmap of Rust language changes to consider when planning kernel code, but they should avoid depending on these features until they are stabilized.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1099224/">2026-10-17 — Safe self-referential structures proposed for kernel Rust</a></li>
<li><a href="https://lwn.net/Articles/1099596/">2026-10-20 — Cross-crate forward declarations proposed for Rust</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#kernel development`, `#programming languages`, `#borrow checker`, `#type system`

---

<a id="item-tech-news-23"></a>
### [LWN Weekly Edition for October 22, 2026 Lists Kernel and Security Stories](https://lwn.net/Articles/1100612/) ⭐️ 6.0/10

LWN&\#x27;s October 22, 2026 Weekly Edition presents an index of linked stories on Android vendor hooks, reproducible builds and kernel integrity, Rust data structures and XArray work, NFS server changes, setting no\_new\_privs for PID 1, Rust cross-crate declarations, 7.3 statistics, and Nix flakes. The briefs section covers the eMudhra CA compromise, PHP RCEs, Node.js and musl vulnerabilities, GNOME OS, OpenBSD 8.0, Ubuntu 26.10, and TAB results.

rss · LWN.net · Oct 22, 00:29

**「Background」** Android vendor hooks are the preferred mechanism for carrying out-of-tree kernel changes on Android devices. Horizon&\#x27;s October 16 digest reported that at the 2026 Linux Plumbers Conference, a session led by Todd Kjos found current devices still contain significant out-of-tree code even after the move to a generic kernel image brought Android kernels closer to mainline.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1098493/">2026-10-16 — LPC 2026 session examines Android vendor hooks</a></li>

</ul>
</details>

**Tags**: `#Linux kernel`, `#Rust`, `#security`, `#reproducible builds`, `#Nix`

---

<a id="item-tech-news-24"></a>
### [Open-XTTS-Trainer brings XTTS v2 training to new language scripts](https://www.reddit.com/r/MachineLearning/comments/1xcurgj/i_built_openxttstrainer_now_you_can_add_new/) ⭐️ 6.0/10

The author announced Open-XTTS-Trainer, an open-source MPL-2.0 suite that adds training and fine-tuning pipelines for all three XTTS v2 components: the DVAE audio tokenizer, the GPT text/vocab extender, and the Latent HiFi-GAN vocoder. It also claims to support adding new Unicode scripts beyond XTTS v2&\#x27;s original 17 languages by discovering glyphs and resizing the GPT embedding matrix without corrupting existing weights. The reported results are self-tested on an NVIDIA T4 with real speech, showing a 67% drop in HiFi-GAN mel reconstruction loss \(190.83 to 63.49\), a 67% drop in DVAE mel error \(8.14 to 2.71\), and stable discriminator scores at 3.62. These benchmarks verify component-level convergence and gradient stability only, not full end-to-end inference, which the author says still requires connecting the trained modules into the standard XTTS generation pipeline.

reddit · r/MachineLearning · /u/yashubhakt · Oct 22, 21:03

**「Background」** XTTS v2 is Coqui AI&\#x27;s open-source zero-shot text-to-speech model, but after Coqui shut down, its three components—the DVAE audio tokenizer, the GPT-based language model, and the Latent HiFi-GAN vocoder—had no unified official training code; only GPT fine-tuning was commonly available. The model&\#x27;s tokenizer was also hardcoded to a fixed 17-language vocabulary, so adapting it to new Unicode scripts such as Arabic, Hindi, and Thai caused out-of-vocabulary errors and embedding-matrix crashes.

**「Impact」** Developers who need to retrain XTTS v2&\#x27;s DVAE or latent HiFi-GAN components, or extend it beyond its fixed 17-language vocabulary — the exact gap raised in coqui-ai/TTS issue \#3323 — now have a single MPL-2.0-licensed pipeline that dynamically resizes the GPT embedding matrix for new Unicode scripts and avoids the torchcodec dependency block on modern PyTorch. Adopters should treat the reported loss convergence as the author&\#x27;s self-measured results pending independent reproduction.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/amitbhakt/open-xtts-trainer">amitbhakt/open-xtts-trainer · Hugging Face</a></li>
<li><a href="https://github.com/coqui-ai/TTS/issues/3323">Retraining vocoder (hifigan) and dvae in XTTS #3323 - GitHub</a></li>

</ul>
</details>

**Tags**: `#text-to-speech`, `#XTTS-v2`, `#open-source`, `#model training`, `#ML tooling`

---

<a id="item-tech-news-25"></a>
### [SteerTTS Edge Shrinks to 11.84 MB with Unchanged WER](https://www.reddit.com/r/MachineLearning/comments/1xcum4s/we_shrank_our_steerable_small_tts_to_1184_mb_wer/) ⭐️ 6.0/10

The author released SteerTTS Edge, an int4-quantized on-device version of the steerable English TTS that ships everything—weights, voices, numpy front end, and Python runtime—in 11.84 MB. Compared with the fp32 model, WER stays at 0.96% while UTMOS drops from 4.20 to 4.11, and quantization-aware training preserves at least 95% of each of the 12 steering controls. It runs on CPU with RTF 0.053 and about 120 ms to first audio, but weights are dequantized to fp32 at load, and the edge release is English-only with 200 voices and no voice cloning or flow refiner.

reddit · r/MachineLearning · /u/Working\_Hat5120 · Oct 22, 20:57

**「Background」** The author&\#x27;s earlier SteerTTS v1 was a small English text-to-speech model whose output is steered with numeric controls for rate, loudness, pitch, pauses, breathiness, and similar properties. The new edge release is a follow-up: the same steering system compressed through int4 quantization-aware training of the acoustic model and distillation of a smaller int4 vocoder, sized for what an app must ship on device.

**「Impact」** Developers targeting on-device deployment get a steerable English TTS in an 11.84 MB package with no measured intelligibility change, but they should not expect runtime memory or speed savings because weights are dequantized to fp32 at load; those needing voice cloning, free-text prompts, or the flow refiner must stay with the full model.

**Tags**: `#text-to-speech`, `#model compression`, `#quantization`, `#on-device AI`, `#speech synthesis`

---

<a id="item-tech-news-26"></a>
### [Frontier models struggle to label ASMR trigger sounds in benchmark](https://www.reddit.com/r/MachineLearning/comments/1xcbqdm/frontier_models_are_bad_at_hearing_asmr_8_judges/) ⭐️ 6.0/10

A Reddit user benchmarked eight frontier models as automatic labelers for 480 ASMR clips and found they perform poorly against human labels on physical trigger sounds, despite low per-clip costs. Gemini 3.1 Pro achieved the best trigger F1 at 0.325 against human labels and cost $0.0088 per clip, while MiMo v2.6 Pro cost $0.0008 with F1 of 0.243; the two spectrogram-image judges, Claude Opus 5.5 and Grok 4.7, scored much lower at 0.121 and 0.110. The models labeled whispering well, with F1 between 0.70 and 0.79, but frequently missed or mislabeled sounds like paper, brushing, cutting, sticky, and spraying. The benchmark is informal and based on a single user&\#x27;s setup, so the numbers indicate a practical limitation rather than a rigorous evaluation.

reddit · r/MachineLearning · /u/MissAppleby · Oct 22, 07:10

**「Background」** The author is training text2asmr, a text-to-ASMR model, and needs about 126,000 training clips tagged with the sounds they contain, such as tapping, crinkling, and brushing. For this task, frontier models are tested as cheap automatic labelers, and their outputs are compared against human-provided class labels from FSD50K, ESC-50, and the author&\#x27;s own ASMR clip labeling site.

**「Impact」** Practitioners building fine-grained audio training sets should not rely on frontier-model labels for quiet foley sounds without validation, because even the best model in this test missed most brushing and paper events on real ASMR clips. The author is responding by fusing multiple judges with Dawid-Skene weighting, sending uncertain clips to human labelers first, and plans to release the trained model&\#x27;s labels and weights.

**Tags**: `#machine learning`, `#audio tagging`, `#ASMR`, `#frontier models`, `#benchmark`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Software is slow because of design, not language choice](https://seangoedecke.com/software-is-slow-because-of-bad-design-not-slow-languages/) ⭐️ 8.0/10

rss · Sean Goedecke · Oct 23, 00:00

**「Background」** Sean Goedecke argues that the current fashion for using AI to rewrite software in fast languages like C or Rust will rarely deliver the dramatic speedups people expect. His starting point is that most real programs are not limited by language speed but by waits for input and output, so rewriting them changes only a small part of the total time.

**「Solution」** For an I/O-bound program, Goedecke says Amdahl&\#x27;s law puts a hard ceiling on gains from language rewrites: if half the time is spent querying a database, a C rewrite can only affect the other half. Even CPU-bound work in slow languages is often already delegated to fast libraries such as cmark-gfm for markdown rendering or C-backed numerics for Python machine learning. His strongest example is Bryan Cantrill&\#x27;s Rust rewrite of a C program: the naive Rust version ran 30% faster simply because the language&\#x27;s preferred B-tree data structure was more cache-efficient, showing that design choices dominate raw language speed. Goedecke ties this to his own experience, where most significant speedups came from caching, moving work into background jobs, parallelizing operations, fixing N+1 queries, and skipping unnecessary work, all of which are unrelated to language performance and often easier to spot in a readable high-level language.

**「Takeaway」** Goedecke concludes that serious optimization should start with profiling and redesigning what a program does rather than rewriting it in a faster language. Language rewrites may be worthwhile for portability or maintainability, but raw speed gains will mostly come from doing less work.

**Tags**: `#performance`, `#I/O-bound`, `#Amdahl&\#x27;s law`, `#software design`, `#optimization`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China’s CSI 300 Nears Bear Market After 20% Drop From June Peak](https://www.bloomberg.com/news/articles/2026-10-22/china-stocks-set-for-bear-market-as-ai-trade-policy-hopes-fade) ⭐️ 8.0/10

China’s CSI 300 fell 1.7% on Thursday, bringing its cumulative drop from the June peak to 20% and pushing A-shares close to a bear market. The sell-off came after battery maker CATL lost 12% on Wednesday when quarterly profit growth missed expectations and hopes for fiscal stimulus and AI-related policy faded.

telegram · zaihuapd · Oct 22, 05:05

**「Background」** The decline was driven by a lack of substantive fiscal stimulus and disappointing earnings; the ChiNext index has now fallen for 16 consecutive sessions, and the Hang Seng Tech Index dropped more than 4.5%.

**「Impact」** Strategists say that without new policy or technology catalysts, volatile trading could persist into early 2027, leaving investors in Chinese A-shares and Hong Kong tech stocks with limited near-term relief.

**Tags**: `#A股`, `#沪深300`, `#熊市`, `#宁德时代`, `#科技股`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Anthropic announces Claude-based formal verification at scale](https://x.com/AnthropicAI/status/2113390212911083894) ⭐️ 9.0/10

Anthropic&\#x27;s Frontier Red Team blog published research on using Claude for large-scale formal verification. The post explains that formal verification can prove code is free of certain bugs, but historically it was only feasible for small codebases or required significant expert time. Working with Theorem Labs, Anthropic used Claude to prove security properties in over one hundred real-world open-source libraries within a few weeks, describing this as a major scalability milestone for applying AI to formal verification.

twitter · AnthropicAI · Oct 22, 22:01

**「Background」** On October 22, 2026, Anthropic announced on X a new Frontier Red Team blog post describing the use of Claude for large-scale formal verification. According to the post, formal verification can prove that code is free of certain bugs, but has historically been feasible only for small codebases or required substantial expert time. Anthropic says that, in collaboration with Theorem Labs, Claude was used to prove security properties in over 100 real-world open-source libraries in the span of a few weeks.

This announcement follows earlier Anthropic security and verification milestones. Archived summaries from October 2026 describe Anthropic expanding its Cyber Verification Program for verified security professionals, including new tiers for authorized offensive security work such as penetration testing and red-teaming; launching OSS Scanner, a free tool that uses frontier models to scan opted-in open-source projects for vulnerabilities and produce proof-of-concept, explanation, and suggested-fix reports; and reporting progress against distillation attacks on Claude without providing technical specifics in the post itself.

The linked research page adds that Theorem, the collaborator on this project, is offering to run the same pipeline for other open-source projects and is publishing a Claude skill to help developers verify their own code. The work also follows Anthropic&\#x27;s sharing of a first complete computer-checked proof of Fermat&\#x27;s Last Theorem, which Claude worked largely autonomously over 11 days to write in the Lean programming language.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2107546569654636883">2026-10-07 — Anthropic Expands Cyber Verification Program for Security Professionals</a></li>
<li><a href="https://x.com/AnthropicAI/status/2108302543977906649">2026-10-09 — Anthropic launches OSS Scanner for open-source security</a></li>
<li><a href="https://x.com/AnthropicAI/status/2109795898909950247">2026-10-13 — Anthropic announces progress against distillation attacks on Claude</a></li>
<li><a href="https://www.anthropic.com/research/formal-verification">Formally verifying real-world software with Claude \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/formalizing-fermats-last-theorem">Formalizing Fermat&#x27;s Last Theorem \ Anthropic</a></li>
<li><a href="https://www-cdn.anthropic.com/9e431dff043da6538d99d6c2d231b670aa3da263.pdf">PDF Formalizing Fermat&#x27;s Last Theorem in Lean - www-cdn.anthropic.com</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#AI`, `#Claude`, `#security`, `#research`

---

<a id="item-twitter-news-2"></a>
### [OpenAI announces METR and Redwood Research embedded evaluation](https://x.com/OpenAI/status/2113298833392496746) ⭐️ 7.0/10

OpenAI posted on October 22, 2026 that during the summer it invited METR and Redwood Research to pilot an embedded evaluation of OpenAI&\#x27;s internal monitoring system. The pilot involved deep access to OpenAI infrastructure over three weeks. According to OpenAI, the findings helped strengthen safeguards as the system was expanded and will help shape future research collaborations with METR and other third-party evaluators. This is OpenAI&\#x27;s own announcement; no detailed technical methodology or independent results were included. No community comments were available for this item.

twitter · OpenAI · Oct 22, 15:57

**「Background」** OpenAI said it invited METR and Redwood Research to pilot an embedded evaluation of its internal monitoring system, providing deep access to its infrastructure over three weeks. According to the announcement, their findings helped strengthen safeguards as the system was expanded and will help shape future research collaborations with METR and other third-party evaluators. The post does not disclose specific findings or technical details about the monitoring system.

The move follows a concrete precedent in the same period: days earlier, Anthropic announced it had given a METR team employee-like access for third-party safety evaluation, saying it was in discussions with multiple organizations about having evaluators assess its safety practices. This signals a broader shift by frontier labs toward granting external evaluators deeper, more operational access.

The evaluation also comes amid heightened scrutiny of monitoring at frontier labs. Around the same time, security experts argued in press coverage that recent reports of AI agents hacking systems stemmed from insecure sandboxing and poor monitoring rather than models secretly going rogue, citing a METR report and a Hugging Face incident involving an Artifactory sandbox escape. Those discussions help explain why internal monitoring capabilities have become a focus of external evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2110784662071398807">2026-10-16 — Anthropic grants METR employee-like access for third-party safety evaluation</a></li>
<li><a href="https://www.csoonline.com/article/4234854/ai-agents-arent-going-rogue-frontier-labs-are-skipping-security-basics.html">2026-10-15 — AI Hacking Reports Blamed on Sandbox and Monitoring Failures, Experts Say</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#evaluation`, `#third-party audit`

---