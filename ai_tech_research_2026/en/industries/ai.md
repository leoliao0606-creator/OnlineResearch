# Industry Deep Dive 4: The AI Industry

Written October 12, 2026 · World Industry Map series · Previous: [Finance](finance.md) · Chinese version: [../../industries/ai.md](../../industries/ai.md)

Key terms appear with their Chinese equivalent the first time they show up. The full list is in the [bilingual glossary](../../glossary.md).

This piece is about the structure and economics of AI as an **industry**: who invests, who makes money, and where the money comes from. For specific technical progress (models, agents, voice, robotics and so on), see the first round [report.md](../report.md).

**Disclosure**: I (Claude) am made by Anthropic, and Anthropic comes up below. All the related figures come from public reporting, and I have tried to hold Anthropic to the same standards as the other companies.

---

## 0. The Industry in One Sentence

The AI industry is a long chain that runs from **electricity** all the way to **applications**. The picture in 2026:

* **Upstream (上游), the chips,** makes the most money: NVIDIA's gross margin (毛利率) is 75 percent
* **The middle (中游), the large model (大模型) companies,** has seen revenue explode but is still losing large sums
* **Downstream (下游), the applications,** is growing users fast, but inference costs (推理成本) eat a big share of the profit

The whole industry comes down to one central question: **can the downstream eventually create enough value to sustain more than 700 billion dollars a year of investment upstream?**

---

## 1. The Industry Value Chain (产业链)

