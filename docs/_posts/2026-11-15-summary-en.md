---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 66 items, 19 important content pieces were selected

---

**Technology News**
1. [SpaceX catches Starship upper stage after Flight 15](#item-tech-news-1) ⭐️ 8.0/10
2. [Lovable apps expose passport details and 200K private messages](#item-tech-news-2) ⭐️ 8.0/10
3. [PyPI project pages add clearer security and provenance signals](#item-tech-news-3) ⭐️ 7.0/10
4. [EFF Warns Tech Companies Are Redefining Privacy Again](#item-tech-news-4) ⭐️ 7.0/10
5. [Italy fines Meta $887M over Android photo access](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI Disbands Robotics Team, Shifts to General-Model Control](#item-tech-news-6) ⭐️ 7.0/10
7. [W5000 Unmanned Cargo Aircraft Completes Technical Verification Test Flights](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare Open-Sources Kitesurf AI Agent Browser](#item-tech-news-8) ⭐️ 7.0/10
9. [A Family Tree of Software Job Titles](#item-tech-news-9) ⭐️ 6.0/10
10. [KDE: The Documentary \[video\]](#item-tech-news-10) ⭐️ 6.0/10
11. [Survey Proposes Three-Decision Framework for AI Research Autonomy](#item-tech-news-11) ⭐️ 6.0/10
12. [Should Short-Horizon Price Forecasting Papers Benchmark Against Market-Implied Forecasts?](#item-tech-news-12) ⭐️ 6.0/10
13. [Google Exec Uses Gemini to Run Windows 11 on Foldable iPhone](#item-tech-news-13) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly ROCm Release](#item-ai-projects-1) ⭐️ 7.0/10
2. [LMCache Nightly Release](#item-ai-projects-2) ⭐️ 5.0/10

**Financial News**
1. [Nvidia turmoil and a Democratic Congress may reshape the AI trade, ETF experts say](#item-finance-news-1) ⭐️ 8.0/10
2. [Anthropic IPO said to exclude mainland China and Hong Kong investors](#item-finance-news-2) ⭐️ 8.0/10

**Twitter News**
1. [SpaceX First Uses Mechanical Arms to Catch and Recover Second-Stage Spacecraft](#item-twitter-news-1) ⭐️ 7.0/10
2. [Pieter Levels on user-uploaded furniture to 3D generation](#item-twitter-news-2) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SpaceX catches Starship upper stage after Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 8.0/10

SpaceX’s Flight 15 launched from Texas on November 13, 2026; the Starship upper stage deployed 26 Starlink V3 satellites, completed about 22.5 hours and 14 orbits, then returned to Starbase and was caught by the launch tower’s arms on its first orbital-return catch attempt. The Super Heavy booster did not attempt a tower catch: it aborted its return and was destroyed in a controlled splashdown in the Gulf of Mexico, with no cause disclosed.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**「Earlier Starship flights set the stage」** Flight 15 follows the 14th Starship launch, which Horizon’s September 29 digest reported as the first to reach orbit and deploy 26 Starlink satellites before ending early with a Pacific splashdown; that flight did not attempt a ship catch. On the current flight, the booster aborted its own tower catch and splashed down in the Gulf, leaving the ship upper stage as the first to be caught.

**「Community discussion」** Commenters compared Starship to a corrected Space Shuttle, removing solid boosters and side-mounted orbiter failure modes, and noted that the next proof would be re-flying and catching a caught ship again. One commenter estimated Falcon 9 is about 60% reusable by cost, while another said the outcome hinges on whether the heat shield holds up.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/spacex-starship-orbit-262d3c58d56bf7a525b49115d6c5dfe8">2026-09-29 — SpaceX Starship Reaches Orbit, Deploys Starlink Satellites</a></li>

</ul>
</details>

**Tags**: `#spacex`, `#starship`, `#reusable-rockets`, `#space-hardware`, `#aerospace`

---

<a id="item-tech-news-2"></a>
### [Lovable apps expose passport details and 200K private messages](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

A security analysis found that Lovable&\#x27;s AI-generated applications exposed passport details and more than 200,000 private messages due to insufficient Row-Level Security in Supabase backends. Lovable&\#x27;s head of security said the company scans every app before publishing, offers free SAST with a &quot;Fix&quot; option, and supports auto-fix, but the findings highlight the risk of permissive database defaults in AI code generation.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**「Background」** Lovable is an AI app-building platform whose generated applications commonly use Supabase as a Postgres-based backend. Supabase&\#x27;s Row-Level Security \(RLS\) policies control which rows each authenticated user can access; when RLS is insufficient or permissive, a client-side query can retrieve other users&\#x27; data. Lovable&\#x27;s Head of Security stated the root cause in the affected apps was insufficient RLS, while another commenter noted that Supabase&\#x27;s historical onboarding defaults made such misconfigurations easy.

**「Direct data exposure for affected app users」** At least 24,664 Lovable-generated apps exposed passport records, payment details, and more than 200,000 chat messages to unauthenticated database queries, putting affected users at risk of identity theft and account compromise. Developers who used Lovable should audit Row-Level Security settings and apply the platform&\#x27;s security fixes before publishing or continuing to operate these apps.

**「Community Discussion」** In Hacker News comments, SOLAR\_FIELDS argued that Supabase shares blame for its permissive defaults, and reported that the October 30 fix may not cover existing projects. Others called the incidents &quot;canaries in the coalmines&quot; and said AI-generated apps are easy targets that need deny-by-default databases and automated auth tests.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/security/lovable-ai-apps-expose-personal-information/">Lovable AI apps exposed sensitive data in open databases ...</a></li>
<li><a href="https://dailysecurityreview.com/cyber-security/24664-lovable-built-apps-leak-passports-and-chat-messages/">24,664 Lovable-Built Apps Leak Passports and Chat Messages</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI code generation`, `#Supabase`, `#Row-Level Security`, `#data exposure`

---

<a id="item-tech-news-3"></a>
### [PyPI project pages add clearer security and provenance signals](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI has launched redesigned project pages that surface security and provenance signals more clearly, such as whether a package has provenance attestation. The update is a UI change that exposes existing trust data rather than a new security mechanism or detection capability.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**「Background」** PyPI already exposes package provenance through attestations: a project page explains that provenance describes where a file came from and is shared as a verifiable record of build or publishing details \(tool-2-2\). The redesigned pages arrive after supply-chain concerns such as Horizon&\#x27;s October 22 digest report of a compromised LiteLLM 1.107.0 package on PyPI \(tool-1-2\).

**「Impact」** Developers can now check provenance status directly on a project page, but they should not treat the redesign as protection against malicious packages; it primarily aids in spotting formerly benign projects whose PyPI entries may have been compromised.

**「Community Discussion」** Commenters debated whether the emphasis on cloud-based trusted publishing increases centralization and lock-in, while others welcomed the shift toward keyless signing. Some also noted the change does not detect inherently malicious packages and that reusable workflow support is still lacking.

<details><summary>References</summary>
<ul>
<li><a href="https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/">2026-10-22 — Compromised LiteLLM 1.107.0 on PyPI Ships Credential Stealer and Backdoor</a></li>
<li><a href="https://pypi.org/project/amoorion-blogger/">amoorion-blogger · PyPI</a></li>

</ul>
</details>

**Tags**: `#python`, `#pypi`, `#security`, `#supply-chain`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [EFF Warns Tech Companies Are Redefining Privacy Again](https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again) ⭐️ 7.0/10

According to an Electronic Frontier Foundation analysis, technology companies are attempting to shift the concept of privacy in ways that could weaken user protections. The piece connects this shift to AI-driven surveillance, including AI meeting recorders and workplace transcription, and highlights opt-out challenges for employees.

hackernews · gslin · Nov 14, 12:45 · [Discussion](https://news.ycombinator.com/item?id=50496602)

**「Background」** Horizon&\#x27;s October 24 digest reported that Google updated its privacy policy to potentially use Gmail and Google Photos data for ad targeting, an announced policy change without confirmed rollout or opt-out details. That example illustrates the kind of privacy-policy shift the EFF now criticizes, where companies redefine what data use is permissible rather than seeking affirmative consent.

**「Community Discussion」** Commenter toddmorey reports that every professional meeting they attend is recorded by AI guests, making opting out seemingly impossible while staying employed, and asks whether anyone has made &\#x27;no AI notetaker&\#x27; a meeting norm. Others cite Article 12 of the UN Universal Declaration of Human Rights and suggest practical privacy measures, while one commenter questions why current recording products face less hostility than Google Glass did.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theverge.com/tech/1017600/google-personal-intelligence-privacy-policy-ads-update">2026-10-24 — Gmail and Google Photos data may target ads under updated Google policy</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#technology-policy`, `#AI`, `#surveillance`, `#EFF`

---

<a id="item-tech-news-5"></a>
### [Italy fines Meta $887M over Android photo access](https://www.reuters.com/world/italy-fines-meta-887-million-over-android-users-data-access-2026-11-14/) ⭐️ 7.0/10

Italy&\#x27;s privacy regulator fined Meta $887 million after finding its Facebook Android app accessed users&\#x27; photos, videos, and metadata without specific consent. The regulator said the photo-recommendation feature launched in 2023 was enabled by default with a vague permission prompt and affected about 20 million Italian users. Meta must make the feature opt-in by default and obtain separate consent within 60 days, or disable it for users without valid authorization.

hackernews · giuliomagnifico · Nov 14, 13:48 · [Discussion](https://news.ycombinator.com/item?id=50497009)

**「Regulatory context」** Under the EU GDPR and Italy&\#x27;s Privacy Code, photo content and metadata are personal data, and processing them requires specific, informed consent rather than a generic device permission. The Italian Garante enforces these rules and has a record of high-profile privacy actions, including the 2023 temporary ChatGPT block and a €20 million Clearview AI fine in 2022.

**「Impact」** Meta is required to change the feature to default-off and collect specific consent within 60 days; affected Android users in Italy should not have their photos used without explicit authorization.

**「Community Discussion」** Hacker News commenters asked why the equivalent iOS app was not penalized and how the Android app accessed photos without a visible consent prompt, while noting the article lacked technical details.

<details><summary>References</summary>
<ul>
<li><a href="https://gdprfine.com/dpa/italy-garante">Italian Garante GDPR Fines : Enforcement Record &amp; AI Cases</a></li>
<li><a href="https://www.recordinglaw.com/world-laws/world-data-privacy-laws/italy-data-privacy-laws/">Italy Data Privacy Laws: GDPR, Privacy Code &amp; Garante Guide (2026)</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#privacy`, `#Android`, `#data access`, `#regulation`

---

<a id="item-tech-news-6"></a>
### [OpenAI Disbands Robotics Team, Shifts to General-Model Control](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/) ⭐️ 7.0/10

OpenAI has disbanded its independent robotics team and reassigned those researchers to broader research groups, Fortune reported. The company says GPT-6 Astra and other general frontier models can now directly control robots, making a dedicated robotics team unnecessary, though the report offers no independent verification of that capability. OpenAI previously shut down a robotics team in 2020, rebuilt one in 2024 with Figure, ended that partnership in February 2025, and is still developing an in-house humanoid robot with a target first public demonstration in 2027.

telegram · zaihuapd · Nov 14, 04:00

**「Prior robotics reorganizations and model approach」** OpenAI has previously disbanded and rebuilt robotics teams: an early team was shut down in 2020, a new one created in 2024 with a Figure partnership, and the Figure collaboration ended in February 2025. Fortune also reports that OpenAI researchers initially thought video models such as Sora were the best robotics route before concluding that general frontier models, including GPT-6 Astra, could control robots directly.

<details><summary>References</summary>
<ul>
<li><a href="https://casrai.org/news/openai-disbands-robotics-team-2026">OpenAI Disbands Its Robotics Team: What It Means — CASRAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#robotics`, `#general AI models`, `#AI strategy`, `#humanoid robots`

---

<a id="item-tech-news-7"></a>
### [W5000 Unmanned Cargo Aircraft Completes Technical Verification Test Flights](https://www.ithome.com/1/027/068.htm) ⭐️ 7.0/10

The company developing the W5000 announced on Nov. 14 that the large unmanned cargo aircraft completed technical verification test flights in Otog Front Banner, Inner Mongolia, with climb, level flight, turns, descent, and approach/landing all performed as planned. The developer describes it as the world&\#x27;s largest unmanned cargo aircraft by payload, with a maximum takeoff weight of 10.8 tonnes, maximum payload of 5 tonnes, and design range of 2,600 km. It uses turboprop power and an autonomous flight with ground monitoring mode, designed so one crew can monitor six to seven aircraft simultaneously. The company expects airworthiness certification in the first half of 2027.

telegram · zaihuapd · Nov 14, 05:00

**「Background」** Large unmanned cargo aircraft still require airworthiness certification before commercial use. The W5000&\#x27;s technical verification flights are an earlier stage in that process; the developer says certification is expected in the first half of 2027.

**「Impact」** The aircraft&\#x27;s design calls for one crew to monitor six to seven aircraft at once, which, once certification is complete, could lower per-flight crew costs on regional cargo routes compared with conventional piloted freighters.

**Tags**: `#autonomous-cargo-aircraft`, `#unmanned-aerial-vehicle`, `#aviation`, `#logistics`, `#autonomous-systems`

---

<a id="item-tech-news-8"></a>
### [Cloudflare Open-Sources Kitesurf AI Agent Browser](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) ⭐️ 7.0/10

Cloudflare has released Kitesurf, an Apache 2.0-licensed stateless browser for AI agents built on Cloudflare Workers; code is published on GitHub. It parses HTML, processes CSS, and executes JavaScript without browser containers. Cloudflare says it is designed to use less CPU and memory than Chromium and to scale on demand across the Workers network.

telegram · zaihuapd · Nov 14, 09:33

**「Background」** Cloudflare Workers is Cloudflare&\#x27;s serverless edge platform that runs JavaScript across its global network. Kitesurf is built on Workers to parse HTML, handle CSS, and execute JavaScript directly without a browser container, which lets an AI agent avoid the CPU and memory overhead of a Chromium-based browser.

**「Impact」** AI agent developers can run lightweight web-page processing on Cloudflare Workers without deploying or managing Chromium browser containers, potentially reducing CPU and memory overhead for automated browsing workloads.

**Tags**: `#AI agents`, `#browser`, `#Cloudflare`, `#open source`, `#edge computing`

---

<a id="item-tech-news-9"></a>
### [A Family Tree of Software Job Titles](https://zwischenzugs.com/2026/11/03/a-family-tree-of-software-job-titles/) ⭐️ 6.0/10

A blog post maps the historical relationships and evolution of software job titles. The discussion highlights overlapping and ambiguous titles: one practitioner reports that roles like DevOps Engineer, Systems Development Engineer, and Site Reliability Engineer all described the same generalist work, while another says Scrum and Agile certifications now feel dated. The article is a descriptive taxonomy, not a new industry standard or policy change.

hackernews · umerf · Nov 14, 17:45 · [Discussion](https://news.ycombinator.com/item?id=50499038)

**「Background」** Software job titles are unstable and context-dependent. For example, the article notes that &quot;Systems Engineer&quot; referred to a pre-sales role at IBM in the 1960s and later became a senior, design-oriented sysadmin in the 1990s through Microsoft&\#x27;s MCSE certification.

**「Impact」** Software professionals evaluating or applying for roles may need to verify actual responsibilities rather than trust the title. Several commenters report that &quot;DevOps Engineer&quot; and &quot;SRE&quot; are used inconsistently and sometimes do not match the methodology they are named after.

**「Community Discussion」** A recurring disagreement is whether &quot;DevOps Engineer&quot; is a legitimate role or a contradiction, since DevOps is meant to be a culture rather than a job title. Commenter stroebs says every title they held except Cloud Infrastructure Engineer was &quot;meaningless,&quot; while siva7 reports dropping Scrum and Agile certifications because they felt obsolete.

<details><summary>References</summary>
<ul>
<li><a href="https://zwischenzugs.com/2026/11/03/a-family-tree-of-software-job-titles/">A Family Tree of Software Job Titles – zwischenzugs.com</a></li>

</ul>
</details>

**Tags**: `#software-engineering`, `#careers`, `#job-titles`, `#technology-industry`, `#devops`

---

<a id="item-tech-news-10"></a>
### [KDE: The Documentary \[video\]](https://tube.kockatoo.org/w/fFinNHfanLT7aBEb2B8y4c) ⭐️ 6.0/10

The item links to a video documentary about the history, technical challenges, and community behind the KDE desktop environment. No source content is available to verify specific production details, interviews, or release claims. The linked video is a historical and community retrospective, not a new software version or urgent development.

hackernews · mrkn1 · Nov 14, 13:43 · [Discussion](https://news.ycombinator.com/item?id=50496976)

**「Documentary scope and premiere」** The film covers KDE from Matthias Ettrich&\#x27;s 1996 Usenet call for a better Linux desktop, through the Qt licensing fight and the KDE 4 release that nearly broke the community, to its later reemergence. An official KDE fundraiser page announced the documentary would premiere on October 14 at 19:30 CEST.

**「Community Discussion」** Commenters describe personal experiences: one recalls seeing the original Usenet post seeking volunteers for the “Kool Desktop Environment” and the enthusiasm around early betas. Others praise KDE 3 applications such as Amarok 1.4 and k3b while criticizing KDE 4 as unstable.

<details><summary>References</summary>
<ul>
<li><a href="https://kde.org/fundraisers/yearend2026/">The next 30 years start here - KDE Community</a></li>
<li><a href="https://m-zone.cc/details/movie/1777637">KDE : The Documentary Movie Details - M-Zone</a></li>

</ul>
</details>

**Tags**: `#KDE`, `#open source`, `#desktop environment`, `#documentary`, `#software history`

---

<a id="item-tech-news-11"></a>
### [Survey Proposes Three-Decision Framework for AI Research Autonomy](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+%E3%80%8C%E8%AE%A9AI%E7%A0%94%E7%A9%B6AI%E3%80%8D%E6%9C%80%E6%96%B0%E7%BB%BC%E8%BF%B0%EF%BC%9A%E4%B8%89%E9%A1%B9%E5%85%B3%E9%94%AE%E5%86%B3%E7%AD%96%E6%A1%86%E6%9E%B6%EF%BC%8C%E9%87%8D%E6%96%B0%E5%AE%A1%E8%A7%86%E7%A0%94%E7%A9%B6%E8%87%AA%E4%B8%BB%E6%80%A7) ⭐️ 6.0/10

Nankai University and Zhongguancun College researchers have published a survey that proposes a framework for measuring how much research decision-making AI systems actually control. The survey decomposes AI-driven research into three decisions: search direction \(what to explore next\), search space \(which modifications are allowed\), and evaluation signal \(how results are judged\), and maps them to L0–L3 control-source levels. It reviews representative AI4AI work across learning, reasoning, data, and infrastructure, but is presented as a conceptual survey rather than a shipped system. The preprint is available at preprints.org \(manuscript 202610.2999\), with a project page at ai4ai-research.github.io.

rss · 新智元 · Nov 14, 09:03

**「What counts as research autonomy」** AI research agents can already read papers, write code, and run experiments, but the reported survey argues that these capabilities do not by themselves determine how much of the research process is automated. The three-decision framework is intended to distinguish executing a human-defined plan from making choices about where to search, what to allow, and how to judge success.

**「Impact」** For developers of AI research agents, the L0–L3 control-source framework offers an audit tool to explicitly assign human or AI control over search direction, search space, and evaluation signal, making it easier to compare systems and identify whether an agent is merely executing predefined experiments or actually choosing research directions.

**Tags**: `#AI research`, `#research autonomy`, `#survey`, `#machine learning`, `#AI agents`

---

<a id="item-tech-news-12"></a>
### [Should Short-Horizon Price Forecasting Papers Benchmark Against Market-Implied Forecasts?](https://www.reddit.com/r/MachineLearning/comments/1xw6fk9/should_shorthorizon_price_forecasting_papers/) ⭐️ 6.0/10

A Reddit post asks why short-horizon crypto and commodity price forecasting papers rarely compare against market-implied forecasts or evaluate interval coverage. The author notes that most papers using transformers or LSTMs benchmark only against ARIMA, a random walk, or a simple LSTM and report lower RMSE. They argue that beating naive baselines is not meaningful unless models also beat market expectations from options-implied volatility or prediction markets, and that for assets like BTC, coverage of an 80% interval is more informative than RMSE.

reddit · r/MachineLearning · /u/happypeanut-t · Nov 14, 16:23

**「Existing crypto price forecasting benchmarks」** The poster&\#x27;s observation reflects standard practice in many short-horizon crypto price forecasting papers, which compare point forecasts from ARIMA, random-walk, and LSTM baselines using RMSE. Existing published benchmarking studies illustrate this model-comparison framing; for example, a 2024 ScienceDirect comparative analysis contrasts traditional statistical methods with ensemble and deep learning, and a 2025 Springer study benchmarks hourly and daily crypto price predictions using market indicators and social media data.

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s13278-025-01520-0">Benchmarking modeling architectures for cryptocurrency price ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1057521923005719">Cryptocurrency price forecasting – A comparative analysis of ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#forecasting`, `#model evaluation`, `#finance`, `#benchmarking`

---

<a id="item-tech-news-13"></a>
### [Google Exec Uses Gemini to Run Windows 11 on Foldable iPhone](https://www.windowslatest.com/2026/11/14/windows-11-can-run-on-apples-foldable-iphone-and-googles-ai-boss-proved-it-using-gemini-years-after-microsoft-gave-up-on-windows-phones/) ⭐️ 6.0/10

Ammaar Reshi, product design lead at Google AI Studio, demonstrated Windows 11 24H2 running locally on an Apple foldable iPhone Duo using Gemini 4 Carbon. The setup relies on the open-source WindowsiOS project, which uses JIT translation to execute ARM64 code without jailbreaking, and supports Microsoft Prism for some legacy applications. The ~12 GB image requires an Apple Silicon Mac and developer tools, and the feat is a community-documented demo rather than an official product.

telegram · zaihuapd · Nov 14, 06:52

**「Background」** The demonstration builds on WindowsiOS, an open-source project that runs Windows 11 on unjailbroken iOS devices by using JIT translation for ARM64 code and Microsoft Prism for some traditional x86 applications. The setup typically requires an Apple Silicon Mac and development tools, with a disk image around 12 GB.

**「Impact」** For OS and emulation enthusiasts, this shows that Windows 11 can run on recent iPhones via a non-jailbreak community tool, but practical use is limited by the 12 GB image size, JIT translation overhead, and the need for an Apple Silicon Mac and development environment.

**Tags**: `#Windows 11`, `#iOS`, `#JIT emulation`, `#Gemini AI`, `#Open source`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly ROCm Release](https://github.com/LMCache/LMCache/releases/tag/nightly-rocm) ⭐️ 7.0/10

This nightly release provides ROCm 7.2 wheels of LMCache for AMD Instinct MI300X/MI325X \(gfx942\) and MI350X/MI355X \(gfx950\), ABI-matched to upstream vLLM ROCm containers, allowing pip installation into those containers.

github · github-actions\[bot\] · Nov 14, 07:47

**「解决的痛点」** It solves the lack of a ready-to-install LMCache build for AMD GPUs. Previously, using LMCache on ROCm required compiling from source or dealing with dependency mismatches. These wheels are ABI-matched to the torch 2.13/cp312 environment of upstream vLLM ROCm images, so users can simply pip install without breaking the container.

**「Background &amp; ecosystem impact」** This nightly release provides ROCm 7.2 wheels for AMD Instinct gfx942 \(MI300X/MI325X\) and gfx950 \(MI350X/MI355X\), ABI-matched to upstream vLLM ROCm containers \(torch 2.13, cp312\). In the broader AI ecosystem, LMCache serves as a KV cache management layer that turns transient KV cache into reusable state across serving engines \(tool-1-2\). Adding ROCm support extends LMCache beyond NVIDIA-centric deployments to AMD Instinct GPUs commonly used with vLLM, broadening platform coverage for enterprise-scale LLM inference.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#ROCm`, `#LLM inference`, `#AMD`, `#nightly`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly Release](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache nightly release provides pre-built Python wheels compiled against CUDA 13.0 for Linux amd64 and arm64, pulled directly from the development branch.

github · github-actions\[bot\] · Nov 14, 09:48

**「Problem Solved」** This release eliminates the need to manually compile LMCache from source for CUDA 13.0 environments. Users can install compatible wheels directly via pip, reducing setup complexity and potential build failures.

**「Background and ecosystem context」** LMCache is a KV cache management layer for LLM inference that turns transient KV cache into reusable, persistent knowledge across requests and engine instances \[tool-1-1\]\[tool-1-2\]. This nightly release provides prebuilt CUDA 13.0 wheels from the dev branch for Linux amd64 and arm64, allowing early adopters to install and test the latest unreleased code against PyTorch&\#x27;s cu130 index without building from source. As a nightly snapshot, it is primarily an infrastructure update rather than a feature release, extending compatibility with newer CUDA and Arm environments for developers who track upstream changes.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache ! | LMCache</a></li>
<li><a href="https://github.com/LMCache/LMCache">GitHub - LMCache / LMCache : LMCache : Supercharge Your LLM with...</a></li>

</ul>
</details>

**Tags**: `#llm-infrastructure`, `#cuda`, `#nightly`, `#release`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nvidia turmoil and a Democratic Congress may reshape the AI trade, ETF experts say](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 8.0/10

Nvidia founder and CEO Jensen Huang resigned after a week in which the stock posted its longest losing streak since 2012, and ETF experts said investors may rotate AI capital from Nvidia toward other chipmakers, cloud companies and Big Tech. Yorkville Ives partner Dan Ives cut his Nvidia price target to $225 from $300 while maintaining a buy rating, as the stock closed the week at $162.85 per share.

rss · CNBC Finance · Nov 14, 15:50

**「Background」** The remarks on CNBC&\#x27;s &quot;ETF Edge&quot; came after the Nov. 3 Democratic sweep of Congress, which ETF experts said could slow data-center construction; Nvidia&\#x27;s interim CEO Colette Kress is scheduled to report third-quarter earnings next Tuesday.

**Tags**: `#Nvidia`, `#AI trade`, `#ETFs`, `#data centers`, `#semiconductors`

---

<a id="item-finance-news-2"></a>
### [Anthropic IPO said to exclude mainland China and Hong Kong investors](https://m.economictimes.com/markets/us-stocks/news/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed/articleshow/135809948.cms) ⭐️ 8.0/10

Anthropic&\#x27;s reported IPO is said to bar investors from mainland China and Hong Kong because of U.S. International Traffic in Arms Regulations \(ITAR\) export controls, as the company targets a $1.4 trillion valuation and up to $90.4 billion in proceeds.

telegram · zaihuapd · Nov 14, 10:18

**「Background」** This follows SpaceX&\#x27;s record IPO, which also barred China and Hong Kong investors, citing US export rules.

**「Impact」** Some affected investors are reportedly routing money into British Virgin Islands trusts, special purpose vehicles, and swap structures, with demand about six times the shares available.

<details><summary>References</summary>
<ul>
<li><a href="https://thedailybugle.bartlettpublications.com/p/26-0616-tuesday-s-export-import-daily-bugle">26-0616: Tuesday&#x27;s &quot; Export /Import Daily Bugle&quot;</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO`, `#export controls`, `#China`, `#valuation`

---

## Twitter News

<a id="item-twitter-news-1"></a>
### [SpaceX First Uses Mechanical Arms to Catch and Recover Second-Stage Spacecraft](https://x.com/op7418/status/2121756191495954772) ⭐️ 7.0/10

A tweet by 歸藏 \(guizang.ai\) posted on 2026-11-15 announces that SpaceX has for the first time used mechanical arms to catch and recover a second-stage spacecraft. The tweet expresses enthusiasm \(🐂🍺\) and includes a link to the original media or report.

twitter · 歸藏\(guizang.ai\) · Nov 15, 00:04

**「Background」** On 2026-11-15, X user @op7418 \(歸藏/guizang.ai\) posted that SpaceX had for the first time used mechanical arms to catch and recover a second-stage spacecraft. The post links to external content but does not include technical details.

SpaceX&\#x27;s Starship system consists of a Super Heavy booster and a second-stage spacecraft, with full reusability as a central goal \[tool-1-1\]. The launch tower uses &\#x27;chopstick&\#x27; arms referred to as Mechazilla \[tool-1-2\]. Previously documented catch milestones focused on the first-stage booster: on 13 October 2024, SpaceX performed a historic booster catch after a Starship test flight \[tool-1-1\]\[tool-1-3\]. That event was described as the first-ever mechanical catch of a returning orbital rocket booster \[tool-1-2\].

No supplied tool results confirm a prior mechanical-arm catch of a second-stage spacecraft, so the tweet may describe a new milestone beyond the documented booster catch, or may conflate the stages; the available evidence does not resolve this. No community comments were available.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/roderick-beck-94868948_spacex-catches-starship-rocket-booster-in-activity-7253027931701080064-WUgI">SpaceX catches Starship rocket booster in historic test launch</a></li>
<li><a href="https://satfleetlive.com/blogs/spacex-starship/">SpaceX Starship : Next Flight, Full History &amp; Everything... | SatFleet Live</a></li>
<li><a href="https://www.france24.com/en/live-news/20241013-spacex-will-try-to-catch-giant-starship-rocket-shortly-before-landing">SpaceX successfully catches returning Starship booster... - France 24</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starship`, `#space technology`, `#engineering`, `#news`

---

<a id="item-twitter-news-2"></a>
### [Pieter Levels on user-uploaded furniture to 3D generation](https://x.com/levelsio/status/2121712181125525706) ⭐️ 6.0/10

Pieter Levels proposes an alternative to building a large furniture library: let users upload a photo of their own furniture and convert it into a 3D object in under 30 seconds using an image-to-3D model.

twitter · @levelsio · Nov 14, 21:09

**「Background」** The tweet, published on November 14, 2026 by @levelsio, frames this approach as a practical workaround to the effort of assembling a giant furniture catalog. It assumes the availability of an image-to-3D model capable of generating a usable 3D object quickly.

**Tags**: `#AI`, `#3D generation`, `#user-generated content`, `#product design`

---