# Horizon Daily - 2026-09-30

> From 54 items, 20 important content pieces were selected

---

**Technology News**
1. [OpenAI DevDay 2026 Launches Dots Agent, GPT-6.1 Sol, and 20+ Updates](#item-tech-news-1) ⭐️ 9.0/10
2. [Anthropic finds GLM-5.3 and Claude Mythos Preview can hijack control flow](#item-tech-news-2) ⭐️ 8.0/10
3. [PostgreSQL expert Freund discusses Linux kernel improvements](#item-tech-news-3) ⭐️ 8.0/10
4. [Language Models for Text Classification: From Bag-of-Words to Jev](#item-tech-news-4) ⭐️ 8.0/10
5. [CoWindow and MassAlloc Attention reduce redundant compute in long-context transformers](#item-tech-news-5) ⭐️ 8.0/10
6. [A Privacy Analysis of Web and Mobile Conversational AI Agents \[pdf\]](#item-tech-news-6) ⭐️ 7.0/10
7. [Oracle Cites Force Majeure on Stargate&\#x27;s Delayed New Mexico Data Center](#item-tech-news-7) ⭐️ 7.0/10
8. [China&\#x27;s generative AI users top 700 million, CNNIC report says](#item-tech-news-8) ⭐️ 7.0/10
9. [Cloudflare launches cf CLI with 3,000+ API operations for humans and AI agents](#item-tech-news-9) ⭐️ 7.0/10
10. [Google fixes Firebase server bug that crashed iOS apps](#item-tech-news-10) ⭐️ 7.0/10
11. [PS5 Relapse Exploit Targets WebKit JavaScriptCore for Jailbreak](#item-tech-news-11) ⭐️ 6.0/10
12. [Tcl/Tk 9.1 released, continues legacy of simplicity](#item-tech-news-12) ⭐️ 6.0/10
13. [Rust GPU as a standard compiler target: vision and prototype](#item-tech-news-13) ⭐️ 6.0/10
14. [AI-Has-Taste Finds Confirmed Counterexample; Repo Tops 453 Manuscripts](#item-tech-news-14) ⭐️ 6.0/10
15. [Free open-source book: &\#x27;How to Make Your Model Fast&\#x27; teaches ML performance engineering](#item-tech-news-15) ⭐️ 6.0/10

**Financial News**
1. [Trump&\#x27;s municipal bond portfolio grows to as much as $1 billion](#item-finance-news-1) ⭐️ 8.0/10
2. [Goldman Sachs board reportedly weighs replacing CEO David Solomon](#item-finance-news-2) ⭐️ 7.0/10
3. [Fair Isaac drops 18% after FHFA mortgage-pricing change; AMD, AstraZeneca and CarMax lead premarket moves](#item-finance-news-3) ⭐️ 7.0/10
4. [China Tightens IPO Criteria for Humanoid Robot Startups](#item-finance-news-4) ⭐️ 7.0/10
5. [China to Subsidize New First-Home Mortgages From Oct 1](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI DevDay 2026 Launches Dots Agent, GPT-6.1 Sol, and 20+ Updates](https://openai.com/zh-Hant/index/devday-2026-recap/) ⭐️ 9.0/10

OpenAI DevDay 2026 shipped over 20 updates, including the always-on Dots agent that learns user habits to handle complex tasks autonomously; GPT-6.1 Sol, a coding- and computer-use-focused model offering near-Astra intelligence at one-fifth the price; Astra Ultrafast with up to 8× speed gains \(6× on the API\); Codex with voice control and automatic error fixing on the cloud; the Agents API with native computer control and AWS Bedrock hosting; the Decisions API for lightweight real-time decision-making using Luna; a “Sign in with ChatGPT” account system that lets users allocate subscription credits to third-party tools like Devin and Notion; and a new Pro 500 tier with 25 times the compute of Plus and exclusive access to Astra Ultrafast.

telegram · zaihuapd · Sep 29, 17:52

**「Background」** Before the DevDay announcements, TestingCatalog reported that OpenAI planned to expand its Ultrafast API beyond invite-only customers around the September 29 event, a mode previewed with GPT-5.6 Sol at up to 750 tokens per second and 14x faster inference than the Standard tier. The new DevDay recap presents Astra Ultrafast as an evolved form of that fast-inference option, claiming up to an 8x speed increase \(6x for the API\). Those earlier reports were pre-announcement and had not been officially confirmed by OpenAI at the time.

**「Impact」** The fivefold cost reduction of GPT-6.1 Sol and the 25× compute allocation of the Pro 500 tier allow development teams to run substantially more code-generation and agent tasks per dollar compared to prior OpenAI offerings, lowering the barrier for continuous AI-assisted workflows.

**「Community Discussion」** Some developers argue that even the new pricing cannot compete with DeepSeek’s cost-per-token, with one user noting they never hit quotas on DeepSeek and find intelligence differences negligible. Others criticize GPT-6 Sol as a regression from Sol 5.6, having switched to Anthropic’s Opus 5.5, and express skepticism that GPT-6.1 Sol will resolve those issues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/">2026-09-27 — OpenAI reportedly expands Ultrafast API access around DevDay</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-6.1`, `#Dots agent`, `#AI agent`, `#DevDay`

---

<a id="item-tech-news-2"></a>
### [Anthropic finds GLM-5.3 and Claude Mythos Preview can hijack control flow](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 8.0/10

Anthropic&\#x27;s Frontier Red Team reports that GLM-5.3 and Claude Mythos Preview achieved full control flow hijacks in 4% and 6% of binary exploitation trials, respectively, a capability earlier models like Claude Opus 4.6 and GLM-5.2 failed to demonstrate. Anthropic also says GLM-5.3 can build end-to-end attacks \(50 of 410 ExploitBench attempts, close to Claude Mythos Preview&\#x27;s 56\) and that its safeguards can be bypassed in 64-100% of simulations.

rss · Simon Willison · Sep 29, 22:20

**「Background」** The internal Binary Exploitation benchmark tests whether models can turn memory-safety vulnerabilities into control of program execution, rather than just produce plausible exploit code. This frontier red-team evaluation previously produced zero successes for the prior Claude Opus 4.6 and GLM-5.2 generation, which is why even single-digit percentages are treated as a capability threshold.

**「Impact」** Because GLM-5.3 is open weight, users can modify it to weaken safety refusals, and Anthropic reports that simple methods bypassed its guardrails in simulations. Security teams should treat autonomous exploit-generation capability as present even at low success rates, rather than assuming the limitations of earlier models still hold.

**Tags**: `#anthropic`, `#AI security`, `#cyber capabilities`, `#LLM capabilities`, `#binary exploitation`

---

<a id="item-tech-news-3"></a>
### [PostgreSQL expert Freund discusses Linux kernel improvements](https://lwn.net/Articles/1096827/) ⭐️ 8.0/10

At Kernel Recipes 2026, PostgreSQL core contributor Andres Freund presented his experience working with, or around, Linux kernel features and behaviors that affect PostgreSQL performance, suggested ways the kernel could better support database applications, and touched on recent developments in PostgreSQL. The LWN report describes a conference talk rather than a shipped kernel or PostgreSQL change, so no specific versions, benchmarks, or concrete outcomes are available from the source material.

rss · LWN.net · Sep 29, 15:42

**「Background」** Kernel Recipes is an annual conference where Linux kernel developers and upstream users discuss low-level kernel behavior and how it interacts with real workloads. Andres Freund is a long-time PostgreSQL contributor whose performance work has often required working with or around specific Linux kernel features, and his 2026 talk reflects that ongoing relationship.

**「Impact」** Kernel and database developers can use the talk as a starting point for identifying kernel behaviors that materially affect PostgreSQL workloads, and may want to follow Freund&\#x27;s proposals for potential optimization work, since the source does not yet document any landed patches or measured improvements.

**Tags**: `#PostgreSQL`, `#Linux kernel`, `#database performance`, `#kernel development`, `#systems engineering`

---

<a id="item-tech-news-4"></a>
### [Language Models for Text Classification: From Bag-of-Words to Jev](https://magazine.sebastianraschka.com/p/classifier-history-and-jev) ⭐️ 8.0/10

Sebastian Raschka published a visual guide that traces text classification from bag-of-words to the JEV method, with hands-on experiments comparing RNNs, CNNs, Transformers, and calibration techniques on accuracy and efficiency. The guide provides practical insights for selecting the right architecture.

rss · Ahead of AI · Sep 29, 10:50

**「Background」** Text classification methods have evolved from simple bag-of-words representations through specialized neural architectures such as RNNs, CNNs, and Transformers. The recently introduced JEV model represents a shift toward general-purpose classifiers that can handle diverse tasks without task-specific training \(tool-1-2\). This article surveys that progression with visual guides and hands-on accuracy and efficiency experiments, positioning JEV within the broader history of language models for classification.

**「Impact」** Practitioners can use the guide&\#x27;s experimental comparisons to evaluate accuracy and efficiency trade-offs across different text classification architectures, directly informing their model choice for specific applications.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/classifier-history-and-jev">Language Models for Text Classification: From Bag-of-Words to Jev</a></li>
<li><a href="https://sebastianraschka.com/blog/2026/jev-classification-generalization.html">Jev and Generalization | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**Tags**: `#text classification`, `#language models`, `#machine learning`, `#transformers`, `#tutorial`

---

<a id="item-tech-news-5"></a>
### [CoWindow and MassAlloc Attention reduce redundant compute in long-context transformers](https://www.reddit.com/r/MachineLearning/comments/1wt1gbk/cowindow_and_massalloc_attention_collective/) ⭐️ 8.0/10

Two new attention mechanisms, CoWindow Attention \(CoWA\) and MassAlloc Attention \(MALA\), aim to reduce redundant computation in long-context transformers. CoWA distributes distant context across KV heads using complementary windows, achieving sparse head-wise attention while the union of heads covers the full causal history without a learned router. MALA retains full causal query-key scoring but uses attention&\#x27;s softmax statistics to skip low-contribution post-score computation for tiles, using a common tolerance for both training and inference. On 8 H100 GPUs with TP=8 at 128K tokens, attention-operator speedups relative to full attention are: CoWA forward 7.4×, backward 8.6×, decode 3.0×; MALA forward 2.2×, backward 3.0×, decode 1.6×. At 14B parameters with 32K context, total training FLOPs decreased by 28.5% for CoWA and 23.1% for MALA while maintaining comparable model capabilities on reported evaluations. The authors note that neither method guarantees universal lossless equivalence to dense attention.

reddit · r/MachineLearning · /u/BitExternal4608 · Sep 29, 05:16

**「Background」** Standard transformer attention computes pairwise interactions across all positions, leading to quadratic cost in sequence length. This becomes a major bottleneck for long-context models \(e.g., 128K tokens\). Prior work has proposed sparse, sliding-window, or learned routing patterns to reduce computation, but often introduces overhead or sacrifices training fidelity. The presented CoWA and MALA target complementary sources of redundancy without requiring a learned indexer.

**「Impact」** Researchers and engineers working on long-context transformers can directly apply CoWA or MALA to reduce compute during both training and inference, potentially enabling longer contexts or larger batch sizes on existing hardware. However, because collective coverage does not imply identical head-wise outputs and MALA still pays for full QK scoring, practitioners should validate model quality and downstream task performance for their specific use cases before adoption.

**Tags**: `#attention mechanisms`, `#long-context`, `#efficiency`, `#transformer`, `#sparse attention`

---

<a id="item-tech-news-6"></a>
### [A Privacy Analysis of Web and Mobile Conversational AI Agents \[pdf\]](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A privacy analysis of conversational AI agents highlights emerging data-exposure and tracking risks across web and mobile chat platforms.

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**Tags**: `#privacy`, `#conversational AI`, `#security`, `#tracking`, `#AI agents`

---

<a id="item-tech-news-7"></a>
### [Oracle Cites Force Majeure on Stargate&\#x27;s Delayed New Mexico Data Center](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

Oracle has issued a force majeure notice for Project Jupiter, Stargate&\#x27;s data center in New Mexico, after environmental and power approvals for its 2.45GW microgrid stalled and threatened the expected 2028 start date. The notice would let Oracle defer some project payments if the delay stems from external factors. The financing market has reacted by trading the project&\#x27;s $18bn syndicated loan at a discount, as most Stargate sites remain in construction, approval, or energy-work phases and only a few, such as the Abilene campus in Texas, are operational; Texas has also paused new data-center approvals.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** Stargate is a joint venture among Oracle, SoftBank, and OpenAI to build massive AI data centers; Project Jupiter in New Mexico is one of its largest campuses with a planned 2.45 GW capacity. Force majeure clauses allow a party to suspend obligations when events beyond its control—such as regulatory delays—prevent performance. Oracle&\#x27;s notice aims to delay rent payments if power approvals and a gas pipeline are not completed in time for a 2028 operational target.

**「Impact」** Developers and lenders tied to Stargate now face concrete financial exposure: the $18bn syndicated loan is trading at a discount, and Oracle&\#x27;s force majeure notice means project entities could absorb deferred payment risk if the New Mexico power approvals continue to slip. The 2028 timeline is therefore a direct factor in loan performance and construction financing, not just a scheduling concern.

<details><summary>References</summary>
<ul>
<li><a href="https://app.dealroom.co/news/note/oracle-files-force-majeure-on-2-45gw-new-mexico-stargate-data-center">Oracle files force majeure on 2.45GW New Mexico Stargate data center | Dealroom.co</a></li>
<li><a href="https://coloprice.com/guides/oracle-force-majeure-project-jupiter/">Oracle Invokes Force Majeure on Stargate&#x27;s Project Jupiter as…</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#Oracle`, `#energy grid`, `#Stargate`

---

<a id="item-tech-news-8"></a>
### [China&\#x27;s generative AI users top 700 million, CNNIC report says](https://ysxw.cctv.cn/article.html?toc_style_id=feeds_default&amp;amp;item_id=187569887152346976&amp;amp;channelId=1119) ⭐️ 7.0/10

On September 29, China&\#x27;s CNNIC published the 2026 Generative AI Application Development Report, finding that the country&\#x27;s generative AI users surpassed 700 million in the first half of 2026, an adoption rate above 50%. Intelligent Q&amp;A was the most common use case, cited by 76.0% of users, while usage of AI general assistants and AI efficiency office tools both grew more than 100% year over year. The report also estimated China&\#x27;s intelligent computing capacity at 2185 EFLOPS, up 177% year over year.

telegram · zaihuapd · Sep 29, 06:39

**「Background」** China&\#x27;s rapid growth in generative AI adoption follows an equally fast expansion of domestic AI computing capacity. Horizon&\#x27;s September 26 digest reported that industry analysis firm SemiAnalysis mapped over 1,000 AI datacenter facilities in China, much of it originally built for retail workloads and later repurposed for AI compute. That earlier supply-side analysis provides context for the CNNIC report&\#x27;s 177% year-over-year jump in intelligent computing power.

**「Impact」** Product teams targeting Chinese consumers should treat intelligent Q&amp;A as a baseline generative AI capability rather than an optional feature, since the report attributes it to over three-quarters of the user base. The reported growth in AI assistant and office tool usage also signals that these workflow-oriented applications are becoming primary adoption drivers.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom">2026-09-26 — SemiAnalysis Maps China’s AI Datacenter Boom with 1,000+ Facilities</a></li>

</ul>
</details>

**Tags**: `#generative AI`, `#China`, `#AI adoption`, `#user statistics`, `#intelligent computing`

---

<a id="item-tech-news-9"></a>
### [Cloudflare launches cf CLI with 3,000+ API operations for humans and AI agents](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare has released an open beta of cf, a new CLI tool that exposes over 3,000 API operations—up from the roughly 280 covered by the existing Wrangler CLI. Built automatically from Cloudflare’s API schema, cf outputs JSON by default and includes command search and guidance features designed to help both human developers and AI agents discover, execute, and interpret API calls. Cloudflare demonstrates using the same tool to create Workers, monitor services, configure Access and WAF, and purchase domains. The beta may have rough edges; it is a broader coverage tool, not a replacement for Wrangler in all scenarios.

telegram · zaihuapd · Sep 29, 13:46

**「Background」** Cloudflare’s existing Wrangler CLI is focused on managing Cloudflare Workers and covers roughly 280 API operations. The new cf CLI is generated directly from Cloudflare’s full API schema, giving it substantially broader coverage across the entire platform without requiring per-endpoint maintenance.

**「Impact」** Developers and AI agent builders can now automate and script virtually any Cloudflare operation from a single CLI, reducing the need to switch between tools or write custom API wrappers. Because cf is still in open beta, users should expect API surface changes and potential instability before a stable release.

**Tags**: `#Cloudflare`, `#CLI`, `#AI Agents`, `#DevTools`, `#API`

---

<a id="item-tech-news-10"></a>
### [Google fixes Firebase server bug that crashed iOS apps](https://github.com/firebase/firebase-ios-sdk/issues/16728) ⭐️ 7.0/10

Google has confirmed and fixed a server-side bug in Google Analytics for Firebase that returned malformed data and caused many iOS apps using the component to crash on launch. The issue began on September 28, 2026 at 17:41 PDT, and the fix finished rolling out at 19:52 PDT the same day. No SDK or app update is required; due to caching, some apps may continue crashing for up to about four hours after the fix before residual effects clear on their own.

telegram · zaihuapd · Sep 29, 16:29

**「Background」** Google Analytics for Firebase is an analytics service that iOS apps embed via the Firebase SDK, which receives data from Google&\#x27;s servers during app startup. Because the crash-causing bug was in Firebase&\#x27;s backend rather than in the SDK, correcting it required no SDK or app update from developers—only Google&\#x27;s server-side fix, with cached bad data clearing on its own.

**「Impact」** iOS developers using Google Analytics for Firebase do not need to release an emergency app update, but should expect lingering launch crashes to resolve automatically within roughly four hours as cached bad data expires.

**Tags**: `#Firebase`, `#iOS`, `#crash`, `#Google Analytics`, `#bug fix`

---

<a id="item-tech-news-11"></a>
### [PS5 Relapse Exploit Targets WebKit JavaScriptCore for Jailbreak](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 6.0/10

A GitHub-hosted exploit named Relapse, shared on Hacker News, targets a WebKit JavaScriptCore vulnerability on the PS5, apparently for jailbreak purposes. Commenters note that key open questions are whether the console&\#x27;s WebKit runs JavaScriptCore with JIT enabled and whether Sony will narrow the attack surface by disabling JIT, but the supplied material provides no firmware compatibility details or evidence of a working jailbreak.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「Background」** The Relapse project is described as an exploit chain for PlayStation 5 firmware versions 7.00 through 13.60, using a WebKit vulnerability as the entry point and a separate kernel exploit afterward. Its published stability notes warn that the WebKit stage may need several page reloads and that a kernel attempt can hang or panic the console, requiring a reboot before retrying.

**「Impact」** PS5 owners should treat the exploit as unverified and avoid running its code until firmware compatibility and a working jailbreak are independently demonstrated; the available discussion does not establish which firmware versions are affected.

**「Community discussion」** Commenters focused on the exploit&\#x27;s attack surface: MaxBarraclough asked whether the PS5&\#x27;s WebKit runs JavaScriptCore with JIT enabled and whether Sony would disable JIT in response, while Muromec said such communities typically hold additional undisclosed vulnerabilities. Other comments were aspirational, including hopes for playing Steam games on PS5 or waiting until GTA6.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/ Relapse - Exploit : Exploit chain for PS 5 7.00 - 13.60</a></li>
<li><a href="https://www.superpsx.com/ps5-relapse-jailbreak-13-60-and-lower-complete-guide/">PS 5 Relapse Jailbreak 13.60 and Lower – Complete Guide</a></li>

</ul>
</details>

**Tags**: `#security`, `#exploit`, `#PS5`, `#WebKit`, `#jailbreak`

---

<a id="item-tech-news-12"></a>
### [Tcl/Tk 9.1 released, continues legacy of simplicity](https://www.tcl-lang.org/software/tcltk/9.1.html) ⭐️ 6.0/10

Tcl/Tk 9.1 is an incremental release of the long-established scripting language and GUI toolkit, now available for download. The release maintains Tcl/Tk&\#x27;s reputation for simplicity and continues to support modern platforms, though no specific new features or changes are detailed in the available announcement. The update is primarily of interest to existing Tcl/Tk users and enthusiasts.

hackernews · dmux · Sep 29, 17:13 · [Discussion](https://news.ycombinator.com/item?id=49896712)

**「Background」** Tcl/Tk is a long-established open-source scripting language and GUI toolkit, originally valued for making GUI programming on Unix and the X Window System relatively easy. The 9.1 release builds on the Tcl/Tk 9.0 foundation by adding new features and interfaces, and an earlier alpha \(9.1a1\) had already summarized the differences from 9.0.

**「Community Discussion」** Commenters on Hacker News express fondness for Tcl/Tk&\#x27;s unique design and ease of use, with several noting it remains the simplest GUI toolkit available. One commenter cautions against professional use while praising its playful character, while others highlight Tk&\#x27;s historical role in making GUI programming accessible through minimal code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tcl-lang.org/software/tcltk/9.1.html?ref=upstract.com">Tcl / Tk 9 . 1</a></li>
<li><a href="https://comp.lang.tcl.narkive.com/KwC5CCg9/tcl-9-1a1-released">Tcl 9 . 1 a 1 RELEASED</a></li>

</ul>
</details>

**Tags**: `#Tcl/Tk`, `#release`, `#GUI toolkit`, `#scripting language`, `#programming languages`

---

<a id="item-tech-news-13"></a>
### [Rust GPU as a standard compiler target: vision and prototype](https://lwn.net/Articles/1095731/) ⭐️ 6.0/10

At RustConf 2026, rust-gpu and Rust CUDA maintainer Christian Legnitto described a plan to make the GPU a standard compiler target for ordinary Rust code, with no dedicated libraries or ecosystem support required. He has not yet shipped this capability; the plan rests on a prototype that he says he is preparing to release, and the talk supplied no measured results. For now, Rust GPU programming still depends on the existing rust-gpu and Rust CUDA projects.

rss · LWN.net · Sep 29, 17:57

**「背景」** Traditionally, writing Rust code for GPUs has required special libraries such as rust-gpu or Rust CUDA, which translate Rust into API- or vendor-specific forms such as SPIR-V for Vulkan or CUDA for NVIDIA hardware. Christian Legnitto, who maintains those libraries, is proposing a different approach in which the Rust compiler itself treats the GPU as a standard target, eliminating the need for such libraries.

**Tags**: `#Rust`, `#GPU`, `#compilers`, `#programming languages`, `#open source`

---

<a id="item-tech-news-14"></a>
### [AI-Has-Taste Finds Confirmed Counterexample; Repo Tops 453 Manuscripts](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+AI%E6%89%BE%E5%87%BA%E6%95%B0%E5%AD%A6%E5%8F%8D%E4%BE%8B%E6%8E%A8%E7%BF%BB%E8%AE%BA%E6%96%87%EF%BC%8C%E4%BD%9C%E8%80%85%E7%A1%AE%E8%AE%A4%EF%BC%81453%E7%AF%87%E6%89%8B%E7%A8%BF%EF%BC%8CAI%E5%BC%80%E5%A7%8B%E8%87%AA%E5%B7%B1%E5%87%BA%E9%A2%98%E4%BA%86) ⭐️ 6.0/10

新智元 reports that researcher Zeng Zaijian’s AI-Has-Taste system at UCSI University constructed a counterexample to a conjecture from a paper and received a reply from the paper’s author confirming it holds. The project’s public GitHub repository now lists 453 mathematics research manuscripts totaling 2,312 pages, with six explicitly categorized as AI-proposed conjectures. According to the report, this confirmed counterexample shifted the project from answer generation toward research-agenda generation, with topic selection, proof attempts, counterexample search, failure management, review, and writing increasingly run by agents on parallel machines.

rss · 新智元 · Sep 29, 03:40

**「Background」** AI Has Taste is a research system developed at UCSI University that automates mathematical research tasks including proof attempts, counterexample search, and conjecture generation. The system has produced over 450 mathematical manuscripts and six original conjectures, and is designed to move from answering given questions to proposing new research directions.

**「Impact」** The AI Has Taste system produced a counterexample to a published mathematical conjecture that the original paper&\#x27;s author confirmed as valid, demonstrating that current AI can autonomously refute claims in mathematical research. The project&\#x27;s public repository now contains 453 manuscripts and 6 AI-proposed conjectures, indicating a shift from answer generation to research-agenda generation. For mathematicians, this suggests that AI-driven counterexample search can serve as an additional verification layer for new results, though the system&\#x27;s reliability and breadth of coverage remain to be independently assessed.

**Tags**: `#AI for Mathematics`, `#Automated Theorem Proving`, `#Counterexample Search`, `#AI Research`, `#Research Integrity`

---

<a id="item-tech-news-15"></a>
### [Free open-source book: &\#x27;How to Make Your Model Fast&\#x27; teaches ML performance engineering](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 6.0/10

The author released How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents as a free, open-source book on GitHub at github.com/usamahz/make-your-model-fast. It targets ML performance engineers and developers by covering the full stack, from roofline analysis and hardware fundamentals through kernels, compilers, quantization, pruning, profiling, serving, and agent systems. The book&\#x27;s core argument is that reducing FLOPs alone does not make models faster; instead, engineers should determine whether a system is compute-, bandwidth-, memory-, or system-bound before choosing an optimization. It is a self-published resource with no external validation yet and invites feedback and contributions.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Background」** In ML performance engineering, reducing FLOPs does not automatically make a model faster; the real bottleneck may be compute, memory bandwidth, or system overhead. A common starting point is roofline analysis, which compares a workload&\#x27;s arithmetic intensity with a given piece of hardware&\#x27;s limits to estimate the fastest possible runtime. The announced book is a new free and open-source educational resource, so it has no direct predecessor or follow-up development to compare it with.

**「Impact」** The first edition of How to Make Your Model Fast is now freely available at ai.usamah.me, offering ML engineers and researchers a structured, systems-level guide to optimizing model performance from hardware to agents. The open-source license invites community contributions and feedback, enabling practitioners to both learn from and help improve the resource.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/usamahz/make-your-model-fast/releases/tag/v1.0">Release How to Make Your Model Fast, first edition · usamahz/make-your-model-fast</a></li>

</ul>
</details>

**Tags**: `#ML performance`, `#Systems optimization`, `#Open source`, `#LLM inference`, `#Hardware`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Trump&\#x27;s municipal bond portfolio grows to as much as $1 billion](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 8.0/10

President Donald Trump’s municipal bond portfolio — debt issued by cities, hospitals, schools, utilities and other public institutions — now totals more than 1,000 positions worth between $300 million and $1 billion, according to a CNBC analysis of his financial disclosures. The holdings include bonds tied to issuers affected by his administration’s policies; CNBC found no evidence of wrongdoing, and the White House says outside managers make all investment decisions.

rss · CNBC Finance · Sep 29, 14:37

**「Background」** Trump ended 2025 with 807 municipal bond positions worth between $240.7 million and $797.6 million, and as president he is exempt from typical federal conflict-of-interest laws that would restrict such holdings.

**Tags**: `#Municipal Bonds`, `#Trump Administration`, `#Conflict of Interest`, `#Financial Disclosures`, `#Ethics`

---

<a id="item-finance-news-2"></a>
### [Goldman Sachs board reportedly weighs replacing CEO David Solomon](https://www.cnbc.com/2026/09/29/goldman-sachs-ceo-succession-planning.html) ⭐️ 7.0/10

Goldman Sachs&\#x27; board has reportedly discussed replacing CEO David Solomon with president John Waldron as early as next year, according to The Wall Street Journal, with a vote possible in coming months. The plan faces uncertainty because Solomon may resist handing over the role and Waldron may not wait indefinitely.

rss · CNBC Finance · Sep 29, 20:50

**「Background」** Solomon, 64, has led Goldman since 2018, and the bank is coming off a strong period as a top pure-play investment bank, with over $1 trillion in merger deals advised and more than $12 billion in equities revenue in the first half of the year.

**Tags**: `#Goldman Sachs`, `#CEO succession`, `#corporate governance`, `#David Solomon`, `#John Waldron`

---

<a id="item-finance-news-3"></a>
### [Fair Isaac drops 18% after FHFA mortgage-pricing change; AMD, AstraZeneca and CarMax lead premarket moves](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

In CNBC’s premarket roundup, Fair Isaac shares plunged 18% after Federal Housing Finance Agency director Bill Pulte said Fannie Mae and Freddie Mac will move to one mortgage-pricing grid and add VantageScore alongside FICO; AMD traded more than 1% higher after agreeing to buy AI firm World Labs for $8.2 billion; Summit Therapeutics jumped 18% after AstraZeneca announced a $2 billion strategic investment; and CarMax gained more than 6% after reporting second-quarter earnings of $1.16 per share on $7.88 billion in revenue, above the FactSet consensus of 73 cents per share and $7.09 billion.

rss · CNBC Finance · Sep 29, 12:03

**「Background」** Fair Isaac provides FICO credit scores used in mortgage pricing, and the FHFA change replaces the current two pricing grids with one grid that also includes VantageScore.

**Tags**: `#stock movers`, `#FHFA mortgage pricing`, `#M&amp;A`, `#earnings`, `#biotech financing`

---

<a id="item-finance-news-4"></a>
### [China Tightens IPO Criteria for Humanoid Robot Startups](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has told humanoid-robot startups seeking IPOs they must meet three criteria — sustainable revenue and commercial orders, narrowing losses backed by a three-year forecast, and core technology such as a robotic brain or hands — and sources say few, if any, of the companies can qualify. At least two dozen humanoid-related companies have filed to list in Hong Kong alone, but expectations are now for only a handful, or none, to reach public markets.

rss · CNBC Finance · Sep 29, 07:19

**「Background」** The rules follow a boom: sector investment hit 47.09 billion yuan \($6.95 billion\) in the second quarter, up more than sixfold year over year, according to industry data provider Xiniu, and posterchild Unitree listed in Shanghai on Aug. 19 with shares surging over 460% on debut before nearly halving by Monday. Founder Wang Xingxing cautioned a day after the IPO that commercialization beyond dancing robots was years away.

**「Impact」** For the more than 100 Chinese humanoid-robot startups and their early investors, the stricter listing bar narrows the IPO exit path at a time when listed peers are already losing value, with Hong Kong-listed Ubtech down more than 40% this year.

**Tags**: `#China regulatory policy`, `#humanoid robots`, `#IPO criteria`, `#embodied AI`, `#CSRC`

---

<a id="item-finance-news-5"></a>
### [China to Subsidize New First-Home Mortgages From Oct 1](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 7.0/10

China’s finance ministry, central bank and financial regulator announced on Sept 29 that, starting Oct 1, 2026, eligible families buying a first home with a new commercial mortgage will receive a central-government interest subsidy of 1 percentage point per year for up to five years, on loan principal capped at 1 million yuan.

telegram · zaihuapd · Sep 29, 10:18

**「Background」** The subsidy is for new loans only; replacing an existing mortgage does not qualify, and the home must be no larger than 120 square meters and priced no higher than 1.5 million yuan. The program is initially set to run for one year.

**「Impact」** Eligible first-home buyers can cut their annual interest cost by up to about 10,000 yuan for as long as five years, subject to the loan, size and price limits.

**Tags**: `#住房贷款`, `#财政贴息`, `#房地产政策`, `#首套住房`, `#宏观政策`

---

