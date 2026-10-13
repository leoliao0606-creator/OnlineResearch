# Which Directions Fit Your Background

Written October 6, 2026, and revised October 7 based on what you added. The earlier documents are [two_kinds_of_opportunities.md](two_kinds_of_opportunities.md) (two kinds of opportunities) and [report.md](report.md) (first round of research). Chinese version: [../personal_fit.md](../personal_fit.md).

---

## 0. What I Know About You, and What I Do Not

**What you told me**
* Sophomore at Olin College of Engineering (欧林工程学院), majoring in ECE, with limited industry experience
* Has studied software, algorithms and AI and machine learning, and uses AI and agents heavily every day
* Does not yet know global industries well; helping you learn them is one goal of this conversation. That is why I also wrote [world_industry_map.md](world_industry_map.md)
* Future products need not be limited to ECE

**What I could not open**: your LinkedIn. This environment's network policy blocks linkedin.com, so I did not see your profile. If there are projects or skills you want me to consider, paste them in.

**A corrected assumption**: in the first version I assumed you knew China's tech industry fairly well. That was wrong, and the judgments based on it have been removed.

---

## 1. A Realistic Starting Point

Against the seven questions from *Zero to One*, your weakest areas right now are "team" and "secret." That is completely normal for a sophomore and not a problem.

A sophomore's biggest assets are not experience but these:
* **Time**: mistakes are cheap, so you can try several directions
* **Being a student**: professors, labs and companies are more willing to spend time with a student
* **Building skills**: you can build both hardware and software, which is rare among founders
* **Location**: you are in Boston, next to clusters of robotics and life science companies

Thiel's "secrets" usually come from three places: depth at the technical frontier, an unusual position or experience, and frontline observation. With little industry experience, you do not have the third yet, but you can deliberately build the first two.

So my advice: **over the next two years or so, the goal is not to find your second type company right away, but to put yourself where secrets become visible.** Meanwhile, use small first type projects to practice, earn money and gather frontline observations.

---

## 2. Your Possible Unfair Advantages (不公平优势)

1. **ECE**. Many second type directions combine hardware and AI: power electronics (电力电子), sensors, robotics, embedded systems, chips. Founders with only a software background find these hard to enter, which is itself a barrier.
2. **Olin's way of teaching**. Olin is known for projects and hands on work. The senior SCOPE capstone is a full year project with a real company, and you can cross register for one entrepreneurship course per semester at Babson.
3. **Boston**. The MassRobotics accelerator (加速器) supports a cohort of hardware robotics startups each year: 13 weeks and 100,000 dollars of non dilutive funding (不占股份的资助) per company, with an acceptance rate of about 8 percent. Labs at MIT and Harvard, and many life science and robotics companies, are nearby.
4. **Software, algorithms and machine learning**. You are not limited to hardware; pure software and AI directions are also open to you.
5. **You are a heavy user of AI and agents**. This may be underrated. Paul Graham's advice is to "live in the future, then build what's missing." Most people and companies are far behind you in how they use AI. The inconveniences you hit every day with agents, and the steps you keep fixing by hand, may be problems most people will only meet years from now. Start a "missing log" (缺失日志): every time you think "I wish something could do this," write it down along with what you were doing and where you got stuck. Months later, it may contain clues to a secret.
6. **You can read information in both Chinese and English**. Much industry information exists in only one language; people who can read both see a more complete picture.

---

## 3. Something That Happened This Summer That Affects You Directly

On July 28, 2026, the US Federal Communications Commission (FCC) added two kinds of foreign made equipment to its Covered List (覆盖清单). **New models can no longer get authorization for import or sale.** Previously approved models are not affected, and government use is exempt.

### 3.1 Robots

* The ban covers foreign made humanoid robots (人形机器人) and quadruped robots, and reportedly autonomous mobile robots and connected wheeled robots weighing more than 4.4 pounds
* China holds about 85 percent of the market for these robots. Media widely report that **US university robotics labs rely heavily on cheap Chinese robots**; Unitree's main US customers are universities and research institutes
* Background: K Scale Labs, a US startup building low cost open source (开源) humanoids, failed to find a lead investor, canceled all orders and released its full hardware and software designs. That was before the ban, in a different market environment

