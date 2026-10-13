# Product Opportunity Cards

Companion files: [Research report](report.md) · [Technology list](tech_list.csv) · [Sources](sources.md). Chinese version: [../product_cards.md](../product_cards.md).

Key terms appear with their Chinese equivalent the first time they show up. The full list is in the [bilingual glossary](../glossary.md).

Research date: October 6, 2026. Because you did not specify a direction, the default assumptions here are: **a small team of 3 to 10 people, mainly calling APIs and open source (开源) models, not developing its own hardware, and considering both the Chinese and overseas markets**. Each card notes which market it suits.

## Overview

| Card | Product direction | Main underlying technologies | Target market | Priority |
| :--- | :--- | :--- | :--- | :--- |
| A | AI voice receptionist for vertical industries | Full duplex (全双工) voice, managed agents (托管智能体), MCP | Overseas first, also viable in China | **High** |
| B | AI search visibility monitoring and optimization (generative engine optimization, GEO, 生成式引擎优化) | AI assistants becoming the new entry point, falling prices of midrange models (中档模型) | China first; competition is fiercer overseas | **High** |
| D | MCP connectors and industry agent templates for Chinese SaaS | New MCP specification, open source models, managed agents | China | **High** |
| C | Compliance (合规) labeling and detection SaaS for AI generated content (AIGC) | China's labeling measures, Article 50 of the EU AI Act | China and the EU | Medium high |
| E | Real time translation and dubbing for cross border livestreams and foreign trade communication | Full duplex voice, speech translation, video lip sync | Chinese merchants selling overseas | Medium high |
| F | On device (端侧) AI note taker for privacy sensitive professions | Small on device models, Apple Foundation Models | Overseas first | Medium |
| G | AI glasses assistant for frontline workers | AI glasses developer tools, multimodal (多模态) vision | China and overseas | Medium |
| H | GLP 1 companion and metabolic health management | Oral GLP 1, cheaper generics, over the counter (非处方) continuous glucose monitors (CGM, 连续血糖仪) | Overseas; China after generics launch | Medium |
| I | AI code security audits for small and medium sized businesses | AI vulnerability discovery, coding agents | China and overseas | Medium |
| J | Embodied AI (具身智能) applications and data services | Vision language action (VLA, 视觉语言动作) models, cheaper humanoid robots (人形机器人) | China | Low to medium |

The priority weighs five factors: whether demand has been validated, whether the technology is ready to use, whether a small team can build a minimum viable product (MVP, 最小可行产品) in 4 to 8 weeks, the risk of giants entering directly, and regulatory risk.

---

## A. AI Voice Receptionist for Vertical Industries

**In one sentence**: An AI receptionist that answers the phone 24 hours a day for small businesses that live on phone bookings, such as dental clinics, medical aesthetics clinics, veterinary clinics and auto repair shops. It answers common questions and writes appointments directly into the business's booking system.

**Target users**: Businesses with 5 to 50 staff that take 30 to 200 calls a day and run mainly on appointments. I suggest starting with dental clinics, because overseas data show that small healthcare businesses have the highest rate of AI phone adoption, at 48%.

**Pain points**
* One missed call can mean one lost customer, and after hours nobody answers at all
* Front desk staff are expensive. A small dental practice overseas typically spends more than 3,000 dollars a month to employ one receptionist, while an AI answering solution costs only 50 to 500 dollars a month
* The front desk spends most of its time answering the same questions: opening hours, price ranges, address, whether insurance is accepted

**Why now**
1. Voice models have entered the "full duplex" stage. They can listen while speaking and pick up naturally after being interrupted, and the experience is close to talking with a person. OpenAI opened the GPT Live 1 API on September 10, 2026, at 0.05 dollars per minute; NVIDIA's open source NemotronLabs VoiceChat natively supports tool use (工具调用) and can be deployed privately (私有化部署).
2. Market education is done. The share of small and medium sized businesses (中小企业) in the US and Europe that use AI to answer the phone rose from 11% in 2024 to 34%.
3. Connecting to booking systems has become much easier. Managed agent platforms (Claude Managed Agents, OpenAI Agents API) take care of the runtime environment, MCP takes care of tool integration, and the main work left is writing connectors.

