# Two Kinds of Opportunities: Fads and Monopolies

Written October 6, 2026, as a correction to the first round of research. See [report.md](report.md) and [product_cards.md](product_cards.md) for the first round. Chinese version: [../two_kinds_of_opportunities.md](../two_kinds_of_opportunities.md).

Key terms appear with their Chinese equivalent the first time they show up. The full list is in the [bilingual glossary](../glossary.md).

---

## 0. What the First Round Got Wrong

The first round scored each technology on "can a small team build with it right now," so mature, cheap and easy technologies scored highest. By Thiel's standard, that criterion points almost exactly the wrong way: **the easier something is to build, the more people build it, the fiercer the competition, and the thinner the profits.** Most of the ten product cards from the first round belong to what you call the first type: a hot trend (风口).

So this round takes a different approach:
1. Treat the two types separately and judge them by different standards
2. For the second type, offer directions, possible "secrets" and entry points rather than specific products, so as not to box in your imagination
3. End with a set of building blocks and questions you can combine on your own

---

## 1. Thiel's Framework: The Filter for This Round

The video you shared is Lecture 5 of the 2014 Stanford course "How to Start a Startup," titled [Competition is for Losers](https://www.youtube.com/watch?v=5_0dVHMpJlo), given by Peter Thiel. Together with his book *Zero to One* (从 0 到 1), the core ideas are these:

**1. There are only two kinds of businesses: perfect competition (完全竞争) and monopoly (垄断).**
Companies in perfect competition cannot make money because competitors eat away their profits. Every valuable company is a monopoly in some sense.

**2. Two kinds of lies.**
Competitive businesses like to describe their market as small and unique, as the "intersection" of several small markets, for example "the only British restaurant in Palo Alto." They look like they have no rivals, but they are really competing with every restaurant. Monopolies do the opposite. They describe their market as huge, as the "union" of many markets, to hide their dominance.

**3. Four sources of monopoly.**
* **Proprietary technology (专有技术)**: it should be ten times better than the next best option
* **Network effects (网络效应)**: the more people use it, the more valuable it becomes
* **Economies of scale (规模经济)**: the bigger you get, the lower your unit cost
* **Brand (品牌)**

**4. Start small: win a large share of a small market, then expand in concentric circles.** Amazon started with books. Facebook started with Harvard.

**5. Last mover advantage (最后进入者优势).** Most of a company's value comes from cash flows ten or twenty years out. What matters is not being first, but being the last company in a category, the one nobody can replace.

**6. Secrets (秘密).** His most famous question: "What important truth do very few people agree with you on?" Great businesses are often built on a belief that others have not seen yet, or do not believe.

**A small note**: you used the phrase "disruptive product," but in *Zero to One* Thiel specifically warns against being obsessed with disruption (颠覆). If you define yourself as the one who will topple some giant, your attention goes to the opponent rather than to creating something new. In his framing, the better phrase is "**create something new that has no competition yet**." The difference shapes how you choose a direction: look for what nobody is doing, not for whom you can beat.

**The seven questions from *Zero to One***, which you can apply to every direction below:
1. Engineering: is your technology a breakthrough, or just an incremental improvement?
2. Timing: is now the right time to start?
3. Monopoly: are you starting with a big share of a small market?
4. People: do you have the right team?
5. Distribution: can you not only build the product but also sell it?
6. Durability: will your position still be defensible in ten or twenty years?
7. Secret: have you found an opportunity that others do not see?

---

## 2. The Second Type: Ten Directions That Could Grow into Monopolies

These are not products. Each is "a direction plus a possible secret." For each one, I cover what recently changed, what the secret might be, where a monopoly would come from, which small market you could start in, who is already there, and what would make the thesis wrong.

One overall observation first: **in the past six months, capital outside China has already rushed into several of these directions**, such as AI driven scientific discovery, grid (电网) scheduling and insurance for agents. By Thiel's logic, arriving late is not necessarily fatal, but you should not compete head on. Either find a smaller, more specific entry point, or choose a market the leaders do not cover, such as China, a particular industry, or an unusual data source.

### Direction 1: A Data Flywheel for the Physical World

**What changed**
* Robot foundation models (基础模型) are starting to show "compositional generalization": Physical Intelligence's pi 0.7 can fold laundry on a robot it was never trained on, and Google's Gemini Robotics 2 is now available through an API
* The industry estimates the data gap at over 99 percent. Collecting data by teleoperation (遥操作) needs equipment worth over 200,000 yuan per set plus labor at about 300 yuan a day; portable collection kits cost 0.6 to 1.2 dollars per episode; real robot data sells for 500 to 1,000 yuan per hour
* China already has at least 90 data collection centers, 64 of them operating; embodied AI (具身智能) startups in China raised nearly 30 billion yuan in the first quarter of 2026

**Possible secret**: Everyone is racing to build robots and train large models. But what stays scarce over time may be **real interaction data generated continuously inside one specific setting**. Data collection centers that sell data by the hour will soon be crowded, which makes them a first type business. The second type approach is to actually deploy robots in one setting, use the data from deployment to improve the model, deploy more as the model improves, and then expand into neighboring settings.

**Where the monopoly comes from**: data network effects, scale within the setting, and customers' switching costs (切换成本).

**Where to start**: sample handling in labs (standardized workflows, high value per task), supply and medicine delivery inside hospitals, folding in commercial laundries, food prep in chain restaurant kitchens.

**Who is already there**: many data collection centers; robot makers such as AgiBot building their own data; outside China, Physical Intelligence and Google.

**What would make it wrong**: if models can learn from simulation and internet video alone, real robot data stops being scarce; or robot makers move up into applications themselves.

**Time and barriers**: 5 to 10 years; needs hardware, operations, and access to customers in the target setting.

### Direction 2: Verifiable AI, Proving That AI Output Is Correct

**What changed**
* AxiomProver wrote machine checkable proofs in Lean and solved all 12 problems of the Putnam competition
* In July, Mistral released Leanstral 1.5, a model built for Lean proofs; Amazon made the largest donation to date to the Lean foundation; someone has already built a working pipeline from Rust code to Lean proofs
* Pramaana Labs raised a 27 million dollar seed round (种子轮) in June to apply formal verification (形式化验证) to law, pharma and tax
* Meanwhile, the volume of AI written code is exploding (Claude Code's annualized revenue (年化收入) already exceeded 2.5 billion dollars in February 2026 and has kept growing fast since), and AI is better than most human experts at finding vulnerabilities (Claude Mythos found thousands of zero day vulnerabilities (零日漏洞))

**Possible secret**: When AI writes most code and documents, the bottleneck shifts from "production" to "trust." Formal verification used to be so expensive that only aerospace and chip companies used it. AI cuts the cost of writing proofs by orders of magnitude, so "provably correct" may go from a luxury to an entry requirement in some industries. Whoever becomes the accepted verification standard in an industry gains a position similar to a certification body.

**Where the monopoly comes from**: proprietary technology, acceptance by regulators and industry standards, and a brand built on trust.

**Where to start**: automotive functional safety software, smart contracts, financial clearing and billing rules, medical device software, chip design verification, tax rule engines.

**Who is already there**: Harmonic, Pramaana Labs, Logical Intelligence, and research teams at the major model labs.

**What would make it wrong**: customers and regulators only accept "testing" and will not pay more for "proof"; or models become reliable enough that proof is unnecessary.

**Time and barriers**: 3 to 8 years; best for someone with a formal methods background or deep familiarity with a safety critical industry.

### Direction 3: Own the Discoveries Instead of Selling AI Research Tools

**What changed**
* Lila Sciences reached a valuation (估值) above 1.3 billion dollars after its 2025 Series A, and in June 2026 it was reported to be in talks to raise about 2 billion dollars at a valuation of about 8.5 billion dollars; Periodic Labs raised a 300 million dollar seed round, and in 2026 it was reported to be raising at least 500 million dollars at a valuation of about 7.5 billion dollars. Both are building autonomous labs with AI scientists
* Isomorphic Labs' new drug design engine doubled AlphaFold 3's performance, and the company chose not to release it
* Google opened AlphaEvolve to all Google Cloud customers in July 2026; Google's Co Scientist and FutureHouse's Robin both have discoveries validated by experiments

**Possible secret**: The market for research software is small and budgets are tight, so selling tools does not make much money; and tools like AlphaEvolve are becoming available to everyone, so the tool itself is hard to defend. **The money is in the intellectual property of the discoveries.** That is why Isomorphic keeps its model private. A small team's opportunity is not to build "general scientific superintelligence" but to pick a narrow category where experiments are cheap, iteration is fast, patents are defensible and there are clear buyers downstream. Then run the experimental loop yourself and hold the patents yourself.

**Where the monopoly comes from**: patents, plus experimental data that keeps accumulating.

**Where to start**: fragrance and flavor molecules, industrial enzymes, battery electrolyte additives, coating and adhesive formulas, agricultural biostimulants, pet nutrition.

**Who is already there**: Lila and Periodic pursue general directions with large capital; industry incumbents have their own R&D departments.

**What would make it wrong**: the experimental loop costs more than expected; or the discoveries are hard to sell because downstream buyers have too much bargaining power.

**Time and barriers**: 5 to 10 years; needs a chemistry or biology background and a lab.

### Direction 4: A Trust Layer for the Agent Economy: Identity, Audit and Insurance

**What changed**
* Starting in January 2026, ISO, the US body that drafts standard policy forms, introduced optional generative AI exclusions (除外条款) that insurers can add to commercial general liability policies at renewal; AIG, W. R. Berkley and others have filed similar exclusions with regulators. If a company's agent makes a mistake, more and more policies may not pay
* Specialized agent insurance has appeared: AIUC (which certifies and insures), Klaimee (backed by YC), and Testudo (backed by Lloyd's)
* Agents are beginning to pay and sign on behalf of users (protocols such as ACP and AP2); 31 percent of enterprises already run at least one agent in production

**Possible secret**: Once software starts signing, paying and making commitments on behalf of people and companies, society needs infrastructure like credit reporting (征信) and insurance to price "how reliable is this agent." The most valuable asset may not be an insurance license but **historical data on agent failures**: whoever collects the most incident data can set the most accurate prices, accurate prices win more business, and more business brings more data.

**Where the monopoly comes from**: data network effects, scale, and regulatory licenses.

**Where to start**: coverage for errors made by AI phone receptionists or AI bookkeeping at small businesses; behavior audits and certification labels for agents, similar to product quality certification; handling disputes caused by AI customer service in China.

**Who is already there**: AIUC, Klaimee, Testudo and Munich Re outside China. Nothing found in China yet (not verified).

**What would make it wrong**: large insurers quickly launch standardized AI coverage; or models become reliable so fast that the risk, and the demand, disappears.

**Time and barriers**: 3 to 7 years; needs a background in insurance, actuarial work or compliance (合规).

### Direction 5: Authenticity Infrastructure: Proving "This Is Real" in a World Flooded with AI Content

**What changed**
* China now enforces its AI content labeling rules, and the EU's transparency obligations (透明度义务) have taken effect
* C2PA content credentials (内容凭证) are now built into professional cameras from Sony, Leica, Nikon and Canon and into the camera pipelines of most phone makers; the upload systems of AP and Reuters support them
* In May 2026, SAS reported that AI faked damage photos are becoming a new insurance fraud threat; advanced fakes can already forge metadata such as capture time, and even fake C2PA marks

**Possible secret**: Detecting fakes is an arms race you can never win, because detection falls behind every time generative models improve. The durable approach is to **prove what is real**: sign at the moment of capture and keep the chain of credentials unbroken. The value is not the technology itself but becoming the widely accepted proof of authenticity in an industry, somewhat like a notary.

**Where the monopoly comes from**: network effects (capture devices and verifiers use the same credentials), standard setting status, and brand.

**Where to start**: claim (理赔) photos in auto and property insurance, inspections of used cars and secondhand luxury goods, acceptance photos on construction projects, photos in ecommerce reviews, legal evidence.

**Who is already there**: Truepic, Adobe's Content Authenticity Initiative, the major camera makers, and court backed blockchain evidence platforms in China.

**What would make it wrong**: phone makers or platforms turn this layer into a free system feature; or industries refuse to change how they capture images.

**Time and barriers**: 3 to 6 years.

### Direction 6: Neurorehabilitation: Noninvasive Brain Computer Interfaces plus AI plus Home Therapy

**What changed**
* In March 2026, China approved Neuracle's NEO, the world's first implantable brain computer interface (脑机接口) to win market approval; by June, China had approved five BCI products, three of them noninvasive EEG rehabilitation systems
* Of China's registered BCI studies, 79.1 percent are noninvasive, and stroke rehabilitation accounts for 65 percent of them
* China's national medical insurance has created billing items for BCI: a noninvasive fitting fee of up to about 966 yuan per session, and an invasive implantation fee of about 6,000 to 6,600 yuan
* BCI is one of six "future industries" in China's 15th Five Year Plan; new rules effective May 1 make it easier for hospitals to lead early clinical research

**Possible secret**: Everyone is watching the science fiction story of invasive implants. But stroke patients are numerous, rehabilitation resources are chronically short, and national insurance has opened a billing channel for noninvasive BCI. The real business may be a closed loop: **the hospital prescribes, the patient keeps training at home, and AI adjusts the program based on brain signals**. The moat (护城河) is clinical data and hospital channels.

**Where the monopoly comes from**: device registrations, clinical data, insurance billing codes, hospital channels.

**Where to start**: upper limb rehabilitation after stroke; attention and autism interventions for children (some reported effects, but standardization is still hard).

**What would make it wrong**: weak evidence of efficacy leads insurers to pull back; hardware becomes a commodity and a price war (价格战) follows.

**Time and barriers**: 5 to 10 years; needs experience with medical device registration.

### Direction 7: Let Compute Follow Power: A Scheduling Layer Between AI Workloads and the Grid

**What changed**
* Emerald AI is valued at 1.05 billion dollars; in a pilot it cut a data center's (数据中心) power use by 25 percent during peak demand while keeping compute (算力) quality; it formed an AI energy management alliance with Google and NVIDIA
* US tech giants have signed more than 9.8 GW of nuclear power deals; electricity has become the bottleneck for AI expansion
* China has its "East Data, West Computing" program, and renewable power in the west is often curtailed; mass produced sodium ion batteries will make energy storage (储能) cheaper

**Possible secret**: Many AI training and inference tasks can run a bit later or somewhere else. Flexible load (负荷) is exactly what the grid lacks most. Whoever sits between "schedulable compute" and "the grid and renewables" connects both sides and builds two sided network effects (双边网络效应).

**Where the monopoly comes from**: two sided network effects, scheduling data, licenses to trade in power markets.

**Where to start**: edge inference clusters with storage next to renewable plants in western China; or aggregating small and midsize computing centers to join demand response (需求响应) programs.

**Who is already there**: Emerald AI in the US; some virtual power plant (虚拟电厂) companies in China.

**What would make it wrong**: power market reform moves too slowly; or AI workloads turn out to be less flexible than expected.

**Time and barriers**: 5 to 10 years; needs a background in the power industry.

### Direction 8: Vertical World Models: Simulation as Training Ground and "Exam Hall"

**What changed**
* Google's Genie 3 generates interactive worlds in real time; in the open source (开源) and academic world there are low compute real time world models (世界模型) such as Matrix Game 3.5 and DreamForge World
* By the end of 2025, China had 3.287 million drones registered under its real name system, and they flew 45.3 million hours that year (the Civil Aviation Administration of China says the number passed 4.7 million in the first half of 2026); Meituan's drones have a commercial license covering all territory; China's three carriers have deployed 5G Advanced low altitude sensing networks in more than 20 major cities

**Possible secret**: The first big business for world models may not be games but **exams**. Self driving cars, drones and robots all need testing across huge numbers of extreme scenarios before they go live. Whoever owns the most trusted simulated world for a domain becomes part of the certification process.

**Where the monopoly comes from**: proprietary technology, scenario data, acceptance by regulators.

**Where to start**: simulation and safety assessment for urban low altitude drone routes (customers are local governments and drone operators); predeployment testing for warehouse robots.

**What would make it wrong**: regulators only accept real flight tests; or world models never become physically accurate enough.

**Time and barriers**: 4 to 8 years.

### Direction 9: AI Native Service Companies: Deliver Results, Not Tools

**What changed**
* Models can now work autonomously for hours, and managed agent infrastructure has matured
* Global IT services spending is about 1.6 to 1.9 trillion dollars a year (Gartner, depending on the definition), more than five times the SaaS market; YC's summer 2026 list of startup ideas features AI native services
* An industry blog estimates that companies delivering services with AI could reach 75 to 85 percent gross margins, close to software, while charging three to five times what a software subscription costs; but ICONIQ data show that the average gross margin of AI products was only about 45 percent in 2025 and is expected to be about 53 percent in 2026

**Possible secret**: In many industries, customers do not want to buy software; they want "the job done." A service company where AI does 80 percent of the work and charges by outcome (按结果收费) can cut prices in a niche to a fraction of what traditional providers charge while earning far higher margins than providers that deliver with people, and possibly approaching software margins over time.

**Through Thiel's lens**: services are naturally close to perfect competition. A monopoly is only possible if you become ten times cheaper and ten times faster in a niche, and turn case data and reputation into a brand. So this direction sits between the two types: it starts fast, but whether it becomes the second type depends on execution.

**Where to start**: cross border ecommerce compliance (taxes and product certification in many countries), patent search and office action responses, export documentation, bookkeeping and tax filing for small businesses, preparing insurance claim files.

**Time and barriers**: can reach meaningful revenue in 1 to 3 years; the key is knowing one service industry extremely well.

### Direction 10: Redesign Consumer Products for the "GLP 1 Era"

**What changed**
* About one in eight US consumers uses a GLP 1 drug. A Cornell study found that households on these drugs spend 5.3 to 8 percent less per grocery trip, about 10 percent less on snacks, and about 8 percent less at fast food restaurants and coffee shops
* JPMorgan estimates this could cost the food and beverage industry 30 to 55 billion dollars in annual sales by 2030 to 2034
* An oral GLP 1 was approved in April; semaglutide's core patent in China expired in March, prices fell by more than 50 percent, and Chinese generics are under review

**Possible secret**: Tens of millions of people are having their appetite and tastes changed by drugs, but the food industry's recipes, portion sizes and channels are all designed for people who want to eat more. This is a rare structural shift in consumer demand caused by technology, and China's wave has only just started.

**Where the monopoly comes from**: brand, one of Thiel's four sources; combined with users' health data, there is also a data advantage.

**Where to start**: high protein, small portion meals; nutrition supplements that prevent muscle loss while on the drug; community plus ecommerce for people taking these drugs.

**What would make it wrong**: many people stop taking the drugs, so demand does not last; or big food companies quickly launch matching product lines.

**Time and barriers**: 2 to 5 years; also sits between the two types.

---

## 3. The First Type: Hot Trends That Can Make Quick Money Now

Start with a typical example of a wave that is already receding: **humanoid robot (人形机器人) rentals**. In early 2025, renting a humanoid robot for a commercial performance typically cost 10,000 to 20,000 yuan a day, and people talked about "paying back the robot in a week." By 2026, most event rentals had fallen to 3,000 to 5,000 yuan, some platforms offered a 999 yuan trial package, and a Unitree robot on JD.com rented from 1,796 yuan a day. The market grew from about 1 billion yuan toward 10 billion yuan, but the price per rental fell by more than half within a year.

This is the typical path of a hot trend: **the demand is real, but the barrier is low, so many people rush in and prices fall fast.** The keys to a first type business are to move fast, stay asset light, put cash flow first, and decide in advance when you will leave.

| Hot trend | How it makes money | Estimated window | Signs the wave is receding |
| :--- | :--- | :--- | :--- |
| AI voice receptionists and phone agents | Deploy for clinics and stores, charge monthly | 12 to 24 months | Booking software and telecom vendors build the same feature |
| GEO as a managed service | Monitor and improve how AI recommends a brand, charge a service fee | 12 to 18 months | AI platforms launch official ads or brand data products |
| AI content labeling compliance | Tools plus consulting to fix labeling workflows | 6 to 12 months (EU grace period ends December 2) | Platforms label content automatically at generation |
| Enterprise AI coding and agent rollout | Training and implementation, priced per project | About 12 months | Vendors' official training and certification mature |
| Apps for AI glasses | Launch early in the Rokid Agent Store and on Meta's toolkit when it opens | 6 to 18 months | Stores flood with similar apps, or platforms build them in |
| Localizing short videos for cross border sellers | Dubbing and lip sync with tools like Kling | 6 to 12 months | Ecommerce and video platforms add one click translation |
| Agent templates and workflows for heavy spenders | Sell templates, skill packs and courses. a16z data shows the top 1 percent of spenders pay 903 dollars a month on AI, mostly for automation and building tools | 6 to 12 months | Templates become free, platforms launch official template stores |
| Early apps in new channels | Claim a spot early in ChatGPT plugin extensions and the agent ecosystems of Yuanbao and Doubao | 6 to 12 months | Platforms start taking a big cut, or a few apps dominate traffic |
| GLP 1 related products | High protein food, companion apps, community commerce | 1 to 2 years after Chinese generics launch | Big brands launch similar lines |
| Outsourced data collection for embodied AI | Build collection sites and sell data by the hour (currently 500 to 1,000 yuan per hour) | About 12 months; 90 centers already exist | The hourly price of data falls fast |
| Humanoid robot rentals and performances | Already receding; not recommended | Past the peak | Already visible: prices fell by more than half in a year |

**The two types are not opposites.** Many second type companies found their "secret" on the front line while running a first type business. Slack, for example, started as an internal chat tool at a game company. If you do a first type business now, carry one question with you: "In this business, what data or patterns can I see that others cannot?"

---

## 4. Reclassifying the Ten Cards from the First Round

| Card | Type | Reason | What it would take to become the second type |
| :--- | :--- | :--- | :--- |
| A Voice receptionist | First | Low barrier, many rivals, platforms will build it in | Accumulate call and booking data in one industry, extend into payments and customer management, become that industry's operating system |
| B GEO monitoring | First | Several players abroad; platforms may step in anytime | Become the data standard or settlement layer between brands and AI assistants; very hard |
| C Content labeling | First | The window is set by regulatory grace periods | Move toward the authenticity infrastructure in Direction 5 |
| D MCP connectors | Mostly first | Low technical barrier | Become the de facto standard for connecting an industry to agents |
| E Translation and dubbing | First | Platforms will build it in soon | Hard |
| F On device (端侧) meeting notes | First | Apple and phone makers may do it directly | Hard |
| G Assistant for frontline workers on glasses | In between | Deep use case, but you do not control the hardware | Accumulate first person industrial data, move toward Direction 1 |
| H GLP 1 companion | In between | Brand opportunity | Move toward Direction 10 |
| I Code security audits | First (crowded) | Many competitors | Move toward verifiable software in Direction 2 |
| J Embodied AI applications | Entry point to the second type | Long cycle, high barrier | Move toward the data flywheel in Direction 1 |

---

## 5. Thinking Tools for You

### 5.1 New Building Blocks from the Past Six Months

These are things that became **possible** or **cheap** between April and October 2026. Treat them as building blocks and combine them with old problems in an industry you know.

**AI capabilities**
1. AI can work autonomously for hours on complex tasks, for example porting a C project to Rust in 9.5 hours
2. Natural voice conversation that can be interrupted and can listen while speaking, at 5 cents a minute
3. Free local models on phones (flagship phone NPUs reach 45 to 60 TOPS)
4. Machine checkable mathematical proofs written in Lean
5. AI that finds and patches software vulnerabilities on its own
6. Diffusion language models (扩散语言模型) that generate over 1,000 tokens per second, about ten times faster than ordinary models
7. Any software can be called by AI through a common protocol (MCP)
8. Early protocols for AI paying on behalf of users
9. A 15 second video with multilingual lip sync and sound effects, generated in one pass
10. Textured 3D models ready for games, generated in 30 to 60 seconds
11. 3D worlds you can walk around in, generated in real time

**The physical world**

12. A humanoid robot that can walk and run for about 6,000 dollars
13. Robots that complete tasks they were never taught, following spoken instructions
14. A skin patch that tracks both blood sugar and ketones, sold over the counter (非处方)
15. An oral weight loss drug (减重药) with no food restrictions; semaglutide prices in China down more than 50 percent
16. One time gene editing inside the human body to treat disease: Intellia's in vivo CRISPR therapy already has Phase 3 results, and in vivo base editing has entered clinical trials
17. Brain computer interfaces approved for commercial use and with insurance billing codes (China)
18. Drone delivery with a commercial license covering all territory (Meituan)
19. Ordinary phones connecting directly to satellites (Starlink's direct to cell service has served more than 16 million users in total)
20. Mass produced sodium ion batteries: cheap and good in the cold
21. AI glasses with developer access to first person video and audio

### 5.2 A Combination Exercise

1. List the three industries or groups of people you know best, as specific as possible, for example "dental clinics in small Chinese county towns" or "factory owners who export"
2. For each, write down the problems everyone complains about but nobody has solved for years
3. Randomly pick two or three building blocks from the list above and combine them with those problems. Can you assemble something that was impossible before?
4. Run it through the seven questions from *Zero to One*, especially three: is it ten times better? Does it start in a small market? Will it still be defensible in ten years?
5. Finally, ask yourself Thiel's question: on this topic, what do you believe that most people disagree with?

### 5.3 Watch Out for the "Intersection Market" Trap

If you catch yourself proving there is no competition by saying "we are the only company doing A plus B plus C," for example "the only company using AI to answer phones for pet clinics in small towns," be careful. It often means you are drawing a small empty circle inside a crowded big market. A real small market is a group of people with highly similar needs, where you can quickly win most of the share and then expand outward.

---

## 6. What I Can Help with Next

1. Pick 2 or 3 of these ten directions that resonate most, and I will dig deeper: map the players globally and in China, find which small markets are still open, list the key assumptions, and design cheap ways to test them
2. If you are willing to share your background (major, industry experience, resources), I can help judge where you have an unfair advantage (不公平优势). This matters in Thiel's framework, because secrets often come from your unique experience
3. If you want to start with a first type trend to make money, I can turn one into an actionable plan

---

## References Added in This Document

* [Lecture 5: Competition is for Losers, Peter Thiel (YouTube)](https://www.youtube.com/watch?v=5_0dVHMpJlo)
* [Peter Thiel lecture transcript, annotated (Genius)](http://tech.genius.com/Peter-thiel-lecture-5-business-strategy-and-monopoly-theory-annotated)
* [Zero to One (Wikipedia)](https://en.wikipedia.org/wiki/Zero_to_One)
* [How Peter Thiel teaches Stanford students to create monopolies (VentureBeat)](https://venturebeat.com/entrepreneur/how-peter-thiel-teaches-stanford-students-to-create-billion-dollar-monopolies-in-3-quotes/)
* [2026 Outlook on China's Embodied AI Data Collection and Data Industry (EO Intelligence, in Chinese)](https://www.fxbaogao.com/detail/5506283)
* [Data gap above 99 percent: three companies race to million hour embodied datasets (21st Century Business Herald, in Chinese)](https://m.21jingji.com/article/20260807/herald/c3f0293737efe64214803b10e38cc8ca.html)
* [Prediction: AI will make formal verification go mainstream (Martin Kleppmann)](https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html)
* [A Rust to Lean Verification Pipeline with AI Provers (arXiv 2605.30106)](https://arxiv.org/abs/2605.30106)
* [Formal verification is becoming AI's next competitive moat (Gray Reserve)](https://grayreserve.com/articles/formal-verification-enterprise-ai-reliability-moat)
* [Lila Sciences tops $1.3 billion valuation (Yahoo Finance)](https://finance.yahoo.com/news/exclusive-ai-lab-lila-sciences-101645391.html)
* [Startups raise $1.3B for AI scientists in materials discovery](https://kronosteknoloji.com.tr/news/startups-raise-1-3b-for-ai-materials-discovery-20260307)
* [Who Pays When an Agent Gets It Wrong: 2026 AI agent liability and insurance (Zylos)](https://zylos.ai/research/2026-07-10-ai-agent-liability-insurance-underwriting/)
* [Insurers face hidden AI liability as agent risks multiply (Insurance Business)](https://www.insurancebusinessmag.com/us/news/technology/insurers-face-hidden-ai-liability-as-agent-risks-multiply-582433.aspx)
* [Verisk to roll out new general liability exclusions for generative AI exposures (Big I, late 2025)](https://www.independentagent.com/vu_resource/verisk-to-roll-out-new-general-liability-exclusions-for-generative-ai-exposures/)
* [Insurers grapple with new fraud threat: AI generated images (SAS)](https://www.sas.com/en_us/news/press-releases/2026/may/synthetic-images-ai-insurance-fraud.html)
* [Digital provenance explained (Devoteam)](https://www.devoteam.com/expert-view/digital-provenance-explained/)
* [BCI pricing standards announced (Sina Finance, in Chinese)](https://finance.sina.com.cn/roll/2026-04-23/doc-inhvnnwy4995730.shtml)
* [National Healthcare Security Administration creates BCI pricing items (Xinhua, in Chinese)](https://www.news.cn/politics/20250312/fe2136ab44e84620b9e93c35de17822b/c.html)
* [China grants world's first market approval for invasive BCI product (Macau Business)](https://macaubusiness.com/china-grants-worlds-first-market-approval-for-invasive-bci-product/)
* [Emerald AI and Nvidia fast pass for data center grid connects (Fortune)](https://fortune.com/2026/03/31/emerald-ai-nvidia-fast-pass-data-center-grid-connects/)
* [Emerald AI, Google and NVIDIA launch grid flexible alliance (DataCenter News)](https://datacenter.news/story/emerald-ai-google-nvidia-launch-grid-flexible-alliance)
* [From flying aircraft to managing the sky: building low altitude networks in 2026 (in Chinese)](https://yuanxiangsky.com/N/752.html)
* [AI Native Service Companies: why YC bets big on them in 2026 (Kanopy)](https://kanopylabs.com/blog/ai-native-service-companies-yc-bets-2026)
* [GLP 1 drug use cuts grocery spending by 6% (Food Dive)](https://www.fooddive.com/news/glp-1-drug-use-cuts-grocery-spending-by-6-study-finds/736313/)
* [GLP 1 drugs are changing how Americans eat (CNBC)](https://www.cnbc.com/2026/03/21/glp-1-diets-restaurants-protein-fiber-weight-loss-drugs.html)
* [Humanoid robot rentals grew ninefold in a year: real trend or transition? (National Business Daily, in Chinese)](https://www.nbd.com.cn/articles/2026-03-15/4292843.html)
* [The price and survival battle in humanoid robot rentals (China News Service, in Chinese)](https://www.chinanews.com.cn/cj/2026/02-04/10565239.shtml)
* [CRISPR clinical trials: a 2026 update (Innovative Genomics Institute)](https://innovativegenomics.org/news/crispr-clinical-trials-2026/)
