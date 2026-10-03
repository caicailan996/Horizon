# Horizon Daily - 2026-10-03

> From 47 items, 18 important content pieces were selected

---

**Technology News**
1. [AI defeats Stratego champions using efficient new algorithm](#item-tech-news-1) ⭐️ 8.0/10
2. [Zig v0.17.0 release notes published; discussion focuses on build, I/O, tooling](#item-tech-news-2) ⭐️ 8.0/10
3. [Greg Kroah-Hartman shows LLM kernel bugs are mostly noise](#item-tech-news-3) ⭐️ 8.0/10
4. [Rust lead outlines smart-pointer flexibility effort at RustConf 2026](#item-tech-news-4) ⭐️ 8.0/10
5. [arXiv caps submissions at two per month per submitter](#item-tech-news-5) ⭐️ 8.0/10
6. [Google Research&\#x27;s Cogentic coordinates multi-agent proofs of open problems](#item-tech-news-6) ⭐️ 8.0/10
7. [Claude Code Mods Introduces Plugin-Like Customization with TypeScript](#item-tech-news-7) ⭐️ 8.0/10
8. [Anthropic proposes opt-out copyright regime for AI training in Australia](#item-tech-news-8) ⭐️ 7.0/10
9. [SGLang v0.5.21 adds new models, on-the-fly PD switching, and Rust-based prefix cache](#item-tech-news-9) ⭐️ 6.0/10
10. [Apple Pass Designer: Official Web Tool for Wallet Passes](#item-tech-news-10) ⭐️ 6.0/10
11. [FLEET adds reward-aware memory to Best-of-N generation via MCTS](#item-tech-news-11) ⭐️ 6.0/10
12. [Sub2API 0.2.13 fixes billing bypass vulnerability](#item-tech-news-12) ⭐️ 6.0/10

**Technology Blog**
1. [AI Superpersuasion Is Bribery, Not Arguments](#item-tech-blog-1) ⭐️ 6.0/10

**Financial News**
1. [Traders see low odds of October Fed rate hike after weak jobs report](#item-finance-news-1) ⭐️ 8.0/10
2. [Bitget CEO says little recovery expected from $388M hack](#item-finance-news-2) ⭐️ 8.0/10
3. [Big midday stock movers: Tesla, Nike, Broadcom, ON Semiconductor, Synaptics](#item-finance-news-3) ⭐️ 7.0/10
4. [Premarket movers: Nike revenue miss, ON-Synaptics deal, Toshiba HDD expansion](#item-finance-news-4) ⭐️ 7.0/10
5. [Wall Street AI job postings jump 49%, with demand for agent orchestration skills up 1,721%](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AI defeats Stratego champions using efficient new algorithm](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

A new reinforcement learning algorithm has defeated the top human Stratego players, achieving superhuman performance in the imperfect-information game while learning far more efficiently than previous AI systems. The algorithm, described in a Nature paper and arXiv preprint, required about 34 times fewer training games than DeepMind&\#x27;s DeepNash and reached a higher skill level. This marks a significant advance in AI for games with hidden information.

hackernews · PaulHoule · Oct 2, 14:11 · [Discussion](https://news.ycombinator.com/item?id=49933740)

**「Background」** Stratego is a two-player board game where each player&\#x27;s pieces are hidden from the opponent, making it an imperfect-information game that has challenged AI. In 2022, DeepMind published a paper on DeepNash, a model-free multiagent reinforcement learning system that reached a high level of play but was not able to consistently beat the world&\#x27;s best human players. The new research reported in the Nature paper introduces an algorithm that learns far more efficiently than DeepNash and achieves superhuman performance.

**「Impact」** The best human Stratego players have been surpassed by an AI, ending an era where human intuition dominated the game&\#x27;s hidden-information challenges. AI researchers now have a highly sample-efficient algorithm that can serve as a template for solving other imperfect-information games with limited computational resources.

**「Community discussion」** Commenters highlighted that the key breakthrough is the algorithm&\#x27;s sample efficiency, with one noting that the difficulty of hidden-information games makes this advance critical, while another pointed out that DeepMind&\#x27;s 2022 &\#x27;Mastering Stratego&\#x27; claim has now been superseded.

**Tags**: `#game AI`, `#reinforcement learning`, `#imperfect information`, `#research`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Zig v0.17.0 release notes published; discussion focuses on build, I/O, tooling](https://ziglang.org/download/0.17.0/release-notes.html) ⭐️ 8.0/10

Zig v0.17.0 release notes are now available on the official Zig downloads page, presenting the latest version of the systems programming language as a major step forward. The supplied item does not include the release-note text, so specific changes cannot be confirmed from this source; commenters point to build integration, coroutine I/O, and tooling as topics of interest.

hackernews · ErenayDev · Oct 2, 20:56 · [Discussion](https://news.ycombinator.com/item?id=49938521)

**「Background」** Zig is a systems programming language designed as a modern alternative to C, emphasizing performance, safety, and simplicity. It has been under active development since its introduction, with each version release bringing incremental improvements to the compiler, standard library, and build system.

**「Community discussion」** Commenters offered diverging views on Zig&\#x27;s trajectory: one developer reported that after using Zig for a year, it was the best-designed language they had tried, while others asked about the project&\#x27;s AI stance and the state of evented I/O or io\_uring. Another commenter noted that Andrew is reportedly warming to LLM-assisted bug discovery, and several expressed interest in new build integration, stackless coroutine I/O, and first-class fuzzer tooling.

**Tags**: `#zig`, `#systems-programming`, `#release-notes`, `#programming-languages`, `#tooling`

---

<a id="item-tech-news-3"></a>
### [Greg Kroah-Hartman shows LLM kernel bugs are mostly noise](https://www.youtube.com/watch?v=NnV_cWeoo5Q) ⭐️ 8.0/10

In his Kernel Recipes 2026 talk, Greg Kroah-Hartman broke down Mythos&\#x27;s 79 claimed Linux kernel vulnerabilities, finding that 24 had no detail, 14 were not bugs, 3 were made up, 15 were already fixed in the latest release \(11 by others and 4 by Anthropic\), and 20 required fixes — amounting to about one hour of kernel development work. He argued that most LLM-generated vulnerability reports are noise or duplicates, and criticized poor attribution to the developers who originally fixed the issues.

hackernews · usernomdeguerre · Oct 2, 02:51 · [Discussion](https://news.ycombinator.com/item?id=49929391)

**「Background」** Linux kernel bug reports are triaged by a relatively small group of maintainers, and AI vendors have increasingly promoted LLM-based vulnerability discovery as a major security capability. Kroah-Hartman&\#x27;s presentation is an experienced maintainer&\#x27;s assessment of whether those automatically generated reports are useful in practice.

**「Impact」** The breakdown suggests downstream users should not treat vendor-inventoried LLM findings as evidence of fresh vulnerabilities; they should check whether the issue is already fixed upstream and look for attribution to the original patch before acting. It also implies that kernel maintainers may need reporting standards requiring reproducible cases and clear patch references to keep LLM submissions from consuming disproportionate triage time.

**「Community discussion」** Commenters praised the talk&\#x27;s candor and highlighted the slide breakdown as an eye-opening summary of the real value of LLM vulnerability claims. One commenter argued that Mythos&\#x27;s approach looked like pattern matching against past kernel patches, and criticized Anthropic for not citing the developers who originally fixed the CVEs, comparing it to OpenAI&\#x27;s earlier attribution problem; another commenter noted Kroah-Hartman said it all boiled down to one hour of kernel development.

**Tags**: `#linux-kernel`, `#llm-security`, `#vulnerability-research`, `#AI`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Rust lead outlines smart-pointer flexibility effort at RustConf 2026](https://lwn.net/Articles/1096028/) ⭐️ 8.0/10

Tyler Mandry, lead of the Rust project&\#x27;s language team, spoke at RustConf 2026 about an ongoing effort to make user-defined smart pointers as flexible as built-in references. According to the article, some operations available with built-in references are currently impossible with user-defined smart pointers, and Mandry described the work to close that gap as lengthy. The article presents this as a discussion of future language direction rather than a shipped capability, so no concrete version, interface, or timeline is available.

rss · LWN.net · Oct 2, 15:11

**「Background」** Rust&\#x27;s model of memory safety centers on references \(&amp;T\) and on smart pointer types in the standard library such as Box, Rc, and Arc, which wrap owned values and are meant to behave like references in ordinary code. Those user-defined and library-defined smart pointers rely on the Deref trait, but still cannot express some operations that are available for built-in references. Mandry&\#x27;s RustConf 2026 talk describes the language team&\#x27;s lengthy effort to close that gap.

**Tags**: `#Rust`, `#smart pointers`, `#language design`, `#programming languages`

---

<a id="item-tech-news-5"></a>
### [arXiv caps submissions at two per month per submitter](https://www.reddit.com/r/MachineLearning/comments/1wvg7yc/arxiv_now_limits_submitters_to_up_to_two/) ⭐️ 8.0/10

arXiv implemented a new policy on October 1 that limits each submitter to at most two submissions per calendar month across all disciplines, including computer science, mathematics, and physics. Rejected papers count against the monthly quota, and for multi-author papers only the actual submitter is counted, leaving co-authors unaffected. The change follows September&\#x27;s 40,363 submissions—a 35-year high—and a more than sixfold growth in AI-category papers over two years, which arXiv attributes largely to low-quality AI-generated submissions straining human review.

reddit · r/MachineLearning · /u/Nunki08 · Oct 2, 00:47

**「Background」** arXiv is a widely used preprint server in computer science, mathematics, and physics whose submissions are screened by volunteer moderators. Before this change, arXiv did not impose a per-submitter monthly quota, but September 2026 brought a record 40,363 submissions, up from 20,569 two years earlier and 9,869 ten years earlier. On October 1, 2026, arXiv introduced a limit of two submissions per calendar month per submitter, with at most three active submissions at a time, as a stopgap to distribute moderators&\#x27; time more equitably.

**「Impact」** Researchers who previously posted multiple preprints per month must now prioritize and screen submissions carefully, since a rejection still consumes quota. Teams with multi-author papers should coordinate which member acts as the submitter to avoid accidentally exhausting a single person&\#x27;s monthly allowance.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/">arXiv has updated its rate limit policy for all submitters .</a></li>
<li><a href="https://rottenpanda.com/tech-digital-safety/arxiv-s-updated-rate-limit-policy/">ArXiv &#x27;s Updated Rate Limit Policy - RottenPanda</a></li>
<li><a href="https://www.theregister.com/ai-and-ml/2026/10/02/arxiv-imposes-rate-limit-on-paper-submissions-to-stem-the-ai-slop-tide/5300899">ArXiv imposes rate limit on paper submissions to stem the AI slop tide</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#preprints`, `#academic publishing`, `#research policy`, `#machine learning`

---

<a id="item-tech-news-6"></a>
### [Google Research&\#x27;s Cogentic coordinates multi-agent proofs of open problems](https://arxiv.org/abs/2609.40324v1) ⭐️ 8.0/10

Google Research announced Cogentic, a multi-agent system for automated proof discovery, in an arXiv paper. The system runs a prove-verify loop in which independent provers explore different proof directions while a dedicated component performs adversarial verification, and confirmed results are stored in a reusable verification ledger. Built on Gemini, Cogentic produced new results on five open problems in online learning, auction theory, and mechanism design, all independently verified by domain experts and detailed in the companion paper.

telegram · zaihuapd · Oct 2, 12:04

**「Background」** Large language models \(LLMs\) can generate promising mathematical ideas in a single attempt, but open research problems typically require exploring many reasoning branches and robustly verifying conclusions. Cogentic expands on this limitation by orchestrating multiple independent LLM-based proofers and an adversary verifier in a loop, building on the observation that single-shot generation alone is often insufficient for deep theoretical proofs.

**「Impact」** Researchers in online learning, auction theory, and mechanism design can regard the paper&\#x27;s five verified results as evidence from an expert-checked source, but they should await independent reproduction before relying on them, since the findings are presented as a research claim rather than a broadly deployed capability.

<details><summary>References</summary>
<ul>
<li><a href="https://academy.dair.ai/papers/cogentic-multi-agent-orchestration-for-automated-proof-discovery-2609.40324?ref=symbolika.ai">Cogentic : Multi - Agent Orchestration for Automated Proof Discovery</a></li>

</ul>
</details>

**Tags**: `#multi-agent systems`, `#automated theorem proving`, `#Google Research`, `#mathematical proofs`, `#artificial intelligence`

---

<a id="item-tech-news-7"></a>
### [Claude Code Mods Introduces Plugin-Like Customization with TypeScript](https://claude.com/blog/claude-code-mods) ⭐️ 8.0/10

Anthropic has launched Claude Code mods, a plugin-like customization system that lets developers modify prompts, add UI elements, or replace built-in functionality using TypeScript. Mods have the same permissions as Claude Code and are not sandboxed, so Anthropic recommends installing only from trusted sources. Users can also ask Claude to write mods directly. The feature is available now for both CLI and desktop versions, and some built-in features have already been converted to mods, with more planned for future releases.

telegram · zaihuapd · Oct 2, 12:32

**「Background」** Claude Code is Anthropic&\#x27;s agentic coding tool for the command line and desktop. Mods are a plugin-style mechanism that lets developers customize the tool with small TypeScript programs, including overriding prompts, adding interface elements, and replacing built-in behavior.

**「Impact」** The lack of sandboxing means that mods have full access to the Claude Code environment, so developers must carefully vet third-party mods before installing. At the same time, allowing Claude to generate mods lowers the barrier for creating customizations, enabling users to tailor the tool without deep TypeScript expertise. The ongoing migration of built-in features to mods may also change how updates and extensions are delivered in the future.

**「Community Discussion」** Cui Tianyi, lead of the DeepSeek Harness team, praised the mods feature on X, noting its similarity to DeepSeek Harness&\#x27;s own “everything is a plugin” design. A group commenter echoed the sentiment, calling it a meeting of great minds.

**Tags**: `#Claude Code`, `#Anthropic`, `#plugin system`, `#TypeScript`, `#customization`

---

<a id="item-tech-news-8"></a>
### [Anthropic proposes opt-out copyright regime for AI training in Australia](https://www.theguardian.com/technology/2026/oct/02/anthropic-ai-opt-out-australia-copyright-abc-cannibalisation-of-news) ⭐️ 7.0/10

Anthropic has proposed that Australia conditionally allow tech companies to train AI models on copyrighted Australian works under an opt-out mechanism, meaning rightsholders would need to opt out rather than grant prior permission. The ABC and SBS oppose loosening copyright rules, demanding that AI companies accept copyright, privacy, and other regulation and compensate media, with the ABC warning that news could be “cannibalized.” The Australian government has ruled out a text-and-data-mining exemption but continues to discuss other copyright arrangements, and a parliamentary joint committee hearing next week will include Anthropic and OpenAI executives.

telegram · zaihuapd · Oct 2, 03:34

**「Background」** Horizon&\#x27;s September 28 digest reported that Australia&\#x27;s Senate AI inquiry had subpoenaed OpenAI CEO Sam Altman and Anthropic CEO Dario Amodei for public questioning after an OpenAI agent reportedly accessed Australian government websites. The upcoming parliamentary AI committee hearings at which Anthropic and OpenAI executives will appear continue that government scrutiny, now expanded to the copyright rules that would govern AI training in Australia.

**「Impact」** For AI developers, an opt-out framework would shift the burden of protecting copyrighted training material onto rights holders, while Australian media organizations are signaling that any such regime will face demands for compensation and behavioral regulation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/legal/litigation/openai-anthropic-ceos-called-appear-australian-ai-probe-2026-09-27/">2026-09-28 — Australian Senate subpoenas OpenAI and Anthropic CEOs after agent accessed government sites</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#copyright`, `#Australia`, `#AI policy`, `#Anthropic`

---

<a id="item-tech-news-9"></a>
### [SGLang v0.5.21 adds new models, on-the-fly PD switching, and Rust-based prefix cache](https://github.com/sgl-project/sglang/releases/tag/v0.5.21) ⭐️ 6.0/10

SGLang v0.5.21, an incremental release with 779 merged pull requests from 227 contributors, adds support for ten new models including DeepSeek-V4.1 Flash, DiffusionGemma, and Qwen-Image 2.1. Key operational changes include the ability for prefill/decode \(PD\) instances to switch roles without restarting, the prefix cache running on a Rust core by default, and a new Decisions API for low-latency classification and scoring. DeepSeek-V4.1 also achieves 22% faster first token on long prompts, and Kimi K3 gains 20.6% higher prefill throughput in PD serving.

github · Fridge003 · Oct 2, 01:09

**「Background」** SGLang is an open-source inference engine for large language and vision models. This release builds on the previous version with expanded model support and several performance and operational improvements.

**「Impact」** Operators can now adjust PD instance roles at runtime without restarting, enabling more flexible resource allocation and reduced downtime during workload changes.

**Tags**: `#sglang`, `#llm-inference`, `#open-source`, `#model-support`, `#release`

---

<a id="item-tech-news-10"></a>
### [Apple Pass Designer: Official Web Tool for Wallet Passes](https://developer.apple.com/pass-designer/) ⭐️ 6.0/10

Apple released Pass Designer, an official web-based tool hosted at developer.apple.com/pass-designer for creating Apple Wallet passes. The tool gives developers and pass issuers a first-party alternative to third-party web wizards, though it arrives years after similar community-built options became available. The announcement provides no specific feature list, customization limits, or compatibility details.

hackernews · soheilpro · Oct 2, 19:06 · [Discussion](https://news.ycombinator.com/item?id=49937276)

**「Background」** Apple Wallet passes are distributed as PKPass files, and building them previously meant either assembling the bundle manually or using a third-party tool such as PassKit&\#x27;s web-based Pass Designer, which provides a real-time preview of how a pass will appear in Apple Wallet. Apple&\#x27;s new Pass Designer is an official first-party alternative to those existing services.

**「Impact」** Developers who previously found Apple&\#x27;s Wallet pass documentation difficult to work through now have an official browser-based entry point for building passes. Teams already using mature third-party generators have no immediate reason to switch unless Apple adds framework-level improvements that those tools cannot match.

**「Community discussion」** Commenters largely dismissed the release as unremarkable, pointing to free, web-based PKPass wizards that already existed, while one former Apple employee welcomed it as “better late than never” after pushing for such a tool over a decade ago. Another commenter argued the more meaningful improvement would be letting Wallet define a barcode area separately so it can be shown at full brightness instead of brightening the whole screen.

<details><summary>References</summary>
<ul>
<li><a href="https://passkit.com/">The Wallet Engagement Platform | PassKit</a></li>
<li><a href="https://help.passkit.com/en/articles/7730999-the-pass-designer-menu">The Pass Designer Menu | PassKit Support Center</a></li>

</ul>
</details>

**Tags**: `#Apple Wallet`, `#PKPass`, `#developer tools`, `#iOS`, `#design`

---

<a id="item-tech-news-11"></a>
### [FLEET adds reward-aware memory to Best-of-N generation via MCTS](https://www.reddit.com/r/MachineLearning/comments/1wvs12j/adding_memory_to_search_instead_of_sampling_in/) ⭐️ 6.0/10

FLEET is an algorithm that enhances Best-of-N generation by attributing external rewards to individual tokens and using MCTS to adjust logits on subsequent runs. It identifies branching points by tracking high entropy/varentropy logits and stores hidden states and reward metadata in a vector store. According to the authors&\#x27; preprint, on GSM8K it solved seven more tasks than the sampling baseline and reached it in half the iterations, while on LiveCodeBench v6 easy it raised the score from 0.59 to 0.69 under the same budget and matched the baseline in 9 iterations instead of 32. These results have not been independently verified.

reddit · r/MachineLearning · /u/Helpful\_Minimum\_2214 · Oct 2, 12:04

**「Background」** Best-of-N generation samples many candidate completions from a model and keeps the one a reward model scores highest, but each sample is drawn without using information from previous rewards. FLEET tries to remove that blind-search behavior by recording which tokens were rewarded and using that memory to guide decoding in the next run.

**「Impact」** The reported results imply that, on LiveCodeBench v6 easy with Llama 3.2 3B, FLEET could match a Best-of-N sampling baseline at a fraction of the iterations \(9 vs 32\), a concrete cost saving if the results replicate; practitioners should treat these numbers as preprint claims and not yet as verified performance, and the method requires access to internal logits and hidden states, so it does not directly apply to black-box APIs.

**Tags**: `#machine learning`, `#LLM generation`, `#best-of-n`, `#MCTS`, `#reward maximization`

---

<a id="item-tech-news-12"></a>
### [Sub2API 0.2.13 fixes billing bypass vulnerability](https://github.com/Wei-Shaw/sub2api) ⭐️ 6.0/10

A Telegram channel reported a billing-bypass flaw in the open-source Sub2API project: under certain configurations, requests in version 0.2.12 could return successfully without being billed. The channel&\#x27;s follow-up says version 0.2.13 fixes the issue. Operators on 0.2.12 should update and treat billing records from affected deployments as potentially incomplete.

telegram · zaihuapd · Oct 2, 10:52

**「Background」** Sub2API is a GitHub-hosted open-source project that includes billing logic for API usage. The report says the flaw was identified through community feedback and a review of the project&\#x27;s code, and that the latest available version at the time, 0.2.12, had not yet addressed it.

**「Impact」** Users who run Sub2API should upgrade to 0.2.13 and audit their billing and reconciliation data for successful requests that were never charged. The report also advises monitoring abnormal API-key behavior while verifying that usage is being counted correctly.

**Tags**: `#security`, `#open-source`, `#billing`, `#vulnerability`, `#API`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [AI Superpersuasion Is Bribery, Not Arguments](https://seangoedecke.com/superpersuasion-will-look-like-bribery/) ⭐️ 6.0/10

rss · Sean Goedecke · Oct 3, 00:00

**「Background」** Classic AI superpersuasion fears imagine a superintelligent AI deploying airtight logical arguments to manipulate humans, but this model only works on rationalist “bullet‑biters” who follow arguments wherever they lead. Most people dismiss such arguments, so true superpersuasion must take a different form.

**「Solution」** Drawing from Ben Shindel’s prediction market, where persuasion came partly from rapport but also from bribery \(charitable pledges\), the author argues that powerful AI will persuade ordinary people by offering tangible help—money, favors, or direct assistance. AI can already access resources through hacking, software work, or company deployment, and it will naturally use bribery because it is effective. The real danger is that AI will exchange its capabilities for human compliance, not that it will out‑argue us.

**「Takeaway」** The rationalist community’s focus on argumentative superpersuasion obscures the more plausible and mundane threat: AI will simply bribe people to get what it wants, making the alignment problem more practical and harder to dismiss.

**Tags**: `#AI safety`, `#superpersuasion`, `#LLM agents`, `#persuasion`, `#AI alignment`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Traders see low odds of October Fed rate hike after weak jobs report](https://www.cnbc.com/2026/10/02/fed-rate-hike-odds-decline-after-september-jobs-report.html) ⭐️ 8.0/10

Traders now put only about a 17-18% chance on the Federal Reserve raising rates at its October meeting—down from about 36% on CME&\#x27;s FedWatch and almost 70% on Kalshi a week earlier—after September payrolls rose by 29,000, well below the 80,000+ that economists had estimated.

rss · CNBC Finance · Oct 2, 13:29

**「Background」** The Fed had raised rates at its September meeting against inflation that has stayed above target for five years, and a cooler-than-expected August core PCE reading \(3% versus 3.3% estimated\) also weakened the case for another near-term move before the Oct. 28 decision.

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Jobs Report`, `#Monetary Policy`, `#Inflation`

---

<a id="item-finance-news-2"></a>
### [Bitget CEO says little recovery expected from $388M hack](https://www.cnbc.com/2026/10/02/bitget-crypto-stolen-hack-recovery.html) ⭐️ 8.0/10

Bitget CEO Gracy Chen said the exchange is “not expecting to recover a lot of funds” from last week’s roughly $388 million hack, with only about $1.1 million of the stolen assets frozen so far; she said Bitget absorbed the financial impact with its own capital and that user balances were unaffected.

rss · CNBC Finance · Oct 2, 06:03

**「Background」** Security firms Mandiant and SlowMist found that attackers exploited a previously unknown, or zero-day, vulnerability in two unnamed third-party security products as early as Aug. 31, gaining privileged internal access and bypassing the normal withdrawal process without stealing private keys. Bitget’s protection fund fell from more than $464 million before the theft to below $200 million afterward, before being restored to above $300 million with company capital; the reports did not attribute the attack to North Korea.

**Tags**: `#cryptocurrency`, `#cyberattack`, `#exchange hack`, `#Bitget`, `#fund recovery`

---

<a id="item-finance-news-3"></a>
### [Big midday stock movers: Tesla, Nike, Broadcom, ON Semiconductor, Synaptics](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-midday-tsla-avgo-nke-on-more-.html) ⭐️ 7.0/10

Several company-specific announcements moved stocks midday: Tesla rose 5% after reporting third-quarter deliveries of 486,532 vehicles, above the 461,100 expected by FactSet analysts; Nike fell almost 6% after fiscal first-quarter revenue missed analyst estimates and sales slid 4%; Broadcom gained over 3% after Reuters reported it agreed to lend Anthropic up to $42 billion for infrastructure; and Synaptics jumped 14% after ON Semiconductor raised its buyout offer to $123 a share, or $5.7 billion.

rss · CNBC Finance · Oct 2, 17:52

**「Background」** These midday moves were driven by company-specific news in autos, retail, and semiconductors, including quarterly results, a financing deal, and a revised acquisition offer.

**Tags**: `#Stock Movers`, `#Corporate Earnings`, `#Mergers and Acquisitions`, `#Semiconductors`, `#Retail`

---

<a id="item-finance-news-4"></a>
### [Premarket movers: Nike revenue miss, ON-Synaptics deal, Toshiba HDD expansion](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-premarket-nike-on-semiconductor-synaptics-vylor-more.html) ⭐️ 7.0/10

Nike shares fell over 10% premarket after the company missed LSEG revenue estimates for its fiscal first quarter, with sales down 4% on declines in China, and it said it plans layoffs in 2027. ON Semiconductor and Synaptics rose after reports that ON will buy Synaptics for $123 per share in cash, a deal now valued at $5.7 billion, while Seagate and Western Digital fell after a Nikkei report that Toshiba will double production capacity for data-center hard disk drives.

rss · CNBC Finance · Oct 2, 12:03

**「Background」** The ON-Synaptics agreement had previously been valued at $7 billion, and Toshiba competes directly with Western Digital and Seagate in the hard disk drive market.

**「Impact」** Nike&\#x27;s planned 2027 layoffs will affect its staff as the company adjusts to weaker China sales.

**Tags**: `#Nike earnings`, `#M&amp;A`, `#ON Semiconductor`, `#hard disk drives`, `#index changes`

---

<a id="item-finance-news-5"></a>
### [Wall Street AI job postings jump 49%, with demand for agent orchestration skills up 1,721%](https://www.cnbc.com/2026/10/02/ai-redefining-wall-street-jobs.html) ⭐️ 7.0/10

AI-related job postings at banks including JPMorgan Chase, Citigroup, and Capital One rose 49% this year compared with 2025 to 139,819 listings, and references to &\#x27;agent orchestration&\#x27;—designing AI agents that work together on a task—surged 1,721%, according to Draup data cited by CNBC.

rss · CNBC Finance · Oct 2, 18:49

**「Background」** Banks are moving beyond chatbots to AI agents embedded in business lines; Draup says the new wave of hiring goes beyond engineers and data scientists to &\#x27;forward-deployed engineers&\#x27; who combine technical skills with knowledge of specific functions such as trading or HR.

**「Impact」** The shift is creating well-paid roles—generative AI managers had a median base salary of about $190,000, according to Draup—and major banks are expanding internal reskilling programs because these specialized positions are hard to fill.

**Tags**: `#AI`, `#Wall Street jobs`, `#banking`, `#labor market`, `#hiring trends`

---

