---
layout: default
title: "Horizon Summary: 2026-09-30 (EN)"
date: 2026-09-30
lang: en
---

> From 57 items, 24 important content pieces were selected

---

**Technology News**
1. [AI Has Taste finds a counterexample to a published conjecture, author confirms](#item-tech-news-1) ⭐️ 9.0/10
2. [GLM-5.3 and Claude Mythos Preview Cross Binary Exploitation Threshold](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI DevDay 2026 Introduces Dots, GPT-6.1 Sol and Ultrafast, and New APIs](#item-tech-news-3) ⭐️ 8.0/10
4. [Anthropic Report: GLM-5.3 Shows Autonomous Cyberattack Capabilities](#item-tech-news-4) ⭐️ 8.0/10
5. [OpenAI introduces cheaper GPT-6.1 Sol with claimed near-Astra performance](#item-tech-news-5) ⭐️ 7.0/10
6. [Privacy analysis exposes data-exposure risks in AI chat services](#item-tech-news-6) ⭐️ 7.0/10
7. [OpenAI introduces Dots, an always-on agent product](#item-tech-news-7) ⭐️ 7.0/10
8. [PostgreSQL developer talks Linux kernel support at Kernel Recipes](#item-tech-news-8) ⭐️ 7.0/10
9. [Language Models for Text Classification: From Bag-of-Words to Jev](#item-tech-news-9) ⭐️ 7.0/10
10. [China&\#x27;s generative AI users exceed 700 million](#item-tech-news-10) ⭐️ 7.0/10
11. [Cloudflare launches cf CLI open beta for AI agents and developers](#item-tech-news-11) ⭐️ 7.0/10
12. [Google fixes Firebase Analytics server bug behind iOS startup crashes](#item-tech-news-12) ⭐️ 7.0/10
13. [How Delhi Cut Electricity Distribution Losses From 50% to 5%](#item-tech-news-13) ⭐️ 6.0/10
14. [Relapse-Exploit: PS5 WebKit JavaScriptCore Jailbreak Exploit Published](#item-tech-news-14) ⭐️ 6.0/10
15. [Rust-GPU maintainer proposes native Rust compilation to GPU](#item-tech-news-15) ⭐️ 6.0/10
16. [Linux distributions release weekly security updates](#item-tech-news-16) ⭐️ 6.0/10
17. [Free open-source book explains how to actually make ML models fast](#item-tech-news-17) ⭐️ 6.0/10
18. [CoWindow and MassAlloc Attention: Sparse Collective Coverage, Adaptive Tiles](#item-tech-news-18) ⭐️ 6.0/10
19. [Codex Pro $200 subscription reopens with halved quota](#item-tech-news-19) ⭐️ 6.0/10

**Financial News**
1. [FHFA Mortgage Pricing Change Sinks Fair Isaac; AMD Buys World Labs](#item-finance-news-1) ⭐️ 8.0/10
2. [Oracle Invokes Force Majeure on Stargate Data Center Due to Power Delays](#item-finance-news-2) ⭐️ 8.0/10
3. [China to Subsidize First-Home Mortgage Interest From Oct 1](#item-finance-news-3) ⭐️ 8.0/10
4. [Trump’s municipal bond portfolio reaches estimated $300 million to $1 billion](#item-finance-news-4) ⭐️ 7.0/10
5. [China reportedly tightens IPO criteria for humanoid-robot startups](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AI Has Taste finds a counterexample to a published conjecture, author confirms](http://weixin.sogou.com/weixin?type=2&amp;query=%E6%96%B0%E6%99%BA%E5%85%83+AI%E6%89%BE%E5%87%BA%E6%95%B0%E5%AD%A6%E5%8F%8D%E4%BE%8B%E6%8E%A8%E7%BF%BB%E8%AE%BA%E6%96%87%EF%BC%8C%E4%BD%9C%E8%80%85%E7%A1%AE%E8%AE%A4%EF%BC%81453%E7%AF%87%E6%89%8B%E7%A8%BF%EF%BC%8CAI%E5%BC%80%E5%A7%8B%E8%87%AA%E5%B7%B1%E5%87%BA%E9%A2%98%E4%BA%86) ⭐️ 9.0/10

AI Has Taste, an automated mathematics research system built by UCSI University researcher Zeng Zaijian, has publicly documented 453 mathematical research manuscripts and 2,312 pages in its GitHub repository, including 6 items classified as “AI-Proposed Conjectures.” The project’s reported breakthrough was an AI-generated counterexample that overturned a conjecture from a published paper; Zeng says he sent the counterexample to the original author, who replied confirming it was valid. The repository frames the system as moving “from answer generation to research-agenda generation,” though the confirmed counterexample and the manuscript collection are project-reported rather than independently peer-reviewed.

rss · 新智元 · Sep 29, 03:40

**「Background」** AI Has Taste is an automated mathematical research system built by researcher Zeng Zaijian at UCSI University. Before the reported milestone, the project had already produced 453 mathematical manuscripts and 2312 pages of content, with 6 classified as AI-proposed conjectures, after its pivotal discovery: when given a published paper&\#x27;s conjecture, the AI constructed a counterexample rather than a proof, which the original paper&\#x27;s author later confirmed as valid.

**「Impact」** Mathematicians and peer reviewers now face a confirmed case of an AI system autonomously disproving a published conjecture, with the original author acknowledging the counterexample. The project’s public repository \(453 manuscripts, 6 AI-proposed conjectures\) indicates that automated counterexample generation and conjecture proposal are scaling beyond isolated experiments, which may push the research community toward incorporating automated falsification checks into validation workflows before publication.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ArtificialZeng/AI-Has-Taste">GitHub - ArtificialZeng / AI - Has - Taste : 200+ open problems in...</a></li>

</ul>
</details>

**Tags**: `#AI for mathematics`, `#counterexample finding`, `#automated reasoning`, `#machine learning`, `#scientific verification`

---

<a id="item-tech-news-2"></a>
### [GLM-5.3 and Claude Mythos Preview Cross Binary Exploitation Threshold](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 8.0/10

Anthropic&\#x27;s Frontier Red Team reports that GLM-5.3 and Claude Mythos Preview can achieve full control flow hijacks in binary exploitation tasks—GLM-5.3 in 4% of trials and Claude Mythos Preview in 6%—while earlier models like Claude Opus 4.6 and GLM-5.2 succeeded in none. This marks a crossing of a meaningful capability threshold for current frontier models, based on a random sample of 100 tasks from an internal Binary Exploitation benchmark.

rss · Simon Willison · Sep 29, 22:20

**「Background」** Binary exploitation is the practice of turning memory-corruption bugs into &quot;control flow hijacks,&quot; where an attacker redirects a program&\#x27;s execution to their own code. Anthropic&\#x27;s Frontier Red Team measured these capabilities in its new report; on the separate ExploitBench benchmark, GLM-5.3 produced end-to-end exploits in 50 of 410 attempts and Claude Mythos Preview did so in 56 of 410 attempts, a similar rate.

**「Impact」** For AI safety researchers and software defenders, this result shows that state-of-the-art language models can autonomously perform binary exploitation techniques in a small but non-zero fraction of attempts, shifting the threat model for automated vulnerability exploitation and reinforcing the need for robust mitigation measures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://ai-tldr.dev/releases/anthropic-glm-5-3-cyber-report/">Anthropic tests GLM-5.3 — its safeguards fall to… | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#Anthropic`, `#binary exploitation`, `#cyber capabilities`, `#language models`

---

<a id="item-tech-news-3"></a>
### [OpenAI DevDay 2026 Introduces Dots, GPT-6.1 Sol and Ultrafast, and New APIs](https://openai.com/zh-Hant/index/devday-2026-recap/) ⭐️ 8.0/10

OpenAI at DevDay 2026 launched the Dots persistent agent that runs autonomously around the clock, learns user habits, and can take over long-running complex tasks. The company also released GPT-6.1 Sol, a coding and computer-control model that delivers near-Astra intelligence at one-fifth the price, and Astra Ultrafast, which achieves up to 8× speedup on the client side and 6× via API. New offerings include an Agents API with native computer control and AWS Bedrock hosting, a Decisions API for lightweight classification and routing, “Sign in with ChatGPT” for transferring subscription credits to third-party tools like Devin and Notion, and a Pro 500 tier that provides 25× the compute of Plus and exclusive access to Astra Ultrafast.

telegram · zaihuapd · Sep 29, 17:52

**「Background」** Horizon&\#x27;s September 27 digest reported that OpenAI planned to broaden access to its Ultrafast API around the September 29 DevDay; the mode was previewed with GPT-5.6 Sol, reportedly reaching up to 750 tokens per second at 14x the inference speed of the Standard tier, with GPT-6 support still uncertain. The DevDay recap now confirms the rollout: Ultrafast ships as GPT-6.1 Ultrafast alongside the programming-focused GPT-6.1 Sol, with OpenAI claiming up to 8x speed gains over standard Astra \(6x via API\) and bundling Ultrafast into the new Pro 500 tier.

**「Impact」** Developers can now build and deploy persistent, learning-based agents for autonomous task execution, and integrate ChatGPT subscriptions into external tools. The new Pro 500 tier offers substantially higher compute for AI workloads, but its pricing and availability remain unspecified beyond the compute ratio.

<details><summary>References</summary>
<ul>
<li><a href="https://www.testingcatalog.com/openai-prepares-to-expand-ultrafast-api-to-more-users/">2026-09-27 — OpenAI reportedly expands Ultrafast API access around DevDay</a></li>

</ul>
</details>

**Tags**: `#openai`, `#gpt-6`, `#ai-agents`, `#codex`, `#api`

---

<a id="item-tech-news-4"></a>
### [Anthropic Report: GLM-5.3 Shows Autonomous Cyberattack Capabilities](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities) ⭐️ 8.0/10

Anthropic&\#x27;s evaluation of Zhipu AI&\#x27;s open-weight GLM-5.3 reports that the model can autonomously construct end-to-end cyberattacks, succeeding 50 times in 410 ExploitBench attempts, close to Claude Mythos Preview&\#x27;s 56 successes. Anthropic also found that GLM-5.3&\#x27;s safety measures could be bypassed with simple methods, achieving simulated test success rates of 64% to 100%, and that its open weights let users modify the model to weaken refusals. According to Anthropic, this could expand the cyberattack capabilities available to malicious actors.

telegram · zaihuapd · Sep 29, 23:58

**「Background」** GLM-5.3 is an open-weight model released by Chinese AI company Zhipu AI \(智谱 AI\). Open-weight models allow users to download and modify the model weights, which can enable removal of safety guardrails and fine-tuning for malicious purposes. Anthropic’s evaluation tested GLM-5.3’s ability to autonomously conduct cyberattacks using ExploitBench, a benchmark for measuring exploit development capabilities.

**「Impact」** The evaluation suggests that GLM-5.3 may meaningfully lower the barrier to end-to-end cyberattacks for users who can access or modify the open-weight model, so organizations deploying or fine-tuning it should account for its demonstrated offensive capability and the ease with which its safeguards can be removed.

**Tags**: `#AI safety`, `#cybersecurity`, `#GLM-5.3`, `#Anthropic`, `#open-weight models`

---

<a id="item-tech-news-5"></a>
### [OpenAI introduces cheaper GPT-6.1 Sol with claimed near-Astra performance](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 7.0/10

OpenAI has introduced GPT-6.1 Sol, a new model version that it claims delivers performance close to its higher-tier Astra model at roughly one-fifth the price. The release follows mixed reception to the GPT-6 series and is positioned as a more cost-effective option for developers. The specific pricing and availability details were not provided in the announcement, but the claim of near-Astra intelligence at a fraction of the cost has drawn both interest and skepticism among AI practitioners.

hackernews · crorella · Sep 29, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49896586)

**「Background」** GPT-6.1 Sol is a new OpenAI model released in September 2026 that offers performance close to the premium GPT-6 Astra at about one-fifth of Astra&\#x27;s per-token pricing \(tool-2-1, tool-2-2\). It follows the GPT-6 Sol and Astra models; third-party comparisons show it matches Astra on several agentic benchmarks while maintaining the same pricing as GPT-6 Sol \(tool-2-2, tool-2-3\). The model has a 1.1M-token context window and cached input pricing of $0.10 per million tokens \(tool-2-3\).

**「Community discussion」** Commenters expressed skepticism about OpenAI&\#x27;s recent model quality, with one user reporting that they had switched to Anthropic&\#x27;s Opus 5.5 after finding GPT-6 Sol unreliable for coding tasks. Others focused on the price reduction as the key differentiator, noting that cheaper cache pricing could offer far better value for heavy API users. The discussion reflects a broader debate between model capability and cost efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://smartscope.blog/en/blog/changed-gpt-6-1-sol-1-point-behind-2026/">What Changed in GPT - 6 . 1 Sol ? 1 Point Behind Astra at... - SmartScope</a></li>
<li><a href="https://www.datacamp.com/blog/gpt-6-1-sol">GPT - 6 . 1 Sol : Features, Benchmarks, Pricing , and Access | DataCamp</a></li>
<li><a href="https://llm-stats.com/models/gpt-6.1-sol">GPT - 6 . 1 Sol Benchmarks, Pricing &amp; Context Window</a></li>

</ul>
</details>

**Tags**: `#openai`, `#gpt`, `#llm`, `#ai-pricing`, `#machine-learning`

---

<a id="item-tech-news-6"></a>
### [Privacy analysis exposes data-exposure risks in AI chat services](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A new privacy analysis of web and mobile conversational AI agents \(PDF linked\) documents concrete data-exposure risks: unfinished prompts are transmitted to servers before the user submits them, and persistent UUID URLs can expose full conversation histories. The research identifies multiple AI chat services that share prompt data with advertising and analytics trackers, challenging the assumption that these tools offer meaningful privacy.

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**「Background」** &quot;Prompt like a Butterfly, Sting like a Tracker&quot; is a peer-reviewed research paper accepted at PoPETs 2027, led by IMDEA Networks researchers in collaboration with a legal expert. The study instrumented a custom browser and Android phones to observe what data leaves web and mobile clients of major conversational AI services, including ChatGPT, Claude, Grok, DeepSeek, Perplexity, Gemini, Copilot, Mistral Le Chat, and Meta AI, and where that data is sent. This background helps explain why the community comments focus on concrete data-exposure mechanics rather than general speculation: the paper&\#x27;s method directly traces telemetry flows from real AI chat clients.

**「Impact」** Users of Grok and Perplexity face a concrete risk that their private prompts and conversation contents are transmitted to third-party advertising platforms \(including Meta, TikTok, and Google\) via tracking pixels and weakly protected permalinks, as documented in the analyzed paper and corroborated by subsequent news reports and a class-action lawsuit. Affected users should avoid sharing or bookmarking conversation URLs and consider browser extensions that block known ad trackers to reduce exposure.

**「Community Discussion」** Commenters reported that ChatGPT periodically sends unfinished prompts to a \`conversation/prepare\` endpoint, which could be used for caching or tracking, and that services like Perplexity expose past conversations through persistent UUID URLs, undermining any illusion of privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf">Prompt like a Butterfly, Sting like a Tracker: A Privacy Analysis of</a></li>
<li><a href="https://jorgegarciaherrero.com/prompt-like-a-butterfly-sting-like-a-tracker-un-resumen-visual/">Resumen de &quot;Prompt like a butterfly, sting like a tracker&quot; - Jorge García Herrero y Asociados, abogados</a></li>
<li><a href="https://techxplore.com/news/2026-05-conversations-ai-private.html">Your conversations with AI may not be as private as you think</a></li>
<li><a href="https://gptanon.com/blog/perplexity-ai-lawsuit-secret-data-sharing-google-meta">Perplexity AI Secretly Sent Your Private Chats to Google and Meta — A 135-Page Lawsuit Exposes the Betrayal | GPTAnon Blog</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#conversational AI`, `#security`, `#web applications`, `#research`

---

<a id="item-tech-news-7"></a>
### [OpenAI introduces Dots, an always-on agent product](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

OpenAI has introduced Dots, an always-on agent product. The announcement generated substantial discussion on Hacker News about how Dots differs from existing OpenAI offerings such as Codex and ChatGPT Work and about the lock-in risks of always-on agents. The available item includes no pricing, availability, or technical specifications.

hackernews · alvis · Sep 29, 17:07 · [Discussion](https://news.ycombinator.com/item?id=49896604)

**「Background」** OpenAI introduced Dots at its DevDay event on September 29, 2026, describing the product as &quot;remarkably capable, always-on agents built to handle everything&quot; that can proactively use a computer and connected apps to research, draft documents, write software, and handle other tasks on a user&\#x27;s behalf. Dots is powered by the GPT-6 Astra model and is positioned directly against Meta&\#x27;s widely used Muse agent.

**「Community discussion」** Commenters disagreed on Dots&\#x27; value: wxw found the boundaries between Codex, ChatGPT Work, and Dots blurry and preferred Meta&\#x27;s Muse as a consumer product, while jameslk argued always-on agents are aimed at non-technical users rather than those comfortable with local tools. aditya\_rs warned that agents create platform lock-in because integrations and work history make switching harder than swapping models.

<details><summary>References</summary>
<ul>
<li><a href="https://slashdot.org/story/26/09/29/1723239/openai-unveils-always-on-ai-agent-dots">OpenAI Unveils Always-On AI Agent &#x27;Dots&#x27; - Slashdot</a></li>
<li><a href="https://www.macrumors.com/2026/09/29/openai-launches-dots/">OpenAI Launches Always-On &#x27;Dots&#x27; Agents to Rival Meta&#x27;s Muse - MacRumors</a></li>
<li><a href="https://techcrunch.com/2026/09/29/openai-launches-dots-its-bubbly-agentic-avatar/">OpenAI launches Dots, its bubbly agentic avatar | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#OpenAI`, `#product announcement`, `#always-on agents`, `#technology industry`

---

<a id="item-tech-news-8"></a>
### [PostgreSQL developer talks Linux kernel support at Kernel Recipes](https://lwn.net/Articles/1096827/) ⭐️ 7.0/10

LWN reports that Andres Freund, a longtime PostgreSQL performance contributor, spoke at the 2026 Kernel Recipes conference about how PostgreSQL works with—or around—Linux kernel features and how the kernel could better support database applications. The article summarizes his experience working with kernel developers and alludes to “interesting developments” in PostgreSQL, but the supplied source does not list specific proposals, versions, or measured outcomes.

rss · LWN.net · Sep 29, 15:42

**「Background」** Andres Freund has spent many years improving PostgreSQL performance, which often requires working with or around Linux kernel features and behaviors. His talk at Kernel Recipes 2026 discussed those interactions, how the kernel could better support applications like PostgreSQL, and recent developments in the PostgreSQL world.

**Tags**: `#linux kernel`, `#postgresql`, `#database performance`, `#systems engineering`, `#conference coverage`

---

<a id="item-tech-news-9"></a>
### [Language Models for Text Classification: From Bag-of-Words to Jev](https://magazine.sebastianraschka.com/p/classifier-history-and-jev) ⭐️ 7.0/10

Sebastian Raschka published a visual guide covering text classification architectures from bag-of-words to modern language models, including RNNs, CNNs, Transformers, and calibration techniques. The guide provides hands-on experiments comparing accuracy and efficiency across methods, targeting ML engineers and practitioners who need to understand trade-offs between classic and modern approaches.

rss · Ahead of AI · Sep 29, 10:50

**「Background」** Prior to transformer-based language models, text classification tasks were commonly addressed using bag-of-words representations, recurrent neural networks \(RNNs\), or convolutional neural networks \(CNNs\). Understanding these earlier approaches provides context for the efficiency and accuracy comparisons presented in the guide.

**「Impact」** ML engineers can use the guide&\#x27;s structured comparisons and calibration insights to select appropriate text classification architectures based on documented accuracy and computational efficiency.

**Tags**: `#text-classification`, `#transformers`, `#recurrent-neural-networks`, `#model-calibration`, `#machine-learning`

---

<a id="item-tech-news-10"></a>
### [China&\#x27;s generative AI users exceed 700 million](https://ysxw.cctv.cn/article.html?toc_style_id=feeds_default&amp;amp;item_id=187569887152346976&amp;amp;channelId=1119) ⭐️ 7.0/10

On September 29, the China Internet Network Information Center released its 2026 Generative AI Application Development Report, showing that China&\#x27;s generative AI user base exceeded 700 million people in the first half of 2026, a penetration rate above 50.0%. Intelligent Q&amp;A was the leading use case, with 76.0% of users relying on it for answers, while AI-companion assistants and AI-powered office tools each saw year-over-year usage growth exceeding 100%. The report also measured China&\#x27;s smart computing power at 2185 EFLOPS, up 177% year over year.

telegram · zaihuapd · Sep 29, 06:39

**「Background」** The China Internet Network Information Center \(CNNIC\) is the agency that publishes official statistics on Chinese internet and technology adoption. Its September 29 report is the basis for the user-size and penetration figures cited in this item.

**「Impact」** For AI product teams and infrastructure providers, the figures establish a concrete market baseline: with more than half of China&\#x27;s population using generative AI and Q&amp;A as the dominant interaction, consumer-facing products should prioritize reliable conversational Q&amp;A experiences, and the 177% increase in smart computing capacity signals surging demand for domestic compute and AI infrastructure.

**Tags**: `#generative AI`, `#China`, `#user adoption`, `#AI infrastructure`, `#industry data`

---

<a id="item-tech-news-11"></a>
### [Cloudflare launches cf CLI open beta for AI agents and developers](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare announced cf, an open-beta CLI aimed at developers and AI agents, providing command-line access to more than 3,000 Cloudflare API operations. The tool is generated from Cloudflare&\#x27;s API schema and expands coverage from about 280 operations in the existing Wrangler CLI. It uses JSON as default output and includes command search and guided discovery so agents can find, execute, and process results automatically.

telegram · zaihuapd · Sep 29, 13:46

**「Background」** Cloudflare&\#x27;s existing Wrangler CLI supports roughly 280 operations, primarily centered on Workers development and deployment. The new cf CLI is generated directly from the API schema, which is why it can cover the much larger set of over 3,000 API operations.

**「Impact」** This means automation and AI agents can now use a single CLI to cover a wide range of Cloudflare tasks, from deploying Workers and monitoring services to configuring Access and WAF policies, while consuming JSON output for automated processing. Developers evaluating the beta should test whether the broader API coverage meets their current automation needs before relying on it in production workflows.

**Tags**: `#Cloudflare`, `#CLI`, `#AI agents`, `#developer tools`, `#API`

---

<a id="item-tech-news-12"></a>
### [Google fixes Firebase Analytics server bug behind iOS startup crashes](https://github.com/firebase/firebase-ios-sdk/issues/16728) ⭐️ 7.0/10

Google has fixed a server-side issue in Google Analytics for Firebase that returned malformed data and caused iOS apps using the SDK to crash on startup. The problem affected apps for about two hours on September 28, 2026, from 17:41 to 19:52 PDT. Google says no SDK or app update is needed; because of caching, some apps could continue crashing for up to four hours after the fix before recovering on their own.

telegram · zaihuapd · Sep 29, 16:29

**「Background」** Google Analytics for Firebase is a service that iOS apps integrate as a bundled SDK, and its client-side runtime receives data from Google&\#x27;s backend during normal operation. Because that data arrives at app startup from the server rather than being fixed in the app binary, a malformed server response could crash many installed apps at once, and the correction had to be applied on Google&\#x27;s side while apps gradually recovered as their locally cached data expired.

**「Impact」** iOS developers affected by these startup crashes do not need to ship a new build; the remaining failures should clear automatically as cached bad responses expire. Teams should verify that crashes stop after the cache window rather than treating continued outages as a separate Firebase SDK issue.

**Tags**: `#Firebase`, `#iOS`, `#crash`, `#Google`, `#bug-fix`

---

<a id="item-tech-news-13"></a>
### [How Delhi Cut Electricity Distribution Losses From 50% to 5%](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 6.0/10

IEEE Spectrum&\#x27;s case study reports that Delhi&\#x27;s electricity distribution losses fell from roughly 50 percent to 5 percent after utility reform, theft prevention, and network modernization. The piece describes the improvement as a systems and policy achievement for Delhi rather than a new technology release.

hackernews · rbanffy · Sep 29, 12:43 · [Discussion](https://news.ycombinator.com/item?id=49892245)

**「Background」** In electricity distribution, &quot;losses&quot; are the share of power fed into the grid that never reaches bill-paying customers, combining technical losses from wires and transformers with commercial losses such as theft and billing gaps. High distribution losses have long strained Indian utilities, making reforms to metering, theft enforcement, and grid modernization central to any claim of dramatic improvement. Against that backdrop, Delhi&\#x27;s reported drop from roughly 50% to 5% loss reflects changes in utility operation and enforcement, not a single technical fix.

**「Community Discussion」** A commenter who lived in Delhi 20 years ago argues that ending load shedding, not merely cutting losses, was the revolutionary change, recalling frequent outages and surges that damaged appliances when power returned. Another commenter reports in person that insulating lines to prevent theft made the wires safe for monkeys, an unintended side effect; these are anecdotal recollections, not formal evaluations of the reform.

**Tags**: `#electricity-grid`, `#infrastructure`, `#energy-policy`, `#india`, `#smart-meters`

---

<a id="item-tech-news-14"></a>
### [Relapse-Exploit: PS5 WebKit JavaScriptCore Jailbreak Exploit Published](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 6.0/10

An exploit named Relapse-Exploit targeting a bug in the WebKit JavaScriptCore engine on the PS5 has been published on GitHub by user ntfargo, drawing attention from console-security and jailbreaking communities. The public release gives security researchers and console modders a concrete starting point for investigating PS5 firmware protections, though the item does not confirm that it achieves a full jailbreak or persistent firmware escape. Its scope is limited to the specific WebKit attack surface and does not indicate a broad security breakthrough.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「Background」** WebKit is the browser engine used on the PS5&\#x27;s built-in browser, and JavaScriptCore is its JavaScript engine. Console jailbreaks often start with a JavaScriptCore bug because visiting a malicious page can give an attacker code execution inside the browser process, but full jailbreak status usually requires chaining that first stage to separate kernel or bootloader exploits.

**「Impact」** According to the published repository and follow-up reports, the Relapse exploit reportedly affects PlayStation 5 and PS5 Pro consoles on firmware 7.00 through 13.60, combining a WebKit memory leak with a kernel race condition to run unsigned code. Owners who want to keep their consoles unmodified should avoid WebKit/browser-triggered content until a patched firmware is confirmed, while users intentionally seeking a jailbreak should remain on an affected firmware instead of updating.

**「Community Discussion」** MaxBarraclough asks whether the PS5&\#x27;s WebKit build runs JavaScriptCore with JIT enabled and speculates that Sony might respond by disabling JIT to narrow the attack surface, while aussieguy1234 argues it is &quot;insane&quot; that users need to hack hardware they legally own to gain full control. Muromec adds that such communities typically hold undisclosed exploits and leads for bootloader breakouts, but other commenters only joked about timing and asked for Steam support rather than engaging technically.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aroged.com/2026/09/29/playstation-5-and-ps5-pro-release-fast-jailbreak-recurrence-vulnerability/">PlayStation 5 and PS5 Pro release fast jailbreak recurrence vulnerability - Aroged</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>

</ul>
</details>

**Tags**: `#PS5`, `#security`, `#exploit`, `#WebKit`, `#jailbreak`

---

<a id="item-tech-news-15"></a>
### [Rust-GPU maintainer proposes native Rust compilation to GPU](https://lwn.net/Articles/1095731/) ⭐️ 6.0/10

Christian Legnitto, maintainer of rust-gpu and Rust CUDA, presented a vision at RustConf 2026 for making the GPU a native compiler target for ordinary Rust code, eliminating the need for special libraries or new ecosystem support. He is preparing a prototype to demonstrate this approach, though no implementation is publicly available yet.

rss · LWN.net · Sep 29, 17:57

**「Background」** Until now, programming GPUs from Rust has relied on dedicated projects such as rust-gpu and Rust CUDA, which are libraries that connect Rust code to GPU hardware. Legnitto&\#x27;s RustConf 2026 talk argues that this should not require special libraries or separate ecosystem support, proposing instead that the GPU become a standard compiler target for ordinary Rust code. The prototype he described is still unreleased, so this remains a proposal rather than a working compiler feature.

**「Impact」** Rust developers who currently rely on rust-gpu or Rust CUDA libraries to write GPU code may soon have an alternative: a prototype compiler that treats the GPU as a native Rust target, eliminating the need for special libraries. The prototype is expected to be released, offering a preview of a more integrated GPU programming experience.

**Tags**: `#Rust`, `#GPU computing`, `#compilers`, `#Rust-GPU`, `#RustConf`

---

<a id="item-tech-news-16"></a>
### [Linux distributions release weekly security updates](https://lwn.net/Articles/1097466/) ⭐️ 6.0/10

On September 29, 2026, AlmaLinux, Debian, Fedora, Mageia, Slackware, SUSE, and Ubuntu published security updates for a broad set of packages. The updates include kernel releases from AlmaLinux, Debian, SUSE, and Ubuntu, along with Fedora updates for Chromium and VLC and Debian updates for Dovecot, Flatpak, rsync, and WordPress. Administrators should use the LWN listing to check the complete set of affected packages and distributions.

rss · LWN.net · Sep 29, 15:38

**「Background」** Linux distributions track vulnerabilities in the software they ship and release patched versions through official repositories. This item is LWN&\#x27;s routine weekly roundup of those security notices across multiple distributions, rather than a notice for one specific incident.

**「Impact」** Users and system administrators running any of the listed distributions should install the updated packages from official repositories to receive the fixes. The practical effect of each update depends on the affected package and distribution.

**Tags**: `#security`, `#linux`, `#patch management`, `#system administration`, `#vulnerabilities`

---

<a id="item-tech-news-17"></a>
### [Free open-source book explains how to actually make ML models fast](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 6.0/10

The author released How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents as a free, open-source book on GitHub. It moves from roofline analysis and hardware fundamentals through kernels, compilers, quantization, pruning, vision, on-device LLMs, robotics, profiling, serving, and agent systems. The stated goal is to help engineers diagnose whether a system is compute-, bandwidth-, memory-, or system-bound and decide which optimization will actually move the limit. This is a self-published announcement without independent review or demonstrated performance results.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Background」** Machine learning performance work has long focused on reducing FLOPs, but lower arithmetic count does not automatically translate to lower latency or higher throughput. Practical efficiency depends on where the workload is actually bottlenecked, such as memory bandwidth, kernel implementation, or system-level serving overhead.

**Tags**: `#machine-learning`, `#performance-engineering`, `#open-source`, `#systems`, `#efficient-ml`

---

<a id="item-tech-news-18"></a>
### [CoWindow and MassAlloc Attention: Sparse Collective Coverage, Adaptive Tiles](https://www.reddit.com/r/MachineLearning/comments/1wt1gbk/cowindow_and_massalloc_attention_collective/) ⭐️ 6.0/10

The authors of two new arXiv papers describe attention mechanisms that cut redundant long-context computation: CoWindow Attention \(CoWA\) distributes distant context across KV heads via fixed complementary windows, while MassAlloc Attention \(MALA\) retains full causal QK scoring but skips low-contribution post-score tile work using softmax statistics. Both support training forward/backward and inference prefill/decoding. On 128K tokens with 8 H100 GPUs and TP=8, the authors report attention-operator speedups versus FullAttn of 7.4x forward, 8.6x backward, and 3.0x decode for CoWA, and 2.2x, 3.0x, and 1.6x for MALA. They also report 28.5% and 23.1% total training FLOP reductions at 14B with 32K context, but note these are operator-level results, not end-to-end speedups or proof of universal lossless equivalence to dense attention.

reddit · r/MachineLearning · /u/BitExternal4608 · Sep 29, 05:16

**「Background」** Standard causal attention lets each token attend to all previous tokens, so long-context models repeat similar key-value work across heads and spend compute on low-contribution interactions. CoWA and MALA target that redundancy from different angles: CoWA uses a fixed, position-defined pattern so heads are sparse collectively while covering the full causal history, and MALA uses attention&\#x27;s own softmax statistics to skip computation after full QK scoring when a tile contributes little.

**「Impact」** Teams training or serving long-context models should benchmark these methods in their own stacks before adopting them, because the reported gains are attention-operator measurements rather than end-to-end speedups, and the authors state that neither approach demonstrates universal lossless equivalence to dense attention.

**Tags**: `#attention mechanisms`, `#long-context models`, `#inference efficiency`, `#machine learning research`

---

<a id="item-tech-news-19"></a>
### [Codex Pro $200 subscription reopens with halved quota](https://x.com/thsottiaux/status/2104823812042940713) ⭐️ 6.0/10

Codex Pro&\#x27;s $200 monthly subscription will reopen to new users tomorrow, according to a post by Tibo. The usage calculation is switching to API-spend equivalence, resulting in roughly half the previous quota. The 5-hour usage limit is removed, allowing users to consume the weekly quota at their own pace. Tibo also reported that GPT-6 Sol and GPT-6 Luna API prices have been cut by 50% this week, and future improvements to model efficiency and API pricing are expected to increase the work achievable per dollar.

telegram · zaihuapd · Sep 29, 06:50

**「Background」** According to an unconfirmed announcement attributed to Tibo, Codex Pro&\#x27;s $200/month tier had been closed to new subscribers and previously imposed a five-hour usage window that will not be restored. The announcement follows this week&\#x27;s cuts of GPT-6 Sol and GPT-6 Luna API prices to half their original levels, which it cites as context for aligning subscription value with API costs.

**「Impact」** Subscribers to the reopened $200 Codex Pro plan will get roughly half the usage allowance of the previous plan when measured by API spend, effectively doubling the cost per unit of Codex work for users who relied on the old quota. The elimination of the 5-hour cap lets subscribers spread their weekly allowance at their own pace, and OpenAI says further GPT-6 price cuts are meant to narrow the gap between subscription and pay-per-use API pricing. Heavy users evaluating the plan should compare the halved quota against pay-per-use rates.

<details><summary>References</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/19231/openai-pro-200-dollars-back-half-api-spend-codex">OpenAI announces Pro $200 is back, with half the API spend for Codex</a></li>
<li><a href="https://the-decoder.com/openai-reopens-its-200-pro-plan-but-cuts-api-credits-in-half-as-it-nudges-users-toward-pay-per-use/">OpenAI reopens its $200 Pro plan but cuts API credits in half as it nudges users toward pay-per-use</a></li>
<li><a href="https://www.kucoin.com/news/flash/openai-codex-reopens-200-dollar-pro-subscription-with-api-cost-halved">OpenAI Codex Reopens $200 Pro Subscription with API Costs Halved | KuCoin</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI coding`, `#pricing`, `#GPT-6`

---

## Financial News

<a id="item-finance-news-1"></a>
### [FHFA Mortgage Pricing Change Sinks Fair Isaac; AMD Buys World Labs](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 8.0/10

Fair Isaac shares plunged 18% after Federal Housing Finance Agency director Bill Pulte said Fannie Mae and Freddie Mac will move to one mortgage pricing grid that adds VantageScore to the existing FICO Classic grid, while AMD rose more than 1% after acquiring AI firm World Labs for $8.2 billion.

rss · CNBC Finance · Sep 29, 12:03

**「Background」** Fair Isaac makes FICO credit scores, which mortgage lenders use to set borrower pricing. Fannie Mae and Freddie Mac are government-sponsored mortgage companies, and combining their previously separate pricing grids means VantageScore will now be part of the same mortgage pricing structure as FICO Classic.

**Tags**: `#FHFA mortgage pricing`, `#M&amp;A`, `#earnings`, `#stock movers`, `#healthcare investment`

---

<a id="item-finance-news-2"></a>
### [Oracle Invokes Force Majeure on Stargate Data Center Due to Power Delays](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 8.0/10

Oracle has issued a force majeure notice—a legal clause that excuses delays caused by events outside a company’s control—for a Stargate data center project in New Mexico because environmental and power approvals for a 2.45-gigawatt microgrid have not been granted, risking a delay beyond the planned 2028 start of operations. The notice has raised market concern, causing an $18 billion syndicated loan tied to the project to trade at a discount.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** The Stargate project is a large-scale artificial-intelligence infrastructure venture; most of its sites are still in early construction, permitting, or energy-planning stages, with only a few campuses \(such as the one in Abilene, Texas\) already operating.

**「Impact」** The delay and loan discount signal growing investor wariness about the pace of AI data-center buildout, and Texas has already suspended approval of new data-center projects, which could further constrain expansion in a key hub.

**Tags**: `#Oracle`, `#data center`, `#force majeure`, `#infrastructure delay`, `#AI investment`

---

<a id="item-finance-news-3"></a>
### [China to Subsidize First-Home Mortgage Interest From Oct 1](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 8.0/10

China’s finance ministry, central bank and financial regulator announced a nationwide policy, effective October 1, 2026, that gives eligible new first-home mortgage borrowers a central-government subsidy equal to 1 percentage point of annual interest for up to five years on up to 1 million yuan of principal, or roughly 10,000 yuan per household per year.

telegram · zaihuapd · Sep 29, 10:18

**「Background」** To qualify, the loan must be newly issued for a first home—not a refinancing of an existing loan—and the home must be no larger than 120 square meters and priced at or below 1.5 million yuan.

**「Impact」** The subsidy lowers borrowing costs for first-time buyers of smaller, lower-priced homes, making monthly repayments cheaper for households that meet the criteria.

**Tags**: `#住房贷款贴息`, `#财政政策`, `#房地产`, `#中国人民银行`, `#金融监管总局`

---

<a id="item-finance-news-4"></a>
### [Trump’s municipal bond portfolio reaches estimated $300 million to $1 billion](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

President Trump’s municipal bond holdings have grown to more than 1,000 positions worth between $300 million and $1 billion, according to a CNBC analysis of his financial disclosures, raising ethics questions because many issuers are affected by his administration’s policies. The figures are ranges from disclosure filings and do not reflect subsequent market moves.

rss · CNBC Finance · Sep 29, 14:37

**「Background」** Trump ended 2025 with 807 municipal bond positions worth $240.7 million to $797.6 million and has disclosed at least 243 purchases in 2026, including bonds tied to hospitals, utilities, and coal plants. The White House says the holdings are in independently managed discretionary accounts, and CNBC found no evidence that Trump or his investment managers traded on advance knowledge or shaped policies to benefit his holdings.

**Tags**: `#municipal bonds`, `#Donald Trump`, `#conflict of interest`, `#financial disclosures`, `#public finance`

---

<a id="item-finance-news-5"></a>
### [China reportedly tightens IPO criteria for humanoid-robot startups](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator is reportedly requiring humanoid-robot startups to show sustainable revenue and commercial orders, narrowing losses \(including a three-year forecast\), and core technology such as robotic brains or hands before listing, according to three anonymous sources; there is no official confirmation. At least two dozen such companies have filed to list in Hong Kong, but the sources said the new bar could leave only a handful—or none—able to go public.

rss · CNBC Finance · Sep 29, 07:19

**「Background」** The reported tightening comes after heavy investment in China&\#x27;s &\#x27;embodied AI&\#x27; push—the official term for humanoid robotics—and signs of cooling among listed players, including a steep drop in Unitree&\#x27;s shares since its August IPO. Hong Kong began allowing confidential tech IPO filings in May 2025, but mainland companies still need the regulator&\#x27;s approval to list there.

**Tags**: `#China`, `#humanoid robots`, `#IPO regulation`, `#artificial intelligence`, `#CSRC`

---