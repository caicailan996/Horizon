---
layout: default
title: "Horizon Summary: 2026-09-25 (ZH)"
date: 2026-09-25
lang: zh
---

> 从 39 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [英国双层加密：苹果撤回高级数据保护](#item-tech-news-1) ⭐️ 8.0/10
2. [F-Droid 2.0 发布：十年最大更新](#item-tech-news-2) ⭐️ 7.0/10
3. [OpenAI 称苹果 ChatGPT 集成不佳致合作破裂](#item-tech-news-3) ⭐️ 7.0/10
4. [OpenAI 发布心理健康基准 MentalHealthBench](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [北京商品房预售新政：封顶方可预售](#item-finance-news-1) ⭐️ 8.0/10
2. [费城联储主席暗示需要进一步小幅加息以抑制通胀](#item-finance-news-2) ⭐️ 7.0/10
3. [中方确认首次对美 AI 对话，贸易休战延长至明年 1 月](#item-finance-news-3) ⭐️ 7.0/10
4. [DeepSeek 年化营收破 10 亿美元，拟融资约 75 亿美元并筹备上交所上市](#item-finance-news-4) ⭐️ 7.0/10
5. [三大运营商暂停金融分期购机，0 元购机停办](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [英国双层加密：苹果撤回高级数据保护](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

苹果已于英国撤回高级数据保护（ADP），以回应政府发出的监视令。此前，ADP 将端到端加密的 iCloud 类别从 14 个扩展至 23 个；撤销后，英国用户新增的 9 个类别（包括 iCloud 备份、照片、备忘录和 iCloud Drive）降级为标准数据保护，苹果持有解密密钥并可依法应诉。这造成了事实上的双层加密系统：默认类别维持端到端加密，而扩展类别仅由苹果持有的密钥保护。

hackernews · ReturnoftheHack · 9月24日 10:39 · [社区讨论](https://news.ycombinator.com/item?id=49828731)

**「背景」** 苹果的“高级数据保护”（Advanced Data Protection, ADP）是一项可选功能，可将原本未加密的 iCloud 类别（如备份、照片、备忘录等，共 9 类）升级为端到端加密，使受保护的 iCloud 类别从默认的 14 类增加到 23 类。2025 年，英国政府依据《2016 年调查权力法》向苹果发出“技术能力通知”，要求提供后门访问权限，迫使苹果在英国停止提供 ADP，导致英国用户的部分 iCloud 数据降级为标准保护，由苹果保留解密密钥。

**「影响」** 英国 iCloud 用户的隐私保护实质性降低：一旦启用 ADP 后撤回，此前由 ADP 加密的备份、照片等数据现在可由苹果在合法程序下解密，而用户无法自行关闭这一访问通道。

**「社区讨论」** 多位评论者指出，苹果的妥协打破了此前“公开对抗政府”的形象——有用户直言因 Tim Cook 曾对 FBI 说“不”而选择 Mac，如今感到被背叛。另有人质疑，即使默认 14 个类别仍加密，但额外类别的密钥暴露已破坏整体用户信任，且苹果可能已在设置中强制要求年龄验证等类似让步，说明“一旦让政府进门，就再也关不上”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://contentbuffer.com/news/apple-withdraws-uk-advanced-data-protection-icloud-b0c2cd2b">Apple Withdraws UK Advanced Data Protection for iCloud</a></li>

</ul>
</details>

**标签**: `#encryption`, `#privacy`, `#Apple`, `#UK technology policy`, `#cloud security`

---

<a id="item-tech-news-2"></a>
### [F-Droid 2.0 发布：十年最大更新](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 7.0/10

F-Droid 于 2026 年 9 月 24 日发布 2.0 版，这是官方 Android 应用十年来最大的一次更新：重做界面与底层代码，将结构简化为“发现、搜索、我的应用”三大区域，并改进应用发现、分类、搜索与筛选，支持搜索应用描述、分类及翻译内容，同时加强对中日韩文字的支持。新版还引入更顺畅的安装更新流程和后台检查更新，将在未来数周逐步推送，此前已进行 14 次测试发布。首批版本暂不支持 F-Droid Privileged Extension，并放弃对 Android 6 的支持。

hackernews · daveoc64 · 9月24日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=49831968)

**「背景」** F-Droid 是 Android 平台历史悠久的自由/开源软件应用商店，官方客户端长期保持较为朴素的管理界面，并曾依赖 Privileged Extension 实现静默安装等系统级功能。此次 2.0 版本是官方应用十年来最大规模的重写，同时也在发布说明中确认 Privileged Extension 暂不支持，并将最低支持版本提升至 Android 7。

**「影响」** 对仍在使用 Android 6 或依赖 F-Droid Privileged Extension 的用户来说，F-Droid 2.0 意味着官方支持路径将发生变化：Android 6 被放弃，Privileged Extension 暂不支持。相关用户应保留旧版客户端，或改用 droid-ify 等替代客户端，并为特权扩展的迁移或替换提前规划。

**「社区讨论」** 评论对新设计反应不一：有人欢迎这次大改，并乐见 F-Droid Privileged Extension 被逐步淘汰；也有人批评新界面沿用不画分隔线的现代设计风格，导致区块、可点按元素和滚动区域缺乏清晰提示。还有用户指出宣传截图里“Syncthing-For k”的文字换行错误，认为这出现在展示改版的素材中不太合适。

**标签**: `#F-Droid`, `#Android`, `#Open Source`, `#App Store`, `#Privacy`

---

<a id="item-tech-news-3"></a>
### [OpenAI 称苹果 ChatGPT 集成不佳致合作破裂](https://www.ft.com/content/256c4b36-a6c8-49ee-aa15-81cb089b2ced) ⭐️ 7.0/10

OpenAI 在 2026 年 9 月 23 日提交的法庭文件中称，苹果对 ChatGPT 的集成“表现严重不佳”，对用户缺乏兴趣感到失望。2024 年双方达成协议由 ChatGPT 为 Apple 智能提供支持，但集成默认关闭且需多步骤激活，被指导致采用率低。随后关系恶化，苹果对 OpenAI 提起商业秘密诉讼，并于 2026 年 1 月与谷歌合作使用 Gemini 重建 Siri AI。该文件出自 xAI 提起的反垄断诉讼。

telegram · zaihuapd · 9月24日 05:15

**「背景」** 2024 年，苹果与 OpenAI 达成协议，将 ChatGPT 集成到 Siri 和 Apple Intelligence 中，但该集成默认关闭，用户需经过多步骤选择加入才能使用，导致采用率低迷。随后双方关系恶化，苹果于 2025 年对 OpenAI 提起商业秘密诉讼，并于 2026 年 1 月与谷歌达成每年 10 亿美元的 Gemini 合作，以重建 Siri AI。

**「影响」** 苹果已转向谷歌 Gemini 重建 Siri AI，OpenAI 失去关键平台集成机会，双方合作彻底破裂并进入法律纠纷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/09/23/openai-siri-chatgpt-underperforming/">ChatGPT in Siri &#x27;Persistently Underperforming,&#x27; Says OpenAI</a></li>
<li><a href="https://9to5mac.com/2026/09/23/openai-says-apple-intelligence-users-showed-little-interest-in-chatgpt-integration/">OpenAI says Apple Intelligence users showed little interest... - 9to5Mac</a></li>
<li><a href="https://www.how2shout.com/news/apple-google-gemini-siri-partnership-2026.html">Apple Picks Google Gemini AI at $1B/Year to Power New Siri</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Apple`, `#ChatGPT`, `#AI integration`, `#legal dispute`

---

<a id="item-tech-news-4"></a>
### [OpenAI 发布心理健康基准 MentalHealthBench](https://openai.com/zh-Hans-CN/index/introducing-mentalhealthbench/) ⭐️ 7.0/10

OpenAI 发布开放基准 MentalHealthBench，用于评估 AI 在真实心理健康对话中的表现。该基准由 22 个国家/地区的 80 多名持证心理健康专家共同制定，衡量安全、收集背景信息、维护用户自主权和提供可行建议等行为，覆盖成人、青少年、照护者和临床人员等场景。评估显示 AI 在处理心理健康问题上取得稳步进展，但 OpenAI 强调 ChatGPT 不能替代专业治疗。

telegram · zaihuapd · 9月24日 06:00

**「背景」** MentalHealthBench 是一个包含 1215 个合成心理健康对话的数据集，模拟了真实 ChatGPT 使用场景，由 80 多名持证专家参与制定，用于系统评估 AI 在心理健康对话中的关键行为表现。在此之前，业界缺乏一个经过专业临床验证、可全面衡量 AI 在心理支持场景下安全性与有效性的开放基准。

**「影响」** 对于从事 AI 心理健康应用的开发者和研究机构，MentalHealthBench 提供了可重复的标准化评估框架，有助于推动更安全、更尊重用户自主权的对话系统开发。使用该基准时需注意其结论仅限于模型表现评估，不改变现有临床诊疗流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cdn.openai.com/ctf-cdn/MentalHealthBench_A_Comprehensive_Benchmark_of_AI_Capabilities_in_Realistic_Mental_Health_Conversations.pdf">MentalHealthBench: An Expert-Informed Benchmark of AI</a></li>

</ul>
</details>

**标签**: `#mental-health`, `#benchmarks`, `#AI-evaluation`, `#OpenAI`, `#AI-safety`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [北京商品房预售新政：封顶方可预售](https://mp.weixin.qq.com/s/g-nwBAIGMCfuhENgs6o9-g) ⭐️ 8.0/10

9 月 24 日，北京发布商品房预售新政：8 月 28 日后新出让地块的商品住房项目须主体结构封顶方可申请预售，并优先实行现房销售；预售资金实行全额、全过程监管，新出让住宅用地价款可分期缴纳（首付不低于总价 50%，余款两年内缴清不计利息），项目竣工备案后银行方可发放个人住房按揭贷款。

telegram · zaihuapd · 9月24日 11:10

**「背景」** 此前商品房预售允许房屋未建成时先卖，开发商可提前回款；新政把预售门槛提高到“封顶”，并收紧预售资金监管，意味着购房者付款与房屋交付之间的风险被进一步压缩。

**「影响」** 新政直接作用于 8 月 28 日后在北京新拿地的开发商和购买这些项目的购房者：开发商须等封顶才能开始预售回款，购房者须等竣工备案后才能办理按揭贷款。

**标签**: `#房地产政策`, `#预售制度`, `#北京楼市`, `#资金监管`, `#按揭贷款`

---

<a id="item-finance-news-2"></a>
### [费城联储主席暗示需要进一步小幅加息以抑制通胀](https://www.cnbc.com/2026/09/24/philadelphia-feds-anna-paulson-says-modest-rate-moves-likely-ahead-to-tame-inflation.html) ⭐️ 7.0/10

费城联邦储备银行行长安娜·保尔森周四表示，可能需要进一步“适度”加息，因为核心通胀率仍在 2.5%至 3%之间，远高于美联储 2%的目标。她指出，除伊朗战争和关税导致的石油供应冲击外，物价压力依然顽固。

rss · CNBC Finance · 9月24日 17:12

**「背景」** 美联储公开市场委员会一周前刚将基准利率上调 25 个基点至 3.75%至 4%的区间。保尔森称此次加息使政策更接近所需水平，但通胀回落进展甚微，劳动力市场保持稳定。

**「影响」** 市场预期已迅速转向进一步收紧：交易员认为 10 月再次加息概率为 64%，长期国债收益率升至 2004 年以来最高，投资者预计到 2027 年底利率可能达到 4.8%。

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#economic outlook`

---

<a id="item-finance-news-3"></a>
### [中方确认首次对美 AI 对话，贸易休战延长至明年 1 月](https://www.cnbc.com/2026/09/24/china-confirms-first-ai-talks-with-us-have-taken-place-hints-at-trade-truce-extension.html) ⭐️ 7.0/10

中国商务部周四确认，中美已举行首次人工智能（AI）对话；发言人何亚东表示，双方还讨论了降低关税及延长去年 10 月达成的贸易休战。美国财长贝森特称，休战将从此前 11 月的到期日延长至明年 1 月 10 日。

rss · CNBC Finance · 9月24日 14:16

**「背景」** 去年 10 月达成的休战协议使双方维持较低关税，并限制中国的稀土出口管制；此前美方曾提出建立 AI 对话和风险预警机制。相关表态正值中国国家主席习近平访问华盛顿并与美国总统特朗普会谈前夕。

**「影响」** 若延长落实，依赖较低关税和稀土出口的半导体及制造业企业短期内可缓解政策不确定性；但商界仍面临稀土出口许可证申请缺乏标准化流程等问题。

**标签**: `#US-China trade`, `#AI policy`, `#rare earths`, `#tariffs`, `#semiconductors`

---

<a id="item-finance-news-4"></a>
### [DeepSeek 年化营收破 10 亿美元，拟融资约 75 亿美元并筹备上交所上市](https://weibo.com/1642634100/RjAoNli86) ⭐️ 7.0/10

新浪科技援引知情人士称，DeepSeek 年化营收运行率（按当前速度推算一整年的收入）已达 10 亿美元，较数月前不足 5 亿美元明显增长；CEO 梁文锋在投资者会议上表示，上调 API 定价未造成客户流失。公司正推进第二轮融资，计划 10 月底前完成，目标募资 500 亿元人民币（约合 75 亿美元）、估值 5000 亿元，并筹备在上交所上市。

telegram · zaihuapd · 9月24日 07:56

**「背景」** DeepSeek 由量化对冲基金 High-Flyer 联合创始人梁文锋创立，2026 年 6 月完成首轮外部融资约 510 亿元人民币（约 70 亿美元），投后估值约 520 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ventureatlas.org/company/deepseek">DeepSeek - Company Profile, Milestones &amp; Funding - Venture Atlas</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI大模型`, `#融资`, `#估值`, `#上交所`

---

<a id="item-finance-news-5"></a>
### [三大运营商暂停金融分期购机，0 元购机停办](https://finance.sina.com.cn/jjxw/2026-09-24/doc-inisxhnx5270778.shtml) ⭐️ 7.0/10

据新浪科技报道，自 2026 年 9 月 24 日起，中国移动、中国电信、中国联通均已暂停受理金融分期购机新业务，和包信用购、橙分期、沃分期等“0 元购机”产品全面停办；已办理用户的存量分期合约继续有效，恢复时间尚未确定。

telegram · zaihuapd · 9月24日 08:46

**「背景」** 所谓“0 元购机”通常并非免费，而是用户办理分期贷款、按月还款的业务，此前常被包装成“免费领手机”，并成为消费投诉的重灾区。

**「影响」** 对新购机用户而言，短期内无法再通过三大运营商办理此类分期购机，可能转向其他消费金融渠道或选择全款购机。

**标签**: `#电信运营商`, `#消费金融`, `#手机分期`, `#金融监管`

---