### 3.2 Inverters (逆变器), plus Plug In Solar (插电式太阳能)

* The rule covers foreign made inverters that operate in parallel with the grid (grid tied under UL 1741) and **have remote communication capability**. After the FCC's August 20 revision, wired connections such as Ethernet, and models with a reserved port for a communication module, also count. "Foreign made" is judged by the Buy American standard: the cost of US made components (domestic content, 本土含量) must exceed 65 percent of the cost of all components, rising to 75 percent from 2029; domestic products that qualify for the 45X advanced manufacturing tax credit are not considered foreign made
* Department of Energy data from 2020, cited by the FCC, show that US headquartered manufacturers accounted for only **7 percent** of US inverter shipments; since then domestic capacity has grown substantially under Inflation Reduction Act (IRA) incentives, and Wood Mackenzie counts more than 100 GW of announced new domestic inverter capacity
* At the same time, a new product category is emerging in the US: **plug in balcony solar (插电式阳台太阳能)**, small solar panels you plug straight into an ordinary wall outlet
  * As of the end of September, ten states have signed laws allowing it: New Jersey signed on September 1, and California Governor Newsom signed SB 868 on September 30 (effective January 1, 2027). The New York legislature has passed a bill awaiting the governor's signature; about 30 states have introduced bills
  * **Massachusetts**: the House passed its bill on February 26 and the Senate on July 1; a conference committee was formed on July 16 and first met on July 29, but as of early October it has not produced a compromise version, so the bill has not reached the governor yet
  * The dedicated safety standard, UL 3700, was published between late 2025 and early 2026 (sources differ slightly on the date). The first certified products appeared only in July and August; APsystems' EZ1 sells for 325 dollars. Enphase has no balcony solar product in the US yet

### 3.3 Through Thiel's Lens

This is an unusual situation: **a brand new small market where the strongest competitors (the lowest cost foreign makers) are shut out of new models, and the skill required is exactly a core ECE skill.**

But one point must come first: **protection created by policy can disappear when policy changes.** A new administration or a court ruling could remove it. That is Thiel's durability question: will you still hold your position in ten years? If you take this path, the product must be competitive even without protection; policy is only a tailwind at the start.

Also, competition is not zero: previously approved foreign models can still be sold, and off grid (non grid tied) inverters and products with no communication capability at all are outside the ban; but since the August 20 revision, grid tied inverters that connect only through wired interfaces, or that have a reserved port for a communication module, are restricted too.

---

## 4. Directions Ranked for Your Background

You added a software, algorithms and AI background and said you are not limited to ECE, so this table is ranked for the combination of hardware, software and AI.

| Direction | Fit | Reason |
| :--- | :--- | :--- |
| **New A: US made connected microinverters (微逆变器) for plug in solar, and aggregation later** | High | Power electronics is core ECE; the later step of "aggregating into a virtual power plant (虚拟电厂)" is a software and algorithms problem; the market is brand new; new foreign models are blocked |
| **New B: US made research and teaching robot platforms** | High | Uses hardware, embedded systems and machine learning; clear demand from university labs; can grow into "Direction 1: a data flywheel for the physical world" |
| **Direction 2: verifiable AI** | High | Works from both the software and the hardware side: verifying chips and embedded firmware, or verifying AI generated code; AI's ability to write Lean proofs just broke through |
| **Direction 4: a trust layer for the agent economy** | Medium high | As a heavy agent user you are among the first to feel agents making mistakes, overstepping permissions and leaving no clear accountability; you can build the technical part (identity, permissions, audit logs), and you would need a cofounder who understands actuarial work for the insurance part |
| **Direction 9: AI native service companies** | Medium high | Fluency with agents is a direct advantage; the weakness is that you need to know one service industry very well, which you can start building through the industry map |
| Direction 5: hardware signatures for sensors and cameras | Medium | Needs embedded and hardware security knowledge; insurance claims (理赔) and industrial inspection have clear demand |
| Direction 8: vertical world models (世界模型) for simulation testing | Medium | A machine learning direction; can extend from the robotics direction |
| Direction 6: noninvasive brain computer interfaces (脑机接口) plus rehabilitation | Medium | Brain signal acquisition and signal processing are your strengths, but medical registration takes years; best with a cofounder from medicine |
| Directions 3 and 10 | Low for now | Need chemistry or biology, or consumer brand experience. You could partner with people who have these later |