**Technical approach**: Phone line (SIP or cloud communications) → full duplex voice model → a midrange model for intent recognition and tool calls (for example GPT 6.1 Sol, or a Chinese model) → write to the booking system or CRM through MCP connectors → push a call summary to the store manager.

**MVP scope (4 to 6 weeks)**: One industry and one booking system only. Features: answering calls, Q&A, booking, rescheduling, cancellation, transfer to a human, and call summaries.

**Cost estimate (overseas version)**: Assuming an average of 3 minutes per call and 600 calls a month, the voice model costs about 90 dollars; adding the large model (大模型) and phone charges, the total is about 150 dollars. At a price of 299 dollars a month, the gross margin (毛利率) is about 50%. A China version would need to switch to Chinese voice models, and costs would have to be recalculated.

**Competitors**: Overseas, there are Retell (0.07 to 0.31 dollars per minute), Synthflow, Goodcall (from 59 dollars a month), Nextiva XBert (from 99 dollars a month) and CloudTalk. In China, the big companies' smart customer service products mainly focus on outbound calling for large enterprises, and the niche of inbound calls for local stores is still fragmented (Chinese competitors not systematically verified).

**Risks**
* China regulates outbound marketing calls strictly, so handle only "inbound call reception," never outbound marketing
* Callers must be told the call is being recorded
* Medical Q&A must not give diagnostic advice
* Large models may quote wrong prices, so key information such as prices and insurance should live in a structured knowledge base instead of being left to the model to improvise

**How to validate in the first 2 weeks**: Interview 10 clinics and measure their missed call rate and daily call volume; build a demo on an off the shelf voice agent platform, give 3 clinics a free one week trial, and look at the answer rate and the booking conversion rate (转化率).

---

## B. AI Search Visibility (GEO) Monitoring and Optimization

**In one sentence**: Help brands answer one question: "When users ask Doubao (豆包), DeepSeek or ChatGPT, will the AI recommend me?" Then give suggestions for improving their content.

**Target users**: Marketing departments of consumer brands, local services merchants, B2B software companies and brands expanding overseas, plus the agencies that do marketing for them.

**Pain points**: The traffic entry point is shifting from search engines to AI assistants, but traditional search engine optimization (SEO, 搜索引擎优化) tools cannot see how often a brand appears in AI answers (the industry calls this share of model).

**Why now**
1. Similarweb's 2026 data show that 35% of US consumers use AI when looking for products, while only 13.6% use search engines
2. Users who arrive from ChatGPT convert at 7%, versus 5% for those from Google
3. Ahrefs found that 28.3% of the pages ChatGPT cites most often have no organic ranking on Google at all, which shows that GEO and SEO follow two different logics
4. Chinese AI assistants have huge user bases: according to QuestMobile, in June 2026 Doubao had 382 million monthly active users (月活), Qwen (千问) 167 million and DeepSeek 130 million. But there are few monitoring tools built specifically for Chinese AI assistants (not systematically verified)

**Technical approach**: Build a question bank (generated automatically by category, plus custom questions from the client) → sample answers every day across several AI assistants → use a midrange model to extract brand mentions, sentiment and cited sources → generate dashboards and competitor comparisons → give content suggestions (which Q&A is missing, which structured data is missing, which third party sources are worth investing in).

**MVP scope (4 weeks)**: Support 5 AI assistants. For China: Doubao, DeepSeek, Qwen, Yuanbao (元宝) and Kimi; for overseas: ChatGPT, Gemini, Perplexity, Claude and Copilot. 100 questions per brand, with one report a week.

**Cost estimate**: 100 questions times 5 assistants comes to about 500 queries a day. At current midrange model prices, the API cost is a few dollars a day. The main difficulty is not cost but getting the real answers that consumer apps give.

**Competitors**: Overseas, there are already Profound, Similarweb AI Search, Writer and others. China is still at an early stage.

**Risks**
* Answers in consumer apps may differ from what the API returns, and automated collection may violate platform terms of service
* AI answers are highly random, so you need repeated sampling and statistics rather than a single result
* Platforms may later launch official advertising or data products that squeeze the space for third party tools

