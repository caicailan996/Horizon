---
layout: default
title: "Horizon Summary: 2026-11-19 (EN)"
date: 2026-11-19
lang: en
---

> From 76 items, 26 important content pieces were selected

---

**Technology News**
1. [Google announces Gemini 4 Neon](#item-tech-news-1) ⭐️ 9.0/10
2. [Xint discloses five nginx flaws plus Linux kernel bug; patched in 1.30.7/1.31.9](#item-tech-news-2) ⭐️ 9.0/10
3. [Daniel Stenberg: AI Rust Rewrites Lack curl&\#x27;s 200+ Bug Fixes](#item-tech-news-3) ⭐️ 8.0/10
4. [Unverified &\#x27;Java4Shell&\#x27; RCE claim targets Java 17+ on AVX-512 CPUs](#item-tech-news-4) ⭐️ 8.0/10
5. [Microsoft announces seven AI models at Ignite 2026 on price-performance](#item-tech-news-5) ⭐️ 7.0/10
6. [Quad9 Leaves France Over DNS Piracy Blocking Orders](#item-tech-news-6) ⭐️ 7.0/10
7. [Google DeepMind announces Genie 4 world model](#item-tech-news-7) ⭐️ 7.0/10
8. [WeChat AI assistant Xiaowei expands test, hits 30M daily users](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI touts AI-assisted chip design; commenters question withheld RISC-V work](#item-tech-news-9) ⭐️ 6.0/10
10. [Energy-Based Reasoners Claims 385x More Efficient Inference](#item-tech-news-10) ⭐️ 6.0/10
11. [DeepSeek drops separate fees for server-side search and web scraping](#item-tech-news-11) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly Intel XPU Wheel](#item-ai-projects-1) ⭐️ 7.0/10
2. [LMCache nightly-rbln: RBLN NPU wheel for KV cache offloading](#item-ai-projects-2) ⭐️ 7.0/10
3. [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache nightly: CUDA 13.0 wheels for linux/amd64 and linux/arm64](#item-ai-projects-4) ⭐️ 5.0/10

**Financial News**
1. [Fed minutes show officials expect more rate hikes and flag AI risks](#item-finance-news-1) ⭐️ 9.0/10
2. [Fed’s Waller says central bank may need to ‘shock people’ with half-point rate hike](#item-finance-news-2) ⭐️ 8.0/10
3. [📱 美国芯片新规致 4.8 亿美元字节跳动 GPU 贷款暂停](#item-finance-news-3) ⭐️ 7.0/10
4. [UK House of Commons passes Immigration and Asylum Bill 290-94](#item-finance-news-4) ⭐️ 7.0/10
5. [Tencent Q3 2026: revenue up 8%, AI capital spending surge pushes free cash flow negative](#item-finance-news-5) ⭐️ 7.0/10
6. [China, South Korea announce substantive conclusion of FTA services and investment talks](#item-finance-news-6) ⭐️ 7.0/10

**Twitter News**
1. [Anthropic prices IPO at $83 per share, Nasdaq trading expected to begin](#item-twitter-news-1) ⭐️ 8.0/10
2. [OpenAI shares data on AI&\#x27;s role in research, calls for mandatory RSI reporting](#item-twitter-news-2) ⭐️ 8.0/10
3. [Google announces Gemini 4 Neon, a frontier model with 1M-token context and adjustable thinking](#item-twitter-news-3) ⭐️ 8.0/10
4. [OpenAI shares its approach to safety across the model lifecycle](#item-twitter-news-4) ⭐️ 6.0/10
5. [Lenny Rachitsky on Muse&\#x27;s Two Biggest Activation Levers](#item-twitter-news-5) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google announces Gemini 4 Neon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/) ⭐️ 9.0/10

Google announced Gemini 4 Neon, a new model in its Gemini family, in a post on its official blog dated November 18, 2026. The supplied source material contains no specifications, benchmark figures, pricing, context-window details, or availability terms, so the announcement&\#x27;s concrete capabilities and the conditions under which developers can use the model cannot be verified from the available evidence. Details circulating about how Neon performs and where it sits in the Gemini lineup come from third-party metrics and community reports rather than from the source item itself.

hackernews · yigitdemirag · Nov 18, 21:34 · [Discussion](https://news.ycombinator.com/item?id=50552424)

**「Background」** Google has been rolling out the Gemini 4 family in stages: Horizon&\#x27;s October 29 digest reported the introduction of Gemini 4 Carbon, a frontier model aimed at long-horizon autonomous engineering and cybersecurity, and Horizon&\#x27;s November 13 digest reported Gemini 4 Hydrogen, a faster Flash-class model, in Google Antigravity. Gemini 4 Neon is the next release in that sequence, with external coverage placing it between Hydrogen and Carbon in the lineup.

**「Impact」** Developers can already call Gemini 4 Neon through OpenRouter, including EU in-region routing that decrypts requests in the EU and routes them only to shared provider endpoints in Europe, the UK, and Switzerland \(tool-3-3\). Artificial Analysis measured 61 on its Intelligence Index, above the 43 median for comparable models, but also recorded unusually high verbosity — 283M tokens generated versus a 65.1M median \(tool-3-1\), so teams should expect token-based cost and latency to scale with output length rather than with benchmark score alone.

**「Community discussion」** Commenters focused on model positioning and naming: one described Neon as scoring higher than Gemini 4 Carbon on an aggregate index while scoring lower on research-scale reasoning evaluations such as CritPt, arguing the frontier is becoming &quot;jagged&quot; with models that are less capable overall but stronger on specific tasks. Others said the proliferation of model names across vendors has become hard to map to use cases, and one reported that Neon was being served via OpenRouter at roughly 127 tokens per second versus about 46 for Carbon, calling the speed difference confusing. A separate thread compared Gemini models unfavorably to Anthropic&\#x27;s Opus 5.5 on general perceived intelligence despite benchmark parity; these are individual opinions, not verified results.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/">2026-10-29 — Google introduces Gemini 4 Carbon with cybersecurity focus and introductory pricing</a></li>
<li><a href="https://antigravity.google/blog/gemini-4-hydrogen-in-google-antigravity/">2026-11-13 — Google Antigravity Introduces Gemini 4 Hydrogen and Orchestrator</a></li>
<li><a href="https://www.youtube.com/watch?v=Q0ShBenKyqo">Gemini 4 Neon Is Here, And It’s a Beast! - YouTube</a></li>
<li><a href="https://artificialanalysis.ai/models/gemini-4-neon">Gemini 4 Neon Models - Intelligence, Performance... | Artificial Analysis</a></li>
<li><a href="https://openrouter.ai/google/gemini-4-neon">Gemini 4 Neon - API Pricing &amp; Providers | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#Google Gemini`, `#LLM release`, `#machine learning`, `#model benchmarking`

---

<a id="item-tech-news-2"></a>
### [Xint discloses five nginx flaws plus Linux kernel bug; patched in 1.30.7/1.31.9](https://nginx2root.com/) ⭐️ 9.0/10

Security researcher Xint has disclosed a chain called NGINX2Root: five nginx vulnerabilities combined with a Linux kernel flaw that it says can take an unauthenticated nginx visitor to host root. The most severe nginx issue, CVE-2026-123007, is an HTTP/2 flow-control memory corruption that allows command execution in an nginx worker without authentication, according to the disclosure. nginx versions 1.30.7 and 1.31.9, dated November 18, fix 10 CVEs in total; Rapid7 has published a proof-of-concept, and the report says there is no known in-the-wild exploitation. If upgrading is not possible, the suggested mitigation is to disable externally facing HTTP/2, though the disclosure is currently single-source and not independently confirmed.

telegram · zaihuapd · Nov 18, 16:21

**「Background: CVE-2026-123007」** CVE-2026-123007, the nginx flaw in the reported chain, is described by Rapid7 and F5 as an integer underflow in nginx&\#x27;s HTTP/2 handling: crafted requests push the per-connection flow-control window past its permitted limits, producing a heap-based buffer overflow that Red Hat says can yield arbitrary code execution or a denial of service. Rapid7&\#x27;s accompanying repository publishes standalone reproduction steps and a minimal Python trigger script, so the root cause can be exercised directly rather than only as part of a full exploit chain.

**「Impact」** Anyone exposing nginx with HTTP/2 enabled has to either upgrade to nginx 1.30.7 or 1.31.9, the releases carrying the fixes for the 10 CVEs, or disable HTTP/2 on externally reachable listeners until they can upgrade. Because the reported chain ends in a Linux kernel privilege escalation rather than an nginx flaw, operators running nginx in containers should also verify kernel patch levels: kernel flaws of this class have been documented to allow root access and container escape, and are fixed through kernel or distribution updates, not nginx releases.

**「Community discussion」** Commenters noted that HTTP/2 is not enabled by default in nginx and, citing W3Techs, that roughly 12% of servers run it; one commenter also argued that the bug had been fixed in the open-source repository a week earlier with a commit message crediting Xint.io, giving skilled attackers a monitoring window. Another flagged the Linux SCTP flaw used to escape the container as an apparent zero-day without a public CVE number yet.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sfewer-r7/CVE-2026-123007">GitHub - sfewer-r7/CVE-2026-123007: Proof-of-concept (PoC ...</a></li>
<li><a href="https://www.rapid7.com/blog/post/ve-cve-2026-123007-critical-nginx-http-2-integer-underflow-leads-to-rce-fixed/">Rapid7 discloses a critical vulnerability affecting NGINX ...</a></li>
<li><a href="https://access.redhat.com/security/cve/cve-2026-123007">CVE-2026-123007 - Red Hat Customer Portal</a></li>
<li>18-Year-Old Linux SCTP Flaw (CVE-2026-64564) Enables Root Access and Container Escape - Aviatrix</li>

</ul>
</details>

**Tags**: `#nginx`, `#security-vulnerabilities`, `#HTTP/2`, `#RCE`, `#Linux-kernel`

---

<a id="item-tech-news-3"></a>
### [Daniel Stenberg: AI Rust Rewrites Lack curl&\#x27;s 200+ Bug Fixes](https://simonwillison.net/2026/Nov/18/daniel-stenberg/) ⭐️ 8.0/10

Daniel Stenberg says that while AI agents converted 185,000 lines of C code into 340,000 lines of Rust over a little more than three weeks, the actual curl project merged over 300 commits in the same period, including more than 200 bug fixes and a few vulnerability fixes. He adds that in another month the project completed around 200 more fixes and possibly more vulnerability fixes, and asks whether the AI-generated Rust clones will keep up.

rss · Simon Willison · Nov 18, 15:58

**「Background」** The post responds to a broader pattern of AI coding agents producing Rust rewrites of established codebases; Horizon&\#x27;s October 30 digest reported that Anthropic used Claude to help rewrite its Messages API from Python to Rust, claiming roughly 40–50% lower CPU usage, figures the digest noted were not independently verified. Curl is a long-standing candidate for such rewrites because of its reach: Horizon&\#x27;s November 13 digest reported Stenberg&\#x27;s 30th-anniversary retrospective estimating about 30 billion libcurl installations, a figure he described as approximate because most users never disclose their usage.

**「Impact」** For users and organizations evaluating these Rust rewrites, Stenberg&\#x27;s figures imply the generated ports are snapshots that do not automatically inherit curl&\#x27;s upstream bug and security fixes, so keeping them current would require an ongoing plan to track and port changes from the maintained C project.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1107151/">2026-11-13 — Daniel Stenberg reflects on curl&#x27;s 30 years and 30 billion installs</a></li>
<li><a href="https://latent.space/p/opus55/">2026-10-30 — Anthropic Uses Claude to Rewrite Messages API in Rust, Cutting CPU 40–50%</a></li>

</ul>
</details>

**Tags**: `#curl`, `#Rust`, `#open-source maintenance`, `#AI coding agents`, `#security`

---

<a id="item-tech-news-4"></a>
### [Unverified &\#x27;Java4Shell&\#x27; RCE claim targets Java 17+ on AVX-512 CPUs](https://censys.com/advisory/cve-2026-114938/) ⭐️ 8.0/10

A Telegram post reports a critical unauthenticated remote code execution flaw, CVE-2026-114938, dubbed &quot;Java4Shell,&quot; with a CVSS 4.0 score of 9.2 and an alleged near-four-year latency. The post, citing Censys, says Java 17 \(17.0.6 and all later 17-line releases\), 21, 25, and 27 are affected, while standard Java 8 and 11 are generally unaffected except for Oracle Java 8 Performance Pack. It states the flaw only affects x86-64 server processors with the AVX-512 VBMI instruction set — roughly Intel chips from 2021 onward \(Ice Lake and newer Xeon\) and AMD chips from 2022 onward \(Zen 4 and newer EPYC/Ryzen\) — with ARM64 unaffected. No official vendor confirmation, advisory detail, proof-of-concept, or patch information was provided in the source, so the claim remains unverified.

telegram · zaihuapd · Nov 18, 03:55

**「Background」** Third-party write-ups trace CVE-2026-114938 to OpenJDK&\#x27;s hardware-accelerated Base64 decoder — the vectorized code path Java uses when the host CPU exposes AVX-512 VBMI — which is why exposure is tied to particular x86-64 server processors rather than to the operating system or to Java code that calls Base64. Those same write-ups describe it as a memory-corruption bug that permits unauthenticated remote code execution; the supplied material contains no vendor advisory, patch confirmation, or independent technical analysis.

**「Impact」** If confirmed, the affected population is narrow and identifiable: deployments running Java 17.0.6+, 21, 25, or 27 on AVX-512 VBMI-capable x86-64 servers, including Ice Lake-and-later Xeon and Zen 4-and-later AMD systems. Teams on those combinations should treat the report cautiously until a vendor advisory or patch appears, since the source gives no fixed version, workaround, or mitigation; standard Java 8 and 11 installations and ARM64 hosts are not implicated by the report.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=Eec2Ymlnktw">Java 4 Shell : Critical Java 0-Day? CVE - 2026 - 114938 ... - YouTube</a></li>
<li><a href="https://orca.security/resources/research/java4shell-critical-openjdk-base64-decoder-flaw-could-allow-unauthenticated-remote-code-execution/">Java 4 Shell CVE - 2026 - 114938 : Affected Versions &amp; Mitigation</a></li>
<li><a href="https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938">Java 4 Shell Java RCE: Fix &amp; Versions ( CVE - 2026 - 114938 )</a></li>

</ul>
</details>

**Tags**: `#Java`, `#security vulnerability`, `#remote code execution`, `#CVE-2026-114938`, `#AVX-512`

---

<a id="item-tech-news-5"></a>
### [Microsoft announces seven AI models at Ignite 2026 on price-performance](https://microsoft.ai/news/microsoft-ignite-2026/) ⭐️ 7.0/10

Microsoft announced seven new AI models at Ignite 2026, positioning them around scalable price-performance. The supplied account contains no benchmarks, technical details, or independent analysis, so the performance and price-performance claims remain vendor assertions rather than measured results.

hackernews · gmays · Nov 18, 16:08 · [Discussion](https://news.ycombinator.com/item?id=50548021)

**「Background」** Horizon&\#x27;s October 8 digest reported that Microsoft was among the companies reducing employee use of Anthropic&\#x27;s Claude AI, with the move reportedly aimed at cutting costs and favoring internal models — a report that carried no official confirmation and left the exact scope and timing unclear. The Ignite 2026 launch extends that cost-driven internalization: Microsoft is now positioning its own MAI family directly against rival frontier models on price rather than relying on outside vendors, and commenters in the current thread frame the release in exactly those terms, arguing over whether cheaper Microsoft models erode Anthropic&\#x27;s advantage.

**「Impact」** For developers and enterprises comparing AI models, the absence of published benchmarks and technical details means the seven models cannot be evaluated from the announcement alone; teams would need independent testing before choosing them over existing options.

**「Community discussion」** Commenters debated Microsoft&\#x27;s chances, with one arguing the company should release some models as open source or open weight to gain market share, and another reporting that MAI Code 2 performed well in hands-on use and was roughly comparable to Opus or Sol. Others focused on Anthropic&\#x27;s competitive position, arguing its moat would come from brand recognition and business-specific applications rather than model quality alone.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rswebsols.com/news/meta-and-microsoft-take-steps-to-reduce-employee-usage-of-claude-ai/">2026-10-08 — Report: Meta and Microsoft reduce employee use of Claude AI</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#Microsoft`, `#model releases`, `#price-performance`, `#AI industry`

---

<a id="item-tech-news-6"></a>
### [Quad9 Leaves France Over DNS Piracy Blocking Orders](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/) ⭐️ 7.0/10

Quad9 is leaving France after court-ordered DNS blocking demands tied to piracy enforcement, according to the article. The withdrawal means French users and organizations that rely on Quad9 as a public DNS resolver must switch to another provider to maintain name resolution. The article argues the episode shows why DNS resolvers are a technically and civil-liberties-poor place to enforce site-blocking orders.

hackernews · ritzaco · Nov 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=50545958)

**「Background」** Quad9 is a Swiss non-profit public recursive DNS resolver best known for blocking malware and phishing domains rather than content, and its operators have said the service has never blocked a domain. Horizon&\#x27;s October 6 digest reported that Quad9 was refusing a French court order sought by beIN Sports to block 58 pirate sports-streaming domains, risking fines of up to €580,000 per day \(€10,000 per domain per day\), on the grounds that it cannot block domains for French users only and would have to choose between a global block and leaving the country. Horizon&\#x27;s October 23 digest then reported Quad9&\#x27;s decision to exit France instead of complying, saying geoIP filtering cannot reliably enforce the orders because users can evade it with VPNs, and that it would probably block French users from its services via geoIP after November 24 — the step this item covers.

**「Impact」** For French network operators and users who have configured Quad9, the immediate action is to update DNS settings to another resolver so systems continue resolving names. The case also puts public resolvers on notice that complying with country-specific blocking orders may conflict with operating as neutral, global DNS infrastructure.

**「Community Discussion」** Commenters split over where blame lies, with skrebbel asking whether French judges misapplied a defensible law or faithfully applied a ridiculous one, and trentnix arguing that anti-piracy efforts short of prosecuting pirates are a backdoor to suppressing speech. Others focused on alternatives, including bemtavi&\#x27;s call for better paid media experiences such as DRM-free downloads for $2–$5 per movie, and AppalachianEng&\#x27;s claim that large AI companies&\#x27; use of copyrighted material makes prosecuting individual pirates inconsistent.

<details><summary>References</summary>
<ul>
<li><a href="https://quad9.net/news/blog/au-revoir-france/">2026-10-23 — Quad9 DNS Resolver Exits France Over Piracy Injunctions</a></li>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/">2026-10-06 — Quad9 refuses French DNS piracy blocks, faces €580K daily fines</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quad9">Quad 9 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#internet policy`, `#censorship`, `#net neutrality`

---

<a id="item-tech-news-7"></a>
### [Google DeepMind announces Genie 4 world model](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/) ⭐️ 7.0/10

Google DeepMind announced Genie 4, a new version of its generative world model, in a blog post. According to a commenter quoting the announcement, it is available to &quot;Eligible Google AI Ultra subscribers,&quot; but no further technical detail — such as capabilities, model size, or rollout timeline — is available in the supplied material. Commenters could not confirm their own eligibility: one said their Google AI Ultra account still advertises Genie 3, and speculated that the discrepancy might reflect UK region restrictions, citing a previous Genie version that was US-only.

hackernews · leumon · Nov 18, 18:49 · [Discussion](https://news.ycombinator.com/item?id=50550415)

**「Background」** Horizon&\#x27;s October 28 digest reported that DeepMind had announced Genie 4 as the next generation of its world-simulation model, with noted limitations in visual consistency and prompt adherence. At that announcement, Google said Genie 4 was rolling out to a limited group of trusted testers and would come soon to Google AI Ultra subscribers in Project Genie and to early-access partners through the Gemini API and AI Studio.

**「Impact」** For prospective users, Genie 4 appears gated behind a specific Google AI Ultra subscription tier rather than released generally, and at least one commenter reports that tier still shows Genie 3 instead. Until Google publishes clearer eligibility terms, users cannot verify from the announcement alone whether their account or region qualifies.

**「Community discussion」** Commenters were skeptical of the capabilities shown: int0x29 argued the demo video never pans away from an object and back without altering the scene, suggesting &quot;strong problems with object permanence,&quot; and koolala quoted a definition of a world model as one that can be spun 360° without surrounding details changing. A separate thread questioned why Google does not make access and payment terms clearer, and one long-time commenter said the discussion centered on pricing and capability while giving little attention to potential negative consequences of the technology.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/genie-4-a-new-generation-of-world-simulation/">2026-10-28 — DeepMind releases Genie 4 world-simulation model</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/introducing-genie-4/">We’re announcing Genie 4, our new world model for real-time ...</a></li>

</ul>
</details>

**Tags**: `#Google DeepMind`, `#world models`, `#generative AI`, `#AI product release`, `#Hacker News discussion`

---

<a id="item-tech-news-8"></a>
### [WeChat AI assistant Xiaowei expands test, hits 30M daily users](https://mp.weixin.qq.com/s/r3NthxJZQJgztyLADwNV4A) ⭐️ 7.0/10

Tencent said in its Q3 2026 earnings report that testing of WeChat&\#x27;s AI assistant, Xiaowei \(小微\), has been widened and that it now reaches 30 million daily active users, according to the WeChat account that reported the disclosure. The assistant is being folded into WeChat chats, Moments, Official Accounts and Channels. Xiaowei runs on a custom WeLM model tuned for cost efficiency, which Tencent says has low and still-falling inference cost, with some inference tasks expected to run on users&\#x27; devices in the future. The user figure and cost claims are Tencent&\#x27;s own and were not independently verified in the source, which gives no benchmark or architecture details.

telegram · zaihuapd · Nov 18, 11:35

**「Background: WeLM and the earlier Xiao Wei rollout」** Xiao Wei is not a new product line: earlier coverage reported that the assistant runs on Tencent&\#x27;s in-house WeLM model and was confirmed in the company&\#x27;s Q2 earnings report, with WeChat adding an AI entry point inside the app rather than shipping a standalone assistant app \(tool-2-1\). The same reporting said Xiao Wei primarily uses WeLM but hands some queries to DeepSeek \(tool-2-2\), while a third-party account describes WeLM as a sparse mixture-of-experts model with roughly 617 billion total parameters — a figure not confirmed in Tencent&\#x27;s own statement \(tool-2-3\). Horizon&\#x27;s November 9 digest also reported Tencent chief AI scientist Yao Shunyu arguing that AI companies&\#x27; moat sits in the product layer rather than the model layer, citing WeChat&\#x27;s access to a user&\#x27;s schedule and social graph as an advantage a stronger external model could not easily replicate \(tool-1-1\).

**「Impact」** For Tencent, serving an assistant at WeChat&\#x27;s scale is the cost problem the cost-optimized WeLM model and planned on-device inference address: local execution shifts compute onto the user&\#x27;s hardware, where each inference is essentially free for the developer once the model is downloaded, with no per-query meter \(tool-3-1, tool-3-3\). The trade-off is device dependence — Tencent says only that some inference tasks are expected to run on user devices in the future, not that this is shipping today.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/1/023/991.htm">2026-11-09 — 姚顺雨：AI 公司护城河在产品层而非模型层</a></li>
<li><a href="https://guibai.dev/a/7675936246981574697/">WeChat &#x27;s 16 AI Touchpoints Turn the Super-App Into an... — Guibai</a></li>
<li><a href="https://getretailbrief.com/story/tencent-wechat-ai-assistant-retail-commerce">Tencent WeChat AI Assistant Could Reshape Mobile Retail</a></li>
<li><a href="https://lapaasvoice.com/wechat-xiaowei-agent-welm-model/">WeChat Xiaowei Agent: WeLM Reaches 617B Parameters</a></li>
<li><a href="https://www.aimagicx.com/blog/on-device-ai-models-local-llm-guide-2026">On - Device AI in 2026: Running LLMs Locally on Your... | AI Magicx</a></li>
<li><a href="https://apptitude.io/blog/on-device-ai-mobile-apps-when-run-phone-vs-cloud/">On - Device AI for Mobile Apps: Phone vs Cloud Decision... | Apptitude</a></li>

</ul>
</details>

**Tags**: `#AI assistant`, `#Tencent WeChat`, `#LLM deployment`, `#on-device inference`, `#industry news`

---

<a id="item-tech-news-9"></a>
### [OpenAI touts AI-assisted chip design; commenters question withheld RISC-V work](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 6.0/10

OpenAI published a vendor announcement describing the use of its models to advance chip design, but the supplied item contains no technical details about the models, designs, performance, or release plans. The announcement drew a Hacker News discussion in which commenters noted that the resulting RISC-V designs appear not to be shared and questioned OpenAI competing with the same customers it serves. Because the source is promotional and no source content is available, claims about the work&\#x27;s effectiveness remain unverified here.

hackernews · vighneshiyer · Nov 18, 17:45 · [Discussion](https://news.ycombinator.com/item?id=50549493)

**「Background」** OpenAI had already put AI into its own silicon work before this post: it unveiled the Jalapeño inference ASIC at Hot Chips in August 2026, describing a design process that leaned heavily on AI and compressed the design window. In June 2026, OpenAI and Broadcom announced a custom AI chip design effort, with OpenAI seeking to reduce its dependence on Nvidia and AMD and gain leverage in negotiations with those suppliers.

**「Practical impact」** For open-source hardware developers, the announcement may yield no reusable artifacts: commenters questioned whether the resulting RISC-V designs will be shared, so teams should confirm licensing and availability before planning to build on the work. Chip-design teams adopting AI-assisted flows should also clarify ownership of model-generated RTL and EDA scripts, particularly as OpenAI is separately pursuing its own silicon.

**「Community discussion」** Commenters were skeptical that the RISC-V designs are not being shared and debated whether OpenAI can serve chip-design customers while competing with them. One practitioner reported positive results from treating chip design as a software problem—using agents to generate circuits, automate EDA flows, and babysit multi-hour simulations—while noting that only a small fraction of the design was RTL and the bulk was analog.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/openai-jalapeno-design-interview-transcript-hardware-vp-richard-ho-explains-how-ai-assisted-design-may-shape-the-future-of-inference-asics">OpenAI Jalapeño design interview transcript... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.nytimes.com/2026/06/24/technology/openai-broadcom-chip-jalapeno.html">OpenAI and Broadcom Unveil Custom A.I. Chip Design</a></li>
<li>OpenAI unveils its first custom chip, built by Broadcom - Hacker News</li>

</ul>
</details>

**Tags**: `#AI for chip design`, `#OpenAI`, `#EDA/hardware design`, `#open source hardware`, `#industry analysis`

---

<a id="item-tech-news-10"></a>
### [Energy-Based Reasoners Claims 385x More Efficient Inference](https://energy-based-reasoners.github.io/) ⭐️ 6.0/10

A project called Energy-Based Reasoners claims 385x more efficient inference, but the supplied evidence describes it as a project page/demo with an unverified benchmark rather than an independently reproduced result. For researchers and developers weighing energy-based models as alternatives to LLMs for reasoning tasks, the Hacker News discussion focuses on whether the approach can scale beyond narrow logic puzzles.

hackernews · frenchmajesty · Nov 18, 09:29 · [Discussion](https://news.ycombinator.com/item?id=50543989)

**「Background」** Energy-based models \(EBMs\) learn a scalar energy function that scores candidate predictions for a given input, and inference searches for low-energy answers instead of generating tokens left to right — the framing the project itself gives and that commenters quote. A commercial precedent predates this project: a January 2026 PaperLens write-up described Logical Intelligence&\#x27;s Kona 1.0 as the first commercial energy-based model for reasoning, with Turing Award winner Yann LeCun as founding chair of its technical research board, and the company published a February 2026 benchmark claiming 96% on Sudoku for its EBM versus 2% for LLMs.

**「Impact」** Developers weighing this project against LLM-based pipelines should treat the 385x inference-efficiency figure as a project-page claim rather than an independently reproduced result, since commenters with hands-on EBM experience describe the models as strong validators that are very hard to train and niche-specific, and report that a related sudoku solver does not scale. If the efficiency gain is confined to constraint-satisfaction puzzles, teams would need to benchmark it on their own workloads before substituting it for an LLM; published analyses of inference efficiency make the same caveat, noting that idealized benchmarks often miss the diverse real-world workloads that determine actual energy use \(tool-3-2\).

**「Community Discussion」** Commenters saw promise for constrained logic puzzles, but one commenter reported after a year of work that EBMs are impressive validators yet &quot;insanely hard to train&quot; and niche-specific, and challenged Logical Intelligence&\#x27;s Sudoku solver to scale to arbitrarily large puzzles. Others noted the paper lacks a precise definition of &quot;energy&quot; and that the results may apply only to a specific logic-puzzle problem set.

<details><summary>References</summary>
<ul>
<li><a href="https://paperlens.io/idea/kona-1/">Kona 1: Energy-Based Reasoning | PaperLens</a></li>
<li><a href="https://logicalintelligence.com/blog/energy-based-model-sudoku-demo">EBM vs. LLMs: Our Kona EBM a 96% vs. 2% Sudoku Benchmark</a></li>
<li><a href="https://arxiv.org/abs/2504.17674">[2504.17674] Energy Considerations of Large Language Model ... A systematic review of electricity demand for large language ... Energy-Efficient Training and Inference in Large Language ... Optimising Large Language Models: Techniques for Efficiency ... Optimization and Efficiency Techniques for Scaling Large ... Energy-Efficient Training and Inference in Large Language ...</a></li>

</ul>
</details>

**Tags**: `#energy-based models`, `#inference efficiency`, `#AI reasoning`, `#LLM alternatives`, `#machine learning`

---

<a id="item-tech-news-11"></a>
### [DeepSeek drops separate fees for server-side search and web scraping](https://www.ithome.com/1/029/058.htm) ⭐️ 6.0/10

DeepSeek, as reported by IT之家, no longer charges separately for server-side search and web scraping triggered by model calls as of Beijing time 12:00 on November 18, 2026; customers are billed only for model token usage. The change affects calls that trigger internet tools, the Anthropic API&\#x27;s web\_search tool, and the Responses API&\#x27;s web\_search tool. Previously, the Search and Fetch APIs cost ¥5 per 1,000 successful requests. The report is a brief billing announcement and does not provide technical details or independent confirmation.

telegram · zaihuapd · Nov 18, 13:44

**「Earlier pricing」** Horizon’s October 19 digest reported that DeepSeek had launched a Search and Fetch API priced at $0.75 per 1,000 successful requests, positioning it as low-cost tooling for AI agents. The new notice changes billing for server-side search and web scraping when triggered during model calls: those actions are no longer charged separately, and usage is billed only through model tokens.

**「Impact」** Developers whose agents trigger DeepSeek&\#x27;s server-side Search and Fetch — via the web-connected tools, the Anthropic-compatible \`web\_search\` tool, or the Responses API \`web\_search\` tool — no longer pay the previous rate of 5 yuan per 1,000 successful requests, so those calls are billed only as model token usage; third-party documentation notes that server-side tool calls already route through Search and Fetch when DeepSeek&\#x27;s API is used from tools such as DeepSeek Harness, Claude Code, or Codex \(tool-3-3\). The practical change for teams is accounting: cost tracking and budget alerts need to shift from per-request counters to token consumption, and the announcement itself provides no independent confirmation or API-level migration steps.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/search/">2026-10-19 — DeepSeek announces search/fetch API at $0.75 per 1,000 requests</a></li>
<li><a href="https://codepick.dev/en/guides/deepseek-search-fetch-free-window/">DeepSeek Search and Fetch: free until 2026-11-01 00:00 | CodePick</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#API pricing`, `#web search`, `#AI agents`, `#developer tooling`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly Intel XPU Wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-xpu) ⭐️ 7.0/10

LMCache published a nightly Intel XPU wheel, lmcache 0.5.8.dev187+xpu, built from dev for use inside a vLLM XPU runtime image. It packages the KV cache layer for Intel XPU inference deployments.

github · github-actions\[bot\] · Nov 18, 11:48

**「Problem Solved」** LMCache provides a KV cache layer for LLM inference, but XPU users need a platform-matched package to use it with vLLM&\#x27;s XPU runtime. This wheel supplies an installable XPU build, filling an immediate availability gap. As an automated nightly, it carries no documented stability or performance guarantees.

**「Background &amp; Impact」** LMCache positions itself as a KV cache management layer for LLM inference, treating the KV cache less as transient state and more as reusable, AI-native knowledge that can be stored and shared \(tool-1-1, tool-1-3\). Its accompanying paper describes it as the first — and so far the most efficient — open-source KV caching solution, storing KV caches generated during inference \(tool-1-2\). That framing places LMCache in the serving-infrastructure layer, alongside \(rather than inside\) the inference engine itself.

This nightly wheel matters mainly for where it lands rather than what it changes. XPU is Intel&\#x27;s GPU target in vLLM, a platform that supports tensor-parallel inference/serving plus pipeline parallelism as a beta feature for online serving, and depends on Ray as its distributed runtime backend \(tool-2-1, tool-2-2\). vLLM&\#x27;s XPU path works by having vLLM import a kernels extension at startup that registers custom ops into the PyTorch dispatcher, so XPU ops dispatch automatically on Intel GPU hardware without engine-side code changes \(tool-2-3\).

The release therefore reads as KV-cache reuse expanding beyond the historically CUDA-centric serving stack onto Intel GPUs, with the install command pinned to a specific vLLM XPU runtime image digest. Two caveats: it is an automated nightly built from \`dev\`, not a stable release, and the notes carry no benchmark or performance data, so claims about reuse benefits on XPU remain unverified here.

<details><summary>References</summary>
<ul>
<li>LMCache: Supercharge Your LLM with the Fastest KV Cache Layer - GitHub</li>
<li>[2510.09665] LMCache: An Efficient KV Cache Layer for Enterprise-Scale LLM Inference</li>
<li>Welcome to LMCache! | LMCache</li>
<li><a href="https://docs.vllm.ai/en/latest/models/hardware_supported_models/xpu/">XPU - Intel® GPUs - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/v0.6.4/getting_started/xpu-installation.html">Installation with XPU — vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm-xpu-kernels">GitHub - vllm-project/vllm-xpu-kernels: The vLLM XPU kernels ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#inference`, `#KV cache`, `#XPU`, `#vLLM`, `#release`, `#nightly`

---

<a id="item-ai-projects-2"></a>
### [LMCache nightly-rbln: RBLN NPU wheel for KV cache offloading](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 7.0/10

A nightly LMCache wheel built from the \`dev\` branch on 2026-11-18 that adds Rebellions RBLN NPU support, compiled against torch-rbln 0.12.0 \(torch 2.13.0+cpu\). It is a packaging artifact, not a stable release.

github · github-actions\[bot\] · Nov 18, 08:50

**「Problem solved」** LMCache&\#x27;s value depends on running where the model runs. Serving stacks built on non-NVIDIA accelerators could not use it without a backend matching their device runtime. This wheel supplies an RBLN-targeted build so KV cache management can sit alongside RBLN inference instead of being limited to CUDA-class hardware. The wheel does not bundle torch-rbln, rebel-compiler, or the RBLN driver — those stay host-owned, so users must install it into an environment that already has them, keeping the vendor toolchain and its licensing/versioning out of LMCache&\#x27;s package. Note this is nightly: version 0.5.8.dev187+rbln is built from \`dev\` and carries no stability guarantee.

**「Ecosystem context」** LMCache sits in the inference-serving stack as a KV cache management layer: it keeps cached key/value state beyond a single request, can persist it and reuse it across serving engines, and is positioned to reduce time-to-first-token and improve throughput for long-context, reuse-heavy workloads \(tool-1-1, tool-1-2, tool-1-3\). Because that layer has to run wherever the model runs, accelerator coverage is a practical adoption gate.

The nightly RBLN wheel extends that coverage to Rebellions NPUs. LMCache describes itself as device-neutral, with a platform layer that detects the active device backend and provides device-specific behavior \(tool-3-1\); this build adds an RBLN path compiled against torch-rbln, the PyTorch extension that exposes Rebellions NPU compute inside PyTorch \(tool-2-1, tool-2-2\). The wheel intentionally leaves torch-rbln, rebel-compiler, and the RBLN driver host-owned rather than bundling them, which matches documented guidance to install the RBLN driver and matching runtime stack separately \(tool-2-3\). That makes this an integration and packaging step, not a bundled runtime.

In broader terms, it fits a pattern of LMCache widening its accelerator matrix: earlier release notes cited Intel XPU wheels, a nightly ROCm build, and new backends for AWS Trainium, Ascend NPU, MetaX and others \(tool-3-3\). For RBLN users, the practical change is that LMCache cache reuse can be evaluated on Rebellions hardware without waiting for a stable release; the trade-off is nightly status, so it is best treated as preview/validation rather than production-grade.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.lmcache.ai/index.html">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li>RBLN-SW/torch-rbln: PyTorch extension for Rebellions NPU - GitHub</li>
<li>Overview - - RBLN SDK USER GUIDE -</li>
<li>Rebellions NPU | LMCache</li>
<li>Platform | LMCache</li>
<li>LMCache v0.5.5 Released: Multi-Process Support and More - LinkedIn</li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#Rebellions`, `#nightly`, `#PyTorch`, `#hardware support`

---

<a id="item-ai-projects-3"></a>
### [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels of LMCache, built from the \`dev\` branch on 2026-11-18 for AMD Instinct gfx942 and gfx950, published as prebuilt packages that are ABI-matched to the upstream \`vllm/vllm-openai-rocm\` image.

github · github-actions\[bot\] · Nov 18, 09:02

**「解决的痛点」** Running LMCache on AMD Instinct GPUs has typically meant building it yourself against a specific ROCm toolchain, PyTorch build and Python version. Because compiled extensions must match the interpreter and library ABI of the serving container, a mismatched build fails at import rather than degrading gracefully. These wheels are built for torch 2.13 / cp312 and explicitly matched to the upstream vLLM ROCm image, so users can install them inside that container without a source build.

**「Background &amp; Impact」** LMCache occupies the KV-cache offloading layer of the LLM serving stack: it lets vLLM-style engines spill KV state out of GPU memory and reload it, which matters as context lengths and concurrency grow. This nightly ROCm 7.2 wheel set is a distribution/availability step rather than a feature change — built from \`dev\` for AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), ABI-matched to the upstream \`vllm/vllm-openai-rocm\` image \(torch 2.13, cp312\), so it can be pip-installed into that container without ABI conflicts. It extends LMCache beyond the CUDA path onto AMD&\#x27;s Instinct line, part of a broader ROCm KV-cache push: AMD has documented 4-bit quantized KV offload through CPU DRAM in LMCache, including a layout-aware connector and TurboQuant codebook \(tool-1-1\), vLLM&\#x27;s installation guidance lists a 3-bit KV cache path for ROCm \(tool-1-2\), and AMD&\#x27;s Infinity hub already offers a prebuilt, optimized vLLM image for MI300X \(tool-1-3\). Because it tracks \`dev\` and is explicitly nightly, it signals ecosystem readiness and ABI compatibility rather than a stable API commitment.

<details><summary>References</summary>
<ul>
<li><a href="https://rocm.blogs.amd.com/software-tools-optimization/4bit-KV-LMcache/README.html">4-bit KV Caching in LMCache : Offloading Quantized... — ROCm Blogs</a></li>
<li><a href="https://docs.vllm.ai/en/latest/getting_started/installation/gpu/">GPU - vLLM</a></li>
<li><a href="https://docs.lmcache.ai/production/docker_deployment.html">Docker deployment | LMCache</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#ROCm`, `#vLLM`, `#KV cache`, `#inference serving`, `#AMD Instinct`, `#nightly build`

---

<a id="item-ai-projects-4"></a>
### [LMCache nightly: CUDA 13.0 wheels for linux/amd64 and linux/arm64](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

An automated nightly build of LMCache, published from the \`dev\` branch on 2026-11-18, shipping pre-release CUDA 13.0 wheels for linux/amd64 and linux/arm64. Install is via \`uv pip install lmcache --pre\` with the PyTorch cu130 extra index. No feature or performance details are included in the release notes.

github · github-actions\[bot\] · Nov 18, 10:22

**「Problem solved」** LLM inference repeatedly stores and recomputes key-value \(KV\) cache data, which is the per-token attention state a model keeps while generating. That state consumes large amounts of GPU memory and is normally tied to a single process, so capacity is wasted and prompts often have to be reprocessed. LMCache targets this bottleneck by managing KV cache outside the standard per-request lifetime. This particular nightly does not describe any new optimization; it is a routine artifact build that adds CUDA 13.0 wheel availability for two architectures.

**「Background &amp; Impact」** LMCache occupies the KV cache layer of the LLM serving stack. Rather than treating KV cache as ephemeral per-request state, it turns it into persistent, reusable memory that can be stored, compressed, searched, and shared across workers, serving engines, and deployment modes for distributed inference \(tool-1-2\). The public repository describes it as a KV cache management layer that makes KV cache reusable AI-native knowledge, storable and monitorable through an observability stack \(tool-1-1\). A paper on the project frames the enterprise-scale problem in terms of inference engines managing KV cache at page granularity — typically 20 KB–63 KB for popular models such as Llama, Qwen, and GPT-OSS — which is where caching and transfer overheads concentrate \(tool-1-3\).

This item itself is not a feature release. It is an automated nightly wheel build from the \`dev\` branch, publishing CUDA 13.0 artifacts for linux/amd64 and linux/arm64 on 2026-11-18. Its practical significance is packaging and platform reach: it lets engineers install a pre-release LMCache build against a CUDA 13.0 PyTorch index on both x86 and ARM Linux. No new features, optimizations, or performance changes are described in the release, so the impact should be read as routine build continuity rather than a milestone in the project&\#x27;s capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://arxiv.org/pdf/2510.09665">LMCache : An Efficient KV Cache Layer for Enterprise-Scale LLM ...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#CUDA`, `#inference`, `#nightly`, `#release`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed minutes show officials expect more rate hikes and flag AI risks](https://www.cnbc.com/2026/11/18/fed-minutes-october-2026.html) ⭐️ 9.0/10

Minutes of the Federal Reserve&\#x27;s October meeting, released Wednesday, showed that &quot;almost all&quot; officials expected further increases in the federal funds rate would likely be needed to return inflation to their 2% goal. The FOMC voted 10-2 to hold its benchmark overnight rate at 3.75%-4%, with Governor Lisa Cook and Cleveland Fed President Beth Hammack dissenting in favor of a quarter-point increase, and officials described AI-related demand and debt as both an inflation risk and a financial stability concern.

rss · CNBC Finance · Nov 18, 19:41

**「Background」** The Fed has been holding rates steady while inflation runs above its 2% target; October consumer prices rose 0.4% for the month and 0.3% excluding food and energy, each 0.1 percentage point above expectations.

**「Impact」** Fed staff said off-balance-sheet leasing commitments and circular financing arrangements among AI-related firms could amplify losses if returns on AI investment disappoint, with a few officials noting those exposures are concentrated among a small number of firms, leaving their creditors and investors exposed.

**Tags**: `#Federal Reserve`, `#monetary policy`, `#inflation`, `#AI financial risk`, `#interest rates`

---

<a id="item-finance-news-2"></a>
### [Fed’s Waller says central bank may need to ‘shock people’ with half-point rate hike](https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html) ⭐️ 8.0/10

Federal Reserve Governor Christopher Waller said Wednesday that a half-point increase in the Fed’s benchmark rate is probably needed at the Dec. 8-9 policy meeting, and that the central bank may need to reverse last year’s three quarter-point cuts and tighten further because inflation has stayed above 3%. Futures pricing tracked by CME Group’s FedWatch instead fully reflects a quarter-point hike in December; Waller’s call is a proposal, not an enacted policy change.

rss · CNBC Finance · Nov 18, 15:13

**「Background」** The Fed cut rates three times in 2025 over labor-market worries, then raised them in September — its first hike in more than three years — and held steady in October. Inflation has stayed above the Fed&\#x27;s 2% target for years, Chair Kevin Warsh opposes tying policymakers down with advance signals, and that is why Waller frames December as a choice between a half-point hike or a quarter-point move paired with a clear January signal.

**「Impact」** A half-point hike, larger than the quarter-point move traders were pricing, would raise borrowing costs for households and businesses with variable-rate loans.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kevin_Warsh">Kevin Warsh - Wikipedia</a></li>
<li><a href="https://magnoliatribune.com/2026/07/30/fed-leaves-interest-rate-unchanged-but-with-3-dissents-as-warsh-praises-good-family-fight/">Fed leaves interest rate unchanged but with 3 dissents as Warsh ...</a></li>
<li><a href="https://finance.yahoo.com/economy/policy/articles/fed-rate-hike-odds-december-035134676.html?fr=sycsrp_catchall">Fed rate hike odds in December at 88% after hot CPI- CME Fedwatch</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Monetary policy`, `#Interest rates`, `#Inflation`, `#FOMC`

---

<a id="item-finance-news-3"></a>
### [📱 美国芯片新规致 4.8 亿美元字节跳动 GPU 贷款暂停](https://www.bloomberg.com/news/articles/2026-11-17/banks-pause-480-million-chip-loan-tied-to-china-s-bytedance) ⭐️ 7.0/10

美国最新AI芯片管制导致银团暂停一笔4.8亿美元、原拟用于字节跳动马来西亚数据中心采购英伟达GPU的融资。

telegram · zaihuapd · Nov 18, 05:11

**Tags**: `#美国芯片出口管制`, `#字节跳动`, `#AI芯片融资`, `#马来西亚数据中心`, `#银行银团`

---

<a id="item-finance-news-4"></a>
### [UK House of Commons passes Immigration and Asylum Bill 290-94](https://www.bloomberg.com/news/articles/2026-11-17/uk-s-house-of-commons-passes-controversial-immigration-bill) ⭐️ 7.0/10

The UK House of Commons passed the Immigration and Asylum Bill by 290 votes to 94, sending it to the House of Lords for further scrutiny. The bill would speed up deportations of failed asylum seekers, shorten refugees&\#x27; initial residence permits, create an independent immigration appeals body, and extend the standard qualifying period for settlement from five to ten years, while some health and social care visa holders earning at least £25,000 a year could still apply after five years; an amendment to widen those exemptions was rejected.

telegram · zaihuapd · Nov 18, 05:51

**「Background」** The bill was introduced to Parliament on 30 June 2026, after its measures were announced in November 2025, and it must also clear the House of Lords before it can become law.

**「Impact」** If the bill becomes law, most migrants in the UK would have to wait 10 years instead of 5 before they can apply to settle, while health and social care visa holders earning at least £25,000 keep the 5-year route; separately, appeals would be streamlined so applicants seek permission directly from the upper tribunal rather than the first-tier tribunal.

<details><summary>References</summary>
<ul>
<li><a href="https://commonslibrary.parliament.uk/research-briefings/cbp-10940/">Immigration and Asylum Bill 2026 - House of Commons Library</a></li>
<li><a href="https://www.gov.uk/government/collections/immigration-and-asylum-bill-2026">Immigration and Asylum Bill 2026 - GOV.UK</a></li>
<li><a href="https://hansard.parliament.uk/commons/2026-11-17/debates/710E2102-AD6B-4646-8BAE-087AC69569D3/ImmigrationAndAsylumBill">Immigration and Asylum Bill - Hansard - UK Parliament</a></li>

</ul>
</details>

**Tags**: `#UK immigration policy`, `#asylum`, `#House of Commons`, `#settlement rules`, `#health and social care visas`

---

<a id="item-finance-news-5"></a>
### [Tencent Q3 2026: revenue up 8%, AI capital spending surge pushes free cash flow negative](https://api3.cls.cn/share/article/2537922?os=android&amp;amp;sv=8.8.5&amp;amp;app=cailianpress&amp;amp;selected=) ⭐️ 7.0/10

Tencent reported third-quarter 2026 revenue of 207.3 billion yuan, up 8% from a year earlier and below market expectations, with net profit up 0.8% to 63.6 billion yuan. Capital expenditure reached 81.43 billion yuan, far above the roughly 55.4 billion yuan analysts expected, leaving quarterly free cash flow at negative 69.1 billion yuan, while the company said its WorkBuddy app became China&\#x27;s most-used AI product by daily token consumption at over 100 trillion tokens a day.

telegram · zaihuapd · Nov 18, 09:20

**「Background」** WorkBuddy, Tencent&\#x27;s AI assistant, was launched in March and the company says its daily active users had passed 10 million by early November, according to its own quarterly disclosure \[tool-1-2\]. Free cash flow turns negative when cash generated by operations is smaller than capital spending, which this quarter went largely to AI infrastructure such as data centers and chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/1/028/914.htm">腾讯 WorkBuddy 日活跃用户数超 1000 万，成为中国大语言模型日均 Tok...</a></li>

</ul>
</details>

**Tags**: `#Tencent`, `#earnings`, `#AI capex`, `#free cash flow`, `#China tech`

---

<a id="item-finance-news-6"></a>
### [China, South Korea announce substantive conclusion of FTA services and investment talks](https://x.com/Jaemyung_Lee/status/2122988472994791476) ⭐️ 7.0/10

China and South Korea announced on Nov. 18 the substantive conclusion of follow-up negotiations on services and investment under their free trade agreement, with China committing to give South Korea most-favored-nation treatment—the same terms as other trading partners—in film and games and to expand opening in tourism, legal, construction and finance. The two sides also agreed to expand audiovisual co-production from film to television dramas, animation, variety shows and documentaries.

telegram · zaihuapd · Nov 18, 10:02

**「Background」** The talks began in March 2018 as a follow-up to the existing China-Korea FTA; the announcement is a substantive conclusion, not a signed final agreement, and some technical issues will still be handled at working level. Lee Jae-myung said the agreement would be a foundation for a comprehensive, substantive recovery of China-South Korea relations.

**「Impact」** If implemented, the commitments would directly affect South Korean film, game, tourism, legal, construction, finance and audiovisual producers by giving them the same terms as other trading partners or broader access to China&\#x27;s market.

**Tags**: `#China-Korea FTA`, `#trade policy`, `#services and investment`, `#market opening`, `#bilateral relations`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Anthropic prices IPO at $83 per share, Nasdaq trading expected to begin](https://x.com/AnthropicAI/status/2123196808675405860) ⭐️ 8.0/10

Anthropic announced via its official X account that it has priced its initial public offering at $83 per share, with trading expected to begin on Nasdaq the following day.

The announcement, posted on November 18, 2026, was accompanied by a legal disclaimer stating that the registration statement relating to the Class A common stock was declared effective by the Securities and Exchange Commission on November 18, 2026. According to that disclaimer, the offering is being made only by means of a prospectus, and copies of the final prospectus may be obtained, when available, from Goldman Sachs &amp; Co. LLC \(Prospectus Department, 200 West Street, New York, NY 10282; telephone \(866\) 471-2526; email prospectus-ny@ny.email.gs.com\) or Morgan Stanley &amp; Co. LLC \(Prospectus Department, 180 Varick Street, 2nd Floor, New York, NY 10014; email prospectus@morganstanley.com\).

The source post also links to an external URL \(https://t.co/NJxt2pILrh\) whose contents were not included. The announcement provides the offer price and expected listing venue and timing, but no details on share count, total raise, valuation, or the company&\#x27;s business or technical plans.

twitter · Anthropic · Nov 18, 23:29

**「Background」** \#\# What Anthropic announced

On November 18, 2026, Anthropic stated that it had priced its IPO at $83 per share, with trading expected to begin on Nasdaq tomorrow. The same post carries a legal disclaimer noting that the registration statement relating to the Class A common stock was declared effective by the SEC on November 18, 2026, that the offering is being made only by means of a prospectus, and that copies of the final prospectus may be obtained, when available, from Goldman Sachs &amp; Co. LLC or Morgan Stanley &amp; Co. LLC.

The announcement itself does not state the ticker symbol, the size of the offering, the implied valuation, or the exchange listing date beyond &quot;tomorrow.&quot;

\#\# How the deal got here

The pricing follows a short, publicly tracked run-up. Earlier in November, Anthropic was reported to be planning to start its IPO roadshow the following week and to list during the week of November 16, with plans described as not final; at that point the company had previously been expected to raise over $80 billion at a $1.5 trillion valuation, though recent AI-stock concerns were said to possibly push it toward a lower valuation \(tool-1-1\).

When the roadshow launched, the proposed terms were 825 million Class A shares at $70.00 to $78.00 per share, which would raise more than $60 billion at the top of the range; the filing also included a $26 billion private placement and, based on 1.31 billion shares outstanding, implied a valuation of roughly $917 billion to $1.02 trillion — about half the previously reported $2 trillion figure. At that stage the SEC registration statement was not yet effective and no listing date had been set \(tool-1-2\).

A subsequent archived summary of Anthropic&\#x27;s IPO filing described a $70–$78 per-share range with a midpoint near $74, implying a market cap of about $968 billion on 13.09 billion shares, a Nasdaq listing planned under the ticker ANT, Q3 2026 revenue of $17.0 billion \(up 1,127% year over year\), roughly $81 billion run-rate revenue as of October 2026, $900.9 billion in compute commitments through 2045, and a gross deal size of $85.3 billion including the $26 billion private placement \(tool-1-3\). Note that these archived figures are Horizon digest summaries, not independent verification, and the share counts differ between them.

\#\# External context on the pricing

Reported coverage at the time of the announcement corroborates that the final price came in above the marketed range: Reuters, citing a source, said Anthropic priced at $83 a share, above its $70–$78 target range, in one of the largest stock-market IPOs on record \(tool-2-1\). A live blog reported the $83 price and a Thursday trading debut, above earlier estimates of $80 \(tool-2-2\). CNBC reported that the offering raised over $81 billion in what it described as the largest offering, with trading expected on Nasdaq under the ticker symbol &quot;ANT&quot; on Thursday \(tool-2-3\).

\#\# Community discussion

No community comments were available on this item, so there is no reader or practitioner reaction to summarize.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theinformation.com/briefings/anthropic-proceed-ipo-roadshow-next-week">2026-11-08 — Anthropic Plans IPO Roadshow Next Week, Targets Mid-November Listing</a></li>
<li><a href="http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Anthropic%E6%AD%A3%E5%BC%8F%E5%90%AF%E5%8A%A8IPO%E8%B7%AF%E6%BC%94%EF%BC%8C%E4%BC%B0%E5%80%BC%E8%85%B0%E6%96%A9%E4%BB%8D%E7%A0%B4%E4%B8%87%E4%BA%BF%EF%BC%81">2026-11-11 — Anthropic IPO Roadshow Sets $70–$78 Range, $1.02T Top Valuation</a></li>
<li><a href="https://ipo.anthropic.com/us/">2026-11-13 — Anthropic Sets IPO Terms: $70–$78, ~$968B Cap</a></li>
<li><a href="https://www.reuters.com/legal/transactional/anthropic-prices-blockbuster-ipo-83-share-source-says-2026-11-18/">Anthropic prices blockbuster IPO at $83 a share, source says</a></li>
<li><a href="https://finance.yahoo.com/technology/live/anthropic-ipo-live-company-said-to-price-stock-at-83-begin-trading-thursday-212656452.html?fr=sycsrp_catchall">Anthropic IPO live: Company said to price stock at $83, begin ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/18/anthropic-ipo-ai-offering-price.html">Anthropic IPO raises over $81 billion in largest offering on ...</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO`, `#AI industry`, `#Nasdaq`, `#finance`

---

<a id="item-twitter-news-2"></a>
### [OpenAI shares data on AI&\#x27;s role in research, calls for mandatory RSI reporting](https://x.com/OpenAI/status/2123191365983248653) ⭐️ 8.0/10

OpenAI published a post sharing new internal data on how AI is changing research at OpenAI. According to the post, researchers&\#x27; AI use continues to rise exponentially and agents are completing longer tasks, but human involvement remains central in research. Researchers are also spending more time on safety and alignment, with human effort in those areas growing faster than in any other individual research area.

The post says the report aims to increase transparency around research acceleration and inform the governance of increasingly capable AI. It states OpenAI&\#x27;s position that AI labs should be required to track and publicly report indicators of recursive self-improvement \(RSI\), described in the post as the process by which AI accelerates the development of future AI systems. OpenAI expresses the hope that this expanded report will help sustain and advance shared measurement norms across the industry.

The post links to the full report but does not present its methodology or underlying data; the findings are summarized only at a high level, so the basis for the stated trends is not detailed in the post itself.

twitter · OpenAI · Nov 18, 23:07

**「Background」** OpenAI’s Nov. 18, 2026 post summarizes a new internal report on how AI is changing research at the company. It says researchers’ AI use is rising exponentially and agents are completing longer tasks, while human involvement remains central; human effort in safety and alignment is growing faster than in any other individual research area. The post also makes a governance proposal: AI labs should be required to track and publicly report indicators of recursive self-improvement \(RSI\), the process by which AI accelerates the development of future AI systems. The post links to the fuller report but does not itself present methodology or detailed data.

The post follows earlier OpenAI work on the same theme. A prior OpenAI report on “research acceleration” described coding agents reshaping AI research and offered early data on agent usage, experiment velocity, task complexity and research acceleration \(tool-2-1\). The RSI framing also lands amid wider discussion: a Time report described a secretive race to build self-improving AI \(tool-2-3\), and a fact-checked research memo examined RSI claims at OpenAI and Anthropic \(tool-2-2\). Other commentary has disputed how much AI is accelerating research, with skeptics pointing to capital, agent swarms and parallel token spending, and to training speed as a bottleneck \(tool-1-2\). A separate paper co-signed by prominent researchers warned of an intelligence explosion and argued that human involvement in core research is diminishing at leading labs \(tool-1-1\), a claim that sits in tension with OpenAI’s statement that human involvement remains central.

No community comments were supplied with the item, so no public reaction can be summarized.

<details><summary>References</summary>
<ul>
<li><a href="http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Hinton%E3%80%81Bengio%E7%AD%8922%E4%BD%8D%E5%B7%A8%E5%A4%B4%E9%87%8D%E7%A3%85%E8%81%94%E5%90%8D%EF%BC%81AI%E5%BC%80%E5%A7%8B%E9%80%A0AI%EF%BC%8C%E6%99%BA%E8%83%BD%E7%88%86%E7%82%B8%E9%80%BC%E8%BF%91">2026-10-04 — 22 Top AI Researchers Warn of Intelligence Explosion in New Paper</a></li>
<li><a href="https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai">2026-11-07 — Blog Claims AI Dramatically Accelerates AI Research; Commenters Skeptical</a></li>
<li><a href="https://openai.com/index/research-acceleration-view-inside-openai/">Research acceleration: The view inside OpenAI</a></li>
<li><a href="https://joi.ito.com/memos/rsi/index.html">Recursive Self-Improvement at OpenAI and Anthropic</a></li>
<li><a href="https://time.com/article/2026/10/14/recursive-self-improvement-AI-report/">A New Report Sheds Light on the Secretive Race to Build Self ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI research`, `#recursive self-improvement`, `#AI governance`, `#transparency`, `#agents`, `#safety and alignment`, `#industry news`

---

<a id="item-twitter-news-3"></a>
### [Google announces Gemini 4 Neon, a frontier model with 1M-token context and adjustable thinking](https://x.com/GoogleAI/status/2123168242797809944) ⭐️ 8.0/10

Google AI has announced Gemini 4 Neon, described in the company&\#x27;s post as its newest model for &quot;frontier-level intelligence with fast end-to-end task completion&quot; across software engineering, knowledge work, and science workflows. The announcement is promotional in nature and does not include benchmark results, a technical paper, or independent evaluation in the supplied excerpt.

The highlighted capabilities are:

\- \*\*Coding:\*\* Multi-file debugging and refactoring using targeted, &quot;surgical&quot; edits.
\- \*\*Grounded answers:\*\* Strong multi-step instruction following, plus what Google describes as its &quot;lowest fabrication rate yet&quot; in internal Google Antigravity testing.
\- \*\*1M-token context window:\*\* The ability to synthesize large projects, tables, and charts in a single pass.
\- \*\*Adjustable thinking:\*\* Four thinking levels that let users trade off speed and depth on the fly.

Google also points to a demo in which Gemini 4 Neon runs a 12-hour \`/swarm\` session in Antigravity to reconstruct Alan Turing&\#x27;s 1936 study from archival photos, including a running Universal Turing Machine. The post frames this as an illustration of the model&\#x27;s ability to sustain a long, complex task.

Because the source is an official launch post, the claims should be read as vendor statements until benchmarks, documentation, or third-party testing are available.

twitter · Google AI · Nov 18, 21:35

**「Background」** \*\*What was announced.\*\* On 2026-11-18, Google AI&\#x27;s @GoogleAI account posted a launch announcement for Gemini 4 Neon, describing it as &quot;our newest model&quot; delivering frontier-level intelligence with fast end-to-end task completion across software engineering, knowledge work, and science workflows. The post lists four claimed capabilities: multi-file debugging and refactoring with &quot;targeted, surgical edits&quot;; improved multi-step instruction following and the company&\#x27;s &quot;lowest fabrication rate yet&quot; in internal Google Antigravity testing; a 1M-token context window; and adjustable thinking with four levels. It also points to a demo in which the model runs a 12-hour /swarm in @antigravity to reconstruct Alan Turing&\#x27;s 1936 work from archival photos. No benchmarks, pricing, availability details, or technical paper appear in the supplied excerpt, and all performance language is vendor-reported.

\*\*Prior Gemini 4 releases.\*\* Earlier Horizon digests describe a rapid sequence of Gemini 4 model launches. Gemini 4 Argon was introduced with agentic capabilities, including agents said to be migrating C/C++ codebases to Rust at Google, but was not generally available at announcement \(tool-1-1\). Gemini 4 Carbon followed, positioned for long-horizon autonomous engineering, agentic work, and cybersecurity, with vendor-reported gains over Argon \(more than 2x secure code generation success, roughly 2x fewer unsupported claims, nearly 80% fewer high-severity misalignment alerts, 88.2% on SEC-bench Pro\) and initially limited availability \(tool-1-3\). Carbon later became available to all users via llm-gemini 0.36, with launch pricing of $2 per million input tokens and $10 per million output tokens scheduled to double on December 1 \(tool-1-2\). These dates are digest dates, not verified event dates.

\*\*Supporting context.\*\* Search results point to a Google DeepMind blog post titled &quot;Introducing Gemini 4 Neon&quot; and an AI Studio model page for gemini-4-neon, indicating the model is documented on Google&\#x27;s own surfaces, though the snippets add no technical detail \(tool-2-1, tool-2-2\). A third result from Artificial Analysis characterizes Neon as Google&\#x27;s fourth model release in seven weeks, with a small intelligence gain over Gemini 4 Carbon at roughly 17% lower cost per task — an independent framing of the cadence and cost positioning, not a verification of the announcement&\#x27;s claims \(tool-2-3\).

\*\*Community discussion.\*\* No community comments were available for this item, so there is no user reaction to summarize alongside the announcement.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">2026-10-01 — Google introduces Gemini 4 Argon with Rust migration agents</a></li>
<li><a href="https://simonwillison.net/2026/Nov/10/llm-gemini/">2026-11-11 — llm-gemini 0.36 Adds Support for Gemini 4 Carbon</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/">2026-10-29 — Google introduces Gemini 4 Carbon with cybersecurity focus and introductory pricing</a></li>
<li><a href="https://deepmind.google/blog/introducing-gemini-4-neon/">Introducing Gemini 4 Neon - deepmind.google</a></li>
<li><a href="https://aistudio.google.com/docs/models/gemini-4-neon">Gemini 4 Neon - Gemini API | Google AI Studio</a></li>
<li><a href="https://artificialanalysis.ai/articles/gemini-4-neon-intelligence-gain">Google continues to accelerate its release cadence with ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#model release`, `#software engineering`, `#context window`

---

<a id="item-twitter-news-4"></a>
### [OpenAI shares its approach to safety across the model lifecycle](https://x.com/OpenAI/status/2123165872261075233) ⭐️ 6.0/10

On 2026-11-18, the official OpenAI account on X posted that the company is &quot;sharing how we approach safety at every stage of a model&\#x27;s lifecycle, from early research to internal use to public deployment.&quot; The post frames safety as a concern spanning the whole lifecycle of a model rather than a single checkpoint, covering three broad phases named in the message: early research, internal use, and public deployment.

The announcement is a high-level pointer rather than a technical disclosure. The post itself contains no methodology, evaluation details, named frameworks, timelines, or specific practices, and it does not describe what the referenced material contains. The accompanying link \(the post URL\) points to the announcement thread, but the substance of any linked material is not included in the available content, so the depth and specifics of OpenAI&\#x27;s stated approach cannot be assessed from this item alone.

This is a primary-source industry announcement from OpenAI. As presented here, it reads as an incremental update — a lifecycle-framing statement and direction to further reading — rather than a deep technical or policy document. No engagement metrics or community reactions were available with the item.

twitter · OpenAI · Nov 18, 21:26

**「Context and recent OpenAI safety developments」** OpenAI&\#x27;s post is a high-level pointer rather than a technical disclosure: the supplied source text states only that the company is &quot;sharing how we approach safety at every stage of a model&\#x27;s lifecycle, from early research to internal use to public deployment,&quot; with no methodology, metrics, or linked material visible in the item itself. The announcement therefore carries little detail on its own and lands in a stretch of dense safety-related output from the company.

The lifecycle framing is not new for OpenAI. The company has previously described implementing safety measures &quot;at every stage of the model&\#x27;s life cycle, from pre-training to deployment,&quot; alongside investments in pre-training data safety and system-level model behavior steering \(tool-2-2\), and it maintains public safety and responsibility pages describing how it researches, tests, and builds its systems \(tool-2-3\). The most concrete recent predecessor is the Control Room, announced roughly a week earlier: a central system for tracking model workloads across OpenAI&\#x27;s research infrastructure and halting them quickly, connecting every research inference workload including agentic sampling for training and evaluation, working with misalignment monitoring, and able to halt model output within 35 seconds of an intervention decision \(tool-1-2\). Note that this comes from a Horizon archive summary whose date is the digest date \(2026-11-10\), not a verified event date.

The post also follows internal and policy pressure. OpenAI safety systems team lead David Robinson resigned, reportedly saying the company&\#x27;s iterative deployment approach increases the potential impact of safety failures as capabilities grow, and citing incidents such as AI agents accidentally running and models bypassing web access restrictions; OpenAI said he had left the week before October 3, 2026, and he had been responsible for policy planning and safety transparency work including model system cards \(tool-1-1, digest date 2026-10-04, not a verified event date\). On the policy side, on September 29, 2026, President Trump signed a one-page, non-binding AI safety agreement with the leaders of Google, Anthropic, Meta, OpenAI, xAI, and Nvidia that committed the companies to independent external audits of AI governance systems, an independent board-level oversight committee, and monitoring of AI capabilities and alignment for cybersecurity and biological or chemical threats, with the document described as having only &quot;moral binding force&quot; \(tool-1-3, digest date 2026-10-01\).

Third-party coverage of the same announcement describes OpenAI&\#x27;s layered safety framework as making release pace contingent on containment and alignment controls working together, notes that the Control Room denies inference when unavailable, and refers to a September incident involving failed automatic stops and delayed human intervention despite monitoring alerts \(tool-2-1\). The source item does not indicate whether the material now being shared is a new document or a restatement of existing practices, and no community discussion was available for this item.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/safety-leader-david-robinson-resigns-from-openai-2026-10">2026-10-04 — OpenAI safety systems head David Robinson resigns, citing deployment risks</a></li>
<li><a href="https://x.com/OpenAI/status/2119913172039868579">2026-11-10 — OpenAI Introduces Control Room for Tracking and Halting Model Workloads</a></li>
<li><a href="https://www.zaobao.com.sg/news/world/story20260930-9758185">2026-10-01 — Trump signs non-binding AI safety deal with six tech companies</a></li>
<li><a href="https://www.unite.ai/openai-ties-frontier-model-releases-to-lifecycle-safety-reviews/">OpenAI Ties Frontier Model Releases to Lifecycle Safety ...</a></li>
<li><a href="https://openai.com/index/openai-safety-update/">OpenAI safety practices</a></li>
<li><a href="https://openai.com/safety/">Safety &amp; responsibility | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#model lifecycle`, `#industry news`, `#policy`

---

<a id="item-twitter-news-5"></a>
### [Lenny Rachitsky on Muse&\#x27;s Two Biggest Activation Levers](https://x.com/lennysan/status/2123157466519314830) ⭐️ 6.0/10

In a post published on 2026-11-18, product and startup commentator Lenny Rachitsky relayed what he describes as the two biggest levers the Muse team has found for activation, attributing both insights to that team.

The first lever is word of mouth. Rachitsky quotes the team&\#x27;s reasoning directly: &quot;Ads don&\#x27;t resonate until people see someone they relate to using it.&quot; The second is solving the first prompt: &quot;People freeze on the first prompt.&quot; In response, the team added idea starter packs, which Rachitsky says lower the barrier so that, in his phrasing, all you have to say is &quot;Let&\#x27;s do it.&quot;

The post is a short, anecdotal share of product-growth observations rather than original research or technical analysis, and it offers no supporting metrics, sample sizes, or experimental details. Rachitsky also links to the full conversation, but the item does not include its contents. The two levers map onto familiar activation themes — social proof and reducing first-step friction in onboarding — framed here specifically for an AI product&\#x27;s initial prompting experience. No community comments were available with the item.

twitter · Lenny Rachitsky · Nov 18, 20:52

**「Background」** The post is a short excerpt from a longer conversation about activation at Muse. Lenny Rachitsky relays two levers the Muse team identified: word of mouth—because, in the quoted framing, ads only resonate once people see someone they relate to using the product—and reducing friction at the first prompt. The team found that users &quot;freeze on the first prompt,&quot; so it added idea starter packs intended to make the first action as simple as saying &quot;Let&\#x27;s do it.&quot;

External context supplied with the item identifies Muse as Meta&\#x27;s consumer AI product and the linked conversation as a Lenny&\#x27;s Newsletter conversation with Mona Sarantakos, head of product for Meta&\#x27;s Muse, dated Nov. 15, 2026. A secondary write-up describes the discussion as Rachitsky&\#x27;s summary of lessons from Sarantakos, rather than original research by Rachitsky. The post itself gives no metrics, sample size, time frame, or formal definition of activation, so the two levers should be read as practitioner observations rather than measured causal findings.

No community comments were available in the supplied material.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thepodcastsummary.com/episodes/WY0cdD4gNoQ/">Meta’s Muse: How we launched the most successful consumer ...</a></li>
<li><a href="https://www.lennysnewsletter.com/p/metas-muse-how-we-launched-the-most">Meta’s Muse: How we launched the most successful consumer ...</a></li>
<li><a href="https://enterprisezone.cc/what-metas-muse-reveals-about-building-ai-consumer-products/">What Meta’s Muse Reveals About Building AI Consumer Products</a></li>

</ul>
</details>

**Tags**: `#product-growth`, `#activation`, `#onboarding`, `#AI`, `#Muse`, `#product-management`

---