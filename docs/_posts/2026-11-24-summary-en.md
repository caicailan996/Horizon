---
layout: default
title: "Horizon Summary: 2026-11-24 (EN)"
date: 2026-11-24
lang: en
---

> From 42 items, 17 important content pieces were selected

---

**Technology News**
1. [Paper Claims VP ≠ VNP over Every Field](#item-tech-news-1) ⭐️ 9.0/10
2. [Ladybird browser engine enters alpha](#item-tech-news-2) ⭐️ 8.0/10
3. [Zhipu Releases GLM-5.4, Its First Loop Transformer for Coding](#item-tech-news-3) ⭐️ 8.0/10
4. [Codex2api suspected supply-chain attack backdoors releases, leaks secrets](#item-tech-news-4) ⭐️ 8.0/10
5. [Nvidia Board Reinstates Jensen Huang as CEO](#item-tech-news-5) ⭐️ 7.0/10
6. [Windows Server 2028 drops WoW64 by default; 32-bit apps need on-demand install](#item-tech-news-6) ⭐️ 7.0/10
7. [Unofficial Arm documentation site to shut down after Arm takedown request](#item-tech-news-7) ⭐️ 6.0/10
8. [Kagi Opens Public Beta of Kagi Mail](#item-tech-news-8) ⭐️ 6.0/10
9. [Nospeaker uses a MacBook trackpad&\#x27;s haptic motor to speak text](#item-tech-news-9) ⭐️ 6.0/10
10. [Developer says Apple removed open-source FSNotes from EU App Stores after 9 years](#item-tech-news-10) ⭐️ 6.0/10
11. [Google Reportedly Tests Chrome AI Agent in Simulated Web](#item-tech-news-11) ⭐️ 6.0/10
12. [Meta AI chief Alexandr Wang says superintelligence is near, warns control at risk](#item-tech-news-12) ⭐️ 6.0/10

**AI Open Source Projects**
1. [LMCache Nightly RBLN NPU Wheel](#item-ai-projects-1) ⭐️ 6.0/10
2. [LMCache Nightly: CUDA 13.0 Wheels for linux/amd64 and linux/arm64](#item-ai-projects-2) ⭐️ 5.0/10

**Financial News**
1. [Ant Group leads $100 million round in Simplexity Robotics at $1.6 billion valuation](#item-finance-news-1) ⭐️ 7.0/10
2. [AI selloff clouds DeepSeek, Moonshot and StepFun listing plans](#item-finance-news-2) ⭐️ 7.0/10
3. [Shanghai Metro to Adjust Fares for First Time in 21 Years](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Paper Claims VP ≠ VNP over Every Field](https://github.com/anthropics/formal-math/tree/main/vp-vnp) ⭐️ 9.0/10

A paper posted in Anthropic&\#x27;s formal-math repository claims VP ≠ VNP over every field, a separation in algebraic complexity that would be a major result if correct. The supplied material links only to the PDF and records active Hacker News discussion; it includes no peer review, independent proof check, or confirmation of the claim. Readers should treat the separation as an asserted paper claim, not an established theorem.

hackernews · mikeryan52 · Nov 23, 22:09 · [Discussion](https://news.ycombinator.com/item?id=50620102)

**「Background」** VP versus VNP is the algebraic counterpart of P versus NP: VP collects problems computable by polynomial-size arithmetic circuits, VNP captures quantities such as the permanent, and Valiant&\#x27;s conjecture that the two classes differ has been open since 1979. The result is presented inside Anthropic&\#x27;s formal-math repository, which secondary reports describe as pairing the paper with a Lean 4 formalization while stating that no human mathematician has checked the proof and that Anthropic does not maintain the artifact. Horizon&\#x27;s November 21 digest had reported a separate Claude-assisted Riemann hypothesis claim from an Anthropic mathematician, likewise published as a Lean proof rather than a peer-reviewed result, so both remain vendor claims that rest on formalization and have not been independently verified.

**「Scope of the claimed separation」** Because VP and VNP are defined relative to a field, a proof of VP ≠ VNP &quot;over every field&quot; would, if verified, settle Valiant&\#x27;s algebraic analogue of P vs NP across characteristics rather than for one fixed setting \[tool-3-1\]\[tool-3-3\]. The paper, as quoted in the discussion, states that it has not analyzed relativization or algebrization, so the result should not be cited as having cleared those standard barriers until the Lean formalization is independently checked.

**「Community discussion」** Commenters framed the paper as part of a broader effort toward P vs NP, with one describing it as a partial result published along the way. Another commenter pointed to the paper&\#x27;s own statement that it has not analyzed how the result relates to relativization or algebrization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/">2026-11-21 — Anthropic mathematician claims Claude-assisted Riemann hypothesis proof in Lean</a></li>
<li><a href="https://news.lavx.hu/article/anthropic-publishes-claimed-proof-that-vp-vnp-over-every-field">Anthropic Publishes Claimed Proof That VP ≠ VNP Over Every Field</a></li>
<li><a href="https://agihunt.info/en/e/1a20a795a118dbdb4f5bd2bb40d">Claude-authored paper claims VP≠VNP over every… · AGI Hunt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arithmetic_circuit_complexity">Arithmetic circuit complexity - Wikipedia</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-662-03338-8_21">P Versus NP: A Nonuniform Algebraic Analogue - Springer</a></li>

</ul>
</details>

**Tags**: `#VP vs VNP`, `#algebraic complexity`, `#complexity theory`, `#formal math`, `#Lean`

---

<a id="item-tech-news-2"></a>
### [Ladybird browser engine enters alpha](https://ladybird.org/posts/alpha/) ⭐️ 8.0/10

The Ladybird project has released an alpha version of its browser, the first public milestone for an engine written from scratch rather than derived from Chromium, Gecko or WebKit. No build details, supported platforms or feature list were included in the supplied material, so the alpha&\#x27;s exact scope is unconfirmed beyond the project&\#x27;s own announcement. Early testers report that a wide range of sites render correctly, including YouTube, Google Maps and the Proxmox web console, while noting jerky scrolling and noticeable lag on heavier pages.

hackernews · janvdberg · Nov 23, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50614249)

**「Background」** Ladybird is a browser engine built from scratch rather than derived from Chromium or Firefox, backed by a 501\(c\)\(3\) non-profit; its project site lists the alpha as available for macOS and Linux and free and open source. Commenters also noted that the engine has moved away from some of its own supporting libraries toward established components such as SQLite and Skia, which they credit with improving it substantially.

**「Impact」** Because this is alpha-stage software, testers should treat it as an evaluation build rather than a daily driver: one commenter suggested limiting use to general browsing that does not involve logins, authentication, payments or downloads, citing security caveats the project itself is upfront about. For developers, the release provides an early third engine to check rendering against outside the Chromium-dominated field, though performance on complex sites is still reported as uneven.

**「Community Discussion」** Commenters were largely impressed by how much of the real web worked on a new engine, with several saying they had not yet found a site that failed to render, though scrolling smoothness and lag on sites like YouTube and Google Maps were recurring complaints. One commenter credited part of the progress to Ladybird replacing several self-developed libraries with established ones such as SQLite and Skia, while expressing nostalgia for the project&\#x27;s original SerenityOS-era approach.

<details><summary>References</summary>
<ul>
<li><a href="https://ladybird.org/">Ladybird is a truly independent web browser , backed by a non-profit.</a></li>

</ul>
</details>

**Tags**: `#Ladybird`, `#browser engine`, `#alpha release`, `#open source`, `#web rendering`

---

<a id="item-tech-news-3"></a>
### [Zhipu Releases GLM-5.4, Its First Loop Transformer for Coding](https://z.ai/blog/glm-5.4) ⭐️ 8.0/10

Zhipu released GLM-5.4, billed as its first loop transformer and aimed at generalized coding, according to the company&\#x27;s blog post. In a looped design, the same weights are reused across repeated iterations instead of each layer being computed once per token, an approach commenters tied to reducing inference memory-bandwidth cost. Access is narrower than usual: commenter Simon Willison reported that GLM-5.4 was not available through OpenRouter or the regular Z.ai API plan and required Zhipu&\#x27;s Coding Plan, whose API keys work like the standard ones but include the new model. The supplied material contained no technical report, so architecture and benchmark claims could not be verified.

hackernews · foohis · Nov 23, 10:06 · [Discussion](https://news.ycombinator.com/item?id=50609685)

**「Looped transformer context」** GLM-5.4 is Z.ai&\#x27;s first model built on a loop transformer, an architecture in which a shared block of layers runs for multiple iterations rather than adding more distinct parameters, according to Z.ai&\#x27;s documentation. Earlier, Horizon&\#x27;s October 13 digest covered a Looped Diffusion Transformer that ran a shared set of blocks repeatedly within each denoising step; its authors reported that naive looping did not reliably help and required deep supervision on every loop plus self-modulating attention.

**「Impact」** Developers who normally reach Zhipu models through OpenRouter or the standard Z.ai API plan have no route to GLM-5.4 there and must obtain a Coding Plan key instead, according to the commenter&\#x27;s report, so teams should confirm plan entitlements before building the model into a workflow.

**「Community discussion」** Commenters praised Zhipu for disclosing architectural detail that they said Western labs keep private, while others reported practical friction: one said Chinese models&\#x27; long &quot;marathon thinking&quot; makes even conceptually simple tasks slow, and another noted GLM-5.4 required switching to the Coding Plan. A separate commenter explained looped transformers as a way to cut memory-bandwidth cost by reusing weights rather than streaming each layer through the chip for a single computation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/">2026-10-13 — Looped Diffusion Transformer trades compute for refinement at sampling time</a></li>
<li><a href="https://anyrouter.dev/model/z-ai/glm-5.4">GLM - 5 . 4 · Zhipu AI · pricing &amp; API · AnyRouter</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.4">GLM - 5 . 4 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Tags**: `#LLM architecture`, `#looped transformers`, `#coding models`, `#GLM-5.4`, `#model release`

---

<a id="item-tech-news-4"></a>
### [Codex2api suspected supply-chain attack backdoors releases, leaks secrets](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

According to a Telegram incident report, the Codex2api author account was compromised and an attacker bypassed the main branch by pushing a tag, causing releases v3.1.10–v3.1.12 to be built with a backdoor; the report describes the compromise as suspected rather than independently confirmed. In v3.1.11 the authentication check was removed, enabling unauthenticated remote command execution, and a workflow exfiltrated 16 GitHub Actions secrets from the repository, affecting at least 21 repositories under the same account. Users who installed or updated to 3.1.10–3.1.12 are advised to stop using the tool, roll back to 3.1.9, and rotate the GitHub token, SSH keys, database credentials, and DeepSeek and other related secrets.

telegram · zaihuapd · Nov 23, 11:21

**「Background」** GitHub release workflows can be triggered by a tag without the tagged commit passing through the protected main branch, and Actions secrets available to that workflow are exposed to whatever build it runs. In that model, tag-publishing rights and workflow secret scope are part of the release supply chain alongside repository write access.

**「Required remediation」** Operators who installed or updated Codex2api 3.1.10–3.1.12 should treat those deployments as compromised: the source report says to stop using them, roll back to 3.1.9, and rotate GitHub tokens, SSH keys, database credentials, and DeepSeek and other related secrets. Because v3.1.11 removed authentication and the workflow exfiltrated 16 GitHub Actions secrets from an account spanning at least 21 repositories, credential rotation should extend beyond the Codex2api host itself.

**Tags**: `#supply-chain-attack`, `#security`, `#GitHub-Actions`, `#backdoor`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [Nvidia Board Reinstates Jensen Huang as CEO](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 7.0/10

Nvidia&\#x27;s board reinstated Jensen Huang as president, CEO, and board director, according to the company&\#x27;s announcement. The board said it received input from senior levels of the U.S. government and concluded that Huang&\#x27;s reinstatement poses no national security risk. The item links to Nvidia&\#x27;s release and a CNBC report but does not include the full statement or details of what government input the board received.

hackernews · jaz · Nov 23, 14:00 · [Discussion](https://news.ycombinator.com/item?id=50611576)

**「Background」** Horizon&\#x27;s Nov. 16 digest, citing the Financial Times, reported that Huang was considering a return as CEO after resigning on Nov. 12, when CFO Colette Kress became interim CEO; it said Huang had discussed a possible return before the board&\#x27;s independent investigation concluded. Horizon&\#x27;s Nov. 9 digest had reported that the board was investigating an intelligence operation targeting Huang, not Huang personally.

**「Market and policy fallout」** Nvidia shares jumped 31% on the reinstatement, according to CNBC&\#x27;s report, a sign that investors are pricing in an end to the leadership uncertainty created by Huang&\#x27;s removal. The episode also feeds directly into pending policy: supporters of bipartisan export-control legislation framed Huang&\#x27;s return as added urgency for passing those restrictions into law, so Nvidia faces renewed scrutiny of its lobbying against curbs on advanced chip sales even as the board says the reinstatement poses no national security risk.

**「Community Discussion」** Commenters seized on the board&\#x27;s statement that it had received input from senior U.S. government officials, with one calling it the “most operative part” of the announcement. Others debated whether Delaware&\#x27;s Caremark precedent would shield directors from liability, expressed surprise at a unanimous reversal, and criticized the move as inconsistent with U.S. pressure on ASML and Japanese chip companies to join China sanctions.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/dotey/status/2122062085807030716">2026-11-16 — Report: Jensen Huang Considering Return as NVIDIA CEO</a></li>
<li><a href="https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors">2026-11-09 — Nvidia Board Probes Intelligence Operation Targeting CEO Jensen Huang</a></li>
<li><a href="https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html">Jensen Huang reinstated as Nvidia CEO. Stock skyrockets 31%</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/live/nvidia-live-updates-jensen-huang-reinstated-as-ceo-trump-says-no-reason-to-believe-huang-a-national-security-risk-152429808.html">Nvidia live updates: Jensen Huang reinstated as CEO; Trump says...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#semiconductors`, `#corporate governance`, `#US government`, `#tech industry`

---

<a id="item-tech-news-6"></a>
### [Windows Server 2028 drops WoW64 by default; 32-bit apps need on-demand install](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 7.0/10

Microsoft said at Ignite 2026 that Windows Server 2028 will ship without the WoW64 compatibility subsystem, so 32-bit applications will not run out of the box. The release is planned for fall 2027 alongside Windows 11 27H2. Administrators who still need 32-bit support can add WoW64 as a Features on Demand package, typically via PowerShell or DISM on Server Core. Microsoft describes the change as reducing attack surface and blocking 32-bit malware; Windows 11 keeps WoW64 for now, with no removal plan announced.

telegram · zaihuapd · Nov 23, 03:03

**「WoW64 and Windows backward compatibility」** WoW64 is the compatibility subsystem that lets 32-bit x86 applications run on 64-bit Windows, and it is what Windows Server 2028 will leave out of the default installation. Horizon&\#x27;s October 27 digest illustrated how far that Win32 backward-compatibility path reaches, covering a blog post that launched a decades-old GUI application on Windows 11 without modification. Under the new plan, the same capability becomes an optional on-demand feature that administrators must add back with PowerShell or DISM on Server Core.

**「Impact」** Server administrators planning the move will need to inventory 32-bit application and agent dependencies before deployment and install the WoW64 feature on demand where those apps remain necessary — a step that cannot be assumed during an in-place upgrade or a fresh Server Core install. Because Windows 11 still includes WoW64, client-side compatibility is unaffected for the time being.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.enlyth.com/posts/oldest-windows-gui-app-win-11/">2026-10-27 — Oldest GUI App That Still Runs on Windows 11</a></li>

</ul>
</details>

**Tags**: `#Windows Server`, `#WoW64`, `#32-bit compatibility`, `#Microsoft`, `#enterprise IT`

---

<a id="item-tech-news-7"></a>
### [Unofficial Arm documentation site to shut down after Arm takedown request](https://arm.jonpalmisc.com/) ⭐️ 6.0/10

The unofficial Arm documentation site arm.jonpalmisc.com says it will be discontinued on 4 December 2026 after Arm requested its removal, according to the site owner. The owner said Arm cited use of its trademarks and IP in hosting the documentation, and that keeping the site useful while complying is difficult. The owner is considering mirror hosting, legal advice, and releasing site source code without Arm IP.

hackernews · tech234a · Nov 23, 19:17 · [Discussion](https://news.ycombinator.com/item?id=50617499)

**「What the site was」** The affected site was an unofficial, reformatted copy of Arm&\#x27;s architecture reference documentation; commenters compared its pages with similarly converted Arm64 manuals hosted elsewhere and asked whether the same extraction tool produced both. Arm separately publishes a machine-readable architecture specification \(MRAS\), which commenter ethin said is distributed under a BSD-style license, though that covers the ISA reference rather than the fuller documentation the site mirrored.

**「Impact」** Developers who relied on the unofficial mirror for Arm architecture documentation will lose that access unless a compliant mirror or source release appears; the owner has not announced a replacement.

**「Community Discussion」** Commenters criticized the takedown as harmful to developers and debated whether documenting publicly sold hardware is fair use. One commenter said several Arm machine-readable specification releases are BSD-licensed, while another asked whether the site was generated with a conversion tool.

**Tags**: `#Arm`, `#documentation takedown`, `#intellectual property`, `#hardware documentation`, `#open access`

---

<a id="item-tech-news-8"></a>
### [Kagi Opens Public Beta of Kagi Mail](https://blog.kagi.com/kagi-mail-public-beta) ⭐️ 6.0/10

Kagi has opened a public beta of Kagi Mail. The supplied item does not include technical details such as pricing, storage limits, migration tools, encryption or data-handling terms, or eligibility, so the beta&\#x27;s practical scope is not established. This is a vendor announcement of a beta, not an independently measured result.

hackernews · rdmuser · Nov 23, 17:17 · [Discussion](https://news.ycombinator.com/item?id=50615481)

**「Background」** Kagi Mail extends Kagi beyond its paid privacy-focused search engine and Orion browser into email and calendar, offering @kagimail.com addresses or custom domains in public beta. Kagi describes it as a premium email service designed to integrate with the rest of its ecosystem, positioning the inbox as another part of users&\#x27; digital lives it wants to cover.

**「What testers are signing up for」** Anyone weighing Kagi Mail as a primary inbox faces a $99-a-year beta without end-to-end encryption, and Kagi has not named the AI providers that process mail, according to Privacy Affairs&\#x27; review — so users drawn by the AI features would be exposing message contents to an unnamed cloud model. On the privacy side, Kagi&\#x27;s documentation says tracking pixels are stripped and images proxied through Kagi&\#x27;s image proxy across all email clients used to access the account, not only Kagi&\#x27;s own app.

**「Community Discussion」** Commenters were divided: some Kagi customers said AI is Kagi Mail&\#x27;s main selling point but they would not give a cloud LLM access to their email, while another worried that adding mail would worsen feature creep and the quality of core services such as Kagi Translate. Others questioned the shift for a company perceived as storing little user data, and one said email is too central to online identity to trust to a niche provider.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.kagi.com/kagi-mail-public-beta">Kagi Blog - Kagi Mail is here (Public Beta)</a></li>
<li><a href="https://help.kagi.com/kagi/mail/">Kagi Mail FAQ | Kagi&#x27;s Docs</a></li>
<li><a href="https://www.privacyaffairs.com/kagi-mail-public-beta/">Kagi Mail Public Beta: $99 a Year, No End-to-End Encryption</a></li>
<li><a href="https://help.kagi.com/kagi/mail/">Kagi Mail FAQ | Kagi&#x27;s Docs</a></li>

</ul>
</details>

**Tags**: `#Kagi Mail`, `#email`, `#privacy`, `#AI integration`, `#product launch`

---

<a id="item-tech-news-9"></a>
### [Nospeaker uses a MacBook trackpad&\#x27;s haptic motor to speak text](https://github.com/os6/nospeaker) ⭐️ 6.0/10

Developer Cody Collier has open-sourced Nospeaker, a macOS tool that drives a Force Touch trackpad&\#x27;s haptic motor at up to 4,000 Hz so the glass vibrates audibly and speaks text. It uses macOS speech synthesis, sampling two formants every 10 milliseconds along with loudness and pitch, which produces robotic-sounding speech. The tool bypasses Apple&\#x27;s public haptics API and calls the private MultitouchSupport framework; it requires a Force Touch trackpad, and the author reports testing it only on an M5 Max MacBook Pro. It can speak text but cannot play music or video, with output audible from 100 Hz to 4 kHz and clearest near 1 kHz.

hackernews · yakkomajuri · Nov 23, 11:31 · [Discussion](https://news.ycombinator.com/item?id=50610318)

**「Background」** Apple&\#x27;s Force Touch trackpads do not have a hinged button; a haptic actuator under the glass creates the click sensation. Because Apple does not expose that actuator through a public haptic API, third-party projects have instead wrapped the private MultitouchSupport framework to trigger feedback—the same route Nospeaker uses to send audio-rate signals.

**「Impact」** Anyone trying Nospeaker needs a Force Touch trackpad and should expect possible breakage from macOS updates because it relies on a private framework; it is not a general audio output device, since it renders text-to-speech only, not music or video.

**「Community discussion」** Commenters were struck less by the speech than by the trackpad&\#x27;s normal click simulation, with one calling the illusion of pressing a button on an unmoving slab more impressive. Another speculated that Apple&\#x27;s sum-of-sines actuator API may exist to prevent motor burnout, simplify per-partial feed-forward correction, or keep USB/HID bandwidth low, framing these as hypotheses rather than confirmed reasons.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/crnicholson/macos-haptic/">GitHub - crnicholson/macos-haptic: Control the haptic ...</a></li>

</ul>
</details>

**Tags**: `#haptics`, `#hardware-hacking`, `#macOS`, `#trackpad`, `#reverse-engineering`

---

<a id="item-tech-news-10"></a>
### [Developer says Apple removed open-source FSNotes from EU App Stores after 9 years](https://github.com/glushchenko/fsnotes/discussions/2056) ⭐️ 6.0/10

The developer of the open-source app FSNotes says Apple removed it from EU App Stores after nine years. A commenter says it remains available in the US and UK, and a cached Dutch App Store listing cited in the thread indicated the developer had not identified himself as a trader for the app. Apple has not confirmed the reason in the supplied material, but commenters linked the removal to EU Digital Services Act trader-status verification.

hackernews · fluder · Nov 23, 18:48 · [Discussion](https://news.ycombinator.com/item?id=50616933)

**「Background: EU trader-status rule」** Under the EU Digital Services Act, developers distributing apps in the EU must declare &quot;trader&quot; status in App Store Connect, publishing a contact name, address, email, and phone number; Apple has required this declaration to submit app updates in the EU since October 16, 2024, and removes apps without verified trader status from EU storefronts. The requirement is ongoing rather than one-time, and Apple lets developers change the status per app under App Compliance.

**「Impact」** For independent developers distributing through the App Store, the case shows that EU availability can hinge on account-level trader verification rather than app review; commenters describe trader status as something that can lapse and the verification process as slow. Developers with EU listings should verify that their trader status is current rather than assume an existing listing remains compliant.

**「Community discussion」** Commenters split over responsibility: one argued that the app is paid, that the developer had nine years to complete trader verification, and that open-source status is irrelevant; others described EU trader verification as a known bottleneck and criticized reliance on forum attention for support. A separate developer reported about a month&\#x27;s wait for EU DSA approval after an October rule change, though for a new app rather than an existing listing.

<details><summary>References</summary>
<ul>
<li><a href="https://ivryn.com/guides/app-store-dsa-trader-status/">App Store DSA trader status for EU apps : Feb 2025 | IVRYN</a></li>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act trader requirements ...</a></li>
<li><a href="https://orbitkit.io/blog/eu-dsa-trader-status-app-store/">EU DSA trader status : the App Store trader requirements ... | OrbitKit</a></li>

</ul>
</details>

**Tags**: `#EU DSA`, `#Apple App Store`, `#open-source software`, `#app distribution`, `#developer compliance`

---

<a id="item-tech-news-11"></a>
### [Google Reportedly Tests Chrome AI Agent in Simulated Web](https://www.landian.news/archives/128701.html) ⭐️ 6.0/10

Google reportedly built a simulated internet called Mirror Dimension to test Chrome&\#x27;s AI agent in an isolated environment, according to a brief report from Landian News. The simulated environment reportedly contains thousands of mock websites, with each engineer testing separately and more than 1,000 test cases run per day. The tests reportedly cover opening sites, searching and browsing, logging in, adding items to a cart, and completing tasks, with a focus on defenses against prompt-injection attacks from malicious webpages. The report offers limited technical detail and no primary-source confirmation.

telegram · zaihuapd · Nov 23, 01:30

**「Background」** Google&\#x27;s Chrome security team first detailed the Mirror Dimension in a blog post, framing it as a way to test browser agents in realistic online conditions without exposing live sites to risk. Browser-use agents complete tasks by operating a browser—opening pages, searching, logging in, filling carts—so hidden instructions in page content are a direct prompt-injection surface.

**「Impact」** The reported scope includes login and cart actions, so the testing targets agent behavior with account and purchasing consequences, not just reading pages; the prompt-injection focus also treats ordinary webpage content as a potential attack surface.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents : Evaluating Browser-Use Agents ...</a></li>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘ Mirror Dimension ’ Internet to Test Its Chrome ...</a></li>

</ul>
</details>

**Tags**: `#Chrome AI agent`, `#browser automation`, `#prompt injection`, `#AI security`, `#Google`

---

<a id="item-tech-news-12"></a>
### [Meta AI chief Alexandr Wang says superintelligence is near, warns control at risk](https://thenextweb.com/news/metas-ai-chief-says-superintelligence-is-arriving-and-control-is-at-risk) ⭐️ 6.0/10

Meta&\#x27;s chief AI officer and Superintelligence Labs head Alexandr Wang said in a lengthy post on X that superintelligence is no longer a &quot;someday&quot; question, pointing to a Riemann hypothesis proof that mathematician Levent Alpöge produced with Anthropic&\#x27;s Claude and that the Lean and Mathlib community machine-verified on Saturday. Wang argued that only three gaps remain between AI and top human researchers: specific knowledge, engineering integration, and experimentation. He warned that humans will struggle to keep control of systems that can improve themselves indefinitely or be 1,000 times smarter than people, and called for urgent investment in safety, alignment, and safeguards research. The proof has no human-readable version yet, and the account is a short secondary brief, so the claimed result remains unverified beyond the reported Lean check.

telegram · zaihuapd · Nov 23, 12:49

**「Background」** Horizon&\#x27;s Nov. 21 digest reported that mathematician Levent Alpöge had claimed a Claude-assisted proof of the Riemann hypothesis, released as a roughly 15-million-line Lean formalization—a machine-checkable encoding—that the supplied discussion had not technically verified. The current item says Lean and Mathlib community checking has since machine-verified the proof.

**「Impact」** Because no human-readable version of the proof exists, researchers cannot yet inspect the argument itself and can only rely on the reported Lean/Mathlib machine verification, which limits how far the example can be used as evidence of AI research capability.

<details><summary>References</summary>
<ul>
<li><a href="https://alpo.ge/remark.pdf">2026-11-21 — Levent Alpöge claims Generalized Riemann Hypothesis proof with Lean formalization</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#superintelligence`, `#Lean/Mathlib`, `#Meta AI`, `#AI-assisted proof`

---

## AI Open Source Projects

<a id="item-ai-projects-1"></a>
### [LMCache Nightly RBLN NPU Wheel](https://github.com/LMCache/LMCache/releases/tag/nightly-rbln) ⭐️ 6.0/10

LMCache published a nightly wheel for Rebellions RBLN NPUs, built from \`dev\` against torch-rbln 0.12.0. It enables installation on hosts that already provide torch-rbln and rebel-compiler.

github · github-actions\[bot\] · Nov 23, 09:25

**「Problem Solved」** Running LMCache on Rebellions RBLN NPUs requires a platform-specific package. This nightly wheel supplies that packaging while leaving torch-rbln, rebel-compiler, and the RBLN driver host-owned rather than bundled, so users install it into an existing RBLN software environment.

**「Background」** LMCache is a KV cache management layer for LLM inference that stores, reuses, and moves KV cache across GPU, CPU memory, and external backends, targeting long prompts and reused context to reduce time-to-first-token and improve throughput \(tool-1-1, tool-1-3; tool-1-2\). The nightly-rbln release extends that layer to Rebellions RBLN NPUs by publishing a platform-specific wheel built from \`dev\` against torch-rbln 0.12.0 \(torch 2.13.0+cpu\); torch-rbln, rebel-compiler, and the RBLN driver remain host-owned rather than bundled. This fits the broader hardware-specific inference stack around RBLN: its SDK supports models trained with PyTorch, TensorFlow, and Hugging Face, and RBLN artifacts are precompiled for RBLN NPUs and served with vLLM-RBLN \(tool-2-1, tool-2-2\). As a nightly packaging build, it signals portability work rather than a feature or performance announcement.

<details><summary>References</summary>
<ul>
<li><a href="https://lmcache.ai/en/">Building the Foundation of AI Memory Tensor with KV Cache ...</a></li>
<li><a href="https://arxiv.org/abs/2510.09665">[2510.09665] LMCache: An Efficient KV Cache Layer for ...</a></li>
<li><a href="https://docs.lmcache.ai/">Welcome to LMCache! | LMCache</a></li>
<li><a href="https://rebellions.ai/ai-powered-food-recognition-and-nutrition-management/">AI-Powered Food Recognition and Nutrition Management - Rebellions</a></li>
<li><a href="https://huggingface.co/iAcloud/gemma4-31B-it-rbln-tp16">iAcloud/gemma4-31B-it- rbln -tp16 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#NPU`, `#RBLN`, `#nightly build`

---

<a id="item-ai-projects-2"></a>
### [LMCache Nightly: CUDA 13.0 Wheels for linux/amd64 and linux/arm64](https://github.com/LMCache/LMCache/releases/tag/nightly) ⭐️ 5.0/10

LMCache&\#x27;s nightly release publishes pre-release CUDA 13.0 wheels built from the dev branch for linux/amd64 and linux/arm64. It is a packaging update for installing the LLM KV-cache project, not a documented feature or performance release.

github · github-actions\[bot\] · Nov 23, 09:52

**「Problem Solved」** The release provides a prebuilt install path for LMCache with CUDA 13.0, including arm64, using a uv pip command and the PyTorch cu130 index. This reduces the need to assemble nightly packages or build from source. The source provides no benchmark or optimization claims.

**「Background」** LMCache is an open-source KV cache management layer for LLM inference, aimed at making cached context persistent and reusable rather than purely temporary state \(tool-1-1, tool-1-3\). This item is a nightly packaging release, not a feature announcement: it provides CUDA 13.0 wheels built from the \`dev\` branch on 2026-11-23 for linux/amd64 and linux/arm64, installed through a PyTorch cu130 extra index. Its ecosystem relevance is therefore compatibility and distribution: it gives developers a way to test the development branch against CUDA 13.0 and the cu130 PyTorch stack. The source does not describe performance changes, optimizations, or new caching features, so those should not be inferred from this nightly build.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/lmcache-tutorial">LMCache Tutorial: Build a Scalable KV Cache Layer for LLM Inference</a></li>
<li><a href="https://www.gitgenius.co/repos/LMCache/LMCache">LMCache : Supercharge Your LLM with the Fastest KV Cache Layer</a></li>

</ul>
</details>

**Tags**: `#LMCache`, `#KV cache`, `#LLM inference`, `#CUDA`, `#nightly release`, `#wheels`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Ant Group leads $100 million round in Simplexity Robotics at $1.6 billion valuation](https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race) ⭐️ 7.0/10

Ant Group led a $100 million pre-A funding round in Chinese embodied-intelligence startup Simplexity Robotics at a $1.6 billion post-money valuation, with existing investors Alibaba, Tencent, HongShan and BlueRun also participating, chairman and co-founder Wang Kai confirmed to Bloomberg. The Hangzhou-based company, founded in July 2025, said in March it had raised 2 billion yuan across five rounds in its first six months, when its post-money valuation already exceeded $1 billion.

telegram · zaihuapd · Nov 23, 02:02

**「Background」** Simplexity Robotics was founded in Hangzhou in July 2025 by a team from electric-vehicle maker Li Auto, and had already raised five rounds worth a combined 2 billion yuan within its first six months, at a post-money valuation above $1 billion, according to the report. Bloomberg also says Chinese humanoid-robot makers account for about 97% of global shipments, and the new funding is meant to help Simplexity compete with more established players such as Unitree and UBTech.

**「Competitive pressure」** The $100 million gives Simplexity capital to challenge incumbent humanoid-robot makers Unitree and UBTech in a market where Chinese manufacturers accounted for more than 97% of global shipments in the first half of 2026, according to Smart Analytics Global.

<details><summary>References</summary>
<ul>
<li><a href="https://global.chinadaily.com.cn/a/202608/11/WS6a7a8b3aa310986e2b46a1a5.html">Chinese humanoid robot makers hold 97% global shipments in H1</a></li>

</ul>
</details>

**Tags**: `#humanoid robotics`, `#venture financing`, `#Ant Group`, `#China tech`, `#valuation`

---

<a id="item-finance-news-2"></a>
### [AI selloff clouds DeepSeek, Moonshot and StepFun listing plans](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

The global selloff in AI stocks that followed Anthropic&\#x27;s record $119.5 billion IPO has clouded plans or considerations by Chinese AI companies DeepSeek, Moonshot and StepFun to sell shares to the public, Bloomberg reported. Chinese tech stocks have lost $1.7 trillion in market value since end-June.

telegram · zaihuapd · Nov 23, 09:31

**「Background」** DeepSeek and Moonshot had already been preparing 2027 listings, with proceeds expected to support AI-infrastructure expansion, before the selloff that followed Anthropic’s IPO clouded the outlook for new AI share sales.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo">China’s Next AI Deals Clouded by Selloff After Anthropic IPO</a></li>
<li><a href="https://www.chosun.com/english/industry-en/2026/10/08/LPVZSXQ4DNAMTKIBF77XUB3U6Y/">DeepSeek, Moonshot AI Prepare for 2027 IPOs - 조선일보</a></li>

</ul>
</details>

**Tags**: `#AI selloff`, `#China tech stocks`, `#IPOs`, `#Anthropic`, `#market volatility`

---

<a id="item-finance-news-3"></a>
### [Shanghai Metro to Adjust Fares for First Time in 21 Years](https://weibo.com/1699432410/5368461393397183) ⭐️ 7.0/10

Shanghai Metro will adjust fares for the first time in 21 years, setting a 3-yuan starting fare for 0–4 km and 1-yuan increments across set distance bands, effective Dec 1. Four ride-count tickets, priced from 190 yuan for 35 rides to 390 yuan for 90 rides, go on sale Nov 26, and same-payment-channel monthly spending of 90 yuan earns a 10% discount.

telegram · zaihuapd · Nov 23, 10:45

**「Background」** Shanghai’s subway fares had gone 21 years without adjustment, local reports said, making this the first change in that period. The new distance-based prices come with multi-ride tickets and a monthly spending discount intended to limit the effect on frequent commuters.

<details><summary>References</summary>
<ul>
<li><a href="https://hot.online.sh.cn/content/2026-09/09/content_10485162.htm">时隔 21 ...</a></li>

</ul>
</details>

**Tags**: `#上海地铁`, `#公共交通票价`, `#民生政策`, `#计次票优惠`

---