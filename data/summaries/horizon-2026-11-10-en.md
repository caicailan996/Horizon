# Horizon Daily - 2026-11-10

> From 83 items, 34 important content pieces were selected

---

**Technology News**
1. [E-means claims 10x faster k-means at equal loss](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta Releases Muse Ember, Its Smallest and Most Efficient Model](#item-tech-news-2) ⭐️ 8.0/10
3. [Anthropic announces Claude Fable 5.2 and Mythos 5.2; 1,000 agents formalize FLT in 30 hours](#item-tech-news-3) ⭐️ 8.0/10
4. [LingBot-Touch: Latent Prediction Outperforms Reconstruction for Tactile Pretraining](#item-tech-news-4) ⭐️ 8.0/10
5. [Google consumer Gemini may route Drive and Gmail data to human annotators](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Fable 5.2 Scores 65 on Artificial Analysis, Highest So Far](#item-tech-news-6) ⭐️ 7.0/10
7. [Canada launches Real-Time Rail 24/7 payment system](#item-tech-news-7) ⭐️ 7.0/10
8. [Show HN: watched.earth Finds Every Satellite Pass and Photo Over Any Place](#item-tech-news-8) ⭐️ 7.0/10
9. [Benchmark Topic Pages Now Cover 2026 ICML, CVPR, ICLR, AAAI Papers](#item-tech-news-9) ⭐️ 7.0/10
10. [SwarmEvolve Uses Latent-Agent Swarms for Faster Math Discovery](#item-tech-news-10) ⭐️ 7.0/10
11. [Twindex: exact replayable proofs of parameter indistinguishability for ODE/PDE/PINN models](#item-tech-news-11) ⭐️ 7.0/10
12. [AI-designed avian flu vaccine candidate shows broad protection in mice and ferrets](#item-tech-news-12) ⭐️ 7.0/10
13. [Google Unveils TPU 8tx and 8i Max, Stepping Up Nvidia Rivalry](#item-tech-news-13) ⭐️ 7.0/10
14. [USPS Releases Official ZIP Code Boundary Polygons](#item-tech-news-14) ⭐️ 6.0/10
15. [Opus 5.5 November 3 Change Debated; Benchmark Rerun Stable](#item-tech-news-15) ⭐️ 6.0/10
16. [Simon Willison&\#x27;s Beep Locator triangulates mystery beep using Claude Code](#item-tech-news-16) ⭐️ 6.0/10
17. [Hide verbose AI-generated PR descriptions with details/summary in GitHub Markdown](#item-tech-news-17) ⭐️ 6.0/10
18. [Git Considers Voting to Set LLM Contribution Policy](#item-tech-news-18) ⭐️ 6.0/10
19. [Tsinghua Open-Sources OpenMise for Spatial Scene Editing in Video Generation](#item-tech-news-19) ⭐️ 6.0/10
20. [County-level power outage forecast beats NWS+SPC baseline by 2.4x PR-AUC](#item-tech-news-20) ⭐️ 6.0/10
21. [Siri AI Lead Mike Rockwell May Leave Apple in 2027](#item-tech-news-21) ⭐️ 6.0/10
22. [BYD Shows Robotic Charging Arm Delivering 1,000 kW in UAE](#item-tech-news-22) ⭐️ 6.0/10
23. [OPPO, vivo, Xiaomi, Honor Launch Android Sideload Developer Verification in China](#item-tech-news-23) ⭐️ 6.0/10
24. [EU Draft Digital Fairness Act Targets Addictive Design and Game Currency](#item-tech-news-24) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache nightly ROCm wheels for AMD Instinct GPUs](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache nightly-rbln release](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache Nightly CUDA 12.9 Wheels Released](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache Nightly Release \(CUDA 13.0 Wheels\)](#item-ai-projects-4) ⭐️ 5.0/10

**Financial News**
1. [China extends suspension of 24% US tariff, keeps 10% rate](#item-finance-news-1) ⭐️ 8.0/10

**Twitter News**
1. [OpenAI Introduces Control Room for Tracking and Halting Model Workloads](#item-twitter-news-1) ⭐️ 8.0/10
2. [Deedy demos Fable 5.2 generating a photorealistic real-time honey simulation in WebGL](#item-twitter-news-2) ⭐️ 7.0/10
3. [OpenAI dot Adds Multi-Computer Connection](#item-twitter-news-3) ⭐️ 7.0/10
4. [Fable 5.2: +10% Intelligence, +164% Cost](#item-twitter-news-4) ⭐️ 6.0/10
5. [Ryan Hoover: AI Agents Can Now Talk to Product Hunt](#item-twitter-news-5) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [E-means claims 10x faster k-means at equal loss](https://e-means.github.io/) ⭐️ 8.0/10

E-means, a new k-means variant, claims to converge in far fewer iterations while matching Lloyd’s algorithm’s clustering loss, advertised as about 10x faster. The project page offers no reproduced benchmarks in this source, but a commenter reports a 146x GPU speedup after adapting the method to an IVF index. Another commenter found no improvement when substituting E-means for Lloyd’s algorithm to relax an icosahedral equal-area mesh, indicating gains are workload-dependent.

hackernews · porridgeraisin · Nov 9, 18:45 · [Discussion](https://news.ycombinator.com/item?id=50429734)

**「Background」** K-means clustering conventionally uses Lloyd&\#x27;s algorithm, which alternates between assigning each point to the nearest centroid and recomputing centroids as the mean of assigned points; each iteration requires a full pass over the dataset. The e-means project page describes the new method as a modern, robust k-means algorithm developed at Meta FAIR and open-sourced to reduce the number of such epochs.

**「Impact」** Practitioners considering E-means should benchmark on their own workload: the reported 146x IVF-index speedup suggests large-dataset clustering may benefit, while the spherical-mesh case shows replacements for Lloyd’s algorithm do not always improve results.

**「Community discussion」** Commenters split on applicability: real\_faxenoff reported a 146x GPU speedup in IVF indexing, while jlhawn tried the same swap for spherical mesh relaxation and found no improvement, attributing E-means’ advantage to needing fewer passes over large datasets. shiandow speculated the update rule resembles expectation maximization with a friction term and preserves the centroid within the convex hull.

<details><summary>References</summary>
<ul>
<li><a href="https://e-means.github.io/">e - means : 10 x faster k - means at equal loss - Blog</a></li>

</ul>
</details>

**Tags**: `#clustering`, `#k-means`, `#algorithm-optimization`, `#machine-learning`, `#performance`

---

<a id="item-tech-news-2"></a>
### [Meta Releases Muse Ember, Its Smallest and Most Efficient Model](https://research.meta.ai/blog/muse-ember) ⭐️ 8.0/10

Meta released Muse Ember, its smallest and most efficient model, aimed at complex reasoning and agentic tasks. It supports a 1-million-token context window, handles text, image, audio, and video input, and can call tools. One commenter lists pricing of $0.10 per million input tokens, $0.004 per million cached input tokens, and $0.50 per million output tokens.

hackernews · dvaplima · Nov 9, 17:58 · [Discussion](https://news.ycombinator.com/item?id=50429024)

**「Context」** Meta&\#x27;s Muse line already includes two recent releases: Horizon&\#x27;s October 13 digest reported Muse Wonder, a multimodal model with mixed early tests, and the October 16 digest reported Muse Spark Open, a 816B-parameter open-weight model. Muse Ember now appears as the smaller, efficiency-focused counterpart in that same family.

**「Community Discussion」** Comments focused on evaluation caveats and open-weights availability: one commenter noted the best results appeared on mini-swe-agent rather than Meta&\#x27;s own harness, while another reported that higher effort levels did not visibly improve SVG generation. A third user said they could not locate open weights.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/muse-wonder">2026-10-13 — Meta AI unveils Muse Wonder multimodal model with mixed early tests</a></li>
<li><a href="https://research.meta.ai/blog/muse-spark-open">2026-10-16 — Meta launches Muse Spark Open, an 816B-parameter open-weight model</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#large language models`, `#model release`, `#meta`, `#agentic AI`

---

<a id="item-tech-news-3"></a>
### [Anthropic announces Claude Fable 5.2 and Mythos 5.2; 1,000 agents formalize FLT in 30 hours](https://www.anthropic.com/claude-fable-and-mythos-5-2) ⭐️ 8.0/10

Anthropic announced Claude Fable 5.2 and Mythos 5.2, claiming that a team of 1,000 Fable 5.2 agents fully formalized Fermat&\#x27;s Last Theorem in 30 hours with minimal human intervention. The announcement says this contrasts with an earlier research version that took 11 days using a purpose-built harness and guidance from a human researcher. The agents reportedly started from minimal prompts, built their own coordination, and used no mathematical references beyond a list of intermediate theorem statements. These are vendor claims from the announcement, not independently verified results.

hackernews · meetpateltech · Nov 9, 18:56 · [Discussion](https://news.ycombinator.com/item?id=50429906)

**「Earlier specialized Claude models」** Anthropic&\#x27;s earlier specialized Claude models already targeted hard technical and security tasks: Horizon&\#x27;s September 30 digest reported Claude Mythos Preview crossing a binary-exploitation threshold, and Horizon&\#x27;s October 17 digest reported Claude Mythos 5 designing more efficient quantum circuits. The formalization claim builds on a prior benchmark where a research Claude took 11 days to formalize Fermat&\#x27;s Last Theorem with a human-guided harness, according to coverage cited for this release.

**「Impact」** Users who mostly do ordinary software development may see little benefit from Fable 5.2 over current models: one commenter reports that Opus 5.5 on xhigh is already sufficient for aggressive development on a ~125k-line project, and that clear separation from Fable 5.2 appears mainly with unusually ambitious prompts.

**「Community discussion」** Commenters expressed skepticism about the release context and benchmark choices. One suspected that Claude 5.5 had been deliberately nerfed ahead of this version release, while another questioned benchmark pairings such as Fable xHigh versus Carbon Med, the omission of Carbon from the single cyber benchmark, and the switch to Argon for robodojo.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2111152183240511640">2026-10-17 — Anthropic: Claude Mythos 5 Designs More Efficient Quantum Circuits</a></li>
<li><a href="https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/">2026-09-30 — Anthropic Frontier Red Team: GLM-5.3 and Claude Mythos Preview cross binary exploitation threshold</a></li>
<li><a href="https://aiweekly.co/alerts/anthropics-1000-fable-52-agents-formalize-fermat-in-30-hours">Anthropic&#x27;s 1,000 Fable 5.2 Agents Formalize Fermat in 30 ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#multi-agent-systems`, `#theorem-proving`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [LingBot-Touch: Latent Prediction Outperforms Reconstruction for Tactile Pretraining](https://www.reddit.com/r/MachineLearning/comments/1xs05uo/latent_prediction_beats_reconstruction_for/) ⭐️ 8.0/10

LingBot-Touch, a self-supervised tactile encoder, predicts latent representations of masked contact instead of reconstructing raw sensor signals. On the same data, it achieves tactile-to-video top-5 recall of 32.1% at 1K hours and 49.3% at 4K hours, compared with 5.6% and under 9% for MAE, and 4.4% and 3.1% for VAE. Using three sensor types through a shared Transformer with canonical fingertip coordinates and 5D RoPE, frozen encoder features scored highest in 89 of 104 policy-task combinations, and LingBot-VLA improved from 57.21 to 75.04 on an unseen magnetic hand.

reddit · r/MachineLearning · /u/Zealousideal-War7154 · Nov 9, 18:52

**「Why Reconstruction Baselines Fall Short」** Tactile clips are mostly near-zero background, so reconstruction loss can decrease without learning to represent actual contact. LingBot-Touch uses JEPA-style latent prediction, and its masking ratio warms up from 40% to 80% over 300 steps because starting with high masking hid every contacting taxel in sparse signals and caused gradient explosions.

**「For Robotics Researchers」** Inference code and checkpoints are public, so researchers can evaluate the JEPA-pretrained encoder on their own dexterous manipulation tasks. The reported downstream gains are from the paper and have not been independently verified, but the Tiny model levels off around 4K hours while Small keeps improving, suggesting a larger version trained on more data is a possible next step.

**Tags**: `#self-supervised learning`, `#tactile sensing`, `#robotics`, `#representation learning`, `#JEPA`

---

<a id="item-tech-news-5"></a>
### [Google consumer Gemini may route Drive and Gmail data to human annotators](https://github.com/thisisme6598/gemini_files/) ⭐️ 7.0/10

A Hacker News discussion reports that consumer Google Gemini with Connected Apps can pass personal Gmail and Drive content to human annotators when a user enables the relevant app connections. The claim distinguishes consumer Gemini from Workspace Gemini, which Google states is not subject to human review. No official policy confirmation or technical documentation is provided in the source, so this remains a user-reported privacy concern rather than a confirmed change.

hackernews · gf74918 · Nov 9, 18:24 · [Discussion](https://news.ycombinator.com/item?id=50429426)

**「Earlier privacy pledge and recent policy reversal」** Before this change, Google&\#x27;s 2023 blog post said personal content from Gmail, Docs, and Drive used with Workspace features &quot;is not seen by human reviewers.&quot; An October 16, 2026 edit to that post and updated help documentation now state that consumer Gemini with Connected Apps can route personal Drive and Gmail content into human review pipelines, reversing the earlier assurance.

**「Practical takeaway」** Consumer Gemini users who have authorized Gmail or Drive through Connected Apps should treat their personal messages as potentially visible to human reviewers, and may want to disable those connections or use Workspace accounts if human review is a concern.

**「Community response」** The most substantive discussion distinguishes consumer Gemini from Workspace Gemini: one commenter points to Google&\#x27;s documentation claiming Workspace is not subject to human review, while another reports Gemini answers that appeared uncannily tuned to their Gmail content, suggesting connected-app data is being used in practice.

<details><summary>References</summary>
<ul>
<li><a href="https://daily.dev/posts/google-gemini-routes-personal-drive-files-and-emails-to-human-annotators-1yiwwc2e8">Google Gemini routes personal Drive files and emails to...</a></li>
<li><a href="https://emergent.sh/news/gemini-routes-drive-gmail-human-reviewers">Gemini Routes Drive and Gmail to Human Reviewers</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#google-gemini`, `#ai-ethics`, `#human-annotation`, `#data-practices`

---

<a id="item-tech-news-6"></a>
### [Claude Fable 5.2 Scores 65 on Artificial Analysis, Highest So Far](https://artificialanalysis.ai/models/claude-fable-5-2) ⭐️ 7.0/10

Artificial Analysis lists Anthropic&\#x27;s Claude Fable 5.2 with an intelligence score of 65, the highest result reported so far on that leaderboard. The score comes with a steep increase in token use: one commenter reports output tokens per task rose from 118,000 in Fable 5.1 \(46,000 answer and 71,000 reasoning\) to 274,000 in Fable 5.2 \(81,000 answer and 192,000 reasoning\), raising cost per task even with a claimed price cut. Another commenter notes that low and medium Fable 5.2 variants sit on the Pareto frontier between time per task and intelligence.

hackernews · theanonymousone · Nov 9, 20:04 · [Discussion](https://news.ycombinator.com/item?id=50431144)

**「Prior Artificial Analysis scores」** Horizon&\#x27;s October 24 digest reported that Artificial Analysis scored Claude Fable 5.1 at 53 and Claude Opus 5.5 at 58, making Fable 5.2&\#x27;s new 65 the highest score for the benchmark so far.

**「Impact」** For users evaluating the model, the cost change is material: per-task output token count more than doubled in the community-reported figures, so effective inference cost per task may be much higher than a unit price cut alone suggests. Teams should remeasure cost per completed task before adopting Fable 5.2 over 5.1.

**「Community discussion」** Commenters focused on cost rather than the score: rgbrenner reported the output-token jump from 118k to 274k per task, and brachkow argued the model&\#x27;s price is &\#x27;100x&\#x27; DeepSeek-Flash for only a few percent better, calling it unsustainable. Oliwary pushed back with a Pareto-frontier view that low/medium Fable 5.2 improves time-to-intelligence trade-offs, while GMoromisato shared an anecdote in which Fable produced shorter podcast scripts than Opus 5.5.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Oct/23/kimi-k31-pro/">2026-10-24 — Kimi K3.1 Pro 上线 API，承诺 11 月 4 日开放权重</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#benchmark`, `#cost-efficiency`, `#Anthropic`

---

<a id="item-tech-news-7"></a>
### [Canada launches Real-Time Rail 24/7 payment system](https://www.payments.ca/canada-launches-real-time-rail-bringing-247-payment-infrastructure-national-economy) ⭐️ 7.0/10

Payments Canada announced the launch of Canada&\#x27;s Real-Time Rail \(RTR\), a 24/7 real-time payment system, with an initial participant list that includes Wealthsimple, Questbank, Peoples Trust Company, Paramount Commerce, KOHO, DoBusiness.com, Digital Commerce Bank, and Bank of America. None of Canada&\#x27;s major banks appear on that list.

hackernews · ocd · Nov 9, 16:00 · [Discussion](https://news.ycombinator.com/item?id=50427362)

**「Real-time vs. legacy payment rails」** A Real-Time Rail \(RTR\) is a payment infrastructure that clears and settles transactions continuously, 24/7, rather than in batches during business hours. Canada’s prior retail payment landscape relied heavily on Interac’s proprietary e-Transfer system and batch-based clearing, which did not provide a general-purpose, always-on settlement rail for banks and fintechs.

**「Impact」** The announced launch gives fintech developers and smaller institutions a shared real-time rail to build on, though early reach may be limited because the initial participant list omits Canada&\#x27;s major banks.

**「Community Discussion」** One commenter welcomed the move as making Interac&\#x27;s proprietary e-Transfer functionality available as a public good, while another questioned near-term usefulness because the initial participant list omits Canada&\#x27;s major banks. A separate comment compared the US FedNow system unfavorably, noting its limited bank support and transaction fees.

**Tags**: `#fintech`, `#payments`, `#infrastructure`, `#Canada`, `#banking`

---

<a id="item-tech-news-8"></a>
### [Show HN: watched.earth Finds Every Satellite Pass and Photo Over Any Place](https://www.watched.earth/) ⭐️ 7.0/10

The creator released a browser tool at watched.earth that computes every satellite pass over a typed location in the last 7 days using SGP4 against the CelesTrak catalog, returning results in about half a second, and retrieves real Sentinel-2/Landsat/NASA imagery for those passes. It draws all ~17,000 cataloged objects on the GPU and solves Kepler&\#x27;s equation per frame, and the author claims a brute-force check found zero missed passes at poles, the antimeridian, and tiny swaths. The tool only labels a pass as &quot;watched&quot; when a real image exists and does not store the user&\#x27;s location; the code is available on GitHub.

hackernews · a585gupt · Nov 9, 17:51 · [Discussion](https://news.ycombinator.com/item?id=50428907)

**「Background」** Satellite overpass prediction depends on orbital propagation using SGP4 from CelesTrak TLEs; the imagery side uses Sentinel-2 and Landsat scenes whose timestamps can be offset by 5–10 minutes from the actual crossing time. The tool addresses the gap between predicted passes and available imagery by matching only passes with real photos.

**「Impact」** Because the pass search runs in the browser, users can check which satellites photographed a location without sending the location to a server, which matters for privacy-sensitive queries.

**「Community Discussion」** Comments were split: one commenter accused the post of being LLM-generated and argued it should be removed, while others praised its style and execution; another user reported that typing in the location field was almost impossible due to cursor spacing issues.

**Tags**: `#satellite-imagery`, `#open-source`, `#sgp4`, `#webgl`, `#geospatial`

---

<a id="item-tech-news-9"></a>
### [Benchmark Topic Pages Now Cover 2026 ICML, CVPR, ICLR, AAAI Papers](https://www.reddit.com/r/MachineLearning/comments/1xs6494/followup_2026_papers_are_finally_in_the_topic/) ⭐️ 7.0/10

The research topic pages at atlas.scime.ai have been updated to include 2026 ICML, CVPR, ICLR, and AAAI papers, with AI-extracted benchmark results from about 101,000 full texts, up from 79,000 when the pages first launched. Coverage is nearly complete for ICML, CVPR, and AAAI, plus 4,100 of 5,400 ICLR papers; NeurIPS 2026 remains only about half covered because many PDFs are not yet public. The update also adds &quot;newspaper&quot; summaries for ICML, CVPR, and ICLR 2026, reporting that LLM agents rose from 1.2% to 4.4% of ICML papers and Qwen is the most-used base model in results tables at all three. The author cautions that the numbers are AI-extracted, not manually checked, and papers over-report what worked, so the pages should be treated as a starting point rather than a leaderboard.

reddit · r/MachineLearning · /u/latenticlabs · Nov 9, 22:39

**「Earlier topic pages stopped at 2025」** Horizon&\#x27;s November 4 digest reported the original Atlas topic pages, which organized roughly 109,000 accepted ML papers from ICML, NeurIPS, ICLR, CVPR, and AAAI into about 1,260 topic pages and extracted results tables and ablations from 79,000 full texts; at that time the benchmark records and ablations stopped at 2025. This follow-up expands extraction to about 101,000 full texts and adds 2026 ICML, CVPR, ICLR, and AAAI papers, with NeurIPS 2026 still incomplete because many PDFs are not public.

**「Impact」** Researchers can now browse 2026 benchmark results and trends—for example, compact/efficient Gaussian splatting&\#x27;s Mip-NeRF 360 PSNR reaching 30.1 this year—but should verify individual numbers against the source papers because the extraction is automated and includes over-reported results; the author explicitly asks domain experts to flag apparent errors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xmk8rx/we_turned_10_years_of_ml_papers_into_one_page_per/">2026-11-04 — Atlas research map turns 109k ML papers into benchmark topic pages</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#benchmarking`, `#research tools`, `#computer vision`, `#conference papers`

---

<a id="item-tech-news-10"></a>
### [SwarmEvolve Uses Latent-Agent Swarms for Faster Math Discovery](https://www.reddit.com/r/MachineLearning/comments/1xrunu7/using_latentagent_swarms_for_math_discovery_and/) ⭐️ 7.0/10

SwarmEvolve, a new framework described in a self-published Reddit post and accompanying paper, uses swarms of hundreds of latent-reasoning agents built on Qwen3 8B, 14B, and 32B models that share KV caches instead of writing out thoughts. The authors claim these swarms reach optimization scores in about 5 minutes that previous open-source evolutionary systems—OpenEvolve, ShinkaEvolve, and CodeEvolve—needed more than 1 hour to achieve, and the 8B model matched the best known circle packing. The framework has been extended to Qwen3.5 and Muse models, but code is listed as &\#x27;available soon&\#x27; and the claims have not been independently verified.

reddit · r/MachineLearning · /u/QileHQ · Nov 9, 15:30

**「Background」** Earlier work such as Google DeepMind&\#x27;s AlphaEvolve demonstrated evolution-style program discovery by having an LLM generate candidate solutions, score them, and iteratively improve them, including finding a faster 4x4 complex matrix multiplication than the long-standing 1969 record. The post notes that AlphaEvolve relied on Gemini models and that similar open-source evolutionary frameworks were typically slow and expensive to run.

**「Practical impact」** For teams running open-source LLM evolutionary optimizers, SwarmEvolve&\#x27;s reported speedup—matching OpenEvolve/ShinkaEvolve/CodeEvolve scores in about 5 minutes instead of over 1 hour using Qwen3 8B–32B—would cut per-experiment compute time by roughly an order of magnitude. The framework&\#x27;s code is only &\#x27;available soon,&\#x27; so independent reproduction and benchmarking are not yet possible.

**Tags**: `#machine learning`, `#latent reasoning`, `#evolutionary algorithms`, `#LLM agents`, `#mathematical optimization`

---

<a id="item-tech-news-11"></a>
### [Twindex: exact replayable proofs of parameter indistinguishability for ODE/PDE/PINN models](https://www.reddit.com/r/MachineLearning/comments/1xryhhg/twindex_exact_replayable_proofs_that_your_data/) ⭐️ 7.0/10

Twindex produces exact, replayable JSON certificates that show whether two parameter sets are indistinguishable by a given dataset under a stated bounded-noise assumption, aimed at ODE, PDE, and PINN parameter estimation. In a real-data example using the 1978 boarding-school flu outbreak, after five days of counts SIR models with R0=2.5 and R0=20 both fit every count; Twindex identified a next-day count that separated them, and the real count ruled out both. It is available via pip and a browser demo, with limitations including bounded noise, conditional proofs, difficulty scaling beyond a few parameters, and no independent expert proof audit yet.

reddit · r/MachineLearning · /u/Longjumping\_Glass852 · Nov 9, 17:50

**「Background」** Standard PINN, least-squares, and Bayesian fits return parameter values but do not prove that very different parameters would not fit the data equally well. Bounded-error estimation with validated integration is established prior work; Twindex&\#x27;s new part is portable exact certificates and a small rational-arithmetic checker anyone can replay.

**「Impact」** Researchers fitting ODE/PDE/PINN models can install Twindex or use the browser checker to produce certificates locally and replay them with standard-library Python rational arithmetic \(~0.2 s per proof in the browser\). A VALID twin pair means that, under the stated bounded-noise assumption, no estimator can recover that parameter better than ± half the gap, letting users detect practical non-identifiability before relying on fitted values.

**Tags**: `#parameter identifiability`, `#scientific machine learning`, `#PINNs`, `#uncertainty quantification`, `#formal verification`

---

<a id="item-tech-news-12"></a>
### [AI-designed avian flu vaccine candidate shows broad protection in mice and ferrets](https://www.cam.ac.uk/stories/ai-developed-vaccines-against-viruses) ⭐️ 7.0/10

Cambridge researchers used AI to design a novel avian influenza vaccine candidate and reported in Cell Reports Medicine that it induced broad immune and protective responses in mice and ferrets, outperforming a control formulation based on a WHO candidate vaccine virus. The team plans to advance the candidate into human clinical trials, but no protection in people has been demonstrated yet.

telegram · zaihuapd · Nov 9, 03:00

**「Background」** The study compares its AI-designed antigen against a control based on WHO candidate vaccine viruses, which are conventional starting points for avian influenza vaccines. The AI-generated broad-spectrum antigen does not exist in nature, and its protective effect has so far been demonstrated only in mice and ferrets.

**Tags**: `#AI`, `#vaccine design`, `#avian influenza`, `#computational biology`, `#biotech`

---

<a id="item-tech-news-13"></a>
### [Google Unveils TPU 8tx and 8i Max, Stepping Up Nvidia Rivalry](https://www.bloomberg.com/news/articles/2026-11-09/google-escalates-nvidia-rivalry-with-new-versions-of-its-tpu-systems) ⭐️ 7.0/10

Google announced two new Tensor Processing Units, TPU 8tx and TPU 8i Max, as announced products without detailed specs or availability. TPU 8tx targets government and strictly regulated industries for secure, confidential data and will work alongside AMD chips; TPU 8i Max targets ultra-long-context AI by packaging two TPU chips together for more compute and memory. The company says it is breaking its previous two-year processor cadence and aims to position TPUs as an alternative to Nvidia GPUs for customers such as Apple, Meta, Oracle, and Anthropic.

telegram · zaihuapd · Nov 9, 13:36

**「Earlier TPU ecosystem moves」** Horizon&\#x27;s November 6 digest reported Google positioning its Ironwood TPU as an alternative to NVIDIA&\#x27;s CUDA for AI inference, citing TorchTPU, vLLM, SGLang, llm-d, and Ray support. Horizon&\#x27;s October 21 digest reported Google open-sourcing TorchTPU, a native PyTorch backend for TPUs. Those ecosystem moves set the stage for the latest 8tx and 8i Max variants aimed at secure regulated workloads and ultra-long-context AI.

**「Impact」** Potential enterprise and government buyers cannot yet assess the new chips against Nvidia equivalents because Google did not publish watts-per-token or dollars-per-token figures, pricing, or release dates.

**「Community Discussion」** Hacker News commenters expressed skepticism about actual access and detail, asking why Google does not sell the chips and where the watts-per-token or dollars-per-token comparison figures are relative to Nvidia.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/tpu-strikes-the-king">2026-11-06 — Google Ironwood TPU Positions as CUDA Inference Alternative</a></li>
<li><a href="https://github.com/google-pytorch/torch_tpu">2026-10-21 — Google open-sources TorchTPU, native PyTorch backend for TPUs</a></li>

</ul>
</details>

**Tags**: `#Google`, `#TPU`, `#AI hardware`, `#Nvidia`, `#cloud computing`

---

<a id="item-tech-news-14"></a>
### [USPS Releases Official ZIP Code Boundary Polygons](https://postalpro.usps.com/zcb) ⭐️ 6.0/10

USPS has published official ZIP Code boundary polygons through its PostalPro portal. According to community comments, the lowest pricing tier costs about $10,000, and free Census ZCTA shapefiles remain a widely used alternative for many geospatial purposes.

hackernews · munro · Nov 9, 19:58 · [Discussion](https://news.ycombinator.com/item?id=50431058)

**「Background」** ZIP codes were created as postal delivery routes rather than fixed geographic areas, so precise boundary polygons have not previously been available directly from USPS. Users have instead relied on Census ZCTA approximations, which may miss some commercial-only ZIP codes.

**「Impact」** Organizations that need authoritative USPS ZIP boundaries will need to budget for the paid offering, while many noncommercial or small-scale users can continue using free ZCTA shapefiles as an imperfect substitute.

**「Community Discussion」** Commenters debated whether federally produced geospatial data should be free; SwellJoe argued that the $10,000 minimum undermines transparency and accountability, while showerst noted that free Census ZCTA shapefiles are close enough for many uses despite some fuzziness and missing commercial-only ZIP codes.

**Tags**: `#geospatial`, `#USPS`, `#open-data`, `#government-data`, `#GIS`

---

<a id="item-tech-news-15"></a>
### [Opus 5.5 November 3 Change Debated; Benchmark Rerun Stable](https://twitter.com/shanemelaugh/status/2119192075505893695) ⭐️ 6.0/10

Hacker News commenters are debating whether the Opus 5.5 model was silently changed on November 3, 2026, but the supplied evidence is inconclusive. A user who re-ran Opus 5.5 on November 9 with the same prompt and settings as a September benchmark reported 128,000 streamed tokens costing $2.56 with an empty file in both runs, and Batch API output of 255,957 tokens in September versus 243,707 tokens today, describing the output as stable. Other commenters allege unannounced A/B testing or quantization and account-freshness variation, but no vendor confirmation or authoritative evaluation is provided.

hackernews · rzk · Nov 9, 07:04 · [Discussion](https://news.ycombinator.com/item?id=50422069)

**「Context」** Anthropic introduced Claude Opus 5.5 on September 22, 2026 as its new leading model for complex coding and agent work, with early testers reporting large performance jumps. Horizon&\#x27;s September 29 digest noted that a max-thinking bug already affected Opus 5.5, consuming 128,000 tokens and failing to produce an SVG, which provides a concrete earlier quality issue to compare with the new reports of a November 3 behavior change.

**「Impact」** Developers using Opus 5.5 cannot currently rely on community anecdotes to confirm a capability change; the one public benchmark rerun cited found comparable token output and cost, but no vendor statement or controlled evaluation establishes whether an unannounced change occurred. Teams should track their own reproducible benchmarks rather than treating the November 3 reports as confirmed.

**「Community Discussion」** Substantive comments split between speculation and measurement: PhunkyPhil and a linked Reddit thread suggest A/B testing or release-cycle fiddling with quantization, while ianberdin’s rerun and losvedir’s reference to a public eval see no regression. PaulKeeble argues that local models such as Qwen 3.8 27B avoid such unannounced changes, even if less capable.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/28/claude-sonnet-5-5/">2026-09-29 — Claude Sonnet 5.5: faster, cheaper, but max thinking fails</a></li>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5.5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#large-language-models`, `#model-evaluation`, `#developer-tools`, `#software-engineering`

---

<a id="item-tech-news-16"></a>
### [Simon Willison&\#x27;s Beep Locator triangulates mystery beep using Claude Code](https://simonwillison.net/2026/Nov/9/mysterious-beeps/) ⭐️ 6.0/10

Simon Willison used Claude Code \(Opus 5.5, extra thinking mode\) to build Beep Locator, an open-source Python web app that triangulates sounds using spare phones, tablets, and laptops as browser-based listeners. Listeners record a 60-second audio buffer and report FFT-detected beeps over WebSockets; a server-requested chirp aligns audio clips from each device. The system localized a mystery intermittent beep to within about 40 cm, leading him to an old carbon monoxide detector needing new batteries. Because automatic device self-positioning did not work well, he added a manual &\#x27;Rough mode&\#x27; for initial device placement.

rss · Simon Willison · Nov 9, 23:57

**「Background」** Claude Code found the 2007 BeepBeep paper, which demonstrated high-accuracy acoustic ranging and localization using only commodity speakers, microphones, and device-to-device communication; Beep Locator applies that same approach to browser-based multi-device triangulation.

**「Impact」** The working code is available on GitHub, giving developers a concrete example of browser-based multi-device acoustic localization that combines Python/WebSockets coordination with FFT beep detection and chirp-aligned clip syncing. Users adapting it should expect to provide initial device locations manually because self-positioning proved unreliable.

**Tags**: `#AI-assisted development`, `#audio triangulation`, `#Claude Code`, `#open source`, `#software engineering`

---

<a id="item-tech-news-17"></a>
### [Hide verbose AI-generated PR descriptions with details/summary in GitHub Markdown](https://simonwillison.net/2026/Nov/9/details-summary/) ⭐️ 6.0/10

Simon Willison describes a personal workflow for GitHub pull requests: he writes a short human-curated opener, then wraps the full AI-generated description in &lt;details&gt;&lt;summary&gt; tags, using the model name and effort level as the summary text. GitHub Markdown renders these tags as a collapsed expandable section, so the reader sees only the high-level introduction first. He shows examples from datasette, datasette-agent, and llm PRs, noting the full agent-written text remains expandable.

rss · Simon Willison · Nov 9, 04:25

**「Background」** AI coding agents such as Claude Code and Codex often generate accurate but lengthy PR descriptions, which can overwhelm reviewers and read as &quot;slop.&quot; GitHub Markdown already supports the HTML &lt;details&gt;&lt;summary&gt; elements directly in PR bodies and issue comments.

**「Impact」** For developers with AI-assisted PRs on GitHub, this lets the human-selected summary and optional screenshot act as the visible entry point, while the full agent-written text remains accessible under an expandable element.

**Tags**: `#AI coding agents`, `#pull requests`, `#developer workflow`, `#HTML`, `#software engineering`

---

<a id="item-tech-news-18"></a>
### [Git Considers Voting to Set LLM Contribution Policy](https://lwn.net/Articles/1104195/) ⭐️ 6.0/10

The Git project is considering adopting a voting process to settle its policy on accepting LLM-written contributions, following discussion at the recent Git Contributor&\#x27;s Summit. The project, which has never been governed democratically, has not yet reached a decision or published a policy.

rss · LWN.net · Nov 9, 15:05

**「Background」** The Git Contributor&\#x27;s Summit recently discussed whether and how to accept LLM-written contributions, part of a wider 2026 debate among development projects. Git has never been governed as a democracy, making the proposed voting process a notable procedural shift for the project.

**Tags**: `#git`, `#open source`, `#llm`, `#software development`, `#governance`

---

<a id="item-tech-news-19"></a>
### [Tsinghua Open-Sources OpenMise for Spatial Scene Editing in Video Generation](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E8%A7%86%E9%A2%91%E7%94%9F%E6%88%90%E4%B8%8D%E5%86%8D%E5%8F%8D%E5%A4%8D%E6%8A%BD%E5%8D%A1%EF%BC%81%E6%B8%85%E5%8D%8E%E5%BC%80%E6%BA%90%EF%BC%8C%E7%BB%99%E6%A8%A1%E5%9E%8B%E8%A3%85%E4%B8%8A%E3%80%8C%E4%B8%89%E7%BB%B4%E7%A9%BA%E9%97%B4%E5%A4%A7%E8%84%91%E3%80%8D) ⭐️ 6.0/10

Tsinghua University and University of Pennsylvania researchers have open-sourced OpenMise, an agent-oriented spatial scene editing tool that splits video generation into a &\#x27;Builder + Render&\#x27; pipeline. The builder stage uses a coding agent with Blender to lay out scene, characters, actions, cameras, and lighting as an editable 3D draft; the render stage hands that draft to an existing video generation model for final visual output. The project is available on GitHub and is presented as a way to reduce repeated sampling by separating spatial consistency from rendering quality. The source does not include independent benchmarks or quantitative comparisons.

rss · 新智元 · Nov 9, 04:54

**「Previous Seedance release and OpenMise&\#x27;s role」** ByteDance released Seedance 2.5 4K in late October, which Horizon&\#x27;s October 24 digest described as the strongest version of the Seedance video-generation series, currently available only to select enterprise customers \[tool-1-2\]. The OpenMise GitHub repository describes the project as a bridge connecting Agents to spatial scenes, where the Agent interprets requests and OpenMise supplies spatial editing workflows and operation conventions for scene tools such as Blender \[tool-2-1\].

**「Impact」** Video creators and agent developers can replace repeated full-clip generation with an editable 3D draft in Blender before final rendering, reducing wasted compute; the workflow requires using OpenMise with an existing video generation model as the renderer.

<details><summary>References</summary>
<ul>
<li><a href="https://mp.weixin.qq.com/s/yUa8oh-IWfl5lDQzGSKWeg">2026-10-24 — ByteDance Releases Seedance 2.5 4K With 480P Draft Mode</a></li>
<li><a href="https://github.com/Rath-Team/OpenMise/blob/main/README.en.md">OpenMise/README.en.md at main · Rath-Team/OpenMise · GitHub</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#open source`, `#3D spatial understanding`, `#AI`, `#Tsinghua`

---

<a id="item-tech-news-20"></a>
### [County-level power outage forecast beats NWS+SPC baseline by 2.4x PR-AUC](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 6.0/10

The author reports an XGBoost model that forecasts the probability that at least 5% of customers in each of 216 Missouri and Illinois counties are newly without power during the 6 hours starting 2 hours ahead. Trained on 2020–2024 HRRR storm fields and county/outage features and tested on issued 2025 forecasts, the model achieved PR-AUC 0.094 versus 0.039 for a NWS warning plus SPC Day 1 outlook baseline, a reported 2.4× ratio \(95% bootstrap range 2.0–3.3×\). At equal alert volume it caught 30% of new outages versus 17% baseline, with precision 15% versus 11%; the base rate is 0.5% of county-hours. The author also reports an early transfer test catching 31% versus 19% in Iowa, Indiana, and Michigan, and the model has been live since Nov 1 with forecasts saved for a blind test.

reddit · r/MachineLearning · /u/CarRepresentative843 · Nov 9, 21:34

**「Background」** The baseline uses a rate table of National Weather Service warnings and Storm Prediction Center Day 1 outlooks fit on the same rows. HRRR provides the storm-related inputs—gusts, shear, CAPE, icing—used as forecast features, and the model deliberately targets only new outages rather than outages already underway, which makes the prediction task harder and avoids crediting the model for reporting current conditions.

**「Impact」** Utilities and emergency managers using the reported model should expect low precision: even with the 2.4× PR-AUC improvement, only 15% of equal-volume alerts correspond to new outages, given the 0.5% base rate.

**Tags**: `#machine learning`, `#time series forecasting`, `#power outage prediction`, `#XGBoost`, `#weather forecasting`

---

<a id="item-tech-news-21"></a>
### [Siri AI Lead Mike Rockwell May Leave Apple in 2027](https://9to5mac.com/2026/11/08/john-ternus-pushing-craig-federighi-to-move-faster-software-engineering/) ⭐️ 6.0/10

Bloomberg&\#x27;s Mark Gurman reports in Power On that Mike Rockwell, the executive behind Vision Pro and the new Siri AI, is seriously considering leaving and may step down as Siri engineering VP or leave Apple next year. If he departs, his responsibilities would likely go to Amar Subramanya, who joined from Google last year, and Sebastien Marino, a deputy to Craig Federighi. Some favor Marino as future software engineering head, but Federighi has no succession plan. The report remains an unconfirmed personnel rumor.

telegram · zaihuapd · Nov 9, 04:33

**「Siri AI leadership context」** Mike Rockwell is the Apple executive responsible for the Vision Pro and the new Siri AI. Horizon&\#x27;s October 1 digest reported that Apple was preparing a smart home hub with an upgraded Siri AI, indicating that the Siri overhaul was already moving into product plans before this personnel rumor emerged.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-09-30/apple-is-finally-ready-to-enter-its-next-big-category-the-smart-home">2026-10-01 — Apple Plans October 13 Launch of Smart Home Hub with Siri AI</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Siri`, `#AI`, `#leadership`, `#rumor`

---

<a id="item-tech-news-22"></a>
### [BYD Shows Robotic Charging Arm Delivering 1,000 kW in UAE](https://m.mydrivers.com/newsview/1164193.html) ⭐️ 6.0/10

BYD demonstrated a robotic charging arm in the UAE that automatically opens the EV charge port, inserts and removes the connector, and closes the cover, letting drivers leave after parking. The displayed system supplies up to 1,000 kW; paired with BYD&\#x27;s second-generation blade battery, the official demonstration claimed 5 minutes for a fast top-up and 9 minutes for a full charge. The site combined solar, storage, and charging, and showed a &\#x27;one-click park-and-charge&\#x27; mode in which the car parks itself before the arm connects. These capabilities were shown as a demonstration rather than a commercially available product.

telegram · zaihuapd · Nov 9, 05:20

**「Background」** The demonstration’s fast-charging figures depend on BYD’s second-generation blade battery, which the source says enables the advertised 5-minute top-up and 9-minute full charge at up to 1000 kW. The UAE station is also described as an integrated solar-storage-charging system with a “one-click park-and-charge” function.

**「Impact」** For EV drivers, a commercial version could reduce charging wait times and remove the need to handle charging cables, but the source only reports a demonstration with vendor performance claims, not independent verification or a shipping rollout.

**Tags**: `#electric vehicles`, `#robotic charging`, `#hardware`, `#energy storage`, `#automation`

---

<a id="item-tech-news-23"></a>
### [OPPO, vivo, Xiaomi, Honor Launch Android Sideload Developer Verification in China](https://mp.weixin.qq.com/s/ZiKBASSLzvsZ6WR2AUmFeg) ⭐️ 6.0/10

OPPO, vivo, Xiaomi, and Honor have jointly launched Android sideloading developer identity verification \(ADV\) in mainland China, with verification results mutually recognized among the four vendors. The mechanism is intended to establish a trusted association between developers and their apps and help users identify app origin and safety. Apps already registered and listed on the four vendors&\#x27; open platforms are automatically submitted for verification without a separate application; when an unverified app is sideloaded, an &\#x27;unverified&\#x27; prompt appears and the user must manually confirm to continue installation.

telegram · zaihuapd · Nov 9, 11:44

**「Background」** Android allows users to sideload APK files from outside official app stores, bypassing store-level review and making developer identity harder to verify. In mainland China, OPPO, vivo, Xiaomi, and Honor each run their own Android-based systems and device ecosystems, so a cross-vendor verification scheme has to work across these platforms.

**Tags**: `#Android`, `#sideloading`, `#app security`, `#developer verification`, `#China tech`

---

<a id="item-tech-news-24"></a>
### [EU Draft Digital Fairness Act Targets Addictive Design and Game Currency](https://www.mlex.com/mlex/articles/2546584/digital-businesses-face-addictive-design-controls-under-draft-eu-consumer-law) ⭐️ 6.0/10

A leaked draft of the EU&\#x27;s Digital Fairness Act would impose new consumer-protection rules on digital businesses, including limits on addictive design features such as autoplay and continuous-use rewards, clearer subscription cancellation with a cancel button, renewal reminders and human support, and explicit consent before free trials convert to paid subscriptions. It would ban in-game paid loot boxes, pay-to-win mechanics and profiling advertising aimed at minors, and require game virtual currencies to disclose their real-money value. The European Commission is scheduled to present the proposal on November 11 together with a reform of the consumer protection cooperation framework; violations could draw fines up to 6% of global annual turnover. The draft still requires approval by the European Parliament and EU governments before it can take effect.

telegram · zaihuapd · Nov 9, 16:42

**「Prior EU action on harmful design」** EU regulators have already pursued harmful platform design under the Digital Services Act: Horizon&\#x27;s November 7 digest reported that the European Commission charged TikTok&\#x27;s recommendation algorithm with creating harmful &\#x27;rabbit hole&\#x27; effects, with potential fines of up to 6% of global annual revenue. The leaked draft Digital Fairness Act would broaden such controls from a specific DSA case to general consumer-facing digital businesses.

**「Impact」** If adopted, digital businesses operating in the EU would need to allow users to disable certain engagement-driving features, make subscription cancellation and renewal terms clearer, and display real-money values for in-game virtual currencies, with non-compliance risking fines of up to 6% of global annual turnover.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/06/eu-charges-tiktok-harmful-algorithmic-rabbit-hole-effects.html">2026-11-07 — EU charges TikTok recommendation algorithm with harmful rabbit-hole effects</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#consumer protection`, `#addictive design`, `#subscription`, `#gaming`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache nightly ROCm wheels for AMD Instinct GPUs](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly automated build of LMCache Python wheels for AMD Instinct GPUs \(MI300X/MI325X, MI350X/MI355X\), ABI-matched to upstream vLLM ROCm images with torch 2.13 and cp312.

github · github-actions\[bot\] · Nov 9, 07:57

**「解决的痛点」** Users on AMD Instinct GPUs often face ABI mismatches or need to build from source when combining LMCache with vLLM ROCm containers. These pre-built ROCm 7.2 wheels match upstream vLLM&\#x27;s torch/cp312 ABI, allowing pip installation with --no-deps to avoid dependency conflicts.

**「背景与影响」** LMCache is an LLM caching layer. This nightly release tracks the dev branch and provides ROCm support for AMD Instinct gfx942/gfx950, aligning with the upstream vllm-openai-rocm image. It is an early testing artifact, not a stable feature release.

**Tags**: `#llm-cache`, `#rocm`, `#amd`, `#nightly`, `#vllm`

---

<a id="item-ai-projects-2"></a>
### [LMCache nightly-rbln release](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

Nightly wheel release of LMCache \(v0.5.8.dev74+rbln\) targeting Rebellions RBLN NPU, built from the dev branch on 2026-11-09 against torch-rbln 0.12.0 \(torch 2.13.0+cpu\).

github · github-actions\[bot\] · Nov 9, 07:44

**「Problem Solved」** This wheel addresses the friction of installing and running LMCache on RBLN NPU hardware. It provides a prebuilt binary that matches the RBLN software stack \(torch-rbln, rebel-compiler, driver\), which are not bundled and must be installed separately, reducing manual build and compatibility issues.

**「Background」** LMCache is an LLM inference acceleration library focused on KV cache management. RBLN is Rebellions&\#x27; NPU for AI workloads. This nightly release from the dev branch is an automated snapshot, indicating ongoing integration for RBLN support, but it is not a major version update and introduces no architectural changes.

**Tags**: `#LMCache`, `#LLM`, `#inference`, `#KV cache`, `#nightly`, `#RBLN NPU`

---

<a id="item-ai-projects-3"></a>
### [LMCache Nightly CUDA 12.9 Wheels Released](https://github.com/LMCache/LMCache/releases/tag/nightly-cu129) ⭐️ 5.0/10

Nightly release of LMCache providing pre-built CUDA 12.9 wheels for linux/amd64 and linux/arm64, built from the dev branch on 2026-11-09. Users can install via pip with the provided command.

github · github-actions\[bot\] · Nov 9, 12:32

**「Problem Solved」** Eliminates the need to compile LMCache from source with CUDA 12.9, simplifying installation and testing on common platforms. Addresses compatibility issues with the latest CUDA toolkit and speeds up deployment for developers using nightly builds.

**「Background &amp; Impact」** LMCache is an open-source KV cache management layer for LLM inference, designed to store, reuse, compress, and move KV caches across GPU, CPU, and external backends \(tool-1-2, tool-1-3\). This nightly release provides pre-built CUDA 12.9 wheels for linux/amd64 and linux/arm64, built from the dev branch on 2026-11-09. It lowers installation friction for users running PyTorch with CUDA 12.9, fitting into the project&\#x27;s routine distribution across CUDA versions. No new features or major optimizations are described; the release primarily serves compatibility with the latest CUDA toolchain.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#nightly`, `#CUDA`, `#wheels`, `#LLM caching`

---

<a id="item-ai-projects-4"></a>
### [LMCache Nightly Release \(CUDA 13.0 Wheels\)](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

Automated nightly build of LMCache with prebuilt CUDA 13.0 wheels for Linux amd64 and arm64, built from the dev branch.

github · github-actions\[bot\] · Nov 9, 09:27

**「Problem Solved」** Provides ready-to-install nightly wheels that avoid manual compilation, enabling developers to test the latest development branch on CUDA 13.0 environments across x86\_64 and ARM64 Linux systems.

**「Background」** LMCache is an open-source KV cache management layer for LLM inference, described as becoming a de-facto standard for reusing prompt and conversation context across serving engines \(tool-1-1, tool-1-2, tool-1-3\). This nightly release provides prebuilt CUDA 13.0 wheels for Linux \(amd64/arm64\) from the dev branch, giving early adopters a convenient way to test the latest development state without building from source. It is a routine automated update rather than a feature release, and the source item does not detail performance or architectural changes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#inference`, `#caching`, `#nightly`, `#CUDA`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China extends suspension of 24% US tariff, keeps 10% rate](https://mp.weixin.qq.com/s/nNxJB3y0YA_2zJvOK6onUQ) ⭐️ 8.0/10

China&\#x27;s State Council Tariff Commission announced that the 24% additional tariff on U.S. goods will remain suspended for two months starting November 10, 2026, while the 10% tariff will be retained.

telegram · zaihuapd · Nov 9, 04:03

**「Background」** The State Council Tariff Commission previously announced a 90-day suspension of the 24% additional tariff on US goods while retaining the 10% rate, which serves as the basis for this two-month extension.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/K6PK1HVO0514E1NL.html">中 美 发布联合声明： 24 % 对 等 关 税 暂 停 90天，保留 10 ...</a></li>

</ul>
</details>

**Tags**: `#tariffs`, `#US-China trade`, `#trade policy`, `#China`, `#economic policy`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [OpenAI Introduces Control Room for Tracking and Halting Model Workloads](https://x.com/OpenAI/status/2119913172039868579) ⭐️ 8.0/10

OpenAI announced Control Room, a central system for tracking model workloads across its research infrastructure and stopping them quickly when safety or security concerns arise. It connects every research inference workload, including agentic sampling for model training and evaluation and data processing, and works with OpenAI&\#x27;s misalignment monitoring systems. Control Room can halt model output within 35 seconds of a decision to intervene. The post describes it as one part of a holistic approach to safe frontier model training and deployment.

twitter · OpenAI · Nov 9, 22:01

**「Background」** This announcement from OpenAI&\#x27;s official account highlights a specific operational safety measure: rapid intervention. The 35-second halt target is presented as a concrete responsiveness benchmark. The post places Control Room within broader safety infrastructure but does not detail the misalignment monitoring systems or other components in this announcement.

**Tags**: `#AI safety`, `#OpenAI`, `#infrastructure`, `#model monitoring`

---

<a id="item-twitter-news-2"></a>
### [Deedy demos Fable 5.2 generating a photorealistic real-time honey simulation in WebGL](https://x.com/deedydas/status/2119930300990177509) ⭐️ 7.0/10

Deedy shared a demo of Fable 5.2 generating a photorealistic, physics-based real-time honey simulation in WebGL from the prompt: “Can you write the most intricate photorealistic simulation of honey in WebGL in the browser.” The post states the video is completely physics-based realtime render, with no additional technical details provided.

twitter · Deedy · Nov 9, 23:09

**「Background」** Deedy&\#x27;s post shows a prompt to Fable 5.2 for &\#x27;the most intricate photorealistic simulation of honey in WebGL in the browser,&\#x27; with a video described as completely physics-based realtime render. Fable 5.2 is an Anthropic model; Anthropic&\#x27;s announcement reports a RoboDojo Sim score of 64.9% at Max effort, more than double Fable 5.1&\#x27;s 27.6% \(tool-1-1\). Artificial Analysis provides independent comparisons of Fable 5.2 Max across quality, price, and performance metrics \(tool-1-3\). Earlier Horizon coverage noted that Fable 5 and 5.1 were used to ship prompt-driven game changes in Spawn, a predecessor demonstration of Fable&\#x27;s interactive generation \(tool-2-1\). No community comments were available on the post.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://artificialanalysis.ai/models/claude-fable-5-2">Claude Fable 5 . 2 (max) - Intelligence, Performance... | Artificial Analysis</a></li>
<li><a href="https://simonwillison.net/2026/Oct/29/how-i-built-the-most-ai-pilled-company-in-the-world/">2026-10-30 — Spawn uses autonomous Fable agents to ship prompt-driven game changes hourly</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Fable`, `#WebGL`, `#simulation`, `#generative AI`

---

<a id="item-twitter-news-3"></a>
### [OpenAI dot Adds Multi-Computer Connection](https://x.com/dotey/status/2119898580131725439) ⭐️ 7.0/10

OpenAI&\#x27;s dot assistant can now connect to multiple personal computers, letting users assign each task to a specific machine. dot is a cloud-resident AI assistant introduced at OpenAI&\#x27;s DevDay in late September, with its own cloud computer and browser, and can be messaged from ChatGPT, Slack, or Teams. Previously, dot could connect to one personal computer to use its files, code, and software. Now it can connect to several, so users can delegate work to a dedicated machine without occupying their current one. Example use cases from OpenAI&\#x27;s developer account include: running an iOS app change test in Xcode on a second Mac and sending a screenshot; reproducing a bug by running the same test on a laptop and a machine with an older SDK to compare results; and clicking through a UI flow on a second computer to record where an error occurs while the user&\#x27;s own screen and mouse remain free. On connected computers, dot creates local Codex or ChatGPT Work tasks and can continue existing Codex tasks. Tasks are managed in the cloud but use the files and tools on the selected computer. Each thread uses only one computer at a time; to have multiple computers work independently, users can start separate threads per computer. Tasks already started do not move when the selected computer changes. The feature is rolling out gradually to ChatGPT Pro tiers and Business Premium users. Pro users must be at least 18; the feature is not available in the European Economic Area, UK, or Switzerland. For Enterprise, Edu, and Healthcare, admins must enable it, and it becomes enabled by default on November 18 unless the organization opts out. Chatting with dot does not consume ChatGPT usage limits, but tasks delegated to Codex or Work count toward those products&\#x27; quotas. To connect a computer, open the ChatGPT app on that device, go to dot&\#x27;s profile page, find the computer under &quot;Computers&quot;, click &quot;Allow&quot;, then &quot;Allow access&quot;. Repeat on each additional computer. Connections remain valid, but the computer must be online and the ChatGPT app open for dot to use it. &quot;Offline&quot; means temporarily unavailable; &quot;Revoke access&quot; fully disconnects. This authorization is separate from connecting the computer to Codex or enabling Work Sync, and enabling those alone does not let dot access the computer. The source also compares dot with Anthropic&\#x27;s Claude Duet and xAI&\#x27;s Grok Bot. Claude Duet, released October 21 as a research preview for US Pro, Max, and Ultra users, has its own cloud VM and browser but the official introduction does not mention connecting the user&\#x27;s own computers; users who want Claude to use local files currently go through Claude Code Projects with Remote Control. Grok Bot is more similar to dot in connecting to local computers: all bots share one cloud computer, and with permission it can execute commands on connected computers, with each computer configured separately and command approval required by default. Grok Bot can also route cloud computer traffic through the user&\#x27;s computer IP to bypass sites that block cloud servers; dot&\#x27;s approach for such sites is to start a separate local task on the connected computer without carrying over the cloud browser login state.

twitter · 宝玉 · Nov 9, 21:03

**「Background」** dot was announced by OpenAI at DevDay in late September as an always-on AI assistant that lives in the cloud, with its own cloud computer and browser, and can keep working even when the user&\#x27;s computer is off. It can be reached via ChatGPT, Slack, and Teams. Initially, dot could connect to one of the user&\#x27;s personal computers to access files, code, and software on that device. The update described here expands that to multiple computers, enabling task delegation to specific machines for testing, bug reproduction, and UI checks. Competing assistants include Anthropic&\#x27;s Claude Duet and xAI&\#x27;s Grok Bot, which take different approaches to local computer access and cloud browsing.

**Tags**: `#OpenAI`, `#AI assistant`, `#multi-device`, `#developer tools`, `#tech news`

---

<a id="item-twitter-news-4"></a>
### [Fable 5.2: +10% Intelligence, +164% Cost](https://x.com/ding_liam/status/2119922378264436741) ⭐️ 6.0/10

A tweet by 丁洪Liam \(@ding\_liam\) states that Fable 5.2 offers a 10% improvement in intelligence at a 164% increase in cost. The post provides only this concise data point without additional explanation or context.

twitter · 丁洪Liam · Nov 9, 22:37

**「Background」** The tweet highlights a key trade-off for Anthropic&\#x27;s Claude Fable 5.2 model: a 10% improvement in intelligence accompanied by a 164% increase in cost. Anthropic officially introduced Claude Fable 5.2 alongside Mythos 5.2, with external safety and capability evaluations by the UK AI Security Institute, Frontier Design, and METR \(tool-1-1\). The model is positioned for complex software engineering, robot control, long-running projects, and coordinating over 1,000 AI agents simultaneously \(tool-1-2\). Official platform documentation lists model IDs, context window, output limits, and pricing, which presumably underpin the cost figures \(tool-1-3\). Earlier Horizon digests note that the Fable model family has already been used in production with significant token costs—Spawn&\#x27;s autonomous game development reportedly spent over $3 million per month using Fable 5 and 5.1 \(tool-2-1\)—and that Fable 5.1 allegedly achieved a perfect score on the Mensa Norway IQ test \(tool-2-3\). No community comments are available on this tweet.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5.2 and Claude Mythos 5.2 \ Anthropic</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-launches-fable-5-2-193609974.html?fr=sycsrp_catchall">Anthropic launches Fable 5.2 and Mythos 5.2 AI models ahead ...</a></li>
<li><a href="https://platform.claude.com/docs/en/models/fable-5-2/overview">Claude Fable 5.2 - Claude Platform Docs</a></li>
<li><a href="https://simonwillison.net/2026/Oct/29/how-i-built-the-most-ai-pilled-company-in-the-world/">2026-10-30 — Spawn uses autonomous Fable agents to ship prompt-driven game changes hourly</a></li>
<li><a href="http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%97%A8%E8%90%A8%E6%99%BA%E5%95%86%E6%B5%8B%E8%AF%95%E8%A2%ABAI%E8%80%83%E7%88%86%E4%BA%86%EF%BC%81151%E6%BB%A1%E5%88%86%E7%99%BB%E9%A1%B6%EF%BC%8C99.97%25%E4%BA%BA%E7%B1%BB%E8%A2%AB%E7%A2%BE%E5%8E%8B">2026-09-27 — Report: AI Scores Perfect 151 on Mensa Norway IQ Test</a></li>

</ul>
</details>

**Tags**: `#AI`, `#model release`, `#cost efficiency`

---

<a id="item-twitter-news-5"></a>
### [Ryan Hoover: AI Agents Can Now Talk to Product Hunt](https://x.com/rrhoover/status/2119889958593036340) ⭐️ 6.0/10

On November 9, 2026, Ryan Hoover, founder of Product Hunt, posted on X: &quot;Rad. Now your agent can talk to Product Hunt.&quot; The announcement indicates that AI agents can now interact with Product Hunt, likely through a new integration or API release. The tweet itself is brief and does not include technical details.

twitter · Ryan Hoover · Nov 9, 20:28

**「Background」** Ryan Hoover, founder of Product Hunt, announced that AI agents can now talk to Product Hunt. Product Hunt is a platform that curates new tech products daily. The announcement indicates an integration or API release enabling AI agents to interact with Product Hunt, though the tweet itself provides no technical details.

<details><summary>References</summary>
<ul>
<li><a href="https://www.producthunt.com/">Product Hunt – The best new products in tech.</a></li>
<li><a href="https://www.youtube.com/watch?v=p9XOLBKayhM">Triangulation 188: Product Hunt Founder Ryan Hoover - YouTube</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Product Hunt`, `#integration`, `#announcement`

---

