---
layout: default
title: "Horizon Summary: 2026-10-17 (EN)"
date: 2026-10-17
lang: en
---

> From 52 items, 25 important content pieces were selected

---

**Technology News**
1. [Claude traces five NIST ECDSA seeds to lrand48 and a Unix timestamp](#item-tech-news-1) ⭐️ 8.0/10
2. [Jailbroken PS5 runs llama.cpp natively for GGUF models](#item-tech-news-2) ⭐️ 8.0/10
3. [Big Fish report shows 37-year-old OpenBSD kernel bug exploited](#item-tech-news-3) ⭐️ 8.0/10
4. [Open-source ORL hits 2,788 tokens/s on one RTX 5090 for diffusion LLMs](#item-tech-news-4) ⭐️ 8.0/10
5. [Tesla Roadster promo shows cold-gas thrusters and rocket option](#item-tech-news-5) ⭐️ 7.0/10
6. [Apple MLX Cluster Runs Near-Trillion-Parameter Muse Spark Open on Mac Studios](#item-tech-news-6) ⭐️ 7.0/10
7. [JPEG XL vs. AVIF: Compression, Quality, and Trade-offs](#item-tech-news-7) ⭐️ 7.0/10
8. [Claude Code team details AI-assisted code review workflow](#item-tech-news-8) ⭐️ 7.0/10
9. [Mercor: 90% of U.S. work hours miss AI benchmark coverage](#item-tech-news-9) ⭐️ 7.0/10
10. [StarSkirmish Bench v0.2 tests flagship LLMs by playing StarCraft](#item-tech-news-10) ⭐️ 7.0/10
11. [Safe self-referential structures proposed for kernel Rust](#item-tech-news-11) ⭐️ 7.0/10
12. [StepFun Releases Step 5 Preview Sparse MoE Agent Model](#item-tech-news-12) ⭐️ 7.0/10
13. [Telegram Gave U.S. Phone, IP, and User ID in Court Case](#item-tech-news-13) ⭐️ 7.0/10
14. [Waymo announces autonomous ride-hailing launch in Toronto](#item-tech-news-14) ⭐️ 6.0/10
15. [Home Assistant users object to unannounced HIBP secret scans; opt-out exists](#item-tech-news-15) ⭐️ 6.0/10
16. [Software Rendering Love Letter Draws Aliasing Debate](#item-tech-news-16) ⭐️ 6.0/10
17. [GNOME OS Preview brings stable-based testing to non-developers](#item-tech-news-17) ⭐️ 6.0/10
18. [LWN covers Linux NFS server recent and planned changes](#item-tech-news-18) ⭐️ 6.0/10
19. [Rust framework DenseCore claims bit-exact PyTorch nanoGPT training](#item-tech-news-19) ⭐️ 6.0/10
20. [Kling 4.0 fully launches on klingai.com with developer tooling planned](#item-tech-news-20) ⭐️ 6.0/10

**Financial News**
1. [AI Data-Center Deals Face Market Selloff and Rising Rates](#item-finance-news-1) ⭐️ 7.0/10
2. [China proposes export registration for 40 AI, biotech, and solar technologies](#item-finance-news-2) ⭐️ 7.0/10
3. [Investors temper Anthropic IPO valuation expectations to $1.5 trillion](#item-finance-news-3) ⭐️ 7.0/10

**Twitter News**
1. [Anthropic: Claude Mythos 5 Designs More Efficient Quantum Circuits](#item-twitter-news-1) ⭐️ 8.0/10
2. [OpenAI Announces GPT-6 Astra Pro Upgrade with Parallel Multi-Agent Tasks](#item-twitter-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Claude traces five NIST ECDSA seeds to lrand48 and a Unix timestamp](https://www.anthropic.com/research/ecdsa-curve-origins) ⭐️ 8.0/10

A new write-up linked from Anthropic&\#x27;s research page reports that Claude discovered the origins of the NIST ECDSA seeds for P-192, P-224, P-256, P-384, and P-521: rather than being outputs of a hash algorithm, they came from the C library&\#x27;s lrand48 random-number generator seeded with a Unix timestamp. The fifth seed, B-163, remains unexplained. If correct, the finding closes a long-standing mystery about those five seeds, though it does not by itself prove the curves were selected benignly.

hackernews · ahlCVA · Oct 16, 18:55 · [Discussion](https://news.ycombinator.com/item?id=50122800)

**「Background」** The NIST elliptic-curve standards P-192 through P-521 and ANSI X9.62 include published 160-bit seeds that, since the 1990s, could not be explained by the SHA-1 hashing process the documentation implied, which fueled speculation that the curves might be backdoored. The reported discovery is that the seeds match the output of the C library&\#x27;s lrand48 pseudo-random generator shifted right by 23 bits: each recovered 48-bit state regenerates all 160 bits of a seed, a pattern that would not occur by chance. This matters because lrand48 is a seeded PRNG defined in systems such as OpenBSD, not a cryptographic hash, and Anthropic&\#x27;s report traces the seeds to 1997-98 Unix timestamps.

**「Impact」** The finding undercuts a major source of suspicion about NIST P-curves, but it does not fully prove their origins were benign: as one commenter noted, generated-and-discarded candidate seeds are invisible, so the method alone cannot rule out targeted selection. The still-unexplained B-163 seed leaves one loose end for auditors and standards watchers.

**「Community discussion」** Commenters largely celebrated the result—tptacek called it &quot;devastating news... for an entire generation of NIST cryptography conspiracy theories,&quot; and sweis summarized it as &quot;13 years of tinfoil hats for srand48\(time\(NULL\).&quot; However, fidotron cautioned that knowing the generation method says nothing about selection because discarded candidates are unobservable, and teddyh speculated that the unresolved B-163 seed might come from a typo during publication.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/ecdsa-curve-origins">Claude reveals ECDSA curve origins \ Anthropic</a></li>
<li><a href="https://t.me/heartysender/367367">Закрепи.sender – Telegram</a></li>
<li><a href="https://man.openbsd.org/lrand48.3">rand48(3) - OpenBSD manual pages</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#NIST curves`, `#Claude`, `#random number generation`, `#security research`

---

<a id="item-tech-news-2"></a>
### [Jailbroken PS5 runs llama.cpp natively for GGUF models](https://github.com/cobanov/PS5LM) ⭐️ 8.0/10

A jailbroken PlayStation 5 can now run llama.cpp natively, letting GGUF-format large language models execute directly on the console&\#x27;s hardware rather than through emulation or remote serving. The project is hosted on GitHub and repurposes the console as a low-power LLM inference device. Practical use is still constrained: it relies on jailbroken hardware, and community-reported examples are limited to 2-bit quantized models such as Qwen 3.8 27B.

hackernews · Anon84 · Oct 16, 18:32 · [Discussion](https://news.ycombinator.com/item?id=50122431)

**「Background」** The project depends on two earlier developments: a jailbroken PS5 and llama.cpp&\#x27;s portable GGUF model format, which allows quantized language models to run locally as single files. Horizon&\#x27;s September 30 digest reported the Relapse exploit targeting a WebKit/JavaScriptCore bug as a potential jailbreak path, though no independent confirmation was available at the time.

**「Impact」** Commenter estimates suggest practical use as an always-on, low-power inference box: a 27B Qwen model at 2-bit quantization can produce roughly 2 million output tokens per day at about 70 cents of electricity, suitable for long-running low-intensity tasks such as monitoring or status checks. Commenters also point to AMD BC-250 boards as a cheaper PS5-adjacent route: they use a cut-down version of the PS5&\#x27;s custom silicon and are listed secondhand for $60–$100 on eBay, though listings warn that standard Windows AMD drivers do not provide GPU acceleration for the BC-250, so community drivers or a port like this one remain prerequisites.

**「Community discussion」** Commenters disagreed on where to host the project, with Rabbit504030201 warning that GitHub is vulnerable to a Sony takedown and recommending a custom domain. Others noted the port could extend to AMD&\#x27;s Cyan Skillfish-based BC250 ex-mining boards, a cut-down PS5 APU, and saw value in a cheap, always-on token stream for long-running tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">2026-09-30 — PS5 Relapse exploit reportedly targets WebKit JavaScriptCore bug</a></li>
<li><a href="https://www.ebay.com/itm/327403530900">ASRock AMD BC-250 PS5 APU Board RDNA2 16GB GDDR6- - eBay</a></li>
<li><a href="https://pithwire.com/en/articles/the-60-gaming-pc-amd-bc-250-2025/">AMD BC-250: The $60-$100 PS5-Chip Gaming PC | PithWire</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#PS5`, `#GGUF`, `#LLM inference`, `#hardware hacking`

---

<a id="item-tech-news-3"></a>
### [Big Fish report shows 37-year-old OpenBSD kernel bug exploited](https://calif.io/research/big-fish) ⭐️ 8.0/10

A security research report published at calif.io/research/big-fish documents the exploitation of a 37-year-old kernel bug in OpenBSD, one of the most heavily audited codebases. The write-up highlights how such defects can survive for decades despite extensive review; the available material does not include a patch, affected version, or technical exploit details.

hackernews · rs\_rs\_rs\_rs\_rs · Oct 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=50118977)

**「Background」** The bug concerns a shared-memory attachment counter in the BSD-derived SysV IPC code that was originally declared as a signed 16-bit short; the declaration traces back roughly 37 years to the original BSD sources. The age refers to that inherited design decision, not to modern OpenBSD, which has carried the same code forward as a separate project.

**「Community discussion」** One commenter reported that NetBSD accidentally fixed the same code during a rewrite in August 1999. Another questioned whether fuzzing or static analysis could realistically have caught this bug class, or whether it required a human reasoning about the exploit primitive.

<details><summary>References</summary>
<ul>
<li><a href="https://calif.io/research/big-fish">Big Fish : Exploiting a 37 - Year - Old Kernel Bug in OpenBSD | Calif</a></li>
<li><a href="https://dzen.ru/a/atJi8f5wA2igUvxy">Calif получила root в OpenBSD через 37 -летнюю ошибку ядра | Дзен</a></li>

</ul>
</details>

**Tags**: `#openbsd`, `#kernel-security`, `#exploitation`, `#operating-systems`, `#security-research`

---

<a id="item-tech-news-4"></a>
### [Open-source ORL hits 2,788 tokens/s on one RTX 5090 for diffusion LLMs](https://www.reddit.com/r/MachineLearning/comments/1x7qgr0/research_2788_tokenss_on_a_single_rtx_5090_with_a/) ⭐️ 8.0/10

ORL, an open-source on-policy residual learning method paired with the custom dlmrt inference engine, reports peak single-request decoding of 2,788 tokens/s for LLaDA-2.1-mini on a single RTX 5090 and 7,708 tokens/s for DiffusionGemma 26B MoE on 8× B200 with NVFP4. On QwenDLM-4B, ORL reports roughly 6.9× higher end-to-end throughput with comparable or better quality, including a HumanEval pass@1 improvement from 82.9% to 89.6%, and a 1.74× speedup over DFlash speculative decoding in matched single-H100 comparisons. Models, training code, evaluation pipeline, and the dlmrt inference engine are released as open source; the cited figures are peak single-request benchmark results, not aggregate throughput across concurrent requests.

reddit · r/MachineLearning · /u/arty\_photography · Oct 16, 20:03

**「Background」** Diffusion language models \(dLLMs\) can refine and finalize multiple tokens in parallel, unlike autoregressive LLMs that emit one token at a time, but making them converge in fewer forward passes is a known bottleneck. ORL trains on fresh, self-generated residual trajectories and uses Adjacent Entropy Contraction to encourage each denoising step to reduce uncertainty faster.

**「Impact」** Practitioners with an RTX 5090 can download the LLaDA-2.1-mini ORL NVFP4 checkpoint and try dlmrt locally for low-latency diffusion decoding, but because the reported numbers are peak single-request benchmarks, users should measure performance against their own workloads and prompts before relying on them.

**Tags**: `#diffusion LLMs`, `#inference optimization`, `#open source`, `#efficient decoding`, `#GPU performance`

---

<a id="item-tech-news-5"></a>
### [Tesla Roadster promo shows cold-gas thrusters and rocket option](https://www.tesla.com/roadster) ⭐️ 7.0/10

Tesla released a promotional video for the Roadster that demonstrates a version using cold-gas thrusters, with a separate &quot;invite only&quot; combustion rocket-engine mode, as well as stunts such as driving vertically and sticking to a ceiling. The footage is a marketing-forward demonstration rather than evidence of a shipped product, and it has not been independently verified. Commenters noted the demonstrator appears to use spacecraft-style cold-gas thrusters and guidance hardware, while pre-order delivery remains officially unguaranteed.

hackernews · shekhar101 · Oct 16, 01:32 · [Discussion](https://news.ycombinator.com/item?id=50112657)

**「Background」** Tesla&\#x27;s Roadster is the company&\#x27;s production-intent electric hypercar, and this newly released promotional video shows it equipped with cold-gas thrusters for extra forward acceleration as well as a combustion rocket-engine configuration. The demo positions the Roadster as an unusually extreme vehicle, but it remains a marketing showcase rather than a delivered production model.

**「Impact」** Interested buyers can now reserve the Roadster for a $5,000 deposit plus $45,000 due within 10 days for the base vehicle, with cold-gas thrusters and the air suction system priced separately \(tool-2-1\). The concrete consequence is a $50,000 commitment to a vehicle that has not shipped; community commenters point out that Tesla has previously said delivery of Roadster pre-orders is not guaranteed, and the reported 1.1-second 0-60 time with the thruster option comes from third-party outlets rather than an official spec \(tool-2-3\).

**「Community discussion」** Commenters were impressed by the engineering spectacle but disagreed about real-world feasibility and safety: some questioned how a 1,000+ kg car with limited compressed-gas storage could drive vertically or stick to a ceiling, while others warned that COPV-powered thrusters could endanger anyone beside the vehicle. Several also criticized the business side, calling the years-long pre-order deposits akin to free loans for a car that may never be delivered.

<details><summary>References</summary>
<ul>
<li><a href="https://www.engadget.com/2288437/teslas-redesigned-roadster-cold-gas-thruster-option-reservation/">Tesla &#x27;s Redesigned Roadster Has A Cold - Gas Thruster Option, But...</a></li>
<li><a href="https://www.motorbiscuit.com/insane-tesla-roadster-0-60-mph-in-1-1-seconds-uses-gas-thruster-option/">Insane: Tesla Roadster 0-60 MPH in 1.1 Seconds Uses Gas Thruster ...</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#electric vehicles`, `#rocket propulsion`, `#automotive engineering`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [Apple MLX Cluster Runs Near-Trillion-Parameter Muse Spark Open on Mac Studios](https://machinelearning.apple.com/research/mlx-distributed-inference) ⭐️ 7.0/10

Apple ML Research published a demonstration of running Muse Spark Open, a nearly trillion-parameter open-weights model, on a cluster of Mac Studios using the latest MLX release. The system reportedly reaches over 36 tokens per second and scales from a single Mac Studio with up to 512GB of unified memory to multiple machines. This is a vendor demonstration rather than an independently verified benchmark, and the reported throughput was measured at an 8,192-token context.

hackernews · antipaul · Oct 16, 13:43 · [Discussion](https://news.ycombinator.com/item?id=50118320)

**「Background」** MLX is Apple&\#x27;s array-based framework for running machine learning models on Apple Silicon, and Meta&\#x27;s open-weight Muse Spark Open model has been positioned as optimized for Apple hardware, with Apple and Meta cooperating on the launch. Earlier in the same week, Horizon&\#x27;s Oct 14 digest reported that Apple Research described a distributed virtual GPU cloud pooling idle Apple Silicon devices; the new post applies that distributed-execution direction to running a near-trillion-parameter model across a cluster of Mac Studios.

**「Impact」** For MLX users, the result makes cluster-scale local inference of very large open-weights models more concrete, but the practical benefit is limited by memory cost and the short context used in the measurement. Commenters also questioned the benchmark&\#x27;s fairness, noting that the Meta model was quantized to 4-bit while Qwen was compared only in native BF16.

**「Community discussion」** One commenter argued the comparison unfairly favored Meta by benchmarking its model at 4-bit while leaving Qwen in BF16, and another countered that a single M5 Ultra already runs DeepSeek 4.1 Flash at roughly 45 tokens per second, making a multi-Mac cluster less compelling for many workloads. A separate comment noted that 8,192 tokens of context is too short for many practical uses.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearning.apple.com/research/distributed-gpu-cloud">2026-10-14 — Apple Research Details Virtual GPU Cloud from Idle Apple Silicon</a></li>
<li><a href="https://www.theverge.com/news/1012293/meta-apple-muse-spark-open-ai-model-mlx">Meta and Apple team up to make Muse AI models run... | The Verge</a></li>

</ul>
</details>

**Tags**: `#MLX`, `#distributed inference`, `#Apple`, `#large language models`, `#Mac Studio`

---

<a id="item-tech-news-7"></a>
### [JPEG XL vs. AVIF: Compression, Quality, and Trade-offs](https://jakearchibald.com/2026/jpeg-xl-vs-avif/) ⭐️ 7.0/10

A detailed technical comparison on jakearchibald.com evaluates JPEG XL versus AVIF for web image use, examining compression efficiency, output quality, and practical trade-offs. The article gives developers a focused basis for choosing between the formats rather than presenting either as universally superior.

hackernews · farlight · Oct 16, 16:12 · [Discussion](https://news.ycombinator.com/item?id=50120224)

**「Background」** Horizon&\#x27;s October 8 digest reported that Chrome shipped JPEG XL support, reversing its 2023 removal of the format and joining Safari as well as the upcoming Firefox stable release, giving JPEG XL majority browser coverage. Even with that support, third-party 2026 analyses still describe JPEG XL as experimental for production use at roughly 10–25% of users, while AVIF reaches about 93.4% of global browser traffic. This browser-support gap is the practical context for comparing the two codecs for web delivery.

**「Community Discussion」** Commenters offered sharply different practical lessons: one shared ffmpeg settings that produced very small AVIF files with good quality, another argued AVIF visibly erased highlights in a Formula 1 image, and another contended that current JPEG XL encoders are immature, citing much smaller lossless files from alternative encoders. A separate commenter noted libjxl&\#x27;s slow maximum effort comes from its Butteraugli optimization loop and that an alternative encoder reaches similar results faster.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/blog/jpeg-xl-in-chrome">2026-10-08 — Chrome ships JPEG XL support, joining Safari and Firefox</a></li>
<li><a href="https://www.inverity.ai/posts/avif-vs-webp-vs-jpeg-xl-2026">AVIF vs WebP vs JPEG XL in 2026: Which Format Wins?</a></li>
<li><a href="https://coretoolshub.com/blog/avif-vs-webp-vs-jpeg-xl-2026/">AVIF vs WebP vs JPEG XL — 2026 Format Comparison</a></li>

</ul>
</details>

**Tags**: `#jpeg-xl`, `#avif`, `#image-compression`, `#web-performance`, `#codecs`

---

<a id="item-tech-news-8"></a>
### [Claude Code team details AI-assisted code review workflow](https://claude.dev/blog/solving-code-review-at-anthropic/) ⭐️ 7.0/10

In a new blog post, Anthropic&\#x27;s Claude Code team explains its AI-assisted code review pipeline, which automates most review paths, routes human attention to risky changes, and scores every reviewer change against an eval set that grows with incidents. They report processing 30,000 pull requests per day and argue that &quot;did a human read the code?&quot; is an imprecise proxy for catching what could go wrong with a change. The post is an internal workflow description for engineering teams considering similar tooling, not a shipped product or an externally verified benchmark.

hackernews · pretext · Oct 16, 19:04 · [Discussion](https://news.ycombinator.com/item?id=50122951)

**「Background」** Claude Code is Anthropic&\#x27;s terminal-based AI coding assistant, and this post describes how the team that builds it reviews changes in its own development workflow. No earlier Horizon summary covered this specific internal process, so the necessary context is limited to what the article itself presents about the team&\#x27;s approach to pull-request review.

**「Impact」** Engineering teams evaluating this model should treat the reported 30,000 pull requests per day as an unverified internal claim rather than a proven benchmark: the post does not provide churn-rate or cost-per-line data, and commenters specifically asked for both measurements when assessing whether the approach is actually efficient.

**「Community discussion」** Several Hacker News commenters challenged the article&\#x27;s rigor: vb-8448 doubted humans can meaningfully keep pace with 30,000 pull requests per day and asked for churn and cost-per-LOC figures, while koolba called the policy of letting an LLM write documentation without human review &quot;pure insanity.&quot; mk12 noted the prose appears AI-assisted, and dieortin disputed the post&\#x27;s framing that slowing down mostly lowers error rate, pointing out that doing less overall is not the same as improving rates.

**Tags**: `#ai-code-review`, `#anthropic`, `#claude-code`, `#software-engineering`, `#developer-tools`

---

<a id="item-tech-news-9"></a>
### [Mercor: 90% of U.S. work hours miss AI benchmark coverage](https://www.mercor.com/research/labor-index/benchmark-map/) ⭐️ 7.0/10

A Mercor research report argues that 90% of U.S. working hours are spent on tasks that existing AI benchmarks cover poorly or not at all, making benchmark scores a weak proxy for real-world usefulness. The analysis points to a mismatch between benchmark prompts and the work Americans actually do, and it flags that high-wage occupations are overrepresented among benchmark prompts. This is the report&\#x27;s methodology-based argument, not an independent measurement of model capability.

hackernews · speckx · Oct 16, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50121179)

**「Background」** AI benchmarks score models against curated prompts, and those scores are widely treated as proxies for real-world usefulness in jobs. Mercor — the company publishing this Labor Index report — develops benchmarks, evaluation environments, and large-scale human datasets through an expert marketplace and publishes the APEX benchmark family, which measures whether AI models can perform economically valuable professional work; the report is therefore an evaluation vendor&\#x27;s own analysis of the gap between benchmark coverage and actual US working hours.

**「Impact」** For organizations choosing AI tools, high benchmark scores should not be treated as proof of usefulness for most job tasks; buyers and developers may need task-level, occupation-specific evaluation before deployment.

**「Community discussion」** Commenters mostly accepted the gap but disputed its meaning: OtherShrezzing argued the report treats &quot;covered well&quot; as if it meant &quot;covered at all,&quot; since 13 prompts cannot represent the range of a social worker&\#x27;s job, while 10111001 said the wage-bill overrepresentation suggests benchmark designers are effectively steering AI toward high-wage work. Another comment likened the problem to the &quot;Doorman Fallacy,&quot; where secondary functions are missed when a task appears automatable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mercor.com/research/">Mercor Research | Frontier AI Training Data &amp; Human Evaluation</a></li>
<li><a href="https://www.everydev.ai/tools/mercor">Mercor - AI Expert Workforce Platform | EveryDev. ai</a></li>

</ul>
</details>

**Tags**: `#AI benchmarks`, `#labor market`, `#AI evaluation`, `#O\*NET`, `#AI adoption`

---

<a id="item-tech-news-10"></a>
### [StarSkirmish Bench v0.2 tests flagship LLMs by playing StarCraft](https://starskirmish.com/bench/v0-2/) ⭐️ 7.0/10

StarSkirmish Bench v0.2 has been refreshed, adding results from the flagship models of OpenAI, Anthropic, Google, and Muse, all evaluated by having LLMs write code to play StarCraft: Brood War. The benchmark treats the task as an agentic coding challenge rather than a direct game-playing comparison.

hackernews · \_\_cayenne\_\_ · Oct 16, 14:18 · [Discussion](https://news.ycombinator.com/item?id=50118688)

**「Background」** StarSkirmish Bench is a benchmark that tests frontier LLMs by having them write code to play StarCraft: Brood War. In the v0.2 setup, each model runs inside its lab&\#x27;s first-party CLI agent harness—such as Claude Code, Codex, Antigravity CLI, or Muse Code—with web search and fetch tools disabled and no other internet access. The refresh compares flagship models from OpenAI, Anthropic, Google, and Muse on this agentic coding task.

**「Community Discussion」** One commenter reports that the StarSkirmish ordering—GPT-6 Astra &gt; GPT-6.1 Sol &gt; Gemini 4 Argon &gt; Claude Opus 5.5 &gt; Claude Fable 5.1 &gt; Claude Sonnet 5.5—matches the order of a friend&\#x27;s independent 9x9 Go benchmark exactly. Another commenter questions whether the time-limited, agent-written StarCraft bots reveal anything beyond being inferior versions of the best human-coded bots.

**Tags**: `#AI agents`, `#LLM benchmarks`, `#StarCraft`, `#machine learning`, `#software engineering`

---

<a id="item-tech-news-11"></a>
### [Safe self-referential structures proposed for kernel Rust](https://lwn.net/Articles/1099224/) ⭐️ 7.0/10

Gary Guo presented an approach at Kangrejos 2026 for implementing self-referential data structures in kernel Rust without unsafe code, building on the pin\_init crate for immovable data structures. If adopted, the changes could remove most unsafe lifetime-related code from the Nova GPU driver and eventually other kernel Rust components. The presentation describes a proposed technique rather than a shipped capability.

rss · LWN.net · Oct 16, 18:30

**「Background」** Rust&\#x27;s ownership and lifetime rules normally make self-referential data structures—where a structure holds a reference into its own storage—difficult to implement safely, because moving the structure can invalidate the reference. The kernel&\#x27;s pin\_init crate was created to help construct immovable data structures, typically for interoperability with C, but that construction has traditionally required unsafe code to manage the lifetimes involved.

**「Impact」** For kernel Rust developers, adopting Guo&\#x27;s pin\_init changes could eliminate most unsafe blocks tied to lifetimes in the Nova driver, shrinking the area of kernel code that requires manual unsafe auditing and easing the use of self-referential structures elsewhere in the kernel.

**Tags**: `#rust`, `#linux-kernel`, `#self-referential-structures`, `#unsafe-code`, `#systems-programming`

---

<a id="item-tech-news-12"></a>
### [StepFun Releases Step 5 Preview Sparse MoE Agent Model](https://huggingface.co/stepfun-ai/Step-5-Preview) ⭐️ 7.0/10

StepFun has released Step 5 Preview on Hugging Face, a flagship sparse-MoE model for agentic work with 600B total parameters and 270B active parameters. It supports up to 1M-token context and text, image, and video inputs, and is positioned as leading in software engineering, long-horizon agent execution, and professional knowledge tasks, especially in finance. The model can be deployed through an OpenAI-compatible API with vLLM or SGLang under the StepFun Model License 1.0; because this is a preview release, the announced capabilities still await independent benchmark and adoption results.

telegram · zaihuapd · Oct 16, 06:36

**「Background」** Step 5 Preview uses a sparse mixture-of-experts \(MoE\) architecture, meaning only a subset of its 600 billion total parameters — 270 billion — is active for each token, which is the design principle behind large models that promise long-context handling. Because it is released as a Hugging Face preview with an OpenAI-compatible API, it is intended to be deployable through standard open-source inference frameworks rather than only through a vendor-hosted endpoint.

**「Impact」** Development teams can now deploy Step 5 Preview themselves or call it through an OpenAI-compatible API using vLLM or SGLang, but they must review the StepFun Model License 1.0 terms before production use. Its 600B-parameter sparse MoE design \(with 270B active parameters\) means serving it in production will require substantial multi-GPU infrastructure.

**Tags**: `#AI models`, `#sparse MoE`, `#agentic AI`, `#software engineering`, `#long context`

---

<a id="item-tech-news-13"></a>
### [Telegram Gave U.S. Phone, IP, and User ID in Court Case](https://www.404media.co/heres-what-telegram-giving-data-to-the-u-s-government-looks-like/) ⭐️ 7.0/10

Newly released U.S. court documents show Telegram provided authorities with a user&\#x27;s phone number, user ID, and IP address in response to a court order, describing the disclosure as voluntary and not acknowledging U.S. jurisdiction. The case concerns Mahmoud Al-Muhtadi, who is accused of involvement in the October 7, 2023 attack on Israel. According to 404 Media, Telegram had shared data on 2,253 users with U.S. authorities as of January.

telegram · zaihuapd · Oct 16, 14:57

**「Background」** The new filings come from a US prosecution of Mahmoud Al-Muhtadi, who is accused of involvement in the October 7, 2023 attack on Israel, and they show how authorities obtained subscriber data from Telegram through a court order.

**「Impact」** For Telegram users in similar U.S. investigations, this case shows that court-ordered requests can produce phone numbers, user IP addresses, and user IDs despite Telegram&\#x27;s stance that it is not under U.S. jurisdiction, so account identifiers should be treated as potentially discoverable.

**Tags**: `#privacy`, `#telegram`, `#government-data-requests`, `#surveillance`, `#tech-policy`

---

<a id="item-tech-news-14"></a>
### [Waymo announces autonomous ride-hailing launch in Toronto](https://waymo.com/blog/2026/10/waymo-in-toronto/) ⭐️ 6.0/10

Waymo has announced that its autonomous ride-hailing service is launching in Toronto, adding the city as a new market. The official blog post confirms the expansion, but the available item provides no service date, coverage details, or vehicle specifics.

hackernews · ChrisArchitect · Oct 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=50118981)

**「Background」** Waymo had earlier signaled plans to expand into Canada, with reports naming Toronto and British Columbia as candidate cities and noting that Ontario government approval would be needed for what could become Canada&\#x27;s first driverless taxi fleet \(tool-2-1, tool-2-3\). The same reporting cautioned that Canadian winters would test Waymo&\#x27;s systems, which were first developed for warm, dry climates and would have to handle snow and altered driving behaviour \(tool-2-2\).

**「Impact」** Toronto riders will not be able to hail Waymo immediately: the company says it is only laying the groundwork and targets its first riders in 2028, so local officials and regulators now have roughly two years to address testing, approval, and deployment questions. If the launch proceeds, Toronto would become the first Canadian city with fully autonomous ride-hailing service.

**「Community discussion」** Commenters report mixed rider experiences: one described an Austin trip that was extended from a planned 9 minutes to 45, in what the rider attributed to the vehicle getting lost, with support eventually ending the ride at a restaurant, while several others said Waymo rides in San Francisco and elsewhere have been smooth. Another commenter contrasted the Toronto announcement&\#x27;s job-creation framing with Waymo&\#x27;s stalled Boston expansion amid legislative opposition tied to job-loss concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://driveteslacanada.ca/news/waymo-eyes-canadian-launch-in-toronto-and-b-c/">Waymo eyes Canadian launch in Toronto and B.C. - Drive Tesla</a></li>
<li><a href="https://www.cbc.ca/news/canada/toronto/waymo-self-driving-taxis-toronto-9.7023379">Could Torontonians soon ride self-driving taxis? That’s Waymo ’s plan</a></li>
<li><a href="https://www.readthepeak.com/p/take-the-wheel">Waymo eyes Toronto expansion, Discount grocery stores are...</a></li>
<li><a href="https://waymo.com/blog/2026/10/waymo-in-toronto/">Hello Toronto! Waymo is En Route</a></li>
<li><a href="https://toronto.citynews.ca/2026/10/16/waymo-cars-autonomous-toronto-2028-launch/">Waymo eyes Toronto launch in 2028 - CityNews Toronto</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#waymo`, `#ride-hailing`, `#AI-transportation`, `#expansion`

---

<a id="item-tech-news-15"></a>
### [Home Assistant users object to unannounced HIBP secret scans; opt-out exists](https://github.com/home-assistant/home-assistant.io/issues/49314) ⭐️ 6.0/10

Home Assistant users report that the Supervisor&\#x27;s password-breach check scans secrets and sends short prefixes of them to Have I Been Pwned without a clear opt-in. Maintainer Frenck apologized for initially dismissive responses and clarified that the check has been part of the Supervisor for years, that a recent release made its warning visible, and that users can disable it with \`ha security options --pwned=false\`. According to the maintainer, only the first five characters of the secret are sent.

hackernews · trvrprkr · Oct 16, 20:33 · [Discussion](https://news.ycombinator.com/item?id=50124251)

**「Background」** Home Assistant is an open-source home-automation platform whose Supervisor layer manages add-ons and system options, including options marked as passwords. Password-breach checking often uses Have I Been Pwned&\#x27;s k-anonymity model, which compares only a short hash prefix rather than the full secret, and the controversy here is whether that design still requires explicit user consent.

**「Impact」** Users who object to the scan can disable it by running \`ha security options --pwned=false\`; anyone who leaves the check enabled should understand that a third-party service receives short prefixes of secrets stored in Supervisor app options.

**「Community discussion」** The strongest objection, from eranation, is that even a mathematically &quot;safe&quot; hash-prefix scan should require opt-in before any user data is handed to a third party. Maintainer frenck acknowledged his earlier replies were dismissive and provided the opt-out command, while janice1999 separately cited past maintainer conduct as turning them away from the project.

**Tags**: `#home-assistant`, `#privacy`, `#security`, `#open-source`

---

<a id="item-tech-news-16"></a>
### [Software Rendering Love Letter Draws Aliasing Debate](https://www.jamesfmackenzie.com/2026/10/13/i-love-software-rendering/) ⭐️ 6.0/10

An essay on James F. Mackenzie&\#x27;s site celebrates the distinctive low-resolution visuals of CPU-based software rendering, including unfiltered textures and lookup-table effects, and contrasts them with the smoothed output of early 3D cards. Commenters push back that much of the look is simply disabled spatial anti-aliasing and unfiltered texture sampling, which modern GPU-based games can still reproduce, while acknowledging that GPU triangle rasterization differs at low resolutions.

hackernews · speckx · Oct 16, 12:52 · [Discussion](https://news.ycombinator.com/item?id=50117746)

**「Background」** Software rendering draws a 3D scene on the CPU, deciding each pixel&\#x27;s color directly rather than relying on a GPU&\#x27;s hardware rasterization. That flexibility let CPU renderers produce effects that fixed-function graphics cards of the 1990s could not easily match, while early 3D cards smoothed textures with bilinear filtering.

**「Impact」** For developers and hobbyists chasing the retro look, the discussion suggests that the aliased, unfiltered appearance can be reproduced on modern hardware by disabling spatial anti-aliasing and using unfiltered textures. One remaining difference is that GPUs rasterize triangles using pixel-center coverage, so exact low-resolution output will not match classic CPU renderers.

**「Community Discussion」** Commenters disagree over whether the article captures a unique software-rendering aesthetic or just the absence of anti-aliasing: delta\_p\_delta\_x argues the effect is available in modern games simply by turning off spatial anti-aliasing, while buffportion notes that GPU triangle rasterization uses a different pixel-coverage rule and Bob1029 recalls that CPU software rendering could express effects fixed-function GPU pipelines of the time could not.

**Tags**: `#software rendering`, `#computer graphics`, `#GPU rasterization`, `#retro gaming`, `#game development`

---

<a id="item-tech-news-17"></a>
### [GNOME OS Preview brings stable-based testing to non-developers](https://lwn.net/Articles/1101057/) ⭐️ 6.0/10

The GNOME Project has announced GNOME OS Preview, a new edition of GNOME OS built from the latest stable GNOME release, currently GNOME 51.1, instead of nightly commits. Unlike the existing Nightly edition aimed at GNOME developers, Preview targets non-developer enthusiasts and is available to download today. The project cautions that Preview has only seen limited real-life testing and is not yet considered complete or stable for the broader public.

rss · LWN.net · Oct 16, 19:05

**「Background」** GNOME OS has been available for some time, but until now the project provided only a Nightly edition built from the latest commits and intended solely for GNOME developers. GNOME OS Preview is based on the same GitLab branches as the stable org.gnome.Platform Flatpak runtimes, providing a more stable pre-release option for non-developers.

**「Impact」** Adventurous non-developer users can now try GNOME OS for daily use from a stable-based build, but they should expect initial issues and be prepared to reinstall once a stable version is declared.

**Tags**: `#GNOME`, `#Open Source`, `#Linux`, `#Desktop`, `#Operating Systems`

---

<a id="item-tech-news-18"></a>
### [LWN covers Linux NFS server recent and planned changes](https://lwn.net/Articles/1098611/) ⭐️ 6.0/10

LWN reports on Jeff Layton&\#x27;s Linux Plumbers Conference 2026 talk, which surveyed recent enhancements to the Linux NFS server and outlined near-term development plans. The excerpt does not name specific features, versions, or release dates.

rss · LWN.net · Oct 16, 14:26

**「Background」** The Linux kernel has long provided an NFS server, implementing the Network File System protocol that lets clients access files over a network. NFS has evolved over decades, so the kernel implementation must be periodically updated to track new protocol features and performance improvements. Talks like Jeff Layton&\#x27;s at the 2026 Linux Plumbers Conference are how kernel developers share the state of those ongoing changes with the wider community.

**Tags**: `#Linux`, `#NFS`, `#kernel`, `#filesystems`, `#conference`

---

<a id="item-tech-news-19"></a>
### [Rust framework DenseCore claims bit-exact PyTorch nanoGPT training](https://www.reddit.com/r/MachineLearning/comments/1x7ojxo/p_my_rust_framework_trains_nanogpt_with_the_exact/) ⭐️ 6.0/10

A CS student reports that DenseCore, a Rust deep-learning framework with a PyTorch-like Python API, runs Karpathy&\#x27;s nanoGPT unchanged and produces bit-for-bit identical weights, losses, and gradients to PyTorch for 50 training steps on Apple Silicon, even with dropout enabled. The author says matching PyTorch required reproducing internal quirks such as CPU flash attention and fused Adam tail-loop rounding; DenseCore is about 2 MB versus roughly 580 MB for PyTorch. The result is self-reported and not independently verified.

reddit · r/MachineLearning · /u/Mental-Feature-2377 · Oct 16, 18:49

**「Background」** nanoGPT is Andrej Karpathy&\#x27;s minimal GPT implementation commonly used as a training-loop benchmark. Bit-exact reproduction means matching PyTorch&\#x27;s floating-point outputs exactly, not just approximately; the author reports that achieving it required mimicking PyTorch&\#x27;s CPU kernels and optimizer rounding rather than the textbook formulas.

**「Impact」** For developers who need deterministic small CPU training on Apple Silicon, a verified DenseCore could act as a lightweight PyTorch substitute, but the reported compatibility is currently limited to 50 steps on one platform and lacks independent evaluation, so production use would be premature.

**Tags**: `#rust`, `#deep learning framework`, `#pytorch compatibility`, `#nanogpt`, `#bit-exactness`

---

<a id="item-tech-news-20"></a>
### [Kling 4.0 fully launches on klingai.com with developer tooling planned](https://mp.weixin.qq.com/s/Dn2jAxV0m6kpt7y4edRvdg) ⭐️ 6.0/10

Kling 4.0 has fully launched on klingai.com as of the October 15 announcement, with a redesigned creation page that the vendor says offers a more flexible and open workflow. The announcement also states that Kling 4.0 already supports MCP and CLI integration, while 4K and 1080p 10-bit HDR output and an API for enterprises and developers are planned for the near future. The HDR output and API availability remain announced plans rather than currently shipped capabilities.

telegram · zaihuapd · Oct 16, 04:30

**「Background」** Horizon&\#x27;s September 29 digest reported that Kuaishou announced Kling 4.0 would launch in October and began a limited preview of Kling 4.0 Flash on September 28, with plans for 4K and 1080p 10-bit HDR output. This item confirms that the full Kling 4.0 model has now gone live on klingai.com, while the promised HDR output formats remain a future offering and API access is still to come.

**「Impact」** Developers can begin experimenting with MCP and CLI integration for Kling 4.0 now, but should not build production pipelines around the promised API until Kling publishes the actual API service and documentation.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.sina.com.cn/stock/t/2026-09-28/doc-initmeau2827369.shtml">2026-09-29 — Kuaishou&#x27;s Kling 4.0 Arrives in October with 4K and HDR Upgrades</a></li>

</ul>
</details>

**Tags**: `#AI video generation`, `#Kling 4.0`, `#MCP`, `#API`, `#HDR`

---

## Financial News

<a id="item-finance-news-1"></a>
### [AI Data-Center Deals Face Market Selloff and Rising Rates](https://www.kitco.com/news/off-the-wire/2026-10-15/market-selloff-rising-rates-test-ai-data-centre-deal-boom) ⭐️ 7.0/10

A market selloff and higher interest rates are testing AI data-center investments: AirTrunk’s REIT listing, Nvidia-backed Firmus, and SoftBank-backed SB Energy saw their listing plans withdrawn or paused in the past week. Dealogic data show Asian data-center M&amp;A has reached $21.3 billion this year, roughly double 2025’s $10 billion full-year total, while equity financing is down 4.6% from a year earlier.

telegram · zaihuapd · Oct 16, 05:10

**「Background」** AirTrunk and Firmus had been preparing large listings before the market turbulence: AirTrunk was targeting a Singapore REIT IPO that could raise about US$1.5 billion, and Firmus had planned an IPO of up to US$5 billion until it withdrew on October 8.

<details><summary>References</summary>
<ul>
<li><a href="https://www.freemalaysiatoday.com/category/business/2026/09/11/blackstone-s-airtrunk-seeks-us-1-6bil-loan-for-singapore-ipo">Blackstone’s AirTrunk seeks US$1.6bil loan for Singapore IPO | FMT</a></li>
<li><a href="https://au.finance.yahoo.com/news/stock-sinks-23-australia-30bn-034730756.html">A stock sinks 23% as Australia’s $30bn Firmus AI data - centre IPO ...</a></li>

</ul>
</details>

**Tags**: `#AI数据中心`, `#IPO撤回`, `#利率上升`, `#并购`, `#资本市场`

---

<a id="item-finance-news-2"></a>
### [China proposes export registration for 40 AI, biotech, and solar technologies](https://aqygzj.mofcom.gov.cn/flzc/gzjgfxwj/art/2026/art_c99f95ca0cd043829ac9991495fc283c.html) ⭐️ 7.0/10

China’s Ministry of Commerce has proposed temporary registration and export controls on 40 technologies in artificial intelligence, biopharmaceuticals, and photovoltaics, and is seeking public comment on the draft. The proposal covers 23 AI-related technologies, 5 biopharma technologies, and 12 photovoltaic technologies, and would include key equipment carrying those technologies.

telegram · zaihuapd · Oct 16, 09:12

**「Background」** The Catalogue of Technologies Prohibited or Restricted from Export is China&\#x27;s main export-control list: technologies on it cannot be exported, or only under licence. The Ministry of Commerce&\#x27;s Oct. 16 notice opens public comment on a draft revision adding the 40 items, and Reuters reports that most AI technologies would remain freely exportable under the draft, with simplified licensing for open-source exports and overseas Chinese-run computing centres.

**「Impact」** If finalized, the proposal would add export-licensing requirements for 40 AI, biopharma, and photovoltaic technologies, creating new hurdles and potential delays for Chinese and foreign firms that license or transfer these technologies abroad, particularly to U.S. and other Western buyers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/asia-pacific/china-proposes-adding-40-ai-biotech-solar-technologies-export-control-list-2026-10-16/">China proposes adding 40 AI, biotech, solar technologies to ...</a></li>
<li><a href="https://www.independent.co.uk/asia/china/china-export-controls-ai-solar-biotech-us-trade-war-b3068046.html">China proposes export controls on AI, solar and biopharma ...</a></li>
<li><a href="https://www.wsj.com/economy/trade/china-proposes-export-controls-on-ai-technologies-75ac2030">China Proposes Export Controls on AI Technologies - WSJ</a></li>

</ul>
</details>

**Tags**: `#export-controls`, `#artificial-intelligence`, `#biotechnology`, `#photovoltaics`, `#china-regulation`

---

<a id="item-finance-news-3"></a>
### [Investors temper Anthropic IPO valuation expectations to $1.5 trillion](https://www.reuters.com/business/finance/investors-temper-anthropic-ipo-valuation-expectations-over-revenue-growth-2026-10-15/) ⭐️ 7.0/10

According to Reuters, some investors have cut their IPO valuation expectations for Anthropic to about $1.5 trillion from $2 trillion, citing slowing growth, intensifying model-price competition, and heavy computing costs even though the company reported $16.8 billion in third-quarter revenue, up 45% quarter over quarter, with adjusted profitability and positive quarterly cash flow.

telegram · zaihuapd · Oct 16, 15:46

**「Background」** Anthropic&\#x27;s private-market valuation had climbed to about $1.5 trillion by August 2026, a 25% increase over one month, and its founders were seeking 50.1% voting control ahead of a planned IPO after the valuation rose from $965 billion earlier in 2026.

**「Impact」** The valuation downgrade could pressure Chinese AI rivals preparing capital raises, such as DeepSeek, which is reportedly preparing a STAR Market IPO, and Moonshot, which raised at a reported $20B valuation, as investors focus on revenue durability, gross margins, and capital efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lteHJYZUVSRTZGVGJVRWRwSnJ5Z0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Anthropic prepares for potential initial public offering ...</a></li>
<li><a href="https://techbeat.co/story/anthropic-founders-seek-50-1-voting-control-ahead-of-expected-1-5-trillion-ipo">Anthropic Founders Seek 50.1% Voting Control Ahead of Expected ...</a></li>
<li><a href="https://andrew.ooo/answers/deepseek-vs-moonshot-vs-z-ai-vs-minimax-chinese-ai-ipo-race-september-2026/">DeepSeek vs Moonshot vs Z.ai vs MiniMax: China&#x27;s AI IPO Race</a></li>
<li><a href="https://entrepreneurloop.com/moonshot-ai-funding-20-billion-valuation-kimi-2026/">Moonshot AI Funding Hits $20B: Kimi&#x27;s 2026 Surge</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO估值`, `#AI行业`, `#财报`, `#估值预期`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Anthropic: Claude Mythos 5 Designs More Efficient Quantum Circuits](https://x.com/AnthropicAI/status/2111152183240511640) ⭐️ 8.0/10

In a tweet from October 16, 2026, Anthropic announced new work from its STEM Fellows Program on designing more efficient quantum circuits with Claude. According to the announcement, when given plain-language instructions, Claude Mythos 5 designed quantum circuits that improve on the best published ones, sometimes by an order of magnitude or more.

The tweet states that more efficient circuits reduce the resources needed by quantum algorithms, which could bring quantum computing applications in chemistry and materials science within reach sooner. Anthropic linked to a longer article for details, but the tweet itself does not explain the technical methodology. These claims are Anthropic&\#x27;s own announcement and are not independently verified in the available source material.

twitter · AnthropicAI · Oct 16, 17:47

**「Background」** Anthropic announced a new result from its STEM Fellows Program: Claude Mythos 5 designed quantum circuits that, based on plain-language instructions, improve on the best published versions, sometimes by an order of magnitude or more. The announcement frames this as significant because more efficient circuits reduce the resources required by quantum algorithms, potentially bringing quantum computing applications in chemistry and materials science closer. The linked Anthropic research post reports that Claude worked largely on its own in a closed loop with an automated evaluator. These are Anthropic&\#x27;s own reported results; the supplied material includes no independent verification or community comments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/designing-efficient-quantum-circuits">Designing more efficient quantum circuits with Claude \ Anthropic</a></li>
<li><a href="https://x.com/AnthropicAI/status/2111152183240511640">Anthropic on X: &quot;New from our STEM Fellows Program: Designing ...</a></li>
<li><a href="https://www.unite.ai/anthropic-says-claude-beat-best-published-quantum-circuit-designs/">Anthropic Says Claude Beat Best Published Quantum Circuit ...</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#AI research`, `#Claude`, `#Anthropic`, `#circuit design`

---

<a id="item-twitter-news-2"></a>
### [OpenAI Announces GPT-6 Astra Pro Upgrade with Parallel Multi-Agent Tasks](https://x.com/OpenAI/status/2111192259073094035) ⭐️ 7.0/10

OpenAI announced an upgrade to GPT-6 Astra Pro in ChatGPT. The update includes faster responses and improved use of plugins and tools. It also enables multiple agents to work on different parts of a task in parallel, with progress tracking and the ability to open completed tasks for review. The feature is available to Pro users in the Chat tab.

twitter · OpenAI · Oct 16, 20:27

**「Background」** OpenAI has been rapidly expanding the GPT-6 Astra ecosystem in recent weeks. An earlier Horizon summary dated 2026-09-30 records the introduction of “dot”s, which OpenAI described as always-on agents powered by GPT-6 Astra and built to handle everything, available to Pro, Business Premium, and Enterprise users in eligible markets. That same digest period also includes OpenAI’s announcement of GPT-6.1 Sol, positioned as a more cost-efficient model offering near-Astra intelligence, and the launch of an Ultrafast premium speed tier for GPT-6 Astra. Against this backdrop, the October 16, 2026 announcement extends the agentic push: Pro users in the Chat tab can now run multiple agents in parallel on different parts of a task, follow each agent’s progress, and open completed tasks to review their work, alongside faster responses and improved plugin and tool support.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/OpenAI/status/2104984504133918973">2026-09-30 — OpenAI Introduces “dots,” Powered by GPT-6 Astra</a></li>
<li><a href="https://x.com/OpenAI/status/2104986129686741046">2026-09-30 — OpenAI Announces GPT-6.1 Sol with Cost-Efficiency Claims</a></li>
<li><a href="https://x.com/OpenAI/status/2104993966043320759">2026-09-30 — OpenAI announces Ultrafast premium speed tier</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-6 Astra Pro`, `#AI product update`, `#multi-agent`, `#ChatGPT`

---