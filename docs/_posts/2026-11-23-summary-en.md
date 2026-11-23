---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 61 items, 18 important content pieces were selected

---

**Technology News**
1. [OpenAI Examines Perplexity as a Measure of Model Intelligence](#item-tech-news-1) ⭐️ 7.0/10
2. [O&\#x27;Reilly Essay Asks What Silicon Valley Should Optimize For](#item-tech-news-2) ⭐️ 7.0/10
3. [Analysis projects Anthropic 2028 power mix: 87% gas, 11% coal](#item-tech-news-3) ⭐️ 7.0/10
4. [FT alleges Prince Group-linked figure helped smuggle Nvidia chips to China](#item-tech-news-4) ⭐️ 7.0/10

**Technology Blog**
1. [Deliberate Flailing: A Heuristic for Uncertain Engineering Work](#item-tech-blog-1) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache v0.5.8 Release Summary](#item-ai-projects-1) ⭐️ 8.0/10
2. [LMCache v0.5.8 ROCm 7.2 Wheel for AMD Instinct](#item-ai-projects-2) ⭐️ 7.0/10
3. [LMCache v0.5.8 Intel XPU/SYCL Wheel](#item-ai-projects-3) ⭐️ 6.0/10
4. [LMCache v0.5.8-rbln: Rebellions NPU Wheel](#item-ai-projects-4) ⭐️ 6.0/10
5. [LMCache Nightly ROCm 7.2 Wheels](#item-ai-projects-5) ⭐️ 5.0/10
6. [LMCache nightly RBLN wheel \(2026-11-22\)](#item-ai-projects-6) ⭐️ 5.0/10
7. [LMCache Nightly: CUDA 13.0 Wheels for Linux](#item-ai-projects-7) ⭐️ 5.0/10
8. [LMCache v0.5.8 ROCm Wheel Release](#item-ai-projects-8) ⭐️ 5.0/10

**Financial News**
1. [US tech selloff triggers Asian market-stabilization measures](#item-finance-news-1) ⭐️ 9.0/10
2. [China Urges US to Withdraw Phone-Number Access Limits](#item-finance-news-2) ⭐️ 7.0/10
3. [Record El Niño ocean warming raises pressure on food aid](#item-finance-news-3) ⭐️ 7.0/10

**Twitter News**
1. [Making AI Agents Prove They’re Done: Five Verification Practices](#item-twitter-news-1) ⭐️ 7.0/10
2. [OpenAI&\#x27;s Perplexity Curves and the Shift to Post-Training](#item-twitter-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Examines Perplexity as a Measure of Model Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 7.0/10

OpenAI published an article on Nov. 22 examining the relationship between perplexity and intelligence in language models, with cross-entropy and benchmark progress as the technical context. The supplied material describes no new model, product, or independently measured result, so the piece is explanatory rather than a claimed capability breakthrough.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**「Background」** Perplexity is the exponentiated cross-entropy loss of a language model&\#x27;s next-token predictions — a measure of how surprised the model is by each token in a sequence, where 1 corresponds to perfect prediction and the vocabulary size to random guessing. OpenAI chief scientist Jakub Pachocki&\#x27;s essay treats perplexity and cross-entropy loss as equivalent and argues for using the metric as a common yardstick to compare model developers and inform shared safety standards.

**「Impact」** For model evaluators, the discussion highlights a concrete limitation: perplexity is a next-token prediction score bounded between 1 and vocabulary size, and a model specialized on one domain can have high general perplexity while still performing well there. That makes it a compression-style signal to read alongside task-specific benchmarks, not a standalone intelligence score.

**「Community Discussion」** One commenter noted that the article does not define perplexity and supplied the standard definition—next-token surprise, with 1 as the best case and vocabulary size as the worst—while others debated its significance. One argued that prediction and compression are exactly the right metric for world-model learning; another was skeptical that abilities “emerge” at specific perplexity thresholds because small math-specialized models can have high general perplexity; and a third was surprised that cross-entropy loss still shows such a clear trend amid RL-based training.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#perplexity`, `#language models`, `#cross-entropy`, `#AI benchmarks`, `#OpenAI`

---

<a id="item-tech-news-2"></a>
### [O&\#x27;Reilly Essay Asks What Silicon Valley Should Optimize For](https://www.oreilly.com/radar/what-happened-to-silicon-valley/) ⭐️ 7.0/10

An O&\#x27;Reilly Radar essay published Nov. 22 examines Silicon Valley&\#x27;s evolution through capitalism, incentive design, and the industry&\#x27;s shift toward AI. It argues that the tech sector&\#x27;s direction is shaped by the incentives it builds around, and it asks what the industry should optimize for instead. The piece is commentary rather than an announcement of a product, policy, or measured technical result.

hackernews · greenyouse · Nov 22, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50602947)

**「Background」** The essay draws on Tim O&\#x27;Reilly&\#x27;s lecture at Johns Hopkins University on October 16, 2026, which traced Silicon Valley&\#x27;s move from customer-centered innovation toward extraction driven by shareholder capitalism, monopoly ambitions, and hype, linking that shift to the current AI boom. Its argument turns on mechanism design — the idea that technology&\#x27;s value depends on the rules, incentives, and interfaces around it — which the essay frames as &quot;reverse game theory&quot;: asking what game we ought to be playing rather than how to win the one we are in.

**「Community Discussion」** Commenters largely endorsed the essay&\#x27;s call to scrutinize incentives: one described mechanism design as &quot;reverse game theory&quot; and argued the key question is what game humanity ought to play, while another traced current behavior to the zero-interest-rate era and said AI spending now risks cannibalizing companies&\#x27; core businesses. A more skeptical commenter dismissed &quot;VC influencers&quot; as self-serving and questioned whether Silicon Valley ever had integrity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.oreilly.com/radar/what-happened-to-silicon-valley/">What Happened to Silicon Valley? – O’Reilly</a></li>
<li><a href="https://news.lavx.hu/article/tim-o-reilly-traces-silicon-valley-s-shift-from-value-creation-to-extraction">Tim O&#x27;Reilly Traces Silicon Valley&#x27;s Shift From Value ...</a></li>

</ul>
</details>

**Tags**: `#Silicon Valley`, `#tech industry`, `#mechanism design`, `#venture capital`, `#AI`

---

<a id="item-tech-news-3"></a>
### [Analysis projects Anthropic 2028 power mix: 87% gas, 11% coal](https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/) ⭐️ 7.0/10

A Better Data Center Project analysis projects that 87% of Anthropic’s power will come from natural gas and 11% from coal in 2028, leaving about 2% unaccounted for in the headline breakdown. The article is an analysis of projected AI data-center energy sourcing and its environmental costs, not a report of a new Anthropic energy commitment.

hackernews · happosai · Nov 22, 08:57 · [Discussion](https://news.ycombinator.com/item?id=50597612)

**「Why Anthropic&\#x27;s power mix is tied to Memphis」** Anthropic&\#x27;s projected 2028 electricity mix is largely a consequence of where it bought compute: in May 2026 it announced a deal with xAI parent SpaceX to use all of the compute capacity at Colossus 1, part of xAI&\#x27;s data-center cluster in the Memphis, Tennessee–Southaven, Mississippi area. Reporting has noted that Anthropic has not directly addressed Memphis residents&\#x27; concerns about pollution and water use, and that its green commitments have centered on joining the Frontier carbon-removal coalition in June 2026 rather than on renewable power procurement. That makes the grid mix of a leased, fossil-heavy campus the relevant baseline for the 87% gas and 11% coal figures.

**「Site-level power sourcing」** Because Anthropic&\#x27;s capacity is largely contracted from third parties — former crypto miners, data-center startups, chipmakers and hyperscalers — an organization&\#x27;s location-based emissions from using its models will track whichever host sites serve the workload, not a single company-wide figure. Buyers and sustainability teams should expect site-level power-mix data, since the same provider&\#x27;s footprint varies sharply between gas-heavy US sites and lower-carbon grids such as the French data center cited in discussion of a 95% low-carbon mix.

**「Community Discussion」** Commenters condemned Anthropic over its leasing of Colossus 1 and alleged local pollution in Memphis, and criticized the company for making no U.S. renewable commitments; others argued that regulation is needed because purely financial accounting ignores environmental and social costs. One commenter also said the scale of data-center energy use is hard for most people to visualize.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_%28data_center%29">Colossus (data center) - Wikipedia</a></li>
<li><a href="https://www.eenews.net/articles/anthropic-moves-into-musks-memphis-data-center/">Anthropic moves into Musk’s Memphis data center</a></li>
<li><a href="https://www.thebureauinvestigates.com/stories/2026-08-14/misaligned-colossus-musks-data-empire-anthropic">How Musk’s toxic data empire is powering Anthropic’s ...</a></li>
<li><a href="https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/">How AI is powered : a breakdown of BYOP and grid power</a></li>
<li><a href="https://news.ycombinator.com/item?id=50597612">87% of the Anthropic power will come from gas and 11% from coal in...</a></li>
<li><a href="https://www.nytimes.com/2026/11/02/technology/anthropic-ai-computing-power.html">Inside Anthropic ’s Hunt for A.I. Computing Power - The New York...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#energy`, `#sustainability`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [FT alleges Prince Group-linked figure helped smuggle Nvidia chips to China](https://www.ft.com/content/f3ad8a81-3890-4a8a-8853-ff0a94b08ba9?syn-25a6b1a6=1) ⭐️ 7.0/10

An FT report, summarized in a Telegram post, alleges that Hu Xiaowei—described by the U.S. Treasury as the &quot;number two&quot; figure in Cambodia&\#x27;s Prince Group—helped move Nvidia chips into China through shell companies, underground financing, and private aircraft. Citing trade data, the report says a Malaysian subsidiary of Megaspeed declared about $4.6 billion in imported goods between December 2024 and December 2025, with some chips alleged to have reached China&\#x27;s black market. Prince Group denied that Hu worked for it and said the allegations about an illegal network and private-aircraft smuggling lacked factual basis. The claims remain allegations, and the item is a secondhand summary of the FT report.

telegram · zaihuapd · Nov 22, 04:34

**「Background」** The Megaspeed thread predates the FT report: Horizon&\#x27;s Nov. 18 digest reported that the U.S. Commerce and Justice departments had issued a joint statement describing a 2024 export-control and criminal investigation into Singapore-based Megaspeed, including a May 2025 request to Nvidia for its sales records to the company and Nvidia&\#x27;s June 2025 decision to place Megaspeed on a no-sale list. That investigation is the regulatory backdrop for the FT report&\#x27;s focus on a Malaysian Megaspeed subsidiary.

**「Impact」** The allegation gives export-control investigators a specific trail to examine: the Malaysian subsidiary&\#x27;s declared imports, the alleged shell-company network, and the claimed private-aircraft route. Because Prince Group denies the claims and no wrongdoing has been established, any compliance or enforcement exposure remains potential rather than confirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.commerce.gov/sites/default/files/2026-11/DOC-DOJ-Joint-Statement.pdf">2026-11-18 — US Commerce and DOJ issue joint statement on Megaspeed export-control investigation</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#chip smuggling`, `#export controls`, `#semiconductor supply chain`, `#Cambodia`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Deliberate Flailing: A Heuristic for Uncertain Engineering Work](https://seangoedecke.com/when-in-doubt-flail-about/) ⭐️ 6.0/10

rss · Sean Goedecke · Nov 23, 00:00

**「Background」** Sean Goedecke argues that when guidance is unclear—whether in a new product, a tangled system, or an organizational impasse—waiting for a clearer picture is usually worse than deliberately experimenting. He concedes the approach is risky: badly handled, it can look like a stream of bad ideas and damage an engineer’s reputation.

**「Solution」** The method is to try many different things, attend carefully to feedback from colleagues and actual results, and ruthlessly drop plans that are not getting a positive response. A portfolio of attempts matters because most plans will fail and because it prevents overinvestment in any one idea. Goedecke applies this in three settings. In product work, he cites GitHub Models \(now retired\), where many features failed but running AI inference from a GitHub Actions token proved surprisingly sticky and seeded “Continuous AI.” In engineering, instead of exhaustively mapping a large, fast-changing system, he favors speculative changes—AI agents can generate several refactors to skim—then dropping anything that does not improve matters and investigating anything that does. In organizational work, senior engineers can automate manual tasks, volunteer for work, or propose long-term plans; most will miss, but the effort can build trust if failing plans are dropped immediately rather than defended. He calls it “flailing” because it feels like repeated failure from the inside, even when managers see proactive experimentation.

**「Takeaway」** Goedecke’s thesis is that feedback-sensitive experimentation is often the fastest route to understanding in genuinely uncertain situations, provided the experimenter tolerates the feeling of failure and abandons losing plans quickly. The discomfort of flailing is a signal to manage, not a sign that the approach is wrong.

**Tags**: `#engineering judgment`, `#experimentation`, `#feedback loops`, `#organizational dynamics`, `#uncertainty`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache v0.5.8 Release Summary](https://github.com/LMCache/LMCache/releases/tag/v0.5.8) ⭐️ 8.0/10

LMCache v0.5.8 is a production-focused release for its LLM KV-cache runtime, expanding multiprocess cache architecture, strengthening cache identity across requests, model revisions, LoRA adapters, and tensor-parallel residency, while adding RDMA peer transfer, serving compatibility, and endpoint security.

github · travisVux · Nov 22, 15:39

**「Problem Solved」** Distributed LLM inference caching can suffer from cache-identity collisions, fragile multiprocess services, and slow peer-to-peer KV movement. This release restructures the multiprocess runtime, tightens cache identity for tagged requests, model revisions, LoRA adapters, and tensor-parallel KV residency, and expands RDMA-based transfer. It also hardens service boundaries with API-key authentication and loopback-only coordinator binding by default.

**「Background and impact」** LMCache is a KV-cache management layer for LLM inference that extends serving engines such as vLLM with multi-tier storage across GPU memory, CPU memory, and disk or remote backends, so cached blocks can be reused across requests and engines \[tool-1-2\]\[tool-1-3\]. It is designed for workloads where long prompts, conversation history, and retrieved content are reused \[tool-1-1\]. In that ecosystem, v0.5.8 is a production-hardening release: the notes emphasize a more modular multiprocess runtime, stronger cache identity across requests, model revisions, LoRA adapters, and tensor-parallel residency, expanded RDMA peer-to-peer transfer, serving compatibility, and API-key/coordinator security controls. It is an incremental release rather than a foundational breakthrough, but it matters because KV-cache reuse and movement are central to production LLM serving efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li><a href="https://docs.lmcache.ai/developer_guide/architecture.html">Architecture Overview | LMCache</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#KV cache`, `#inference`, `#distributed`, `#RDMA`, `#serving`, `#multiprocess`, `#CUDA`, `#security`

---

<a id="item-ai-projects-2"></a>
### [LMCache v0.5.8 ROCm 7.2 Wheel for AMD Instinct](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rocm) ⭐️ 7.0/10

LMCache published a ROCm 7.2 wheel for v0.5.8, built for AMD Instinct MI300X/MI325X and MI350X/MI355X and ABI-matched to the upstream vLLM ROCm container \(torch 2.13, cp312\).

github · github-actions\[bot\] · Nov 22, 17:35

**「Problem Solved」** Running LMCache&\#x27;s KV-cache serving layer on AMD ROCm GPUs previously required a build that matched the vLLM container&\#x27;s ABI and GPU architecture. This release supplies a prebuilt wheel for gfx942 and gfx950, ABI-matched to the upstream vLLM ROCm image, reducing source-build steps and deployment friction from version or ABI mismatches.

**「Background &amp; Impact」** LMCache sits in the vLLM serving stack as a KV-cache layer. Where vLLM&\#x27;s own prefix caching reuses KV state only within a single node, LMCache adds a distributed cache so multiple vLLM workers on different machines can share the same KV cache over Ethernet, RDMA, or NVLink, eliminating redundant prefill across replicas in a multi-replica cluster \(tool-1-2\). Adoption is deliberately low-friction — a one-line code change in vLLM unlocks far more KV-cache storage for multi-turn conversation and document QA workloads \(tool-1-3\) — and LMCache MP mode can also run as a standalone cache service decoupled from vLLM, allowing cache capacity to scale independently \(tool-1-1\).

Against that backdrop, v0.5.8-rocm is primarily a packaging and platform-enablement release rather than a core architectural change. It ships a ROCm 7.2 wheel built for AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), ABI-matched to the upstream vllm/vllm-openai-rocm image \(torch 2.13, cp312\), so the layer can be installed directly into an existing vLLM ROCm container with --no-deps. The practical effect is that the same distributed KV-cache sharing and offload machinery becomes available on AMD data-center GPUs, which matters as vLLM deployments diversify across accelerator vendors and operators need cache tiers that match their serving image rather than being tied to one hardware stack.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for... | DataCamp</a></li>
<li><a href="https://www.spheron.network/blog/deploy-lmcache-vllm-kv-cache-sharing-gpu-cloud/">Deploy LMCache on GPU Cloud: Share KV Cache Across vLLM ...</a></li>
<li><a href="https://blog.lmcache.ai/2024-09-23-pip-install/">Are you a vLLM user? Change just ONE line of code to unlock...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#ROCm`, `#vLLM`, `#KV cache`, `#AMD Instinct`, `#wheel`, `#inference serving`

---

<a id="item-ai-projects-3"></a>
### [LMCache v0.5.8 Intel XPU/SYCL Wheel](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-xpu) ⭐️ 6.0/10

The v0.5.8-xpu release packages LMCache v0.5.8 as an Intel XPU/SYCL wheel for upstream Intel vLLM XPU containers. It is a platform-specific binary build, not a new core feature or performance release.

github · github-actions\[bot\] · Nov 22, 17:35

**「Problem Solved」** It reduces deployment friction for LMCache’s KV-cache layer on Intel XPU systems by providing a prebuilt wheel compatible with an Intel vLLM XPU container. The wheel is built against a pinned torch-xpu and oneAPI toolchain and binds at runtime to host oneAPI/SYCL libraries, avoiding the need to assemble that platform-specific package from source.

**「Ecosystem context」** LMCache v0.5.8-xpu is a platform-specific wheel rather than a new core release: it packages the existing LMCache KV-cache layer for Intel XPU/SYCL, built against a pinned torch-xpu + oneAPI toolchain and intended for installation into an upstream Intel vLLM XPU container. The source provides no new feature, performance, or architecture claims; the main change is availability on Intel hardware.

That matters because LMCache sits in the inference-serving stack as a KV-cache connector/reuse layer for vLLM-style deployments. vLLM&\#x27;s optimization guidance lists LMCache&\#x27;s multi-process connector among KV-cache connector options \[tool-1-1\], and Intel&\#x27;s llm-scaler vLLM documentation describes starting LMCache with vLLM and tuning cache/chunk settings \[tool-1-2\]. The broader premise—retrieving a saved KV cache instead of recomputing it—is also the kind of tradeoff LMCache has publicly discussed \[tool-1-3\]. This XPU wheel therefore extends an existing ecosystem component to Intel accelerators; it does not by itself establish new capabilities or performance gains.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/configuration/optimization/">Optimization and Tuning - vLLM</a></li>
<li><a href="https://github.com/intel/llm-scaler/blob/main/vllm/README.md">llm-scaler/ vllm /README.md at main · intel /llm-scaler · GitHub</a></li>
<li><a href="https://teapawt.org/lmcache">LMCache Lab (@ lmcache ) | teapawt</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#Intel XPU`, `#SYCL`, `#vLLM`, `#inference serving`, `#packaging`, `#release`

---

<a id="item-ai-projects-4"></a>
### [LMCache v0.5.8-rbln: Rebellions NPU Wheel](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rbln) ⭐️ 6.0/10

A Rebellions RBLN NPU-specific build of LMCache v0.5.8, compiled against torch-rbln 0.12.0 \(torch 2.13.0+cpu\). It lets users install the LLM KV-cache layer on RBLN hardware via pip, while torch-rbln, rebel-compiler, and the RBLN driver remain host-owned rather than bundled.

github · github-actions\[bot\] · Nov 22, 17:35

**「Problem Solved」** Getting a KV-cache system onto a specialized NPU normally means either building from source or accepting a wheel that drags in its own copies of the vendor runtime. Bundling torch-rbln, rebel-compiler, and the RBLN driver would pin those components inside the package and risk clashing with the versions and drivers already installed on the host. This release ships only the LMCache build, so it installs into an environment that already has torch-rbln and rebel-compiler present \(for example via \`pip install lmcache==0.5.8+rbln --find-links &lt;release assets URL&gt;\`\), keeping the vendor toolchain and driver under host control.

**「Background」** LMCache sits in the LLM serving stack as a KV-cache layer: it reuses cached KV states for repeated text, not only strict prefixes, to avoid redundant prefill work and cut time to first token, and it extends GPU memory with multi-tier storage for long-context workloads \(tool-1-2, tool-1-3\). Its stated design also spans network and storage tiers for scaling KV caches \(tool-1-1\). This v0.5.8-rbln artifact is a platform-specific distribution update rather than a core feature release: an \`lmcache==0.5.8+rbln\` wheel built against torch-rbln 0.12.0 \(torch 2.13.0+cpu\) for Rebellions RBLN NPUs. Notably, torch-rbln, rebel-compiler, and the RBLN driver remain host-owned and are not bundled, so installation assumes an environment already containing them. The practical impact is that LMCache is being packaged for an additional accelerator target, broadening where its KV-cache reuse can be deployed; the supplied material contains no new architecture, benchmark data, or major feature changes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=rINy7mFyRAU">Introducing LMCache - YouTube</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for... | DataCamp</a></li>
<li><a href="https://github.com/neeltom92/lmcache">neeltom92/ lmcache : Supercharge Your LLM with the Fastest KV ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#KV cache`, `#inference`, `#NPU`, `#Rebellions`, `#release`, `#hardware acceleration`

---

<a id="item-ai-projects-5"></a>
### [LMCache Nightly ROCm 7.2 Wheels](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels of LMCache, built from the dev branch for AMD Instinct gfx942/gfx950 and ABI-matched to the upstream vLLM ROCm container \(torch 2.13, cp312\), are published for installation into that serving environment.

github · github-actions\[bot\] · Nov 22, 07:45

**「Problem Solved」** The pain point is platform and ABI alignment: LMCache must match ROCm GPU targets, Python cp312, torch 2.13, and the upstream vLLM ROCm image. Prebuilt nightly wheels let engineers install LMCache into that container without resolving those compatibility details themselves. The release makes no performance or capability claims beyond platform/ABI compatibility.

**「Background」** LMCache is a KV-cache layer for LLM serving, so its wheels must match both the serving engine&\#x27;s ABI and the target accelerator stack. This entry is a routine nightly build rather than a feature or optimization release: it keeps LMCache installable inside AMD&\#x27;s ROCm vLLM container for gfx942/gfx950 Instinct GPUs, pinned to \`0.5.8.dev221+rocm7.2\` and installed with \`--no-deps\` to reuse the container&\#x27;s torch 2.13/cp312 environment. In the broader ecosystem, AMD and LMCache have positioned KV-cache reuse and offload as a way to improve vLLM serving on Instinct; an earlier LMCache post reported 3–10x gains on MI300X for several model families when integrated with vLLM \[tool-1-1\]. AMD also maintains a separate disaggregated KV-cache stack, ROCm AIC, spanning MI300X/MI350 and later MI450/Helios \[tool-1-2\]\[tool-1-3\]. Those points are context, not claims about this nightly build.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.lmcache.ai/en/2026/01/09/amd-x-lmcache-amd-gpu-acceleration-with-lmcache/">AMD × LMcache: AMD GPU Acceleration with LMcache</a></li>
<li><a href="https://github.com/ROCm/rocm-aic">GitHub - ROCm/rocm-aic: ROCm AMD Infinity Context - A ...</a></li>
<li><a href="https://rocm.blogs.amd.com/software-tools-optimization/amd-infinity-context/README.html">Introducing ROCm™ AMD Infinity Context: A Purpose-Built KV ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#KV cache`, `#serving`, `#vLLM`, `#ROCm`, `#AMD Instinct`, `#nightly build`, `#packaging`

---

<a id="item-ai-projects-6"></a>
### [LMCache nightly RBLN wheel \(2026-11-22\)](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

Nightly LMCache wheel built from \`dev\` for Rebellions RBLN NPUs, targeting torch-rbln 0.12.0 with torch 2.13.0+cpu. The wheel leaves torch-rbln, rebel-compiler, and the RBLN driver host-owned, and installs into an environment where those components are already present.

github · github-actions\[bot\] · Nov 22, 07:39

**「Problem solved」** Deploying LMCache on an NPU backend requires matching the runtime and compiler versions. This wheel provides a platform-specific package without bundling vendor components, avoiding conflicts and keeping the host toolchain authoritative. Users must preinstall torch-rbln and rebel-compiler; this is a nightly packaging artifact, not a feature or performance release.

**「Ecosystem context」** LMCache is documented as a KV cache management layer for LLM inference that extends engines such as vLLM with multi-tier KV cache storage across GPU memory, CPU memory, and disk or remote backends, making cached state reusable across serving engines. This nightly item is not a feature or architecture release; it is a platform-specific wheel for Rebellions RBLN NPUs, built against torch-rbln 0.12.0. Its ecosystem role is distribution reach: torch-rbln is a PyTorch extension for using Rebellions NPU compute, and rebel-compiler is required but not bundled with torch-rbln, so LMCache keeps those dependencies host-owned and installs into an already provisioned RBLN environment. The impact is therefore modest and infrastructure-oriented—another accelerator packaging target for LMCache rather than a major update to its KV cache capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.lmcache.ai/developer_guide/architecture.html">Architecture Overview | LMCache</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch - rbln · PyPI</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">RBLN -SW/ torch - rbln : PyTorch extension for Rebellions NPU · GitHub</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly build`, `#packaging`, `#torch-rbln`

---

<a id="item-ai-projects-7"></a>
### [LMCache Nightly: CUDA 13.0 Wheels for Linux](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache&\#x27;s nightly release publishes pre-release CUDA 13.0 wheels for linux/amd64 and linux/arm64, built from the dev branch on 2026-11-22, plus an install command using PyTorch&\#x27;s cu130 wheel index.

github · github-actions\[bot\] · Nov 22, 09:28

**「Problem Solved」** It gives engineers a direct way to install LMCache&\#x27;s dev-branch build for CUDA 13.0 on both Linux architectures instead of building from source. This is a packaging/CI update; the source lists no feature or performance changes.

**「Background」** LMCache describes itself as a KV cache management layer for LLM inference, built around cache reuse, offloading, compression, and serving optimization \(tool-1-2\). In practice that means cached KV states can be made available across multiple inference workers instead of staying tied to a single model process \(tool-1-1\), and can be reused across GPU, CPU DRAM, and local disk \(tool-1-3\). That places the project in the serving-infrastructure layer of the LLM stack, where cache reuse is a lever for memory pressure and throughput rather than a model-level capability.

This item is a nightly build rather than a feature release: CUDA 13.0 wheels built from the \`dev\` branch on 2026-11-22 for linux/amd64 and linux/arm64, installed with \`--pre\` and pointed at PyTorch&\#x27;s cu130 wheel index. Nightlies typically serve users who need to track unreleased changes or validate compatibility with newer CUDA/PyTorch toolchains. The item itself carries no changelog, performance numbers, or feature details, so its practical impact is confined to packaging and CI availability.

The broader significance is ecosystem alignment: downstream KV-cache and serving projects need wheels that match the CUDA/PyTorch builds their users run, and a cu130 nightly is part of maintaining that install path. Beyond that, this release says little about LMCache&\#x27;s roadmap or runtime performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/a0x8o/lmcache">GitHub - a0x8o/ lmcache : LMCache : Supercharge Your LLM with the...</a></li>
<li><a href="https://landscape.jimmysong.io/projects/lmcache/">LMCache | AI Native Landscape</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#LLM inference`, `#KV cache`, `#CUDA`, `#nightly release`, `#packaging`

---

<a id="item-ai-projects-8"></a>
### [LMCache v0.5.8 ROCm Wheel Release](https://github.com/LMCache/LMCache/releases/tag/v0.5.8-rocm-torch210) ⭐️ 5.0/10

LMCache v0.5.8 ROCm wheel is a prebuilt AMD-compatible package for the existing release, pinned to ROCm 7.2.4 and PyTorch 2.10.0. It ships gfx942/gfx950 code objects and LMCache integrations, enabling installation in a matching AMD PyTorch container.

github · github-actions\[bot\] · Nov 22, 17:35

**「Problem Solved」** AMD GPU users can hit ABI mismatches when building LMCache from source against ROCm and PyTorch. This wheel removes that build step by pinning the exact torch runtime, ROCm version, Python/platform tag, C++ ABI, and GPU code objects, so installation is limited to a matching container but avoids local compilation. It is a packaging release, not a new core feature update.

**「Ecosystem context」** LMCache sits in the LLM serving stack as a KV-cache layer: it stores reusable KV caches so serving engines can reuse them across requests and even across vLLM instances \(tool-1-3\). That matters more as vLLM supports multiple GPU backends, including AMD ROCm \(tool-1-2\); AMD benchmark work has shown vLLM plus LMCache on MI300X using the ROCm LMCacheConnector V1 path \(tool-1-1\). This v0.5.8-rocm-torch210 build is therefore an ecosystem-enablement release, not a core feature release: it pins the ROCm 7.2.4 / PyTorch 2.10 / Python 3.12 / C++ ABI combination and ships gfx942/gfx950 code objects, making AMD installation reproducible against a named container.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/upto-107x-speedup-llm-inference-lmcache-rohan-paul-ibxkf">Upto 10.7X speedup on LLM inference with LMCache</a></li>
<li><a href="https://docs.vllm.ai/en/latest/getting_started/installation/gpu/">GPU - vLLM</a></li>
<li><a href="https://github.com/EmbeddedLLM/LMCache-ROCm">GitHub - EmbeddedLLM/ LMCache - ROCm : ROCm support of...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#ROCm`, `#AMD GPU`, `#release packaging`, `#wheel`

---

## Financial News

<a id="item-finance-news-1"></a>
### [US tech selloff triggers Asian market-stabilization measures](https://news.bjd.com.cn/2026/11/22/12039852.shtml) ⭐️ 9.0/10

US AI-related technology stocks sold off sharply on Friday, with the Nasdaq falling 5.28% in a single session and the Philadelphia Semiconductor Index dropping nearly 11%. Asian markets responded with market-stabilization and trading-rule measures: mainland China cut its minimum margin-financing ratio to 80%, South Korea eased daily buyback-order limits for listed companies for three months from Nov. 24, and Taiwan banned short selling below the closing price from Nov. 23 while raising its securities-lending margin ratio to 150% from 130%.

telegram · zaihuapd · Nov 22, 13:24

**「Background」** The selloff began on Wall Street on Nov. 20, when worries that the AI investment boom is slowing triggered heavy selling: the tech-heavy Nasdaq 100 fell 5.6% that day and 10.4% for the week, its worst week in more than six years, while the Philadelphia Semiconductor Index dropped 10.7% and was down 43% from its June peak, according to Guanchazhe \(tool-1-1\). The measures now being rolled out in Asia use levers such as margin requirements — the share of a trade an investor must fund from their own pocket — and restrictions on short-selling, which is betting that a stock will fall.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guancha.cn/GuoJi%C2%B7ZhanLue/2026_11_21_909399.shtml">AI 恐慌爆发，华尔街震荡，美国 科 技 股 跌 入熊市</a></li>

</ul>
</details>

**Tags**: `#US tech stocks`, `#market disruption`, `#Asian markets`, `#regulatory response`, `#short-selling rules`

---

<a id="item-finance-news-2"></a>
### [China Urges US to Withdraw Phone-Number Access Limits](https://www.bloomberg.com/news/articles/2026-11-22/china-objects-to-us-curbs-on-telecoms-access-to-phone-numbers) ⭐️ 7.0/10

China&\#x27;s Commerce Ministry on Nov. 22 urged the US to withdraw a measure barring China Mobile, China Telecom and China Unicom from directly obtaining US phone numbers, saying it violates non-discrimination and fair-competition principles and that the FCC cited national-security risks without factual basis. The FCC voted on Nov. 19 to tighten security requirements for VoIP providers seeking direct access to US numbers, adding national-security certification intended to block entities, equipment and services on its Covered List.

telegram · zaihuapd · Nov 22, 06:44

**「Background」** The U.S. Federal Communications Commission adopted the restriction on Nov. 19, 2026, requiring interconnected VoIP providers—internet-based phone services linked to the public phone network—that seek direct access to U.S. numbers to certify that they do not rely on equipment or services on the FCC’s Covered List of national-security risks.

**「Who is affected」** The restriction directly targets China Mobile, China Telecom and China Unicom, which lose direct access to U.S. phone numbers, leaving U.S. carriers and cross-border callers dependent on intermediary providers to complete calls between the two countries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fcc.gov/document/fcc-cracks-down-bad-actors-access-us-phone-numbers-0">FCC Cracks Down on Bad Actors&#x27; Access to U.S. Phone Numbers</a></li>
<li><a href="https://fccid.io/news/fcc-voip-direct-number-access-covered-list-certifications-fcc-26-82">FCC 26-82: New National Security Rules for VoIP Number Access</a></li>
<li><a href="https://www.globaltimes.cn/page/202611/1374802.shtml">China urges US to revoke proposed telecom restrictions , warns of...</a></li>
<li><a href="https://www.foxbusiness.com/politics/fcc-bans-chinese-firms-direct-access-us-phone-numbers-bid-curb-robocalls">FCC regulators bar Chinese telecom giants from direct number access</a></li>

</ul>
</details>

**Tags**: `#美中关系`, `#电信监管`, `#FCC`, `#中国商务部`, `#国家安全`

---

<a id="item-finance-news-3"></a>
### [Record El Niño ocean warming raises pressure on food aid](https://www.wired.com/story/how-this-years-super-el-nino-will-worsen-global-hunger/) ⭐️ 7.0/10

Tropical Pacific warming used to measure El Niño reached 3.5°C in October, breaking the previous record of about 2.75°C and forecast to peak near 4°C in early winter, climate scientist Zeke Hausfather said. The World Food Programme warned in August that this El Niño could push an additional 49 million people into acute food insecurity by the end of 2027, bringing the total to 274 million.

telegram · zaihuapd · Nov 22, 14:09

**「Background」** The 2026–2027 El Niño was declared by the World Meteorological Organization on 2 June 2026 and is already classified as a “very strong”—or Super—El Niño, with Pacific temperatures exceeding those of the 1997 and 2015 events. El Niño is measured by abnormal warming of the tropical Pacific; such warming can shift rainfall and crop conditions far from the ocean, which is the link between this climate event and food insecurity.

**「Impact」** Aid agencies facing a 30% drop in global funding in 2025 from the 2022 peak may be less able to reach affected households; during a similar drought in Somalia, the World Food Programme said it could cover fewer than 1 million people, down from 10 million.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026%E2%80%932027_El_Ni%C3%B1o_event">2026–2027 El Niño event - Wikipedia</a></li>
<li><a href="https://news.un.org/en/story/2026/10/1168537">From drought to deluge: ‘Super’ El Niño’s expanding reach</a></li>

</ul>
</details>

**Tags**: `#厄尔尼诺`, `#粮食安全`, `#人道援助`, `#气候风险`, `#经济影响`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Making AI Agents Prove They’re Done: Five Verification Practices](https://x.com/dotey/status/2124603209394078089) ⭐️ 7.0/10

In a thread on X, practitioner 宝玉 \(dotey\) addresses a familiar failure mode for people using AI coding agents: the agent confidently reports that work is complete and verified, but the result fails after release. The author argues the problem is not simply agent dishonesty or carelessness, but how users ask agents to verify. Agents often lack a concrete definition of “done,” and users lack a cheap way to confirm the claim. The thread offers five practices drawn from the author’s experience; it is practitioner commentary rather than a controlled study or a report of measured results.

First, the author warns against relying on adversarial verification, where one or more reviewer agents critique the output and the executing agent iterates until approval. In practice this can fail to converge, especially with weaker models, and may consume tokens while making the output worse. The stated cause is the absence of a shared acceptance standard: reviewer agents may lack full context and invent their own criteria, which the executing agent then follows.

Second, define clear acceptance criteria and provide an environment where the agent can test against them. The author’s example is converting design mockups into a web page: a vague request produces an approximate result, while asking the agent to screenshot the page and compare it pixel by pixel against the mockup pushes it to build comparison tooling and iterate. The author notes that pixel-perfect output is often unnecessary; the point is that the agent knows the standard and has a way to check itself.

Third, validate earlier because rework gets more expensive later. The author says this is long-standing software engineering wisdom that becomes easy to forget when Vibe Coding lowers the cost of generating code. The thread names three pre-implementation gates: feasibility analysis \(is the project worth doing, will anyone use it, what is the return on investment\), prototype development \(build a low-cost runnable prototype with mock data to test direction, citing tools such as Claude Design or a local alternative\), and system design \(technology choices, module boundaries, data structures, database design, and API schema\). The author recommends having the agent write a technical design document before implementation so the user can understand the approach and correct problems early.

Fourth, reduce the human cost of acceptance by asking the agent for evidence. The author insists humans remain in the loop and says fully delegating review is likely to produce “AI Slop,” but human review capacity is a bottleneck. Suggested evidence includes screenshots of new features, before-and-after screenshots for bug fixes, and dynamically generated screenshots of different scenarios using simulated API responses. Screenshots, screen recordings, and visual HTML reports let a person spot problems at a glance, and the act of taking screenshots can also surface issues to the agent.

Fifth, focus code review on issues that matter. Because agents generate code quickly, review and verification become the bottleneck. The author recommends keeping pull requests small, using agents to review but not trusting their conclusions wholesale, grading findings so humans focus on P0 and P1 issues—especially security and performance—and letting minor style or best-practice comments go.

The thread’s conclusion ties the practices together: an agent’s claim of completion should not be treated as a conclusion but converted into something the user can inspect. Define “done” before work starts, validate direction with prototypes and design documents, require screenshots and comparisons as proof after work, and spend human attention on the most consequential problems. The source does not include quantitative evidence, tool benchmarks, or a detailed implementation guide, and no community comments were available with the item.

twitter · 宝玉 · Nov 22, 20:37

**「Background: Making Agent Verification Trustworthy」** On 2026-11-22, practitioner 宝玉 \(@dotey\) published a thread on X arguing that the recurring failure mode with coding agents — an agent confidently reports “验证完了” \(“verified”\) and then ships broken work — is less a honesty problem than a verification-design problem. The thread&\#x27;s framing is that agents are not given a definition of “done,” and users lack a low-cost way to confirm the claim. It offers five practices: avoid adversarial multi-agent review loops, which often fail to converge; specify acceptance criteria plus an environment where the agent can check itself \(for example, screenshot pixel diffs against a design\); validate early through feasibility analysis, prototyping, and system design; require evidence such as screenshots, recordings, or HTML reports to lower human review cost; and focus code review on P0/P1 issues with small PRs.

The thread sits in the broader “Vibe Coding” discussion: generation is now cheap enough that non-specialists build software and traditional engineering gates get skipped. 宝玉 explicitly invokes feasibility analysis, prototyping, and system design from conventional software engineering, and mentions tooling such as Claude Design \(or a local alternative\) for prototypes and Antigravity, where per-file confirmation across workspaces illustrates the human review bottleneck.

No community comments were available with the source. Adjacent discussion in the Horizon archive — not a direct response to this thread — includes Sphinx, an early-stage open-source tool that gates production pushes behind a comprehension questionnaire about AI-generated code \[tool-1-1\]; a Hacker News thread where engineers describe treating models like junior engineers and shifting saved coding time into testing \[tool-1-2\]; and a practitioner prompt for AI-driven product and UX walkthrough reviews \[tool-1-3\]. Archive dates are digest dates, not verified event dates.

<details><summary>References</summary>
<ul>
<li><a href="https://sphinx-six-theta.vercel.app/">2026-10-19 — Sphinx: open-source hook quizzes developers on AI-generated code before deployment</a></li>
<li><a href="https://news.ycombinator.com/item?id=50151036">2026-10-20 — Engineers Share How to Ship AI-Written Code Safely</a></li>
<li><a href="https://x.com/vista8/status/2119574943021371755">2026-11-09 — AI Walkthrough Prompt for Product &amp; UX Review</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#verification`, `#agent workflows`, `#software engineering`, `#Vibe Coding`, `#practitioner insights`

---

<a id="item-twitter-news-2"></a>
### [OpenAI&\#x27;s Perplexity Curves and the Shift to Post-Training](https://x.com/dongxi_nlp/status/2124602615543595393) ⭐️ 7.0/10

Dongxi NLP argues that OpenAI&\#x27;s published perplexity curves point to a change in LLM training strategy. The thread identifies GPT-4.5 at roughly 0.877 perplexity as the endpoint of the pretraining approach based on making ever-larger base models. After that, it says, o3&\#x27;s perplexity rises to about 0.90 rather than continuing downward.

The explanation offered is that post-training, especially reinforcement learning, requires many rollouts whose cost scales with base-model size. Using a smaller base and applying heavy RL can therefore be more cost-effective, shifting compute from pretraining toward post-training. RL does not directly improve perplexity: it narrows the model&\#x27;s output distribution toward high-reward patterns, which can raise capability while reducing fit to the overall text distribution. The thread adds that post-training can still indirectly strengthen future base models when strong RL-trained models generate synthetic data, reasoning traces, and clean code for next-generation pretraining or mid-training. On this view, post-training does not lower perplexity directly, but its data-generation loop can improve later bases—an effect the thread associates with a sharp perplexity drop in 2026. The specific perplexity values and the 2026 projection are presented without cited sourcing in the thread.

twitter · Dongxi 东锡 NLP · Nov 22, 20:35

**「Background」** The item is a technical X thread by Dongxi 东锡 NLP, not an OpenAI announcement. Its central claim is that OpenAI’s published perplexity curves show a shift in training emphasis: from making pretrained base models larger toward heavy post-training and RL on smaller bases. The author identifies GPT‑4.5 at roughly 0.877 as the endpoint of the “bigger base model” pretraining era, then reads o3’s rise back to roughly 0.90 as a post-training effect rather than a simple capability regression. The proposed mechanism is that RL rollouts become costlier as base models grow, so compute moves toward post-training; RL narrows the output distribution toward high-reward modes, which can improve capability while worsening fit to the overall text distribution. The thread then argues that post-training indirectly strengthens future bases by generating synthetic data, reasoning traces, and clean code for pretraining or mid-training, and attributes an expected 2026 perplexity drop to that loop. These specific figures, the curve interpretation, and the 2026 projection come from the thread and are presented without sourcing, so they should be treated as the author’s analysis rather than a verified OpenAI statement.

For external context, OpenAI’s own “Perplexity and Intelligence” page discusses log-perplexity as a lens on model progress and cites GPT‑3.5 at approximately 0.99 on its main evaluation dataset. That shows public precedent for using perplexity in OpenAI commentary, but it does not verify the thread’s GPT‑4.5/o3 values or its interpretation of the curve \[tool-2-1\]. No community comments were available in the supplied item, so there is no community reaction to summarize.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#LLM training`, `#perplexity`, `#post-training`, `#reinforcement learning`, `#scaling laws`, `#synthetic data`, `#OpenAI`

---