### New A: US Made Connected Microinverters for Plug In Solar

**Possible secret**: plug in solar may be one of the most underrated new consumer electronics categories in the US, and it is being born exactly when the strongest foreign competitors are shut out of new models.

**Expanding from a small market in concentric circles**: renters in states with laws → more states (Massachusetts and others are moving) → adding batteries → aggregating thousands of small systems into a virtual power plant and selling flexibility to the grid (电网) → an energy data platform.

**First steps you can take now**
1. Read the full UL 3700 standard and the FCC rule, and work out what "domestic components above 65 percent of component cost" means for a real bill of materials (for example, where the chips come from and where assembly happens). This is a key question I have not verified
2. Find a professor who works on power electronics and turn a low power microinverter prototype into a course project or independent study
3. Interview 20 renters and installers in states with plug in solar laws: what they buy now, what worries them, and how much they would pay

**What would make it wrong**: the policy is reversed; previously approved foreign models are cheap and good enough; imported grid tied products with no communication features at all take the market; the capital needed for UL and FCC certification and US manufacturing is beyond a student team; Enphase launches a similar product.

### New B: US Made Research and Teaching Robot Platforms

**Possible secret**: research in US university labs is built largely on Chinese robots, and new models can no longer come in. Whoever becomes the default platform for labs after the ban accumulates papers, code and datasets, creating network effects (网络效应), much as TurtleBot and ROS did in teaching and research.

**Expanding in concentric circles**: teaching kits → research platforms → hardware for robot data collection → small scale commercial deployments.

**First steps you can take now**
1. Ask robotics labs at Olin and around Boston: which robots do you use now? What problems do you face buying new models after the ban? What is your budget?
2. Starting from K Scale's open source designs, estimate the cost of manufacturing in the US
3. Study why K Scale failed, and judge whether the ban changes those reasons

**What would make it wrong**: US manufacturing costs too much for labs to afford; existing older models are good enough for years; established US makers cut prices; the policy changes.

---

## 5. First Type Projects That Suit a Student

**Principle: pick projects next to your second type candidates.** That way you earn money while gathering frontline observations in that direction.

