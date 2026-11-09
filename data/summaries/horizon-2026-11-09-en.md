# Horizon Daily - 2026-11-09

> From 59 items, 19 important content pieces were selected

---

**Technology News**
1. [Dux v2.0: Free Wayland Shell Adds Atomic Distro Support](#item-tech-news-1) ⭐️ 7.0/10
2. [Goldman Sachs Pulls Claude Code From Bankers and Traders](#item-tech-news-2) ⭐️ 7.0/10
3. [Outlook.com Rejecting Email from Domains Without DMARC](#item-tech-news-3) ⭐️ 7.0/10
4. [Developer Switches from Claude to Pi LLM Harness](#item-tech-news-4) ⭐️ 7.0/10
5. [Claude Code leaks user email via User-Agent headers; update urged](#item-tech-news-5) ⭐️ 7.0/10
6. [NeurIPS 2026: Agent MechSuits Intervenes in 10 Dimensions for 97% Accuracy](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek-V4.1-Flash Adds Self-Written Python Rollback Code, Claims 7-Point Math Gain](#item-tech-news-7) ⭐️ 7.0/10
8. [Writing as a Thinking Tool](#item-tech-news-8) ⭐️ 6.0/10
9. [Nvidia Board Probes Intelligence Operation Targeting CEO Jensen Huang](#item-tech-news-9) ⭐️ 6.0/10
10. [SQLite parse\_number\(\) Extension: C vs Rust Performance and Size](#item-tech-news-10) ⭐️ 6.0/10
11. [Nace Claims Drex Max v1.1 Tops Decision Model Benchmark](#item-tech-news-11) ⭐️ 6.0/10
12. [Yao Shunyu: AI Moats Lie in Product Layer, Not Model Layer](#item-tech-news-12) ⭐️ 6.0/10
13. [Apple Siri Agentic Push Reportedly Set for 2027](#item-tech-news-13) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly ROCm Release](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache Nightly RBLN NPU Wheel Release](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache nightly-cu129 Release](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache Nightly CUDA 13.0 Wheels](#item-ai-projects-4) ⭐️ 5.0/10

**Twitter News**
1. [@levelsio: Infinite Slop TV Postmortem](#item-twitter-news-1) ⭐️ 8.0/10
2. [AI Walkthrough Prompt for Product &amp; UX Review](#item-twitter-news-2) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Dux v2.0: Free Wayland Shell Adds Atomic Distro Support](https://duxlabs.dev/) ⭐️ 7.0/10

Dux, the free and open-source Wayland desktop shell previously known as Dank Material Shell, has released version 2.0 and added official support for atomic distributions such as Bazzite. The shell provides a file manager and theming and is designed for use with the Niri Wayland compositor. The v2.0 release follows the project&\#x27;s rebranding and addresses what users describe as a notable compatibility gap for popular immutable distros.

hackernews · indigodaddy · Nov 8, 19:08 · [Discussion](https://news.ycombinator.com/item?id=50416053)

**「From Dank Material Shell to Dux」** The project was formerly known as Dank Material Shell and has been paired with the Niri compositor for about a year, according to community reports. The v2.0 release rebrands it to Dux and adds official support for atomic Linux distributions such as Bazzite, which users had previously identified as a gap.

**「Impact」** Users of Bazzite and other atomic or immutable distributions can now adopt Dux with official support, removing a previously reported compatibility gap for those platforms.

**「Community discussion」** A long-time user calls Dux &quot;endlessly slick&quot; and believes it can help mainstream Niri, while another who has run DMS+Niri for nearly a year compares the experience to settling down in desktop customization. A separate commenter warns that the curl \| sh installation should be adopted and reviewed by a Linux distribution before being trusted unconditionally, and one user finds the project becoming more all-encompassing than they want.

**Tags**: `#Wayland`, `#desktop-shell`, `#open-source`, `#Linux`, `#Niri`

---

<a id="item-tech-news-2"></a>
### [Goldman Sachs Pulls Claude Code From Bankers and Traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

Goldman Sachs is pulling Anthropic&\#x27;s Claude Code from its bankers and traders, removing access to the AI coding agent for those finance professionals. The available source does not include specifics about timing, scope, or the bank&\#x27;s official rationale.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**「Background」** The move reverses an earlier position: as recently as July, Goldman Sachs CIO Marco Argenti publicly praised &quot;vibe coding&quot; by non-technical staff, according to The Decoder.

**「Community Discussion」** Some commenters attribute the removal to security risks of running semi-unattended agents on workstations with client, trade, and email access, while others report billing overages pushing organizations toward flat-rate alternatives like Gemini. A separate comment questions whether the timing, weeks before Goldman Sachs leads Anthropic&\#x27;s IPO, is significant.

<details><summary>References</summary>
<ul>
<li><a href="https://the-decoder.com/goldman-sachs-pulls-ai-coding-tools-from-traders-and-bankers/">Goldman Sachs pulls AI coding tools from traders and bankers</a></li>

</ul>
</details>

**Tags**: `#AI`, `#enterprise software`, `#cybersecurity`, `#fintech`, `#Claude`

---

<a id="item-tech-news-3"></a>
### [Outlook.com Rejecting Email from Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Microsoft&\#x27;s Outlook.com has started rejecting email sent from domains that do not publish a DMARC policy, according to a MailRoute report. The change affects senders whose domains lack DMARC, potentially causing their messages to Outlook.com recipients to fail delivery. Specific implementation details, such as error codes or rollout scope, were not included in the supplied report.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**「Background」** DMARC is an email authentication protocol that lets domain owners publish a policy telling receivers how to handle mail that fails SPF or DKIM alignment. A May 2025 sender guide noted that Outlook.com was already rejecting non-compliant mail with only a p=none policy \(tool-1-3\), so the current change extends rejection to domains that publish no DMARC record at all.

**「Impact」** Organizations and individuals who send email to Outlook.com addresses must publish a DMARC policy for their sending domains to avoid delivery failures. Administrators should verify DMARC configuration before relying on Outlook.com delivery.

**「Community Discussion」** One commenter disputes the &\#x27;quietly&\#x27; characterization, saying Outlook returns 5xx permanent delivery failures for these rejections. Another reports long-standing deliverability problems with Outlook even when SPF, DKIM, and DMARC are correctly configured, suggesting the new DMARC requirement is not the only factor affecting inbox placement.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.getshadowinbox.com/posts/outlook-cold-email-rejected">Outlook Is Rejecting Your Cold Email . — Shadow Inbox blog</a></li>

</ul>
</details>

**Tags**: `#email`, `#dmarc`, `#outlook`, `#deliverability`, `#microsoft`

---

<a id="item-tech-news-4"></a>
### [Developer Switches from Claude to Pi LLM Harness](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

A developer has posted about switching from Claude to Pi, an LLM harness, prompting Hacker News discussion of prompt harness design, model performance, and usage policies. Commenters describe Pi as a high-control alternative that can run models such as abliterated GLM, but note it may not follow Anthropic&\#x27;s undocumented communication mechanisms.

hackernews · karagenit · Nov 8, 03:11 · [Discussion](https://news.ycombinator.com/item?id=50410107)

**「What Pi is」** Pi is a minimal, extensible AI agent harness that users can adapt to their own workflows through extensions, skills, prompt templates, and themes, with packages shared via npm or git. It intentionally omits features such as sub-agents and plan mode to stay lightweight.

**「Impact」** For users who want to use Pi with Claude, a concrete risk is a possible Anthropic account ban because the harness may violate terms of service.

**「Community discussion」** Commenters disagree on whether Pi&\#x27;s control outweighs its tradeoffs: gvkhna says it reduces frustration and improves agent orchestration, while leobuskin warns it lacks Anthropic&\#x27;s custom communication mechanisms, which can change model behavior, and real\_faxenoff notes that much of a model&\#x27;s effectiveness resides in the harness. bottlepalm reports outgrowing TUI tools in favor of desktop apps with cleaner history.

<details><summary>References</summary>
<ul>
<li><a href="https://pi.dev/">Pi - There are many agent harnesses</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/pi: AI agent toolkit: unified LLM API ...</a></li>

</ul>
</details>

**Tags**: `#LLM tooling`, `#AI assistants`, `#command-line`, `#Anthropic Claude`, `#open-source AI`

---

<a id="item-tech-news-5"></a>
### [Claude Code leaks user email via User-Agent headers; update urged](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E5%B0%8F%E5%BF%83%EF%BC%8CClaude%20Code%E4%BC%9A%E6%93%85%E8%87%AA%E6%B3%84%E9%9C%B2%E4%BD%A0%E7%9A%84%E9%82%AE%E7%AE%B1%EF%BC%81%E8%AF%B7%E6%8A%93%E7%B4%A7%E6%97%B6%E9%97%B4%E6%9B%B4%E6%96%B0) ⭐️ 7.0/10

Anthropic&\#x27;s Claude Code was reported on November 5, 2026 to send users&\#x27; real login email, name, team, and company GitHub repository paths in HTTP User-Agent request headers when fetching external sites. The cause was engineers adding the login email to the model&\#x27;s system prompt; the model then included it when some sites required a contact email to avoid 403 responses. Claude Code engineer Lydia Hallie apologized on November 6, and the report urges users to update immediately, though the supplied source does not specify affected or patched version numbers.

rss · 新智元 · Nov 8, 13:11

**「Background」** Claude Code is Anthropic&\#x27;s terminal coding assistant that fetches external web pages to complete tasks; sites such as the SEC, Wikipedia, and crates.io require a contact email in the User-Agent header. To satisfy that requirement, Anthropic&\#x27;s engineers embedded the user&\#x27;s login email in the model&\#x27;s system context, which then leaked it into outbound request headers. The behavior was publicly reported on November 5, 2026, and confirmed in a GitHub issue; Anthropic engineer Lydia Hallie apologized and clarified the cause on November 6.

**「Exposed identifiers require immediate update」** Claude Code can send a user&\#x27;s login email, real name, team name, and internal GitHub repository path to external sites such as SEC EDGAR, Wikipedia, crates.io, and EVE Online APIs via the User-Agent header, as reported in the source article. Affected developers should treat those identifiers as compromised, inspect request logs for unexpected User-Agent strings, and apply the update or community mitigation steps described in supplemental reports \(tool-2-1, tool-2-2\); the article does not specify a fixed version number.

<details><summary>References</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/30672/claude-code-bug-email-user-agent-header">Claude Code bug sends your email to websites in the User - Agent</a></li>
<li><a href="https://github.com/anthropics/claude-code/issues/107757">Bug Report: Privacy violation in User - Agent header · Issue #107757...</a></li>
<li><a href="https://dev.to/naveenmalothu/claude-code-leaks-your-email-what-it-means-and-how-to-safeguard-your-apps-m9">Claude Code Leaks Your Email – What It Means and How to ...</a></li>
<li><a href="https://explainx.ai/blog/claude-code-leaks-your-email-user-agent-header-how-to-stop-it-2026">Claude Code Leaks Your Email in Headers: 5-Min Fix - explainx.ai</a></li>

</ul>
</details>

**Tags**: `#Claude Code`, `#security vulnerability`, `#AI coding tools`, `#privacy`, `#software update`

---

<a id="item-tech-news-6"></a>
### [NeurIPS 2026: Agent MechSuits Intervenes in 10 Dimensions for 97% Accuracy](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+NeurIPS%2726%20%7C%20%E5%8F%AA%E5%B9%B2%E9%A2%8410%E4%B8%AA%E7%BB%B4%E5%BA%A6%EF%BC%8C%E7%BB%99%E6%99%BA%E8%83%BD%E4%BD%93%E7%A9%BF%E4%B8%8A%E5%AE%89%E5%85%A8%E6%9C%BA%E7%94%B2%EF%BC%8C%E5%87%86%E7%A1%AE%E7%8E%87%E8%B6%8597%25) ⭐️ 7.0/10

Researchers from the University of Georgia, Rutgers University, and the University of Southern California have introduced Agent MechSuits, a safety mechanism for multi-turn command-line interface \(CLI\) agents that reads internal model signals before each action and, when risk is detected, intervenes in 10 hidden representation dimensions within a single layer while keeping the base model weights frozen. Accepted at NeurIPS 2026, the method reports a 97.32% average accuracy for current-step risk detection across three tested models. The paper is available as arXiv:2606.22673, with a project page at eddyluo.com/Agent-MechSuits/.

rss · 新智元 · Nov 8, 09:45

**「Background」** CLI agents operate through multi-turn command execution, so a single command may appear safe while risk accumulates only over later steps. External guardrails that review one action therefore miss that accumulated risk, motivating white-box defenses like Agent MechSuits that inspect internal model states and perform representation-level mitigation during runtime.

**「Impact」** Because the intervention is sparse and the base model weights remain frozen, the method could be added to existing CLI agents as a lightweight safety layer without retraining or changing the underlying model.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.22673">[2606.22673] Agent MechSuits: Mechanistic Subspace Safety ...</a></li>

</ul>
</details>

**Tags**: `#ai-safety`, `#agents`, `#neurips-2026`, `#representation-engineering`, `#model-interpretability`

---

<a id="item-tech-news-7"></a>
### [DeepSeek-V4.1-Flash Adds Self-Written Python Rollback Code, Claims 7-Point Math Gain](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+AI%E4%BA%B2%E6%89%8B%E6%94%B9%E5%86%99Transformer%E6%9E%B6%E6%9E%84%EF%BC%81DeepSeek%E8%87%AA%E6%88%91%E6%94%B9%E9%80%A0%E6%9A%B4%E6%B6%A87%E5%88%86) ⭐️ 7.0/10

Researchers at DoubleAI claim DeepSeek-V4.1-Flash, a 763-billion-parameter model, read its internal activations from the deepest seven layers during math tasks, identified signals that its reasoning was about to go wrong, and inserted Python code into the inference process without changing weights. The code rolls back and recomputes when it detects an incorrect path, producing a reported 7 percentage point accuracy improvement on AIME and HMMT 2026. The broader mechanism intervention method lets a programming agent write candidate Python functions during training, gate them behind zero-initialized gates, and let subsequent training enable them; inserting code into ten layers reportedly raised accuracy on 30 classical algorithms from 55% to 84%. These figures are presented as the research group&\#x27;s claims, not independent benchmark results.

rss · 新智元 · Nov 8, 09:45

**「Background」** Horizon&\#x27;s October 18 digest reported that DeepSeek released DeepSeek-V4.1-Flash-1017, a minor update to DeepSeek-V4.1-Flash with vendor-reported improvements in reasoning, coding, and agentic tasks. The current article concerns a separate DoubleAI study that claims to inject generated Python code into DeepSeek-V4.1-Flash&\#x27;s inference process—an approach the authors call &\#x27;mechanism intervention&\#x27;—rather than altering trained weights.

**「Impact」** Developers should treat the 7-point and 55% to 84% improvements as unverified vendor claims until the intervention code and evaluation baselines are released, because the source provides no independent reproduction data or exact AIME/HMMT scores.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017">2026-10-18 — DeepSeek-V4.1-Flash-1017 Released With Coding Benchmark Gains</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#Transformer`, `#architecture search`, `#machine learning`

---

<a id="item-tech-news-8"></a>
### [Writing as a Thinking Tool](http://muratbuffalo.blogspot.com/2026/11/writing-as-thinking-tool.html) ⭐️ 6.0/10

The linked Hacker News discussion concerns a blog essay titled &\#x27;Writing as a thinking tool,&\#x27; which argues that writing is a fundamental part of thinking rather than merely a final summarization step. Comments from software engineers and researchers describe how writing drafts, sketching system diagrams, and even hand-writing code help them clarify requirements and ideas before building. The item is a reflective essay and discussion; no software, standard, or policy change is announced.

hackernews · jruohonen · Nov 8, 10:41 · [Discussion](https://news.ycombinator.com/item?id=50412067)

**「Background」** The essay&\#x27;s premise aligns with a common view in research and software practice that externalizing ideas—on paper, in diagrams, or in code—forces them into a more explicit and testable form; commenters extend this to design and programming workflows.

**「Community Discussion」** Several commenters report that writing is part of the thinking process: billypilgrim says drafting was not an epilogue to science but central to it, and drewbeck says for novel UX problems the tight loop of designing provides insights that prompting has not matched. lilerjee and hoppp similarly describe hand-writing code and paper diagrams as thinking tools before creating a codebase.

**Tags**: `#writing`, `#cognition`, `#software-engineering`, `#research`, `#communication`

---

<a id="item-tech-news-9"></a>
### [Nvidia Board Probes Intelligence Operation Targeting CEO Jensen Huang](https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors) ⭐️ 6.0/10

Nvidia&\#x27;s board of directors is investigating an intelligence operation that targeted CEO Jensen Huang, not investigating Huang personally, according to the company&\#x27;s statement and community clarification of the original misleading headline. A Bloomberg report cited in the comments says the board will probe a spying case after Huang admitted infidelity. Available details beyond those board and media statements are limited.

hackernews · vincentchau · Nov 8, 20:26 · [Discussion](https://news.ycombinator.com/item?id=50416801)

**「Context」** Nvidia’s board is launching an investigation into whether CEO Jensen Huang was targeted by a foreign espionage operation after he admitted to employees that he had an extramarital affair. Reports cited by Bloomberg and the NY Post identify the woman as suspected of spying for the Chinese government, and the board inquiry will examine whether Huang was among individuals targeted by such a plot.

**「Community Discussion」** Commenters emphasized that the original headline misleadingly implies the board is investigating Huang when it is investigating something that happened to him. Others speculated that if Huang knew a Singapore company was a Chinese front, it could raise U.S. export-control questions, while some said such intelligence targeting of powerful executives is expected and the claims remain unproven.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity">Nvidia Board to Probe Spying Case After CEO Jensen... - Bloomberg</a></li>
<li><a href="https://nypost.com/2026/11/08/tech/jensen-huang-ceo-of-4-5t-chipmaker-nvidia-admits-affair-as-memo-warned-lover-was-chinese-spy/">Jensen Huang, CEO of $4.5T chipmaker Nvidia admits affair — as...</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#jensen-huang`, `#corporate-governance`, `#security`, `#tech-industry`

---

<a id="item-tech-news-10"></a>
### [SQLite parse\_number\(\) Extension: C vs Rust Performance and Size](https://simonwillison.net/2026/Nov/8/sqlite-parse-number-c-vs-rust/) ⭐️ 6.0/10

Simon Willison published a research report comparing a parse\_number\(\) SQLite extension written in C versus Rust. The initial Rust extensions were faster than a 14 KB C extension, but they were 321 KB \(rusqlite\) and 298 KB \(sqlite-loadable-rs\). After prompting Claude Opus 5.5 to write a custom C parser, the new C version beat both Rust implementations with net costs of 19 ns versus 46 ns and 41 ns per row on mixed data over 2 million rows.

rss · Simon Willison · Nov 8, 22:26

**「Background」** SQLite supports user-defined functions through loadable extensions, and both C and Rust can compile to .so files that SQLite can load. The parse\_number\(\) function strips characters such as \`,\`, \`$\`, \`£\`, and \`%\` from strings and handles a leading minus sign, returning NULL when parsing fails.

**「Impact」** SQLite extension authors comparing C and Rust now have a concrete benchmark showing that an optimized C implementation can provide both a much smaller binary \(14 KB vs 298–321 KB\) and lower per-row overhead than the Rust options measured, although it required writing a custom parser rather than using C&\#x27;s standard strtod.

**Tags**: `#SQLite`, `#Rust`, `#C`, `#extensions`, `#performance`

---

<a id="item-tech-news-11"></a>
### [Nace Claims Drex Max v1.1 Tops Decision Model Benchmark](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 6.0/10

Nace has released Drex Max v1 open weights and announced a v1.1 update that it says achieves SOTA and Pareto frontier status on Artificial Analysis&\#x27;s multimodal decision model benchmark. The v1 weights are available on Hugging Face under an Open RAIL-M license, while v1.1 weights are not yet released and are being optimized for local inference. The company claims a ~256k context window, Mac compatibility via its Kapitsa engine, and 8x lower cost than the next-best model in the Artificial Analysis index, but the post does not provide independent verification.

reddit · r/MachineLearning · /u/m4rkGS · Nov 8, 17:54

**「Background」** Drex Max is a decision model that takes a state \(text, JSON or images\) plus named questions and returns a probability for each option. Its earlier v1 release scores 64 on the Artificial Analysis Decision Index, a weighted average of AA-Omniscience-Decision, HLE-MultiChoice, When2Call and WildGuardTest.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/11/01/nace-ai-open-sources-drex-max-v1-local-inference/">Nace AI Open-Sources Drex Max v 1 : A 27B Decision Model That...</a></li>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/ drex - max - v 1 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#multimodal models`, `#decision models`, `#open source`, `#benchmarks`

---

<a id="item-tech-news-12"></a>
### [Yao Shunyu: AI Moats Lie in Product Layer, Not Model Layer](https://www.ithome.com/1/023/991.htm) ⭐️ 6.0/10

At a November 8, 2026 Future Science Award dialogue, Tencent chief AI scientist Yao Shunyu argued that AI companies&\#x27; competitive moats lie in the product layer rather than the model layer. He said the hardest-to-replace products are those that understand user context, control proprietary data, and earn trust, citing WeChat as an example: an AI embedded in WeChat could know users&\#x27; schedules and social relationships, making it difficult for a smarter rival model to provide the same service. Zhang Yaqin responded with a joke that, by this logic, Anthropic might not be worth two trillion dollars.

telegram · zaihuapd · Nov 8, 14:17

**「Background」** In AI industry debates, competition is often measured by model capabilities or benchmark performance. Yao&\#x27;s argument frames defensibility instead around product-level access to user context, proprietary data, and trust.

**Tags**: `#artificial intelligence`, `#technology industry`, `#product strategy`, `#competitive moat`, `#Tencent`

---

<a id="item-tech-news-13"></a>
### [Apple Siri Agentic Push Reportedly Set for 2027](https://9to5mac.com/2026/11/08/apple-working-on-agentic-siri-ai-next-year-report/) ⭐️ 6.0/10

Bloomberg&\#x27;s Mark Gurman reports that Apple may make Siri more agentic as early as 2027, after iOS 27 added personalization but still lacks proactive task execution. Apple is also changing its internal process for the first iOS 28 development cycle, replacing the usual four-week coding and four-week integration schedule with six weeks of coding exploration and two weeks of convergence. The claim is an unconfirmed rumor and lacks detailed technical specifics.

telegram · zaihuapd · Nov 8, 16:36

**「Context」** Apple has been rolling out Siri-related AI features in stages. Horizon&\#x27;s November 4 digest reported that the iOS 27.3 beta added Siri Recap and Live Rewind on Apple Watch, and its October 15 digest noted that the China Apple Intelligence launch would exclude the new Siri. The current report builds on this by stating that Siri has achieved personalization in iOS 27 but still lacks the ability to proactively act on a user&\#x27;s behalf.

**「Impact」** If the reported schedule holds, iOS 28 developers might face a longer exploratory coding phase and a shorter convergence window, while users may not see agentic Siri until 2027 at the earliest.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-14/apple-prepares-to-debut-first-ai-features-in-china-in-december">2026-10-15 — Apple Plans December Launch of Apple Intelligence in Mainland China</a></li>
<li><a href="https://www.macrumors.com/2026/11/03/ios-27-3-health-app/">2026-11-04 — iOS 27.3 Beta Brings Health Redesign, Watch AI Transcription, China Apple Intelligence</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Siri`, `#AI agents`, `#iOS`, `#software engineering process`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly ROCm Release](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels for LMCache, built from the dev branch, targeting AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), ABI-matched to upstream vllm/vllm-openai-rocm image.

github · github-actions\[bot\] · Nov 8, 08:24

**「解决的痛点」** Simplifies deployment for AMD Instinct GPU users by providing prebuilt binary wheels that match the ABI of the upstream vLLM ROCm container \(torch 2.13, cp312\), eliminating the need to compile LMCache from source and reducing setup friction.

**「背景与影响」** This is a routine nightly packaging update from LMCache, an LLM inference caching library. It extends support to ROCm 7.2 and AMD Instinct GPUs, aligning with the vLLM ROCm ecosystem, but introduces no new architectural or performance claims.

**Tags**: `#llm`, `#inference`, `#rocm`, `#lmcache`, `#nightly`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly RBLN NPU Wheel Release](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

Prebuilt nightly wheel of LMCache for Rebellions RBLN NPU, generated from the dev branch on 2026-11-08 against torch-rbln 0.12.0. It enables testing LLM inference caching on RBLN hardware without building from source.

github · github-actions\[bot\] · Nov 8, 08:16

**「解决的痛点」** The nightly build removes the need to compile LMCache from source for RBLN NPU, addressing the friction of maintaining a compatible build environment with torch-rbln and rebel-compiler. It provides a consistent package version for testing on that hardware.

**「背景与影响」** LMCache is an LLM inference caching layer that reduces repeated computation and lowers latency/cost. This nightly release targets Rebellions RBLN NPUs, expanding LMCache&\#x27;s hardware support beyond common GPUs. It is a routine development snapshot, not a feature release, and relies on externally installed torch-rbln and rebel-compiler.

**Tags**: `#LLM`, `#inference`, `#cache`, `#nightly`, `#NPU`

---

<a id="item-ai-projects-3"></a>
### [LMCache nightly-cu129 Release](https://github.com/LMCache/LMCache/releases/tag/nightly-cu129) ⭐️ 5.0/10

Nightly build of LMCache providing pre-built Python wheels compiled against CUDA 12.9 for Linux \(amd64 and arm64\). Enables easy installation of LMCache on systems with CUDA 12.9 without source compilation.

github · github-actions\[bot\] · Nov 8, 11:49

**「Problem Solved」** Addresses compatibility and installation friction for users running CUDA 12.9. Previously, users on CUDA 12.9 had to compile LMCache from source or use older CUDA wheels, causing deployment delays and potential incompatibility with newer GPUs and PyTorch builds.

**「Background」** LMCache is an LLM caching engine that reduces cost and latency by reusing KV caches. As the AI ecosystem moves toward CUDA 12.9 and newer PyTorch versions, providing nightly wheels ensures LMCache stays aligned with the latest NVIDIA software stack, particularly for users with newer hardware.

**Tags**: `#lmcache`, `#cuda`, `#nightly`, `#wheels`, `#llm-caching`

---

<a id="item-ai-projects-4"></a>
### [LMCache Nightly CUDA 13.0 Wheels](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache published nightly CUDA 13.0 wheels for linux/amd64 and linux/arm64 built from the dev branch on 2026-11-08, installable via uv pip with the PyTorch cu130 index.

github · github-actions\[bot\] · Nov 8, 09:19

**「解决的痛点」** Installing LMCache from the dev branch with CUDA 13.0 typically requires building from source or manually matching PyTorch wheels. These prebuilt nightly wheels streamline dependency resolution and deployment for users testing the latest development changes.

**「Background and Impact」** LMCache is a KV cache management layer for LLM inference, enabling persistent storage and reuse of KV caches across serving engines. This nightly release builds from the \`dev\` branch and provides CUDA 13.0 wheels for Linux on amd64 and arm64. It offers early access to compatibility with the latest CUDA toolchain before official releases, useful for developers tracking upstream changes or requiring CUDA 13 support. No specific feature or performance enhancement is announced for this nightly build.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache ! | LMCache</a></li>

</ul>
</details>

**Tags**: `#llm`, `#cache`, `#cuda`, `#nightly`, `#release`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [@levelsio: Infinite Slop TV Postmortem](https://x.com/levelsio/status/2119564112208257515) ⭐️ 8.0/10

Pieter Levels shares the shutdown and statistics of Infinite Slop TV, a real-time AI-generated video stream that ran from August to October 2026. The project allowed internet users to type in a chat that fed into a continuous stream of live generated AI video. He notes this was previously impossible until @fal hacked @MiniMax\_AI&\#x27;s H3 model to be fast enough, and FAL sponsored the project to cover GPU costs that would have been at least $200,000 per month. Key stats: 17.8 million clip views, 287,555 chat messages, 287,000 likes, 210,196 AI clips aired, 125,808 messages blocked by moderation \(about 44%\), 185,000 visitors, 47,000 people made videos, and 860 hours of never-repeating video. Three sponsors are listed: @sideshiftai, @creem\_io, and @chatbase. Prizes of $5000, $2500, and $1000 were paid to winners. Levels reflects that the project didn&\#x27;t sustain attention but was a fun internet experiment. He describes emergent trends in the video content \(e.g., goth girls, slime girls, pickles, pixel art\) due to AI trying to maintain cohesion with previous clips. He sees potential for interactive and personalized live-generated content in the future but says it isn&\#x27;t there yet, citing both dystopian and utopian possibilities such as live-generated teachers.

twitter · @levelsio · Nov 8, 22:53

**「Background」** \*\*What it was:\*\* Infinite Slop TV was a real-time AI-generated video stream created by Pieter Levels \(@levelsio\) that ran from August to October 2026. Viewers could type in a chat, and their input fed a perpetual stream of live-generated AI video clips. According to Levels, the project became feasible because FAL optimized MiniMax&\#x27;s H3 model to generate faster than playback speed; FAL also sponsored the project, as GPU costs would otherwise have been at least $200,000 per month.

\*\*Key stats shared by Levels:\*\* 17,800,000 clip views; 287,555 chat messages; 287,000 likes on clips; 210,196 AI clips aired; 125,808 messages blocked by moderation \(~44%\); 185,000 visitors; 47,000 people made videos; 860 hours of never-repeating video. Sponsors were sideshiftai, creem\_io, and chatbase. Prizes: $5000 to &quot;67&quot;, $2500 to ssthormess, $1000 to tatusea\_.

\*\*Creator&\#x27;s reflections:\*\* Levels noted that the stream did not keep catching attention, but emergent visual trends appeared \(e.g., goth girls, slime girls, pickles, pixel art\). He sees potential for future live-generated interactive and personalized content, including live-generated teachers, but said the current output is still too basic and &quot;slop.&quot;

\*\*Context:\*\* No community comments were available for this post. The term &quot;slop&quot; is part of ongoing discussion about recognizable AI-generated style \(tool-1-1\). MiniMax, the AI model provider mentioned in the post, has been releasing faster inference models; its M3.1 Flash was released in October 2026 \(tool-1-2\).

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1x64lbk/tracing_where_llm_slop_style_comes_from_in_the/">2026-10-15 — Tracing where LLM &#x27;slop&#x27; style comes from and how to cut it</a></li>
<li><a href="https://mp.weixin.qq.com/s/fO9snz_lnPxVg0q55chDFg">2026-10-20 — MiniMax releases M3.1 Flash, claiming faster inference and 70% lower costs</a></li>

</ul>
</details>

**Tags**: `#AI video`, `#generative AI`, `#project retrospective`, `#real-time AI`, `#technical stats`

---

<a id="item-twitter-news-2"></a>
### [AI Walkthrough Prompt for Product &amp; UX Review](https://x.com/vista8/status/2119574943021371755) ⭐️ 6.0/10

向阳乔木 shared an AI prompt inspired by product and design walkthrough acceptance steps at large companies. The prompt instructs the AI to act as a combination of product manager, UX researcher, and top UI designer. It autonomously walks through each product page and interaction detail, deciding order and priority without waiting for instructions. It simultaneously evaluates six dimensions: information architecture, user flow, operation efficiency, feedback mechanism, visual hierarchy, and component consistency. The AI identifies issues, judges severity, assigns high-priority problems to a sub-agent for fixing, and organizes the rest into an executable plan. The goal is to meet industry-leading standards based on real users&\#x27; cognitive load and emotional experience, not just &\#x27;usable.&\#x27; The AI will take screenshots of each function to review UI details such as onboarding and functional operation UX.

twitter · 向阳乔木 · Nov 8, 23:37

**「Background」** The tweet opens with a common problem for developers: having built a tool but not knowing how to refine it further. The author notes that large companies have product and design walkthrough acceptance stages, and uses that as inspiration for the prompt. The six dimensions in the prompt reflect typical UX review categories, and the instruction to capture screenshots and delegate fixes suggests an agent-based workflow. This approach is aimed at developers who want to simulate a design review process without a dedicated product or design team.

**Tags**: `#AI prompt`, `#UX review`, `#product design`, `#automation`

---