**How to validate in the first 2 weeks**: Pick 3 categories (for example skincare, coffee machines and SaaS bookkeeping software), run 50 questions by hand, turn them into a report, and show it to 5 brands or agencies to ask whether they would pay for it.

---

## C. AIGC Compliance Labeling and Detection SaaS

**In one sentence**: An API for companies that publish AI generated content. It automatically adds explicit labels and implicit metadata labels, checks whether upstream materials carry labels, and keeps an audit trail.

**Target users**: Advertising agencies, ecommerce merchants and their service providers, MCN agencies, small and medium content apps, and apps expanding into the EU.

**Pain points**
* China's Measures for Labeling AI Generated Synthetic Content (《人工智能生成合成内容标识办法》) took effect on September 1, 2025, and entered a phase of strict enforcement in 2026. AI generated content needs both visible labels (text, corner badges, voice prompts) and implicit labels written into the file metadata; AI advertising materials must also carry a metadata watermark containing the brand's unified social credit code (统一社会信用代码)
* The Article 50 transparency obligations (透明度义务) of the EU AI Act took effect on August 2, 2026, and the watermarking requirements for systems already deployed have a grace period until December 2
* Companies use several AI tools at once to produce images and videos, with no unified compliance process

**Why now**: The rules have just taken effect and enforcement has just begun. After the Cyberspace Administration of China (网信办) pressed platforms to fix the problem in February 2026, researchers found that large numbers of AI videos on Xiaohongshu (小红书) were still unlabeled. The EU grace period ends in December.

**Technical approach**: Delivered as an SDK or API. On the labeling side, it supports explicit labels for images, video, audio and text, plus three kinds of implicit labels: metadata, C2PA manifests (内容凭证) and invisible watermarks. On the detection side, it reads metadata and detects watermarks, and adds a model that estimates the probability that content is AI generated. Every operation is recorded in an audit log.

**MVP scope (6 weeks)**: Start with explicit labels plus metadata labels for images and video, with batch processing and exportable audit reports. Detection starts with reading metadata and C2PA only.

**Competitors**: Labels built into the platforms (Douyin (抖音) and Xiaohongshu add them automatically when content is generated); content safety vendors (such as NetEase Yidun (网易易盾) and Shumei (数美)) may extend into this; overseas there are Digimarc, Truepic and open source C2PA tools.

**Risks**
* The detailed standards may still change
* Once large platforms build the feature in, the space for standalone tools will shrink
* The accuracy of detecting AI generated content is limited, so do not overpromise to customers

---

## D. MCP Connectors and Industry Agent Templates for Chinese SaaS

**In one sentence**: Build high quality MCP connectors for SaaS products widely used in China, such as DingTalk (钉钉), WeCom (企业微信), Yonyou (用友), Kingdee (金蝶) and Youzan (有赞), then package them into industry agent templates such as "order to reconciliation," "sales follow up" and "customer service tickets," with support for private deployment on open source models.

**Target users**: IT leads at small and medium sized manufacturing, trading and retail companies, and the implementation partners that serve them.

**Pain points**: Companies want to automate their processes with agents, but the AI interfaces of mainstream Chinese SaaS products are scattered, and the data is not allowed to leave the company's internal network.

**Why now**
1. The new MCP specification released on July 28, 2026 was designed specifically for multi tenant cloud deployments: stateless, cacheable and with stronger authentication
2. There are already more than 10,000 public MCP connectors worldwide, but most connect to overseas SaaS. Feishu (飞书) already has an official MCP, but it currently covers only cloud documents; as of our search, we had not seen standalone official MCP connectors for DingTalk or WeCom; the status of Yonyou and Kingdee is unverified
3. Open source models are now good enough. The DeepSeek V4 series uses the MIT license, which allows commercial use and private deployment and meets the requirement that data never leaves the organization
4. Managed agent platforms charge by running time (for example, Claude Managed Agents charges 0.08 dollars per running hour), so building a prototype overseas is very cheap

**MVP scope (6 weeks)**: Pick one scenario, such as "order to reconciliation" for small and medium sized manufacturers. Build 3 connectors and 1 agent template, plus a private deployment package (based on DeepSeek V4 Flash or the GLM series).

**Business model (商业模式)**: Open source the connectors to attract users; charge for an enterprise edition that adds permission management, auditing and private deployment; and charge fees for implementation services.

