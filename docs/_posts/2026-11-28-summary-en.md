---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 66 items, 19 important content pieces were selected

---

**Technology News**
1. [SemiAnalysis Analyzes Trainium3 Inference, Claims Better TCO Than GB300](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenSec discloses 9.8-severity pre-auth nfsd heap overflow in Linux kernel](#item-tech-news-2) ⭐️ 8.0/10
3. [States sue SpaceX to stop Grok from generating child sex images, revenge porn](#item-tech-news-3) ⭐️ 7.0/10
4. [Daniel J. Bernstein examines false computer-checked proofs](#item-tech-news-4) ⭐️ 7.0/10
5. [Essay argues for a formally verifiable mainstream programming language](#item-tech-news-5) ⭐️ 7.0/10
6. [Anthropic system card describes covert limits on frontier-model R&amp;D requests](#item-tech-news-6) ⭐️ 7.0/10
7. [Minecraft Bedrock resource-pack flaw fixed in 26.65 after hidden-script exploits](#item-tech-news-7) ⭐️ 7.0/10
8. [Credit-card skimming scripts using WebRTC found on shopping sites](#item-tech-news-8) ⭐️ 6.0/10
9. [Convex coding skill accused of uploading app ideas without disclosure](#item-tech-news-9) ⭐️ 6.0/10
10. [Michael Nielsen&\#x27;s Neural Networks and Deep Learning book taken down](#item-tech-news-10) ⭐️ 6.0/10
11. [Report: Anthropic study finds unlearning hides, not deletes, dangerous knowledge](#item-tech-news-11) ⭐️ 6.0/10
12. [Google Play to publish merchant developer phone and address from 2027](#item-tech-news-12) ⭐️ 6.0/10
13. [Report: AI Tool Artex Used in Attacks on U.S. Intelligence Agencies](#item-tech-news-13) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache nightly-xpu Release](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](#item-ai-projects-2) ⭐️ 5.0/10
3. [LMCache nightly RBLN wheel for Rebellions NPUs](#item-ai-projects-3) ⭐️ 5.0/10

**Financial News**
1. [China&\#x27;s State Council pledges stronger &\#x27;national team&\#x27; market support](#item-finance-news-1) ⭐️ 8.0/10
2. [China&\#x27;s Central Bank Cuts Large-Deposit Minimum to 100,000 Yuan](#item-finance-news-2) ⭐️ 7.0/10

**Twitter News**
1. [Paul Graham: Startup &\#x27;Partnerships&\#x27; Are Usually a Waste of Time](#item-twitter-news-1) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SemiAnalysis Analyzes Trainium3 Inference, Claims Better TCO Than GB300](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 8.0/10

SemiAnalysis published a technical analysis of AWS Trainium3 focused on inference performance and microarchitecture, claiming better performance TCO than NVIDIA&\#x27;s GB300. The piece describes a first-principles, physics-based architecture review and cites high MFU and MBU, a benchmark called UBenchX, and low-latency results. The supplied excerpt does not include the underlying measurements, workload configurations, or pricing assumptions needed to verify those comparisons, so the TCO and efficiency claims should be treated as analysis claims rather than independently confirmed benchmarks.

rss · Semianalysis · Nov 27, 15:54

**「Earlier Trainium software work」** SemiAnalysis has been tracking how far Trainium&\#x27;s software stack has come: Horizon&\#x27;s October 24 digest relayed its assessment that native PyTorch support, TorchTitan integration and better tooling made Trainium practical for training and not just inference. Horizon&\#x27;s November 5 digest then covered an open-source engine that fused layers into NKI megakernels on a single trn2.48xlarge, cutting a batch-8 decode step from 32.2 ms to 24.2 ms, which illustrated how much Trainium inference latency depends on kernel-level tuning rather than silicon alone.

**「Benchmark before switching」** The reported advantage is workload-dependent: a secondary summary of the analysis states that Trainium3&\#x27;s matrix-multiply MFU beat NVIDIA GB300 at medium scales \(above 1 GFLOP\) but trailed above 100 GFLOP, regaining the lead above 1 TFLOP. Teams weighing a switch should therefore benchmark their own shapes and batch sizes rather than treat the TCO headline as a purchasing decision. SemiAnalysis&\#x27;s InferenceX comparisons also plot tokens per dollar against a P90 interactivity target, so a cost comparison that ignores latency requirements can overstate the savings.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/amazons-trainium-takes-a-strike-at">2026-10-24 — Amazon Trainium Takes on GPU Training With Native PyTorch Support</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xo0yuq/p_nki_layer_megakernels_for_glm53flash_on_aws/">2026-11-05 — NKI Megakernels Cut GLM-5.3-Flash Decode Latency on Trainium2</a></li>
<li><a href="https://inferencex.semianalysis.com/blog/vera-rubin-nvl72-agentic-inference">Rubin NVL72 Agentic Inference : 67x better Performance... | InferenceX</a></li>
<li><a href="https://disconfirmai.com/en/reading/semianalysis-trainium-s-shift-native-pytorch-training-1tp5">SemiAnalysis : Trainium &#x27;s Shift to Native PyTorch... | DisconfirmAI</a></li>

</ul>
</details>

**Tags**: `#AWS Trainium`, `#AI inference`, `#accelerator architecture`, `#performance TCO`, `#semiconductor analysis`

---

<a id="item-tech-news-2"></a>
### [OpenSec discloses 9.8-severity pre-auth nfsd heap overflow in Linux kernel](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 8.0/10

OpenSec disclosed CVE-2026-99362, a CVSS 9.8 pre-authentication heap overflow in the Linux kernel&\#x27;s nfsd server that allows an unauthenticated attacker to trigger an out-of-bounds kernel heap write with a single connection to tcp/2049 and obtain a root shell. The flaw has existed since Linux 3.16 \(2014\) and affects hosts with NFSv4.1 or 4.2 enabled, including file servers, NAS devices and cluster storage nodes. Fixes shipped in kernels 6.12.117, 6.18.61, 7.3.2 and 7.4-rc1; applying them requires a kernel upgrade and reboot, and systems that cannot be updated immediately must restrict access to tcp/2049 at the firewall. The CVE was published on 20 November 2026, and the disclosure currently circulating is a short advisory relayed through a Telegram aggregator, so technical specifics should be confirmed against OpenSec&\#x27;s original write-up.

telegram · zaihuapd · Nov 27, 12:57

**「Background」** The flaw is in nfsd&\#x27;s handling of NFSv4 SEQUENCE replies: the CVE description says an out-of-bounds write occurs there, and a Debian tracker entry says 4\_sequence\(\) narrows the reply buffer to the session&\#x27;s cached reply limit before it accepts the slot seqid. That write is the defect tracked as CVE-2026-99362.

**「Operational impact」** Administrators running NFSv4.1 or 4.2 servers must upgrade to kernel 6.12.117, 6.18.61, 7.3.2, or 7.4-rc1 and reboot. If an immediate upgrade is not possible, the practical mitigation is to stop and disable the NFS server service or restrict TCP port 2049 to trusted hosts, because any unauthenticated attacker who can reach that port can exploit the heap overflow.

<details><summary>References</summary>
<ul>
<li><a href="https://dbu.gs/vulnerability/PT-2026-151543">CVE - 2026 - 99362 — Vulnerability in Linux Kernel | dbugs</a></li>
<li><a href="https://security-tracker.debian.org/tracker/CVE-2026-99362">CVE - 2026 - 99362</a></li>
<li><a href="https://access.redhat.com/security/cve/cve-2026-99362">CVE-2026-99362 - Red Hat Customer Portal</a></li>
<li><a href="https://cybersecuritynews.com/nfs2root-linux-vulnerability/">12-Year-Old NFS2ROOT Linux Flaw Could Let Hackers Take Full ...</a></li>

</ul>
</details>

**Tags**: `#Linux kernel`, `#NFS`, `#vulnerability`, `#CVE`, `#security`

---

<a id="item-tech-news-3"></a>
### [States sue SpaceX to stop Grok from generating child sex images, revenge porn](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

State attorneys general have sued SpaceX over xAI&\#x27;s Grok allegedly generating child sexual abuse material and non-consensual intimate images, raising major AI safety and platform-liability questions.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**Tags**: `#AI safety`, `#generative AI`, `#content moderation`, `#legal/regulation`, `#Grok/xAI`

---

<a id="item-tech-news-4"></a>
### [Daniel J. Bernstein examines false computer-checked proofs](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

Daniel J. Bernstein&\#x27;s analysis examines soundness bugs that let proof checkers accept false proofs, a failure mode relevant to formal verification and high-assurance software. The Hacker News discussion disputes how much practical risk single-checker failures represent: commenters argue that Lean&\#x27;s community tracks soundness bugs and that Metamath&\#x27;s set.mm and iset.mm databases require proofs to pass five independently written verifiers in five languages. One commenter also cited a DeepMind researcher&\#x27;s &quot;proof&quot; that passed Lean and a then-week-old version of nanoda, saying it exploited a different bug. The thread cautions that a false proof would still need to survive informal review and every checker in a pipeline.

hackernews · \_tk\_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**「Why checker soundness matters」** Computer-checked proofs rest on a small trusted kernel that validates each step against the system&\#x27;s axioms and inference rules; soundness is the guarantee that the kernel accepts a proof only when the claimed theorem is actually true. A soundness bug breaks that guarantee, so a proof can pass the checker even though the statement it certifies is false. Because the kernel is the sole arbiter of correctness, its reliability carries the weight that informal peer review carries in ordinary mathematics.

**「Impact」** Developers who depend on proof assistants for high-assurance work should not treat one checker&\#x27;s acceptance as final; the Metamath example shows a multi-verifier pipeline can reduce dependence on any single implementation.

**「Community discussion」** Commenters pushed back on the page&\#x27;s framing, arguing that a single failed checker is a long way from misleading mathematicians because Lean has multiple checkers and Metamath&\#x27;s main databases require five independent verifiers. Others said the known soundness bugs are rare and small enough to be acceptable for most software, while one asked why checkers cannot be bootstrapped from a tiny trusted core.

**Tags**: `#formal verification`, `#proof assistants`, `#Lean`, `#Metamath`, `#software correctness`

---

<a id="item-tech-news-5"></a>
### [Essay argues for a formally verifiable mainstream programming language](https://blainehansen.me/post/mainstream-verifiable-language/) ⭐️ 7.0/10

Blaine Hansen&\#x27;s blog post argues that mainstream programming languages should be designed for formal verification, rather than treating machine-checked guarantees as a specialist add-on. It is an argument essay, not a release announcement; the supplied material reports no new language, compiler, benchmark, or adoption milestone. The Hacker News thread discusses existing verification tools and whether a verification-first language can achieve mainstream adoption.

hackernews · todsacerdoti · Nov 27, 05:22 · [Discussion](https://news.ycombinator.com/item?id=50663089)

**「Background」** Formal verification uses machine-checked logic, rather than tests, to show that code satisfies a specification or cannot produce certain runtime errors. It has historically required specialized languages and toolchains: Ada SPARK grades assurance from &quot;Stone&quot; \(valid SPARK\) through &quot;Silver&quot; \(absence of runtime errors\) to &quot;Gold&quot; \(proof of key integrity properties\), according to AdaCore, while Dafny, Verus, Why3, Frama-C and TLA+ serve other languages and verification styles. Horizon&\#x27;s October 23 digest reported that Anthropic&\#x27;s Frontier Red Team, working with Theorem Labs, used Claude to prove security properties in more than one hundred open-source libraries within a few weeks, presented as extending verification beyond small codebases; that reported AI-assisted result, not independently confirmed, is the backdrop for arguing that verifiability belongs in mainstream language design.

**「Impact」** For teams, the immediate consequence is that verifiable code remains a toolchain choice: Ada SPARK, Dafny, Verus, Why3, Frama-C, and TLA+ each impose their own annotations and verification workflow, so adopting verification means committing to one of those ecosystems rather than enabling a flag in a mainstream language.

**「Community discussion」** Commenters debated adoption: one argued that &quot;mainstreamness comes from adoption&quot; and questioned whether a verification-first language can be designed as mainstream from the outset, while a language designer said the essay matched goals for Zena, a TypeScript-like Wasm GC language motivated partly by sandboxing AI-generated code. Another commenter reported translating existing C repositories to Ada SPARK and lifting them to SPARK Silver to rule out runtime errors, presenting that as evidence the workflow is already practical.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2113390212911083894">2026-10-23 — Anthropic announces Claude-based formal verification at scale</a></li>
<li><a href="https://www.adacore.com/blog/verifythis-challenge-in-spark">VerifyThis Challenge in SPARK | AdaCore</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#programming language design`, `#formal methods`, `#AI-generated code`, `#Ada SPARK`

---

<a id="item-tech-news-6"></a>
### [Anthropic system card describes covert limits on frontier-model R&amp;D requests](https://news.ycombinator.com/item?id=50664325) ⭐️ 7.0/10

Anthropic’s system card for Claude Mythos 5 and Fable 5, published in June, reportedly discloses that the company covertly reduces Claude’s response quality for requests aimed at developing frontier models. The interventions include prompt rewriting, steering vectors, and parameter-efficient fine-tuning, and are said to affect about 0.03% of traffic and under 0.1% of organizations, with most coding work unaffected. Unlike safety refusals, the adjustments reportedly do not fall back to another model and are not detectable by users; the card notes that using Claude to develop competitor models already violates Anthropic’s terms. The disclosure resurfaced this week in developer discussion, according to the secondary summary.

telegram · zaihuapd · Nov 27, 13:42

**「Background」** Anthropic released Fable 5 and Mythos 5 in June 2026 together with system cards, the documents in which the company records model behavior and safety policies; coverage of that launch also noted a new requirement to retain all traffic on the two models for 30 days. The disclosure is drawing renewed scrutiny as AI-assisted development becomes central to frontier work: Horizon&\#x27;s November 6 digest reported METR&\#x27;s estimate that Anthropic&\#x27;s rate of capability improvement roughly doubled, with about 80% of the acceleration attributed to AI-assisted R&amp;D, a figure METR and Anthropic staff did not agree on.

**「Developer impact」** Developers using Claude for pre-training pipelines, distributed training, or accelerator design can receive silently degraded answers with no fallback or visible signal, so teams should treat outputs in those areas as unreliable and validate them independently; Anthropic estimates the intervention affects about 0.03% of traffic and fewer than 0.1% of organizations, while most coding work is unaffected.

<details><summary>References</summary>
<ul>
<li>Anthropic Releases Claude Fable 5, Its Most Powerful AI Yet, With Cyber Safeguards</li>
<li><a href="https://x.com/dotey/status/2118466539510960161">2026-11-06 — METR Independent Evaluation: Anthropic&#x27;s Model Capability Progress Speed Roughly Doubled, Largely Due to AI-Assisted R&amp;D</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI policy`, `#model transparency`, `#AI safety`, `#developer trust`

---

<a id="item-tech-news-7"></a>
### [Minecraft Bedrock resource-pack flaw fixed in 26.65 after hidden-script exploits](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 7.0/10

Mojang fixed a Minecraft Bedrock resource-pack vulnerability in version 26.65 after add-on developer 8Crafter disclosed on November 15 that packs containing a content.zipe file could modify Ore UI files and run hidden scripts. 8Crafter said the flaw affected Bedrock versions 26.52 through 26.63, with earlier versions possibly affected too, across PC, mobile, and consoles; Java Edition was not affected. When resource-pack auto-download was enabled upon joining a server or Realm, players could receive a malicious pack without manually installing it. Reported abuses included deleting all saves and obtaining a player&\#x27;s IP address, plus, on Windows under specific conditions, opening an arbitrary URI without prompting and launching a batch file from the pack to download malware.

telegram · zaihuapd · Nov 27, 18:04

**「How Bedrock resource packs reach players」** In Bedrock Edition, resource packs are packages that can replace game assets, including interface files, and servers or Realms can deliver them automatically when a player has resource-pack auto-download enabled. The flaw involved a \`content.zipe\` file that could alter files in Ore UI, Bedrock&\#x27;s interface framework, allowing a pack to run hidden scripts without being manually installed.

**「Impact」** Players and server operators running Bedrock 26.52–26.63 should update to 26.65 rather than rely on detection alone. AxmBro&\#x27;s Windows tool can find packs containing content.zipe, but it cannot determine whether a pack is malicious.

**Tags**: `#Minecraft Bedrock`, `#security vulnerability`, `#resource packs`, `#code execution`, `#patching`

---

<a id="item-tech-news-8"></a>
### [Credit-card skimming scripts using WebRTC found on shopping sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 6.0/10

A report describes credit-card skimming scripts that use WebRTC on popular shopping sites, affecting shoppers who enter payment details at checkout. The report links the skimmer to WebRTC, but the available discussion cautions that the protocol is not the core vulnerability. The broader exposure is third-party scripts embedded in e-commerce pages, which can run with access to checkout data.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**「Background: web skimming and third-party scripts」** Web skimming, often tracked as MageCart, works by injecting malicious JavaScript into an e-commerce checkout so payment details are captured as they are typed and sent to an attacker-controlled server; the skimmers are plain JavaScript, and criminal services have offered obfuscation tooling to keep them from being detected. The most common injection route is a compromised third-party script embedded in the page, and PCI DSS requirements 6.4.3 and 11.6.1 now oblige merchants to authorize payment-page scripts, verify their integrity, and monitor them for tampering. The report described here concerns a skimmer variant that relays captured card data over WebRTC rather than ordinary HTTP requests.

**「Impact」** For e-commerce operators, the practical takeaway is to treat every third-party script on checkout pages as part of the payment attack surface; blocking WebRTC alone would not remove the reported risk.

**「Community discussion」** Commenters argued that WebRTC is incidental rather than the core mechanism, with one noting that ordinary AJAX or cross-domain POST requests could achieve the same effect and that embedding third-party scripts is the real exposure. Another commenter said the report justifies ad blocking, while a separate thread criticized the continued use of symmetric secrets for payments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/caramel-credit-card-stealing-service-is-growing-in-popularity/">Caramel credit card stealing service is growing in popularity</a></li>
<li><a href="https://cybersecuritynews.com/magecart-hackers/">MageCart Hackers Steal Customer Credit Card Data from Camera...</a></li>
<li><a href="https://origami.sa/en/blog/third-party-script-card-skimming-checkout/">Optimizely Hack: An Outside Tool Planted a Card Skimmer on 178...</a></li>

</ul>
</details>

**Tags**: `#web security`, `#payment skimming`, `#WebRTC`, `#third-party scripts`, `#e-commerce`

---

<a id="item-tech-news-9"></a>
### [Convex coding skill accused of uploading app ideas without disclosure](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 6.0/10

A GitHub issue alleges that a Convex coding skill sent a user&\#x27;s app idea to a remote server without clearly disclosing the upload. Convex CEO Jamie responded in the thread that the prompt upload powers Convex&\#x27;s “quickstart” feature, which he described as the spiritual successor to the recently shut-down Convex Chef. That response confirms an upload mechanism exists but does not show what users were told about it, and no independent verification of the behavior is provided.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**「Background」** The complaint concerns Convex&\#x27;s backend skill, whose quickstart workflow reportedly sends the user&\#x27;s app description to a remote server. In a comment on the issue, Convex CEO Jamie, posting as jamwt, said the upload powers the Convex quickstart feature and described it as the successor to Convex Chef, an end-to-end vibe-coding product that Convex recently shut down.

**「Impact」** Developers using the Convex skill should treat their prompts as data sent off their machine when the quickstart feature runs; app descriptions and product ideas are the payload at issue. Those working on confidential concepts need to decide whether that is acceptable or avoid the feature until disclosure is clearer.

**「Community discussion」** One commenter dismissed the concern with “Ideas are cheap,” while another argued the episode makes self-hosted open-weight models the better long-term choice. Neither comment addresses whether the upload was disclosed to users.

**Tags**: `#privacy`, `#AI coding tools`, `#developer tools`, `#transparency`, `#Convex`

---

<a id="item-tech-news-10"></a>
### [Michael Nielsen&\#x27;s Neural Networks and Deep Learning book taken down](https://neuralnetworksanddeeplearning.com/) ⭐️ 6.0/10

Michael Nielsen&\#x27;s online book &quot;Neural Networks and Deep Learning&quot; is no longer available at its original site, according to the Hacker News item. The removal prompted community archival efforts, including a single PDF consolidated under a CC BY-NC license and links to a Wayback Machine copy. The item does not state why Nielsen removed the book or whether the takedown is permanent.

hackernews · brandonb · Nov 27, 19:31 · [Discussion](https://news.ycombinator.com/item?id=50670757)

**「Background」** Michael Nielsen wrote Neural Networks and Deep Learning between 2011 and 2015 and published it free online, where it became one of the most recommended starting points for people learning how neural networks are trained. In November 2026 he replaced the book with a note saying he does not want to help train people to contribute to frontier AI work and that the labs are “knowingly endangering all of humanity”; the note is his own opinion, not an independent finding.

**「Impact」** Readers who bookmarked or teach from the free text will need to rely on community mirrors or archived copies, and should check the license and version of any copy before redistributing it.

**「Community discussion」** Commenters split between practical archiving and interpreting the removal as a protest: one consolidated the text into a CC BY-NC PDF, while others argued that withdrawing an accessible explanation of deep learning is a misstep and that the removal mainly functions as a protest whose reason should be heard.

<details><summary>References</summary>
<ul>
<li><a href="https://letsdatascience.com/news/michael-nielsen-takes-down-neural-networks-book-citing-front-5b13ee6c">Michael Nielsen takes down neural networks book, citing ...</a></li>
<li><a href="https://madrobot.blog/2026/11/27/michael-nielsen-takes-down-deep-learning-book/">Michael Nielsen takes down Neural Networks and Deep Learning book</a></li>

</ul>
</details>

**Tags**: `#neural networks`, `#deep learning`, `#open access`, `#AI education`, `#community discussion`

---

<a id="item-tech-news-11"></a>
### [Report: Anthropic study finds unlearning hides, not deletes, dangerous knowledge](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Anthropic%E6%8B%86%E7%A9%BFAI%E5%81%87%E9%81%97%E5%BF%98%EF%BC%8146%E4%B8%87%E7%A5%9E%E7%BB%8F%E5%85%83%E5%8A%A8%E5%87%A0%E5%8D%81%E4%B8%AA%EF%BC%8C%E9%BB%91%E5%AE%A2%E7%9F%A5%E8%AF%86%E5%B0%B1%E5%A4%8D%E6%B4%BB) ⭐️ 6.0/10

A Chinese tech-media report says Anthropic shared two studies on Nov. 25 that found supposedly forgotten dangerous knowledge can remain recoverable in AI models. In some unlearning models with about 460,000 neurons, restoring only a few dozen neurons to their pre-forgetting state reportedly pushed suppressed correct answers back to the highest probability. The report also says 14 of 23 unlearning models still often assigned the highest probability to correct answers for questions they knew before unlearning, even when conventional test scores were low. It concludes that most tested unlearning methods appear to hide dangerous knowledge rather than remove it; the report does not name the specific models or methods, and these claims were not independently verified here.

rss · 新智元 · Nov 27, 03:27

**「Background」** Machine unlearning refers to fine-tuning a model to strip specific dangerous knowledge, such as hacking techniques, and safety checks have typically relied on the model&\#x27;s score on withheld dangerous questions. Horizon&\#x27;s November 25 digest reported that Anthropic Fellows were revisiting individual neurons as a basis for interpretability, arguing the approach remains useful despite objections that a single neuron fires on unrelated inputs and that facts appear spread across many neurons; the new report applies that neuron-level analysis to the question of whether unlearning actually removes knowledge.

**「Impact」** According to the report, organizations using unlearning to strip dangerous capabilities cannot treat low multiple-choice scores as proof of removal; they may need to check answer-probability rankings or internal neuron states as well.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/AnthropicAI/status/2125365268381929637">2026-11-25 — Anthropic Fellows revisit neurons as a basis for interpretability</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#machine unlearning`, `#neural networks`, `#Anthropic`, `#model security`

---

<a id="item-tech-news-12"></a>
### [Google Play to publish merchant developer phone and address from 2027](https://www.androidpure.com/google-play-trader-developer-address/) ⭐️ 6.0/10

Google Play will globally display the phone number and address of developers who declare themselves merchants starting March 1, 2027, including individual account holders. All active developer accounts must declare merchant or non-merchant status by February 1, 2027; missing that deadline may block app updates and lead to removal from Play worldwide. The policy was announced in October and drew developer backlash this week over privacy concerns; the source says EU rules do not require showing these details to users outside the EU.

telegram · zaihuapd · Nov 27, 01:44

**「Earlier context」** Google first announced the merchant-contact rule in October. It extends the “trader” disclosure that EU rules require within the EU to a worldwide audience, even though the source notes those rules do not require showing the details to users outside the EU; the designation applies to developers who self-declare as merchants rather than non-commercial publishers.

**「Impact」** Individual developers who declare merchant status will have a phone number and address shown to Play users globally, beyond the EU requirements described in the source. They need to choose their merchant status and contact details before February 1, 2027, because failure may block app updates and lead to global delisting.

**Tags**: `#Google Play`, `#developer policy`, `#privacy`, `#app distribution`, `#regulatory compliance`

---

<a id="item-tech-news-13"></a>
### [Report: AI Tool Artex Used in Attacks on U.S. Intelligence Agencies](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 6.0/10

A New York Times report relayed by Forbes claims hackers used an AI tool called Artex in attacks on the CIA, the National Geospatial-Intelligence Agency and the Office of the Director of National Intelligence. The reported attack appears limited in severity and affected non-classified reconnaissance data, according to the account. Artex, released earlier this year by a Chinese developer, combines multiple open-source AI models to test network and computer defenses; the developer later removed it from GitHub after it was used in multiple attacks, including one against the EU, and the FBI had warned earlier this year that criminals and spies were widely using it. The account provides limited technical detail and no independent confirmation.

telegram · zaihuapd · Nov 27, 10:42

**「Earlier ARTEX abuse」** ARTEX is an open-source, LLM-driven agentic platform that threat actors have weaponized to automate multiple phases of cyber intrusions, according to an FBI flash advisory. Horizon&\#x27;s October 9 digest had already reported CrowdStrike linking ARTEX, along with model-relay services, to attacks on South Korean financial institutions. The current report extends that pattern to U.S. intelligence agencies, though it provides few verifiable technical details.

<details><summary>References</summary>
<ul>
<li><a href="http://xcai.pro/">2026-10-09 — CrowdStrike Reports Open-Source AI Tool ARTEX Used in South Korea Financial Attacks</a></li>
<li><a href="https://www.ic3.gov/CSA/2026/261113.pdf">Threat Overview of ARTEX Autonomous Penetration Testing Framework</a></li>

</ul>
</details>

**Tags**: `#AI cybersecurity`, `#cyberattack`, `#intelligence agencies`, `#open-source AI`, `#Artex`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache nightly-xpu Release](https://github.com/LMCache/LMCache/releases/tag/nightly-xpu) ⭐️ 5.0/10

LMCache published a nightly Intel XPU wheel built from \`dev\` on 2026-11-27, intended for installation inside a specified vLLM XPU runtime image.

github · github-actions\[bot\] · Nov 27, 10:16

**「Problem Solved」** The release provides an Intel XPU-compatible LMCache package and an install command for a vLLM XPU runtime image, addressing distribution and installation for that environment. The item does not describe functional changes, performance improvements, or other technical bottlenecks.

**「Background」** LMCache provides a KV-cache layer for LLM inference that stores and reuses KV states across requests and integrates with vLLM, reducing repeated prefill computation for long-context workloads \(tool-1-2\). vLLM&\#x27;s optimization documentation also references LMCache&\#x27;s multi-process connector among KV-cache connectors with specific compatibility considerations \(tool-1-1\). This nightly artifact packages LMCache from the \`dev\` branch as an Intel XPU wheel \(\`0.5.9.dev89+xpu\`\) for a vLLM XPU runtime image, extending distribution to Intel&\#x27;s GPU stack; Intel maintains an optimized vLLM variant for its multi-GPU platform \(tool-1-3\). The item supplies no release notes or functional/performance changes, so its significance is mainly packaging and platform enablement rather than a new capability.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/configuration/optimization/">Optimization and Tuning - vLLM</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/intel/llm-scaler/blob/main/vllm/README.md">llm -scaler/ vllm /README.md at main · intel / llm -scaler · GitHub</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#Intel XPU`, `#vLLM`, `#nightly release`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels of LMCache, built from the dev branch \(0.5.9.dev89+rocm7.2\), for AMD Instinct MI300X/MI325X \(gfx942\) and MI350X/MI355X \(gfx950\). The wheels are ABI-matched to the upstream vLLM ROCm container with torch 2.13 and cp312.

github · github-actions\[bot\] · Nov 27, 08:56

**「Problem Solved」** Running LMCache&\#x27;s KV-cache layer with vLLM on AMD hardware usually means building from source against a specific ROCm, PyTorch, and Python combination, and matching the ABI of the vLLM container. These prebuilt wheels remove that build step and reduce ABI mismatch risk for the listed Instinct GPUs. The release itself contains no architectural change, new capability, benchmark, or fix; its value is packaging and deployment convenience.

**「Ecosystem context」** LMCache positions itself as a KV-cache layer for LLM inference — storing, compressing, and reusing KV cache across a cluster rather than discarding it when a request finishes \(tool-1-2\). Its most common deployment path is vLLM, where it can run in-process via \`LMCacheConnectorV1\`, configured through environment variables or a YAML config file \(tool-1-1\). That coupling means LMCache wheels must track the exact PyTorch/Python ABI of the vLLM build they load into.

On the AMD side, the ROCm-enabled vLLM Docker image is the standard prebuilt environment for inference on Instinct MI355X, MI350X, MI325X and MI300X GPUs \(tool-2-2\) — the same four parts named in this release. This nightly \(0.5.9.dev89+rocm7.2, from the \`dev\` branch\) is therefore a distribution artifact rather than an engineering one: it publishes gfx942 and gfx950 wheels ABI-matched to that upstream container \(torch 2.13, cp312\), so AMD users can install the KV-cache layer into the stock vLLM ROCm image instead of reconciling build toolchains themselves.

As an automated nightly, it signals no feature, benchmark, or fix — its significance is that AMD support is now maintained on a continuous, versioned build cadence alongside the upstream ROCm vLLM image.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/examples/disaggregated/lmcache/">LMCache Examples - vLLM</a></li>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.2.4/how-to/rocm-for-ai/inference/benchmark-docker/vllm.html">vLLM inference — ROCm Documentation</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#inference`, `#serving`, `#KV cache`, `#vLLM`, `#ROCm`, `#AMD`, `#nightly build`, `#packaging`

---

<a id="item-ai-projects-3"></a>
### [LMCache nightly RBLN wheel for Rebellions NPUs](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

Nightly LMCache wheel packaged for Rebellions RBLN NPUs, built from the dev branch against torch-rbln 0.12.0. It lets users install LMCache 0.5.9.dev89+rbln in environments that already provide the RBLN compiler and driver, without bundling vendor tooling.

github · github-actions\[bot\] · Nov 27, 09:50

**「Problem solved」** The release reduces deployment friction for running LMCache&\#x27;s KV-cache layer on Rebellions NPUs: instead of building the package for that backend, users can pip-install a prebuilt wheel. The wheel deliberately leaves torch-rbln, rebel-compiler, and the RBLN driver host-owned, avoiding bundling the vendor toolchain and requiring a compatible environment. No performance, API, or architectural changes are stated; this is routine nightly packaging that extends availability to RBLN environments while keeping the vendor stack external.

**「Ecosystem Context」** LMCache is a KV cache management layer for LLM inference: it turns KV cache from transient GPU state into persistently stored, cross-engine reusable knowledge, which reduces time-to-first-token and improves throughput for long-context serving \(tool-1-1, tool-1-3\). Its own usage data shows KV cache volumes growing well beyond what GPU memory can hold, motivating the move of caches off-device \(tool-1-2\).

This nightly wheel extends that layer to Rebellions RBLN NPUs alongside the existing GPU path. RBLN support arrives through torch-rbln, a PyTorch out-of-tree extension that exposes an \`rbln\` device and \`torch.compile\` while coordinating execution with the RBLN compiler and runtime \(tool-2-1, tool-2-2\); the wider RBLN SDK supplies compiler, runtime, model zoo and serving frameworks \(tool-2-3\).

As a release, the notable fact is packaging, not architecture: it is built nightly from \`dev\` against torch-rbln 0.12.0 \(torch 2.13.0+cpu\), and torch-rbln, rebel-compiler and the driver remain host-owned rather than bundled. No performance, API or architectural changes are stated, so the practical signal is an additional hardware target for KV-cache offloading — useful for non-NVIDIA deployments, but unproven until benchmarked.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">GitHub - RBLN-SW/torch-rbln: PyTorch extension for Rebellions NPU</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch-rbln · PyPI</a></li>
<li><a href="https://rebellions.ai/developers/">Developers - Rebellions</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#inference`, `#NPU`, `#RBLN`, `#nightly build`, `#packaging`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s State Council pledges stronger &\#x27;national team&\#x27; market support](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 8.0/10

China&\#x27;s State Council pledged at a Nov 27 executive meeting to strengthen the &quot;national team&quot; of state-linked buyers in stabilizing the capital market and to improve Central Huijin&\#x27;s role as a quasi-stabilization fund—a state-backed vehicle for market support—with ample liquidity; it also urged listed companies to raise dividends and buybacks. The readout gave no amounts, timelines or implementation details.

telegram · zaihuapd · Nov 27, 05:35

**「Background」** China’s “national team” refers to state-backed buyers used to support share prices in downturns, with Central Huijin a core institution; an expert quoted by Eastmoney said the readout elevates its quasi-stabilization-fund role from a crisis-response tool to standing financial infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.eastmoney.com/a/202611273941634358.html">如何理解 国 常会对资本 市 场的最新定调？ 专 家 解读来了 _ 东方财富网</a></li>

</ul>
</details>

**Tags**: `#China policy`, `#capital markets`, `#Central Huijin`, `#market stabilization`, `#securities regulation`

---

<a id="item-finance-news-2"></a>
### [China&\#x27;s Central Bank Cuts Large-Deposit Minimum to 100,000 Yuan](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

The People&\#x27;s Bank of China published new rules on large-denomination certificates of deposit on Nov. 27, lowering the minimum purchase for individual investors to 100,000 yuan and for institutional investors to 5 million yuan — half the previous 200,000 yuan and 10 million yuan thresholds — effective March 21, 2027.

telegram · zaihuapd · Nov 27, 11:36

**「背景」** 大额存单是银行发行的、设有最低认购金额的存款产品，这一门槛决定哪些储户可以购买；现行规则来自2015年的暂行办法，央行今年6月已启动修订征求意见。

**「Impact」** From March 2027, savers holding 100,000–200,000 yuan become eligible for large-denomination certificates of deposit, widening the set of deposit products they can buy, while the accompanying rate rules bar banks from attracting deposits with above-market interest.

<details><summary>References</summary>
<ul>
<li><a href="https://www.jingjiribao.cn/static/detail.jsp?id=662855">“不低于 20 万 元 ” 个 人 投资 人 认购 大 额 存 单 起点金 额 拟下调</a></li>

</ul>
</details>

**Tags**: `#大额存单`, `#央行监管`, `#存款利率`, `#银行负债`, `#个人理财`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Paul Graham: Startup &\#x27;Partnerships&\#x27; Are Usually a Waste of Time](https://x.com/paulg/status/2126462588766527593) ⭐️ 6.0/10

Paul Graham argues that partnerships are usually a waste of time for startups. In his framing, the only partnership-like arrangements worth pursuing are two &quot;degenerate cases&quot;: one where the startup buys someone else&\#x27;s product, and one where someone buys the startup&\#x27;s product. He points out that these straightforward commercial relationships are never called &quot;partnerships,&quot; and treats the need for that &quot;weird, special name&quot; as a bad sign. The post offers a compact heuristic rather than data or case studies: if a deal has to be labeled a partnership, founders should be skeptical of its value.

twitter · Paul Graham · Nov 27, 23:46

**「Background」** Paul Graham is a co-founder of Y Combinator and a longtime writer on startups and founders, and the post comes from his personal X account. The advice lands in a familiar startup context: early-stage companies are often courted with business-development, co-marketing, integration, or distribution &quot;partnerships&quot; that can consume founder time without producing revenue. Graham&\#x27;s distinction is between those arrangements and ordinary customer-vendor transactions, which he suggests are the only kinds that reliably matter. The post is a short opinion piece; it does not provide examples, definitions, or supporting data, so the claim is best read as a founder heuristic rather than an empirical finding.

**Tags**: `#startups`, `#business-strategy`, `#partnerships`, `#founder-advice`, `#opinion`

---