---
layout: default
title: "Horizon Summary: 2026-09-27 (EN)"
date: 2026-09-27
lang: en
---

> From 36 items, 15 important content pieces were selected

---

**Technology News**
1. [DeepSeek paper describes DSec elastic compute for massive sandboxes](#item-tech-news-1) ⭐️ 8.0/10
2. [Reladraw: text-based diagramming with user-controlled relative placement](#item-tech-news-2) ⭐️ 7.0/10
3. [SemiAnalysis Publishes Free Intel Panther Lake, 18A Teardown](#item-tech-news-3) ⭐️ 7.0/10
4. [Report: AI Scores Perfect 151 on Mensa Norway IQ Test](#item-tech-news-4) ⭐️ 7.0/10
5. [US appeals court upholds Pentagon blacklisting of Anthropic](#item-tech-news-5) ⭐️ 7.0/10
6. [Excel adds lists and nested arrays, allowing multiple values per cell](#item-tech-news-6) ⭐️ 7.0/10
7. [Conversations Leaves Google Play Over Support Frustrations, Goes Free](#item-tech-news-7) ⭐️ 6.0/10
8. [GDB 18.1 debugger release adds environment, history, and Python changes](#item-tech-news-8) ⭐️ 6.0/10
9. [NumPy MLP with GUI Shows Training Internals in Real Time](#item-tech-news-9) ⭐️ 6.0/10
10. [A Little Guide to Distributed Algorithms Learning for LLM Training and Inference](#item-tech-news-10) ⭐️ 6.0/10
11. [LongCat-2.5-Preview launches two-week free trial on OpenCode](#item-tech-news-11) ⭐️ 6.0/10
12. [OpenAI reportedly expands Ultrafast API access around DevDay](#item-tech-news-12) ⭐️ 6.0/10

**Financial News**
1. [10-year Treasury yield hits 5.23%, its highest since 2007](#item-finance-news-1) ⭐️ 8.0/10
2. [Apple Faces Class Action Over Apple Pay Fees Charged to Card Issuers](#item-finance-news-2) ⭐️ 7.0/10
3. [Users Report Suspected Overseas Fraud on Bank of China Mastercards](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek paper describes DSec elastic compute for massive sandboxes](https://arxiv.org/abs/2609.22978) ⭐️ 8.0/10

DeepSeek has published an arXiv paper describing DSec, an elastic compute system that, according to Hacker News discussion, can run hundreds of thousands of concurrent sandboxes on a compact cluster of 160 AMD Epyc server nodes. The listing presents the system&\#x27;s design as a preprint, so the claims are not independently verified and no shipped implementation is shown. Systems and security researchers evaluating large-scale sandboxing or AI-infrastructure designs are the main audience for the proposal.

hackernews · shenli3514 · Sep 26, 18:22 · [Discussion](https://news.ycombinator.com/item?id=49859112)

**「Background」** DeepSeek Elastic Compute \(DSec\), described in a recent arXiv report, is a production sandbox platform that exposes FnCall, container, microVM, and full-VM backends through a unified SDK. The report argues that agentic training workloads require an elastic execution platform rather than a single sandbox runtime.

**「Impact」** The paper reports that DSec achieves over 380,000 concurrent sandboxes and 3 million sandboxes per day using only 160 Epyc-based server nodes, with a creation rate exceeding 5,000 per second. This demonstrates that large-scale, high-throughput sandboxed execution for agentic reinforcement learning is feasible on a relatively compact cluster, which may influence how other organizations design their AI training infrastructure. The comparison to Google&\#x27;s AX project \(an early, unstable open-source release\) highlights that both organizations are pursuing similar declarative orchestration approaches but with different maturity levels.

**「Community Discussion」** Commenters concentrated on the paper&\#x27;s unusually long author list, with one suggesting that listing many employees may be an asset-protection strategy to make poaching harder, while another wondered how 131 authors coordinated the work. Others compared DSec to Google&\#x27;s AX project and cited the unverified claim of 380,000 concurrent sandboxes on 160 Epyc nodes.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://pandaily.com/deepseek-dsec-elastic-compute-agentic-training-sandbox-3m-day">DeepSeek Details DSec Elastic Compute : Agentic-Training... - Pandaily</a></li>
<li><a href="https://arxiv.org/abs/2609.22978v1">[2609.22978v1] DeepSeek Elastic Compute (DSec): A Sandbox ...</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#elastic-compute`, `#ai-infrastructure`, `#sandboxing`

---

<a id="item-tech-news-2"></a>
### [Reladraw: text-based diagramming with user-controlled relative placement](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw is a new open-source domain-specific language \(DSL\) for diagramming that lets users specify relative positions \(e.g., &quot;left of&quot;, &quot;right of&quot;\) while keeping diagrams text-based, unlike auto-placement tools such as Mermaid or Graphviz. It targets both humans and AI agents, and is available via a web playground, npm install, or as a skill for Claude. The approach bridges the gap between full manual layout and fully automated layout.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**「Background」** Traditional text-based diagramming languages like Mermaid and Graphviz automatically position elements, often producing layouts that users cannot adjust. Manual tools like Draw.io give full control but are slow and difficult for AI agents to manipulate. Reladraw offers a middle ground by allowing relative positioning within a declarative language.

**「Impact」** Developers and AI agents can now produce well-laid-out diagrams without manual tweaking, with the DSL designed to be efficient for AI coding assistants to generate and modify.

**「Community Discussion」** Commenters noted that Reladraw addresses a key bottleneck in AI-assisted development, where visual alignment of mental models with agents is crucial \(apinstein\). One user appreciated that relative positioning is likely sufficient for most flowchart needs \(HeavyStorm\), while another reported a bug where edges did not render curved arrows as expected \(recroad\).

**Tags**: `#diagramming`, `#domain-specific-language`, `#developer-tools`, `#ai-agents`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [SemiAnalysis Publishes Free Intel Panther Lake, 18A Teardown](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 7.0/10

SemiAnalysis published a free STEEL teardown looking inside Intel&\#x27;s 18A process technology and Panther Lake processors. The article is publicly available, but no specific technical findings or measurements are disclosed in the announcement.

rss · Semianalysis · Sep 26, 13:36

**「Background」** Intel 18A is Intel&\#x27;s process node built around RibbonFET gate-all-around transistors and PowerVia backside power delivery \(BSPD\), and Panther Lake is a client chip produced on it. This teardown examines a Core Ultra 7 365 sample, tracing 18A structures and tile-level process choices such as PowerVia routing.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown , 18A, BSPD, GAAFET, SemiAnalysis ...</a></li>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18A teardown : what it found | NeoTeo</a></li>

</ul>
</details>

**Tags**: `#Intel`, `#semiconductors`, `#hardware`, `#process technology`, `#teardown`

---

<a id="item-tech-news-4"></a>
### [Report: AI Scores Perfect 151 on Mensa Norway IQ Test](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%97%A8%E8%90%A8%E6%99%BA%E5%95%86%E6%B5%8B%E8%AF%95%E8%A2%ABAI%E8%80%83%E7%88%86%E4%BA%86%EF%BC%81151%E6%BB%A1%E5%88%86%E7%99%BB%E9%A1%B6%EF%BC%8C99.97%25%E4%BA%BA%E7%B1%BB%E8%A2%AB%E7%A2%BE%E5%8E%8B) ⭐️ 7.0/10

According to a New Intelligence report, Claude Fable 5.1 and the image-answering GPT-6 Astra answered all 35 pattern-reasoning questions on the Mensa Norway IQ test in 25 minutes, reaching the test&\#x27;s theoretical maximum of 151, reportedly in seven consecutive attempts. The article says 151 exceeds the 145 typically treated as the human ceiling and that about 98% of people fall below the 130 Mensa admission threshold. These are unverified media claims: the source provides no test methodology, model configuration, or independent replication, and an IQ-test score is not a direct measure of AI capability.

rss · 新智元 · Sep 26, 08:06

**「Background」** The Mensa Norway IQ test is a 25-minute, 35-item nonverbal test of fluid intelligence built around abstract figural reasoning, with a maximum score of 151 and a Mensa membership threshold near 130. In AI benchmarking, such visual tests are often verbalized into text for language models, while vision models can be given the original images directly, so the same test can be administered in different forms depending on the model being evaluated.

**「Impact」** For AI evaluators, the reported result weakens the assumption that non-knowledge-based &\#x27;fluid intelligence&\#x27; tests remain a human-only strength. However, because the article lacks a controlled protocol and verification, the outcome should be treated as an unverified benchmark claim rather than evidence of general reasoning ability.

<details><summary>References</summary>
<ul>
<li><a href="https://trackingai.org/">IQ Test | Tracking AI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IQ test`, `#Mensa`, `#benchmarking`, `#artificial intelligence`

---

<a id="item-tech-news-5"></a>
### [US appeals court upholds Pentagon blacklisting of Anthropic](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 7.0/10

A U.S. federal appeals court in Washington, D.C., ruled 2-1 on September 25 to uphold the Pentagon&\#x27;s decision to place Anthropic on a national security supply chain blacklist, barring the company from military contracts. The majority judges held that the Pentagon&\#x27;s concerns were reasonable because Anthropic refused to allow its AI to be used in autonomous weapons and mass surveillance. Anthropic said it disagrees with the ruling and is considering asking the full appeals court to review the case. The ruling follows an earlier decision by a San Francisco federal judge that overturned the listing under a separate law and blocked broader government restrictions on the company.

telegram · zaihuapd · Sep 26, 05:19

**「背景」** Anthropic is an AI safety company whose product-use policies prohibit applications such as autonomous weapons and mass surveillance. That policy led the U.S. Department of Defense to place Anthropic on a national-security supply-chain blacklist, barring it from military contracts. In an earlier stage of the dispute, a San Francisco federal judge had struck down the listing under a different law and blocked broader government restrictions, before the D.C. Circuit panel now upheld the Pentagon&\#x27;s action.

**「Impact」** Anthropic remains excluded from U.S. military contracts while it decides whether to pursue further review, so its current operational status under the blacklist is unchanged for now. The company&\#x27;s next concrete step is seeking en banc review by the full appeals court.

**Tags**: `#Anthropic`, `#AI policy`, `#national security`, `#military contracts`, `#regulation`

---

<a id="item-tech-news-6"></a>
### [Excel adds lists and nested arrays, allowing multiple values per cell](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

Microsoft has introduced lists, in-cell arrays, and nested arrays to Excel, making it possible to store multiple values in a single cell for the first time in 40 years. The preview is rolling out to Windows and Mac Beta Channel users, who can enter comma- or semicolon-separated items with Ctrl+J or Insert &gt; List and filter or calculate by individual items. Four new array functions—FLATTEN, HAS, HASANY, and HASALL—accompany the feature. Because this is a preview, behavior may change before release, and Microsoft advises against using it in critical workbooks.

telegram · zaihuapd · Sep 26, 16:26

**「Background」** Throughout Excel&\#x27;s 40-year history, each cell could contain only one value; users had to split related data across separate cells or combine them as text strings. This preview allows multiple values per cell via lists and nested arrays, with four new functions \(FLATTEN, HAS, HASANY, HASALL\) to process them.

**「Impact」** Windows and Mac Beta Channel users can now experiment with multi-value cells, but they should avoid relying on this feature in critical workbooks until it reaches general availability, since Microsoft says the preview behavior may still change.

<details><summary>References</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>

</ul>
</details>

**Tags**: `#Excel`, `#Microsoft 365`, `#spreadsheet`, `#data management`, `#arrays`

---

<a id="item-tech-news-7"></a>
### [Conversations Leaves Google Play Over Support Frustrations, Goes Free](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 6.0/10

The developer of the open-source XMPP client Conversations announced that the app is leaving Google Play, citing poor support and policy frustrations, and is now available for free. The move appears to shift distribution away from the store that previously charged for the app, though the post does not detail a specific replacement store or release process.

hackernews · ezst · Sep 26, 10:55 · [Discussion](https://news.ycombinator.com/item?id=49855315)

**「Background」** Conversations is a free and open-source XMPP instant messaging client for Android, written by Daniel Gultsch and first released in 2014. It was long sold as a paid app on Google Play, although it was also available free through the F-Droid store; Gultsch refrained from advertising the free alternative to steer users to the paid version. Gultsch now says he has left Google Play over support and policy frustrations and made Conversations free.

**「Impact」** Users who relied on Google Play for Conversations will need to install it from another distribution source, and the app is now free rather than paid. Developers evaluating Play as a channel may see this as another example of store policy and support burden affecting independent apps.

**「Community Discussion」** Commenters argued that Google&\#x27;s fee is less objectionable than its poor store support, with one describing a year-long failure to verify a business support phone number and another saying Play has shifted from hosting hobbyist projects to a business-oriented platform increasingly hostile to sideloading. These are commenters&\#x27; opinions and experiences, not confirmed facts about the app&\#x27;s removal.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conversations_%28software%29">Conversations (software) - Wikipedia</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**Tags**: `#android`, `#google play`, `#open source`, `#app distribution`, `#developer experience`

---

<a id="item-tech-news-8"></a>
### [GDB 18.1 debugger release adds environment, history, and Python changes](https://lwn.net/Articles/1096897/) ⭐️ 6.0/10

GDB 18.1, the new version of the interactive debugger, has been released. It adds commands to manipulate the environment of the subprocess, the ability to save command history to a file, support for a couple of new targets, and several Python API additions, with the complete list in the NEWS file.

rss · LWN.net · Sep 26, 15:03

**「Background」** GDB \(the GNU Debugger\) is the standard interactive debugger for many compiled languages, particularly C and C++. This release follows the initial 18.x branch and adds incremental improvements and new features.

**Tags**: `#gdb`, `#debugging`, `#developer-tools`, `#release`, `#python-api`

---

<a id="item-tech-news-9"></a>
### [NumPy MLP with GUI Shows Training Internals in Real Time](https://www.reddit.com/r/MachineLearning/comments/1wqy1qd/p_a_small_mlp_from_scratch_in_numpy_with_a_gui_to/) ⭐️ 6.0/10

The project is an educational implementation of a small multilayer perceptron in plain NumPy, with manual backpropagation, SGD with momentum, L2, dropout, cosine decay, and four activation functions; on the full MNIST training set it reaches about 98.5% accuracy according to the author. Its GUI shows per-batch and per-epoch loss, per-layer gradient norms with inactive-neuron percentages, current-versus-initial weight distributions, and first-layer receptive fields. It also provides layer-by-layer PCA/t-SNE of the test set with wrong-prediction links, robustness curves for noise and rotation, and an interactive lab for ablating, pruning, rescaling, or adding noise to neurons and changing softmax temperature with immediate test-accuracy feedback. The code is available on GitHub and is aimed at students, self-learners, and teachers.

reddit · r/MachineLearning · /u/No-Brain-1655 · Sep 26, 18:38

**「Background」** A multilayer perceptron \(MLP\) is a basic feedforward neural network often taught on MNIST, a dataset of handwritten digits. This project implements the network from scratch in NumPy without autograd, meaning the backward pass is derived manually, making the mechanics of training visible instead of hidden behind a deep-learning framework.

**「Impact」** For ML instructors, the repository offers a framework-free demo that can be run in class or explored individually, letting students directly see how gradient norms, inactive neurons, weight distributions, and neuron ablations change during training and how robustness varies with noise or rotation. Because the accuracy figure is the author&\#x27;s own result set in the GitHub description, users should treat it as a reported outcome rather than an independently benchmarked claim.

**Tags**: `#educational tool`, `#NumPy`, `#MLP`, `#visualization`, `#neural network training`

---

<a id="item-tech-news-10"></a>
### [A Little Guide to Distributed Algorithms Learning for LLM Training and Inference](https://www.reddit.com/r/MachineLearning/comments/1wqk0x2/a_little_guide_to_learning_distributed_algorithms/) ⭐️ 6.0/10

A Reddit user shared a curated guide for learning distributed algorithms used in LLM training and inference, centered on a list of papers the author read over three months and on a GitHub repository named smolcluster with basic reference implementations. The post also links an Alphaxiv shared folder containing the papers. It is a community forum starting point rather than an authoritative technical analysis, and the author says the repository is still being maintained and open to feedback.

reddit · r/MachineLearning · /u/East-Muffin-6472 · Sep 26, 07:10

**「Background」** Distributed LLM training and inference rely on multiple forms of parallelism—commonly data, tensor, pipeline, and model parallelism—so learners typically need both distributed-systems fundamentals and implementation practice before running or optimizing large models. This guide targets that gap by pairing selected papers with reference code.

**「Impact」** For people new to the area, the practical consequence is a concrete, code-backed entry point: read the selected papers and experiment with the provided reference implementations instead of reading broadly across the field.

**Tags**: `#distributed systems`, `#LLM training`, `#LLM inference`, `#distributed parallelism`, `#machine learning education`

---

<a id="item-tech-news-11"></a>
### [LongCat-2.5-Preview launches two-week free trial on OpenCode](https://x.com/Meituan_LongCat/status/2103844449550020816) ⭐️ 6.0/10

Meituan&\#x27;s LongCat account announced on September 26, 2026 that LongCat-2.5-Preview is available for a free two-week trial on OpenCode. The announcement claims support for a 1M-token context, multimodal input, and zero data retention. As of now this is a vendor announcement from a single social media post, with no independent confirmation of availability or measured performance.

telegram · zaihuapd · Sep 27, 01:41

**「Background」** LongCat-2.5-Preview is Meituan&\#x27;s long-context multimodal model, listed on Meituan&\#x27;s LongCat API platform on 25 September 2026 with a 1,000,000-token context window, 131,072-token maximum output, image input, an optional thinking mode, and a $0.006 cached-input rate. OpenCode already tracks the model&\#x27;s usage data, so the announced two-week free trial makes the model available through that platform at no charge.

**「Impact」** Developers on OpenCode can trial LongCat-2.5-Preview free for an announced two-week window, with a 1M-token context, multimodal input, and zero data retention, making it feasible for long-horizon agent workloads. Since reporting differs on whether the free access is time-limited or has no published end date, teams should confirm current availability and retention terms before relying on it.

<details><summary>References</summary>
<ul>
<li><a href="https://ahmetbalaman.com/en/blog/how-to-install-longcat-2-5-preview-en/">How to Install LongCat 2 . 5 Preview (Guide)</a></li>
<li><a href="https://www.orcarouter.ai/blog/longcat-2-5-preview-vs-minimax-m3">LongCat - 2 . 5 - Preview vs MiniMax M3: identical rate cards</a></li>
<li><a href="https://x.com/opencode/status/2103841640171614322">OpenCode on X: &quot;LongCat-2.5-Preview is now free on OpenCode for two weeks - 1M Context - Multi-modal - Zero Data Retention&quot; / X</a></li>
<li><a href="https://huggingnews.com/ai/update-opencode-makes-meituan-16t-parameter-longcat-25-free-for-2-weeks-85004eb5">OpenCode Makes Meituan 1.6T Parameter LongCat 2.5 Free for 2 Weeks | HuggingNews</a></li>
<li><a href="https://www.orcarouter.ai/blog/longcat-2-5-preview-free-opencode">LongCat-2.5-Preview free on OpenCode: 1M tokens, no end date</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#multimodal`, `#long context`, `#Meituan`, `#OpenCode`

---

<a id="item-tech-news-12"></a>
### [OpenAI reportedly expands Ultrafast API access around DevDay](https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/) ⭐️ 6.0/10

According to TestingCatalog, OpenAI plans to broaden access to its Ultrafast API around the September 29 DevDay, expanding the mode beyond its current invite-only customers. The mode, previewed with GPT-5.6 Sol, is reported to reach up to 750 tokens per second and run 14x faster inference than the Standard tier. Developers might then choose Standard, Fast, or Ultrafast in the Playground, although OpenAI has not officially confirmed the rollout and GPT-6 support remains uncertain.

telegram · zaihuapd · Sep 27, 02:06

**「Background」** OpenAI has already officially previewed Ultrafast as a limited invitation-only service tier for GPT-5.6 Sol, with reporting describing claimed speeds of up to 750 output tokens per second and up to 14× faster inference than the Standard tier, a comparison based on GPT-5.6 Sol processing on GPU clusters. The current report concerns a planned wider rollout of that preview around OpenAI&\#x27;s September 29 DevDay.

**「Impact」** Developers building on GPT-5.6 Sol should not assume Ultrafast throughput is generally available until OpenAI confirms the expanded rollout, and those planning around GPT-6 should treat Ultrafast support as unverified.

<details><summary>References</summary>
<ul>
<li><a href="https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/">OpenAI prepares to expand Ultrafast API to more users</a></li>
<li><a href="https://www.orcarouter.ai/blog/gpt-5-6-sol-ultrafast-vs-gpt-5-6-sol">GPT-5.6 Sol Ultrafast vs Sol: same model, one missing price</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#API`, `#performance`, `#GPT`, `#AI infrastructure`

---

## Financial News

<a id="item-finance-news-1"></a>
### [10-year Treasury yield hits 5.23%, its highest since 2007](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 8.0/10

The 10-year Treasury yield—the interest rate on US government bonds that influences mortgages—climbed to 5.23% on Friday, its highest since 2007, reflecting sticky inflation, expectations of more Federal Reserve rate hikes, and heavy bond issuance from government deficits and AI-related corporate borrowing.

rss · CNBC Finance · Sep 26, 13:30

**「Background」** The yield was just below 4.8% earlier this month; bond prices move inversely to yields, and traders now price a 64% chance of an October Fed rate hike, according to the CME FedWatch tool, as one-year consumer inflation expectations rose to 4.6% in September from 4% in August.

**「Impact」** Higher yields raise borrowing costs for households and companies and can drag on stocks by making bonds more attractive to income-seeking investors.

**Tags**: `#Treasury yields`, `#Federal Reserve`, `#bond issuance`, `#inflation`, `#AI investment`

---

<a id="item-finance-news-2"></a>
### [Apple Faces Class Action Over Apple Pay Fees Charged to Card Issuers](https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/) ⭐️ 7.0/10

A U.S. federal judge certified an antitrust class action accusing Apple of overcharging payment card issuers for Apple Pay transactions. The lawsuit alleges Apple charges 0.15% on credit card payments and half a cent per debit transaction, taking up to $1 billion a year, and the plaintiffs are seeking refunds and an injunction.

telegram · zaihuapd · Sep 26, 03:32

**「Background」** Apple Pay is Apple&\#x27;s mobile wallet service that lets iPhone users pay by tapping their devices; card issuers pay Apple a fee for each Apple Pay transaction, and Apple controls the iPhone&\#x27;s tap-to-pay technology, which plaintiffs say blocks rival wallets. In September 2026, U.S. District Judge Jeffrey White certified a class of U.S. card issuers in the antitrust lawsuit, allowing them to proceed together against Apple.

<details><summary>References</summary>
<ul>
<li><a href="https://macdailynews.com/2026/09/25/federal-judge-certifies-class-in-apple-pay-fee-antitrust-case-brought-by-credit-union/">Federal judge certifies class in Apple Pay fee antitrust case brought...</a></li>
<li><a href="https://www.macrumors.com/2026/09/25/apple-pay-antitrust-lawsuit-advances/">Banks and Credit Unions to Team Up Against Apple Pay Fees</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Apple Pay`, `#antitrust`, `#class action`, `#payment fees`

---

<a id="item-finance-news-3"></a>
### [Users Report Suspected Overseas Fraud on Bank of China Mastercards](https://finance.sina.com.cn/jryx/2026-09-26/doc-initcyza0450311.shtml) ⭐️ 7.0/10

On Sept. 26, multiple users said on social media that their Bank of China Mastercards were apparently involved in large-scale overseas fraud, with one reporting an overnight Apple Pay card-lock notice and a Brazilian charge despite never carrying the physical card; users said they were locking their cards. The reports say affected cards were mostly British pound cards, with some dollar cards also involved.

telegram · zaihuapd · Sep 26, 12:27

**「Background」** The suspected cause is problems in the issuing bank&\#x27;s card-issuing logic and network authentication; last September, SPD Bank Mastercard users reported a similar incident that also involved Apple Pay-bound cards and Brazilian/Latin American currency.

**Tags**: `#Bank of China`, `#Mastercard fraud`, `#cybersecurity`, `#card security`, `#China`

---