| Layer | What it does | Representative companies | Profitability in 2026 |
| :--- | :--- | :--- | :--- |
| 1. Power and data center (数据中心) construction | Supplying power, building server halls, cooling | Utilities (电力公司), GE Vernova, builders | Very profitable, demand exceeds supply (see [Energy and Power](energy_power.md)) |
| 2. Chip manufacturing | Lithography machines (光刻机), foundries (晶圆代工), memory chips | ASML (the world's only supplier of high end lithography machines), TSMC, SK hynix, Samsung, Micron | Very profitable. The global memory chip market is expected to grow about 250 percent |
| 3. Chip design | GPUs and specialized AI chips | NVIDIA, AMD, Broadcom (designs custom chips for Google and others); Google TPU, Amazon Trainium; China: Huawei Ascend | NVIDIA is the most profitable, with a 75 percent gross margin |
| 4. Cloud and compute (算力) | Renting out compute | Amazon AWS, Microsoft Azure, Google Cloud, Oracle; neoclouds (新兴算力云) such as CoreWeave | Revenue growing fast, but capital expenditure (capex, 资本开支) is enormous |
| 5. Foundation models (基础模型) | Training and serving large models | OpenAI, Anthropic, Google DeepMind, Meta, xAI; China: DeepSeek, Alibaba's Tongyi, Moonshot AI, Zhipu AI, MiniMax, ByteDance | Revenue soaring, most still losing money |
| 6. Tools and infrastructure | Agent (智能体) platforms, evaluation, monitoring, data access | Agent platforms from the major model companies, the MCP ecosystem, many startups | Fierce competition; easily squeezed from upstream and downstream |
| 7. Applications | Products for end users | Coding: Cursor, Claude Code; healthcare: OpenEvidence, Abridge; consumer: ChatGPT, Doubao | Fast growth, gross margins generally not high |

---

## 2. How the Money Flows

### 2.1 Two Kinds of Money

**Investment (spent up front)**: the four tech giants (Amazon, Google, Microsoft, Meta, often grouped together as hyperscalers, 超大规模云厂商) will spend about **730 billion dollars** in capex in 2026, 78 percent more than in 2025, with more than 60 percent of it going to power, cooling and construction. That money ultimately flows to NVIDIA, TSMC, the memory chip makers and the power equipment makers.

**Revenue (what users actually pay)**: users and companies pay applications, applications pay to call model APIs, model companies pay to rent compute, and cloud companies pay to buy chips.

Both kinds of money end up flowing from downstream to upstream, that is, from layer 7 toward layer 1 in the table above. The difference is timing: investment is spent in advance as a bet on future revenue, while revenue is money users have already paid. How big the gap between the two is, and whether it can be closed, is what the bubble debate in Section 2.4 is about.

### 2.2 How Much Each Layer Earns

| Layer | 2026 figures |
| :--- | :--- |
| Chips | NVIDIA's revenue for the quarter ending in late July was 96.2 billion dollars, up 106 percent year over year (同比), of which data centers were 89 billion dollars; gross margin was 75 percent; next quarter is forecast at 108 billion dollars |
| Model companies | Anthropic's annualized revenue (年化收入) at the end of July was about 65 billion dollars (about 14 billion dollars in February); after its May funding round its valuation (估值) was about 965 billion dollars, and in June it confidentially filed to go public. OpenAI's annualized revenue at the end of September was about 50 billion dollars, with a target of more than 70 billion dollars by year end, but it reportedly expects to lose about 14 billion dollars in 2026, with inference costs rising from 8.4 billion dollars in 2025 to about 14.1 billion dollars. All of these figures come from media reports, not audited data |
| Applications | ICONIQ data shows that AI native (AI 原生) companies have an average gross margin of about 52 percent (traditional software usually runs 70 to 80 percent). Coding tools are lower still: one survey found an average of only about 31 percent, with inference costs eating more than half of revenue. Cursor's gross margin in January 2026 was reportedly even negative; thanks to its own models and cheaper third party models, the enterprise customer part of its business later turned positive in April |

### 2.3 One Piece of Good News and One Piece of Bad News

**The good news (for application companies)**: the price of a given level of capability falls about tenfold every year. Renting an H100 GPU cost more than 7 dollars an hour in early 2024; in 2026 the median is about 3 dollars.

**The bad news (for model companies)**: with prices falling this fast, model companies have to keep pushing the frontier to hold on to their pricing power, while the cost of training each next generation model keeps rising.

### 2.4 The Bubble (泡沫) Debate

* **The bear case**: money is circling among a handful of companies. NVIDIA invests in OpenAI, for example, and OpenAI then uses that money to buy NVIDIA chips. In July, NVIDIA reportedly considered guaranteeing 250 billion dollars for OpenAI's data center in Ohio, and after the news came out, the price of insuring NVIDIA's bonds against default jumped. Some estimate that these "circular deals (循环交易)" exceed 800 billion dollars. Morgan Stanley estimates that AI data center spending could approach 3 trillion dollars by 2028
* **The bull case**: the revenue is real, and it is accelerating. Anthropic and OpenAI together already have more than 100 billion dollars in annualized revenue, and NVIDIA's revenue doubled in a year
* **The historical parallel**: in the telecom bubble around 2000, companies laid huge amounts of fiber. Many of them went bankrupt, but that fiber later carried the entire internet era. A bubble and a real technological revolution can exist at the same time. For founders, the important thing is not to call whether there is a bubble, but **not to build your company on the assumption that the funding environment will stay this good forever**

### 2.5 China

* **Models**: China leads in open source (开源) models. DeepSeek V4, Kimi K3 and GLM 5.2 all have open weights (开放权重). Prices are low, and Doubao has about 345 million monthly active users (月活)
* **Chips**: in January, the US switched H200 exports to China to case by case approval, with a 25 percent tariff (关税) and volume caps, and about 10 Chinese companies were approved; but Chinese customs then reportedly blocked H200s from entering the country. NVIDIA acknowledged in its annual report that it has effectively been shut out of China's data center market. Huawei plans to produce about 600,000 Ascend 910C chips this year
* **The result**: the US and Chinese AI industries are forming two almost independent systems, from chips to models to applications

---

## 3. The Main Players

| Layer | US | China | Elsewhere |
| :--- | :--- | :--- | :--- |
| Chip manufacturing | Micron | SMIC | TSMC (Taiwan), ASML (Netherlands), SK hynix and Samsung (South Korea) |
| Chip design | NVIDIA, AMD, Broadcom | Huawei HiSilicon, Cambricon | |
| Cloud | AWS, Azure, Google Cloud, Oracle, CoreWeave | Alibaba Cloud, Huawei Cloud, Volcano Engine, Tencent Cloud | |
| Models | OpenAI, Anthropic, Google, Meta, xAI | DeepSeek, Alibaba, Moonshot AI, Zhipu AI, MiniMax, ByteDance | Mistral (France) |
| Applications | Cursor, Perplexity, Harvey, OpenEvidence and others | Doubao, Yuanbao, Qwen, Kimi and others | |

---

## 4. Major Shifts in History

| Year | What happened | Winners | Losers or lessons |
| :--- | :--- | :--- | :--- |
| 1956 | The Dartmouth conference, where the term "artificial intelligence" was born | | |
| The 1970s and late 1980s | Two "AI winters" (AI 寒冬): too many promises, not enough compute or data, and the funding pulled out | | The price of overhyping |
| 2006 | NVIDIA launched CUDA, which let GPUs be used for general purpose computing | **NVIDIA**. The bet took more than a decade to pay off, and today it is NVIDIA's biggest moat (护城河) | |
| 2012 | AlexNet trained a deep neural network on GPUs, and the deep learning (深度学习) era began | Google (which acquired the AlexNet team's company), NVIDIA | |
| 2017 | Google published the Transformer paper | The company that later commercialized it most successfully was OpenAI | **The inventor is not necessarily the winner** |
| 2020 | GPT 3 and the "scaling laws (规模定律)": the bigger the model, the stronger it is | Companies with the money to buy compute | The start of an arms race |
| 2022 | ChatGPT launched and became one of the fastest growing consumer products in history | OpenAI, Microsoft | Google was caught on the back foot for a while |
| January 2025 | DeepSeek released a cheap open source reasoning model (推理模型) | The open source camp, users | NVIDIA lost about 600 billion dollars of market cap (市值) in a single day, as the market worried for the first time that "AI does not need that much compute" |
| 2025 to 2026 | Coding agents took off, and capex surged to 730 billion dollars | Chips, power, model companies | To be determined |

**Four lessons from history**:
1. **Infrastructure bets take a long time to pay off.** CUDA took more than a decade
2. **The inventor is not necessarily the winner.** Google invented the Transformer, but OpenAI was first to build a hit product with it. The winner is often the company best at turning technology into products and grabbing the distribution channels (分发渠道)
3. **Hype cycles (炒作周期) are real.** AI has already been through two winters
4. **Cheap open source can suddenly change pricing across an entire industry.** DeepSeek is the example

---

## 5. What Is Changing in 2026

### 5.1 The Revenue Has Really Arrived, but Profits Are Very Unevenly Spread
See Section 2: chips earn a 75 percent gross margin, model companies lose money, and application companies' gross margins are pushed down by inference costs.

### 5.2 Getting AI into Production at Companies Is Still Hard
* An MIT study in 2025: only about 5 percent of enterprise AI pilots (试点) made it into production (生产环境)
* PwC's CEO survey: 56 percent of companies say AI has neither brought in more revenue nor reduced costs
* KPMG, second quarter of 2026: only 7 percent of business leaders say they have seen a clear return on investment (ROI, 投资回报)
* McKinsey: about 6 percent of companies are "high performers" (高绩效者) that can attribute more than 5 percent of their profit to AI
* **What this means**: the technology is already good enough; the bottlenecks are data access, process redesign, permissions, security and trust. This "dirty work" (脏活) is exactly where the opportunity lies for startups

### 5.3 The US and China Diverge
Chip export controls (出口管制) keep changing direction, China leads in open source models, and the two sides' industry chains are increasingly independent of each other (see 2.5).

### 5.4 Power Becomes the Bottleneck
"When can the data center get power?" has become the first criterion for choosing a site, and there are long queues for both gas turbines (燃气轮机) and transformers (变压器) (see [Energy and Power](energy_power.md)).

### 5.5 Regulation
* **US**: efforts to unify AI rules at the federal level have stalled. A presidential executive order (行政令) directs the Justice Department to challenge state AI laws, but an executive order cannot by itself override state law. In 2025, 38 states passed 145 AI related laws; California's SB 53 and Texas's TRAIGA took effect in January 2026; Colorado's AI Act was heavily amended and pushed back to take effect in January 2027
* **EU**: the AI Act's transparency obligations (透明度义务) took effect in August 2026, and the high risk obligations were delayed to December 2027
* **China**: mandatory labeling (强制标识) of AI generated content (AIGC)

### 5.6 The Effect on Jobs, Especially for Newcomers
This one matters to you directly.
* A Stanford study found that in jobs heavily exposed to AI (such as software development), employment of young people aged 22 to 25 has fallen about 16 percent in relative terms since late 2022
* New York Fed data: in the second quarter of 2026, the unemployment rate for recent college graduates was about 5.6 percent, and the share who were underemployed (大材小用) was about 42 percent
* But there is evidence the other way too: another study finds no clear evidence that AI has pushed new graduates out of the labor market; data from the National Association of Colleges and Employers shows hiring demand for the class of 2026 up 5.6 percent; and IBM announced it would triple its entry level hiring
* **Conclusion**: entry level jobs really are getting weaker, especially in software; but whether AI is the main cause is still being debated by researchers

### 5.7 The Strongest Capabilities Are Starting to Come with Restricted Access
Anthropic's Mythos and Google's Gemini 4 Argon are open only to a small number of cybersecurity partners; OpenAI canceled the release of GPT 6.1 Astra over safety concerns (see the first round report).

---

## 6. What Frontline Practitioners Complain About Most

| Who | Biggest headaches |
| :--- | :--- |
| Application founders | Inference costs eat the profit; dependence on model companies, which could launch a competing feature at any time; models update too fast for evaluation to keep up |
| Enterprises | Lots of pilots, very few launches; data access is hard; security (for example prompt injection (提示注入) attacks); cannot clearly explain the return on investment |
| Model companies | Compute is expensive and in short supply; the war for talent; power; regulation and safety |
| Cloud and data centers | Cannot get power, cannot buy transformers, cannot hire electricians |
| Developers | Models are unstable and make things up (hallucination, 幻觉); agents fail in ways that are hard to predict; costs are hard to estimate |
| Students and newcomers | Entry level jobs are disappearing |

---

## 7. Opportunities

### 7.1 First, Look at AI Startups Through Thiel's Framework

Most AI startups are competing with the model companies: a feature you build on top of a model today may be built straight into the model tomorrow. So in AI, what can become a monopoly (垄断) is usually not "the technology itself" but one of the following:
1. **Proprietary data and feedback loops (反馈循环)**: within a particular vertical (垂直领域), more users mean more data, and more data means a better product
2. **Becoming the "system of record (记录系统)"**: like Epic for hospitals. The customer's core data and processes live with you, so replacing you is expensive
3. **Network effects (网络效应)**: protocols, marketplaces, platforms with many kinds of participants
4. **Distribution and brand**: claim a place in users' minds first
5. **Trust and verification**: as AI does more and more, whoever can prove it got things right will be valuable

### 7.2 The First Type: Hot Trends (风口)

| Opportunity | Why now | Signs the wave is receding |
| :--- | :--- | :--- |
| Implementation services that help small and midsize businesses put AI and agents to work | The vast majority of enterprise pilots have not made it into production | Big companies launch out of the box solutions |
| Agent templates, skill packs, MCP connectors | Heavy spending users are willing to pay to get more done | Platforms launch official marketplaces |
| AI evaluation (评测) and quality assurance services | Models update too fast, and companies do not know which one to use | Evaluation tools become standardized |
| AI training (for companies and individuals) | Demand is high and supply is low | Training content becomes free |

### 7.3 The Second Type: Directions That Could Grow into a Monopoly

**1. The verification layer (验证层): proving that AI got it right**
* Direction 2 in the [two kinds of opportunities](../two_kinds_of_opportunities.md) document. As AI generates more and more code, documents and decisions, verification becomes the bottleneck. This direction has shown up in healthcare (auditable AI decisions), finance (verifiable rules) and energy (interconnection (并网) studies), making it a thread that runs across several industries

**2. The trust layer for agents: identity, permissions, accountability**
* Direction 4 in the two kinds of opportunities document. In the finance piece it appears as "know your agent"; in the healthcare piece it appears as "machine to machine claims (理赔)." This, too, is a thread that runs across several industries

**3. A "system of record" for industries that have not been digitized**
* In construction, elder care and small scale manufacturing, a lot of data still lives on paper and in WeChat groups. Software could not get into these industries before because entering the data was too much trouble. Now AI can extract data automatically from photos, voice and documents, which gives these industries their first real chance to have an "Epic" of their own

**4. The "last mile" of enterprise AI adoption: data access and permissions**
* Enterprise AI adoption is hard largely because it gets stuck on connecting data from old systems to agents safely. See product card D in the first round ([product_cards.md](../product_cards.md))

**5. Data from the physical world**
* Direction 1 in the two kinds of opportunities document. The data for language models is nearly used up, but real interaction data from robots, factories and hospitals is only beginning to pile up

**6. Training newcomers in the AI era**
* **A possible secret (秘密)**: if companies hire fewer newcomers because of AI, they will be short of senior people in five to ten years, because every senior person started as a newcomer. Whoever can build "apprenticeship for the AI era" (AI 时代的学徒制), letting newcomers grow quickly by working alongside AI agents on real projects and turning that growth into credible proof of ability, could control the future talent supply chain (供应链)
* **Does it fit you**: you are living this problem yourself, and you are also a heavy AI user. This may be the direction where it is easiest for you to get "frontline observations" (一线观察)
* **What would make it wrong**: AI improves to the point where even senior people are not really needed; or companies quickly go back to hiring newcomers

---

## 8. Signals Worth Watching Next

* Revenue growth and progress toward going public at OpenAI and Anthropic
* Whether NVIDIA hits its guidance (指引) of 108 billion dollars for next quarter
* Whether "circular deals" and data center financing run into trouble
* New surveys on the return on enterprise AI investment
* Changes in US and Chinese chip controls
* Whether the US unifies AI rules at the federal level
* Employment data for new graduates
* The trend in GPU rental prices (a reflection of compute supply and demand)

**Sources worth following over the long term**: Stratechery (business model (商业模式) analysis), SemiAnalysis (chips and compute), Epoch AI (data on AI trends), the Import AI newsletter, Latent Space (a podcast and newsletter); in Chinese, LatePost (晚点) and QbitAI (量子位).

---

## References

* [NVIDIA announces financial results for second quarter fiscal 2027](https://nvidianews.nvidia.com/news/nvidia-announces-financial-results-for-second-quarter-fiscal-2027)
* [OpenAI expects $70 billion in annualized revenue by end of 2026 (Yahoo Finance, Bloomberg)](https://finance.yahoo.com/technology/ai/articles/openai-expects-70-billion-annualized-014338719.html)
* [OpenAI's own forecast predicts $14 billion loss in 2026 (Yahoo Finance)](https://finance.yahoo.com/news/openais-own-forecast-predicts-14-150445813.html)
* [OpenAI revenue, valuation and funding (Sacra)](https://sacra.com/c/openai/)
* [Anthropic revenue, valuation and funding (Sacra)](https://sacra.com/c/anthropic/)
* [Anthropic says it hit a $30 billion revenue run rate (VentureBeat)](https://venturebeat.com/technology/anthropic-says-it-hit-a-30-billion-revenue-run-rate-after-crazy-80x-growth)
* [Anthropic valuation 2026: $965B Series H and the IPO filing (ValueAdd VC)](https://valueaddvc.com/blog/anthropic-valuation-2026-965b-series-h-and-the-ipo-filing-explained)
* [How much are companies spending on AI in 2026 (ValueAdd VC)](https://valueaddvc.com/ai-spending)
* [Nvidia reignites circular AI concerns (Axios)](https://www.axios.com/2026/07/27/nvidia-openai-financing-ai-jensen-huang-ssi)
* [Should we worry about AI's circular deals? (Noah Smith)](https://www.noahpinion.blog/p/should-we-worry-about-ais-circular)
* [The $60 billion company with negative gross margins (Tech Economics)](https://techeconomics.substack.com/p/the-60-billion-company-with-negative)
* [AI startup gross margin statistics 2026](https://ai-industry-reviews.com/research/ai-startup-gross-margin-statistics-2026/)
* [H100 rental price in September 2026 (Akash)](https://akash.network/the-bid/h100-rental-price-2026-cost-per-hour/)
* [The plunging price of thought (Epoch AI)](https://epoch.ai/publications/the-plunging-price-of-thought)
* [The 2026 enterprise AI adoption gap, by the numbers](https://firstlinesoftware.com/blog/the-2026-enterprise-ai-adoption-gap-by-the-numbers/)
* [The AI productivity paradox: 95% of GenAI pilots show no ROI (ValueAdd VC)](https://valueaddvc.com/blog/the-ai-productivity-paradox-why-95-percent-of-genai-pilots-show-no-roi-in-2026)
* [US eases restrictions on Nvidia H200 exports to China (Caixin)](https://www.caixinglobal.com/2026-01-14/us-eases-restrictions-on-nvidia-h200-chip-exports-to-china-102403667.html)
* [Nvidia H200 China exports begin (Khan Capital)](https://khancapitals.com/nvidia-h200-china-exports/)
* [NVIDIA Form 10 K, fiscal 2026 (SEC)](https://www.sec.gov/Archives/edgar/data/1045810/000104581026000021/nvda-20260125.htm)
* [State AI laws take hold as federal preemption stalls (Cloud Security Alliance)](https://labs.cloudsecurityalliance.org/research/csa-research-note-us-ai-regulation-preemption-compliance-202/)
* [Colorado AI Act amended and effective date delayed (Hunton)](https://www.hunton.com/privacy-and-cybersecurity-law-blog/colorado-ai-act-amended-and-effective-date-delayed)
* [Recent college grads say AI is making it harder to get a job. Is it? (NPR)](https://www.npr.org/2026/08/18/nx-s1-5910677/recent-college-graduates-employment-job-artificial-intelligence)
* [AI and entry level jobs: what hiring data really shows (IntuitionLabs)](https://intuitionlabs.ai/articles/ai-entry-level-employment-hiring-data)
* [How to stay ahead of AI as an early career engineer (IEEE Spectrum)](https://spectrum.ieee.org/ai-effect-entry-level-jobs)
