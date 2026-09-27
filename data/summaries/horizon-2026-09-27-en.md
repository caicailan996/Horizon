# Horizon Daily - 2026-09-27

> From 38 items, 13 important content pieces were selected

---

**Technology News**
1. [US Appeals Court Upholds Pentagon Blacklist of Anthropic](#item-tech-news-1) ⭐️ 8.0/10
2. [SemiAnalysis STEEL Teardown of Intel Panther Lake and 18A](#item-tech-news-2) ⭐️ 7.0/10
3. [Interactive MLP visualization tool in NumPy with manual backprop and ablation lab](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek Elastic Compute paper: large author list, claimed sandbox scale](#item-tech-news-4) ⭐️ 6.0/10
5. [Reladraw: a text-based diagram DSL with explicit layout control](#item-tech-news-5) ⭐️ 6.0/10
6. [Conversations Goes Free as Its Developer Leaves Google Play](#item-tech-news-6) ⭐️ 6.0/10
7. [GDB 18.1 released with subprocess environment commands and Python API additions](#item-tech-news-7) ⭐️ 6.0/10
8. [Decompose, Look, Reason: Reinforced latent-space reasoning for VLMs at EMNLP &\#x27;26](#item-tech-news-8) ⭐️ 6.0/10
9. [Excel Now Allows Multiple Values in a Single Cell with Lists and Arrays](#item-tech-news-9) ⭐️ 6.0/10
10. [LongCat-2.5-Preview Free for Two Weeks on OpenCode](#item-tech-news-10) ⭐️ 6.0/10

**Financial News**
1. [10-Year Treasury Yield Hits 19-Year High of 5.23% on Inflation and Bond Issuance](#item-finance-news-1) ⭐️ 9.0/10
2. [Apple Faces Class Action Over Apple Pay Card-Issuer Fees](#item-finance-news-2) ⭐️ 7.0/10
3. [Hong Kong Regulator Reaches HK$1 Billion Settlement with PwC Over Evergrande Audit](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [US Appeals Court Upholds Pentagon Blacklist of Anthropic](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 8.0/10

On September 25, the U.S. Court of Appeals for the D.C. Circuit ruled 2-1 to uphold the Pentagon&\#x27;s decision to list Anthropic as a national security supply chain risk, barring the company from military contracts. The majority found the Pentagon&\#x27;s concern reasonable because Anthropic refused to allow its AI products to be used in autonomous weapons and mass surveillance. Anthropic said it disagrees with the ruling and is considering asking the full appeals court to review the case. The decision reverses earlier progress for Anthropic, when a San Francisco federal judge had struck down the listing under a different law and blocked broader government restrictions.

telegram · zaihuapd · Sep 26, 05:19

**「Background」** The Pentagon placed Anthropic on its National Security Supply Chain risk list in 2025, barring the company from military contracts over its refusal to permit AI use in autonomous weapons and mass surveillance. A San Francisco federal judge later overturned that listing under a different legal statute, but the Washington D.C. appeals court has now reversed that decision, upholding the Pentagon&\#x27;s original determination.

**「Impact」** The ruling keeps Anthropic excluded from U.S. military procurement despite its ethical restrictions on weapons and surveillance use, and signals that courts may defer to the Pentagon&\#x27;s national security risk determinations. Anthropic&\#x27;s next practical step is to seek en banc review by the full D.C. Circuit or adjust its usage policies to restore eligibility for defense contracts.

**Tags**: `#AI regulation`, `#national security`, `#Anthropic`, `#autonomous weapons`, `#supply chain risk`

---

<a id="item-tech-news-2"></a>
### [SemiAnalysis STEEL Teardown of Intel Panther Lake and 18A](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 7.0/10

A free SemiAnalysis STEEL teardown of Intel&\#x27;s Panther Lake processor and Intel 18A process node was published on September 26, 2026, authored by Adith Shankar. The piece is presented as an examination of the chip and process, rather than an announced plan, but the supplied content does not include specific findings, measurements, or comparisons.

rss · Semianalysis · Sep 26, 13:36

**「Background」** Intel 18A is Intel&\#x27;s next-generation process node, and Panther Lake is the first client processor line built on it. Intel had slated Panther Lake for a late 2025 launch while partners tested early samples; this teardown examines a Core Ultra 7 365 sample to map the 18A structures, PowerVia routing, and tile-level process choices.

**「Impact」** For semiconductor engineers and industry watchers, the SemiAnalysis teardown provides an early independent physical examination of Intel&\#x27;s 18A process in Panther Lake, the first client SoC built on that node, making it possible to test Intel&\#x27;s process and performance claims ahead of the chip&\#x27;s broader launch. The findings are especially relevant to those evaluating Panther Lake&\#x27;s AI-oriented performance and the Cougar Cove and Darkmont core architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18 A teardown : what it found | NeoTeo</a></li>
<li><a href="https://wccftech.com/intels-18a-process-shows-great-performance-as-panther-lake-socs-are-finally-up/">Intel &#x27;s 18 A Process Shows &quot;Great Performance&quot; As Initial Panther ....</a></li>
<li><a href="https://www.linkedin.com/posts/enigma-security_intel-pantherlake-pctechnology-activity-7382348178563473408-WJUJ"># intel # pantherlake #pctechnology #advancedchips #aiinhardware...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown, 18 A , BSPD, GAAFET, SemiAnalysis...</a></li>
<li><a href="https://www.linkedin.com/posts/nqobile-predict-maseko-78bbb0249_intel-pantherlake-ai-activity-7382096572819496960-1St8">Intel Unveils Panther Lake : AI PC Platform on 18 A Node | LinkedIn</a></li>
<li><a href="https://wccftech.com/intel-panther-lake-confirmed-to-feature-cougar-cove-darkmont/">Intel &#x27;s Panther Lake SoCs Confirmed To Feature Cougar Cove...</a></li>

</ul>
</details>

**Tags**: `#Intel`, `#Panther Lake`, `#Intel 18A`, `#semiconductor`, `#chip teardown`

---

<a id="item-tech-news-3"></a>
### [Interactive MLP visualization tool in NumPy with manual backprop and ablation lab](https://www.reddit.com/r/MachineLearning/comments/1wqy1qd/p_a_small_mlp_from_scratch_in_numpy_with_a_gui_to/) ⭐️ 7.0/10

An educational tool trains a small MLP on MNIST using only NumPy with manual backpropagation, SGD with momentum, dropout, and cosine decay, achieving ~98.5% accuracy. It visualizes weight distributions, gradient norms, PCA/t-SNE per layer, robustness curves, and allows real-time neuron ablation, pruning, and noise injection. The tool is aimed at students from high school to intro ML courses and self-learners, and is available on GitHub.

reddit · r/MachineLearning · /u/No-Brain-1655 · Sep 26, 18:38

**「Background」** A multilayer perceptron \(MLP\) is a type of feedforward neural network. This tool implements the full training loop from scratch without autograd, making the internal mechanics transparent for learners.

**「Impact」** Students and teachers can interactively observe how weight distributions evolve, which neurons are inactive, and how ablating a single neuron affects test accuracy, providing hands-on insight beyond textbook diagrams.

**Tags**: `#machine learning`, `#educational tool`, `#visualization`, `#neural networks`, `#NumPy`

---

<a id="item-tech-news-4"></a>
### [DeepSeek Elastic Compute paper: large author list, claimed sandbox scale](https://arxiv.org/abs/2609.22978) ⭐️ 6.0/10

DeepSeek has posted a paper titled &quot;DeepSeek Elastic Compute \(DSec\)&quot; to arXiv, describing the company&\#x27;s elastic compute infrastructure. The item itself supplies little technical detail, but commenters cite the work as running 380,000 concurrent sandboxes across 160 AMD Epyc-based server nodes and note the paper lists a very large author count, with one commenter saying 131 authors and 31 additional names not shown on the page.

hackernews · shenli3514 · Sep 26, 18:22 · [Discussion](https://news.ycombinator.com/item?id=49859112)

**「Background」** DeepSeek Elastic Compute \(DSec\) is a production sandbox platform designed for training agentic AI models that require execution in isolated environments. It exposes multiple sandbox backends—FnCall, container, microVM, and full-VM—through a unified SDK. According to the paper, a single production-scale unit spans around 160 nodes, supporting over 380,000 concurrent sandboxes and serving roughly 3 million sandboxes per day.

**「Community discussion」** Commenters highlighted the claimed scale and the unusual author list, with some speculating that listing every employee on papers is an asset-protection strategy so competitors cannot tell whom to recruit. Others questioned how so many authors coordinated and asked whether the work is a kind of agent substrate; these remain commenter opinions, not established facts.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>

</ul>
</details>

**Tags**: `#elastic-compute`, `#deepseek`, `#ai-infrastructure`, `#distributed-systems`, `#machine-learning`

---

<a id="item-tech-news-5"></a>
### [Reladraw: a text-based diagram DSL with explicit layout control](https://github.com/reladraw/reladraw) ⭐️ 6.0/10

Reladraw is a new open-source diagramming language that lets users specify relative positions \(e.g., &quot;left of&quot;, &quot;right of&quot;\) in a text file, combining the reproducibility of auto-layout DSLs like Mermaid with the layout control of manual tools like Draw.io. It is available today as a GitHub repository with an online playground, an npm package, and a Claude agent skill. The project aims to work well for both humans and AI agents, but early users report rough edges such as missing curved arrow support.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**「Background」** Text-based diagram languages such as Mermaid and Graphviz automatically determine element positions from a high-level description, which can produce layouts that do not match the author&\#x27;s intent. Manual diagram tools like Draw.io give full control but are time-consuming to edit and difficult for AI agents to modify programmatically. Reladraw attempts to occupy the middle ground by offering a declarative language that preserves placement directives.

**「Impact」** Developers and teams who rely on text-based diagrams for documentation, architecture reviews, or AI-assisted planning now have an option that retains layout control without abandoning a text workflow. Because the language is still early and has acknowledged bugs \(e.g., missing curved arrows\), users should expect to encounter incomplete features and should verify output for production use.

**「Community Discussion」** Several commenters expressed enthusiasm for a diagramming tool that balances simplicity and layout control, especially for AI agent integration and C4-model diagrams. One user reported that the language failed to produce a curved arrow when the source and target positions were specified explicitly, indicating that the implementation is not yet fully robust.

**Tags**: `#diagramming`, `#DSL`, `#developer tools`, `#AI agents`, `#open source`

---

<a id="item-tech-news-6"></a>
### [Conversations Goes Free as Its Developer Leaves Google Play](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 6.0/10

According to a September 26, 2026 post by the developer, the open-source Android app Conversations is now free and is being separated from Google Play, with the post explaining the reasoning behind leaving the store. The announced change means users who previously obtained the app through Google Play will need to use another distribution channel, and the decision is presented as a response to Play Store fees and support rather than a technical update.

hackernews · ezst · Sep 26, 10:55 · [Discussion](https://news.ycombinator.com/item?id=49855315)

**「Background」** Conversations, an open-source XMPP messaging app for Android, was previously sold as a paid app on Google Play even though free builds were also available on F-Droid; according to the developer, he initially did not advertise the free option and only began linking to F-Droid as his relationship with Google worsened, making F-Droid the app&\#x27;s primary distribution route. Horizon&\#x27;s September 25 digest reported the release of F-Droid 2.0, the alternative store&\#x27;s largest client update in a decade, which shipped with a rewritten interface around the same time as this announcement.

**「Impact」** Existing users should expect Conversations to be distributed outside Google Play from now on; anyone relying on Play Store installations will need to obtain the app through an alternative source such as the developer&\#x27;s site or F-Droid to continue receiving updates. This is the developer&\#x27;s stated intention from the post, not an independently observed listing change.

**「Community discussion」** Commenters largely frame the issue as poor Play Store support rather than the fee, with pi-victor arguing Google&\#x27;s 15% cut would be acceptable if reviews and support were good. k1w1 reports being unable to list a product for a year because Google&\#x27;s phone verification rejects IVR numbers, and 999900000999 describes Play as having shifted from hobbyist-friendly uploads to a business platform that discourages sideloading.

<details><summary>References</summary>
<ul>
<li><a href="https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html">2026-09-25 — F-Droid 2.0 launches Android app store overhaul and new UI</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**Tags**: `#Android`, `#Google Play`, `#open source`, `#app distribution`, `#developer experience`

---

<a id="item-tech-news-7"></a>
### [GDB 18.1 released with subprocess environment commands and Python API additions](https://lwn.net/Articles/1096897/) ⭐️ 6.0/10

GDB 18.1, the latest minor release of the GNU interactive debugger, is now available. It adds commands to manipulate the environment of the debugged subprocess, the ability to save command history to a file, support for several new targets, and Python API additions. The full change list is in the project&\#x27;s NEWS file.

rss · LWN.net · Sep 26, 15:03

**「Background」** GDB is the GNU Project&\#x27;s interactive debugger, commonly used to run programs under controlled conditions and inspect their behavior. Version 18.1 is an incremental update to that debugger, with the NEWS file serving as the authoritative list of new commands and features.

**Tags**: `#gdb`, `#debugger`, `#open-source`, `#software-development`, `#gnu`

---

<a id="item-tech-news-8"></a>
### [Decompose, Look, Reason: Reinforced latent-space reasoning for VLMs at EMNLP &\#x27;26](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E9%9D%A2%E5%90%91%E8%A7%86%E8%A7%89%E8%AF%AD%E8%A8%80%E6%A8%A1%E5%9E%8B%E7%9A%84%E5%BC%BA%E5%8C%96%E9%9A%90%E7%A9%BA%E9%97%B4%E6%8E%A8%E7%90%86%EF%BC%9A%E5%85%88%E5%88%86%E8%A7%A3%E3%80%81%E7%9C%8B%EF%BC%8C%E5%86%8D%E6%8E%A8%E7%90%86%7CEMNLP%2726) ⭐️ 6.0/10

Researchers at Emory University introduced Decompose, Look, and Reason \(DLR\), a reinforced latent-space reasoning approach for vision-language models, accepted at the EMNLP 2026 Main Conference. DLR targets the problem that multimodal chain-of-thought often drifts toward long text reasoning while visual evidence fades, by repeatedly decomposing the question, looking at the image for the current subproblem, and reasoning from that visual evidence. The authors position it against three prior lines of work—text-only multimodal CoT, interleaved CoT with image patches or tools, and latent visual reasoning with local ROIs or single visual injection—and argue DLR can support evidence needed at different stages of a reasoning trajectory. The paper is available on arXiv \(2604.07518\); the announcement does not report benchmark results.

rss · 新智元 · Sep 26, 14:00

**「Background」** Vision-language models can produce long reasoning chains, but multimodal reasoning requires repeated interaction between discrete language tokens and high-dimensional continuous visual representations. Existing approaches either compress visual information into text and lose detail, interleave explicit image evidence such as patches, boxes, crops, or zoom at extra tool cost, or project visual information into latent space but often only inject it once or rely on local ROIs that do not match the semantics needed at a given reasoning step.

**「Impact」** For researchers building long-horizon multimodal reasoning systems, DLR offers a latent-space alternative that avoids repeated external tool calls while keeping visual evidence available throughout the chain; because the source provides no evaluation numbers, any claimed gains should be checked against the full paper.

**Tags**: `#vision-language models`, `#reinforcement learning`, `#latent space reasoning`, `#EMNLP`, `#AI research`

---

<a id="item-tech-news-9"></a>
### [Excel Now Allows Multiple Values in a Single Cell with Lists and Arrays](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 6.0/10

Microsoft has previewed support for storing multiple values in a single Excel cell using lists, cell-internal arrays, and nested arrays, rolling out first to Windows and Mac Beta Channel users. This is the first time in Excel&\#x27;s 40-year history that a cell can hold more than one value, with entries separated by commas or semicolons via Ctrl+J or Insert &gt; List, and each item can be individually filtered and calculated. Four new functions—FLATTEN, HAS, HASANY, and HASALL—are also introduced for array handling. All features are preview capabilities subject to change before general availability, and Microsoft advises against using them in critical workbooks.

telegram · zaihuapd · Sep 26, 16:26

**「Background」** Traditionally, each Excel cell stores exactly one data point \(e.g., a single number or text string\), and operations like filtering and calculation treat the entire cell content as a single unit. This preview introduces a fundamental change to that model by allowing a cell to contain a list of independently accessible values, enabling new data organization patterns within the existing grid interface.

**「Impact」** Because the feature is in preview and its behavior may change, users should avoid relying on it for important workbooks until it reaches general availability. Beta Channel subscribers on Windows and Mac can test the new functionality, but compatibility with older Excel versions and file formats is not yet guaranteed.

**Tags**: `#Excel`, `#Microsoft 365`, `#spreadsheet`, `#arrays`, `#productivity tools`

---

<a id="item-tech-news-10"></a>
### [LongCat-2.5-Preview Free for Two Weeks on OpenCode](https://x.com/Meituan_LongCat/status/2103844449550020816) ⭐️ 6.0/10

Meituan made LongCat-2.5-Preview available for a two-week free trial on OpenCode starting September 26, 2026. The preview model supports a 1M-token context, multimodal input, and zero data retention, according to the announcement. The offer covers the preview release only, and the announcement does not specify pricing or availability after the trial window.

telegram · zaihuapd · Sep 27, 01:41

**「Background」** LongCat is a series of multimodal AI models developed by Meituan. OpenCode is a platform that hosts AI models for free trials and deployment.

**「Impact」** Developers using OpenCode can test the 1M-context multimodal preview at no cost within the two-week window; after that, access terms are not stated in the announcement.

**Tags**: `#AI`, `#Large Language Model`, `#Multimodal`, `#OpenCode`, `#Model Preview`

---

## Financial News

<a id="item-finance-news-1"></a>
### [10-Year Treasury Yield Hits 19-Year High of 5.23% on Inflation and Bond Issuance](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 9.0/10

The 10-year Treasury yield, which influences mortgages, rose to 5.23% on September 26, 2026, its highest level since 2007, as investors priced in higher inflation and a possible Federal Reserve rate hike in October.

rss · CNBC Finance · Sep 26, 13:30

**「Background」** Yields move opposite to bond prices. The jump reflects both stubborn inflation—year-ahead expectations hit 4.6%—and a surge in bond issuance by the government and companies borrowing to fund AI infrastructure, which Vanguard says could reach $300–570 billion this year.

**「Impact」** Higher yields can weigh on company profits and stocks by raising borrowing costs, and they make bonds more attractive to income investors, potentially pulling money from equities.

**Tags**: `#Treasury yields`, `#Federal Reserve`, `#Inflation`, `#Bond issuance`, `#AI investment`

---

<a id="item-finance-news-2"></a>
### [Apple Faces Class Action Over Apple Pay Card-Issuer Fees](https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/) ⭐️ 7.0/10

A U.S. federal judge has certified a class action lawsuit alleging Apple charges payment card issuers anticompetitive fees for Apple Pay transactions: 0.15% on credit cards and $0.005 on debit cards. The plaintiffs, who seek refunds and an injunction, claim Apple collects up to $1 billion a year and blocks rivals from making competing mobile wallets.

telegram · zaihuapd · Sep 26, 03:32

**「Background」** Apple Pay is Apple&\#x27;s mobile wallet service, and card issuers are the banks and credit unions that provide the payment cards added to it. The lawsuit says Android phone wallets do not charge issuers these fees, which is the basis of the antitrust claim.

**「Impact」** The certified class covers U.S. institutions that issue Apple Pay-compatible cards and paid the fees, meaning those issuers could recover past fees if the plaintiffs win the case.

**Tags**: `#Apple`, `#Apple Pay`, `#class action`, `#antitrust`, `#mobile payments`

---

<a id="item-finance-news-3"></a>
### [Hong Kong Regulator Reaches HK$1 Billion Settlement with PwC Over Evergrande Audit](https://wallstreetcn.com/articles/3782573) ⭐️ 7.0/10

Hong Kong&\#x27;s securities regulator settled with PwC Hong Kong for HK$1 billion over audit failures at property developer Evergrande. PwC did not admit liability but agreed to pay that amount to compensate independent small shareholders, though the settlement is being challenged in court by Evergrande&\#x27;s liquidators.

telegram · zaihuapd · Sep 26, 07:18

**「Background」** Evergrande, once one of China&\#x27;s largest property developers, collapsed under massive debt and is now being wound up. Regulators said its financial statements contained false information, and Hong Kong&\#x27;s securities regulator investigated PwC Hong Kong, which had audited those statements; in April 2026, PwC Hong Kong agreed to set aside HK$1 billion to compensate certain minority shareholders.

**「Impact」** If approved, the settlement would provide direct compensation to small retail investors hit by Evergrande&\#x27;s collapse, but the court challenge introduces uncertainty and could delay or alter any payout.

<details><summary>References</summary>
<ul>
<li><a href="https://eu.36kr.com/zh/p/3780065714148610">8点1氪： 华 谊兄弟被申请破产重整， 普 华 永 道 因 恒 大 审 计 赔偿 10 ...</a></li>
<li><a href="https://news.qq.com/rain/a/20260424A01VGD00">普 华 永 道 将支付 10 ...</a></li>

</ul>
</details>

**Tags**: `#香港证监会`, `#普华永道`, `#恒大`, `#审计监管`, `#和解`

---

