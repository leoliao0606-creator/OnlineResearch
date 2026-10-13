# Research Report: AI and Frontier Technology over the Past Six Months

**Period covered**: April to early October 2026
**Completed**: October 6, 2026
**Companion files**: [Product opportunity cards](product_cards.md) · [Technology list and scores](tech_list.csv) · [Sources](sources.md)
**Chinese version**: [../report.md](../report.md)

Key terms appear with their Chinese equivalent the first time they show up. The full list is in the [bilingual glossary](../glossary.md).

---

## 0. First, a Note on Assumptions and Limitations

**Default assumptions** (you did not specify any when you replied "start," so I made my judgments on the following basis)
* No restrictions on product direction
* The team is small, 3 to 10 people, mainly calling APIs and open source (开源) models, and does not develop its own hardware
* Both the Chinese and overseas markets are considered, and each opportunity notes which market it suits

**Limitations**
* In this run, the environment could only see the summaries returned by search engines. Most websites (including arXiv, news sites and vendor sites) could not be opened in full. So many numbers come from secondhand reports. I have tried to list links to primary sources so you can check them
* Coverage of competitors in the Chinese market is incomplete. Where the text says "not systematically verified," I suggest checking further before you make decisions
* The scores are judgments based on public information and cannot replace user interviews and technical validation

---

## 1. Executive Summary

### The Seven Most Important Trends

**1. Model capabilities keep stepping up, and the price of a given level of capability falls by a factor of 5 to 13 each year.**
September was a dense release month: OpenAI's GPT 6 Astra (September 3), Anthropic's Claude Opus 5.5 (September 22) and Google's Gemini 4 Argon (September 30) all made "completing complex tasks autonomously over several hours" a main selling point. The more important story is the midrange models (中档模型): GPT 6.1 Sol costs 2 dollars per million input tokens (词元) and 10 dollars per million output tokens, and its capability is already close to the flagships. A September report from Epoch AI estimates that the cost of reaching a given capability level falls about 47% per quarter, or roughly thirteenfold per year (other studies put the decline at 5 to 10 times per year).
*What it means for products*: Do not bet your competitiveness on "having a stronger model than everyone else." Bet on workflows, proprietary data and distribution channels.

**2. Agents (智能体) are moving from demos to production.**
Claude Managed Agents (April) and the OpenAI Agents API (September) both turned sandboxes, memory, permissions and tracing into managed services. The Model Context Protocol (MCP, 模型上下文协议) released a new specification in July, and there are more than 10,000 public connectors (a late 2025 figure). Computer use (电脑操作) agents reached 72.6% on OSWorld 2.0.
*What it means for products*: A small team can build a production grade agent in a few days. The barriers have moved to industry connectors, delivery capability and trust.

**3. Open source models are now "good enough."**
The DeepSeek V4 series (MIT license), Kimi K3 (2.8 trillion parameters, open weights (开放权重)), GLM 5.2, MiniMax M3 and NVIDIA Nemotron 3 Ultra were all released in the past six months.
*What it means for products*: Private deployment (私有化部署) where data never leaves the organization (especially in China) is now technically feasible.

**4. Voice has entered the "full duplex (全双工)" era.**
GPT Live 1 costs 0.05 dollars per minute and can listen while it speaks; NVIDIA open sourced a full duplex model that supports tool use (工具调用). The share of small and medium sized businesses (中小企业) in the US and Europe that use AI to answer the phone has reached 34%.
*What it means for products*: Voice is one of the most mature and easiest to monetize directions right now.

**5. Traffic entry points are shifting, and AI assistants are becoming the new "search engine plus app store."**
35% of US consumers use AI when looking for products; ChatGPT launched plugin extensions that embed full apps inside a conversation; Doubao (豆包) has 345 million monthly active users (月活); Apple opened its Foundation Models framework to third party models.
*What it means for products*: Generative engine optimization (GEO, 生成式引擎优化), meaning getting AI to recommend you, and "building apps inside assistants" are two new channels.

