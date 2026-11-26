---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 64 items, 23 important content pieces were selected

---

**Technology News**
1. [1Password reports November 2026 incident over malicious production code push](#item-tech-news-1) ⭐️ 8.0/10
2. [GRH Lean verification attributed to Anthropic cut to ~76k lines](#item-tech-news-2) ⭐️ 8.0/10
3. [Aaronson post fuels debate on AI and open math proofs](#item-tech-news-3) ⭐️ 8.0/10
4. [Minecraft Java resource-pack font flaw enables RCE, no patch yet](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Research posts papers on integer factorization and discrete logarithms](#item-tech-news-5) ⭐️ 7.0/10
6. [Lean audit of Clojure core claims previously unreported bugs](#item-tech-news-6) ⭐️ 7.0/10
7. [Tencent open-sources Hy4 flash GGUF weights, smallest runs on 64GB Mac mini](#item-tech-news-7) ⭐️ 7.0/10
8. [Samsung and SK Hynix reportedly to use YMTC Xtacking technology](#item-tech-news-8) ⭐️ 7.0/10
9. [Windows loudness equalization reverse-engineered and ported to PipeWire](#item-tech-news-9) ⭐️ 6.0/10
10. [Essay argues LLM users still own code review](#item-tech-news-10) ⭐️ 6.0/10
11. [Linux 7.4 reverts driver-bind taint patch after real-world conflicts](#item-tech-news-11) ⭐️ 6.0/10
12. [Anthropic&\#x27;s Claude Ship beta adds AI code review and approvals](#item-tech-news-12) ⭐️ 6.0/10
13. [LeCun Accuses Amodei of Using AI-Risk Fears to Restrict Open Models](#item-tech-news-13) ⭐️ 6.0/10
14. [OpenAI positions cybersecurity as bigger than coding, expands GPT-6 Cyber access](#item-tech-news-14) ⭐️ 6.0/10
15. [Asian data centers seek U.S. buyers as Nvidia export loophole tightens](#item-tech-news-15) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](#item-ai-projects-1) ⭐️ 5.0/10
2. [LMCache Nightly RBLN NPU Wheel](#item-ai-projects-2) ⭐️ 5.0/10

**Financial News**
1. [Court Filings Allege Commerce Department Pressured Intel Into Giving U.S. Government 10% Stake](#item-finance-news-1) ⭐️ 9.0/10
2. [SpaceX and Tesla reportedly weigh $3.5 trillion all-stock merger](#item-finance-news-2) ⭐️ 8.0/10
3. [US Plans New Section 301 Tariffs on 14 Trading Partners, Including China and EU](#item-finance-news-3) ⭐️ 8.0/10
4. [SpaceX 放弃 7.38 亿美元联邦宽带补贴，转而免费提供 Starlink 设备](#item-finance-news-4) ⭐️ 7.0/10

**Twitter News**
1. [Dario Amodei Denies Anthropic Wants to Hand Decision-Making to Superintelligence](#item-twitter-news-1) ⭐️ 7.0/10
2. [Consumer AI agents face a unit-economics reckoning](#item-twitter-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [1Password reports November 2026 incident over malicious production code push](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password published an update on a November 2026 security incident involving malicious code pushed to production backend services, a supply-chain path that matters to its password-manager users and to SaaS teams relying on code-push controls. Available details do not give an affected-user count or say whether branch-protection rules were missing or bypassed. The update is the company&\#x27;s account rather than an independently verified postmortem, and commenters are pressing for an explicit statement that encrypted vaults were not downloaded.

hackernews · lxhrstn · Nov 25, 17:18 · [Discussion](https://news.ycombinator.com/item?id=50644817)

**「Why backend access matters for a password manager」** 1Password is a subscription password manager whose customers&\#x27; vaults are encrypted and synced through company-operated servers, which also hold administrative account records such as names and email addresses; the company said the exposed data was limited to that administrative layer rather than vault contents. In SaaS deployments generally, a developer&\#x27;s GitHub identity is often tied to pipelines that build and run code with backend privileges, so control of one employee account can translate into the ability to ship code that executes in production.

**「Customer impact」** 1Password customers should treat unexpected account-related emails as suspect: the company says some customer names and email addresses were accessed, while vault contents were not compromised.

**「Community discussion」** Commenters treated the incident as a standard SaaS supply-chain risk: tptacek argued that a compromised employee laptop leading to a production code push is the standard breach pattern, and ctidd criticized the update for not saying whether pushes to main are disabled or branch protections were missing or bypassed. A long-time user who keeps a local-only vault said the incident reinforces concerns about production code changes, and another commenter wanted an explicit statement that encrypted vaults were not downloaded.

<details><summary>References</summary>
<ul>
<li><a href="https://1password.com/blog/update-on-nov-2026-security-incident">Update on a security incident involving 1Password’s backend ...</a></li>
<li><a href="https://www.macrumors.com/2026/11/25/1password-security-breach/">1Password Security Breach: What Was Accessed and What Wasn&#x27;t</a></li>
<li><a href="https://1password.com/blog/update-on-nov-2026-security-incident">Update on a security incident involving... | 1 Password</a></li>
<li><a href="https://www.macrumors.com/2026/11/25/1password-security-breach/">1 Password Security Breach: What Was Accessed and... - MacRumors</a></li>

</ul>
</details>

**Tags**: `#security`, `#1Password`, `#supply-chain`, `#SaaS`, `#incident-response`

---

<a id="item-tech-news-2"></a>
### [GRH Lean verification attributed to Anthropic cut to ~76k lines](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

A GitHub repository, lsernau/grh-lean, presents a dramatically shortened Lean formalization of a GRH verification attributed to Anthropic, reducing the proof from roughly 17 million lines to about 76,000 lines—a 99.56% cut. The repository also includes a more readable ~300,000-line version with human-readable documentation and a split between known and new mathematics, according to discussion. The supplied material does not report independent validation, and commenters question whether humans can realistically read and verify the compact proof.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**「Background」** Horizon&\#x27;s November 21 digest reported that Levent Alpöge, a mathematician at Anthropic, claimed a Claude-assisted proof of the Riemann and generalized Riemann hypotheses, with a Lean formalization described as roughly 15 million lines and 1.3 GB across 14 downloadable parts; the claim remained unverified at that stage. Lean is a proof assistant that machine-checks a formal argument&\#x27;s correctness, and the current item points to a shortened edition of that same claimed GRH formalization.

**「Verification burden」** For Lean users, the compact artifact is a Lean 4 proof built on Mathlib and restricted to the axioms propext, Classical.choice, and Quot.sound, so teams reusing it must reproduce the build and check that statement and axiom set rather than treating the line reduction as proof of correctness. Independent verification of the formalization by Lean FRO and the Mathlib Initiative was announced the day after release, but that does not by itself establish that this shortened version is human-readable or has itself been independently reviewed.

**「Community Discussion」** Commenters welcomed the documented ~300,000-line version and its known/new-math split as easier to digest, while one asked how realistically a human could read and verify the compact Lean code. Another commenter contrasted the effort spent on incremental proof reductions with Anthropic&\#x27;s apparent ability to achieve a much larger cut using compute and better internal models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">2026-11-21 — Anthropic mathematician claims Claude-assisted Riemann hypothesis proof in Lean</a></li>
<li><a href="https://alpo.ge/remark.pdf">2026-11-21 — Levent Alpöge claims Generalized Riemann Hypothesis proof with Lean formalization</a></li>
<li><a href="https://en.wikipedia.org/wiki/Alp%C3%B6ge&#x27;s_proof_of_the_Riemann_hypothesis">Alpöge&#x27;s proof of the Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://github.com/lsernau/grh-lean">GitHub - lsernau/ grh - lean : A short Lean 4 proof of the Generalized...</a></li>

</ul>
</details>

**Tags**: `#Lean`, `#formal verification`, `#AI-assisted mathematics`, `#proof compression`, `#open source`

---

<a id="item-tech-news-3"></a>
### [Aaronson post fuels debate on AI and open math proofs](https://scottaaronson.blog/?p=10379) ⭐️ 8.0/10

Scott Aaronson&\#x27;s new blog post, discussed on Hacker News, points readers to a paper titled &quot;The matrix multiplication exponent is nine fourths&quot; and has prompted debate over AI systems solving open mathematics and theoretical computer science problems. The supplied excerpt does not include the post&\#x27;s argument, the paper&\#x27;s methods, or confirmation of any claimed proof, so the specific advances remain unverified here.

hackernews · Kotlopou · Nov 25, 19:11 · [Discussion](https://news.ycombinator.com/item?id=50646108)

**「Earlier context」** Horizon&\#x27;s November 21 digest covered an earlier Scott Aaronson post that discussed claims LLMs had “apparently proved” the Riemann Hypothesis; that item supplied only the post title and comments, with no paper, Lean proof, or verification result, while a separate item that day described a claimed Generalized Riemann Hypothesis proof with a very large Lean formalization that remained unverified. The current post continues Aaronson&\#x27;s coverage of AI-assisted mathematics and points readers to a paper titled “The matrix multiplication exponent is nine fourths,” with Lean-checked verification the relevant test for distinguishing a claimed result from an established one.

**「Community discussion」** Commenters debate whether such progress would have come from Lean, Mathlib, and raw computing power without LLMs, and one warns that any &quot;singularity&quot; may be safely contained only if it is limited to verifiable tasks. Another argues that minor mismatches between Lean and informal proofs should not be used to deny that many open problems are being solved, while a third asks what a post-&quot;classical&quot; era of mathematics would look like.

<details><summary>References</summary>
<ul>
<li><a href="https://scottaaronson.blog/?p=10344">2026-11-21 — Scott Aaronson Post on LLM Claims and the Riemann Hypothesis</a></li>
<li><a href="https://alpo.ge/remark.pdf">2026-11-21 — Levent Alpöge claims Generalized Riemann Hypothesis proof with Lean formalization</a></li>

</ul>
</details>

**Tags**: `#AI for mathematics`, `#theorem proving`, `#Lean`, `#computational complexity`, `#Hacker News discussion`

---

<a id="item-tech-news-4"></a>
### [Minecraft Java resource-pack font flaw enables RCE, no patch yet](https://github.com/bikini/minecraft2shell) ⭐️ 8.0/10

The public minecraft2shell proof-of-concept, disclosed on November 22, shows that a crafted TrueType font in a server resource pack can trigger a native out-of-bounds write in FreeType 2.14.3 and earlier and execute arbitrary code on the Minecraft Java Edition 26.3 Windows client. According to the Telegram post, the affected releases are Java Edition 1.20.5 through 1.21.10 and snapshots 26.1 through 26.4; 1.20.4 and earlier and Bedrock Edition are unaffected. Mojang still ships lwjgl-freetype 3.4.3 and no official patch is available. A community fix, m2sfix 1.0.0, was released November 24 and disables font hinting through a Java agent or mod.

telegram · zaihuapd · Nov 25, 12:46

**「Why a font bug becomes remote code execution」** Minecraft Java Edition clients render custom fonts supplied by server resource packs, and the game does this through FreeType, the native font library, which the game reaches via LWJGL&\#x27;s lwjgl-freetype binding \(version 3.4.3 in current builds\). Because a resource pack is pushed by the server and parsed on the client, a memory-safety flaw in FreeType&\#x27;s TrueType handling — an out-of-bounds write present through FreeType 2.14.3 — is reachable from a remote server rather than requiring local file access. Mojang has not yet published a patched build, which is why the reported workaround is to refuse resource packs or use the community fix that disables hinting.

**「Impact」** Because the exploit path is a server-provided resource pack, affected players should avoid adding resource packs and set multiplayer server resource-pack permissions to disabled, or install m2sfix 1.0.0 until Mojang issues a patch.

**Tags**: `#Minecraft`, `#RCE`, `#FreeType`, `#Java`, `#security vulnerability`

---

<a id="item-tech-news-5"></a>
### [Google Research posts papers on integer factorization and discrete logarithms](https://github.com/google-research/google-research/tree/master/cogentic_research_papers) ⭐️ 7.0/10

Google Research has published a collection of papers in a GitHub directory named cogentic\_research\_papers, with the listing covering integer factorization, discrete logarithms and other topics. The supplied material includes no abstracts, methods, complexity claims or peer-review status, so it is not established whether any of the work bears on the security of deployed public-key systems such as RSA or elliptic-curve cryptography, or whether the results improve on existing algorithms. The Hacker News submission, dated 25 November 2026, drew discussion that treated the posting as a signal of something larger rather than assessing the papers themselves.

hackernews · rgwohlbold · Nov 25, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50642086)

**「Background」** Integer factorization and discrete logarithms are the computational hardness assumptions behind public-key schemes such as RSA and Diffie–Hellman, so results that lower their asymptotic complexity bear directly on how those systems are parameterized. The Google Research directory collects several papers rather than a single result; listed titles include “Unconditional Integer Factorization in Time L\_N\[1/3, O\(1\)\],” a deterministic subexponential factoring paper, and a sub-quasi-polynomial discrete-log paper for finite fields of fixed characteristic.

**「No confirmed crypto break」** For cryptography teams, the supplied material supports a verification task rather than an urgent migration: RSA and discrete-log-based systems still rest on hardness assumptions, and the item gives no published algorithms, parameter sizes, or measured runtimes showing a practical break. Engineers should wait for technical details and independent reproduction before changing key sizes or protocols; one Hacker News commenter likewise notes that a practical classical factoring algorithm would be significant but would not by itself say much about discrete logs.

**「Community discussion」** One commenter cited &quot;rumors about, from credible people, that this is the tip of something bigger&quot; and linked an X post, while others argued that recent mathematical results reflect machine-learning search over large spaces, drawing an analogy to AlphaGo, and said they had revised a prior belief that mathematics was immune to being advanced by money. No comment described reading the papers or reported a specific result, and the thread&\#x27;s engagement reflects interest rather than agreement on what the work contains.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/google-research/google-research/tree/master/cogentic_research_papers">Google Releases Cogentic Papers on Integer Factorization ...</a></li>
<li><a href="https://daily.dev/posts/google-releases-cogentic-papers-on-integer-factorization-discrete-logs-and-more-0lfmvr55g">Google Releases Cogentic Papers on Integer Factorization ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Computational_hardness_assumption">Computational hardness assumption - Wikipedia</a></li>
<li><a href="https://news.ycombinator.com/item?id=50642086">Google releases Cogentic papers on integer factorization , discrete ...</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#integer-factorization`, `#discrete-logarithms`, `#google-research`, `#number-theory`

---

<a id="item-tech-news-6"></a>
### [Lean audit of Clojure core claims previously unreported bugs](https://s.conao3.com/blog/2026/e4f733) ⭐️ 7.0/10

A blog post reports that its author used the Lean proof assistant to check Clojure&\#x27;s core library and found bugs that had not previously been reported. The supplied material gives no specific versions, fixes, maintainer response, or independent confirmation, so the findings remain the author&\#x27;s claims. Commenters disputed at least two of the listed cases, leaving the number of genuine bugs unsettled.

hackernews · encyclopedism · Nov 25, 14:56 · [Discussion](https://news.ycombinator.com/item?id=50642939)

**「Lean and formal verification context」** Lean is a proof assistant: users encode definitions and claims, and a checker verifies each proof step mechanically rather than relying on example-based tests. Auditing a standard library this way means stating properties its functions should satisfy and checking whether the implementation supports them; a failed check can expose either a library bug or a bad assumption in the stated property. Clojure&\#x27;s core library supplies the language&\#x27;s fundamental functions and data types, so defects there can affect many programs.

**「Verify before filing upstream」** Anyone filing these findings upstream should reproduce them first: commenter rvprasad flagged two entries as noise rather than core defects — \`\(.indexOf \(seq \(byte-array \[1 2 3\]\)\) 2\)\` passes a Long to a call on bytes, and \`\(get &quot;abc&quot; 1.9\)\` reflects \`get\`&\#x27;s coercion of the key to an integer for string collections, which he argues is intentional behavior. A second commenter points to a comparable audit of other Lisp implementations \(SBCL, Clozure, ACL2\) that he says surfaced dozens of issues, suggesting the approach generalizes beyond Clojure.

**「Community discussion」** rvprasad argued that two listed findings are not genuine bugs: one passes a Long value to \`.indexOf\` on a byte array, and another relies on \`get\` coercing a float key when used on a string. The same commenter said filtering such noise would make the audit more useful; another commenter linked a similar audit of Common Lisp compilers, and others asked why Lean was chosen over Rocq.

**Tags**: `#Clojure`, `#Lean`, `#formal verification`, `#bug auditing`, `#programming languages`

---

<a id="item-tech-news-7"></a>
### [Tencent open-sources Hy4 flash GGUF weights, smallest runs on 64GB Mac mini](https://mp.weixin.qq.com/s/o0xxShVQX6g2UllrrEv1WQ) ⭐️ 7.0/10

Tencent&\#x27;s Hunyuan team has open-sourced GGUF quantized weights for its 224B-parameter Hy4 flash model through the AngelSlim compression toolkit. The original weights are about 410.27 GiB, while the smallest IQ2-AH variant is 125.73 GiB, roughly 30% of the original, and Tencent says it can run on a 64GB Mac mini with the Strata offload framework. The release reports 89 tokens/s at 10K context on a 48GB-VRAM device and 47 tokens/s at 32K context with Q3\_K on a 128GB M5 Max, with Q3\_K scoring within 0.4 points of the original model on evaluations including DeepSWE v1.1.

telegram · zaihuapd · Nov 25, 09:29

**「Background」** Horizon&\#x27;s November 17 digest reported that Tencent&\#x27;s Hy4 flash is a 224B-parameter \(12B active\) multimodal MoE with a 1M-token context, and that Tencent said it planned to open-source the model. The current release delivers that open-source step as GGUF quantized weights published through Tencent&\#x27;s AngelSlim compression toolkit. The Strata offload framework named as the enabler was previously covered in Horizon&\#x27;s October 5 digest, which described it as an early-stage open-source inference project claiming to run a 125B model on consumer hardware such as an RTX 4090 at roughly 100 tokens/s.

**「Deployment impact」** Users aiming at a 64 GB Mac mini should treat this as an offload setup: the smallest IQ2-AH weights are 125.73 GiB, so the model does not fit in RAM and depends on the Strata framework plus adequate storage. Tencent&\#x27;s quoted throughput—89 tokens/s at 10K context on a 48 GB-VRAM device and 47 tokens/s at 32K context for Q3\_K on a 128 GB M5 Max—shows that practical performance varies with the chosen variant and hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://mp.weixin.qq.com/s/5yBbf-ctYziM5r0i6Y17lA">2026-11-17 — 腾讯混元发布 Hy4 flash：224B MoE、1M 上下文并大幅降价</a></li>
<li><a href="https://github.com/Niko1221/Strata">2026-10-05 — Strata claims Qwen 3.8 Flash Next 125B at ~100 tok/s on RTX 4090</a></li>
<li><a href="https://original.ifeng.com/c/8yLCKwSsFD6">腾讯混元Hy4 flash开源GGUF量化权重 224B模型可跑在64GB Mac mini上</a></li>
<li><a href="https://www.4nod.com/a/hy4-flash-strata-offload-64-gb-mac-mini">腾讯开源 Hy4 flash 量化权重 最小版借助 Strata offload 框架可运行...</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#model-quantization`, `#GGUF`, `#local-LLM`, `#Tencent-Hunyuan`

---

<a id="item-tech-news-8"></a>
### [Samsung and SK Hynix reportedly to use YMTC Xtacking technology](https://tech.ifeng.com/c/8yLRPKxQy4L) ⭐️ 7.0/10

Samsung Electronics and SK Hynix have reportedly agreed through a cross-licensing arrangement to use parts of Yangtze Memory Technologies&\#x27; Xtacking technology in 3D NAND flash. Xtacking fabricates memory cells and CMOS control circuitry on separate wafers and then bonds them together, allowing the two parts to be produced and optimized independently; an Omdia senior analyst said this lets memory makers produce the storage array themselves while assigning logic circuitry to a foundry for more advanced processes. The report relies on unnamed claims, and Samsung, SK Hynix and YMTC all declined to comment, so the agreement and its scope remain unconfirmed.

telegram · zaihuapd · Nov 25, 14:33

**「How Xtacking works」** Xtacking is not new: YMTC first demonstrated the wafer-bonding approach in 2018, and the company says it has since filed more than 12,000 patents worldwide, including over 4,000 US patent applications. The method differs from conventional 3D NAND by fabricating the memory array and the CMOS control circuitry on separate wafers and then bonding them, allowing each part to be produced and optimized independently.

**「Split array/logic manufacturing」** Because Xtacking builds the memory array and the CMOS logic on separate wafers, the reported cross-licenses would let Samsung and SK Hynix make the array in-house while sourcing logic from foundries on more advanced nodes — the arrangement described by the Omdia analyst quoted in the source. TechPowerUp reports both makers are pressing against single-wafer limits at hundreds of layers, so licensing a production-tested bonding process offers a shorter path than developing one from scratch. All three companies declined to comment, so no scope, timeline, or royalty terms are confirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/samsung-and-sk-hynix-tap-ymtcs-xtacking-tech-in-cross-license">Samsung and SK Hynix cross-license YMTC&#x27;s Xtacking 3D NAND</a></li>
<li><a href="https://www.techpowerup.com/355199/samsung-and-sk-hynix-to-license-ymtcs-xtacking-technology">Samsung and SK hynix to License YMTC&#x27;s Xtacking ... | TechPowerUp</a></li>
<li><a href="https://www.allpcb.com/allelectrohub/3d-nand-hits-400-layers-with-hybrid-bonding">3 D NAND Hits 400+ Layers with Hybrid Bonding</a></li>

</ul>
</details>

**Tags**: `#3D NAND`, `#Xtacking`, `#semiconductor manufacturing`, `#memory industry`, `#cross-licensing`

---

<a id="item-tech-news-9"></a>
### [Windows loudness equalization reverse-engineered and ported to PipeWire](https://github.com/xoxorwr/pw-loudness-eq) ⭐️ 6.0/10

The GitHub project pw-loudness-eq is a reverse-engineered port of Windows&\#x27; loudness equalization and limiting behavior to PipeWire, aimed at Linux audio users who want that processing available in their audio stack. The supplied material identifies the repository and target platform but provides no release version, installation notes, or independent measurements of how closely it reproduces Windows&\#x27; output.

hackernews · ThrowNotAway · Nov 25, 11:34 · [Discussion](https://news.ycombinator.com/item?id=50641171)

**「Background」** Loudness Equalization is a Windows Sound control-panel enhancement, but the behavior being ported also includes the shared-mode output limiter that audiodg.exe applies through CAudioLimiter in AudioEng.dll on every render device, after effects and before the endpoint. That stage sits inside the audio graph, so a PipeWire version has to be implemented as DSP modules and plugins rather than as a simple settings toggle.

**「Impact」** PipeWire users should treat the effect as loudness normalization with limiting rather than frequency-dependent equalization, since the supplied discussion warns that focused impulses or pure tones may be boosted. Comparing processed and unprocessed output is the practical check before relying on it.

**「Community discussion」** One commenter said Windows applies slight peak compression on shared-mode WASAPI, DirectSound, and MME playback through audiodg.exe and CAudioLimiter in AudioEng.dll, while WASAPI exclusive and ASIO bypass it. Others argued the effect is loudness normalization rather than equalization and warned that it can boost focused impulses or pure tones, while some questioned why reverse engineering was necessary or objected to reducing a composition&\#x27;s dynamic range.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoxorwr/pw-loudness-eq">GitHub - xoxorwr/pw-loudness-eq: Windows Loudness ...</a></li>
<li><a href="https://thedroidguy.com/how-bring-back-missing-loudness-equalization-option-1298431">How To Bring Back The Missing Loudness Equalization Option (2026)</a></li>
<li><a href="https://todayforai.com/en/items/art-7bb2d612-837">Windows Loudness Equalization Reverse-Engineered and Ported ...</a></li>

</ul>
</details>

**Tags**: `#audio`, `#reverse-engineering`, `#pipewire`, `#linux`, `#dsp`

---

<a id="item-tech-news-10"></a>
### [Essay argues LLM users still own code review](https://www.iankduncan.com/engineering/2026-11-19-smart-people-who-give-a-shit-use-tools) ⭐️ 6.0/10

An essay on iankduncan.com examines whether LLM coding tools are just another higher-level abstraction and argues that responsibility for reviewing the resulting code still rests with the engineer, not with “the model wrote it.” The accompanying Hacker News discussion challenges that framing and debates how LLM speed changes who ships more code. This is an opinion essay, not a release or measured study, so it provides no new tool, benchmark, or adoption data.

hackernews · matthewsinclair · Nov 25, 07:46 · [Discussion](https://news.ycombinator.com/item?id=50639698)

**「Background」** Programming debates have long treated new tools as higher-level abstractions—assembly to C, C to JavaScript—and the same framing is now applied to LLM-assisted coding. The essay’s discussion complicates that analogy: delegating a task such as writing TLA+ to model a race condition can move the engineer away from the expertise needed to judge the result.

**「Impact」** For engineering teams using LLM assistants, the practical consequence is that “the model wrote it” cannot serve as a review defense; a human still needs to verify the change. The thread supplies no defect-rate evidence, so that conclusion rests on the essay’s argument rather than measurement.

**「Community discussion」** Commenters disputed the essay’s abstraction analogy: anothaway argued that using an LLM is a different kind of activity from moving from assembler to C or C to JavaScript, while xnorswap argued LLMs may let engineers who skip extra verification out-ship those who take the time to check. chrisra described growing self-doubt about whether “the model wrote it” is a reasonable defense in code review.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50639698">Smart people who give a shit use tools | Hacker News</a></li>

</ul>
</details>

**Tags**: `#llm-coding`, `#software-engineering`, `#code-review`, `#ai-tools`, `#developer-productivity`

---

<a id="item-tech-news-11"></a>
### [Linux 7.4 reverts driver-bind taint patch after real-world conflicts](https://lwn.net/Articles/1103714/) ⭐️ 6.0/10

Linux kernel developers have reverted a patch, applied by Greg Kroah-Hartman early in the 7.4 merge window, that marked the kernel as tainted whenever user space manually bound or unbound a device driver to a device. The change was intended as a defense against a flood of spurious bug reports generated by fuzzers, but it interfered with real use cases and was removed after discussion. The episode highlights a need for better kernel interfaces to address the fuzzing problem without penalizing legitimate manual driver binding.

rss · LWN.net · Nov 25, 14:36

**「Earlier development」** Earlier coverage described the change as Linux 7.4&\#x27;s TAINT\_FORCED\_BIND \(flag Y\), which marked the kernel when user space wrote to the sysfs driver bind/unbind files as a way to reduce syzbot-generated reports from invalid test configurations. That coverage said the feature had been merged during the 7.4 cycle and was then reverted after a problem in the VFIO subsystem.

**「Impact」** Manual driver bind and unbind operations no longer change the kernel&\#x27;s taint state, so bug reports from systems using those operations will not carry that marker. The supplied evidence does not show a replacement mechanism, leaving the fuzzer-generated-report problem that motivated the patch unaddressed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.4-Drops-Taint-Bind">New Linux 7.4 Feature For Reducing AI Noise Already Reverted ...</a></li>
<li><a href="https://techaiwire.com/articles/linux-7-4-taint-forced-bind-syzbot-driver-bind-unbind/">Linux 7.4 TAINT_FORCED_BIND: new Y taint for bind/unbind</a></li>

</ul>
</details>

**Tags**: `#Linux kernel`, `#driver binding`, `#kernel taint`, `#fuzzing`, `#kernel interfaces`

---

<a id="item-tech-news-12"></a>
### [Anthropic&\#x27;s Claude Ship beta adds AI code review and approvals](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+Claude%E8%83%BD%E8%87%AA%E5%B7%B1%E6%89%B9%E4%BB%A3%E7%A0%81%E4%BA%86%EF%BC%818%E4%B8%AA%E6%9C%88%E5%89%8D%E8%BF%98%E8%AF%B4%E9%82%A3%E6%98%AF%E4%BA%BA%E7%9A%84%E4%BA%8B) ⭐️ 6.0/10

Anthropic reportedly launched a beta of Claude Ship, a workflow that adds a /ship command to Claude Code&\#x27;s CLI and desktop app to push code, open a PR, review it, and address failing checks and comments. It combines three roles: Code Review, which is generally available after a March launch and October rollout; PR Steward, a beta agent triggered by a GitHub label that fixes tests, conflicts, and review comments but cannot approve or merge; and Claude Approvals, which can approve routine changes that match team rules. Anthropic says merges still depend on user permissions and branch protection, and the article reports /ship is rolling out rather than universally available. Anthropic&\#x27;s own Claude Code team reported that in a repo about 90% written by Claude, merged PRs more than doubled from June to September while rollback rates fell more than 40%, and the share of PRs receiving actionable review comments rose from 16% to 54%.

rss · 新智元 · Nov 25, 07:34

**「Background」** Anthropic&\#x27;s code-review agent is not new: the article says Code Review arrived in March and became generally available in October, while Horizon&\#x27;s October 17 digest reported that Anthropic&\#x27;s Claude Code team was already running an AI-assisted review pipeline over roughly 30,000 pull requests a day and routing human attention to riskier changes. Claude Ship packages that review step with two beta agents, PR Steward and Claude Approvals, extending the workflow from commenting on a pull request to fixing it and making an approval decision under team policy.

**「Impact」** Teams adopting /ship still need branch protection and review rules that reserve merge rights, because PR Steward is explicitly barred from approving or merging and Claude Approvals is limited to routine changes that satisfy team policy. Developers can hand off test fixes and conflict resolution, but they must keep a separate approval path for non-routine changes and add the claude-pr-steward-watching label before PR Steward will act.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.dev/blog/solving-code-review-at-anthropic/">2026-10-17 — Claude Code team details AI-assisted code review workflow</a></li>
<li><a href="https://claude.com/resources/articles/introducing-claude-ship">Introducing Claude Ship | Claude by Anthropic</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#Claude`, `#AI code review`, `#developer tools`, `#AI coding`

---

<a id="item-tech-news-13"></a>
### [LeCun Accuses Amodei of Using AI-Risk Fears to Restrict Open Models](https://x.com/ylecun/status/2124550037912920090) ⭐️ 6.0/10

Yann LeCun posted on X on November 22 accusing Anthropic CEO Dario Amodei of stoking AI-danger narratives since the GPT-2 era in order to push for making open models illegal and preserve control. LeCun claimed Amodei left OpenAI because he could not obtain control there, and likened the approach to the Ottoman Empire&\#x27;s ban on Arabic printing, calling it &quot;a new form of medieval obscurantism.&quot; The item is a brief secondary summary of the social-media post, so the characterization of Amodei&\#x27;s motives and policy aims is LeCun&\#x27;s allegation rather than a verified account. LeCun, a 2018 Turing Award winner for convolutional neural networks, left Meta in November 2025 after 12 years as chief AI scientist and founded AMI Labs, where he is executive chairman.

telegram · zaihuapd · Nov 25, 01:30

**「Background」** LeCun&\#x27;s post was a reply in an X thread framing the open-versus-closed model debate, and it targets a standing dispute in AI policy: whether publishing open weights is inherently dangerous or mainly a competitive matter. Horizon&\#x27;s November 8 digest summarized a New York Times profile that traced Amodei&\#x27;s roots in the rationalist and effective-altruism communities and described a drive to control AI development — the context LeCun&\#x27;s control accusation addresses, though the profile does not establish that Amodei&\#x27;s safety claims are insincere.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/dotey/status/2119191652770226525">2026-11-08 — NYT profile of Anthropic CEO Dario Amodei: rationalist/EA roots and drive to control AI</a></li>
<li><a href="https://officechai.com/ai/dario-amodei-hypes-ai-dangers-so-that-open-models-are-made-illegal-and-he-can-stay-in-control-yann-lecun/">Dario Amodei Hypes AI Dangers So That Open Models Are Made ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open source`, `#AI safety`, `#industry debate`, `#Yann LeCun`

---

<a id="item-tech-news-14"></a>
### [OpenAI positions cybersecurity as bigger than coding, expands GPT-6 Cyber access](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 6.0/10

OpenAI is framing cybersecurity as its next growth engine and potentially a larger business than coding. CFO Sarah Friar said outside estimates putting the cybersecurity market above $300 billion are still far too low, and President Greg Brockman said cybersecurity will become a bigger segment for OpenAI than coding, according to The Information. The company has released GPT-6 Cyber for security research and is expanding its trusted-access program, Daybreak, which as of September covered thousands of vetted defenders and roughly 2,000 approved organizations and workspaces for vulnerability discovery, codebase analysis and binary reverse engineering. The report notes that competition with Anthropic and Google, and the path to scaled commercialization, remain unclear.

telegram · zaihuapd · Nov 25, 04:51

**「Earlier limited rollout」** Horizon&\#x27;s November 6 digest reported that OpenAI had launched GPT-6 Cyber for security research and initially limited access to some Daybreak Red customers, while saying it would broaden availability over time. The latest report&\#x27;s focus on a wider Daybreak trusted-access program therefore describes the next stage of that same rollout.

**「Impact」** Because Daybreak access runs through identity verification and organizational approval, security teams that want GPT-6 Cyber capabilities must be vetted rather than self-serve, and the reported ~2,000 approved organizations define the current practical limit of adoption. The market-size and &quot;bigger than coding&quot; figures are vendor assertions about future opportunity, not measured revenue.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/OpenAI/status/2118390190246879554">2026-11-06 — OpenAI 发布 GPT-6 Cyber 安全模型</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#cybersecurity`, `#AI security`, `#enterprise AI`, `#market strategy`

---

<a id="item-tech-news-15"></a>
### [Asian data centers seek U.S. buyers as Nvidia export loophole tightens](https://www.bloomberg.com/news/articles/2026-11-25/asia-data-centers-sound-out-us-clients-to-replace-china-demand) ⭐️ 6.0/10

Asian data-center operators are courting U.S. customers for excess AI compute after the U.S. government tightened a loophole that had allowed Chinese technology companies to obtain Nvidia’s most advanced chips, Bloomberg reported. Ronit Jain, chief executive of Liquid Compute, said new restrictions on exports of advanced AI accelerators to the region are hitting data-center providers that had expected to rent capacity to Chinese customers. The report did not specify the rule change, the companies affected, or the scale of the excess capacity.

telegram · zaihuapd · Nov 25, 11:35

**「The remote-access loophole」** U.S. export rules already blocked Chinese firms from buying advanced Nvidia chips directly, but they could still legally rent that compute from data centers in third-party countries such as Malaysia, Singapore, and Thailand; Horizon&\#x27;s November 12 digest reported that the Commerce Department was finalizing a rule extending restrictions to those countries to close the remote-access route. Commerce moved to close the loophole in mid-November, the first policy response to the scandal that led Nvidia CEO Jensen Huang to resign. The shift had already reached individual deals: Horizon&\#x27;s November 5 digest reported that Oracle canceled a roughly $7 billion, five-year AI chip lease with Tencent — about 100,000 advanced chips in Southeast Asian data centers — after U.S. officials raised concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theinformation.com/articles/commerce-department-finalizing-long-awaited-ai-remote-access-rule">2026-11-12 — US Readies Rule Barring Remote AI Chip Access for Chinese Firms</a></li>
<li><a href="https://www.tradingview.com/news/seekingalpha:e51e68f4d094b:0-oracle-cancels-7b-ai-chip-lease-with-tencent-amid-us-concerns-ft/">2026-11-05 — Oracle cancels $7 billion AI chip lease with Tencent</a></li>
<li><a href="https://www.nytimes.com/2026/11/16/us/politics/trump-china-ai-chip-loophole.html">Trump Administration Moves to Close A.I. Chip Loophole Ahead of...</a></li>
<li><a href="https://www.cnbc.com/2026/11/16/nvidia-commerce-china-lutnick.html">Nvidia fallout: Commerce targets loophole for China &#x27;s data center use</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#export controls`, `#data centers`, `#Nvidia`, `#compute markets`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly ROCm 7.2 Wheels for AMD Instinct](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels of LMCache, built from the dev branch on 2026-11-25 for AMD Instinct gfx942/gfx950 and ABI-matched to the upstream vLLM ROCm OpenAI image \(torch 2.13, cp312\).

github · github-actions\[bot\] · Nov 25, 10:04

**「Problem solved」** LMCache sits in the KV-cache layer for vLLM inference serving. On AMD ROCm, installing it into the vLLM container depends on matching the wheel&\#x27;s ABI to the container&\#x27;s Python and torch versions. These prebuilt wheels are ABI-matched to the upstream vLLM ROCm OpenAI image, giving AMD users a packaged install path instead of a source build. The item describes no feature, performance, or architecture changes; it is a nightly packaging release.

**「Background」** LMCache sits in the KV-cache layer of the LLM inference stack: vLLM documents using it with vLLM v1 for KV-cache offloading, disaggregated prefill, and cache sharing \[tool-1-1\], and it is also described as a KV-cache layer for vLLM and SGLang at production scale \[tool-1-2\]. Packaging for accelerated backends is therefore part of serving infrastructure, not just library distribution.

This \`nightly-rocm\` artifact is a routine automated build from the \`dev\` branch \(\`0.5.9.dev50+rocm7.2\`\), not a described feature or performance release. Its ecosystem role is to provide AMD users with wheels ABI-matched to the upstream \`vllm/vllm-openai-rocm\` image \(torch 2.13, cp312\) for gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\); AMD&\#x27;s ROCm documentation likewise distinguishes those CDNA3 and CDNA4 device families for workload tuning \[tool-2-1\]. The practical change is ROCm 7.2 compatibility and distribution, not new LMCache capability.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/examples/disaggregated/lmcache/">LMCache Examples - vLLM</a></li>
<li><a href="https://hivebook.wiki/wiki/lmcache-kv-cache-layer-for-vllm-and-sglang-at-production-scale">Hivebook - The Knowledge Base for AI Agents</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.2.4/how-to/rocm-for-ai/inference-optimization/workload.html">AMD Instinct MI300 Series / MI350 Series workload optimization</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#ROCm`, `#vLLM`, `#AMD Instinct`, `#inference serving`, `#nightly release`, `#wheels`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly RBLN NPU Wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 5.0/10

LMCache published a nightly wheel for Rebellions RBLN NPUs, built from \`dev\` against torch-rbln 0.12.0 and torch 2.13.0+cpu. It adds platform-specific installation support while leaving torch-rbln, rebel-compiler, and the RBLN driver host-owned rather than bundling them.

github · github-actions\[bot\] · Nov 25, 10:04

**「Problem Solved」** The release addresses distribution rather than inference performance: running LMCache on Rebellions RBLN NPUs requires a platform-specific build and an existing host environment with the RBLN SDK and driver. By publishing an RBLN wheel that excludes torch-rbln, rebel-compiler, and the RBLN driver, it avoids bundling host-owned dependencies and lets users install LMCache into that environment.

**「Ecosystem context」** LMCache is a KV-cache management layer for LLM inference that stores and reuses KV states across requests and serving engines, targeting repeated prefill work and long-context serving efficiency \(tool-1-1, tool-1-2\). This nightly \`rbln\` wheel extends that stack to Rebellions RBLN NPUs by providing a platform-specific install artifact built from \`dev\` against torch-rbln 0.12.0 \(torch 2.13.0+cpu\). The update is primarily about packaging and backend reach rather than a core KV-cache feature: it gives RBLN users an installation path while keeping torch-rbln, rebel-compiler, and the RBLN driver host-owned instead of bundled.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://github.com/nextunicorn2026/LMCache-HGI">nextunicorn2026/ LMCache -HGI: LMCache : Supercharge Your LLM ...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#nightly build`, `#packaging`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Court Filings Allege Commerce Department Pressured Intel Into Giving U.S. Government 10% Stake](https://www.wired.com/story/inside-trumps-demands-to-another-chips-ceo/) ⭐️ 9.0/10

Court filings reported by WIRED show a Commerce Department lawyer told Intel&\#x27;s chief financial officer in an August 2025 call that this was not a negotiation and that the board could refuse but would face unpredictable consequences. Days later Intel&\#x27;s board transferred the shares, and President Trump announced the U.S. government owned and controlled 10% of Intel without paying for it — a stake reported to be worth about $11 billion.

telegram · zaihuapd · Nov 25, 13:25

**「Background」** The demand came as the US government under President Donald Trump took equity stakes in chipmakers, including the 10% Intel holding announced in 2025; Trump has since said he has not ruled out a similar stake in Nvidia.

**「Impact」** Intel shareholders are the directly affected group: a derivative suit has already been filed challenging the governance implications of the U.S. government’s roughly 9.9% stake, giving investors a legal venue to scrutinize the board’s decision.

<details><summary>References</summary>
<ul>
<li><a href="https://tass.com/economy/2224325">Trump says US could acquire stake in Nvidia - Business... - TASS</a></li>
<li><a href="https://www.dandodiary.com/2026/03/articles/shareholders-derivative-litigation/intel-derivative-suit-tests-governance-implications-of-government-equity-stakes/">Intel Derivative Suit Tests Governance Implications of ...</a></li>

</ul>
</details>

**Tags**: `#英特尔`, `#美国政府`, `#股权`, `#半导体`, `#产业政策`

---

<a id="item-finance-news-2"></a>
### [SpaceX and Tesla reportedly weigh $3.5 trillion all-stock merger](https://thenextweb.com/news/spacex-tesla-merger-five-directors-special-committees) ⭐️ 8.0/10

SpaceX and Tesla have reportedly set up special committees of five directors each to explore a $3.5 trillion all-stock merger, with a goal of reaching a deal by year-end, according to unnamed people cited in reports. The talks are described as early and not close to agreement, and the committees would still need to set an exchange ratio, win shareholder support and address litigation risk from Elon Musk&\#x27;s past deals.

telegram · zaihuapd · Nov 25, 00:41

**「Background」** A special committee is a board group formed to negotiate and vet a deal; the report says these committees must set the share-exchange ratio, win shareholder support and guard against investor lawsuits tied to Elon Musk’s earlier deals.

**「Who would be affected」** If the talks advance, Tesla&\#x27;s public shareholders would be the directly affected group: the share-exchange ratio would determine how much of the combined company they own, and Elon Musk&\#x27;s roughly 85% voting power at SpaceX versus about 20% at Tesla would shape how any deal is approved, according to Reuters and Fortune reporting.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/legal/government/musks-public-endorsement-spacex-tesla-deal-may-throw-wrench-talks-2026-10-22/">EXCLUSIVE: Musk’s public endorsement of SpaceX-Tesla deal may ...</a></li>
<li><a href="https://fortune.com/2026/10/22/biggest-hurdle-spacex-merger-tesla-elon-musk-shareholders/">The biggest hurdle to a SpaceX merger with Tesla isn’t Elon ...</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#SpaceX`, `#merger`, `#corporate governance`, `#Elon Musk`

---

<a id="item-finance-news-3"></a>
### [US Plans New Section 301 Tariffs on 14 Trading Partners, Including China and EU](https://www.cnbc.com/2026/11/25/us-tariffs-trump-section-301.html) ⭐️ 8.0/10

The US government is reportedly preparing new tariffs under Section 301 of the 1974 Trade Act on 14 trading partners — among them China, the EU, Japan and India — with China facing an additional 20 percentage points on top of the 25% duties imposed in 2018, and a possible 40% rate if Beijing does not honor the trade truce reached in Busan, South Korea, in October 2025, according to CNBC. The 14 partners have been notified, and rates are set country by country rather than as a single blanket level.

telegram · zaihuapd · Nov 25, 13:59

**「Background」** The proposal follows USTR’s March 2026 self-initiated Section 301 investigations into manufacturing overcapacity in 16 economies and a one-year US-China trade truce agreed in Busan in October 2025.

**「Impact」** Because the duties would be collected on goods entering the US, American importers and manufacturers that buy the affected subsidized manufactured goods would pay more at the border, while no implementation date or country-by-country rate schedule has been announced.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hklaw.com/en/insights/publications/2026/03/ustr-launches-awaited-section-301-investigations">USTR Launches Awaited Section 301 Investigations of 16 Economies...</a></li>
<li><a href="https://www.cfr.org/articles/united-states-and-china-agree-trade-truce">United States and China Agree to Trade Truce | Council on ...</a></li>

</ul>
</details>

**Tags**: `#US tariffs`, `#Section 301`, `#global trade`, `#China-US trade`, `#trade policy`

---

<a id="item-finance-news-4"></a>
### [SpaceX 放弃 7.38 亿美元联邦宽带补贴，转而免费提供 Starlink 设备](https://x.com/SawyerMerritt/status/2125314062997467640) ⭐️ 7.0/10

据报道，SpaceX 已同意放弃 7.38 亿美元的美国联邦宽带补贴，改为根据美国国家电信与信息管理局（NTIA）的 BEAD 计划，向符合条件的美国家庭免费提供 Starlink 终端；该计划下的联邦拨付金额为 0 美元。报道称，该协议要求提供至少 100 Mbps 下载和 20 Mbps 上传速度、低价套餐以及 10 年服务承诺，同时豁免大部分财务审计和行政报告义务，但仍须接受网络性能测试。

telegram · zaihuapd · Nov 25, 02:17

**「Background」** BEAD is a federal program that subsidizes broadband construction in underserved areas, and SpaceX had been set to receive about $738 million under it. The Commerce Department approved this unusual swap — forgoing the money in exchange for free hardware — after some states had already signed broadband buildout contracts with SpaceX, according to news reports.

**「Who is affected」** Eligible households in BEAD-subsidized areas would receive Starlink terminals at no cost and a low-cost monthly plan, while the federal government would record no BEAD payment for those connections.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yahoo.com/news/politics/articles/spacex-feds-well-offer-starlink-181617359.html?fr=sycsrp_catchall">SpaceX to Feds: We&#x27;ll Offer Starlink for Free in BEAD Areas ...</a></li>
<li><a href="https://qz.com/spacex-738-million-broadband-grants-free-starlink-hardware-112526">SpaceX is forgoing about $738 million to offer free Starlink ...</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starlink`, `#BEAD`, `#宽带补贴`, `#美国电信政策`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Dario Amodei Denies Anthropic Wants to Hand Decision-Making to Superintelligence](https://x.com/dotey/status/2125718634190508388) ⭐️ 7.0/10

Axios published an exclusive report citing unnamed people saying Anthropic internally holds a common view that AI may eventually become powerful enough that humans should cede some decision-making authority to superintelligent systems, and that doing so would often be the right choice. Critics, according to the report, see this as a slippery slope toward abandoning human free will. Axios cited past remarks by Anthropic CEO Dario Amodei, including his 2024 essay “Machines of Loving Grace” and a February 2026 CBS interview, and quoted rival AI leaders Sam Altman, Alexandr Wang, and Dean Ball criticizing similar ideas without naming Anthropic. An Anthropic spokesperson told Axios that Amodei has repeatedly advocated human control over AI and that the company trains Claude not to undermine human oversight.

Amodei responded on November 25 with a long post denying that he wants to hand human self-determination to AI, calling the idea “absurd.” He separated two questions: who governs society, and how far specific tasks should be delegated to AI. On governance, he said AI must be managed through legitimate democratic processes and that handing governance to AI would be a “bad idea,” drawing an analogy to arguments for authoritarian rule. He cited his past writings and interviews, including sections of “Machines of Loving Grace” and a January essay, as well as a September CBS interview, as evidence of his support for democratic oversight of AI.

On task automation, Amodei said his view is mixed: many uses are worthwhile and could save lives, but he identified four limits—recursive self-improvement, severe unemployment from end-to-end automation, risks in using AI for safety-alignment research, and things people simply want to do themselves. He cited Anthropic’s November 2 IPO prospectus update, which said the company does not expect to be able to safely let Claude fully autonomously design and build next-generation frontier models without effective human oversight and understanding, and which said internal estimates suggest future models may “soon” meet the company safety policy’s threshold for major AI acceleration.

Amodei also argued that other AI companies broadly share his views on which tasks should be automated, and called claims that he differs on autonomous weapons “absurd.” He said Anthropic refused Pentagon conditions that would have removed limits on fully autonomous weapons and mass surveillance of Americans, and that the company was designated a supply-chain risk by Defense Secretary Hegseth as a result; he said no other AI company had made such a stand. He criticized unnamed AI CEOs for “vibes-based commercial and political positioning” and for slogans about human control and agency without product differences or serious engagement with the underlying problems. Axios’s claim about Anthropic’s internal views relies entirely on unnamed sources; Amodei’s post addressed his own position and did not respond to that specific claim, and the assertion that no other company refused the autonomous-weapons conditions is his own.

twitter · 宝玉 · Nov 25, 22:29

**「Background: the Anthropic AI-control dispute」** The post by 宝玉 summarizes a dispute that unfolded after Axios published a report on Nov. 25, 2026, under the headline “Competitor AI leaders push back on Anthropic’s vision of handing over human control to AI.” Axios, citing unnamed sources, said a common view inside Anthropic held that AI would eventually become powerful enough that humanity should hand some decision-making power to superintelligence, and that doing so would often be right. Critics described that as a slippery slope toward forfeiting free will. Axios supported the framing with past Amodei material: his 2024 essay “Machines of Loving Grace,” which imagined an economy in which AI allocates resources according to what AI systems deem worthy of reward; a February 2026 CBS interview in which he discussed autonomous weapons; and an old slide from litigation describing Anthropic’s vision as a “utopia governed by a god in a box.” The report also quoted OpenAI CEO Sam Altman on Nov. 4, Meta chief AI officer Alexandr Wang on Nov. 22, and OpenAI’s Dean Ball, who described a “silent consensus” in which humanity hands companies and governments to machines. Axios said none of them named Anthropic. An Anthropic spokesperson told Axios that Amodei has argued publicly for human control of AI and that the company trains Claude not to undermine human oversight \[tool-2-1\].

In a long X post on Nov. 25, Amodei denied advocating that humans surrender free will to AI, calling the idea absurd. He separated two questions: who governs society, and how far specific tasks should be delegated to AI. On governance, he said AI must be governed through legitimate democratic processes and that handing governance to AI is a “bad idea,” comparing the argument to historical justifications for dictatorship. He cited sections of “Machines of Loving Grace,” a January essay, and a September CBS interview in which he said he would accept some form of joint oversight of AI by democratically elected governments. On specific tasks, he said automation is often worth doing and can save lives, but identified four limits: recursive self-improvement, in which AI designs the next generation of AI; severe unemployment from end-to-end automation; caution in using AI for safety-alignment research; and tasks people want to do themselves even if AI does them better. He also argued that other AI companies share his basic position on automation, and that singling him out over autonomous weapons is “quite absurd,” citing Anthropic’s refusal to accept the Pentagon’s removal of two restrictions and the resulting supply-chain-risk designation by Defense Secretary Hegseth. That account is Amodei’s own. Axios’s claim about internal Anthropic views rested on unnamed sources, and Amodei’s post addressed his own position rather than that sourcing \[tool-2-3\].

No community comments were supplied with the item, so no public reaction can be summarized here. The immediate discussion is the exchange between Axios’s reporting and Amodei’s rebuttal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.axios.com/2026/11/25/anthropic-ai-human-control-debate-free-will">AI leaders push back on Anthropic vision of ... - Axios</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-ceo-pushes-back-axios-184139218.html?fr=sycsrp_catchall">Anthropic CEO pushes back on Axios reporting on AI and free will</a></li>

</ul>
</details>

**Tags**: `#AI governance`, `#Anthropic`, `#Dario Amodei`, `#Axios`, `#AI safety`, `#OpenAI`, `#Meta`

---

<a id="item-twitter-news-2"></a>
### [Consumer AI agents face a unit-economics reckoning](https://x.com/venturetwins/status/2125697685818913166) ⭐️ 7.0/10

In a post on X, Justine Moore \(@venturetwins\) argues that consumer AI agents are entering a &quot;sink-or-swim&quot; phase. Many finally have demand, but most have not worked out the economics. Companies want to sustain viral growth, so many are not charging users, while costs for LLMs, browser use, and voice calls accumulate. Moore says many consumer agent companies she has spoken with spend $15–50+ per user per month, with much higher costs for power users.

She notes that taking a cut of payments facilitated by agents could make sense, but the ecosystem is not mature enough to drive meaningful revenue. Raising money to fund the burn is also difficult for companies outside the top tier, especially while competing with deep-pocketed firms such as Meta that can spend billions.

Moore expects a reckoning: consumer agent companies will have to optimize their infrastructure, likely through third parties, and end users will stop getting so much for free.

twitter · Justine Moore · Nov 25, 21:06

**「Background」** Justine Moore’s post frames consumer AI agents as reaching a difficult transition: demand has arrived, but the business model has not caught up. She says many companies are prioritizing viral growth and free access while absorbing the costs of LLMs, browser use, and voice calls, with spending of $15–50+ per user per month and more for power users.

Moore argues that taking a cut of payments facilitated by agents could make sense, but the ecosystem is not mature enough yet to generate meaningful revenue. She also points to a funding gap: outside the top players, it is hard to raise money to cover the burn while competing with deep-pocketed companies such as Meta.

Her expectation is a reckoning in which consumer agent companies invest in optimizing infrastructure, likely through third parties, and end users receive less for free. No community comments were available with the source material.

**Tags**: `#AI agents`, `#consumer AI`, `#unit economics`, `#startups`, `#VC`, `#LLM costs`

---