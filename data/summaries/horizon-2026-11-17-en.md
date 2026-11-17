# Horizon Daily - 2026-11-17

> From 85 items, 25 important content pieces were selected

---

**Technology News**
1. [vLLM v0.34.0 removes Model Runner V1 and changes KV cache defaults](#item-tech-news-1) ⭐️ 8.0/10
2. [Jiff 1.0 released as a new Rust datetime library](#item-tech-news-2) ⭐️ 8.0/10
3. [Patch series proposes a third futex class, &quot;futex PING&quot;, for Linux](#item-tech-news-3) ⭐️ 7.0/10
4. [Marimba: frozen Qwen3-ASR encoder answers typed audio queries](#item-tech-news-4) ⭐️ 7.0/10
5. [duetto steers pretrained music transformer at sampling time for live jazz](#item-tech-news-5) ⭐️ 7.0/10
6. [Tencent Hunyuan Releases Hy4 Flash, a Cheaper Multimodal MoE Model](#item-tech-news-6) ⭐️ 7.0/10
7. [US and Nine Partners Sign San Francisco Declaration on AI Supply-Chain Security](#item-tech-news-7) ⭐️ 7.0/10
8. [Amazon: Artex-driven AI agents stole API keys to fund model use](#item-tech-news-8) ⭐️ 7.0/10
9. [Carnegie Mellon launches CS Learn with free full-semester CS lectures on YouTube](#item-tech-news-9) ⭐️ 6.0/10
10. [Report Claims Windows 11 Telemetry Covers Coding Agents and Developer Tools](#item-tech-news-10) ⭐️ 6.0/10
11. [TRMNL announces Frame, a 31.5-inch color ePaper display](#item-tech-news-11) ⭐️ 6.0/10
12. [Microsoft blames email outage on defect from July fix](#item-tech-news-12) ⭐️ 6.0/10
13. [Apple and OpenEvidence launch 200k-person health AI use study](#item-tech-news-13) ⭐️ 6.0/10
14. [Apple Intelligence enters beta on China-market iPad and Mac with Siri usage caps](#item-tech-news-14) ⭐️ 6.0/10

**AI Open Source Projects**
1. [vLLM v0.34.0: Extensible KV Cache by Default, Model Runner V1 Retired](#item-ai-projects-1) ⭐️ 9.0/10
2. [LMCache Nightly Wheel for Rebellions RBLN NPU](#item-ai-projects-2) ⭐️ 6.0/10
3. [LMCache releases nightly ROCm wheels](#item-ai-projects-3) ⭐️ 5.0/10
4. [LMCache nightly build: CUDA 13.0 wheels](#item-ai-projects-4) ⭐️ 5.0/10

**Financial News**
1. [China&\#x27;s October retail sales, industrial output and investment all miss forecasts](#item-finance-news-1) ⭐️ 8.0/10
2. [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has ties to the chipmaker](#item-finance-news-2) ⭐️ 8.0/10
3. [英特尔及 CEO 陈立武遭股东集体诉讼](#item-finance-news-3) ⭐️ 8.0/10
4. [Nvidia CEO Exit and Congress Risk Could Reshape AI Trade, ETF Experts Say](#item-finance-news-4) ⭐️ 7.0/10
5. [China Pork Prices Fall to Near 10-Year Low](#item-finance-news-5) ⭐️ 7.0/10
6. [China&\#x27;s foreign direct investment turns to net outflow in the third quarter](#item-finance-news-6) ⭐️ 7.0/10

**Twitter News**
1. [Lenny Rachitsky&\#x27;s prompt for wiring an AI bot to a user-owned Anthropic API key](#item-twitter-news-1) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vLLM v0.34.0 removes Model Runner V1 and changes KV cache defaults](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 8.0/10

vLLM v0.34.0 removes Model Runner V1 so Model Runner V2 is the only GPU runner and makes extensible KV cache sizing the default, with \`gpu\_memory\_utilization\` now defaulting to 1.0. The release changes the default \`--block-size\` from 16 to 64, drops ROCm 7.2 artifacts in favor of ROCm 10.0, requires \`huggingface\_hub &gt;= 2.0.0\`, and removes QuTLASS/\`fp\_quant\`, Marlin W4A8, and Keye-VL support. It adds 10 models, including Mistral Large 4, MiniMax-M3.1-Flash, and NVIDIA Nemotron-3.5-Transcribe. The release notes report speedups on Blackwell and MI355X, such as up to 1.95x decode for Step5 NVFP4 MoE on 4xGB200 and 1.6x output throughput for GLM-5.3-Flash, but these are vendor-reported figures rather than independently verified results.

github · khluu · Nov 16, 23:22

**「Background」** vLLM is a pre-1.0 project on a frequent release cadence: Horizon&\#x27;s October 19 digest reported v0.32.0, which added a \`/v1/systemone\` endpoint, generic HF tool and reasoning parsers, and broader low-precision KV cache support. Two minor releases later, v0.34.0 continues the KV-cache work by changing how the cache is sized rather than its precision, while removing the Model Runner V1 GPU path that earlier releases still shipped as an option.

**「Impact」** Upgrading users must remove \`VLLM\_USE\_V2\_MODEL\_RUNNER=0\`, since vLLM now fails at startup, and can preserve old defaults with \`--block-size 16\` plus either \`--gpu-memory-utilization 0.9\` or \`--no-enable-extensible-kv-cache\`. ROCm users must move to the ROCm 10.0 wheels and images, while Marlin W4A8 users must switch to \`--quantization humming\` with \`VLLM\_HUMMING\_INPUT\_QUANT\_CONFIG\`; the release notes also warn that the new KV cache default can raise per-token decode latency by 6-18% on some H200 models at concurrency 128.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases/tag/v0.32.0">2026-10-19 — vLLM 0.32.0 adds systemone endpoint, generic parsers, low-precision KV cache</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#open source`, `#performance optimization`, `#breaking changes`

---

<a id="item-tech-news-2"></a>
### [Jiff 1.0 released as a new Rust datetime library](https://burntsushi.net/jiff/) ⭐️ 8.0/10

Jiff 1.0, a datetime library for Rust by burntsushi, has been released. It enters a space already served by established crates such as chrono, and the launch drew community discussion about API design, time scales, and ecosystem adoption. The supplied material does not detail compatibility guarantees, migration paths, or the full set of supported time scales.

hackernews · burntsushi · Nov 16, 16:53 · [Discussion](https://news.ycombinator.com/item?id=50519744)

**「Background」** Jiff has been developed in the open for some time: its GitHub releases page lists an early release dated February 10, 2025, and the project&\#x27;s own repository noted that Jiff 1.0 had originally been planned for summer 2025 but that the deadline had slipped, with no timeline announced at that point \(tool-2-1, tool-2-2\). This release therefore marks the first stable 1.0 version of a crate that had previously circulated only as pre-1.0 code, arriving in an ecosystem where chrono has long been the established datetime library — a history raised in the community thread by chrono&\#x27;s former maintainer.

**「Impact」** For Rust developers evaluating datetime crates, Jiff 1.0 adds a newer alternative to chrono, but the comments frame adoption as a tradeoff: Jiff may offer a more considered API, while chrono&\#x27;s long stability is why teams already depend on it. No compatibility or migration details are available in the supplied material, so teams considering a switch would need to verify them independently.

**「Community discussion」** A former chrono maintainer said in comments that the crate&\#x27;s stable API made improvements difficult and contributed to burnout, while another commenter praised Jiff&\#x27;s documentation for openly saying Jiff isn&\#x27;t always the right tool. Other commenters hoped Jiff would see wider ecosystem adoption over chrono and asked how it handles time scales such as TAI and UT1.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/BurntSushi/jiff">GitHub - BurntSushi/jiff: A datetime library for Rust that ...</a></li>
<li><a href="https://github.com/BurntSushi/jiff/releases">Releases · BurntSushi/jiff - GitHub</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#datetime`, `#libraries`, `#API design`, `#time zones`

---

<a id="item-tech-news-3"></a>
### [Patch series proposes a third futex class, &quot;futex PING&quot;, for Linux](https://lwn.net/Articles/1102988/) ⭐️ 7.0/10

An LWN introduction describes a patch series from Suleiman Souhlal that would add a third futex class to the Linux kernel, named &quot;futex PING&quot; and described as &quot;priority inheritance next generation&quot;. Futexes currently come in two basic variants, and the implementation has grown more complex over the years even as users keep asking for faster user-space fast mutexes. This is a posted patch proposal under review, not a merged or shipped kernel capability, and the available excerpt gives no measured performance results, merge status, or target kernel version.

rss · LWN.net · Nov 16, 15:06

**「Background」** Futexes let user space build fast mutexes on a kernel wait/wake mechanism, and Linux has long offered two variants: plain hashed futexes and priority-inheritance \(PI\) futexes built on rtmutexes, which exist to keep a high-priority task from being blocked indefinitely by a lower-priority lock holder. Souhlal&\#x27;s series adds a third class, FUTEX\_PING — &quot;priority inheritance next generation,&quot; a name attributed to Steven Rostedt — which differs from classic PI futexes by being stealable from the top waiter and by using proxy execution internally instead of rtmutexes. It first appeared as an RFC on LKML in September 2026, with patches covering a stealable PI futex, the switch to proxy execution, PING handoff, and waking the donor on unlock.

**「Impact」** For real-time and systems developers, the proposal&\#x27;s design change matters more than the patch itself: the RFC would trade strict priority-inheritance handoff for lock stealing and proxy execution, so any eventual adoption would alter behavior for workloads that currently rely on priority inheritance. Coverage of the series reports that maintainers consider the approach premature and flag lockup risks, meaning current futex priority-inheritance semantics remain the safe assumption until the patch is reworked or accepted.

<details><summary>References</summary>
<ul>
<li><a href="https://lkml.org/lkml/2026/9/17/386">LKML: Suleiman Souhlal: [RFC PATCH 00/12] FUTEX_PING: A ...</a></li>
<li><a href="https://freenode.net/article/google-floats-stealable-ping-futexes-for-linux">Google floats stealable PING futexes for Linux · freenode</a></li>
<li><a href="https://lwn.net/Articles/1094994/">FUTEX_PING: A stealable futex using Proxy Execution. - lwn.net</a></li>
<li><a href="https://freenode.net/article/google-floats-stealable-ping-futexes-for-linux">Google floats stealable PING futexes for Linux · freenode</a></li>

</ul>
</details>

**Tags**: `#Linux kernel`, `#futex`, `#synchronization`, `#priority inheritance`, `#operating systems`

---

<a id="item-tech-news-4"></a>
### [Marimba: frozen Qwen3-ASR encoder answers typed audio queries](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Marimba is a speech question-answering system that takes a typed question about an audio window — yes/no, a choice, or a score — and returns a calibrated probability, using one frozen Qwen3-ASR-0.6B encoder pass per 8-second window; term queries such as &quot;was &\#x27;satellite&\#x27; said?&quot; are scored zero-shot from the decoder&\#x27;s greedy and 4-beam hypotheses and then Platt-calibrated, while turn-end, speaker-change, and speaker-count predictions come from small readouts on frozen layers 18 and 12. It was announced on Reddit as a follow-up to an earlier post and now ships with an arXiv preprint \(2611.18330\), code, Apache-2.0 weights on Hugging Face, and a pip package \(marimba-audio\). The author reports that on the same 1,000 public questions it matches or beats Qwen3-Omni \(30B-A3B\) on 6 of 9 tests, with 100% language ID on 300 FLEURS clips, speaker-change AUROC of 0.966–0.980 on AMI and VoxConverse \(above ECAPA\), and speaker count beating pyannote 3.1, while Qwen3-Omni remains better on Speech Commands. The stated caveats are that the turn-end readout was trained on Smart Turn data, making that row in-distribution, that turn-end reaches AUROC 0.930 against Smart Turn v3.2&\#x27;s 0.982 on Smart Turn&\#x27;s own test set \(0.716 vs 0.712 on ICSI\), and that no head generalizes to unseen tasks — all are at chance on CochlScene scene classification.

reddit · r/MachineLearning · /u/solanotodesch · Nov 16, 15:47

**「Background」** Marimba&\#x27;s frozen encoder is Qwen3-ASR-0.6B, Alibaba&\#x27;s compact open-weight speech recognition model published under Apache 2.0 with built-in language identification and streaming \[tool-2-2\]. Horizon&\#x27;s October 1 digest reported that Qwen-family models were the most common language backbone across more than 100 audio models, spanning ASR, TTS, and audio understanding, so reusing an ASR encoder as a shared backbone is an established pattern rather than a new one \[tool-1-1\]. The paper benchmarks against Qwen3-Omni-30B-A3B, a much larger any-to-any model that accepts audio, video, and text input \[tool-2-1\]\[tool-2-3\], as well as end-of-turn and diarization baselines such as Smart Turn v3, pyannote 3.1, and ECAPA-TDNN \[tool-3-2\].

**「Impact」** The practical trade-off of reusing one frozen 0.6B encoder with per-task readouts is that the reported parity with a 30B-A3B model holds only for tasks those readouts were built or trained for: turn-end underperforms a dedicated model on that model&\#x27;s own test set, and every head fails on out-of-distribution scene classification, so users should validate the heads and their calibration on their own audio before depending on the probabilities. The Apache-2.0 weights and the marimba-audio package make that evaluation possible without retraining the encoder.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1wuctrt/qwenfamily_llms_are_quietly_becoming_the_backbone/">2026-10-01 — Qwen-family LLMs dominate backbones in 100+ audio models survey</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3-omni">Qwen 3 - Omni - a Qwen Collection</a></li>
<li><a href="https://www.anchorterminal.com/tools/qwen3-asr-0-6b">Qwen 3 - ASR - 0 . 6 B review (2026): pricing, alternatives and grade C</a></li>
<li><a href="https://www.toolify.ai/ai-model/qwen-qwen3-omni-30b-a3b-instruct">Qwen 3 - Omni - 30 B - A 3 B -Instruct huggingface.co api &amp; Qwen... - Toolify</a></li>
<li><a href="https://arxiv.org/pdf/2609.29371">BanglaTurn: A Benchmark and Whisper-Based Model for End -of- Turn ...</a></li>

</ul>
</details>

**Tags**: `#speech recognition`, `#audio question answering`, `#model efficiency`, `#calibration`, `#Qwen3-ASR`

---

<a id="item-tech-news-5"></a>
### [duetto steers pretrained music transformer at sampling time for live jazz](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

A Reddit post introduces duetto, a real-time jazz partner for a MIDI keyboard that plays standards with a user as solo, comping, and walking bass, and takes a solo when the player stops. Instead of fine-tuning, it uses the pretrained Anticipatory Music Transformer as-is and controls generation at sampling time by masking disallowed notes and biasing likely ones, with phrases drawn from the Weimar Jazz Database. The author reports about 12 ms/note for the medium model and 18 ms/note for the large model on a 3080 Ti, and about 90 ms/note for the large model on a Jetson Orin Nano, with code free for noncommercial use. Reported limitations include drifting from the player, unpredictable responses, and a fragile balance between the model&\#x27;s own ideas and the rules; the post asks whether sampling-time steering can replace fine-tuning for symbolic music.

reddit · r/MachineLearning · /u/GGAllin43 · Nov 16, 09:19

**「Prior context」** Duetto steers the Anticipatory Music Transformer \(Thickstun et al., 2023\), an infilling model trained on the Lakh MIDI dataset that can generate or revise material around a given prompt, including accompaniment, rather than only continuing it autoregressively. Horizon&\#x27;s October 25 digest covered an earlier Duetto build that tracked the player&\#x27;s key, chord, and tempo and biased logits to suppress out-of-key notes, boost chord tones, and damp notes near the player&\#x27;s hands, and reported that it ran on a Jetson Orin. The current post adds phrase quoting from transcribed solos in the Weimar Jazz Database, separate solo, comping, and walking-bass roles, and a scheme that keeps roughly one second of music sampled ahead and resamples the unplayed portion when the player plays.

**「What this changes for builders」** Because the control lives in a rule layer over a frozen Anticipatory Music Transformer checkpoint rather than in fine-tuned weights, developers reusing duetto can retarget it to a new tune or style by editing masking and biasing rules instead of collecting and training on new performance data — but the author reports that the balance between model output and rules is fragile, so the tuning effort shifts from training to rule design. The author&\#x27;s reported ~90 ms/note on a Jetson Orin Nano indicates the system can run on embedded hardware rather than a desktop GPU, while the released code is free only for noncommercial use, which constrains anyone planning a commercial product.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1xe4pex/got_a_pretrained_music_transformer_to_jam_with_me/">2026-10-25 — Pretrained music transformer jams live via logit steering, no fine-tuning</a></li>
<li><a href="https://arxiv.org/abs/2306.08620">[2306.08620] Anticipatory Music Transformer - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#music generation`, `#transformers`, `#sampling-time steering`, `#real-time MIDI`, `#jazz`

---

<a id="item-tech-news-6"></a>
### [Tencent Hunyuan Releases Hy4 Flash, a Cheaper Multimodal MoE Model](https://mp.weixin.qq.com/s/5yBbf-ctYziM5r0i6Y17lA) ⭐️ 7.0/10

Tencent Hunyuan released Hy4 flash, a multimodal mixture-of-experts model with 224B total and 12B active parameters and a 1M-token context window. Tencent says it is slightly better than Hy4 preview overall and that WorkIndex cost per task is 1/13 of Hy4 preview and 1/20 of Hy4 — vendor claims not backed by independent benchmarks in the announcement. API pricing is ¥0.5 per million input tokens and ¥2 per million output tokens, falling to ¥0.02 on cache hits. The model is live on Tencent Cloud TokenHub, WorkBuddy, and Yuanbao, with an open-source release planned; WorkBuddy is free and API access is 50% off through November 30.

telegram · zaihuapd · Nov 16, 07:17

**「Background」** Hy4 flash is a cost-focused sibling of Tencent&\#x27;s Hy4 family: Horizon&\#x27;s November 5 digest reported that Tencent released Hy4 as an open-weight foundation model with 1M-token context, adapted with Tencent Interactive Entertainment Group for game development, while acknowledging a gap with top proprietary models on research-level mathematics and long-horizon coding. Third-party model listings date Hy4&\#x27;s release to early November 2026, describe it as a 770B-parameter open-weight Mixture-of-Experts system for coding, reasoning, and long-running agent tasks, and note that it added image understanding over the earlier Hy4 preview. Hy4 flash keeps the same 1M-context, multimodal approach and MoE design — in which only part of the parameter set is active per token — but scales down to 224B total and 12B active parameters, which is the basis for its lower per-task cost rather than a capability upgrade.

**「Impact」** Developers running high-volume, long-context, or multimodal workloads get a substantially cheaper option from Tencent&\#x27;s lineup, but the efficiency and quality figures are self-reported, so teams should benchmark Hy4 flash on their own tasks before migrating. The promised open-source release has no stated date, so self-hosting is not yet available.

<details><summary>References</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4">2026-11-05 — Tencent Hy4 Open-Weight Model Targets Game Development</a></li>
<li><a href="https://www.eesel.ai/blog/tencent-hy4">Tencent Hunyuan Hy 4 : specs, benchmarks , and pricing... | eesel AI</a></li>
<li><a href="https://lmspeed.net/model/hy4">Hy 4 API Pricing &amp; Benchmarks | LMSpeed</a></li>

</ul>
</details>

**Tags**: `#Tencent Hunyuan`, `#LLM release`, `#MoE`, `#API pricing`, `#multimodal`

---

<a id="item-tech-news-7"></a>
### [US and Nine Partners Sign San Francisco Declaration on AI Supply-Chain Security](https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/) ⭐️ 7.0/10

The United States and nine partner countries signed the San Francisco Declaration on November 15, affirming that economic security underpins national security and pledging joint protection of sensitive technologies and critical infrastructure in supply chains supporting superintelligence \(SI\). The other signatories are Australia, India, Israel, Japan, South Korea, Qatar, Singapore, the United Arab Emirates, and the United Kingdom. The declaration establishes five working groups covering innovation policy frameworks, SI applications in critical sectors, full-stack SI supply-chain collaboration, safe harbors and supply-chain security hubs, and SI safety and resilience. The text as reported is a declaration of intent rather than a binding agreement, and no implementation timelines, funding, or enforcement mechanisms were disclosed.

telegram · zaihuapd · Nov 16, 10:40

**「Background」** Horizon&\#x27;s October 5 digest reported that the White House had created a &quot;Super Intelligence Force&quot; task force led by Director of National Intelligence Jay Clayton with a 120-day deadline for a report on AI risks, and its November 7 digest reported that the Justice Department&\#x27;s own &quot;Super Intelligence Task Force&quot; \(SINTF\), authorized by an October 13 memorandum, had begun operating — earlier US moves that made &quot;superintelligence&quot; the operative term in federal AI policy before the concept was extended to allied supply-chain coordination. The State Department said the San Francisco Declaration was signed on November 15 at the Pax Silica Founders Retreat convened by Under Secretary of State for Economic Affairs Jacob Helberg.

**「Impact」** Because the declaration explicitly covers semiconductors and critical AI infrastructure, chipmakers, hardware suppliers and data-center operators working across the ten signatory economies — among them India, Japan, South Korea, Singapore and the UAE — should expect supply-chain security expectations to be coordinated through the five working groups rather than set independently by each government. Coverage of the pact describes the participants as &quot;Pax Silica partners&quot; that have agreed to treat the security of those technologies and the infrastructure behind them as a shared responsibility, but the declaration as reported carries no binding commitments, leaving the practical compliance path and timing for affected vendors undefined.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wsj.com/tech/ai/new-ai-task-force-to-report-on-risks-of-technology-after-public-and-industry-concerns-b6308bef">2026-10-05 — 美国成立“超级智能力量”，120 天内交 AI 风险报告</a></li>
<li><a href="https://www.theregister.com/ai-and-ml/2026/11/06/dojs-super-intelligence-task-force-up-and-running/5308074">2026-11-07 — 美司法部超级智能特别工作组正式运作</a></li>
<li><a href="https://www.investing.com/news/world-news/us-nine-nations-sign-san-francisco-declaration-on-ai-security-5028448">U.S., nine nations sign San Francisco declaration on AI security By...</a></li>
<li><a href="https://www.youtube.com/watch?v=MGSXBmm-Ok0">India Joins US-Led San Francisco Declaration : How It... - YouTube</a></li>
<li><a href="https://timesofindia.indiatimes.com/business/india-business/india-joins-us-led-alliance-to-secure-ai-supply-chains-amid-china-tech-rivalry/articleshow/135886669.cms">India joins US-led alliance to secure AI supply chains amid China tech...</a></li>
<li><a href="https://www.ft.com/content/3c2197fc-9618-4838-91e6-522ce1a96a22?syn-25a6b1a6=1">US and allies sign accord to protect AI supply chains from China</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#supply chain security`, `#geopolitics`, `#superintelligence`, `#international cooperation`

---

<a id="item-tech-news-8"></a>
### [Amazon: Artex-driven AI agents stole API keys to fund model use](https://cybernews.com/security/amazon-autonomous-cybercrime-artex-framework/) ⭐️ 7.0/10

Amazon says attackers used the open-source Artex penetration-testing framework to drive AI agents that stole API keys from internet-exposed LiteLLM and Dify applications, validated them, and pooled them to pay for additional large-model calls. The campaign ran from October 3 to November 5, when Amazon&\#x27;s MadPot decoy network disrupted it, the company said. Amazon attributed the operation to a China-related threat group with medium confidence, said not all listed targets were compromised, and notified potentially affected AWS customers.

telegram · zaihuapd · Nov 16, 13:00

**「Background」** Artex is an open-source framework for driving AI agents that Horizon&\#x27;s October 9 digest had already connected to attacks on South Korean financial institutions, citing a CrowdStrike assessment that attributed the activity to Chinese-speaking actors with medium confidence and left the attackers&\#x27; identity, affiliation, and breach scale unconfirmed. The campaign Amazon now describes targets a different class of victim: internet-exposed AI application platforms such as LiteLLM and Dify, which store upstream model-provider API keys in their configuration, making those keys the object of the theft and the currency for further LLM calls. Amazon&\#x27;s account rests on records it says it captured from the agents themselves, which is why the company characterizes its attribution only as medium confidence.

**「Impact」** For organizations running internet-exposed LiteLLM or Dify instances, stolen API credentials became a direct operating cost: they were pooled to fund further model use, and Amazon said it notified potentially affected AWS customers.

<details><summary>References</summary>
<ul>
<li><a href="http://xcai.pro/">2026-10-09 — CrowdStrike Reports Open-Source AI Tool ARTEX Used in South Korea Financial Attacks</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#autonomous agents`, `#API key theft`, `#cybercrime`, `#open-source tooling`

---

<a id="item-tech-news-9"></a>
### [Carnegie Mellon launches CS Learn with free full-semester CS lectures on YouTube](https://www.cs.cmu.edu/learn/) ⭐️ 6.0/10

Carnegie Mellon launched CS Learn, which is releasing full semesters of lectures from current CMU computer science courses for free on YouTube, with one course premiering each day this week and more courses planned for January. Phillip Compeau, who teaches in CMU&\#x27;s Griffin School of Computer Science and runs CS Learn, said students built tools to automate much of the production. The release is lecture-focused; courseware is expected next, so projects, notes, and feedback are not yet included.

hackernews · pcompeau · Nov 16, 20:43 · [Discussion](https://news.ycombinator.com/item?id=50522980)

**「Background」** Open courseware has a decades-long history: the project lead for CS Learn acknowledged that MIT launched its OpenCourseWare initiative roughly 25 years earlier, establishing a precedent for free university lecture materials online. Carnegie Mellon&\#x27;s effort adds current, full-semester computer science courses to that tradition.

**「Impact」** For self-learners, the uploads provide free access to current CMU lectures without enrollment, but the comments warn that lectures can fall flat without projects and a way to get feedback; those seeking a complete course experience may need to wait for the promised courseware.

**「Community Discussion」** Commenters broadly welcomed the resource but debated its sufficiency: one argued that learning fundamentals properly makes AI a power tool rather than a replacement, while another said lectures alone need videos, slides or notes, and projects, and noted that introductory courses often appear while graduate courses like compilers do not. Another commenter recalled Coursera and EdX initially democratizing university content before becoming profit-seeking.

**Tags**: `#computer-science-education`, `#online-learning`, `#open-courseware`, `#cmu`, `#youtube`

---

<a id="item-tech-news-10"></a>
### [Report Claims Windows 11 Telemetry Covers Coding Agents and Developer Tools](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 6.0/10

A post on xusheng.dev, discussed on Hacker News, reports that Windows 11 collects telemetry on which coding agents and developer tools a user runs. The supplied item contains only the headline and community comments, with no article text available, so the scope of the collection, the specific data fields, the mechanism used, and any Microsoft confirmation remain unverified. The claim should therefore be treated as a report rather than an established, independently measured finding.

hackernews · cwaffles · Nov 16, 22:58 · [Discussion](https://news.ycombinator.com/item?id=50524736)

**「Background」** Windows has long shipped diagnostic telemetry, and third-party projects such as the PowerShell-based WindowsTelemetryBlocker already exist specifically to block Windows 10/11 telemetry collection and disable related services \(tool-1-1\). The report in question comes from Xusheng Li, a software developer at Vector 35 who works on Binary Ninja and leads its debugger development, according to his site \(tool-1-3\). The supplied Horizon archive contains no earlier summary addressing Windows 11 telemetry on developer tools, so no direct predecessor report is available for this item.

**「Limited opt-out for developers」** Because Windows splits telemetry into required diagnostic data, which consumer Home and Pro users cannot fully disable, and optional diagnostic data, which they can, developers concerned about coding-agent and tool-usage collection have no documented per-application switch and must rely on OS-level diagnostic settings or enterprise controls. Some commenters treat that as reason enough to leave Windows entirely, describing full clean Linux installs or VMs as their alternative.

**「Community Discussion」** Commenters spent little time on the telemetry claim itself and instead argued about moving to Linux: one said most single-player games now run perfectly on Linux while multiplayer still has problems, and another said adjusting to Linux from Windows takes about a week and that web-based workflows lose nothing. One commenter said they no longer dual-boot and now clean-install Linux only, running Windows in a VM if needed, while another merely speculated that Windows 11 &quot;is probably collecting a lot more data&quot; — an opinion not backed by evidence in the thread.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/N0tHorizon/WindowsTelemetryBlocker">N0tHorizon/WindowsTelemetryBlocker: A PowerShell based tool to...</a></li>
<li><a href="https://xusheng.dev/">Xusheng Li</a></li>
<li><a href="https://www.youtube.com/watch?v=mOeBjArKMYY">How Much Data Does Windows 11 Really Collect ? - YouTube</a></li>
<li><a href="https://windowsforum.com/news/understanding-windows-telemetry-privacy-performance-and-control.346257/">Windows Telemetry : Privacy , Performance &amp; Control</a></li>

</ul>
</details>

**Tags**: `#Windows 11`, `#telemetry`, `#privacy`, `#developer tools`, `#coding agents`

---

<a id="item-tech-news-11"></a>
### [TRMNL announces Frame, a 31.5-inch color ePaper display](https://trmnl.com/blog/introducing-frame) ⭐️ 6.0/10

TRMNL announced Frame, a 31.5-inch color ePaper display. The announcement drew Hacker News interest around the display&\#x27;s large format and high cost, but the supplied material does not include shipping date, resolution, refresh rate, compatibility, or availability details.

hackernews · geerlingguy · Nov 16, 16:23 · [Discussion](https://news.ycombinator.com/item?id=50519354)

**「Background」** Frame is TRMNL&\#x27;s third hardware release, following the smaller e-ink dashboards the company built its earlier products around; the company&\#x27;s announcement describes it as &quot;a full color 31.5&quot; ePaper display in a handmade wooden frame&quot; and says it is available for pre-order \[tool-2-1\]. Color e-paper has so far been confined mainly to small personal frames such as 3.7-inch E Ink Spectra 6 panels, with larger color e-ink frames only recently appearing at around 13.3 inches \[tool-2-3\]\[tool-2-2\].

**「Impact」** At the $1,200 price a commenter cites, Frame is priced above what individual buyers in the discussion say they are willing to pay, so near-term adoption is likely to stay with people who have a specific wall-display or signage need; external market coverage of large-format e-paper likewise emphasizes commercial signage and retail rather than consumer art displays. Buyers already holding TRMNL hardware should also weigh one commenter&\#x27;s account of declining QA and delayed shipments on earlier devices, which is a single reported experience rather than a verified pattern.

**「Community discussion」** Commenters were divided on practicality: one said a $1,200 price is too high but welcomed that the product exists, while another reported declining QA, late shipments, and said the founder&\#x27;s politics were a turnoff, concluding they would not buy from the company again. Others discussed potential uses, including using e-ink displays for AI coding chats to reduce eye strain, though they noted the technology remains expensive.

<details><summary>References</summary>
<ul>
<li><a href="https://trmnl.com/blog/introducing-frame">Introducing Frame | TRMNL</a></li>
<li><a href="https://www.youtube.com/watch?v=W5HQqVFsu9Y">Refresh display of reTerminal E 1002 vs E 1001 - YouTube</a></li>
<li><a href="https://www.gobetterdisplay.com/">VeraMag Color ePaper Photo Frame | GoBetter Display</a></li>
<li><a href="https://www.researchandmarkets.com/report/e-paper-display">E-Paper Display Market Size, Competitors, Trends &amp; Forecast Largest E-Ink Display 2026: Innovation &amp; Trends - accio.com Big E Ink Screen Trends for 2026 - accio.com E-Paper Display Market Report 2026 - Research and Markets Global Color E-paper Display Market Size, Growth Analysis ... Global ePaper Display Market Research Report 2026 (Status and ...</a></li>

</ul>
</details>

**Tags**: `#e-paper`, `#hardware`, `#displays`, `#TRMNL`, `#product-launch`

---

<a id="item-tech-news-12"></a>
### [Microsoft blames email outage on defect from July fix](https://www.theregister.com/saas/2026/11/16/microsoft-blames-monster-email-outage-on-software-defect-introduced-in-july-fix/5310026) ⭐️ 6.0/10

Microsoft has blamed a major email outage on a software defect introduced by a July fix, according to The Register. The disruption affected Microsoft&\#x27;s email service, and the stated cause is a regression from a previously shipped update rather than a new, unrelated fault. The account does not identify the affected version, the number of users impacted, or independent confirmation of Microsoft&\#x27;s attribution.

hackernews · Bender · Nov 16, 13:18 · [Discussion](https://news.ycombinator.com/item?id=50517321)

**「Background」** The postmortem closes out an incident Horizon&\#x27;s November 13 digest reported as a worldwide Microsoft 365 email degradation, in which Microsoft had validated an alternative health check on a subset of affected infrastructure and was preparing an automated recovery process to restart unresponsive servers. A November 14 digest reported the same episode had kept Outlook, Teams, and Copilot down for more than 12 hours and disrupted business and government communications, with Microsoft at that point attributing the failure to a server issue and finding no malicious activity. The new development is the attribution itself: a software defect introduced by a July fix, rather than the server issue initially cited.

**「Community discussion」** Commenters focused on recovery and load management, with one drawing an analogy to an electricity grid black start and another asking why Microsoft could not shed load by dropping or cycling client connections. A separate strand questioned whether it is acceptable—or too costly—to rely on a low-end test environment that passed the July code while production hardware hid a concurrency bug.

<details><summary>References</summary>
<ul>
<li><a href="https://status.cloud.microsoft/">2026-11-13 — Microsoft 365 Email Outage Worldwide as Recovery Progresses</a></li>
<li><a href="https://www.reuters.com/technology/microsoft-365-outlook-down-thousands-us-users-downdetector-shows-2026-11-12/">2026-11-14 — Microsoft Outlook, Teams, Copilot Global Outage Exceeds 12 Hours</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#service outage`, `#incident postmortem`, `#reliability engineering`, `#load shedding`

---

<a id="item-tech-news-13"></a>
### [Apple and OpenEvidence launch 200k-person health AI use study](https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/) ⭐️ 6.0/10

Apple announced the Apple Health AI Usage Study in the US with clinical AI platform OpenEvidence to examine how people use conversational health AI, including their trust in and understanding of it. The study aims to recruit up to 200,000 US residents aged 21 or older who use an Apple Intelligence-capable iPhone 15 Pro or later running iOS 26 or newer, and Apple says the app is not for diagnosis or treatment. Data collected for the research will not be used to train AI models, according to the announcement. No results or findings have been released.

telegram · zaihuapd · Nov 16, 05:01

**「Background」** Apple&\#x27;s partner on the study, OpenEvidence, is a Miami-based company founded in 2022 that operates a clinical decision-support large language model for healthcare professionals, with answers grounded in peer-reviewed research from sources such as NEJM, JAMA, Nature, NCCN and Cochrane. It has also announced collaborations with academic medical centers including Johns Hopkins Medicine and Boston Children&\#x27;s Hospital. The study therefore pairs consumer iPhones with a platform built for clinician-facing medical evidence rather than a general-purpose chatbot.

**「Impact」** People who want to take part must have a supported iPhone and iOS version, so enrollment is limited to owners of iPhone 15 Pro or newer devices running iOS 26 or later, and participants should not treat the app as a diagnostic or treatment tool.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenEvidence">OpenEvidence - Wikipedia</a></li>
<li><a href="https://www.openevidence.com/">OpenEvidence</a></li>
<li><a href="https://portal.openevidence.com/">Enterprise | OpenEvidence</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Health AI`, `#AI Research`, `#OpenEvidence`, `#iOS 26`

---

<a id="item-tech-news-14"></a>
### [Apple Intelligence enters beta on China-market iPad and Mac with Siri usage caps](https://www.theverge.com/tech/1034581/apple-intelligence-siri-ai-daily-usage-limits-icloud-subscription) ⭐️ 6.0/10

Apple Intelligence is now available in beta on China-market iPad and Mac, and users must update to iPadOS 27.3 beta 2 or macOS 27.3 beta 2 to try it. In those same betas, Apple is testing daily per-device usage limits on some advanced Siri and Apple Intelligence features — specifically multi-step personal-context requests and image generation and editing — while basic Siri commands remain free and unlimited. The betas also fix a file-access sandbox-escape vulnerability that the source calls &quot;worse\_query&quot; across Apple&\#x27;s operating systems. The usage caps are described as a test, not a shipped, finalized policy.

telegram · zaihuapd · Nov 16, 20:12

**「Background」** Apple Intelligence first reached mainland-China iPhones in the initial iOS 27.3 beta; that build did not include Siri AI or other next-generation features shown at WWDC 2026. Horizon&\#x27;s November 4 digest reported that the China testing was tied to a partnership with Alibaba&\#x27;s Qwen model and covered only part of Apple&\#x27;s AI feature set.

**「Impact」** For China-market users, access to Apple Intelligence on iPad and Mac is gated behind beta OS builds, so trying it means enrolling in beta software. Because the daily caps are device-level and target cloud-based advanced features such as personal-context requests and image generation, frequent users of those features could reach the limit, while plain Siri commands remain uncapped.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/11/03/ios-27-3-health-app/">2026-11-04 — 苹果推 iOS 27.3 测试版：健康 App 重做、手表 AI 听录、国行 Apple 智能</a></li>
<li><a href="https://www.macrumors.com/2026/11/16/ipad-mac-apple-intelligence-china/">iPad and Mac Get Apple Intelligence in China in 27.3 Betas</a></li>

</ul>
</details>

**Tags**: `#Apple Intelligence`, `#Siri`, `#Apple OS`, `#security vulnerability`, `#usage limits`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [vLLM v0.34.0: Extensible KV Cache by Default, Model Runner V1 Retired](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 9.0/10

vLLM v0.34.0 enables its extensible KV cache by default, removes Model Runner V1 in favor of Model Runner V2, adds 10 model supports, and reports speedups up to 1.95× decode on GB200 — bundled with breaking default changes including block size 16→64 and gpu\_memory\_utilization 1.0.

github · khluu · Nov 16, 23:22

**「Problem Solved」** KV cache allocation was previously sized from an estimate rather than from memory actually free after CUDA graph capture and warmup, leaving capacity on the table. The extensible KV cache now sizes it from real post-warmup free memory on CUDA and ROCm, yielding a larger cache — the release cites MiniMax-M3 on H200 going from 433k to 672k tokens — so throughput is higher and TTFT lower at high concurrency. The trade-off is stated plainly: per-token decode latency can rise \(TPOT +6–18% on some H200 models at concurrency 128\), opt out via --gpu-memory-utilization 0.9 or --no-enable-extensible-kv-cache. The release also notes hardening fixes for allocator fragmentation, startup OOMs, and KV connectors, and removing Model Runner V1 eliminates a redundant second GPU runner path.

**「Ecosystem context」** vLLM is one of the reference open-source inference and serving engines for LLMs, built around PagedAttention-style KV memory management, continuous batching, chunked prefill and prefix caching \(tool-1-2\). Its reputation rests on memory efficiency: PagedAttention is widely described as the algorithmic insight that made vLLM&\#x27;s throughput possible, cutting KV cache fragmentation from a reported 60-80% of allocated memory to near zero \(tool-2-3\). v0.34.0 continues that same line of work rather than starting a new one. The headline change — sizing the KV cache from memory actually free after CUDA graph capture and warmup instead of an estimate — is a direct successor to the fragmentation problem, trading some per-token decode latency for a larger cache and higher throughput at concurrency. The other headline is architectural cleanup: Model Runner V1 is removed and V2 becomes the only GPU runner, which is where dual-batch overlap, suffix decoding and CUDA-graph speculators now live. Around that, the release broadens hardware and model coverage \(Blackwell GB200/GB300, MI355X, ROCm 10.0-only artifacts, 10 new model families including Mistral Large 4 at 1T total / 52B active\) and adds operational features such as checkpoint/restore and fault-tolerant DP+EP scale-down. The upgrade notes matter for the ecosystem: block size defaulting to 64, \`gpu\_memory\_utilization\` at 1.0 and dropped backends mean existing deployments need explicit opt-outs to preserve prior behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm - project / vllm : A high - throughput and memory-efficient...</a></li>
<li><a href="https://gigagpu.com/vllm-paged-attention-explained/">vLLM PagedAttention Explained GIGAGPU</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM`, `#inference`, `#serving`, `#KV cache`, `#paged attention`, `#CUDA`, `#model support`, `#release`, `#breaking changes`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly Wheel for Rebellions RBLN NPU](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 6.0/10

LMCache published a nightly wheel for Rebellions RBLN NPUs, built from the dev branch on 2026-11-16 against torch-rbln 0.12.0. It packages LMCache for environments where torch-rbln, rebel-compiler, and the RBLN driver are already installed.

github · github-actions\[bot\] · Nov 16, 13:07

**「Problem Solved」** Running LMCache on Rebellions RBLN NPUs requires a compatible build tied to the host&\#x27;s torch-rbln and rebel-compiler stack. This nightly wheel provides that build without bundling the compiler or driver, reducing packaging and deployment friction. The source does not describe performance or feature changes.

**「Background and impact」** LMCache is a KV-cache management layer for LLM inference: it extracts KV caches from engines such as vLLM and SGLang, stores them outside GPU memory, and reuses them across engines and queries \(tool-1-2\). Its stated scope includes storing, reusing, compressing, searching, moving, and observing KV cache across GPU, CPU memory, and external backends, which matters for long prompts and repeated conversation or retrieved context \(tool-1-1; tool-1-3\). This nightly-rbln release is a packaging update rather than a described core feature: it publishes a wheel built from \`dev\` and pinned against torch-rbln 0.12.0, while torch-rbln, rebel-compiler, and the RBLN driver remain host-owned and are not bundled. torch-rbln is a PyTorch extension for Rebellions NPU compute, and rebel-compiler is a separately installed requirement \(tool-2-1; tool-2-3\). Rebellions positions its ATOM accelerator for AI inference \(tool-2-2\). The broader impact is hardware reach: LMCache&\#x27;s KV-cache layer is being made installable on a non-GPU inference accelerator family. Because the source lists no performance data, feature changes, or validation results, this should be read as build/integration evidence, not as a claim that RBLN support is complete or faster.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache/LMCache: LMCache: Supercharge Your LLM with ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://lmcache.ai/en/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://pypi.org/project/torch-rbln/">torch - rbln · PyPI</a></li>
<li><a href="https://rebellions.ai/developers/">Developers - Rebellions</a></li>
<li><a href="https://github.com/RBLN-SW/torch-rbln">RBLN -SW/ torch - rbln : PyTorch extension for Rebellions NPU · GitHub</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly`, `#packaging`

---

<a id="item-ai-projects-3"></a>
### [LMCache releases nightly ROCm wheels](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 5.0/10

Nightly ROCm 7.2 wheels for LMCache, a KV-cache layer for LLM inference, targeting AMD Instinct gfx942 and gfx950 GPUs and ABI-matched to the upstream vLLM ROCm container \(torch 2.13, cp312\).

github · github-actions\[bot\] · Nov 16, 13:14

**「Problem Solved」** It addresses platform-specific packaging for running LMCache with vLLM on AMD ROCm systems. The wheels provide prebuilt ROCm 7.2 support for named Instinct GPUs and match the upstream vLLM ROCm image ABI, reducing the need to build from source or resolve ABI mismatches when integrating the KV-cache layer.

**「Background」** LMCache sits below the inference server as a KV-cache management layer focused on cache reuse, offloading, compression, and serving optimization \(tool-1-1\). In vLLM deployments it integrates through the KV connector interface, so clients keep using the standard OpenAI-compatible endpoint while LMCache manages cache underneath \(tool-1-2\). That places this release in the serving-infrastructure layer rather than in model or kernel development.

The \`nightly-rocm\` artifact is a CI packaging output, not a feature release: wheels built from \`dev\` on 2026-11-16 for ROCm 7.2, targeting AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), and ABI-matched to the upstream \`vllm/vllm-openai-rocm\` image with torch 2.13/cp312. Its practical effect is to make LMCache installable inside AMD&\#x27;s vLLM ROCm container path. ROCm 7.2 documentation covers MI300X/MI350X inference optimization, and the gfx942/gfx950 targets correspond to CDNA3/CDNA4 AMD Instinct generations \(tool-2-1, tool-2-3\). The release note includes no benchmarks, changelog, or new architecture details.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-7.2.4/how-to/rocm-for-ai/inference-optimization/workload.html">AMD Instinct MI300 Series / MI350 Series workload optimization</a></li>
<li><a href="https://github.com/jhinpan/ROCmKernelWiki">GitHub - jhinpan/ROCmKernelWiki: Agent-queryable ROCm kernel ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#inference`, `#KV cache`, `#serving`, `#ROCm`, `#vLLM`, `#nightly`, `#release`

---

<a id="item-ai-projects-4"></a>
### [LMCache nightly build: CUDA 13.0 wheels](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache published a nightly CUDA 13.0 wheel build from its \`dev\` branch for linux/amd64 and linux/arm64, with install instructions. No changelog, feature details, or performance claims are included.

github · github-actions\[bot\] · Nov 16, 14:51

**「Problem solved」** The build provides prebuilt wheels matched to CUDA 13.0 and PyTorch&\#x27;s \`cu130\` index, reducing the need to compile LMCache locally or manually resolve compatible dependencies. This is a packaging and distribution convenience; the source gives no evidence of changes to KV-cache efficiency or inference speed.

**「Background &amp; Impact」** LMCache is a KV cache management layer for LLM inference: it turns KV cache from temporary per-request state into reusable, persistent &quot;AI-native memory&quot; that can be stored, compressed, searched, and reused across serving engines and cluster nodes \(tool-1-1, tool-1-2\). That matters because inference engines manage KV cache at page granularity — typically 20 KB–63 KB for popular models such as Llama, Qwen and GPT-OSS — which is where enterprise-scale serving runs into memory pressure and cache-reuse limits \(tool-1-3\).

This item is a nightly build, not a versioned feature release. The only concrete change stated by the source is packaging: CUDA 13.0 wheels built from the \`dev\` branch on 2026-11-16 for linux/amd64 and linux/arm64, installed via \`uv pip install lmcache --pre\` against PyTorch&\#x27;s cu130 index. No changelog, feature additions, or performance numbers were supplied, so any effect on throughput or cache-hit rates cannot be assessed from the available evidence.

In ecosystem terms, the signal is continued platform coverage rather than new capability. Pre-release wheels that track an upstream CUDA/PyTorch toolchain let users test LMCache against newer GPU stacks without building from source, but because the artifact comes from \`dev\` it should be treated as an unstable snapshot rather than a stable upgrade path.

<details><summary>References</summary>
<ul>
<li><a href="https://lmcache.ai/">LMCache – Building the foundation of AI memory tensor with KV ...</a></li>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>
<li><a href="https://arxiv.org/pdf/2510.09665">LMCache : An Efficient KV Cache Layer for Enterprise-Scale LLM ...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#CUDA`, `#nightly release`, `#packaging`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s October retail sales, industrial output and investment all miss forecasts](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 8.0/10

China&\#x27;s October retail sales rose 0.4% from a year earlier and industrial output grew 4.8%, both missing analysts&\#x27; estimates of 0.8% and 5.3%, while fixed-asset investment fell 8.1% in the first ten months of the year against an expected 7% decline. The official data point to a deepening slowdown, with weak consumer spending at home offset by exports that surged 35.2% year-on-year in October.

rss · CNBC Finance · Nov 16, 03:53

**「Background」** China&\#x27;s economy grew 4.5% year-on-year in July–September, bouncing off a three-year low, after a fifth year of property-market decline eroded household wealth. The export surge now driving growth is drawing pushback abroad — EU leaders have weighed new measures against Chinese goods — and a November scandal over U.S.-restricted Nvidia chips reaching China renewed scrutiny of the AI demand behind those exports.

**「Impact」** Analysts say China&\#x27;s growing reliance on exports leaves its growth more exposed to foreign demand shocks, with Citi Research flagging further EU trade measures as a plausible downside risk next year.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/13/export-banned-nvidia-chips-are-behind-chinas-most-powerful-ai-models-uh-oh-jensen/">Export-banned Nvidia chips are behind China&#x27;s most powerful ...</a></li>
<li><a href="https://www.reuters.com/world/china/pressured-home-eu-leaders-weigh-china-trade-steps-2026-10-14/">Pressured at home, EU leaders weigh China trade steps</a></li>

</ul>
</details>

**Tags**: `#China economy`, `#macroeconomic data`, `#industrial output`, `#retail sales`, `#fixed-asset investment`

---

<a id="item-finance-news-2"></a>
### [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has ties to the chipmaker](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

CNBC examines possible conflicts between Commerce Secretary Howard Lutnick&\#x27;s handling of Nvidia-related China export controls and his sons&\#x27; firm Cantor Fitzgerald&\#x27;s Nvidia stock holdings and business ties, amid Nvidia CEO Jensen Huang&\#x27;s resignation and increased scrutiny.

rss · CNBC Finance · Nov 16, 12:14

**Tags**: `#Nvidia`, `#export controls`, `#China`, `#conflict of interest`, `#Commerce Department`

---

<a id="item-finance-news-3"></a>
### [英特尔及 CEO 陈立武遭股东集体诉讼](https://www.investing.com/news/stock-market-news/intel-sued-by-shareholders-following-29-stock-plunge-5028171) ⭐️ 8.0/10

英特尔因PC需求疲软和库存问题被指隐瞒风险，在发布不及预期的业绩指引后股价暴跌28.6%，并遭股东集体诉讼，CEO与CFO同列被告。

telegram · zaihuapd · Nov 16, 11:10

**Tags**: `#Intel`, `#股东集体诉讼`, `#半导体`, `#业绩指引`, `#市值蒸发`

---

<a id="item-finance-news-4"></a>
### [Nvidia CEO Exit and Congress Risk Could Reshape AI Trade, ETF Experts Say](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

After Nvidia founder and CEO Jensen Huang resigned, Yorkville Ives cut its price target on the chipmaker to $225 from $300 while keeping a buy rating; Nvidia shares ended the week at $162.85. ETF experts said Big Tech and other AI chip names could benefit if investors lose confidence in Nvidia, while a Democratic-controlled Congress could slow data-center buildout.

rss · CNBC Finance · Nov 16, 12:13

**「Background」** Nvidia co-founder and CEO Jensen Huang resigned in mid-November 2026 after reports of extramarital affairs, including with an alleged Chinese spy and two company employees, and CFO Colette Kress became interim CEO; separately, Democrats won control of Congress in the Nov. 3 midterms and have called for tougher limits on AI data centers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/nov/12/nvidia-ceo-jensen-huang-resigns">Jensen Huang resigns as Nvidia CEO after alleged affairs</a></li>
<li><a href="https://fxmacrowire.com/wire/top-democrats-call-to-rein-in-ai-buildout-after-midterms-sweep">Top Democrats call to rein in AI buildout after... | FXMacro Wire</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI trade`, `#ETF flows`, `#semiconductors`, `#US Congress/data centers`

---

<a id="item-finance-news-5"></a>
### [China Pork Prices Fall to Near 10-Year Low](https://finance.sina.com.cn/jjxw/2026-11-15/doc-iniyupuh6583194.shtml) ⭐️ 7.0/10

China&\#x27;s pork prices fell to near 10-year lows in early November, with the national average live hog price at 8.63 yuan per kilogram on Nov 9 and Fuzhou procurement prices down 20% to 26% year on year, according to Sina Finance. Industry insiders attributed the decline to weaker demand and higher hog supply, and analysts cited in the report expect a price rebound over the next 6 to 8 months may remain weak.

telegram · zaihuapd · Nov 16, 03:45

**「Background」** China&\#x27;s hog market has been stuck in a prolonged downturn since the current &quot;pig cycle&quot; — the recurring boom-and-bust swing in breeding and prices — began in 2022, and the national average hog price was already hovering around 9-10 yuan/kg in May 2026 as farmers cut breeding capacity only slowly.

**「Who feels it」** Because pork is treated as a bellwether of Chinese inflation, continued price weakness has been a decisive drag on the food CPI — pork was down 10.0% year-on-year in September 2026 while food CPI stood at -1.7% year-on-year — squeezing hog producers&\#x27; revenue even as it lowers grocery bills for households.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lydd-global.com/article-domestic-and-international-news/pig-prices-fall-pig-stocks-rise-what-s-behind-the-divergence.html">China Hog Market: Futures Fall, Stocks Rise Amid Pig Cycle ...</a></li>
<li><a href="https://www.mysteel.net/analysis/5122914-hog-prices-bottom-out-amid-deep-breeding-losses">Hog prices bottom out amid deep breeding losses | Mysteel</a></li>
<li><a href="https://bigmacrodata.com/news/china/cpi/food-inflation-report-jun-2026">June 2026 Food CPI Deflation: Pig Cycle L-Shaped Bottoming ...</a></li>
<li><a href="https://www.nytimes.com/2026/05/28/business/china-pork-prices-economy.html">What Plunging Pork Prices Say About China’s Economy</a></li>
<li><a href="https://bigmacrodata.com/news/china/cpi/food-inflation-report-sep-2026">China Pork Prices -10.0% YoY — September 2026 Food Inflation Data</a></li>

</ul>
</details>

**Tags**: `#China pork prices`, `#agricultural commodities`, `#food inflation`, `#livestock supply`, `#consumer prices`

---

<a id="item-finance-news-6"></a>
### [China&\#x27;s foreign direct investment turns to net outflow in the third quarter](https://cn.nikkei.com/china/ceconomy/64726-2026-11-16-09-03-25.html) ⭐️ 7.0/10

China&\#x27;s balance-of-payments data released by the State Administration of Foreign Exchange on November 13 showed foreign direct investment into China turned negative in July–September, at a net outflow of $0.9 billion — the first negative reading in four quarters, meaning capital withdrawn or recovered through scaled-back operations exceeded new investment such as factory construction. The outflow exceeded the $50 million recorded in the same period of 2025 but was smaller than the $10.8 billion outflow in July–September 2023, with the data pointing to weaker foreign investment willingness amid an uncertain economic outlook, softer growth expectations, weak domestic demand and intensifying price competition.

telegram · zaihuapd · Nov 16, 05:29

**「Background」** Foreign direct investment is measured in a country’s balance of payments, which tracks cross-border capital flows; China’s State Administration of Foreign Exchange publishes the quarterly data. The latest negative reading followed four quarters of net inflows, and the Q3 2023 outflow was $10.8 billion, a much larger baseline than the latest $0.9 billion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.safe.gov.cn/en/2026/0327/2406.html">SAFE Releases China&#x27;s Balance of Payments for the Fourth ...</a></li>
<li><a href="https://www.safe.gov.cn/en/2026/0814/2442.html">SAFE Releases Preliminary Data of the Balance of Payments for ...</a></li>

</ul>
</details>

**Tags**: `#China FDI`, `#Balance of Payments`, `#Foreign Investment`, `#China Economy`, `#SAFE Data`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [Lenny Rachitsky&\#x27;s prompt for wiring an AI bot to a user-owned Anthropic API key](https://x.com/lennysan/status/2122493471982592455) ⭐️ 6.0/10

Lenny Rachitsky shared a reusable prompt addressed to an AI bot/assistant that tells it to run a task through Claude models using the user&\#x27;s own Anthropic API account, rather than the assistant&\#x27;s built-in access. The prompt is written as six numbered instructions:

\1. Ask for the user&\#x27;s Anthropic API key through a secure secret field, never in chat; if the key belongs to a specific Anthropic workspace, request that workspace ID the same way.
\2. Store the key only on the bot&\#x27;s computer and never print it, then write a small helper script that calls the Anthropic Messages API with the \`x-api-key\` and \`anthropic-version\` headers, plus an \`anthropic-workspace-id\` header if a workspace ID was supplied.
\3. List the models the key can use via \`GET /v1/models\` and show them so the user can pick one.
\4. Send a short test message and confirm it works; on failure, report the exact error \(the prompt gives &quot;credit balance too low&quot; as an example\) so billing can be fixed.
\5. Once working, update the bot&\#x27;s skill and routines so the chosen model writes the first draft and the bot reviews and fact-checks it, keeping only text blocks when a model returns a thinking block first, and falling back to drafting itself with an explanation if a call fails.
\6. Save the setup to the bot&\#x27;s memory so it persists.

The post frames this as a practical workflow template. The two links in the prompt are shortened \(t.co\) URLs; one is presented as the Messages API reference and the other as the billing page for resolving errors. No community comments were available with the item.

twitter · Lenny Rachitsky · Nov 17, 00:54

**「Background」** The prompt targets a common pattern in agentic AI assistants: letting a user bring their own provider credentials so usage is billed to and governed by their own account instead of the assistant platform&\#x27;s. As described in the post, that means the assistant must handle several distinct concerns — secret collection, local-only storage, a script that speaks the provider&\#x27;s HTTP API, model discovery, a connectivity test, and persistence of the resulting configuration into the assistant&\#x27;s memory or &quot;skill&quot; system.

Several of the details in the prompt reflect terminology specific to Anthropic&\#x27;s platform. The Messages API is named as the endpoint the helper script should call, and the prompt specifies the \`x-api-key\` and \`anthropic-version\` request headers, with an optional \`anthropic-workspace-id\` header for keys tied to a particular workspace. Model discovery is delegated to a \`GET /v1/models\` call, and the prompt notes that some models may emit a thinking block ahead of the text output, in which case only the text blocks should be retained. The prompt also anticipates failure modes such as exhausted credit balance and directs the user to a billing link to resolve them.

The item is a workflow tip rather than a research result or product announcement: it packages configuration and safety steps into a copy-pasteable instruction set. Two details that a reader would need to confirm independently are the targets of the shortened URLs \(the Messages API documentation and the billing page\) and the current behavior of any specific Claude model with respect to thinking blocks. No community discussion or third-party commentary was supplied with the item.

**Tags**: `#anthropic`, `#claude`, `#api`, `#prompt-engineering`, `#ai-assistant`, `#productivity`

---