**Competitors**: Official MCPs released by the SaaS vendors themselves; plugin marketplaces on platforms such as Dify and Coze; traditional system integrators.

**Risks**: SaaS vendors stepping in officially; low willingness to pay among small and medium sized businesses in China; the business can easily slide into project based work, with delivery getting heavier and heavier.

---

## E. Real Time Translation and Dubbing for Cross Border Livestreams and Foreign Trade Communication

**In one sentence**: Let Chinese livestream hosts and foreign trade salespeople stream or hold meetings in their native language, while viewers and clients hear natural foreign language dubbing in real time (实时) that keeps the speaker's original voice.

**Target users**: Merchants on TikTok Shop and other overseas livestream ecommerce platforms, B2B foreign trade sales teams, and companies exhibiting at trade shows.

**Why now**
1. Full duplex voice models have brought latency down to conversational levels
2. Google Meet's voice dubbing feature became generally available in February 2026, which proves the experience is feasible. But it only translates between English and 5 European languages, and only works inside Meet
3. Kling (可灵) 3.0 supports lip sync in 5 languages, which can be used to localize prerecorded short videos
4. Shokz (韶音) OpenFit 2 AI uses Tongyi (通义) speech models, which shows that Chinese speech models have already shipped in overseas consumer products

**MVP path**: Start with multilingual dubbing (with lip sync) for prerecorded short videos, which brings in cash quickly; then move on to real time subtitles and dubbing for livestreams.

**Competitors**: HeyGen (video translation), iFlytek (讯飞), Google Meet, and translation hardware such as Timekettle (时空壶).

**Risks**
* Latency and accuracy directly determine the livestream experience
* Voice cloning requires the speaker's own authorization and must comply with the rules on deep synthesis (深度合成) and labeling
* Livestream platforms may restrict third party streaming tools

---

## F. On Device AI Note Taker for Privacy Sensitive Professions

**In one sentence**: A tool for meeting and session notes for lawyers, therapists, physicians in independent practice and financial advisors. Recordings never go to the cloud; transcription, summarization and structured notes all happen locally on the phone or computer.

**Why now**
1. On device models are good enough: Gemma 4 has two on device versions, E2B and E4B, and flagship phone NPUs reach 45 to 60 TOPS
2. At WWDC 2026, Apple opened its Foundation Models framework. Small developers with fewer than 2 million downloads can use Private Cloud Compute inference (推理) for free, and can also plug in third party models
3. The value of AI documentation has been proven in healthcare: 29% of US doctors use it, and it saves them 16 minutes a day of paperwork on average. But Epic has launched native AI documentation tools for hospitals, and athenahealth offers athenaAmbient free to its outpatient practice customers, so avoid hospitals and the practices these systems cover, and go after professions outside healthcare such as law and counseling, plus independent practitioners who do not use these systems

**MVP scope (6 weeks)**: An iOS app with local transcription plus summaries from a local model, built in templates for each profession (legal client intake, counseling session notes, due diligence on financial clients), and export.

**Business model**: Inference has almost no marginal cost, which makes a subscription (订阅) a good fit.

**Competitors**: Otter, Feishu Minutes (飞书妙记) and Tongyi Tingwu (通义听悟), all of which process in the cloud; Apple's built in recording transcription and summary features.

**Risks**: Apple's system features expanding to cover this need; the quality of on device models on long recordings; industry compliance requirements (such as HIPAA in the US).

---

## G. AI Glasses Assistant for Frontline Workers

**In one sentence**: Using the developer tools for glasses from Rokid, Meta and others, build a work guidance and automatic recording tool based on "first person photos plus voice" for inspection, warehouse and equipment maintenance staff.

**Why now**
1. Global AI glasses shipments grew 263% in the first half of 2026, and IDC expects 13.6 million units of models without displays to ship for the full year
2. The developer ecosystem has opened up: Meta's glasses developer toolkit can use the 12 megapixel camera and the five microphone array, is currently in preview, and is planned to open fully in 2026; Rokid launched AIUI Studio in September, which can generate apps from natural language, along with an agent store, and has more than 15,000 registered developers in China
3. Multimodal models are already very good at reading images: they can read gauges and spot anomalies

