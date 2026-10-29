# Horizon Daily - 2026-10-29

> From 49 items, 26 important content pieces were selected

---

**Technology News**
1. [Fingerprinting Script Uses Obfuscation and Honeypot Tactics Against AI Crawlers](#item-tech-news-1) ⭐️ 8.0/10
2. [Apple Announces MacBook Pro with ProLED XDR Display and Touch](#item-tech-news-2) ⭐️ 8.0/10
3. [Apple&\#x27;s system git still trusts compromised eMudhra certificates](#item-tech-news-3) ⭐️ 8.0/10
4. [Zero-training null-space PCA lifts EmbeddingGemma-2 to \#1 on MAEB](#item-tech-news-4) ⭐️ 8.0/10
5. [Anthropic hiring manager stops coding interviews, saying Claude outperforms candidates](#item-tech-news-5) ⭐️ 8.0/10
6. [Google&\#x27;s Sleep Framework Helps LLMs Retain Knowledge in Continual Learning](#item-tech-news-6) ⭐️ 8.0/10
7. [Google introduces Gemini 4 Carbon with cybersecurity focus and introductory pricing](#item-tech-news-7) ⭐️ 8.0/10
8. [Kentucky humanist granted first religious AI-use exemption](#item-tech-news-8) ⭐️ 7.0/10
9. [October 2026: vibe coding games hit reliability inflection point](#item-tech-news-9) ⭐️ 7.0/10
10. [sched\_ext microconference covers priority inversion, paravirtual scheduling](#item-tech-news-10) ⭐️ 7.0/10
11. [Campaign to bring LLM-written Nordstjernen browser into Debian and Arch draws scrutiny](#item-tech-news-11) ⭐️ 7.0/10
12. [VentureBeat survey: enterprise GPUs idle half the time, yet firms plan new buys](#item-tech-news-12) ⭐️ 7.0/10
13. [CXMT plans limited HBM3E production with low yields](#item-tech-news-13) ⭐️ 7.0/10
14. [CNC Stone Carving Helps Build a Modern Gothic Monastery](#item-tech-news-14) ⭐️ 6.0/10
15. [Dayjob: Tax benchmark tests AI agents on 50 tax assignments](#item-tech-news-15) ⭐️ 6.0/10
16. [Emacs at 50: A Retrospective on an Enduring Editor](#item-tech-news-16) ⭐️ 6.0/10
17. [Alleged archive.today redirects draw caution, but remain unverified](#item-tech-news-17) ⭐️ 6.0/10
18. [Ted Sanders: model size drives LLM performance; version numbers encode release order](#item-tech-news-18) ⭐️ 6.0/10
19. [GitHub Octoverse 2026: Agentic Development Triples Merged PRs and Commits](#item-tech-news-19) ⭐️ 6.0/10
20. [Amazon: AI tooling gaps are findings, not failings](#item-tech-news-20) ⭐️ 6.0/10
21. [Redox OS completes io\_uring-like ring buffer support and API](#item-tech-news-21) ⭐️ 6.0/10
22. [MIDA Benchmark Shows Multimodal LLMs Fail Werewolf Deception Detection](#item-tech-news-22) ⭐️ 6.0/10
23. [Study: Fixed Feedback Equals Self-Critiques in Hindsight Self-Distillation](#item-tech-news-23) ⭐️ 6.0/10
24. [Cocktail-party CAPTCHA test: humans beat ASR but not enough](#item-tech-news-24) ⭐️ 6.0/10
25. [Discord Public Server Conversations Will Become Web-Searchable](#item-tech-news-25) ⭐️ 6.0/10
26. [South Korea fines Apple $15.5M and Google $32M over app store payment rules](#item-tech-news-26) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Fingerprinting Script Uses Obfuscation and Honeypot Tactics Against AI Crawlers](https://nullpt.rs/fingerprinting-bioweapons) ⭐️ 8.0/10

A technical deep-dive describes an obfuscated fingerprinting script that appears to combine dynamic JavaScript obfuscation with honeypot traps to lure AI crawlers and detect or counter them. The write-up, published October 28, 2026, is positioned as an investigation of an escalating anti-LLM scraping arms race rather than a demonstrated vulnerability or shipped product.

hackernews · hazebooth · Oct 28, 17:13 · [Discussion](https://news.ycombinator.com/item?id=50276998)

**「Background」** Anti-crawler defenses have long distinguished human browsers from automated agents by inspecting client signals, but the recent wave of LLM-powered crawlers has pushed some site operators to hide that logic in obfuscated JavaScript. A common tactic is to serve honeypot content designed to lure scrapers, then fingerprint the request and drop the crawl attempt when the target looks like an AI bot. This post investigates one such script and asks why a fingerprinting routine would carry bioweapons-related strings.

**「Community discussion」** Commenters framed the finding as an escalating &quot;arms race,&quot; with ghm2199 asking whether LLMs are effectively tuning crawl attempts to defeat obfuscation. jacquesm added a reported real-world experience where a similar watermark caused a recipient&\#x27;s security system to quarantine an emailed document until manual review.

**Tags**: `#anti-crawler`, `#LLM bots`, `#obfuscation`, `#fingerprinting`, `#web security`

---

<a id="item-tech-news-2"></a>
### [Apple Announces MacBook Pro with ProLED XDR Display and Touch](https://www.apple.com/macbook-pro/proled-xdr-display/) ⭐️ 8.0/10

Apple announced a new MacBook Pro lineup featuring a ProLED XDR display and touch input, according to the Apple newsroom page shared on Hacker News. The announcement is an Apple claim; the shared item does not include shipping dates, pricing, or independent measurements of the new display or redesigned hardware.

hackernews · etothet · Oct 28, 17:10 · [Discussion](https://news.ycombinator.com/item?id=50276940)

**「Background」** Horizon&\#x27;s October 26 digest reported Bloomberg&\#x27;s forecast that Apple would unveil its first touchscreen MacBook Pro that week, with touch input, an OLED display, Dynamic Island, and 14- and 16-inch sizes priced above the then-current $2,499 starting point. Apple&\#x27;s October 28 newsroom announcement confirms the device as the MacBook Pro with PROLED XDR display, a tandem OLED panel, with pre-orders starting at $2,899 for an M5 Pro configuration and shipping on November 6.

**「Community discussion」** Commenters split over the touch addition: one argues that macOS UI widgets are too small for finger input and will generate usability complaints, while another highlights the reported weight reduction of about 15% \(14-inch from 3.5 lb to 3.0 lb; 16-inch from 4.7 lb to 4.0 lb\) as the more significant change. Others question whether laptop touchscreens are useful at all and express concern about fingerprints on the display.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/newsletters/2026-10-25/apple-to-unveil-touch-screen-macbook-pro-executive-promotions-in-box-checker">2026-10-26 — Apple to Unveil First Touchscreen MacBook Pro With OLED, Dynamic Island</a></li>
<li><a href="https://www.apple.com/newsroom/2026/10/apple-unveils-groundbreaking-macbook-pro-with-proled-xdr-display/">Apple unveils groundbreaking MacBook Pro with PROLED XDR Display</a></li>
<li><a href="https://www.thenationalnews.com/future/technology/2026/10/28/macbook-pro-touch-glowing-apple/">Apple introduces touchscreen MacBook Pro with PROLED XDR display</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#MacBook Pro`, `#hardware`, `#display technology`, `#touchscreen`

---

<a id="item-tech-news-3"></a>
### [Apple&\#x27;s system git still trusts compromised eMudhra certificates](https://emudhra.we-have-a-problem.com/apple.html) ⭐️ 8.0/10

Apple&\#x27;s system git on macOS still trusts the compromised eMudhra certificates, so affected developers must manually remove them from the trust chain. Apple warns that future macOS updates may revert that manual mitigation and re-expose the vulnerability, and commenters say the problem is not limited to git alone.

hackernews · galadran · Oct 28, 11:03 · [Discussion](https://news.ycombinator.com/item?id=50271640)

**「Background」** Several eMudhra intermediate certificate authorities had their keys compromised, and eMudhra and Sectigo revoked the affected certificates. Apple&\#x27;s support page explains that many command-line tools bundled with macOS or the Xcode Command Line Tools—including git, curl, python3, ruby, perl, and openssl—check certificates against /etc/ssl/cert.pem, and for certificates chaining to a root in that file, these tools do not consult Apple&\#x27;s blocklist or revocation status. Security researcher Dennis Jackson&\#x27;s site documented that Apple was notified about the compromise on October 17, 2026, and that the development tools still trusted the compromised certificates on October 28.

**「Impact」** Developers using Apple&\#x27;s bundled git should apply Apple&\#x27;s recommended certificate patch and re-check their trust settings after each macOS update, because the mitigation has already been reverted by an OS update at least once.

**「Community discussion」** Commenters noted the issue affects any utility that relies on macOS trust settings, not just git, and questioned why Apple has not removed the revoked certificates from /etc/ssl in a system update. One user speculated without evidence that the weak key generation may have been intentional, but other commenters focused on the need for a reliable fix.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/149555">About the compromised eMudhra intermediate CAs - Apple Support</a></li>
<li><a href="https://github.com/Steff81/apple_eMudhra_removeScript">GitHub - Steff81/apple_eMudhra_removeScript: Removes and ...</a></li>
<li><a href="https://elsolitario.org/en/2026/10/28/macos-27-2-reverts-manual-patch-against-emudhra-report/">Compromised eMudhra Certificates: What Apple Is Doing</a></li>

</ul>
</details>

**Tags**: `#security`, `#certificates`, `#macOS`, `#git`, `#PKI`

---

<a id="item-tech-news-4"></a>
### [Zero-training null-space PCA lifts EmbeddingGemma-2 to \#1 on MAEB](https://www.reddit.com/r/MachineLearning/comments/1xho7pr/r_taking_embeddinggemma2_577m_from_rank_26_to_1/) ⭐️ 8.0/10

With no additional training, researchers injected PCA-reduced embeddings from the 2nd and 6th Conformer layers of google/embeddinggemma-2 \(577M\) into the 256-dimensional null space of the model&\#x27;s 768x512 terminal projection, preserving text embeddings bit-for-bit. On the MAEB audio benchmark, the macro score rose from 49.3% to 54.4%, moving the model from rank \#26 to \#1 on audio-only MAEB and ahead of larger 8B-9B multimodal models. PCA was fitted on 1,400 clips from four external audio datasets, with no MAEB/MSEB data. The trade-off is that fixed acoustic features hurt spoken-intent tasks—SIBFLEURS drops from 57.2% to 21.3%—and the 512/256/128 Matryoshka truncation options no longer apply.

reddit · r/MachineLearning · /u/JeanMichelRanu · Oct 28, 13:34

**「Background」** Google released EmbeddingGemma 2 in early October 2026 as an open-weight multimodal embedding model that maps text, images, video, and audio into a shared vector space for on-device retrieval, according to Horizon&\#x27;s October 8 digest. An earlier October 14 experiment already showed that this shared text/audio space can be exploited to repurpose the model, which the new PCA null-space method builds on.

**「Impact」** Practitioners using text-aligned audio encoders can recover paralinguistic signal without fine-tuning—gender clustering rises from 0.05% to 63.1%, emotion from 19.7% to 40.2%, and environmental-sound tasks from 38.8% to 56.3%—but should avoid this null-space injection when spoken intent or topic classification matters, or when embedding truncation is required, because orthogonality depends on keeping all 768 dimensions.

<details><summary>References</summary>
<ul>
<li><a href="https://eg2.haku.sh/">2026-10-14 — EmbeddingGemma 2 turned into an experimental local speech-to-text model</a></li>
<li><a href="https://developers.googleblog.com/google-ai-edge-with-embeddinggemma-2/">2026-10-08 — Google DeepMind launches EmbeddingGemma 2 for on-device multimodal retrieval</a></li>

</ul>
</details>

**Tags**: `#audio embeddings`, `#MAEB`, `#null space`, `#PCA`, `#representation learning`

---

<a id="item-tech-news-5"></a>
### [Anthropic hiring manager stops coding interviews, saying Claude outperforms candidates](https://felixrieseberg.com/hunger-beats-tenure-advice-for-junior-engineers/) ⭐️ 8.0/10

Anthropic hiring manager Felix Rieseberg says he stopped using coding problems in interviews this month because Claude already solves them better than candidates, making coding tests ineffective as a screening filter. He argues that falling execution costs reduce the importance of seniority and advises junior engineers to target business goals and build a single weekend prototype to gain support. He cites two junior engineers who prototyped Claude Code&\#x27;s GUI in a weekend; the first public version shipped about eight days later.

telegram · zaihuapd · Oct 28, 01:46

**「Background」** A conventional software engineering loop typically includes a live coding interview — a problem solved by writing working code in a fixed time — because writing code on demand is treated as the core skill of the job. That screen assumes unassisted code production is the main way features get built. AI coding tools now automate much of that production, which is the shift that prompted Anthropic&\#x27;s hiring manager to drop the coding screen from his interviews.

**「Impact」** For candidates, this points to one Anthropic team evaluating engineering skill through shipped prototypes and business outcomes instead of algorithm-style assessments, so junior engineers can compete by quickly demonstrating a working prototype rather than preparing for whiteboard coding.

**Tags**: `#Anthropic`, `#hiring practices`, `#AI-assisted development`, `#Claude`, `#software engineering`

---

<a id="item-tech-news-6"></a>
### [Google&\#x27;s Sleep Framework Helps LLMs Retain Knowledge in Continual Learning](https://research.google/blog/the-sleep-framework-a-new-way-for-llms-to-retain-knowledge-in-continual-learning/) ⭐️ 8.0/10

Google Research proposed the &quot;sleep framework,&quot; a continual-learning approach in which LLMs alternate between active interaction and offline consolidation to convert short-term context into long-term parameters and mitigate catastrophic forgetting. In reported tests, the framework outperformed baselines such as GPT-4 and supervised fine-tuning on a 10-million-token long-context task, continual translation, and math reasoning. These are research results, not an independently verified or shipped product capability.

telegram · zaihuapd · Oct 28, 01:46

**「Background」** Catastrophic forgetting is the failure of neural models, including large language models, to retain previously learned abilities when they are updated with new data. Continual learning research seeks training procedures that let LLMs preserve old knowledge while acquiring new capabilities, and the proposed sleep framework addresses this problem by adding an offline consolidation phase.

**「Impact」** For researchers addressing continual learning, the framework offers an offline consolidation phase as an alternative to replay or regularization-based methods, with reported gains on long-context and reasoning benchmarks. Practitioners should treat the results as preliminary until independent replication and evaluation across more tasks are available.

**Tags**: `#continual learning`, `#LLM`, `#catastrophic forgetting`, `#Google Research`, `#AI research`

---

<a id="item-tech-news-7"></a>
### [Google introduces Gemini 4 Carbon with cybersecurity focus and introductory pricing](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) ⭐️ 8.0/10

Google introduced Gemini 4 Carbon, a new frontier model aimed at long-horizon autonomous engineering, agentic work, and cybersecurity. Compared with its predecessor Argon, Google claims more than 2x improvement in secure code generation success, roughly 2x fewer unsupported claims, nearly 80% fewer high-severity misalignment alerts, and 88.2% on the SEC-bench Pro benchmark, though these are vendor-reported results rather than independent measurements. The model is initially available only to selected cybersecurity defenders and trusted partners, including US government pre-release testing, at introductory API pricing of $2 per million input tokens and $10 per million output tokens, matching Argon, with the price scheduled to double later before broader developer and consumer availability.

telegram · zaihuapd · Oct 28, 17:09

**「Background」** Gemini 4 Carbon is the successor to Gemini 4 Argon, the frontier model Google announced in early October 2026. Horizon&\#x27;s October 1 digest reported that Argon introduced agentic capabilities—including agents that migrate C/C++ codebases to Rust—but was not yet generally available; the October 14 digest reported Argon&\#x27;s eventual release to API users with early quality praise but public-access friction. Carbon builds on that lineage with a focus on long-horizon autonomous engineering and cybersecurity tasks.

**「Impact」** Developers should expect the Gemini 4 Carbon API price to double after the introductory phase, so early adoption is the only way to lock in the $2/$10-per-million-token rates, but most users cannot take advantage immediately because access is currently restricted to select partners and defenders.

**「Community discussion」** Several commenters expressed confusion about how to actually access Gemini 4 models, with one saying they were unsure how to use Gemini 4 Argon and another noting they had not realized Argon had become publicly available. Other commenters argued that showing benchmarks without a widespread release is less meaningful in a fast-moving market and suggested simpler, standardized model naming tiers.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">2026-10-01 — Google introduces Gemini 4 Argon with Rust migration agents</a></li>
<li><a href="https://deepmind.google/models/gemini/">2026-10-14 — Gemini 4 Argon draws early praise but access friction</a></li>

</ul>
</details>

**Tags**: `#google`, `#gemini`, `#ai-models`, `#cybersecurity`, `#agentic-ai`

---

<a id="item-tech-news-8"></a>
### [Kentucky humanist granted first religious AI-use exemption](https://religionnews.com/2026/10/26/in-a-first-a-humanist-granted-a-religious-exemption-from-using-ai/) ⭐️ 7.0/10

A Kentucky man has reportedly become the first person granted a religious exemption from using AI, with humanist beliefs recognized as the basis for the accommodation. The report describes the decision as a novel legal and cultural precedent for AI policy and employment law, though details about the employer and the specific terms of the exemption are not provided.

hackernews · danso · Oct 28, 13:41 · [Discussion](https://news.ycombinator.com/item?id=50273396)

**「Background」** The direct precedent for this accommodation was set earlier in 2026: in April, software engineer Erin Maus, a Unitarian Universalist, asked her employer for a religious exemption from using AI, citing environmental and ethical concerns, and the company granted it in mid-May. The Kentucky case follows that precedent but is framed as a first for humanism, with the American Humanist Association saying it is the first time a humanist received an AI exemption.

**「Impact」** For employers, the exemption creates a concrete precedent: workers can now point to a granted humanist AI accommodation when requesting not to use AI, and a reported U.S. software engineer separately won a Title VII religious accommodation from AI use. Because the Supreme Court has lowered the bar for what counts as a sincerely held religious practice, employers face a harder time denying similar requests without demonstrating undue hardship. HR teams that mandate AI tools should expect more opt-out requests and should prepare a clear accommodation process rather than treating AI refusal as automatically unreasonable.

**「Community discussion」** Commenters split over the significance: some welcomed the accommodation but questioned how courts would distinguish sincere faith-like beliefs from beliefs employers can reject, while another called it a non-story because the request was small and easy to accommodate. Other commenters framed the case as a possible sign of an emerging Amish-like lifestyle for AI refusers and urged legal protections for people who choose not to use AI.

<details><summary>References</summary>
<ul>
<li><a href="https://religionnews.com/2026/10/26/in-a-first-a-humanist-granted-a-religious-exemption-from-using-ai/">A Kentucky man becomes the first humanist granted religious ...</a></li>
<li><a href="https://www.linkedin.com/posts/maureen-pritchard-phd-106b7234_she-won-an-exemption-from-using-ai-at-her-activity-7469026315183009792-6_Sb">Unitarian Universalist Secures Religious Exemption from AI Use at...</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/now-religious-exemption-using-ai-200105422.html?guccounter=1">You Can Now Get a Religious Exemption From Using AI at Work</a></li>
<li><a href="https://www.linkedin.com/posts/alexisdufresne_erin-maus-secures-title-vii-ai-exemption-activity-7472699930638315520-KBeh">US Worker Wins Religious Exemption from AI Use at Work | LinkedIn</a></li>
<li><a href="https://www.troutman.com/insights/scotus-overturns-title-vii-precedent-lowering-bar-for-religious-accommodations/">SCOTUS Overturns Title VII Precedent , Lowering Bar for Religious ...</a></li>

</ul>
</details>

**Tags**: `#ai policy`, `#law`, `#humanism`, `#society`, `#ethics`

---

<a id="item-tech-news-9"></a>
### [October 2026: vibe coding games hit reliability inflection point](https://simonwillison.net/2026/Oct/28/vibe-game-development/) ⭐️ 7.0/10

In an October 28, 2026 post, Simon Willison argues that AI-assisted &\#x27;vibe coding&\#x27; has reached an inflection point for computer games, with Claude Opus 5.5 producing playable, fun HTML and JavaScript browser games from natural-language prompts. He reports building four games this way, including Tree Appreciator, a spot-the-difference three.js game produced in a single shot, and Emberwick, a top-down fantasy RPG prototype. Willison notes that GPT-6 Astra can build a game but does not yet match Opus 5.5&\#x27;s &\#x27;sense of fun,&\#x27; and predicts OpenAI will close that gap by the end of the year. These are the author&\#x27;s evaluations rather than independent benchmarks.

rss · Simon Willison · Oct 28, 13:55

**「Background」** Horizon&\#x27;s September 28 digest covered Willison&\#x27;s argument that November 2025 was the first inflection point, when Claude Opus 4.5 and GPT-5.1 made coding agents reliable daily drivers for software engineers. The current article extends that thesis: October 2026 is a second inflection point, this time for &quot;vibe coding&quot; games — building in HTML and JavaScript with prompts and no code review — where the author says Claude Opus 5.5&\#x27;s 3D modeling, music generation, and game-design output finally makes games fun to play, unlike his earlier August experiments that looked like games but were not enjoyable.

**「Impact」** Developers using Claude Opus 5.5 can now prompt a playable, browser-based game without inspecting the code, and Willison&\#x27;s examples suggest specifying three.js in the request and iterating with prompts like &\#x27;make it a LOT more fun&\#x27; are effective ways to get polished 3D results.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/">2026-09-28 — Simon Willison&#x27;s 2026 LLM keynote: coding agents reached daily-use reliability</a></li>

</ul>
</details>

**Tags**: `#vibe coding`, `#AI coding agents`, `#game development`, `#AI-assisted software engineering`, `#Simon Willison`

---

<a id="item-tech-news-10"></a>
### [sched\_ext microconference covers priority inversion, paravirtual scheduling](https://lwn.net/Articles/1103426/) ⭐️ 7.0/10

The Linux Plumbers Conference&\#x27;s sched\_ext microconference, held in Prague, centered on three scheduler topics: priority inversion handling in sched\_ext \(lock-holder and lock-waiter preemption, time-slice extension, and proxy execution with BPF schedulers\), paravirtualized scheduling that lets host and guest schedulers cooperate with sched\_ext as the host-side policy engine, and device/topology-aware task placement using Intel HFI feedback, accelerator locality, and cache topology. The LPC blog report summarizes the discussions and does not announce any shipped code or final decisions.

rss · LWN.net · Oct 28, 22:11

**「Background」** sched\_ext allows CPU schedulers to be written as BPF programs that run in the kernel, and Horizon&\#x27;s October 19 digest reported that Linux 7.3, released this month, completed the sched\_ext subscheduler feature. The Linux Plumbers Conference microconference in Prague therefore discussed the next phase for BPF-based scheduling, which is already expanding beyond sched\_ext itself — Horizon&\#x27;s October 8 digest noted that the BPF-based LAVD scheduler has grown from gaming to server workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1097209/">2026-10-08 — LAVD scheduler grows from gaming to server workloads</a></li>
<li><a href="https://lwn.net/Articles/1101143/">2026-10-19 — Linux 7.3 kernel released with record commit count</a></li>

</ul>
</details>

**Tags**: `#linux-kernel`, `#sched\_ext`, `#BPF`, `#scheduling`, `#conference-report`

---

<a id="item-tech-news-11"></a>
### [Campaign to bring LLM-written Nordstjernen browser into Debian and Arch draws scrutiny](https://lwn.net/Articles/1102738/) ⭐️ 7.0/10

LWN reports on an active campaign to get Nordstjernen, an LLM-written open-source browser, packaged into Debian and Arch Linux. The push has raised questions about the project&\#x27;s development and security processes, in part because Linux browsers typically depend on the Blink, Gecko, or WebKit engines. Distribution maintainers and users are now weighing whether an LLM-generated browser should join the standard package set.

rss · LWN.net · Oct 28, 14:26

**「Background」** Nordstjernen is an independent open-source browser engine written from scratch in C, pitched as a GPL-3, JIT-free alternative to the Blink, Gecko, and WebKit engines behind most Linux browsers. In an earlier stage of this effort, its developer Andreas Røsdal filed a Debian intent-to-package request and Debian maintainers raised questions about the copyright status of the LLM-generated code — the same kind of scrutiny that now surrounds the campaign to get the browser into Debian and Arch Linux.

<details><summary>References</summary>
<ul>
<li><a href="https://freenode.net/article/debian-questions-copyright-of-llm-built-northstar-browser">Debian questions copyright of LLM -built Northstar browser · freenode</a></li>
<li><a href="https://nordstjernen.org/">Nordstjernen Web Browser</a></li>
<li><a href="https://github.com/nordstjernen-web/nordstjernen-browser">GitHub - nordstjernen -web/ nordstjernen - browser : Nordstjernen ...</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#open source`, `#web browsers`, `#LLM code generation`, `#software security`

---

<a id="item-tech-news-12"></a>
### [VentureBeat survey: enterprise GPUs idle half the time, yet firms plan new buys](https://venturebeat.com/infrastructure/ai-bubble-update-79-of-companies-say-their-gpus-sit-idle-at-least-half-the-time-yet-most-plan-new-ai-platforms) ⭐️ 7.0/10

A VentureBeat enterprise survey reports that 79% of companies have GPUs whose average utilization is below 50%, and 91% of AI infrastructure investments have never undergone a formal ROI audit by finance. Despite this, 70% of the low-utilization companies still plan to purchase and deploy new AI computing platforms within the next 12 months. The findings highlight a disconnect between continued enterprise AI buying and measurable returns.

telegram · zaihuapd · Oct 28, 02:37

**「Background」** Enterprise AI capacity decisions are occurring against a backdrop of tight GPU rental markets: Horizon&\#x27;s October 26 digest reported an a16z price index showing broad rental increases, including roughly +160% for H200 and +35% for H100 SXM by mid-October. The new VentureBeat survey adds an enterprise-side picture, showing that most GPU fleets sit idle and most AI investments have not undergone formal ROI audits even as many companies plan further AI platform deployments.

**「Impact」** Enterprises buying new AI platforms without formal financial review risk repeating the same underutilization, wasting capital on idle GPU capacity. Organizations should tie future AI infrastructure purchases to audited ROI and utilization targets before committing to additional deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/a16z/status/2113741008550990191">2026-10-26 — GPU Rental Prices Rise Broadly, Including Older A100, per a16z Index</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#GPU utilization`, `#enterprise AI`, `#ROI`, `#AI spending`

---

<a id="item-tech-news-13"></a>
### [CXMT plans limited HBM3E production with low yields](https://www.reuters.com/world/china/chinas-cxmt-start-advanced-ai-memory-production-despite-poor-yields-sources-say-2026-10-28/) ⭐️ 7.0/10

Two people with knowledge of the matter told Reuters that Chinese memory maker CXMT has sent HBM3E samples to several domestic AI chip designers and plans to begin limited production within the next two months, despite a yield of only 20–30%, far below SK Hynix’s roughly 70%. The company is proceeding because US export controls have left domestic AI memory in short supply; test results reportedly show performance closer to SK Hynix’s previous-generation HBM3, and CXMT’s expected price is higher than foreign equivalents.

telegram · zaihuapd · Oct 28, 06:19

**「Background」** HBM3E is the latest generation of high-bandwidth memory used in AI accelerators, and its supply is dominated by a small number of foreign manufacturers. US export controls have left Chinese AI chip designers with a severe shortage of such memory, which is why a domestic producer like CXMT attempting production—even at low yields—matters for the local supply chain.

**「Impact」** Domestic AI chip designers evaluating CXMT’s HBM3E gain a potential local supply option outside US export controls, but limited production, low yields, higher expected prices, and performance near HBM3 mean it will not immediately replace imported high-bandwidth memory; these samples should be treated as early, low-volume parts rather than committed volume supply.

**Tags**: `#HBM`, `#semiconductors`, `#AI hardware`, `#China`, `#memory`

---

<a id="item-tech-news-14"></a>
### [CNC Stone Carving Helps Build a Modern Gothic Monastery](https://carmelitegothic.com/cnc-stone-carving/) ⭐️ 6.0/10

An article on Carmelite Gothic describes how CNC stone carving is being used in the construction of a gothic-style monastery, pairing modern machining with traditional masonry. The piece frames the technology as part of a long history of sculptors seeking to automate repetitive work rather than as a break from handcraft.

hackernews · bschne · Oct 28, 14:38 · [Discussion](https://news.ycombinator.com/item?id=50274409)

**「Background」** The item concerns the New Mount Carmel Foundation, a community of monks in Wyoming building a gothic-style monastery with CNC stone-carving machinery. Earlier coverage, including a Modern Machine Shop article and an Arena Magazine feature, describes the project as combining multi-ton granite slabs with computer-programmed machine tools, a choice made partly because granite&\#x27;s hardness had historically made gothic detailing difficult to produce.

**「Community Discussion」** Commenters counter concerns that CNC removes human artistry by noting that sculptors have used grids, molds, casts, and pointing machines for centuries, and one reader points out that Sagrada Familia has combined CNC roughing with manual finishing since the early 1990s, which helped make its completion possible this year. Another commenter admires the monks&\#x27; broader project of saving money, buying mountain land, and building a medieval-style monastery in stone.

<details><summary>References</summary>
<ul>
<li><a href="https://newmountcarmelfoundation.org/the-chapel-carving-granite/">The Chapel: Carving Granite - New Mount Carmel Foundation</a></li>
<li><a href="https://newmountcarmelfoundation.org/monastery-stone-carving-article/">Monastery featured in Modern Machine Shop - New Mount Carmel ...</a></li>
<li><a href="https://arenamagazine.substack.com/p/wyomings-tech-savvy-monastery">Wyoming&#x27;s Tech-Savvy Monastery</a></li>

</ul>
</details>

**Tags**: `#CNC`, `#stone carving`, `#hardware`, `#manufacturing`, `#gothic architecture`

---

<a id="item-tech-news-15"></a>
### [Dayjob: Tax benchmark tests AI agents on 50 tax assignments](https://surgehq.ai/blog/dayjob-tax) ⭐️ 6.0/10

SurgeHQ has introduced Dayjob: Tax, a benchmark that evaluates AI agents on 50 professional tax assignments. The new evaluation targets real-world reliability for AI-assisted tax preparation rather than general LLM trivia, giving developers and taxpayers a concrete way to compare agent performance on tax work.

hackernews · landonxi · Oct 28, 15:46 · [Discussion](https://news.ycombinator.com/item?id=50275626)

**「Background」** Surge AI&\#x27;s DAYJOB benchmark series evaluates AI agents on realistic professional assignments, with earlier releases covering healthcare and finance. DAYJOB: Tax extends that work into tax preparation, compliance, and advisory services, using 50 environments across eight areas of tax practice and 1,789 workspace files such as PDFs, Excel workbooks, and handwritten receipts.

**「Impact」** Taxpayers who delegate preparation or review to AI agents should still independently verify figures before filing. One commenter reported that an accountant&\#x27;s draft they checked with Codex initially understated the refund by nearly $2,000 and placed items in the wrong fields, requiring multiple rounds of correction.

**「Community discussion」** Commenters reported mixed real-world experiences: one used Claude to review a draft return and found a genuinely useful error involving an incorrect exchange rate, while another found a $20,000 accountant mistake only after switching preparers. One reader also questioned whether the benchmark simply gives a general-purpose agent a document-filled workspace and an assignment, rather than testing a meaningful new capability.

<details><summary>References</summary>
<ul>
<li><a href="https://surgehq.ai/blog/dayjob-tax">DAYJOB: Tax — Benchmarking AI Agents on Professional Tax Work</a></li>
<li><a href="https://daily.dev/posts/dayjob-tax-evaluating-ai-agents-on-50-professional-tax-assignments-tknynvr2r">Dayjob: Tax – evaluating AI agents on 50 professional tax ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#benchmarking`, `#LLM evaluation`, `#tax software`

---

<a id="item-tech-news-16"></a>
### [Emacs at 50: A Retrospective on an Enduring Editor](https://www.technologyreview.com/2026/10/20/1145399/emacs-turns-50/) ⭐️ 6.0/10

MIT Technology Review published a retrospective marking Emacs&\#x27;s 50th anniversary and its continued role in software development. The piece is an anniversary retrospective rather than a new release or technical change, so it announces no version, availability, or compatibility updates. Its significance rests on the longevity of the project and the community response it drew.

hackernews · internet\_points · Oct 28, 13:25 · [Discussion](https://news.ycombinator.com/item?id=50273171)

**「Background」** Emacs is a family of extensible text editors that grew out of work at the MIT AI Lab in the 1970s, with GNU Emacs as its most widely used descendant. Its defining feature is deep extensibility: users configure the editor and write extensions in a Lisp-based scripting language, a design that has let it outlive several generations of competing editors. This anniversary retrospective reflects on that history rather than announcing a new release or technical change.

**「Community discussion」** Longtime users shared personal experience: jwr reported more than 30 years with Emacs and praised active maintenance and packages such as Magit, while RedCinnabar described using it across writing, teaching, and work. In contrast, marttt asked whether anyone deliberately keeps their Emacs setup lean, admitting the ecosystem&\#x27;s complexity drove them to simpler editors.

**Tags**: `#emacs`, `#open source`, `#software history`, `#editors`

---

<a id="item-tech-news-17"></a>
### [Alleged archive.today redirects draw caution, but remain unverified](https://www.reddit.com/r/Seattle/comments/1xhf6qp/archivetoday_links_going_forward/) ⭐️ 6.0/10

A Reddit post alleges that archive.today, the web archiving service also known as archive.is, can redirect users to suspicious domains, with one commenter reporting that an archive.ph page led through stolidityseashellshotter\[.\]com to a fake RT news clone. The claim is unverified: the original poster concedes there is no external write-up, and Reddit moderators have not provided details. Hacker News commenters note that similar concerns surfaced before, but no confirmed technical change or malicious campaign has been independently documented.

hackernews · consumer451 · Oct 28, 15:31 · [Discussion](https://news.ycombinator.com/item?id=50275373)

**「Background」** Archive.today has faced similar redirect concerns before: an earlier Reddit thread reported requests to archive.is being redirected to RT when the referer header was set to removepaywall.com. The service has also come under regulatory pressure in 2026, with Spain ordering ISPs to block Archive.today and its mirror domains and Russia blocking access under its own order.

**「Impact」** Users who rely on archive.today links should treat links inside archived captures as unverified until moderators or researchers publish a technical analysis, and may consider using an alternative archiver for untrusted pages.

**「Community discussion」** Commenters disagree on what is happening: surround reports personally seeing a redirect to a fake RT site after clicking a &quot;Filed on Tuesday&quot; link, while avidruntime suggests archived pages could contain JavaScript that behaves differently when served through archive.today and asks for moderator details. efficax says the unresolved claim alone is enough to stop using the service, and lxe points to a previously reported incident about archive.today behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://www.redditmedia.com/r/cybersecurity/comments/1jlqyyi/is_archiveis_archivetoday_compromised_redirect_to/">Is Archive.is / Archive.today Compromised? Redirect to Russia ...</a></li>
<li><a href="https://cyberinsider.com/spain-blocks-anonymous-service-archive-today-and-all-mirror-domains/">Spain blocks anonymous service Archive.today and all mirror ...</a></li>
<li><a href="https://techcrunch.com/2026/03/23/russian-authorities-block-paywall-removal-site-archive-today/">Russian authorities block paywall removal site Archive.today</a></li>

</ul>
</details>

**Tags**: `#security`, `#archive.today`, `#web archiving`, `#malware`, `#community discussion`

---

<a id="item-tech-news-18"></a>
### [Ted Sanders: model size drives LLM performance; version numbers encode release order](https://simonwillison.net/2026/Oct/28/ted-sanders/) ⭐️ 6.0/10

Quoted by Simon Willison from a Hacker News comment, OpenAI&\#x27;s Ted Sanders said that while LLM performance is multidimensional, model size explains much of the variation—larger models are generally more performant and reliable, cost more per token, and recall esoteric facts better. He also described OpenAI&\#x27;s naming scheme, placing model families as Luna &lt; Terra &lt; Sol &lt; Astra. A version like 6.1, he said, signals it launched after 5.6, shares lineage with other 6.1 releases, and is not the magnitude of jump associated with a 7.

rss · Simon Willison · Oct 28, 23:23

**「Background」** LLM performance is rarely a single ladder: a model can be better at math but worse at jokes than its peers, so users cannot assume one ranking applies to every task. Vendors therefore use model family names and version numbers to communicate ordering, lineage, and the scale of an improvement when comparing releases.

**「Impact」** For teams choosing models by price or reliability, the comments imply that paying for larger models buys reliability and factual recall but not uniformly better performance, and that version increments offer a rough signal—6.x changes are more incremental than a major 7 release.

**Tags**: `#llm`, `#model-scaling`, `#ai-versioning`, `#machine-learning`

---

<a id="item-tech-news-19"></a>
### [GitHub Octoverse 2026: Agentic Development Triples Merged PRs and Commits](https://simonwillison.net/2026/Oct/28/github-octoverse-2026/) ⭐️ 6.0/10

GitHub announced Octoverse 2026 at GitHub Universe, reporting 220 million merged pull requests per month, 7.38 billion commits per month, and 30.3 million new repositories per month. According to EVP Jay Parikh and the report, merged PRs tripled in under a year and commits more than tripled, with most of the growth occurring in the second half of 2026, driven by agentic engineering. The report also includes new industry breakdowns and analysis of repositories involving interoperability or reverse engineering; these figures are GitHub&\#x27;s announced metrics and have not been independently verified here.

rss · Simon Willison · Oct 28, 16:45

**「Background」** Octoverse is GitHub&\#x27;s annual report of developer activity across its platform, tracking metrics such as commits, pull requests, and new repositories over a defined measurement year. The 2026 edition was announced live during GitHub Universe by executive vice president Jay Parikh, and the report&\#x27;s methodology section explains how the underlying push, industry, and repository classifications were computed.

**Tags**: `#GitHub`, `#Octoverse`, `#Developer Metrics`, `#AI Agents`, `#Open Source`

---

<a id="item-tech-news-20"></a>
### [Amazon: AI tooling gaps are findings, not failings](https://simonwillison.net/2026/Oct/28/terk-terkowitz/) ⭐️ 6.0/10

Amazon engineering leadership, in a post by Terk Terkowitz titled &\#x27;An update from Amazon engineering leadership on the role of the developer in the age of AI,&\#x27; told software engineers that if their work does not benefit from current AI tooling, that is &\#x27;a finding, not a failing.&\#x27; The guidance directs engineers to document why AI does not help, share that reasoning with peers, and bring it to their manager to work toward solutions. Terkowitz frames the ability to explain where AI does not yet help as &\#x27;the judgement we are asking for.&\#x27; The statement is a policy directive rather than a shipped tooling change.

rss · Simon Willison · Oct 28, 10:09

**「Background」** The quote comes from an official update on Amazon&\#x27;s company news site, written by engineering leader Terk Terkowitz, on the role of software developers in the age of AI. It is presented as formal guidance from Amazon engineering leadership, not as an individual opinion, and it tells engineers to treat cases where AI tooling does not help as findings to document and discuss rather than as personal shortcomings.

**Tags**: `#amazon`, `#generative-ai`, `#software-engineering`, `#ai-tooling`, `#agentic-engineering`

---

<a id="item-tech-news-21"></a>
### [Redox OS completes io\_uring-like ring buffer support and API](https://lwn.net/Articles/1103359/) ⭐️ 6.0/10

Redox OS has reported completing its io\_uring-like ring buffer support at the system task level, including a liburing-like API for applications, support crates such as an async executor for drivers, and performance work to speed switching between applications and system services. The phase, funded by an NLnet grant, was finished in September.

rss · LWN.net · Oct 28, 14:05

**「Background」** Redox OS is a Unix-like, Rust-based microkernel operating system. io\_uring is the Linux asynchronous I/O interface that uses shared ring buffers to exchange requests and completions without frequent system calls, and Redox&\#x27;s project aims to bring that style of communication between applications and system services.

**「Impact」** Application developers on Redox can begin targeting the io\_uring-like API for asynchronous I/O, while driver and service authors have an async executor crate and ring buffer machinery to build on. The report describes completion rather than a measured rollout, so the practical reach depends on which system services have adopted the new communication path.

**Tags**: `#Redox OS`, `#Rust`, `#io\_uring`, `#operating systems`, `#microkernel`

---

<a id="item-tech-news-22"></a>
### [MIDA Benchmark Shows Multimodal LLMs Fail Werewolf Deception Detection](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+EMNLP%2726%EF%BD%9CGPT%E4%B9%9F%E4%B8%8D%E4%BC%9A%E3%80%8C%E8%AF%BB%E7%A9%BA%E6%B0%94%E3%80%8D%EF%BC%8C%E7%8B%BC%E4%BA%BA%E6%9D%80%E5%9F%BA%E5%87%86%E6%B5%8B%E5%87%BA%E7%A4%BE%E4%BA%A4%E7%9B%B2%E5%8C%BA) ⭐️ 6.0/10

University of Tokyo researchers introduced MIDA \(Multimodal Interactive Deception Assessment\), a benchmark built on One Night Ultimate Werewolf gameplay that tests GPT, Gemini, Claude, Qwen, and DeepSeek models on deception detection in multiplayer social interactions. Results show that current multimodal LLMs can process video, audio, and text yet cannot reliably tell whether a statement contradicts what the speaker actually knew, exposing a social-reasoning gap. The paper was accepted to the EMNLP 2026 main conference, and the code, dataset, and project page are publicly available.

rss · 新智元 · Oct 28, 11:48

**「Background」** Earlier deception-detection research usually focused on a single person&\#x27;s statement or a two-person dialogue, where real-world group dynamics and the lack of a reliable ground truth make it hard to decide whether a statement is a lie. The new MIDA benchmark instead uses One Night Ultimate Werewolf, a game in which roles, nighttime actions, and rules can be traced, so a statement can be objectively labeled as true or deceptive based on what the speaker actually knew at the time.

**「Impact」** For developers deploying multimodal LLMs where truthfulness or intent must be judged in multi-party interactions, the MIDA evaluation of 12 leading models reports a large performance gap on deception detection, with failures traced to missing theory of mind and weak grounding in social signals. Model outputs in such settings should not be treated as reliable deception judgments unless corroborated by other evidence or constrained to high-confidence cases.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.16221">Can MLLMs Read the Room ? A Multimodal Benchmark for...</a></li>
<li><a href="https://www.academia.edu/145120659/Can_MLLMs_Read_the_Room_A_Multimodal_Benchmark_for_Assessing_Deception_in_Multi_Party_Social_Interactions">(PDF) Can MLLMs Read the Room ? A Multimodal Benchmark for...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#benchmark`, `#social reasoning`, `#EMNLP`, `#AI evaluation`

---

<a id="item-tech-news-23"></a>
### [Study: Fixed Feedback Equals Self-Critiques in Hindsight Self-Distillation](https://www.reddit.com/r/MachineLearning/comments/1xhv8yp/how_much_does_the_hint_matter_a_generic_feedback/) ⭐️ 6.0/10

A study of hindsight self-distillation for multi-step financial reasoning on GPT-OSS-20B finds that replacing a student-written critique with a fixed generic feedback line preserves the full accuracy gain of about 3 points, and critiques from a 6x larger model add no material improvement. The proposed Fin-SD method matches OPSD based on full reference solutions while using 9.5% fewer tokens, suggesting that the positional information from hindsight distillation reduces how much privileged information is needed for effective training. The paper and code are linked in the post.

reddit · r/MachineLearning · /u/jhzyu · Oct 28, 17:52

**「Background」** In hindsight self-distillation, a student model identifies its own first wrong step and writes a critique, then uses that critique as privileged guidance when learning from a frozen copy of itself under reverse KL. This setup aims to reduce reliance on strong external teachers or full reference solutions during training.

**「Impact」** For practitioners distilling models for financial reasoning, the result implies that generating bespoke critiques and using larger teacher models may be unnecessary; a fixed feedback line can provide most of the benefit, reducing privileged-information requirements and token cost. The demonstrated 9.5% token reduction relative to OPSD is a concrete efficiency gain, though the result is shown on one model and domain.

**Tags**: `#hindsight self-distillation`, `#financial reasoning`, `#large language models`, `#knowledge distillation`, `#research`

---

<a id="item-tech-news-24"></a>
### [Cocktail-party CAPTCHA test: humans beat ASR but not enough](https://www.reddit.com/r/MachineLearning/comments/1xhuado/cocktailparty_audio_as_a_reverse_turing_test/) ⭐️ 6.0/10

In a small study using 40 synthetic cocktail-party clips, human listeners scored 0.71 mean word accuracy while the best instructed model, Gemini 3.8 Flash, scored 0.54 and Qwen3-ASR scored 0.55. The pass rate at a 0.5 word-accuracy threshold was 77% for humans versus 55% for Gemini, producing only a +0.13 paired same-clip gap with an AUC of 0.62. Because no threshold between 0.5 and 0.9 word accuracy cleanly separated humans from models, the author concludes the setup is not a reliable audio CAPTCHA. The results come from 18 testing sessions, 146 human transcriptions, and 8 model configurations, with limitations including a small sample, a single synthetic setup, and no source separation.

reddit · r/MachineLearning · /u/cloud\_kj · Oct 28, 17:17

**「Background」** Audio CAPTCHAs rely on listening tasks that are easy for humans but hard for automated systems. The cocktail-party effect—focusing on one voice amid competing speech—is a candidate for such a task, and the study tested it by mixing one synthetic target sentence with staggered background voices at 4 dB attenuation, then comparing human transcriptions with several speech recognition configurations.

**「Impact」** The measured gap means this particular cocktail-party task is too weak for production CAPTCHA use, and designers cannot simply pick a word-accuracy threshold to block automated transcriptions while admitting most humans. Anyone pursuing this approach would need audio that remains reliably easy for people while being consistently harder for speech models, a combination the study did not identify.

**Tags**: `#speech recognition`, `#audio captcha`, `#ASR benchmark`, `#cocktail party effect`, `#machine learning`

---

<a id="item-tech-news-25"></a>
### [Discord Public Server Conversations Will Become Web-Searchable](https://techcrunch.com/2026/10/27/discord-is-making-its-public-communities-more-searchable-and-people-have-concerns/) ⭐️ 6.0/10

Discord announced on October 27 that conversations in public, discoverable servers will become web-searchable. Starting November 16, each such server will get a dedicated web page that may include auto-generated discussion summaries, and from mid-December selected public channel messages can appear in search results. Server admins can exclude specific channels, members can opt out individually, published messages will not show usernames or avatars, and the feature is off by default in the EU, UK, and similar regions because of legal restrictions. Teen users are excluded from the rollout.

telegram · zaihuapd · Oct 28, 03:21

**「Background」** Discord&\#x27;s discoverable servers are public communities that users can find and join, but their message content has generally not been indexed by external web search engines. This change extends visibility from app-internal search and direct links to public web search results.

**「Impact」** Server owners and moderators who want to keep community discussions off web search should review their discoverable-server and channel settings before the November 16 rollout, since the availability of per-channel opt-outs means privacy now depends on configuration choices.

**Tags**: `#Discord`, `#privacy`, `#search`, `#social media`, `#tech industry`

---

<a id="item-tech-news-26"></a>
### [South Korea fines Apple $15.5M and Google $32M over app store payment rules](https://appleinsider.com/articles/26/10/28/south-korea-becomes-the-latest-to-fine-apple-and-google-millions-over-their-app-stores) ⭐️ 6.0/10

South Korea&\#x27;s media regulator fined Apple $15.5 million and Google $32 million, ruling that both companies nominally allowed third-party payments but used high fees to obstruct developers, in violation of the country&\#x27;s 2021 app store law. The regulator also said the companies appeared to delay app reviews and demanded that they allow in-app links to external payment options and improve their review processes.

telegram · zaihuapd · Oct 28, 12:30

**「Background」** In 2021, South Korea amended its Telecommunications Business Act to require app store operators such as Apple and Google to allow developers to use third-party payment systems instead of being forced into the operators&\#x27; own in-app purchase systems. The new fines were issued after the country&\#x27;s media and communications regulator concluded that the two companies nominally permitted third-party payments but still used high fees and other practices that effectively obstructed developers, allegedly violating that law.

**「Impact」** If enforced, the order would require Apple and Google to let South Korean developers link users to external payment systems, potentially enabling developers to avoid the commissions that triggered the fines, while also facing faster app review decisions.

**Tags**: `#app-store`, `#regulation`, `#antitrust`, `#Apple`, `#Google`

---