| Project | Adjacent second type direction | Notes |
| :--- | :--- | :--- |
| Data collection hardware for robotics labs and startups, such as portable grippers or data gloves | New B, Direction 1 | Uses ECE directly; customers are in Boston |
| AI voice receptionists or agent automation for local small businesses | Direction 9 | Low barrier; quick contact with real customers |
| Apps for AI glasses (Meta's developer toolkit, Rokid) | Direction 5 | Student developers can claim an early spot |
| Selling agent templates, MCP connectors and automation workflows | Direction 4 | Pure software; fast to start |

**A path that has closed**: I had considered a trading business, "sell cheap Chinese robots to US labs." The July ban keeps new models out, so this path is essentially closed.

---

## 6. A Roadmap for the Next Two Years or So

**Now until next summer: explore**
* Build a small prototype in each of two candidate directions, for example a low power inverter and a low cost robot module
* Have 50 conversations with potential customers across the two directions
* Join a relevant lab (power electronics or robotics)
* Take an entrepreneurship course at Babson
* Aim for a summer internship at a frontier company, ideally in one of your candidate directions

**Junior year: converge**
* Choose one direction and take the prototype deeper
* Look for cofounders at Olin, MIT and Babson
* For robotics, apply to the MassRobotics accelerator; for energy, find similar programs
* Try to earn at least a little revenue

**Senior year: decide**
* Try to align your SCOPE capstone with your direction
* Decide whether to start a company right away, or first work for a year or two at a frontier company in that direction. The second path is common, because many secrets are only visible from the inside

**About the Thiel Fellowship**: this is Thiel's own program. It gives 250,000 dollars over two years to people aged 22 or under without a bachelor's degree, who must drop out or pause college if selected. The 2026 class had only 12 people, and applications are accepted year round. My advice: **do not apply for the money.** Consider it once you have found a direction you would pursue full time no matter what and have a working prototype. The cost is losing progress toward your degree and Olin's resources.

---

## 7. What I Still Need from You

1. After reading [world_industry_map.md](world_industry_map.md), which 3 to 5 industries do you most want to explore in depth?
2. Technically, what do you enjoy most: power electronics, embedded systems, signal processing, chip design, robotics, machine learning, or agents and software systems?
3. Over the next few years, do you want to start a company in the US, in China, or are you open to both?
4. Do you have any projects you have done or are working on?

---

## References Added in This Document

* [Olin curriculum and SCOPE (Olin College)](https://www.olin.edu/academics/curriculum)
* [Olin cross registration FAQ (Olin College)](https://www.olin.edu/academics-registrars-office/semester-information-registration-faq)
* [MassRobotics Accelerator](https://www.massrobotics.org/massrobotics-accelerator/)
* [Thiel Fellowship (Wikipedia)](https://en.wikipedia.org/wiki/Thiel_Fellowship)
* [Thiel Fellowship 2026 application guide (Capitaly)](https://www.capitaly.vc/blog/thiel-fellowship-application-guide-2026)
* [FCC bans foreign humanoid robots (Washington Post)](https://www.washingtonpost.com/technology/2026/07/28/fcc-bans-foreign-humanoid-robots-expanding-campaign-against-chinese-tech/)
* [US bans imports of new Chinese robots (Al Jazeera)](https://www.aljazeera.com/economy/2026/7/29/us-bans-imports-of-new-chinese-robots-over-security-concerns)
* [Trump's AI protectionism has come for robotics (MIT Technology Review)](https://www.technologyreview.com/2026/08/03/1141056/trumps-ai-protectionism-has-come-for-robotics/)
* [Experts react to FCC limits on robot imports (The Robot Report)](https://www.therobotreport.com/industry-reacts-fcc-ban-u-s-imports-new-humanoid-quadruped-robots/)
* [FCC robot rule explained (botinfo.ai)](https://botinfo.ai/articles/fcc-robot-rule-2026)
* [K Scale Labs cancels K Bot orders, open sources all IP (Humanoids Daily)](https://www.humanoidsdaily.com/news/k-scale-labs-cancels-k-bot-orders-open-sources-all-ip-after-funding-fails)
* [US FCC bans import of foreign made power inverters (Orrick)](https://www.orrick.com/en/Insights/2026/08/US-FCC-Bans-Import-of-Foreign-Made-Power-Inverters)
* [FCC bans foreign produced solar inverters (pv magazine USA)](https://pv-magazine-usa.com/2026/07/28/fcc-bans-foreign-produced-solar-inverters-grid-lockout-begins-today/)
* [Concerns over lack of clarity as US bans foreign power inverters (Energy Storage News)](https://www.energy-storage.news/concerns-over-lack-of-clarity-transparency-as-us-bans-foreign-power-inverters/)
* [How balcony solar went from illegal to law in 9 US states](https://www.promptquorum.com/balcony-solar/how-balcony-solar-became-legal-in-the-us)
* [The US's first UL 3700 balcony solar microinverter (Electrek)](https://electrek.co/2026/07/20/us-first-ul-3700-balcony-solar-microinverter-hoymiles/)
* [Plug in balcony solar moves from hack to household (IEEE Spectrum)](https://spectrum.ieee.org/plug-in-solar-power)
* [Massachusetts H.5175 plug in solar bill update](https://pluginsolarus.com/learn/massachusetts-h5175-plug-in-solar)
* [States OK balcony solar, safety guidelines haven't caught up (Stateline)](https://stateline.org/2026/09/30/states-want-balcony-solar-safety-guidelines-havent-caught-up/)
* [FCC issues updates to Covered List entry on foreign produced power inverters (Mayer Brown, August 21 2026)](https://www.mayerbrown.com/en/insights/publications/2026/08/fcc-issues-updates-to-covered-list-entry-on-foreign-produced-power-inverters)
* [WoodMac: new domestic inverter manufacturing could meet US solar demand (Solar Power World, August 2026)](https://www.solarpowerworldonline.com/2026/08/woodmac-new-domestic-inverter-manufacturing-could-meet-us-solar-demand/)
* [California gives the green light to balcony solar (Electrek, October 1 2026)](https://electrek.co/2026/10/01/california-gives-the-green-light-to-balcony-solar/)