**MVP scope (6 to 8 weeks)**: An inspection checklist process for one industry. Voice prompts guide each step, the worker takes a photo, a vision model checks gauge readings and anomalies, and an inspection report is generated automatically at the end.

**Competitors**: Traditional AR remote assistance vendors, such as RealWear and HiAR (亮风台).

**Risks**: Publishing apps built with Meta's toolkit still requires partner approval; battery life of the glasses; factory network conditions and data security; the customer decides which hardware to buy. In addition, B2B (To B) payment cycles are relatively long.

---

## H. GLP 1 Companion and Metabolic Health Management

**In one sentence**: A companion app for people taking GLP 1 drugs (减重药) to lose weight (by injection or orally): medication reminders, guidance on protein intake and muscle preservation, side effect management, and a connection to a continuous glucose monitor (CGM) to see how each meal affects blood sugar.

**Why now**
1. Eli Lilly's oral GLP 1 (orforglipron, brand name Foundayo) was approved by the FDA on April 1, 2026, and can be taken without restrictions on food or water
2. Semaglutide's core patent in China expired on March 20, 2026, prices fell by more than 50%, and domestic generics are under review, so the number of people taking these drugs will grow significantly
3. Over the counter CGMs are becoming more common: Dexcom Stelo has expanded to children, and Abbott launched the world's first device that monitors both glucose and ketones

**MVP scope (6 weeks)**: An app with an AI dietitian (recognizes meals from photos and estimates protein), a medication calendar, a side effect diary, and optional CGM data import (through Apple Health or Health Connect).

**Competitors**: Noom and WeightWatchers both have GLP 1 programs; overseas there are also telehealth prescribing platforms such as Ro and Hims; in China there are internet hospitals, Boohee (薄荷健康) and others.

**Risks**: The app must not give diagnosis or treatment advice and should be positioned as health management; anything involving prescriptions requires licenses; health data needs privacy protection.

---

## I. AI Code Security Audits for Small and Medium Sized Businesses

**In one sentence**: An AI agent for small and medium sized software companies that have no security team. It audits code repositories continuously and submits fixes directly when it finds problems.

**Why now**
1. Anthropic's Claude Mythos Preview and Google's Gemini 4 Argon have both shown that AI's ability to find vulnerabilities now exceeds that of most human experts, although both models are currently open only to a few partners
2. Publicly available models are already strong as well. Claude Opus 5.5 can audit 200,000 lines of code in under 3 hours, a job that used to take more than 20 hours
3. Attackers are using AI too, so demand for defense is rising; in China there is also compliance demand from the Multi Level Protection Scheme (等保)

**MVP scope (6 weeks)**: A GitHub or GitLab app that scans every commit, runs a full repository audit once a week, generates fixes automatically, and collects feedback on false positives.

**Competitors**: Snyk, GitHub Advanced Security, Semgrep and others; competition is intense (which AI features they offer was not systematically verified).

**Risks**: Too many false positives will make users lose trust; customer code must stay confidential, so private deployment needs to be supported; this capability can itself be used for attacks, so usage controls are needed.

---

## J. Embodied AI Applications and Data Services

**In one sentence**: Do not build the robot itself. Instead, on complete robots from Unitree (宇树) and AgiBot (智元), use Gemini Robotics 2 or open source VLA models to develop "skill apps" for showroom tours, supermarkets and malls, and education and research; or help robot makers collect teleoperation (遥操作) data.

**Why now**
1. Global humanoid robot shipments in the first half of 2026 were about 4 times the level of the same period last year, with Chinese makers accounting for more than 97%; the entry level Unitree R1 costs about 5,900 dollars
2. Gemini Robotics 2 opened to developers through the Gemini API on July 30, 2026
3. pi 0.7 demonstrated compositional generalization, which suggests that data diversity matters more than data volume, and this will create demand for data collection services

**MVP direction**: An "embodied AI training kit" for universities and vocational schools, including a complete robot, courses and data collection tools.

**Risks**: Heavy pressure from hardware reliability and after sales service; VLA success rates in open environments are still unstable; home use has not been validated (1X NEO still had no verified user deliveries as of mid July). This track has a long cycle and needs a lot of capital, so it is not suitable as a first product.
