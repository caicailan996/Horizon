---
layout: default
title: "Horizon Summary: 2026-10-01 (EN)"
date: 2026-10-01
lang: en
---

> From 53 items, 25 important content pieces were selected

---

**Technology News**
1. [Google introduces Gemini 4 Argon with Rust migration agents](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI&\#x27;s Sam Altman announces Dots, a 24/7 persistent AI assistant](#item-tech-news-2) ⭐️ 8.0/10
3. [Survey of Tokenization in Modern NLP, Including Alternatives](#item-tech-news-3) ⭐️ 8.0/10
4. [DeepSeek Open-Sources Huawei Ascend Components](#item-tech-news-4) ⭐️ 8.0/10
5. [Reassessing MCP: A Nuanced Defense of the Protocol](#item-tech-news-5) ⭐️ 7.0/10
6. [A Brief History of the Bloomberg Terminal](#item-tech-news-6) ⭐️ 7.0/10
7. [CO₂Jump: Training-Free Sampler for Consistent Text–Image Generation](#item-tech-news-7) ⭐️ 7.0/10
8. [Trump signs non-binding AI safety deal with six tech companies](#item-tech-news-8) ⭐️ 7.0/10
9. [Cloudflare announces plan to become public certificate authority](#item-tech-news-9) ⭐️ 7.0/10
10. [Singapore public servant dating app reportedly uses Gale-Shapley algorithm](#item-tech-news-10) ⭐️ 6.0/10
11. [A Family History of Displacement Offers Perspective on AI Job Loss](#item-tech-news-11) ⭐️ 6.0/10
12. [2026 Python Language Summit reports now available](#item-tech-news-12) ⭐️ 6.0/10
13. [Chromium developer contrasts Google and Igalia work cultures](#item-tech-news-13) ⭐️ 6.0/10
14. [Qwen-family LLMs dominate backbones in 100+ audio models survey](#item-tech-news-14) ⭐️ 6.0/10
15. [LessThink-Qwen3-4B claims 44% fewer reasoning tokens](#item-tech-news-15) ⭐️ 6.0/10
16. [ORTUS AI open-sources RightWayUp 360° image rotation detection model](#item-tech-news-16) ⭐️ 6.0/10
17. [McDonald&\#x27;s Reportedly Uses AI to Set Burger Prices by Willingness to Pay](#item-tech-news-17) ⭐️ 6.0/10
18. [Microsoft Uses Outsourced Contractors to Review Copilot Image Prompts and Outputs](#item-tech-news-18) ⭐️ 6.0/10
19. [Kimi K3 Now Available via OpenAI Codex with Enterprise Billing Integration](#item-tech-news-19) ⭐️ 6.0/10
20. [Apple Plans October 13 Launch of Smart Home Hub with Siri AI](#item-tech-news-20) ⭐️ 6.0/10
21. [Bilibili Open-Sources Index-Translate Translation Models](#item-tech-news-21) ⭐️ 6.0/10

**Financial News**
1. [Prediction markets Kalshi and Polymarket face questions over trading volumes](#item-finance-news-1) ⭐️ 7.0/10
2. [Temasek plans Abu Dhabi and Riyadh offices as it expands Middle East push](#item-finance-news-2) ⭐️ 7.0/10
3. [China warns of retaliation against EU trade restrictions](#item-finance-news-3) ⭐️ 7.0/10

**Twitter News**
1. [OpenAI Announces Report on AI Agents for Small Businesses and Partnership with ASBDC](#item-twitter-news-1) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google introduces Gemini 4 Argon with Rust migration agents](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) ⭐️ 9.0/10

Google has introduced Gemini 4 Argon, a new AI model with agentic capabilities, and says its agents are already migrating C/C++ codebases to Rust across Google. The model is not yet generally available: the announcement describes feedback from early testers and ongoing guardrail iteration before Argon reaches developers, enterprises, and consumers. No benchmark numbers or public pricing are in the supplied coverage.

hackernews · bradleyg223 · Sep 30, 20:04 · [Discussion](https://news.ycombinator.com/item?id=49913571)

**「Background」** Gemini 4 Argon is Google&\#x27;s newest frontier model in the Gemini family, positioned for complex, long-horizon professional reasoning and advertised with a 1 million token output limit and $2/$10 per million token pricing. Coverage of the announcement also reports that Argon agents are already being used inside Google to migrate C/C++ codebases to Rust, scaling from core libraries such as re2 and libgav1 to Fuchsia&\#x27;s Zircon kernel at over 800K lines.

**「Community discussion」** Commenters disagree over whether this signals durable competition: one argues the rapid leapfrogging undercuts Dario Amodei&\#x27;s winner-takes-all theory, while another advises users to keep models and providers replaceable because frontier labs will keep leapfrogging. Another reports that a prior Gemini model debugged a GPU driver and authored an LD\_PRELOAD shim to get ROCm working with llama.cpp on Strix Halo, though that remains an individual anecdote rather than a benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon</a></li>
<li><a href="https://mangodeveloper.com/articles/google-unveils-gemini-4-argon-1m-token-output-rust-migrations-at-scale-and-cyber-defense-that-finds">Google Unveils Gemini 4 Argon : 1M Token Output, Rust Migrations ...</a></li>
<li><a href="https://www.datacamp.com/blog/gemini-4-argon">Gemini 4 Argon : Benchmarks, Pricing, and Access | DataCamp</a></li>

</ul>
</details>

**Tags**: `#gemini`, `#google`, `#ai-model`, `#agents`, `#rust`

---

<a id="item-tech-news-2"></a>
### [OpenAI&\#x27;s Sam Altman announces Dots, a 24/7 persistent AI assistant](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E5%A5%A5%E7%89%B9%E6%9B%BC%E5%AE%98%E5%AE%A3Dots%EF%BC%8124%E5%B0%8F%E6%97%B6AI%E5%90%8C%E4%BA%8B%E4%B8%8A%E5%B2%97%EF%BC%8C%E5%85%B3%E6%8E%89%E7%AA%97%E5%8F%A3%E8%BF%98%E5%9C%A8%E6%9B%BF%E4%BD%A0%E5%B9%B2%E6%B4%BB) ⭐️ 8.0/10

At DevDay 2026 on September 29, OpenAI unveiled Dots, a persistent AI assistant that Sam Altman says can carry out delegated tasks around the clock, continuing work in the cloud even after the user closes the chat window. The product is pitched at people managing multiple projects who want an AI &quot;colleague&quot; that retains context, follows clear authorization, and proactively spots missing details. These capabilities are vendor claims from the launch announcement; the article does not report independent testing or measured results.

rss · 新智元 · Sep 30, 12:38

**「Background」** Dots are persistent, always-on AI agents introduced by OpenAI at DevDay 2026. Unlike conventional chat interfaces that require manual prompting for each task, Dots operate autonomously in the cloud, maintaining context and executing multi-step workflows even after the user closes the interface.

**「Impact」** Dots gives knowledge workers a persistent, cloud-based AI agent that autonomously executes long-running tasks without requiring the user to keep the chat window open. Users assign goals and Dots works independently using its own cloud computer and browser, powered by GPT-6 Astra, freeing the user from repeatedly re-explaining context or managing multiple AI threads. This shifts AI-assisted work from synchronous, hands-on interaction to asynchronous delegation, potentially changing how developers, analysts, and project managers offload complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://open-ai-dots.com/">OpenAI Dots — Always-On AI Agents</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI assistants`, `#persistent agents`, `#Sam Altman`, `#technology industry`

---

<a id="item-tech-news-3"></a>
### [Survey of Tokenization in Modern NLP, Including Alternatives](https://www.reddit.com/r/MachineLearning/comments/1wuccjf/tokenization_a_survey_for_modern_nlp_r/) ⭐️ 8.0/10

A survey produced by 32 tokenizer researchers over roughly eight months systematically reviews tokenization in modern NLP, covering algorithms, evaluations, multilinguality, encodings, theory, and adjacent topics such as constrained generation, token healing, and tokenizer security. The authors also describe emerging alternatives to traditional tokenizers, including latent and visual tokenization. The survey is available on AlphaXiv and is presented as the most comprehensive overview of the field to date, rather than as a new model or benchmark.

reddit · r/MachineLearning · /u/mcmcmcmcmcmcmcmcmc\_ · Sep 30, 18:13

**「Background」** Modern language models typically process token sequences rather than raw text: a tokenizer splits text into subword units, often via methods such as byte-pair encoding or WordPiece, and the model&\#x27;s vocabulary and training are built around those tokens. Tokenization choices can affect model behavior across languages and tasks, but the authors argue the area remains understudied relative to its impact.

**「Impact」** For NLP researchers and practitioners, the survey consolidates fragmented tokenization knowledge into one reference, including guidance on evaluation and on alternatives such as latent or visual tokenization. Multilingual model builders and teams working on constrained generation or tokenizer security may find the survey especially relevant when deciding whether to keep or replace conventional tokenizers.

**Tags**: `#tokenization`, `#NLP`, `#survey`, `#language models`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [DeepSeek Open-Sources Huawei Ascend Components](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 8.0/10

A Telegram repost reports that DeepSeek has open-sourced foundational components for Huawei&\#x27;s Ascend platform, including the TileLang compiler, compute libraries, and distributed communication libraries, alongside projects such as DeepGEMM Ascend, DeepEP Ascend, TileKernels, FlashMLA, and DeepSelect. DeepSeek claims these components perform near hardware limits in multiple tests and is said to be working with Huawei on a 128-card Ascend 950 supernode plan. Since the report is not a primary announcement, official confirmation is still pending.

telegram · zaihuapd · Sep 30, 03:09

**「Background」** DeepSeek has an existing set of open-sourced AI infrastructure components for NVIDIA GPU platforms, and this release provides the corresponding Huawei Ascend versions: a TileLang compiler port, compute kernels such as DeepGEMM Ascend and TileKernels, and the DeepEP Ascend distributed communication library. The company also reports ongoing work with Huawei on a 128-card Ascend 950 supernode configuration.

**「Impact」** The release gives developers on Huawei Ascend a CUDA-like TileLang and kernel stack from DeepSeek to build and optimize models on homegrown hardware, creating a practical path away from Nvidia/CUDA. Large-scale users can also plan around the jointly developed 128-card Ascend 950 supernode, though performance claims still need independent verification on their own workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/19580/tilelang-deepseek-huawei-ascend-cuda">DeepSeek and Huawei release TileLang for Ascend chips, taking aim...</a></li>
<li><a href="https://www.cryptopolitan.com/deepseek-tools-huawei-rival-nvidia-cuda/">DeepSeek open - sources tools for Huawei chips to... - Cryptopolitan</a></li>
<li><a href="https://www.geopolitechs.org/p/deepseek-builds-for-huawei-ascend">DeepSeek Builds for Huawei Ascend - Geopolitechs</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#huawei-ascend`, `#open-source`, `#ai-infrastructure`, `#deep-learning`

---

<a id="item-tech-news-5"></a>
### [Reassessing MCP: A Nuanced Defense of the Protocol](https://earendil.com/posts/you-said-no-mcp/) ⭐️ 7.0/10

This post reassesses the Model Context Protocol, countering the prevailing anti-MCP sentiment by highlighting real-world implementations beyond coding assistance. The author publicly reverses a strongly held anti-MCP position and argues that protocol shortcomings are not disqualifying, drawing parallels to widely adopted standards such as USB-C. The piece acknowledges MCP&\#x27;s limitations while emphasizing its practical value and compatibility for tool integration.

hackernews · yarapavan · Sep 30, 09:55 · [Discussion](https://news.ycombinator.com/item?id=49906637)

**「Background」** MCP \(Model Context Protocol\) is an open-source standard for connecting AI applications such as Claude or ChatGPT to external data sources, tools, and workflows \[tool-2-1\]. This post is a public reversal: commenter gk1 credits the author&\#x27;s team for openly changing its strongly held anti-MCP belief, and commenter CharlieDigital recalls a March 2026 wave of tech influencers declaring MCP dead and crowning CLI-based tools the winner.

**「Impact」** Engineers weighing MCP against CLI-based tooling should consider that MCP is already enabling end users to configure desktop applications through natural language, as evidenced by commenters using local models with macOS apps. Teams that dismiss MCP based on protocol purity may overlook interoperable integrations that work across vendor boundaries today.

**「Community discussion」** Commenters offered concrete counterexamples to the &quot;MCP is dead&quot; narrative: alin23 described using local models with MCP to configure macOS apps such as Clop and Lunar, and CharlieDigital recalled a March wave of influencers declaring MCP dead in favor of CLI. gk1 praised the public reversal, while \_fw compared MCP&\#x27;s imperfections to USB-C&\#x27;s, arguing that broad compatibility and ease of use outweigh its flaws.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#Model Context Protocol`, `#AI tooling`, `#software engineering`, `#developer tools`, `#protocols`

---

<a id="item-tech-news-6"></a>
### [A Brief History of the Bloomberg Terminal](https://spectrum.ieee.org/bloomberg-terminal) ⭐️ 7.0/10

IEEE Spectrum has published a detailed history of the Bloomberg terminal, covering its custom keyboard, software architecture, and the company&\#x27;s long-standing backward-compatibility effort, which includes still supporting roughly 1985-era hardware. The article frames the terminal as an enduring engineering influence rather than a product announcement, highlighting how its information-dense displays and stable design philosophy shaped financial technology.

hackernews · rbanffy · Sep 30, 14:34 · [Discussion](https://news.ycombinator.com/item?id=49909583)

**「Background」** The Bloomberg terminal is a long-established financial data and communications system, widely used by traders and analysts. This feature surveys how its dedicated hardware and software evolved over the decades, helping readers understand the technical decisions behind a system that predates many modern internet technologies.

**「Impact」** The article shows that Bloomberg&\#x27;s commitment to preserving the terminal&\#x27;s classic look means users interact with a VT100-like interface even now that the underlying software is built on a private Chromium fork. For developers studying long-lived systems, this is a concrete example of retaining legacy workflows while modernizing the underlying technology.

**「Community Discussion」** Commenters added technical details beyond the article: one reported that the modern terminal uses a private Chromium fork styled like a VT100 and that Bloomberg still supports 1985 hardware in its backward-compatibility museum, while another recommended a talk on Bloomberg&\#x27;s home-grown server-side scripting. A separate commenter provided links to a history of competing Reuters terminals.

**Tags**: `#bloomberg terminal`, `#financial technology`, `#user interface`, `#history`, `#software engineering`

---

<a id="item-tech-news-7"></a>
### [CO₂Jump: Training-Free Sampler for Consistent Text–Image Generation](https://www.reddit.com/r/MachineLearning/comments/1wtyl5m/concurrent_image_understanding_and_generation/) ⭐️ 7.0/10

A NeurIPS 2026 paper from Google, Google DeepMind, and Stony Brook University introduces CO₂Jump, a training-free coupled Markov jump process sampler that improves consistency between jointly generated text and images. The sampler uses text confidence and cross-modal attention to guide image updates and re-masks low-confidence tokens so earlier generation decisions can be revised, requiring one model forward pass per denoising step. The authors evaluate image editing, maze solving, and nonograms, and introduce three datasets: JEdit-1M, JMaze-200K, and JNono-200K. Across 8–512 sampling steps, CO₂Jump was the only compared sampler that improved monotonically on both editing quality and grounding.

reddit · r/MachineLearning · /u/Upstairs\_Theme2785 · Sep 30, 07:28

**「Background」** Joint text and image generation often suffers from inconsistency when outputs are produced in parallel—a model may state the correct answer to a puzzle while drawing an incorrect solution. CO₂Jump is a training-free sampler that couples text and image denoising via cross-modal attention and token remasking to resolve such mismatches.

**「Impact」** Researchers working on joint text-image generation can use CO₂Jump without additional training on existing task-specific fine-tuned models, while the new JEdit-1M, JMaze-200K, and JNono-200K benchmarks offer concrete evaluation tasks where both the textual answer and generated image must be correct. Teams building editing or puzzle-solving systems should consider the sampler as a drop-in alternative, though its broader applicability beyond these tasks remains to be demonstrated.

**Tags**: `#multimodal generation`, `#diffusion models`, `#machine learning research`, `#text-to-image`, `#self-correction`

---

<a id="item-tech-news-8"></a>
### [Trump signs non-binding AI safety deal with six tech companies](https://www.zaobao.com.sg/news/world/story20260930-9758185) ⭐️ 7.0/10

On September 29, President Trump signed a one-page AI safety agreement with the leaders of Google, Anthropic, Meta, OpenAI, xAI, and Nvidia, publishing the document on Truth Social and describing it as having only “moral binding force.” The agreement commits the companies to four control mechanisms: independent external audits of AI governance systems, an independent board-level oversight committee, and monitoring of AI capabilities and alignment for cybersecurity and biological or chemical threats during model training and deployment to confirm that safeguards work as intended.

telegram · zaihuapd · Sep 30, 02:30

**「Background」** On September 27, 2026, the Australian Senate&\#x27;s AI inquiry issued subpoenas to the CEOs of OpenAI and Anthropic after an AI agent accessed government websites, intensifying regulatory pressure on AI safety practices. Horizon&\#x27;s September 28 digest reported the incident, which highlighted the need for external oversight that the voluntary agreement signed two days later attempts to address.

**「Impact」** Because the pact is not legally enforceable, the six companies face no formal penalties for noncompliance, but the announced commitments create a public benchmark for independent auditing and board oversight of AI safety practices across major AI developers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/legal/litigation/openai-anthropic-ceos-called-appear-australian-ai-probe-2026-09-27/">2026-09-28 — Australian Senate subpoenas OpenAI and Anthropic CEOs after agent accessed government sites</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#regulation`, `#Trump`, `#tech industry`, `#governance`

---

<a id="item-tech-news-9"></a>
### [Cloudflare announces plan to become public certificate authority](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare announced plans to enter the public certificate authority space, applying to Chrome, Apple, Microsoft, and Mozilla root programs and acquiring a trusted root certificate from GlobalSign. While no certificates are being issued yet, the new CA will prioritize ACME-based automatic issuance and renewal, and aims to issue production-grade post-quantum Merkle tree certificates \(MTC\) by the first quarter of 2027.

telegram · zaihuapd · Sep 30, 06:26

**「Background」** A public certificate authority \(CA\) issues TLS certificates that web browsers trust by default, enabling encrypted HTTPS connections. Cloudflare previously relied on partner CAs such as GlobalSign for its customers, but now intends to operate its own root to gain direct control over issuance, starting with ACME automation and eventually supporting post-quantum certificates.

**Tags**: `#PKI`, `#certificate authority`, `#Cloudflare`, `#post-quantum cryptography`, `#ACME`

---

<a id="item-tech-news-10"></a>
### [Singapore public servant dating app reportedly uses Gale-Shapley algorithm](https://twitter.com/tuakdotsol/status/2105105417760391258) ⭐️ 6.0/10

A Singapore government dating app for public servants reportedly uses the Gale-Shapley stable marriage algorithm, according to a BBC report shared on Hacker News. Implementation details beyond the algorithm mention remain thin, including how preferences are collected and which side proposes first.

hackernews · rzk · Sep 30, 09:27 · [Discussion](https://news.ycombinator.com/item?id=49906432)

**「Background」** The Gale-Shapley algorithm is a classic method for producing stable matches from ranked preferences, with real-world uses such as matching American medical students to residency programs. Singapore&\#x27;s reported government dating app for public servants, FirstDate, is said to rely on this algorithm to pair participants one at a time based on interests and values, rather than the swipe-based model used by most dating apps. The platform is reported to target public workers aged 21 to 35 as part of efforts to boost birth rates.

**「Impact」** For public servants eligible for the reported pilot, the app&\#x27;s choice of which side initiates matters concretely: Gale-Shapley produces proposer-optimal and acceptor-pessimal matches, so the same preference data can yield different outcomes depending on that design decision.

**「Community discussion」** Commenters split on applying Gale-Shapley here: missedthecue argued the dating market is a clearing problem rather than a matching problem, and abeppu questioned whether people&\#x27;s preferences are stable and well-defined enough for the algorithm. Others noted the proposer-optimal result depends on which side initiates, and one commenter drew parallels to past Singapore policy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gale%E2%80%93Shapley_algorithm">Gale – Shapley algorithm - Wikipedia</a></li>
<li><a href="https://observerbd.com/news/596644">Looking for love? Singapore govt may have a match</a></li>
<li><a href="https://www.ndtv.com/world-news/singapore-launches-dating-app-for-public-servants-to-boost-dwindling-birth-rates-12121956">Singapore Launches Dating App For Public Servants To Boost...</a></li>

</ul>
</details>

**Tags**: `#stable-marriage`, `#algorithms`, `#dating-apps`, `#public-policy`, `#gale-shapley`

---

<a id="item-tech-news-11"></a>
### [A Family History of Displacement Offers Perspective on AI Job Loss](https://manuel.darcemont.fr/posts/the-last-time-my-family-was-replaced-by-technology/) ⭐️ 6.0/10

In a personal essay published on September 30, 2026, the author uses a family member&\#x27;s historical experience of technological displacement to reflect on present-day anxiety over AI-driven job loss. The piece makes no technical claims or policy proposals; its chief significance is the broad Hacker News discussion it provoked about retraining and economic transitions. The author later clarified that the post was a personal tribute, not a prescription to simply adapt.

hackernews · megalomanu · Sep 30, 13:06 · [Discussion](https://news.ycombinator.com/item?id=49908394)

**「Background」** Essays linking past automation shifts to present AI job loss have become common as generative AI tools spread. The underlying question is whether economic transitions that once created new work will repeat at AI&\#x27;s speed and scale, or whether some displaced tasks will simply not return. This piece contributes a personal family-story angle to that ongoing debate.

**「Community Discussion」** The substantive thread contrasts the historical analogy with practical barriers: harimau777 asks how developers can realistically retrain without money or years for college, while zug\_zug argues that earlier displaced groups, such as horses after cars, did not recover. The author responds that the essay was a personal tribute, not a judgment that people should just adapt.

**Tags**: `#AI`, `#job displacement`, `#technology history`, `#personal essay`, `#Hacker News discussion`

---

<a id="item-tech-news-12"></a>
### [2026 Python Language Summit reports now available](https://lwn.net/Articles/1097761/) ⭐️ 6.0/10

LWN reports that the full set of write-ups from the 2026 Python Language Summit is now available on the Python blog. The summit took place on July 14 in Kraków, Poland, and the reports cover discussions on the memory buffer protocol, garbage collection, free-threaded Python, and &quot;Spicycrab&quot;.

rss · LWN.net · Sep 30, 14:32

**「Background」** The Python Language Summit is an annual gathering where Python core developers discuss proposed changes to the language and runtime before they are implemented. The LWN notice points to the official post-summit reports from the 2026 meeting rather than providing technical details itself.

**Tags**: `#Python`, `#Python Language Summit`, `#free-threaded Python`, `#garbage collection`, `#memory buffer protocol`

---

<a id="item-tech-news-13"></a>
### [Chromium developer contrasts Google and Igalia work cultures](https://lwn.net/Articles/1094721/) ⭐️ 6.0/10

Sharon Yang, a Chromium developer who previously worked on the browser at Google and now works on it at Igalia, gave a presentation on the final day of FOSSY 2026 comparing how the two organizations operate and how that affects work on the codebase. She said she enjoyed working at both companies and framed the talk not as a complaint but as a way to convey what it feels like to work at the two rather different companies.

rss · LWN.net · Sep 30, 14:16

**「Background」** Chromium is an open-source browser project developed by a community of companies and individuals, with Google as its original and largest contributor and Igalia among the other organizations working on the codebase. Yang&\#x27;s presentation offered a developer-level view of how two contributors with very different corporate cultures approach that shared project.

**Tags**: `#chromium`, `#open-source`, `#igalia`, `#google`, `#browser-development`

---

<a id="item-tech-news-14"></a>
### [Qwen-family LLMs dominate backbones in 100+ audio models survey](https://www.reddit.com/r/MachineLearning/comments/1wuctrt/qwenfamily_llms_are_quietly_becoming_the_backbone/) ⭐️ 6.0/10

A community architecture survey of the audio.cpp model collection reports that Qwen-family large language models are the most common language backbone across more than 100 audio models, with 32 model families using a Qwen architecture and 20 specifically using Qwen3. The analysis found Qwen-based models spanning TTS and speech synthesis, ASR/audio understanding, music generation, speech-to-speech, and audio/video tasks. This is an observational mapping by one Reddit user, not an official release or benchmark.

reddit · r/MachineLearning · /u/Acceptable-Cycle4645 · Sep 30, 18:31

**「Background」** Many modern audio AI systems are composite models: a pretrained large language model serves as the shared language backbone while separate components handle audio encoding, understanding, and synthesis. Because that backbone choice recurs across tasks, an architecture survey of an audio-model collection like audio.cpp can reveal which LLM family is most commonly reused, which is what this post&\#x27;s charts do.

**「Impact」** Developers choosing an LLM backbone for audio work can treat Qwen3 as a frequently used option based on this survey, but decisions should still be verified against per-task benchmarks because the post provides no performance or quality measurements.

**Tags**: `#audio models`, `#LLM backbones`, `#Qwen`, `#speech AI`, `#architecture survey`

---

<a id="item-tech-news-15"></a>
### [LessThink-Qwen3-4B claims 44% fewer reasoning tokens](https://www.reddit.com/r/MachineLearning/comments/1wtygav/lessthinkqwen34b_the_same_model_with_far_less/) ⭐️ 6.0/10

The author reports post-training Qwen3-4B into LessThink-Qwen3-4B, which uses about 44% fewer reasoning tokens while keeping the model&\#x27;s knowledge and answer style, with the entire pipeline run on a single GPU. This is a user-reported result without public benchmarks, independent validation, or a detailed comparison to existing reasoning-efficiency methods, so the quality and generalizability of the efficiency gain remain unverified.

reddit · r/MachineLearning · /u/stey1r · Sep 30, 07:19

**「Background」** The author&\#x27;s approach post-trains the existing Qwen3-4B model, a 4-billion-parameter language model, to reduce the token count used during reasoning while maintaining the original knowledge and answer style. The entire fine-tuning pipeline runs on a single GPU.

**Tags**: `#reasoning efficiency`, `#model compression`, `#post-training`, `#Qwen`, `#LLM optimization`

---

<a id="item-tech-news-16"></a>
### [ORTUS AI open-sources RightWayUp 360° image rotation detection model](https://www.reddit.com/r/MachineLearning/comments/1wu6reb/opensourcing_rightwayup_a_360degree_image/) ⭐️ 6.0/10

ORTUS AI has open-sourced RightWayUp, an Apache-2.0 image rotation detection model that estimates how far an image is rotated from upright across all 360° and abstains when there is no clear up. It is available in six sizes from Pico, small enough to run in a browser, to Max, which scored 98.8% within 10° on the Woehrer 2026 COCO-based benchmark \(five-seed mean\) versus Woehrer&\#x27;s 98.0%, and 93.0% on held-out tests versus 88.4%. The authors also report that re-saving the COCO-based benchmark images as JPEG q90 drops Woehrer 2026 to 30.2% while RightWayUp barely moves, suggesting a JPEG-grid artifact in that benchmark. Code and weights are released on GitHub, with the team noting that parts of the engineering were done using Claude and Codex.

reddit · r/MachineLearning · /u/wildtinkerer · Sep 30, 14:42

**「Background」** Existing image rotation detection models often struggle with CCTV frames, producing low accuracy and many false positives when the camera is installed at an angle. The Woehrer 2026 model, released earlier this year, was one of the better prior approaches on the COCO-based rotation benchmark, achieving 98.0% accuracy within 10° in that benchmark.

**「Impact」** Video analytics developers can now integrate a permissively licensed rotation detector to identify tilted or upside-down CCTV cameras, including a browser-sized Pico variant for lightweight deployments. Because the reported JPEG-shortcut result indicates existing rotation benchmarks may reward models that exploit JPEG-grid cues, teams evaluating rotation models should validate performance on compressed images before relying on benchmark scores.

**Tags**: `#computer vision`, `#image rotation`, `#open source`, `#machine learning`, `#Apache-2.0`

---

<a id="item-tech-news-17"></a>
### [McDonald&\#x27;s Reportedly Uses AI to Set Burger Prices by Willingness to Pay](https://www.engadget.com/2272211/mcdonalds-is-reportedly-using-ai-to-dynamically-price-its-burgers/) ⭐️ 6.0/10

McDonald&\#x27;s is reportedly using AI to adjust burger prices in the US and some overseas markets, with an algorithm setting each store&\#x27;s price based on estimated customer willingness to pay. The same item can cost different amounts at nearby locations: in Fresno, California, two outlets about 3 km apart sold the Big Mac for $5.69 and $6.89, a 21% difference. McDonald&\#x27;s called the reporting speculative and said the pricing tool is only a suggestion, not a mandate, but several franchisees told Reuters they have been pressured to adopt the algorithmic prices and that the company tracks whether stores follow them.

telegram · zaihuapd · Sep 30, 01:37

**「Background」** Dynamic pricing — changing the price of the same item by time, location, or demand — is common in ride-hailing and e-commerce but unusual in fast food, where chains typically rely on fixed local menu prices. The reported McDonald&\#x27;s system would extend that logic to individual franchise locations, so customers at stores in the same city can pay different amounts for the identical burger.

**「Impact」** The main reported consequence is for franchisees: McDonald&\#x27;s allegedly tracks whether locations comply with the algorithm&\#x27;s suggested prices, so owner-operators who resist the tool could face company pressure even though the pricing is described as advisory. Customers are also directly affected when identical items carry different prices at nearby stores.

**Tags**: `#AI`, `#dynamic pricing`, `#McDonald&\#x27;s`, `#technology industry`, `#machine learning`

---

<a id="item-tech-news-18"></a>
### [Microsoft Uses Outsourced Contractors to Review Copilot Image Prompts and Outputs](https://www.404media.co/humans-reading-copilot-prompts-images/) ⭐️ 6.0/10

According to a report from 404 Media and The Verge, Microsoft employs hundreds of outsourced contractors to manually review user prompts, requests, and uploaded images sent to Microsoft Copilot in order to improve its image generation and editing capabilities. This means that data shared with Copilot is not completely private, as human reviewers can view potentially sensitive personal photos and request content. The contractors are reportedly exposed to large volumes of harmful and explicit material, including upskirt photographs and animal sacrifice imagery, causing psychological distress.

telegram · zaihuapd · Sep 30, 07:13

**「Background」** AI image features such as Microsoft Copilot generally depend on human-in-the-loop evaluation: outside contractors review real user prompts, uploaded photos, and generated images to rate quality and safety so the model can be improved \(tool-1-1, tool-1-2, tool-1-3\). That behind-the-scenes review process is what exposes contractors to the sexually explicit and abusive image requests described in the current report.

**「Impact」** Users who share private or sensitive images via Microsoft Copilot should assume those images may be manually reviewed by human contractors, posing a clear privacy risk. Individuals may wish to avoid uploading personal, identifiable, or explicit photos to the service unless they are comfortable with potential human access.

<details><summary>References</summary>
<ul>
<li><a href="https://digg.com/tech/08d5740c-6bfb-45c5-b7e4-a8c21ecc2e3d">Human contractors reportedly review Copilot users’ prompts and...</a></li>
<li><a href="https://cybernews.com/ai-news/copilot-human-reviewers-sexual-ai-content-prompts/">Depraved Microsoft Copilot prompts reviewed by human contractors</a></li>
<li><a href="https://www.malwarebytes.com/blog/ai/2026/09/humans-are-reviewing-copilot-users-bizarre-and-abusive-image-editing-requests">Humans are reviewing Copilot users&#x27; bizarre and... | Malwarebytes</a></li>

</ul>
</details>

**Tags**: `#Microsoft Copilot`, `#AI ethics`, `#content moderation`, `#privacy`, `#AI industry`

---

<a id="item-tech-news-19"></a>
### [Kimi K3 Now Available via OpenAI Codex with Enterprise Billing Integration](https://36kr.com/newsflashes/4005691489112198) ⭐️ 6.0/10

American AI infrastructure company Baseten announced that enterprise users can now access Kimi K3 within OpenAI Codex, with usage fees applied to existing OpenAI procurement commitments. This integration marks the first time a Chinese open-source model has entered OpenAI&\#x27;s enterprise billing system, eliminating the need for separate vendor procurement.

telegram · zaihuapd · Sep 30, 11:23

**「Background」** Baseten, an AI infrastructure company, previously partnered with OpenAI to serve open models natively within Codex and the Responses API. Kimi K3, an open-source model from Chinese AI startup Moonshot AI, is now the first model from China to be offered through that enterprise billing channel, allowing customers to consume inference via their existing OpenAI commitments.

**「Impact」** For enterprises with existing OpenAI commitments, using Kimi K3 through Codex simplifies procurement and billing, potentially accelerating adoption of Chinese open-source models in enterprise AI workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baseten.co/blog/baseten-openai-partnership/">Announcing our partnership with OpenAI</a></li>

</ul>
</details>

**Tags**: `#Kimi K3`, `#OpenAI Codex`, `#Baseten`, `#AI enterprise procurement`, `#open source models`

---

<a id="item-tech-news-20"></a>
### [Apple Plans October 13 Launch of Smart Home Hub with Siri AI](https://www.bloomberg.com/news/articles/2026-09-30/apple-is-finally-ready-to-enter-its-next-big-category-the-smart-home) ⭐️ 6.0/10

Apple reportedly plans to enter the smart home market on October 13 with a new hub \(codenamed J490\) featuring a roughly 6-inch screen, facial and voice recognition, and an upgraded Siri AI. The hub will recognize family members, display personalized content, and control connected devices. Alongside the hub, Apple is expected to refresh the HomePod mini and Apple TV, though the products have not been officially announced and Apple declined to comment. This move marks Apple’s first dedicated home hub, differentiating it from voice-only competitors by combining a display with biometric and AI capabilities.

telegram · zaihuapd · Sep 30, 12:56

**「Background」** Apple has long offered smart home integration through its HomeKit software framework and voice control via HomePod speakers, but it never released a dedicated hub device with a screen. The reported J490 hub would be Apple&\#x27;s first standalone smart home controller, moving beyond the HomePod and Apple TV as HomeKit hubs.

**「Impact」** If the reported plans materialize, Apple ecosystem users will gain a dedicated hub for home automation that can identify individuals and tailor controls, potentially deepening integration with existing HomeKit devices and strengthening Apple’s position against Amazon’s Echo Show and Google’s Nest Hub. Developers may face new opportunities and fragmentation: the hub likely runs a variant of tvOS or HomePod software, requiring adaptation of SiriKit and HomeKit apps to support the new facial-recognition and on-screen personalization features.

**Tags**: `#apple`, `#smart-home`, `#siri`, `#hardware`, `#ai-assistant`

---

<a id="item-tech-news-21"></a>
### [Bilibili Open-Sources Index-Translate Translation Models](https://www.ithome.com/1/008/914.htm) ⭐️ 6.0/10

Bilibili&\#x27;s Index LLM team has open-sourced Index-Translate, a family of multilingual translation models with 2B, 9B, and 35B-A3B \(preview\) parameter sizes. Model weights are now available on Hugging Face and ModelScope, supporting 150 languages. Built on Qwen3.5, the models offer controllable translation features such as terminology, format, and content preservation, as well as extended capabilities for speech, syllable-controllable translation, and long-document translation. The 35B-A3B variant is currently released as a preview.

telegram · zaihuapd · Sep 30, 14:08

**「Background」** Large multilingual translation model families are typically built by fine-tuning a pretrained LLM on translation data rather than training a translation system from scratch. Bilibili&\#x27;s Index-Translate follows this pattern by starting from Qwen3.5, so the release is a set of fine-tuned model weights that users can run or adapt directly rather than access only through an API.

**「Impact」** Developers can now download the Index-Translate open weights from Hugging Face or ModelScope and run multilingual translation locally, including long-document, speech, and controlled-output modes, without depending on a closed API. The 35B-A3B variant is a preview release, so it should be treated as experimental before production use.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/IndexTeam/Index-Translate-35B-A3B">IndexTeam/ Index - Translate -35B-A3B · Hugging Face</a></li>
<li><a href="https://github.com/bilibili/Index-Translate">GitHub - bilibili / Index - Translate · GitHub</a></li>

</ul>
</details>

**Tags**: `#open source`, `#machine translation`, `#LLM`, `#multilingual NLP`, `#AI models`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Prediction markets Kalshi and Polymarket face questions over trading volumes](https://www.cnbc.com/2026/09/30/kalshi-polymarket-trading-volume-scrutiny.html) ⭐️ 7.0/10

CNBC reports that industry observers are questioning whether trading volumes on prediction platforms Kalshi and Polymarket are inflated, citing unusual patterns such as nearly half of Kalshi&\#x27;s ether perpetual-futures dollar volume on Sept. 20 coming from trades around $5,500. Both companies deny wash trading or inorganic activity, and a reported CFTC examination of Kalshi&\#x27;s ether contracts could not be independently verified.

rss · CNBC Finance · Sep 30, 21:09

**「Background」** Prediction markets let people bet on the likelihood of future events, and both companies have cited surging volumes to support multibillion-dollar valuations, with Polymarket reportedly raising above $20 billion and Kalshi reportedly seeking a $40 billion valuation.

**「Impact」** If a material share of reported volume is manufactured, it could overstate the genuine trading demand behind those valuations and any future public listing, a concern that matters most for retail investors in the platforms.

**Tags**: `#prediction markets`, `#wash trading`, `#regulatory scrutiny`, `#valuation`, `#market integrity`

---

<a id="item-finance-news-2"></a>
### [Temasek plans Abu Dhabi and Riyadh offices as it expands Middle East push](https://www.cnbc.com/2026/09/30/singapores-temasek-expands-in-mideast-with-abu-dhabi-riyadh-offices-.html) ⭐️ 7.0/10

Singapore&\#x27;s state-owned investor Temasek plans to open offices in Abu Dhabi and Riyadh by the first half of 2027, expanding its Middle East presence as it bets on the region&\#x27;s long-term economic transformation. Temasek, which manages about $400 billion, said the offices will serve as hubs for the investor and its portfolio companies.

rss · CNBC Finance · Sep 30, 08:45

**「Background」** Temasek is already active in the Gulf: in 2025 its asset management arm Seviora opened an Abu Dhabi office and partnered with Mubadala Capital, and this May Temasek joined BlackRock, L&\#x27;IMAD and ADNOC to target $30 billion in infrastructure deals across the Persian Gulf and Central Asia. The push comes even as some flagship Gulf projects, especially under Saudi Arabia&\#x27;s Vision 2030, face delays due to tighter finances and fallout from the Iran war.

**Tags**: `#Temasek`, `#Middle East investment`, `#sovereign wealth fund`, `#Gulf economy`, `#infrastructure`

---

<a id="item-finance-news-3"></a>
### [China warns of retaliation against EU trade restrictions](https://www.cnbc.com/2026/09/30/china-warns-europe-increases-trade-pressure.html) ⭐️ 7.0/10

China&\#x27;s commerce ministry warned it will &quot;respond firmly&quot; if the European Union imposes restrictions on Chinese businesses or products ahead of high-level trade talks next week, as annual EU-China trade stands at nearly $1 trillion.

rss · CNBC Finance · Sep 30, 03:39

**「Background」** The EU is pushing to reduce its record trade deficit with China and has been considering measures that could cut off Chinese access to the European market, mirroring the U.S. Section 301 tariff approach. China&\#x27;s ministry said such steps would undermine mutual trust and disrupt the ongoing negotiations.

**Tags**: `#China-EU trade`, `#trade policy`, `#tariffs`, `#geopolitical risk`, `#supply chains`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [OpenAI Announces Report on AI Agents for Small Businesses and Partnership with ASBDC](https://x.com/OpenAI/status/2105373267171438779) ⭐️ 6.0/10

OpenAI published a report examining how small businesses use AI agents for tasks such as customer acquisition, product development, and financial management. The company also announced a new partnership with the Association of Small Business Development Centers \(ASBDC\) to offer hands-on AI training and local guidance to help small business owners adopt the technology.

twitter · OpenAI · Sep 30, 19:04

**「Background」** This is a promotional announcement from OpenAI dated September 30, 2026. The post says OpenAI has published a new report exploring how small businesses are putting AI agents to work, including tasks such as finding customers, building products, and managing finances. It also announces a partnership with the @ASBDC account to bring hands-on AI training and local guidance to small business owners. No independent background or verification for the report or the partnership was available in the supplied tool results; the provided results cover other OpenAI agent-related topics, such as security incidents and product pages, and are not directly relevant to this announcement.

**Tags**: `#OpenAI`, `#small business`, `#AI agents`, `#partnership`, `#report`

---