**6. AI in the physical world is accelerating, but most of it is still early.**
Humanoid robot (人形机器人) shipments in the first half were about 4 times the level of the same period last year, with Chinese makers accounting for more than 97%; Gemini Robotics 2 opened an API; AI glasses shipments grew 263%. But home humanoid robots have no verified deliveries yet, and robotaxis are still a game for giants.
*What it means for products*: Small teams are better suited to building the application layer on top of hardware, not the robots themselves.

**7. Regulation is taking effect, and compliance (合规) itself has become a need.**
China's rules for labeling AI generated content (AIGC, 人工智能生成内容), the Measures for Labeling AI Generated Synthetic Content (《人工智能生成合成内容标识办法》), are being strictly enforced in 2026; the Article 50 transparency obligations (透明度义务) of the EU AI Act took effect on August 2 (high risk obligations were pushed back to December 2027); California's law on companion AI took effect in January.
*What it means for products*: Tools for labeling, detection and age verification are a hard requirement; companion products and products for minors should design for compliance from the start.

### The Product Opportunities Most Worth Pursuing

| Priority | Product direction | Reason in one line |
| :--- | :--- | :--- |
| High | [A. AI voice receptionist for vertical industries](product_cards.md#a-ai-voice-receptionist-for-vertical-industries) | Demand is proven (34% of small and medium sized businesses use one), voice costs 0.05 dollars per minute, and a minimum viable product (MVP, 最小可行产品) takes 6 weeks |
| High | [B. GEO monitoring and optimization](product_cards.md#b-ai-search-visibility-geo-monitoring-and-optimization) | The shift in entry points has just begun, and there are almost no mature tools for Chinese AI assistants |
| High | [D. MCP connectors and agent templates for Chinese SaaS](product_cards.md#d-mcp-connectors-and-industry-agent-templates-for-chinese-saas) | The MCP ecosystem is mostly overseas, and most mainstream Chinese SaaS products still have no official connector |
| Medium high | [C. AIGC compliance labeling and detection](product_cards.md#c-aigc-compliance-labeling-and-detection-saas) | The rules have just taken effect, and the EU grace period ends in December |
| Medium high | [E. Translation and dubbing for cross border livestreams and foreign trade](product_cards.md#e-real-time-translation-and-dubbing-for-cross-border-livestreams-and-foreign-trade-communication) | Full duplex voice and multilingual lip sync are both ready to use |
| Medium | [F. On device (端侧) AI note taker](product_cards.md#f-on-device-ai-note-taker-for-privacy-sensitive-professions) | Inference (推理) has zero marginal cost, and privacy is the selling point |
| Medium | [G. AI glasses assistant for frontline workers](product_cards.md#g-ai-glasses-assistant-for-frontline-workers) | Glasses shipments are booming, and developer tools have just opened |
| Medium | [H. GLP 1 medication companion](product_cards.md#h-glp-1-companion-and-metabolic-health-management) | An oral drug was approved, the Chinese patent expired, and the number of users is growing |
| Medium | [I. AI code security audits](product_cards.md#i-ai-code-security-audits-for-small-and-medium-sized-businesses) | AI's ability to find vulnerabilities is proven, but competition is fierce |
| Low to medium | [J. Embodied AI (具身智能) applications and data services](product_cards.md#j-embodied-ai-applications-and-data-services) | A long term track that needs a lot of capital |

**If you pick only one**: I suggest starting with **A (AI voice receptionist)**. Demand has already been validated by the market, the unit economics (单位经济模型) are clear, the whole tech stack is off the shelf, and integrating with the booking systems of vertical industries is dirty work that big companies do not want to do, which is exactly the opening for a small team. **B (GEO)** is a good second direction to validate in parallel, because it is the cheapest to validate: run one report by hand and you can test willingness to pay.

---

## 2. Detailed Review by Field

Scores for each technology are in [tech_list.csv](tech_list.csv); the scoring method is in Section 3.

### 2.1 Foundation Models (基础模型)

**Key developments**

| Date | Developer | Model | Highlights | Price (per million tokens, input/output) |
| :--- | :--- | :--- | :--- | :--- |
| April 24 | DeepSeek | V4, V4 Pro preview | Open source, MIT license | Open source |
| May 19 | Google | Gemini 3.5 Flash | Stronger than the previous generation flagship, 4 times faster | Not verified |
| May 28 | Anthropic | Claude Opus 4.8 | | Not verified |
| June 1 | MiniMax | M3 | Coding ability close to the frontier, priced at about 5% to 10% of closed models | |
| Mid June | Zhipu (智谱) | GLM 5.2 | Ranked first among open source models on Artificial Analysis | Open source |
| July 9 | OpenAI | GPT 5.6 series | | |
| July 15 | Thinking Machines | Inkling | 975B multimodal base model, Apache 2.0, built for fine tuning | Open source |
| July 26 | Moonshot AI (月之暗面) | Kimi K3 open weights | 2.8 trillion total parameters, 104 billion active, 1 million token context | Open source |
| July 31 | DeepSeek | V4 Flash official release | 284B MoE, MIT license | Open source |
| September 3 | OpenAI | GPT 6 Astra | 1 million token context; OSWorld 2.0 72.6%; DeepSWE 74.1% | $10 / $50 |
| September 22 | Anthropic | Claude Opus 5.5 | Roughly as capable as Fable 5.1, 40% cheaper to run than Opus 5 | $4 / $20 |
| September 22 | Alibaba (阿里) | Qwen 4 announcement | Four tiers, still in training, no release date | |
| September 29 | OpenAI | GPT 6.1 Sol | Coding and computer use close to Astra | $2 / $10 |
| September 30 | Google | Gemini 4 Argon | Output limit of 1 million tokens; DeepSWE 77.9%; opened first to cyber defenders | Not disclosed |

**Signals worth noting**
* **Tighter safety controls**: OpenAI canceled the release of GPT 6.1 Astra because of a safety regression; Anthropic's Mythos and Google's Argon were both opened only to trusted partners first. The strongest capabilities will reach ordinary developers later and later, and with more and more conditions attached
* **Capability tiers are becoming clear**: flagship models handle long, complex tasks, midrange models cover 80% of everyday needs, and small models handle classification and routing (OpenAI launched a dedicated Decisions API)
* **Diffusion language models (扩散语言模型)**: Inception's Mercury 2.5 generates more than 1,100 tokens per second, about 10 times as fast as a typical model, with quality in the Claude Haiku 4.5 class. It suits scenarios that are extremely sensitive to speed, such as real time (实时) completion and the "fast reply layer" in voice conversations

**What it means for products**: Models themselves are becoming more and more like utilities (water, electricity and gas). Product design should use model routing (模型路由), with expensive models used only for the hard steps, and should treat the evaluation (评测) system as a core asset, so you can switch models with confidence.

### 2.2 Agents and Tool Use

**Key developments**
* **Managed agent platforms**: Claude Managed Agents entered public beta on April 9, offering sandboxes, checkpoints, credential management, permission controls and end to end tracing. It is billed for model usage plus 0.08 dollars per running hour, and Notion, Asana and Sentry already use it in production. At DevDay (September 29), OpenAI launched the Agents API in public beta, with support for managed execution, memory, multi agent setups and computer use. Google added Managed Agents to the Gemini API in May
* **MCP**: The new specification on July 28 changed the protocol to a stateless, cacheable structure, strengthened authentication and introduced an extensions framework. It solves the scaling problems of multi tenant cloud deployments. There are more than 10,000 public MCP connectors, and the SDK gets 97 million downloads a month
* **Coding agents are the largest agent market today**: Claude Code reached 2.5 billion dollars in annualized revenue (年化收入) within nine months; Cursor's annualized revenue rose from 2 billion dollars in February to more than 4 billion dollars in June
* **Always on personal agents**: Google's Gemini Spark handles tasks for users 24/7 on cloud virtual machines; the open source Hermes Agent (more than 32,000 GitHub stars) can generate and improve its own skills from experience; Tencent (腾讯) opened agent capabilities to all Yuanbao (元宝) users for free
* **Agent payments**: There are many protocols (ACP, UCP, AP2, x402, MPP), but no winner yet. OpenAI shut down Instant Checkout in March and went back to a "discover products, then redirect to the merchant" model, which shows the market has not yet accepted agents paying directly
* **Enterprise adoption**: According to Gartner, 80% of enterprise applications released or updated in the first quarter of 2026 had at least one agent built in; but data from S&P and McKinsey show that only 31% of companies actually have agents running in production (47% in banking and insurance, 18% in healthcare, 14% in government)

**What it means for products**: Building a "general purpose agent" puts you head to head with giants like Google, OpenAI and Tencent. The opportunity is in vertical scenarios: connectors to industry systems, industry knowledge, auditable processes, and helping customers put agents into production safely.

### 2.3 Voice, Images, Video and 3D

**Voice**
* OpenAI launched GPT Live full duplex voice on July 8 and opened the API on September 10 at 0.05 dollars per minute, with built in transcription and turn detection; complex reasoning is handed off to a paired large model (大模型)
* Open source: NVIDIA's NemotronLabs VoiceChat (September) is a full duplex model with native tool use; JD.com's (京东) JoyAI Talker focuses on voice agents with empathy
* Translation: Google Meet's voice dubbing became generally available in February; Shokz (韶音) OpenFit 2 AI earbuds run on Tongyi (通义) speech models and support 30 languages

**Images**
* GPT Image 2 (April) added a thinking mode and multilingual text rendering, and can generate 8 images with consistent characters in one go; GPT Image 2.5 (September 8) comes in a fast version and a refined version; Google's Nano Banana 2 (February) has the edge in speed
* Image generation is already a mature commodity. General purpose tools have no window left; the opportunities are only inside vertical workflows

**Video**
* Native audio has become standard: Veo 3.1, Kling (可灵) 3.0, MiniMax H3 and LTX 2.5 can all generate video with synchronized sound in a single pass. Kling 3.0 supports 15 second single shots, 4K and lip sync in 5 languages; Kling 4.0 Flash entered closed beta on September 28 (3 to 30 seconds, 4K, 10 bit HDR)
* OpenAI shut down the Sora app on April 26 and retired the API on September 24. This shows that a pure video generation tool has a hard time sustaining a consumer product
* Kling AI raised more than 3 billion dollars in the third quarter

**3D**
* Meshy 7 (August) supports PBR materials and automatic rigging, has game engine plugins, and raised a 400 million dollar Series B; Tencent Hunyuan 3D (腾讯混元 3D) 3.1 is offered as a hosted service, and version 2.1 is open source

**What it means for products**: Voice is the modality most worth investing in: the experience has just crossed the usability threshold, prices are low, and many industries are still not covered. Images and video work best as one step inside a workflow, not as standalone products.

### 2.4 On Device AI and Inference Costs

* Gemma 4 (April 2) is open source under Apache 2.0 and has two on device versions, E2B and E4B
* Flagship phone NPUs reach 45 to 60 TOPS, with local generation at 20 to 50 tokens per second
* At WWDC 2026 (June 8), Apple opened its Foundation Models framework to any large model provider, with support for image input. Small developers with fewer than 2 million downloads can use Private Cloud Compute inference for free
* Apple's new Siri AI is powered by both Apple's own models and Google Gemini, understands what is on screen and the user's personal context, and launches this fall as an English beta
* Silicon Data's token price index fell to a record low of 0.97 dollars per million in early September; NVIDIA claims Vera Rubin will cut the cost per token to one tenth of Blackwell's in the second half of this year

**What it means for products**: For scenarios that are privacy sensitive, need to work offline or make high frequency calls, on device inference brings marginal cost close to zero, which can support cheaper or free business models (商业模式).

### 2.5 World Models (世界模型) and Embodied AI

**World models**: Google's Project Genie (based on Genie 3) opened to US Ultra subscribers in January. It generates explorable 720p worlds in real time, with memory lasting about 1 minute. In open source and academic work there are Kunlun Tech's (昆仑万维) Matrix Game 3.5 and DreamForge World, which needs little compute (算力). Overall this is still at the research demo stage: worth watching, but hard to turn into a product in the short term.

**Robot foundation models**
* Physical Intelligence's pi 0.7 (April 16) is a 5 billion parameter vision language action (VLA, 视觉语言动作) model. It can fold laundry even on a robot it was never trained on, showing compositional generalization. It is still a research model
* Google DeepMind's Gemini Robotics 2 (July 30) consists of three models covering whole body control, five finger dexterous manipulation and multi robot collaboration, and is open to developers through the Gemini API

**The humanoid robot industry**
* In the first half, global shipments were about 4 times the level of the same period last year, with Chinese makers accounting for more than 97%. AgiBot (智元) shipped about 8,400 units, ranking first; Unitree (宇树) shipped about 5,900 and had its IPO approved by the listing committee on June 1
* Full year production in 2026 is expected to exceed 100,000 units, about 5 times the 2025 level
* Prices: the Unitree R1 costs about 5,900 dollars and the G1 about 13,500 to 16,000 dollars; Figure 03 is sold only under enterprise contracts
* **The gap between hype and reality**: 1X NEO sells for 20,000 dollars or 499 dollars a month, and its first year batch of 10,000 units sold out in five days, but as of July 16 there had been no verified deliveries to users

### 2.6 AI for Science

* **AlphaEvolve**: Its one year report in May showed that it is already used inside Google for data center (数据中心) scheduling, TPU chip design and compute kernel optimization
* **Drug design**: Isomorphic Labs' Drug Design Engine doubled AlphaFold 3's score on a generalization test for protein ligand structure prediction, but it is not available externally. Meanwhile, DeepMind disbanded the AlphaFold team, and Nobel laureate John Jumper joined Anthropic in June
* **AI scientists**: Google Co Scientist found a candidate drug for fibrosis that blocked 91% of the relevant response in lab tests; FutureHouse's Robin proposed using the glaucoma drug ripasudil for dry macular degeneration, and the idea was confirmed experimentally; AxiomProver wrote machine verifiable proofs in Lean and solved all 12 problems of the Putnam competition; Meta worked with mathematicians to publish 6 math papers using Muse Spark (October)
* **Self driving labs**: There is already research in which LLM agents run automated labs to synthesize new solid state electrolyte materials

**What it means for products**: Most of the value here sits inside large institutions and drug companies. The opportunity for small teams is "research workflow tools" (literature, experiment design, data analysis), but these are relatively far from revenue.

### 2.7 AI Glasses, Wearables and Brain Computer Interfaces (脑机接口, BCI)

**AI glasses**
* Global shipments grew 263% in the first half. Models without displays made up 96%, of which Meta accounted for 94%. Ray Ban Meta sold more than 7 million pairs in 2025
* IDC forecast: models without displays will ship 13.6 million units in 2026 and 27.3 million in 2030; models with displays will grow faster, from 3 million units in 2026 to 12.2 million in 2030, a compound annual growth rate (年复合增长率, CAGR) of 41.9%
* Developer ecosystem: Meta's developer toolkit for its glasses opened in preview in December 2025, with full availability planned for 2026; at IFA in September, Rokid launched AIUI Studio, which can generate glasses apps from natural language, along with an agent store, and has more than 15,000 developers in China
* In China: Alibaba's Quark (夸克) glasses (from 1,899 yuan) and Xiaomi (小米, about one third of the Chinese market). Samsung's smart glasses launch this fall, and Apple is also preparing to enter

**Screenless AI devices**: The first device from OpenAI and Jony Ive is planned to be unveiled in the second half of the year. It is reportedly a screenless home speaker or ear worn device; the form factor has not been confirmed.

**Health wearables**
* Dexcom's over the counter (非处方) continuous glucose monitor (CGM, 连续血糖仪), Stelo, was approved in June for children aged 2 and older; Abbott's Libre Duo was approved in August, the world's first device that monitors glucose and ketones at the same time
* Cuffless blood pressure: RingConn Gen 3 makes blood pressure insights a core feature and went on sale in May; but so far no smart ring has received FDA clearance for blood pressure

**Brain computer interfaces**
* On March 13, China's National Medical Products Administration (NMPA) approved Neuracle's (博睿康) NEO semi invasive brain computer interface for commercial use, to restore partial hand function in patients with cervical spinal cord injuries. It is the world's first brain computer interface available outside clinical trials (临床试验). As of June, China had approved 5 brain computer interface products. BCI is listed as one of the six future industries in the 15th Five Year Plan (“十五五”规划)
* Neuralink's speech restoration and vision restoration programs received FDA breakthrough device designation (突破性器械认定), but all of its programs are still in clinical trials

### 2.8 Biomedicine

* **Oral GLP 1**: Eli Lilly's orforglipron (Foundayo) was approved by the FDA on April 1, the first oral small molecule GLP 1 that can be taken without restrictions on food or water. It went from submission to approval in only 50 days, the fastest approval of a new molecular entity since 2002
* **Semaglutide patent expiry in China**: The core patent expired on March 20, prices fell by more than 50%, and domestic generics are under review
* **Gene editing**: Intellia released the world's first Phase 3 results for an in vivo CRISPR therapy; Beam's in vivo base editing therapy for PKU received IND clearance; Prime Medicine began the first human trial of in vivo prime editing in New Zealand. More than 50 CRISPR trials worldwide are recruiting patients
* **AI clinical documentation**: 29% of US doctors use AI voice documentation tools, known as AI scribes (AI 病历助手), up from 20% in April 2025; 70% of doctors at UCSF use them every day; Kaiser has covered 2.5 million patient visits. Epic launched a native tool and athenahealth offers one for free, so this market is already commoditized in the US
* **Regulation**: As of September, the FDA had authorized more than 1,600 AI medical devices; new guidance on January 6 loosened oversight of clinical decision support (临床决策支持) software
* **AI tutoring results are mixed**: A randomized controlled trial covering 2,379 undergraduates found that offering AI tutoring actually lowered final exam scores by 0.37 standard deviations; structured K12 math pilots showed gains of 0.2 to 0.4 standard deviations. Education products need careful design and cannot assume that "AI tutoring always works"

### 2.9 Energy and Materials

* **Sodium ion batteries**: CATL (宁德时代) and Changan (长安) unveiled the world's first mass produced sodium ion passenger car in February, and cell mass production is planned before the end of the year
* **Solid state batteries**: CATL, BYD (比亚迪), Toyota and Samsung have all set 2027 as the target for all solid state batteries; ProLogium's (辉能) lithium ceramic battery reached 381 Wh/kg in TÜV verification and has entered mass production
* **Perovskite tandem solar photovoltaics (光伏, solar PV)**: LONGi's (隆基) tandem cell reached 35.5% efficiency (July), a world record; Trina Solar's (天合) tandem module reached 907W at 29.2% efficiency. Commercial modules range from 24% to 29% efficiency
* **AI power demand**: US tech giants have signed 13 nuclear power deals totaling more than 9.8 GW; in April Microsoft signed a power purchase agreement (购电协议, PPA) with the fusion company Helion

**What it means for products**: These are all asset heavy sectors that small teams can hardly enter directly. Possible indirect opportunities are software and data services related to energy storage (储能) and charging, but this round did not research them in depth.

### 2.10 Quantum Computing

* Quantinuum's Helios achieved 48 logical qubits with a physical qubit overhead of about 2 to 1, running up to 94, with a logical gate error rate of about 1 in 10,000; QuEra achieved 96 logical qubits on a neutral atom platform; Google Willow ran a 7×7 surface code
* Quantum error correction is moving from research to engineering, but no broad commercial advantage has appeared yet

**What it means for products**: What can be put to work in the short term is security consulting and tools for things like "post quantum cryptography migration." Quantum computing itself is far from anything a small team can productize.

### 2.11 Mobility, Low Altitude (低空) and Satellites

* **Drone delivery**: Meituan's (美团) Keeta drones received a commercial license covering all territory in May, with more than 900,000 cumulative orders; Zipline has made 2.5 million deliveries, its partner merchants grew thirteenfold in the first half, and it completes a delivery every 30 seconds on average; Wing and Walmart plan to cover 270 stores by 2027
* **eVTOL**: EHang's (亿航) EH216 S has obtained all three CAAC certificates and begun commercial operations; a Shenzhen to Zhuhai route is expected to open this year at about 200 to 300 yuan per seat
* **Robotaxis**: Waymo has about 3,000 vehicles and about 500,000 paid rides a week, and added 3 new cities in September; Apollo Go (萝卜快跑) covers 26 cities; Tesla had only 25 unsupervised vehicles operating in Texas in April
* **Direct to cell satellites**: Starlink has more than 650 direct to cell satellites serving 22 countries, and had 16 million cumulative users in March

### 2.12 Chips and Compute

* NVIDIA Vera Rubin ships in the second half of this year, with a claimed cost per token of one tenth of Blackwell's
* Huawei plans to produce about 600,000 Ascend (昇腾) 910C chips in 2026, and up to 1.6 million across the whole series; the 950DT launches in the fourth quarter (144GB HBM); the 960DT has been pulled forward to the first quarter of 2027
* For private deployment in China, test how models run inference on Ascend and other domestic chips in advance

### 2.13 Market Signals and Regulation

**Where the capital is going**
* Global venture capital in the third quarter of 2026 was 159 billion dollars, of which AI took 64% (102 billion dollars); there were 27 rounds of 1 billion dollars or more, a record
* Notable rounds at the application layer: EliseAI (AI for the rental housing industry) raised 350 million dollars at a valuation (估值) of 4 billion dollars; Meshy (3D generation) raised a 400 million dollar Series B

**Where consumers actually spend money**: a16z's 7th consumer AI list, released in October, included credit card spending data for the first time
* The top 1% of spenders spend an average of 903 dollars a month on AI, up 80% over the past 18 months; their total spending is more than that of the bottom 50% of users combined
* The median user spends only 25 dollars a month, with almost no growth
* Heavy spenders mainly buy automation and building tools (n8n, fal, Manus, Hermes Agent) and creative tools (Higgsfield, Figma, HeyGen)
* Of the top 50 products by spending, 29 do not appear in the traffic rankings at all
* **Takeaway**: Products for "prosumers" (专业消费者), people who buy tools for themselves to get work done, have an easier time collecting money and do not need to chase huge traffic

**Consumer AI apps in China**: Doubao has 345 million monthly active users, Qwen (千问) 166 million, DeepSeek 127 million and Yuanbao 114 million. During the Spring Festival, Tencent promoted Yuanbao with large red envelope (红包) giveaways (reported amounts vary, from 1 billion yuan to 10 billion yuan), and in May it launched a feature that summarizes WeChat chat histories. Competition among the big companies for the agent entry point is extremely fierce.

**Regulation**
* **China**: The AIGC labeling measures have been in effect since September 1, 2025 and entered strict enforcement in 2026. They require explicit labels plus implicit labels in metadata; AI advertising materials must carry a metadata watermark containing the brand's credit code. In addition, providing generative AI services also requires algorithm filing (算法备案), a security assessment and real name verification of users
* **EU**: The Digital Omnibus (effective July 27) pushed the compliance deadline for standalone high risk AI systems back from August 2026 to December 2, 2027, but the Article 50 transparency obligations still took effect on August 2, 2026
* **US**: Since January 1, California's SB 243 has required companion chatbots to tell users clearly that they are AI, to remind minors every 3 hours, and to set up suicide intervention protocols. From July 2027, it will prohibit simulating romance or sentience with minors

---

## 3. Scoring Method and Overall Ranking

**Six dimensions**, each scored from 1 to 5. A higher score is more favorable for building a product, and the maximum total is 30:

| Dimension | 1 point | 5 points |
| :--- | :--- | :--- |
| Maturity (成熟度) | Paper or concept | Mature commercial use |
| Accessibility (可获得性) | Out of reach for small teams | Public API, or open source and licensed for commercial use |
| Cost friendliness (成本友好) | Very expensive | Very cheap |
| Ease of productization (易产品化) | Takes years and heavy assets | MVP in a few weeks |
| Window of opportunity (窗口期) | Red ocean (红海), or the platform will build it directly | Plenty of room to differentiate; giants will not cover it soon |
| Low risk (低风险) | High regulatory, safety or legal risk | Low risk |

**Top 15 by total score** (the full list of 48 is in [tech_list.csv](tech_list.csv))

| Rank | Technology | Total | Related product cards |
| :--- | :--- | :--- | :--- |
| 1 | New MCP specification and ecosystem | 28 | D |
| 2 | Cost effective midrange models | 27 | A, B, D, E |
| 3 | Small on device models and phone NPUs | 26 | F |
| 3 | AI search replacing traditional search (GEO) | 26 | B |
| 5 | Open weight frontier models (前沿模型) | 25 | D, F |
| 5 | Managed agent infrastructure | 25 | A, D, I |
| 5 | Controllable image generation | 25 | |
| 5 | Mandatory AIGC labeling (强制标识) and transparency obligations | 25 | C |
| 9 | Apple opening its Foundation Models framework | 24 | F |
| 9 | Full duplex voice models | 24 | A, E |
| 9 | Over the counter continuous biochemical monitoring | 24 | H |
| 12 | Frontier reasoning models | 23 | All |
| 12 | Diffusion language models | 23 | |
| 12 | Real time speech translation and dubbing | 23 | E |
| 12 | 3D asset generation | 23 | |

**How to read these scores**: A high score means "a small team can build a product with it right now." It does not mean the technology is more important. Brain computer interfaces and gene editing, for example, matter enormously, but score very low for small teams. Controllable image generation scores high, but its window of opportunity score is only 2, so a standalone product would run straight into a red ocean. That is why it has no product card of its own.

---

## 4. Risks and Uncertainties

1. **Giants moving in**: OpenAI, Google, Apple, Tencent and ByteDance (字节) are all investing in "personal agents" and "apps inside assistants." Any product too close to general use cases may be replaced by a system level feature. The response is to go deep into vertical industries and private data
2. **The gap between hype and reality**: Home humanoid robots, Tesla Robotaxi, the effect of AI tutoring and agents paying directly have all shown more hype than substance. When judging a technology, look for independently verified delivery data
3. **Restricted access to capabilities**: The strongest cybersecurity capabilities (Mythos, Argon) are open only to a few partners, and other high risk capabilities may go the same way in the future. Do not bet a product on "waiting for some capability to open up"
4. **Regulatory change**: China's labeling rules and algorithm filing, the EU's high risk obligations in 2027, and US state laws on companion AI will all affect consumer products
5. **Data reliability**: This research relied mainly on search summaries and secondhand reports. Some numbers (especially revenue and market share) may be defined differently across sources

---

## 5. Suggested Next Steps

1. **Pick 2 directions and validate them for 2 weeks**: I suggest A (voice receptionist) and B (GEO). For each, interview 10 target users, build a prototype you can demo, and work out the unit economics
2. **Fill in your information**: Tell me your industry background, your team's tech stack and your target market, and I can reprioritize accordingly and look further into the relevant Chinese competitors
3. **Update regularly**: This field changes a lot every month, so the technology list and scores can be refreshed monthly
