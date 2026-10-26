# Horizon Daily - 2026-10-26

> From 34 items, 8 important content pieces were selected

---

**Technology News**
1. [Brotli Critical Flaw CVE-2026-111497 Hits Python, Node.js HTTP Components](#item-tech-news-1) ⭐️ 8.0/10
2. [Cerebras Says It Deploys Trillion-Parameter Models on Wafer-Scale Systems](#item-tech-news-2) ⭐️ 7.0/10
3. [Apple to Unveil First Touchscreen MacBook Pro With OLED, Dynamic Island](#item-tech-news-3) ⭐️ 7.0/10
4. [Fine-Tuned 10-Year-Old CNN Beats Frontier LLMs on Skin Cancer Diagnosis](#item-tech-news-4) ⭐️ 6.0/10
5. [UC Berkeley Math Professor Says AI Makes Grading Homework Pointless](#item-tech-news-5) ⭐️ 6.0/10
6. [Nanbeige releases Apache 2.0 Nanbeige4.3-33B teacher for smaller agents](#item-tech-news-6) ⭐️ 6.0/10
7. [memt-1.0 memory-native architecture: gated deltanet-2, mixture-of-storage, 66x smaller storage](#item-tech-news-7) ⭐️ 6.0/10

**Financial News**
1. [GPU Rental Prices Rise Broadly, Including Older A100, per a16z Index](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Brotli Critical Flaw CVE-2026-111497 Hits Python, Node.js HTTP Components](https://www.aikido.dev/blog/python-packages-vulnerable-node2shell-brotli-cve-2026-111497) ⭐️ 8.0/10

A critical Brotli decoder vulnerability, CVE-2026-111497, affects versions 1.0.3 through 1.2.0 with a CVSS 4.0 score of 9.2, allowing remote unauthenticated attackers to trigger memory corruption, data leaks, crashes, or possible code execution via crafted compressed streams. The flaw, initially disclosed as Node2Shell and later dubbed HTTP2Shell, affects Python and Node.js HTTP components. Patches are available: Python brotli 1.2.1 and brotlicffi 1.2.1.0, and Node.js 22.23.4, 24.22.1, or 26.12.1. OpenAI reported discovering the issue in February 2026.

telegram · zaihuapd · Oct 25, 02:42

**「Background」** Brotli is a widely used compression format for HTTP responses, and servers and clients routinely decompress data from remote peers. The vulnerability was initially disclosed under the name Node2Shell before being referred to as HTTP2Shell.

**「Impact」** Python deployments should upgrade the brotli package to 1.2.1 and brotlicffi to 1.2.1.0, while Node.js servers should move to the patched 22.23.4, 24.22.1, or 26.12.1 releases; unpatched HTTP components that accept Brotli-encoded requests or responses remain remotely exploitable.

**Tags**: `#Brotli`, `#CVE-2026-111497`, `#security`, `#Python`, `#Node.js`

---

<a id="item-tech-news-2"></a>
### [Cerebras Says It Deploys Trillion-Parameter Models on Wafer-Scale Systems](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

In a vendor blog post, Cerebras describes how it deploys trillion-parameter frontier models on its wafer-scale systems, presenting the effort as a systems engineering achievement. Because the description comes from Cerebras itself and no independent benchmark or public release details are supplied, the deployment claim should be read as vendor-reported rather than independently verified. The post also leaves open how model freshness, cost, and hardware availability affect real customer access.

hackernews · gmays · Oct 25, 01:33 · [Discussion](https://news.ycombinator.com/item?id=50227356)

**「Background」** Cerebras&\#x27;s WSE-3T wafer has only 44 GB of on-chip memory, while trillion-parameter frontier models need terabytes for weights alone. The company&\#x27;s deployment article explains how it maps these models across WSE-3T wafers and claims scalable inference at 1,000–2,000+ tokens per second. This context matters because the core engineering challenge is fitting weights that vastly exceed the memory of a single wafer.

**「Impact」** Practically, developers currently cannot directly evaluate the trillion-parameter deployment claim: one community member reports that the reasonably accessible models on Cerebras are &quot;GPT OSS 120b&quot; and &quot;Qwen 3.8 27B,&quot; with high speed but poor accuracy for their tasks, while another argues the company&\#x27;s capital and manufacturing constraints will delay broader access. This suggests near-term users should treat Cerebras&\#x27;s advertised frontier deployment as separate from what they can actually run.

**「Community Discussion」** Commenters question actual accessibility and model freshness: ilaksh argues that Cerebras&\#x27;s limited resources \(under $3 billion versus OpenAI&\#x27;s over $100 billion\) and difficult wafer-scale manufacturing prevent it from meeting demand, while keyle reports that the accessible models are fast but not accurate enough for their use. pat64 adds that the technology is remarkable but the team is &quot;bafflingly inadequate,&quot; and piterrro expects Cerebras to eventually serve newer models at lower cost and higher speed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras">How we deploy Trillion-parameter frontier models on Cerebras</a></li>
<li><a href="https://x.com/cerebras/article/2113315017714246003">How we deploy Trillion-parameter frontier models on Cerebras</a></li>

</ul>
</details>

**Tags**: `#cerebras`, `#ai inference`, `#trillion-parameter models`, `#wafer-scale hardware`, `#ai infrastructure`

---

<a id="item-tech-news-3"></a>
### [Apple to Unveil First Touchscreen MacBook Pro With OLED, Dynamic Island](https://www.bloomberg.com/news/newsletters/2026-10-25/apple-to-unveil-touch-screen-macbook-pro-executive-promotions-in-box-checker) ⭐️ 7.0/10

Apple plans to unveil its first touchscreen MacBook Pro this Wednesday, making touch input and an OLED display available on the Mac for the first time, with Dynamic Island and 14- and 16-inch sizes. The new model will be priced above the current $2,499 starting point. This is an announced plan rather than a shipped device, and the shift reportedly reflects revenue and marketing considerations after years of ergonomic objections from executives.

telegram · zaihuapd · Oct 25, 14:25

**「Background」** Apple&\#x27;s Mac lineup has historically shipped without touchscreens, and executives repeatedly cited ergonomic arguments against the form factor, making the Mac the company&\#x27;s only device family without direct touch input. That long-held position is what turns this week&\#x27;s announcement into a reversal rather than an incremental update, with the report attributing the shift more to revenue and marketing than to a change in design philosophy.

**Tags**: `#Apple`, `#MacBook Pro`, `#Touchscreen`, `#OLED`, `#Hardware`

---

<a id="item-tech-news-4"></a>
### [Fine-Tuned 10-Year-Old CNN Beats Frontier LLMs on Skin Cancer Diagnosis](https://lynchlab.net/llm-skin-cancer) ⭐️ 6.0/10

A roughly 10-year-old Inception v3 CNN, fine-tuned on skin lesion images, outperformed frontier LLMs on skin cancer diagnosis, according to a benchmark from lynchlab.net. The author fine-tuned all layers on 68,011 dermoscopic and clinical images from the ISIC Archive using a single H100 GPU, then evaluated on 200 test lesions excluded from training and validation. The result is a focused model-selection comparison rather than a medical breakthrough, and it underscores that specialized supervised models can beat general-purpose LLMs on narrow vision tasks.

hackernews · sungam · Oct 25, 17:15 · [Discussion](https://news.ycombinator.com/item?id=50233779)

**「Background」** Inception v3 is a convolutional neural network architecture introduced around 2015 that can be adapted to a specific task by fine-tuning it on domain images. In this case, Dr Magnus Lynch of Lynch Lab tested such a model, tailored to dermoscopic and clinical images from the ISIC Archive, against general-purpose frontier LLMs for skin cancer diagnosis.

**「Impact」** Medical AI developers should treat general-purpose LLMs as a poor default for narrow image-classification tasks: a small fine-tuned CNN can be both cheaper and more accurate, and meaningful evaluation should use held-out test sets that exclude images of the same patient or lesion.

**「Community discussion」** Commenters largely found the result unsurprising, arguing that specialized models naturally beat general ones on narrow tasks, with comparisons to calculators outperforming LLMs at arithmetic and to KataGo beating LLMs at Go. One dissenting comment said the benchmark misses the potential of LLM-based diagnosis in richer workflows, such as incorporating journal notes, generating patient questions, or handling out-of-distribution images like tattoos.

<details><summary>References</summary>
<ul>
<li><a href="https://lynchlab.net/llm-skin-cancer">A 10-year-old CNN outperforms frontier LLMs for skin ... | Lynch Lab</a></li>
<li><a href="https://www.isic-archive.com/">ISIC | International Skin Imaging Collaboration</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#LLMs`, `#computer vision`, `#medical AI`, `#benchmarking`

---

<a id="item-tech-news-5"></a>
### [UC Berkeley Math Professor Says AI Makes Grading Homework Pointless](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 6.0/10

UC Berkeley math professor Richard Borcherds says AI-assisted student work now makes grading homework pointless, sparking debate about whether homework still supports learning. The report presents Borcherds&\#x27;s opinion, not a campus policy change or measured outcome; it offers no evidence that graded homework no longer helps students.

hackernews · romanhn · Oct 25, 16:28 · [Discussion](https://news.ycombinator.com/item?id=50233304)

**「Background」** Richard Borcherds is a UC Berkeley mathematics professor and Fields medalist who had been paying readers to grade his students&\#x27; homework for correctness. After observing that students using AI consistently received top scores, he concluded there was no point in continuing that grading practice.

**「Impact」** For college instructors, the statement highlights that unmonitored homework can no longer be assumed to measure individual student work, and institutions may need to pair it with proctored assessments to verify learning.

**「Community Discussion」** Commenters push back from different angles: one notes Borcherds already delegated grading to assistants, another argues homework still acts as a “forcing function” even when students copy, and a third questions whether graded homework is needed for college students at all.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html">AI use leads UC Berkeley math professor to see ‘no point’ in ...</a></li>
<li><a href="https://newsscore.com/story/197972">UC Berkeley Fields medalist math professor stops grading ...</a></li>

</ul>
</details>

**Tags**: `#AI in education`, `#mathematics`, `#academia`, `#LLMs`, `#Richard Borcherds`

---

<a id="item-tech-news-6"></a>
### [Nanbeige releases Apache 2.0 Nanbeige4.3-33B teacher for smaller agents](https://www.reddit.com/r/MachineLearning/comments/1xf6x35/nanbeige_releases_nanbeige4333b_an_apache_20/) ⭐️ 6.0/10

Nanbeige released Nanbeige4.3-33B, an Apache 2.0 teacher model intended to train smaller agents, including a planned 3B model. The model card lists a 512K context window and reports 80.9 on Terminal-Bench 2.1 versus 73.0 for Qwen3.8-27B, while SWE-Bench Pro shows 60.3 versus 61.7. These scores are the team&\#x27;s own evaluations, not independent replication.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 25, 16:32

**「Background」** Open-weight labs often release a larger &\#x27;teacher&\#x27; model under a permissive license so that its outputs or training recipes can guide smaller, cheaper &\#x27;student&\#x27; models through distillation or fine-tuning. Nanbeige4.3-33B is positioned as exactly that: the designated teacher for Nanbeige&\#x27;s planned smaller agents, starting with an upcoming 3B model, and the Apache 2.0 license means third parties can also build on the weights.

**「Impact」** Developers can freely re-use the Apache 2.0 weights for building smaller agents, but should treat the reported benchmark scores as vendor claims. Reproducing the agent results requires keeping preserve\_thinking=true for multi-turn tool use, as the model card recommends.

**Tags**: `#large language models`, `#open source models`, `#AI agents`, `#benchmarks`, `#model release`

---

<a id="item-tech-news-7"></a>
### [memt-1.0 memory-native architecture: gated deltanet-2, mixture-of-storage, 66x smaller storage](https://www.reddit.com/r/MachineLearning/comments/1xeu0ht/memt10_architecture_breakdown_gated_deltanet2/) ⭐️ 6.0/10

A Reddit breakdown describes memt-1.0 as a memory-native agent architecture that internalizes procedural memory using gated deltanet-2 with a stable token-level memory update and a mixture-of-storage \(MOS\) layer, instead of append-only prompt stacks or external RAG pipelines. The post claims memt-1.0-nano delivers about 1.86x end-to-end inference speedup and a 66x reduction in persistent storage at 128k context versus full-context KV caching, while a two-stage training pipeline over 34b tokens preserves general reasoning. These figures come from an informal post with no primary source or independent verification.

reddit · r/MachineLearning · /u/Mrs-Grumpy23 · Oct 25, 05:31

**「Background」** The arXiv paper describes MemT-1.0 as a memory foundation model architecture that internalizes memory as part of model computation, positioned as an upgrade over the earlier Metis architecture, which combined dynamic local memory with trainable hyper memory. MemT-1.0 replaces Metis&\#x27;s token-selection mechanism with a stable token-level update based on Gated DeltaNet-2 and introduces Mixture-of-Storage to scale native memory capacity. The official repository describes a two-stage training pipeline supported by 34B tokens of data.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.26825">[2610.26825] MemT-1.0: Towards Memory-Native Evolution</a></li>
<li><a href="https://arxiv.org/pdf/2610.26825">MemT-1.0: Towards Memory-Native Evolution - arXiv.org</a></li>
<li><a href="https://github.com/MemTensor/MemT-1.0/">GitHub - MemTensor/MemT-1.0: Official repository for MemT-1.0</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#LLM inference`, `#agentic AI`, `#model architecture`, `#storage efficiency`

---

## Financial News

<a id="item-finance-news-1"></a>
### [GPU Rental Prices Rise Broadly, Including Older A100, per a16z Index](https://x.com/a16z/status/2113741008550990191) ⭐️ 7.0/10

An a16z GPU rental price index, set to 100 on Jan 1, 2026, shows broad rental increases by Oct 19: cumulative changes were about +160% for H200, +120% for B200, +65% for RTX PRO 6000, and +35% for H100 SXM, while the older A100 SXM4 was slightly above its start-of-year level.

telegram · zaihuapd · Oct 25, 06:39

**「Background」** The a16z index converts cloud GPU rental prices into a seven-day moving average, with January 1, 2026 set to 100, so later readings show how much rental rates have risen since the start of the year.

**Tags**: `#GPU rental prices`, `#AI infrastructure`, `#compute demand`, `#H200/B200`, `#price index`

---

