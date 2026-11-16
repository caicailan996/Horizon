# Horizon Daily - 2026-11-16

> From 65 items, 25 important content pieces were selected

---

**Technology News**
1. [Understanding Positional Embeddings in Modern LLMs](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta FAIR and NYU find vision encoder pretraining optional but not parameters](#item-tech-news-2) ⭐️ 8.0/10
3. [MacBook Pro OLED PWM Dimming Flicker Issue](#item-tech-news-3) ⭐️ 7.0/10
4. [Microsoft 365 outage linked to chlorine gas injury of 15 hotel guests](#item-tech-news-4) ⭐️ 7.0/10
5. [All AI-generated code should be Open Source](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Meetings beta lets teams use Claude in Google Meet to draft and whiteboard](#item-tech-news-6) ⭐️ 7.0/10
7. [Training-free gradient-free guidance for discrete diffusion DNA/protein design](#item-tech-news-7) ⭐️ 7.0/10
8. [cudaMemcpy pageable transfers reach 51.5 GB/s on B300 with tuner](#item-tech-news-8) ⭐️ 7.0/10
9. [FAA ground stop tied to copper-to-fiber router issue](#item-tech-news-9) ⭐️ 7.0/10
10. [Washington Post Alleges Rubio and Anthropic Targeted Nvidia CEO](#item-tech-news-10) ⭐️ 7.0/10
11. [Meituan Releases LongCat-2.5, 1.6T Coding Agent Trained Without Nvidia GPUs](#item-tech-news-11) ⭐️ 7.0/10
12. [Emacs as a Web Browser: Personal Workflow and Limitations](#item-tech-news-12) ⭐️ 6.0/10
13. [Reasoning model early exit via linear probe folded into &lt;/think&gt; row](#item-tech-news-13) ⭐️ 6.0/10
14. [Tesla Cybercab Requires $299 Monthly Subscription to Operate](#item-tech-news-14) ⭐️ 6.0/10
15. [Huawei Cloud Launches Open-Source openPangu-2.1-Pro on MaaS](#item-tech-news-15) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly ROCm Build for AMD Instinct GPUs](#item-ai-projects-1) ⭐️ 6.0/10
2. [LMCache nightly-rbln release](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache/LMCache nightly release](#item-ai-projects-3) ⭐️ 5.0/10

**Financial News**
1. [Commerce Secretary Lutnick faces questions over former firm&\#x27;s Nvidia ties and reported 50% holding decline](#item-finance-news-1) ⭐️ 7.0/10
2. [Judge denies motion to dismiss DRAM price-fixing lawsuit against Micron, Samsung, SK Hynix](#item-finance-news-2) ⭐️ 7.0/10

**Twitter News**
1. [Paul Graham Clarifies Confusing Startup Advice List](#item-twitter-news-1) ⭐️ 7.0/10
2. [How Four Neurons Learn to Chase Light](#item-twitter-news-2) ⭐️ 7.0/10
3. [Report: Jensen Huang Considering Return as NVIDIA CEO](#item-twitter-news-3) ⭐️ 7.0/10
4. [Gemini 4 Carbon /swarm feature orchestrates 12 agents for Blender model creation](#item-twitter-news-4) ⭐️ 7.0/10
5. [Paul Graham on Ford Trimotor range and Jacksonville–Savannah stops](#item-twitter-news-5) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Understanding Positional Embeddings in Modern LLMs](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 8.0/10

A new technical article by vismit2000, published on Sebastian Raschka&\#x27;s Magazine on November 15, 2026, explains how modern transformer-based LLMs represent token positions. It covers common positional embedding methods and links them to underlying theory, though it is not a new model release or measured result.

hackernews · Ahead of AI · Nov 15, 12:14 · [Discussion](https://news.ycombinator.com/item?id=50506376)

**「Why positional information is needed」** Transformers&\#x27; self-attention mechanism sees tokens independently of order, so positional embeddings are required to represent sequence position. Earlier models such as GPT-2 added learned absolute position vectors to each token embedding, whereas modern LLMs commonly use rotary positional embeddings \(RoPE\); the article also surveys partial RoPE and NoPE layers across 2025–2026 open-weight architectures.

**「Community Discussion」** A reader \(programjames\) argues that the article focuses on implementation and that really understanding positional embeddings requires viewing them as group representations; rotary positional embeddings are given as representations of the abelian translation group ℝⁿ. This is an opinion, not a fact established in the article.

<details><summary>References</summary>
<ul>
<li><a href="https://daily.dev/posts/understanding-positional-embeddings-in-modern-llms-415mglzuo">Understanding Positional Embeddings in Modern LLMs</a></li>
<li><a href="https://sebastianraschka.com/blog/">Blog and Notes - Sebastian Raschka, PhD Positional embeddings in modern LLMs: from GPT-2 to RoPE and ... RoPE vs NoPE: Modern LLM Position Encoding (2026 ... No Positional Embeddings (NoPE) | Sebastian Raschka, PhD Sebastian Raschka Explains Positional Embeddings… · AGI Hunt</a></li>

</ul>
</details>

**Tags**: `#positional-embeddings`, `#LLMs`, `#transformers`, `#deep-learning`, `#NLP`

---

<a id="item-tech-news-2"></a>
### [Meta FAIR and NYU find vision encoder pretraining optional but not parameters](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR and NYU researchers report results from 200+ multimodal LLMs trained from scratch on matched compute to isolate three vision design choices. In their preprint, separate vision encoder pretraining at best tied training the encoder from scratch alongside the LLM, and did not help even when free; pretraining MetaCLIP 6.5x longer raised ImageNet linear-probe accuracy from 80.4% to 84.4% but not VQA. Vision-only parameters remained essential: encoder-free models trailed at every tested size from 0.6B to 6.4B and needed about 3x the compute to catch up, while giving the LLM the encoder parameters improved text but not VQA. Placing those vision-only weights as zero-initialized branches in the first 8 layers of the LLM matched a standard encoder from 1.7B to 6.4B, with about 13% lower time to first token.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Background」** The paper addresses a current disagreement: published models such as Gemma 4 12B dropped the vision encoder, Kimi K3 trained its encoder from scratch, and Inkling 2 Small brought an encoder back, but their differing data and compute prevent clean comparisons. A standard encoder bundles separate pretraining, parameters used only for vision tokens, and placement before the LLM; this work tests each choice independently.

**「Impact」** For developers of small multimodal models, the results suggest skipping separate encoder pretraining and embedding vision-only weights in early LLM layers can cut pretraining compute and latency while preserving VQA, provided those dedicated vision parameters are kept.

**Tags**: `#multimodal learning`, `#vision encoders`, `#model pretraining`, `#empirical study`, `#MLLMs`

---

<a id="item-tech-news-3"></a>
### [MacBook Pro OLED PWM Dimming Flicker Issue](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

A MacAnorak technical article examines the MacBook Pro&\#x27;s OLED panel and reports that its pulse-width modulation \(PWM\) brightness control may cause flicker and discomfort for sensitive users. The investigation frames the OLED switch as a trade-off where a better display becomes harder to use for people prone to PWM-induced eye strain, nausea, or headaches. In discussion, one commenter disputes the reported 240 Hz measurement, arguing that the tandem OLED&\#x27;s two 480 Hz out-of-phase PWM signals yield an effective 960 Hz.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**「Background」** Pulse-width modulation \(PWM\) controls brightness by rapidly cycling a display&\#x27;s pixels, and lower PWM frequencies are associated with visible flicker and eye strain for some users. Horizon&\#x27;s October 28 digest reported that Apple was expected to announce its first touchscreen MacBook Pro with an OLED XDR display, with sales reportedly possible as early as November 6; the current analysis examines that panel&\#x27;s PWM behavior.

**「Impact」** Flicker-sensitive buyers may need to test an OLED MacBook Pro before purchase or seek mitigation, since PWM-based dimming can trigger eye strain or headaches in affected users.

**「Community Discussion」** A commenter who checked the source of the 240 Hz claim disagrees with the testers, arguing the tandem OLED panels run at 480 Hz each and 180 degrees out of phase for an effective 960 Hz. Other readers describe personal flicker sensitivity that causes nausea and headaches and welcome the attention to the issue.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=uVtylIuB_zQ">Thank you, Xiaomi! No More OLED PWM Headaches... - YouTube</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-27/apple-14-inch-16-inch-macbook-pro-touch-price-is-likely-2-899-laptop-details">2026-10-28 — Apple Reported to Launch Touchscreen MacBook Pro From $2,899</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#display`, `#pwm`, `#macbook`, `#flicker`

---

<a id="item-tech-news-4"></a>
### [Microsoft 365 outage linked to chlorine gas injury of 15 hotel guests](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

A chlorine gas incident at a Phantasialand hotel injured 15 guests. According to the linked WDR report, a Microsoft 365 outage prevented email alerts from the sauna area&\#x27;s maintenance safety system from being received, so staff were unaware that the automatic dosing system had pumped too much chlorine into the pool.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**「Earlier Microsoft 365 outage」** Horizon&\#x27;s November 13 digest reported a Microsoft 365 email and collaboration outage affecting users worldwide, with recovery still in progress. The November 14 digest added that Outlook, Teams, and Copilot remained down after more than 12 hours, and Microsoft attributed the failure to a server issue. The current incident at Phantasialand&\#x27;s Hotel Ling Bao reportedly occurred because the pool-safety system&\#x27;s email alert was not received during that outage.

**「Community Discussion」** Commenters placed responsibility on the hotel rather than Microsoft, arguing that a chlorine dosing safety system should not rely solely on cloud email and should include backup alerts or human checks. One commenter with experience running a closed-loop chlorination system said such systems can fail by measuring low chlorine and overdispensing it, calling the design &\#x27;beyond screwed up.&\#x27;

<details><summary>References</summary>
<ul>
<li><a href="https://status.cloud.microsoft/">2026-11-13 — Microsoft 365 Email Outage Worldwide as Recovery Progresses</a></li>
<li><a href="https://www.reuters.com/technology/microsoft-365-outlook-down-thousands-us-users-downdetector-shows-2026-11-12/">2026-11-14 — Microsoft Outlook, Teams, Copilot Global Outage Exceeds 12 Hours</a></li>

</ul>
</details>

**Tags**: `#safety-critical-systems`, `#cloud-dependency`, `#incident-report`, `#system-design`, `#microsoft-365`

---

<a id="item-tech-news-5"></a>
### [All AI-generated code should be Open Source](https://jakub.jankiewicz.org/blog/ai-code-open-source/) ⭐️ 7.0/10

The article by jcubic argues that all AI-generated code should be open source, rather than being copyrightable proprietary work. It raises questions about whether code produced by models trained on public repositories can be owned by the user who prompted it. The piece is an opinion and policy argument, not a new technical capability or legal ruling.

hackernews · jcubic · Nov 15, 14:46 · [Discussion](https://news.ycombinator.com/item?id=50507303)

**「Background」** The debate hinges on US copyright law, where human authorship is required for protection. A commenter points to Copyright Office guidance stating that existing law can resolve AI copyrightability questions and that using AI to assist rather than replace human creativity does not affect copyright protection. This frames the article&\#x27;s position on forcing AI-generated code to be open source.

**「Community Discussion」** Commenters disagree on whether AI-generated code should be ownable. Some argue AI is a tool like a compiler and that substantial human direction justifies proprietary rights, while others counter that models trained on open-source code can reproduce it nearly verbatim, making open-source or attribution requirements more reasonable.

**Tags**: `#AI`, `#open source`, `#copyright`, `#software licensing`, `#policy`

---

<a id="item-tech-news-6"></a>
### [Claude Meetings beta lets teams use Claude in Google Meet to draft and whiteboard](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Claude%E8%83%BD%E8%BF%9B%E8%A7%86%E9%A2%91%E4%BC%9A%E8%AE%AE%E4%BA%86%EF%BC%81%E8%BE%B9%E5%90%AC%E8%BE%B9%E5%86%99%E6%96%B9%E6%A1%88%EF%BC%8C%E7%99%BD%E6%9D%BF%E5%BD%93%E5%9C%BA%E7%94%BB) ⭐️ 7.0/10

Anthropic announced on November 12 that Claude Meetings is entering beta. Teams can add Claude directly to Google Meet and, during a discussion, ask it to turn the conversation into a structured document or draw on a whiteboard. The feature is a beta capability, not a generally available release, and the announcement describes Anthropic&\#x27;s demo rather than independent testing.

rss · 新智元 · Nov 15, 08:35

**「Background」** Anthropic&\#x27;s Claude is an AI assistant. Horizon&\#x27;s November 13 digest reported that Claude Meetings entered beta on Google Meet, initially for Team and Enterprise plans; Horizon&\#x27;s November 11 digest reported that Claude Whiteboards was introduced for live board editing. This report adds hands-on details of using Claude to draft meeting proposals and edit a whiteboard in real time.

**「Impact」** For teams in the beta, a meeting can produce a draft proposal while the discussion is still happening, so attendees can resolve disagreements or unclear points against the draft in the same session instead of reconstructing action items afterward.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/dotey/status/2120979951599931793">2026-11-13 — Claude Meetings 测试版：Claude 加入 Google Meet 会议</a></li>
<li><a href="https://claude.com/resources/articles/sheets-whiteboards-data">2026-11-11 — Anthropic Introduces Claude Whiteboards, Sheets, and Data</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#video conferencing`, `#productivity`

---

<a id="item-tech-news-7"></a>
### [Training-free gradient-free guidance for discrete diffusion DNA/protein design](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+NeurIPS%2726%EF%BD%9C%E6%97%A0%E9%9C%80%E8%AE%AD%E7%BB%83%2B%E6%A2%AF%E5%BA%A6%EF%BC%9A%E5%BC%95%E5%AF%BC%E7%A6%BB%E6%95%A3%E6%89%A9%E6%95%A3%E6%A8%A1%E5%9E%8B%E8%AE%BE%E8%AE%A1DNA/%E8%9B%8B%E7%99%BD%E8%B4%A8) ⭐️ 7.0/10

Researchers at NeurIPS 2026 introduce D-DOIT, a training-free, gradient-free inference-time sampler that guides frozen masked discrete diffusion models toward arbitrary black-box rewards for DNA and protein design. The method uses a Doob h-transform formulation and requires only reward values, not gradients or fine-tuning. The article reports D-DOIT-Q achieves predicted activity 6.19 on HepG2 enhancer design, exceeding fine-tuned DRAKES \(5.61\), and D-DOIT reaches 68.1% structure–stability joint success on protein inverse folding, above SMC \(63.6%\) and TDS \(62.9%\). Paper, code, and project page are provided.

rss · 新智元 · Nov 15, 05:50

**「Background」** Masked discrete diffusion models generate DNA or protein sequences by progressively revealing masked tokens, but adapting a pretrained model to task rewards typically requires fine-tuning or differentiable reward models. Existing training-free alternatives often rely on gradients or particle/search procedures whose cost grows with trajectory length or search width. The article frames reward adaptation as a distribution transport problem and derives an h-transform for masked discrete diffusion.

**「Impact」** Because D-DOIT needs only query access to reward values and no parameter updates, it can be applied to frozen pretrained discrete diffusion models for black-box scoring functions such as Enformer or structural predictors. The released code and project page support reproduction and application to enhancer and protein design tasks.

**Tags**: `#discrete diffusion models`, `#protein design`, `#DNA synthesis`, `#generative models`, `#bioinformatics`

---

<a id="item-tech-news-8"></a>
### [cudaMemcpy pageable transfers reach 51.5 GB/s on B300 with tuner](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

An open-source tool by /u/makneeee tunes pageable cudaMemcpy transfers. In the author&\#x27;s benchmark, copying a 1 GB torch.uint8 tensor from CPU to GPU on an NVIDIA B300 improved from 10.2 GB/s to 51.5 GB/s when running the script with \`cmt tune -- python bench.py\`. The code is available on GitHub, but the result has not been independently validated.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**「CUDA pageable transfers」** cudaMemcpy is the CUDA API used to copy data between host and device memory. When host memory is pageable rather than pinned, transfers normally run slower because the driver may stage them through an intermediate pinned buffer; the tool described here tunes the transfer settings to improve this path.

**「Impact」** Practitioners experiencing slow host-to-device transfers on B300 GPUs can try the tuner by running \`cmt tune -- python &lt;script&gt;\`. The reported 5x improvement is based on the author&\#x27;s single benchmark and may vary with workload and system configuration.

**Tags**: `#cuda`, `#gpu`, `#performance`, `#machine-learning`, `#data-transfer`

---

<a id="item-tech-news-9"></a>
### [FAA ground stop tied to copper-to-fiber router issue](https://www.theverge.com/transportation/1033898/faa-ground-stop-sean-duffy-faa-copper-wire) ⭐️ 7.0/10

US Transportation Secretary Sean Duffy said on November 14 that the FAA&\#x27;s nationwide ground stop stemmed from a routine copper-to-fiber upgrade at a remote facility. The newly installed fiber router flooded other routers with more than 1,000 connection requests every 4 to 5 seconds, disrupting radar and aircraft communications and grounding thousands of flights. The root cause remains unclear and may be hardware failure, a configuration error, or a mistake by contractor L3Harris. Duffy called for additional congressional funding to modernize air traffic control.

telegram · zaihuapd · Nov 15, 02:10

**「Earlier report of the outage」** Horizon&\#x27;s November 14 digest reported the FAA&\#x27;s initial nationwide ground stop after a critical air-traffic control communications outage, noting the affected network was operated by L3Harris and that early reports pointed to a software update causing a system reboot and crash. The current account narrows the cause to a newly installed fiber router flooding other routers with connection requests after a copper-to-fiber upgrade, while the transport secretary says the root cause is not yet determined.

**「Impact」** Travelers and airlines faced thousands of grounded flights while radar and communications were disrupted; federal officials are requesting additional congressional funding to modernize the FAA&\#x27;s aging copper infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247">2026-11-14 — FAA issues nationwide ground stop after communications outage</a></li>

</ul>
</details>

**Tags**: `#networking`, `#infrastructure`, `#aviation`, `#outage`, `#routing`

---

<a id="item-tech-news-10"></a>
### [Washington Post Alleges Rubio and Anthropic Targeted Nvidia CEO](https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/) ⭐️ 7.0/10

A Washington Post investigative report alleges that Senator Marco Rubio and Anthropic were involved in a coordinated effort to target Nvidia CEO Jensen Huang after his personal lobbying with Trump led to relaxed AI chip export controls to China. The report says Rubio used CIA intelligence to write a hardline memo pressing the president, while Silicon Valley observers suspect Anthropic executives leaked an initial tip to New York Times reporters about a Singapore company linked to a woman connected to Huang; the reporters and Anthropic have not responded. The alleged conflict centers on Anthropic&\#x27;s lobbying for strict export limits and firmware-level tracking or locking of GPUs, which Huang opposed, and House China committee leaders are now using the fallout to push three new clauses into a year-end defense bill: further high-end AI chip export restrictions, mandatory anti-smuggling tracking in chips, and limits on China&\#x27;s access to chipmaking equipment.

telegram · zaihuapd · Nov 15, 08:08

**「Earlier resignation and export-control pressure」** Horizon&\#x27;s November 14 digest reported that Nvidia CEO Jensen Huang resigned after admitting an affair with an alleged Chinese spy and that analysts cited by CNBC saw the scandal raising the chance Congress would tighten advanced chip sales to China before year-end. The Washington Post report now shifts attention to the political figures and companies alleged to have driven that pressure, with specific defense-bill provisions being promoted.

**「Legislative consequence」** The Senate version of the annual defense bill now carries bipartisan chip bills including the AI Overwatch Act, which would give Congress power over chip export licenses, and the Chip Security Act, aimed at smuggling. If enacted, Nvidia would lose the executive-branch flexibility Huang used to ease China export limits, and would face congressional oversight of individual licenses plus anti-smuggling tracking requirements in chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/13/jensen-huang-nvidia-us-china-relations.html">2026-11-14 — Nvidia CEO&#x27;s resignation amid spy allegations raises risk of tighter U.S.-China tech controls</a></li>
<li><a href="https://www.zerohedge.com/ai/who-whacked-jensen-huang-cia-wasnt-convinced-so-rubio-reworked-their-memo">Who Whacked Jensen Huang ? The CIA... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#export controls`, `#Nvidia`, `#Anthropic`, `#semiconductors`

---

<a id="item-tech-news-11"></a>
### [Meituan Releases LongCat-2.5, 1.6T Coding Agent Trained Without Nvidia GPUs](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 7.0/10

Meituan&\#x27;s LongCat team published open weights for LongCat-2.5, a 1.6T-parameter coding agent model with about 48B active parameters per token, under an MIT license. The team states the model was trained entirely on Huawei Ascend accelerators without Nvidia GPUs and supports text, image, and video inputs. It reports a score of 88.4 on Terminal Bench v2.1, slightly below Claude Opus 5&\#x27;s 89.1.

telegram · zaihuapd · Nov 15, 11:08

**「Background」** Horizon&\#x27;s November 2 digest reported that LongCat-2.5 was initially made available for trial and via API; the current announcement is the MIT-licensed weight release roughly one week later. Earlier coverage of LongCat-2.0 established that Meituan already trained its predecessor on a domestic Chinese chip cluster without Nvidia GPUs, so the Huawei Ascend-only training claim is a continuation rather than a first for the company.

**「Impact」** Developers can use or modify the model commercially under the MIT license, but the only reported benchmark comes from the vendor and covers a single test, so independent verification of the claimed coding-agent performance is still lacking.

<details><summary>References</summary>
<ul>
<li><a href="https://longcat.ai/blog/longcat-2.5/">2026-11-02 — LongCat-2.5: 1.6T-Parameter Native Multimodal Model Released</a></li>
<li><a href="https://braindetox.kr/en/posts/longcat_2_open_model_2026.html">LongCat - 2 .0: A 1.6-Trillion-Parameter Open Model Trained Without ...</a></li>

</ul>
</details>

**Tags**: `#open-source AI`, `#large language models`, `#AI agents`, `#non-Nvidia hardware`, `#coding models`

---

<a id="item-tech-news-12"></a>
### [Emacs as a Web Browser: Personal Workflow and Limitations](https://joshblais.com/blog/emacs-as-my-browser/) ⭐️ 6.0/10

Josh Blais published a blog post describing his personal workflow for using Emacs as a web browser, replacing a conventional GUI browser. He presents it as a lightweight, text-oriented approach, but community comments emphasize that it works well mainly for static HTML and blogs while failing on many commercial sites like Reddit.

hackernews · nyc111 · Nov 15, 15:21 · [Discussion](https://news.ycombinator.com/item?id=50507553)

**「Emacs text-mode browsing context」** Emacs has long included eww, a built-in text-mode web browser, and users can also browse inside Emacs with w3m-mode or embedded WebKit widgets. The blog post builds on these tools to use Emacs as a primary browser, but the supplied discussion notes that many modern commercial sites do not render well in text-only modes.

**「Impact」** Users considering an Emacs-based browsing setup should expect compatibility to be limited to static HTML and simple blogs; modern commercial web pages that depend on JavaScript are likely not usable, as multiple commenters report. They may need to retain a standard browser for such sites.

**「Community Discussion」** Commenters note that Emacs browsing works for static HTML and blogs but breaks on commercial sites, with one user sharing a follow-mode columnar hack for eww and another relying on w3m-mode for session management. A dissenting comment argues that such setups are &\#x27;cute&\#x27; but not a substitute for a content-addressable replacement for HTTP\(S\).

<details><summary>References</summary>
<ul>
<li><a href="https://joshblais.com/blog/emacs-as-my-browser/">Emacs is my browser - The Universe of Joshua Blais</a></li>

</ul>
</details>

**Tags**: `#emacs`, `#web-browsing`, `#productivity`, `#open-source`, `#text-mode`

---

<a id="item-tech-news-13"></a>
### [Reasoning model early exit via linear probe folded into &lt;/think&gt; row](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 6.0/10

A Reddit post reports a training-free method that stops reasoning models from overthinking by editing a single output-layer row: it folds a linear-discriminant-analysis probe into the &lt;/think&gt; token’s row. The author ran Qwen3.5-4B on 24 math problems, recorded hidden states, and added the probe direction at strength 14 to the &lt;/think&gt; row. On held-out examples the edited model is claimed to stop by about token 2,000 instead of 7,415, with 98% probability, and to use 54% fewer tokens on 8 unseen MATH-500 problems at the same accuracy. The post also reports DeepSeek V4.1 Flash solving 7/7 vs 6/7 math problems with 40% fewer tokens, but these are small-sample, single-run results and the probe was fitted on math only.

reddit · r/MachineLearning · /u/Good-Presentation-23 · Nov 15, 17:52

**「Background」** Reasoning models such as DeepSeek and Qwen generate a hidden scratchpad and finish when they emit the special &lt;/think&gt; token; the output layer computes each vocabulary token’s score as a row vector multiplied by the hidden state, so the score for “stop thinking now” is determined by exactly one row. The author treated that row as a place to inject a simple linear classifier computed with linear algebra rather than gradient training.

**「Impact」** Developers can download the edited Qwen3.5-4B GGUF from Hugging Face and run it in stock llama.cpp to cut reasoning tokens, but the probe was fitted on math problems, small samples, and the AIME comparison used a 32k-token limit below Qwen’s recommended 81,920, so generalization remains uncertain.

**Tags**: `#reasoning-models`, `#early-exit`, `#llm-inference`, `#weight-editing`, `#machine-learning`

---

<a id="item-tech-news-14"></a>
### [Tesla Cybercab Requires $299 Monthly Subscription to Operate](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 6.0/10

Tesla has published Cybercab subscription terms requiring a $299 monthly fee on top of the $29,990 vehicle price; without the subscription, the car will not operate, and Tesla may adjust the fee with one month&\#x27;s notice. Nonpayment or violation can lead to suspension or cancellation, and three accumulated warnings disable autonomous driving for one week. The vehicle operates only in designated areas and cannot be used on ride-hailing, delivery, or rental platforms without authorization. Electrek reports that Cybercab uses the same AI4 hardware and autonomous driving software as the robotaxi Model Y, but the consumer-facing FSD still requires human supervision.

telegram · zaihuapd · Nov 15, 01:10

**「Earlier Cybercab sales plan」** Horizon&\#x27;s October 23 digest reported Tesla said it would begin selling Cybercabs to customers by the end of the year, after initial production went to its own robotaxi fleet, and that unsupervised FSD was delayed to Q2 next year. The newly published subscription terms now specify the recurring cost and usage limits for those customer vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/10/21/tesla-says-it-will-start-selling-cybercabs-by-end-of-year/">2026-10-23 — Tesla says Cybercab sales start by end of year; FSD slips to Q2</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#autonomous vehicles`, `#subscription pricing`, `#AI4 hardware`, `#robotaxi`

---

<a id="item-tech-news-15"></a>
### [Huawei Cloud Launches Open-Source openPangu-2.1-Pro on MaaS](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 6.0/10

On November 15, 2026, Huawei Cloud made the open-source openPangu-2.1-Pro model available on its MaaS \(Model-as-a-Service\) platform, targeting agent development, AI coding, and inference optimization. The model was optimized with more than 100,000 specialized data items for Skills triggering and tool calls, with particular adaptation for HarmonyOS ArkTS development and Ascend operator generation. It is also integrated with AgentArts, CodeArts, and OfficeAce. Huawei Cloud lists pricing at 0.8 yuan per million input tokens, 3.2 yuan per million output tokens, and 0.016 yuan per million cached input tokens.

telegram · zaihuapd · Nov 15, 16:03

**「Background」** Huawei Cloud’s Model-as-a-Service \(MaaS\) platform hosts AI models, and openPangu is the open-source release of Huawei’s Pangu large language model.

**「Impact」** Developers using Huawei Cloud MaaS can use openPangu-2.1-Pro at the listed token-based prices, and the integrations with CodeArts and AgentArts target ArkTS and Ascend development workflows.

**Tags**: `#AI`, `#large language model`, `#Huawei Cloud`, `#open source`, `#MaaS`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly ROCm Build for AMD Instinct GPUs](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 6.0/10

Nightly ROCm 7.2 wheels for LMCache, built from dev for AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), ABI-matched to upstream vLLM ROCm images.

github · github-actions\[bot\] · Nov 15, 07:46

**「解决的痛点」** Enables LMCache deployment on AMD Instinct GPUs by providing prebuilt ROCm wheels that match the vLLM ROCm container&\#x27;s ABI \(torch 2.13, cp312\). Users can install without dependency resolution \(--no-deps\), avoiding complex builds and compatibility issues.

**「Background &amp; Impact」** LMCache is a modular KV cache management layer for LLM inference that stores and reuses KV cache across requests to reduce time-to-first-token and improve throughput, particularly for long-context and repeated-prompt workloads \(tool-1-1, tool-1-2, tool-1-3\). This nightly release builds LMCache from the dev branch as ROCm 7.2 wheels for AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\) GPUs, ABI-matched to the upstream vllm/vllm-openai-rocm image \(torch 2.13, cp312\). It enables AMD GPU users to install LMCache into a vLLM ROCm container with a simple pip command, bringing the project&\#x27;s KV cache acceleration to AMD hardware environments. Because this is an automated nightly build rather than a feature release, its significance lies in providing current, compatible ROCm wheels for continuous AMD platform testing and deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#ROCm`, `#AMD`, `#LLM`, `#inference`, `#nightly-build`

---

<a id="item-ai-projects-2"></a>
### [LMCache nightly-rbln release](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

A nightly LMCache wheel built from the dev branch for Rebellions RBLN NPU environments, version 0.5.8.dev161+rbln, compatible with torch-rbln 0.12.0 and torch 2.13.0+cpu.

github · github-actions\[bot\] · Nov 15, 07:35

**「Problem Solved」** Simplifies deployment of LMCache on RBLN NPU hardware by providing a prebuilt wheel that matches the expected torch-rbln and rebel-compiler environment, while keeping host-owned dependencies external to avoid bundling or version conflicts.

**「Background」** This is a routine nightly pre-release from the LMCache dev branch, not a feature release. It extends LMCache&\#x27;s KV-cache management for LLM inference to Rebellions RBLN NPUs, aligning with the broader trend of supporting diverse AI accelerators beyond CUDA.

**Tags**: `#LMCache`, `#nightly-release`, `#RBLN-NPU`, `#KV-cache`

---

<a id="item-ai-projects-3"></a>
### [LMCache/LMCache nightly release](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

Automated nightly build of LMCache providing prebuilt Python wheels with CUDA 13.0 support for Linux amd64 and arm64.

github · github-actions\[bot\] · Nov 15, 09:32

**「Solved Pain Point」** Users needing LMCache on CUDA 13.0 otherwise must build from source or wait for stable wheels; the nightly release removes that build burden and enables testing against the latest CUDA toolchain.

**「Background &amp; Impact」** LMCache is an LLM KV-cache optimization project. This nightly exposes current dev-branch changes, letting early adopters validate upcoming features and maintain compatibility with CUDA 13.0 before stable releases.

**Tags**: `#llm`, `#kv-cache`, `#cuda`, `#nightly`, `#inference`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Commerce Secretary Lutnick faces questions over former firm&\#x27;s Nvidia ties and reported 50% holding decline](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

Commerce Secretary Howard Lutnick faces questions about his former firm Cantor Fitzgerald&\#x27;s ties to Nvidia, after Axios reported he resisted cracking down on a Singapore-based company suspected of smuggling Nvidia chips to China; according to a CNBC analysis of securities filings, Cantor&\#x27;s reported Nvidia share count fell nearly 50%, from 3.5 million in September 2025 to 1.78 million by March 2026.

rss · CNBC Finance · Nov 15, 19:58

**「Background」** The questions follow Axios reports that Lutnick resisted adding Singapore-based Megaspeed to the US restricted-entities list over suspected Nvidia chip smuggling to China. Cantor, now led by Lutnick&\#x27;s sons Brandon and Kyle, says the reported Nvidia holdings came from client swap transactions, and there is no evidence the sons had advance knowledge of intelligence concerns or that the share changes were tied to warnings.

**Tags**: `#Nvidia`, `#Howard Lutnick`, `#Cantor Fitzgerald`, `#export controls`, `#conflict of interest`

---

<a id="item-finance-news-2"></a>
### [Judge denies motion to dismiss DRAM price-fixing lawsuit against Micron, Samsung, SK Hynix](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

U.S. District Judge Noël Wise denied motions by Micron, Samsung, and SK Hynix to dismiss a DRAM price-fixing class action, ruling that the plaintiffs&\#x27; new evidence makes collusion plausible. The plaintiffs—17 individuals and small businesses—allege four parallel supply restrictions in one year drove DRAM prices up by as much as 500%.

telegram · zaihuapd · Nov 15, 16:39

**「Background」** The proposed class action, which alleges a DRAM \(computer and server main memory\) supply conspiracy since 2022, is before U.S. District Judge Noël Wise in the Northern District of California; on November 14 she denied the three companies&\#x27; joint motion to dismiss, finding the complaint plausibly alleged a Sherman Act Section 1 agreement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/354863/samsung-sk-hynix-and-micron-fail-to-get-dram-antitrust-suit-dismissed">Samsung, SK hynix, and Micron Fail to Get DRAM Antitrust Suit ...</a></li>
<li><a href="https://hoodline.com/2026/11/judge-lets-dram-price-fixing-suit-against-samsung-micron-sk-hynix-move-forward/">Judge Allows DRAM Price-Fixing Suit Vs Samsung, Micron, SK Hynix</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#price fixing`, `#antitrust`, `#semiconductors`, `#litigation`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Paul Graham Clarifies Confusing Startup Advice List](https://x.com/paulg/status/2122108050584592765) ⭐️ 7.0/10

Paul Graham responded to a list of startup advice from @romanbuildsaas and @ycombinator, saying he is also confused by some points. He explained that the two items about avoiding big deals and steering clear of large companies are really one point: startups should usually sell to other startups first because they decide quickly despite having less money. He corrected the &\#x27;murder&\#x27; reference to &\#x27;suicide&\#x27;, saying more startups kill themselves through poor execution than are killed by competitors, but added that founders shouldn&\#x27;t ignore competitors completely—just pay more attention to users than competitors. He also said he does not understand what &\#x27;Most companies don&\#x27;t die because of no money&\#x27; is supposed to mean.

twitter · Paul Graham · Nov 15, 23:22

**「Background」** Paul Graham posted this reply to @romanbuildsaas and @ycombinator. The context is a thread by @romanbuildsaas revisiting Graham&\#x27;s 2009 essay &\#x27;Startups in 13 Sentences&\#x27; \(tool-1-3\), which Roman said he reread after being accepted into YC \(tool-1-2\). In the tweet, Graham addresses confusion over a list of startup advice: he explains that the two points about avoiding big deals and steering clear of large companies are a single point — sell to startups first because they decide fast; he corrects &\#x27;murder&\#x27; to &\#x27;suicide&\#x27;, saying more startups kill themselves by poor execution than are killed by competitors, while still paying more attention to users than competitors; and he says he doesn&\#x27;t understand what &\#x27;Most companies don&\#x27;t die because of no money&\#x27; means.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/romanbuildsaas/status/2069492465338548714">Paul Graham published “Startups in 13 sentences” back in 2009 ...</a></li>
<li><a href="https://paulgraham.com/13sentences.html">Startups in 13 Sentences - Paul Graham</a></li>

</ul>
</details>

**Tags**: `#startup advice`, `#Paul Graham`, `#Y Combinator`, `#entrepreneurship`

---

<a id="item-twitter-news-2"></a>
### [How Four Neurons Learn to Chase Light](https://x.com/dotey/status/2122106906814935475) ⭐️ 7.0/10

This X thread summarizes the article &quot;Watch a Brain Learn&quot; by science journalist Aatish Bhatia and neuroscientist Arkarup Banerjee. It describes a simulated creature with only four neurons that learns behaviors like chasing light. The thread explains how three numbers determine whether it fears light, collides with it, or becomes attracted to it; framing these numbers as a cube turns learning into a path through that cube. Without direct teaching, the creature uses reward and punishment to find fewer than 2% usable solutions among more than 2,000 possible connection patterns. Changing the reward leads it to learn fleeing, playing dead, and fighting, then connects these findings to songbirds, AI, and human brains.

twitter · 宝玉 · Nov 15, 23:18

**「Background」** The tweet summarizes an interactive article from the Myriad series, “Watch a Brain Learn,” by Aatish Bhatia and Arkarup Banerjee. The article uses a simulated creature with only four neurons to show how reward and punishment can shape behaviors such as chasing light, fleeing, playing dead, or fighting. The virtual creature draws on Valentino Braitenberg’s 1984 synthetic psychology experiments, and the project frames learning as a path through a cube of possible wiring parameters, where only a small fraction of connections produce useful behavior \[tool-1-2\]. The article is presented as a visual explanation of reinforcement learning, and was shared and discussed on Hacker News \[tool-1-3\]. The original article is available at aatishb.com \[tool-1-1\].

<details><summary>References</summary>
<ul>
<li><a href="https://aatishb.com/myriad/how-brains-learn/">Watch a Brain Learn - aatishb.com</a></li>
<li><a href="https://news.lavx.hu/article/four-neurons-four-behaviors-how-a-virtual-spark-reveals-the-roots-of-intelligence">Four Neurons, Four Behaviors: How a Virtual Spark Reveals the ...</a></li>
<li><a href="https://zeli.app/story/50496885">Watch a four-neuron brain teach itself · Hacker News | Zeli</a></li>

</ul>
</details>

**Tags**: `#neuroscience`, `#machine-learning`, `#educational`, `#simulation`, `#AI`

---

<a id="item-twitter-news-3"></a>
### [Report: Jensen Huang Considering Return as NVIDIA CEO](https://x.com/dotey/status/2122062085807030716) ⭐️ 7.0/10

The Financial Times reported on November 15, 2026, that Jensen Huang is considering returning as NVIDIA CEO, having discussed a possible return with close associates. This comes three days after NVIDIA announced on November 12 that Huang had resigned as CEO and director, with CFO Colette Kress serving as interim CEO. According to the FT, Huang was already in talks about returning before the board&\#x27;s independent investigation concluded. Allies are reportedly forming a Silicon Valley executive &quot;war room&quot; to lobby the board and seek White House support. A public letter titled &quot;Stand with Jensen&quot; has reportedly gathered over 100,000 signatures, including Elon Musk, Tim Sweeney, Garry Tan, and Amjad Masad, with more than 5,000 signers identifying as current NVIDIA employees. The letter says signers have not seen evidence to substantiate espionage allegations and calls for due process. Investors Brad Gerstner and Gavin Baker publicly urged the board to handle succession carefully and keep Huang&\#x27;s return as an option, without demanding immediate reinstatement.

twitter · 宝玉 · Nov 15, 20:20

**「Background」** On 12 November 2026, Jensen Huang resigned as NVIDIA CEO and director; CFO Colette Kress was named interim CEO. The resignation followed reports of an alleged affair with a person described as a Chinese spy and possible export-control violations, though those claims were not confirmed in available sources \[tool-1-1\]\[tool-1-3\]. Now the Financial Times reports that Huang is weighing a return as CEO and has discussed the possibility with close associates, according to multiple people familiar with the matter. Allies are reportedly assembling a group of Silicon Valley executives in a &\#x27;war room&\#x27; to lobby the board for his reinstatement and seek White House support. A public letter, &\#x27;Stand with Jensen,&\#x27; calls for due process and has gathered over 100,000 signatures, including from Elon Musk, Tim Sweeney, Garry Tan, and Amjad Masad; Musk confirmed signing. Investors Brad Gerstner and Gavin Baker have written to the board urging a deliberate succession process and keeping Huang&\#x27;s return as an option, without demanding immediate reinstatement.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f">2026-11-13 — Jensen Huang Resigns as NVIDIA CEO</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/jensen-huang-nvidia-us-china-relations.html">2026-11-14 — Nvidia CEO&#x27;s resignation amid spy allegations raises risk of tighter U.S.-China tech controls</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#Jensen Huang`, `#AI industry`, `#leadership`, `#news`

---

<a id="item-twitter-news-4"></a>
### [Gemini 4 Carbon /swarm feature orchestrates 12 agents for Blender model creation](https://x.com/venturetwins/status/2122043781507948954) ⭐️ 7.0/10

Justine Moore \(@venturetwins\) shared a tweet highlighting the /swarm feature in Gemini 4 Carbon as underhyped. Moore asked for a 3D model of the Ferry Building, and the feature orchestrated 12 parallel agents to research, plan, write the Blender Python scripts, and critique each other&\#x27;s work on a shared message board.

twitter · Justine Moore · Nov 15, 19:07

**「Background」** On November 15, 2026, Justine Moore \(@venturetwins\) posted that Gemini 4 Carbon&\#x27;s /swarm feature is underhyped. She described asking for a 3D model of the Ferry Building; the system orchestrated 12 parallel agents to research, plan, write Blender Python scripts, and critique each other&\#x27;s work on a shared message board.

Gemini 4 Carbon was announced by Google on November 11, 2026, as a model focused on long-horizon agentic workflows, and the /swarm feature is associated with Google&\#x27;s Antigravity environment. A video overview from the launch period characterizes the broader release as a multi-day AI blitz that included Gemini 4 Carbon, Gemini 4 Hydrogen, Gemini Decision-1, AlphaProof Code, and Antigravity/swarm; the video claims Carbon autonomously edited a 30-minute video. Third-party model listings describe Gemini 4 Carbon as a frontier model for coding, agentic, and complex reasoning work, with support for long decode and text, image, audio, video, and file inputs.

No community comments were available for the tweet at the time of collection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=Sc6TriRAGnI">Gemini 4 Swarm is out of control... - YouTube</a></li>
<li><a href="https://agihunt.info/en/e/1a1c635d7ef6f674fcbda38ded0">Google launches Gemini 4 Carbon , its strongest… · AGI Hunt</a></li>
<li><a href="https://openrouter.ai/google/gemini-4-carbon">Gemini 4 Carbon - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#Gemini`, `#multi-agent`, `#AI`, `#3D modeling`, `#Blender`

---

<a id="item-twitter-news-5"></a>
### [Paul Graham on Ford Trimotor range and Jacksonville–Savannah stops](https://x.com/paulg/status/2122080094264995922) ⭐️ 6.0/10

Paul Graham, replying to @Itsjoeco, states that the 125-mile Jacksonville–Savannah route was about half the effective range of the Ford Trimotors in use, so only about half of those stops could have been eliminated. The analysis summary frames this as a niche historical aviation fact-check about Trimotor range and stop frequency.

twitter · Paul Graham · Nov 15, 21:31

**「Background」** Paul Graham&\#x27;s post discusses the effective range of the Ford Trimotor, an American three-engined transport aircraft that first flew in 1926 \[tool-1-1\]. The tweet states that the 125-mile Jacksonville–Savannah segment was &\#x27;about half the effective range&\#x27; of the Trimotors in use, so the number of intermediate stops could have been reduced by at most about half. Specifications for the 4-AT-E model list weights and dimensions but do not include range in the available snippet \[tool-1-2\]. The operational history and specifications of the Ford Trimotor as a passenger airliner are covered in additional references \[tool-1-3\]. No community comments are available.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ford_Trimotor">Ford Trimotor - Wikipedia</a></li>
<li><a href="https://www.airminded.net/ford3m/ford3m.html">Ford Tri-Motor - Holcomb&#x27;s Aerodrome</a></li>
<li><a href="https://www.militaryfactory.com/aircraft/detail.php?aircraft_id=1374">Ford Trimotor Transport Aircraft / Passenger Airliner</a></li>

</ul>
</details>

**Tags**: `#aviation`, `#history`, `#Ford Trimotor`, `#fact-check`

---

