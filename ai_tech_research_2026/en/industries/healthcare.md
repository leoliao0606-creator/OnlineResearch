# Industry Deep Dive 2: Healthcare

Written October 12, 2026 · World Industry Map series · Previous: [Energy and Power](energy_power.md) · Chinese version: [../../industries/healthcare.md](../../industries/healthcare.md)

Key terms appear with their Chinese equivalent the first time they show up. The full list is in the [bilingual glossary](../../glossary.md).

This piece focuses mainly on the US, because the US spends more on healthcare than any other country in the world, and because you are in the US. Each section includes a comparison with China.

---

## 0. The Industry in One Sentence

Healthcare is an industry in which **the people who get treated, the people who treat them, the people who pay, and the people who sell the drugs and devices** are four separate groups.

In most industries, the person who uses a product pays for it, so the market keeps price and quality in check. Healthcare does not work that way: patients usually do not know the price, doctors do not bear the cost directly, and insurers do not treat anyone. **Most of the inefficiency, and most of the opportunity, hides in the handoffs between these four groups**: scheduling, authorization, documentation, billing, review, claim denials (拒付) and appeals (申诉).

---

## 1. The Industry Value Chain (产业链)

| Role | What it does | US examples | China examples |
| :--- | :--- | :--- | :--- |
| Patients | Get care and pay part of the cost: out of pocket costs (自付额) and copays (共付额) | | |
| Providers (医疗服务方) | Hospitals, clinics and doctors deliver care | HCA, Kaiser Permanente, regional health systems | Public hospitals dominate overwhelmingly |
| Payers (付款方) | Collect premiums (保费) and pay medical bills on patients' behalf | Commercial insurance (商业保险): UnitedHealth, Elevance, Cigna, Aetna (owned by CVS), Humana; government: Medicare (联邦医疗保险, for older people), Medicaid (医疗补助, for people with low incomes) | Basic medical insurance run by the National Healthcare Security Administration (国家医保局), covering the vast majority of the population |
| Drug makers | Research, develop and manufacture drugs | Eli Lilly, Johnson & Johnson, Merck, Pfizer, AbbVie; from overseas, Novo Nordisk, Roche, AstraZeneca | Hengrui, BeiGene, CSPC |
| Drug middlemen (中间商) | Wholesale, pharmacies, pharmacy benefit managers (PBM, 药品福利管理) | Wholesale: McKesson, Cencora, Cardinal; PBMs: Express Scripts, CVS Caremark and Optum Rx, three companies that handle about 80 percent of prescriptions | Pharmaceutical distribution companies |
| Devices and diagnostics | Equipment, consumables, testing | Medtronic, Abbott, Intuitive Surgical | Mindray, United Imaging |
| Information systems | Electronic health records (EHR, 电子病历), billing systems | Epic (about 43.7 percent of the US acute care hospital EHR market in 2025, according to a 2026 KLAS report), Oracle Health | |
| Regulators | Approve drugs and devices, set payment rules | FDA, CMS | National Medical Products Administration, National Healthcare Security Administration, National Health Commission |

**What is a PBM?** A PBM manages prescription drug benefits for insurers and employers. It decides which drugs are covered and how much is reimbursed, and it negotiates rebates (回扣) with drug makers. Sitting between drug makers, pharmacies and insurers, it is one of the main reasons US drug prices are so opaque.

---

## 2. How the Money Flows

### 2.1 The US: Where 5.3 Trillion Dollars a Year Goes

Total US health spending in 2024 was about **5.28 trillion dollars**, 18 percent of GDP. CMS projects it will reach 9 trillion dollars by 2034, or 20.6 percent of GDP.

**Where the money is spent**
* Hospitals: about 1.63 trillion dollars, 31 percent
* Doctors and clinics: about 1.1 trillion dollars, 21 percent
* Retail prescription drugs: about 467 billion dollars, 8.8 percent; drugs used inside hospitals account for another 4 to 5 percent

**Who pays**
* Commercial insurance: about 1.6 trillion dollars, 31 percent
* Medicare: about 1.1 trillion dollars, 21 percent
* The rest comes from Medicaid, patients' own pockets and other government programs

**How much goes to "administration"**
* A JAMA article estimated that administrative costs make up 15 to 25 percent of total US health spending; in 2019, nonclinical administrative functions cost about 950 billion dollars
* Another JAMA study estimated that US healthcare wastes between 760 billion and 935 billion dollars a year, and that **"administrative complexity" is the largest category, at about 265.6 billion dollars**
* This is why many startup opportunities in healthcare lie not in "treating illness" but in "processing paperwork"

### 2.2 The Claims (理赔) Game

Most of the money in US healthcare moves through "claims":
1. After a visit, the hospital submits the bill (the claim) to the insurer
2. Some tests and procedures require "prior authorization (预授权)" in advance, and can go ahead only if the insurer agrees
3. The insurer reviews the claim and may pay it or deny it
4. After a denial, the hospital can correct and resubmit the claim, or appeal

To get a feel for the numbers (mostly from industry groups and vendors, so treat them as directional):
* About 12 percent of claims are denied on first submission, with Medicaid the highest at about 17 percent
* According to a Premier survey (cited by the American Hospital Association and others), hospitals spend about 19.7 billion dollars a year handling and overturning denials
* Reworking each denied claim costs about 57 dollars

**A trend under way**: both sides of the claim are now using AI. Hospitals use AI to write appeal letters and to code claims automatically; insurers and the government use AI to review them. This is turning into a contest of "AI versus AI (AI 对 AI)" (see 5.3).

### 2.3 Who Makes Money

| Role | Profitability |
| :--- | :--- |
| Hospitals | Very thin. According to Kaufman Hall, as of June 2026 the median year to date hospital operating margin (营业利润率) index was about 2.5 percent, still about 6 percent below the same period of 2025; bad debt and charity care costs rose about 17 percent year to date; rural hospitals are struggling the most |
| Insurers | They earn the gap between premiums and medical payouts. In the second quarter of 2026 UnitedHealth spent 86.7 percent of premiums on medical costs (its medical care ratio, 医疗赔付率), with the rest going to operations and profit. It also owns Optum (clinics, a PBM, data), which makes it a highly vertically integrated (纵向整合) company |
| Drug makers | Innovative drugs are very profitable. Thanks to its weight loss drugs (减重药), Eli Lilly became the world's first drug company with a market cap (市值) above 1 trillion dollars |
| PBMs | As middlemen controlling about 80 percent of prescriptions, they became a main target of reform in 2026 |
| Information systems | Epic is privately held but is close to a monopoly (垄断) in US hospitals, and it controls doctors' daily workflow (工作流) |

### 2.4 China

* China's total health expenditure in 2024 was about 9.09 trillion yuan, or about 6.7 percent of GDP. Spending by the basic medical insurance fund (including maternity insurance) was about 2.98 trillion yuan in 2024 and passed 3 trillion yuan for the first time in 2025 (about 3.01 trillion yuan)
* Public hospitals dominate, and the government sets the prices of medical services
* **Volume based procurement (VBP, 集中带量采购, or 集采 for short)**: the National Healthcare Security Administration pools purchases of similar drugs and consumables into centralized tenders, and winning bid prices often fall sharply. This has squeezed the profits of generic drug makers and pushed drug companies toward innovative drugs
* **Payment by disease group (DRG/DIP, 按病种付费)**: medical insurance no longer reimburses item by item. Instead it pays the hospital a fixed amount for each disease group, and the hospital absorbs any overspending. By 2024 this covered all pooling regions (统筹地区) and more than 80 percent of the insurance fund's inpatient spending. At many hospitals, revenue barely covers costs
* **Innovative drugs going global**: in the first half of 2026, the total value of out licensing (对外授权) deals for Chinese innovative drugs was about 100 to 110 billion dollars, a record, already about 80 percent of the total for all of 2025; 8 of the world's top 10 out licensing deals came from Chinese companies

---

## 3. Major Players

| Category | Global | US | China |
| :--- | :--- | :--- | :--- |
| Drug makers | Novo Nordisk, Roche, AstraZeneca, Novartis | Eli Lilly, Johnson & Johnson, Merck, Pfizer, AbbVie | Hengrui, BeiGene, CSPC |
| Insurance | | UnitedHealth, Elevance, Cigna, Aetna, Humana | National medical insurance at the core, commercial insurance as a supplement |
| Hospitals | | HCA, Kaiser Permanente, university medical centers | Public top tier (Grade 3A, 三甲) hospitals |
| Devices | Siemens Healthineers, Philips | Medtronic, Abbott, Intuitive Surgical, GE HealthCare | Mindray, United Imaging |
| Health IT and AI | | Epic, Oracle Health; AI companies by valuation (估值): OpenEvidence 12 billion dollars, Abridge about 5.3 billion dollars, Hippocratic AI 3.5 billion dollars | |

---

## 4. Major Upheavals in History

| When | What happened | Winners | Losers |
| :--- | :--- | :--- | :--- |
| 1965 | The US creates Medicare and Medicaid | Older and low income people; the government became the largest payer | |
| 1983 | Medicare switches to diagnosis related groups (DRG, 按诊断分组付费), paying hospitals a fixed amount per diagnosis | Hospitals that control costs | Inefficient hospitals with long stays. The DRG system China is rolling out today is modeled on this approach |
| 1990s | Managed care (管理式医疗) through health maintenance organizations (HMOs) rises, and insurers begin to control what doctors can do | Insurers | Doctors' autonomy; it later triggered a public backlash |
| 2003 (effective 2006) | The US passes the Medicare Modernization Act, and Medicare begins covering prescription drugs (Part D) in January 2006 | PBMs grow rapidly | |
| 2009 | The US government spends tens of billions of dollars subsidizing hospitals to adopt electronic health records | **Epic**, which used this to become a near monopoly in US hospitals | Doctors: the paperwork burden soared and is now one of the main causes of burnout |
| 2010 | The Affordable Care Act (ACA, 平价医疗法案) sets up insurance exchanges and expands Medicaid | Tens of millions of newly insured people; large insurers used the moment to integrate vertically | |
| 2018 | China creates the National Healthcare Security Administration and launches volume based procurement | Patients, as drug prices fell sharply | Generic drug makers |
| 2020 | The COVID pandemic | Telemedicine, mRNA vaccine makers | |
| 2023 to 2026 | GLP 1 weight loss drugs take off | Eli Lilly, Novo Nordisk | Some food and retail companies (see the [World Industry Map](../world_industry_map.md)) |
| 2025 to 2026 | Major overhaul of US health insurance policy (see Section 5) | Still unclear | People losing coverage, rural hospitals |

**Three lessons from history**:
1. **Payment rules drive behavior.** Pay per service (fee for service, 按项目付费) and hospitals do more services; pay per disease group (diagnosis related groups, DRG) and hospitals control costs; subsidize electronic health records and every hospital installs one
2. **Whoever controls the "decision point" captures the value.** Insurers do it through prior authorization, PBMs by deciding which drugs are covered, and Epic by controlling the system doctors use every day
3. **Regulation creates winners.** Epic's position comes largely from the 2009 subsidy policy. That is a reminder for founders: in healthcare, understanding policy often matters more than understanding technology

---

## 5. What Is Changing in 2026

### 5.1 The US: The Insured Population Is Shrinking

* **The enhanced ACA subsidies expired at the end of 2025**: 23.1 million people signed up during open enrollment (开放注册) for 2026, 4.9 percent fewer than in 2025, but KFF expects the number who actually pay their premiums to fall by about 21.5 percent, to around 17.5 million. The average premium per enrollee more than doubled, and about 9 percent of last year's enrollees now have no insurance at all
* **Medicaid cuts**: the One Big Beautiful Bill Act (大而美法案) imposes work requirements starting January 2027, and eligibility checks every six months starting at the end of 2026. One consulting firm estimates that 7.8 million people will lose Medicaid; the CBO estimates that the number of uninsured will rise by about 10 million by 2034
* **Impact on hospitals**: bad debt (坏账) and charity care (慈善医疗) are rising; 432 rural hospitals are at risk of closing; the law also created a 50 billion dollar rural health transformation fund

### 5.2 AI Enters Core Workflows

* 29 percent of US doctors use AI voice tools to write their clinical notes (AI scribes, AI 病历助手)
* In March 2026 Epic launched three AI agents (智能体): Art writes notes and provides clinical support, Penny handles billing, prior authorization and appeals, and Emmie answers patient questions and books appointments. Epic says more than 85 percent of its customers already use its AI tools (these figures come mostly from Epic and its partners)
* In January the FDA loosened its oversight of clinical decision support (临床决策支持) software; more than 1,600 AI medical devices have been authorized
* Medical AI companies carry high valuations: OpenEvidence at 12 billion dollars, Abridge at about 5.3 billion dollars

### 5.3 Prior Authorization Becomes "AI Versus AI"

* Starting in January 2026, in six states (Arizona, New Jersey, Ohio, Oklahoma, Texas and Washington), CMS is piloting AI based prior authorization reviews by private technology companies for 15 categories of services in traditional Medicare (the WISeR model), and these companies can **take a share of the money saved on the services they deny**. This has been highly controversial
* Ironically, CMS announced the model just four days after the major insurers publicly pledged to cut back on prior authorization (June 2025)
* Meanwhile, hospitals are using tools such as Epic's Penny to write appeals automatically. One side uses AI to deny, the other uses AI to appeal

### 5.4 The Politics of Drug Prices

* **GLP 1 most favored nation (MFN, 最惠国) pricing deals** (November 2025): Eli Lilly and Novo Nordisk agreed to cut the price paid by Medicare and Medicaid to 245 dollars a month, with Medicare patients paying a 50 dollar monthly copay; Medicare will cover obesity drugs for the first time
* **TrumpRx**: a government website for buying drugs directly, with cash prices for weight loss drugs of about 149 to 350 dollars a month
* **PBM reform**: a law signed in February 2026 requires PBMs to pass all rebates through to their clients, bans them from profiting on the price spread in Medicare prescription drug plans, and delinks PBM fees from drug list prices (标价). The Federal Trade Commission reached settlements (和解) first with Express Scripts and then with CVS Caremark, and Optum Rx is also moving to a flat service fee model

### 5.5 Insurers Are Pulling Back

* UnitedHealth is voluntarily exiting unprofitable Medicare Advantage plans in 2026 and expects to lose about 1.1 million members
* Medical costs in commercial insurance are growing more than 11 percent a year

### 5.6 Not Enough People

* The Health Resources and Services Administration (HRSA) projects a shortage of about 141,000 physicians by 2038, with the gap in nonmetropolitan areas as high as 58 percent
* The shortage of registered nurses is about 109,000; but nurse practitioners (NP, 执业护士) are projected to be in surplus by about 73,000, which could partly make up for the shortage of primary care (基层医疗) doctors

### 5.7 China

* Out licensing of innovative drugs hit a record, and China is becoming an important source of new drugs for the world
* DRG/DIP has been rolled out nationwide and volume based procurement continues, so hospitals are under heavy cost pressure
* The world's first commercial brain computer interface (BCI, 脑机接口) was approved, and BCI procedures now have billing codes in medical insurance
* Semaglutide's patent has expired, and domestic generics are about to launch

---

## 6. What People on the Front Line Complain About Most

The following is compiled from news reporting, not from direct interviews.

| Who | Biggest headache |
| :--- | :--- |
| Doctors | Writing notes eats up huge amounts of time, prior authorization holds them up, burnout |
| Hospital finance departments | Denials and appeals; more and more uninsured patients and rising bad debt; margins of only about 2 to 3 percent |
| Insurers | Medical utilization and costs keep rising; cost pressure from weight loss drugs |
| Patients | Premiums doubled for ACA enrollees, the average deductible (起付额) hit a record (about 3,786 dollars), bills are hard to understand, and appointments are hard to get |
| Drug makers | Prices are being pushed down, and middlemen such as PBMs take a cut of the profits |
| Chinese hospitals | Budget pressure from payment by disease group, price cuts from volume based procurement, heavy workloads for doctors |

---

## 7. Opportunities

### 7.1 The First Type: Hot Trends (风口)

| Opportunity | Why now | Signs the wave is receding |
| :--- | :--- | :--- |
| Specialty AI scribes for small practices Epic does not reach: dental, mental health counseling, physical therapy and rehabilitation, veterinary | Large hospitals are already locked up by Epic and big companies; small specialty practices are not | General purpose AI scribe tools cut prices and move in |
| Handling denial appeals and prior authorization for small clinics, paid as a share of the money recovered | Denial rates are rising, and having AI write appeals is now feasible | Claims rules are reformed, or large platforms offer the service for free |
| Helping hospitals restore coverage for patients who "lost their insurance" (eligibility screening, help enrolling again, charity care applications) | ACA and Medicaid changes are driving up bad debt | Policy shifts again |
| Companion services for weight loss drugs | Medicare coverage begins, TrumpRx cuts prices | Large platforms launch similar services |
| Price comparison of drugs and services for patients paying cash | Cash prices are increasingly common and increasingly transparent | Government websites and insurers build good versions themselves |

### 7.2 The Second Type: Directions That Could Grow into Monopolies

**1. Machine to Machine Claims Infrastructure**
* **Secret (秘密)**: prior authorization and claims are shifting from "person to person" to "agent to agent." Hospitals have Epic's Penny; insurers and the government have AI review companies. When both sides are machines, they need a neutral protocol, an auditable record, and a "rules engine" that everyone accepts. Whoever becomes the standard for this layer will sit in the middle of trillions of dollars of payments every year
* **Where the monopoly comes from**: two sided network effects (双边网络效应), since both hospitals and insurers plug in; standard status; regulatory acceptance
* **Reference point**: today's claims clearinghouses (理赔清算所), such as Change Healthcare and Availity, already form this kind of middle layer. In 2024 a ransomware attack on Change Healthcare froze a huge volume of claims across the country, which showed how critical this layer is
* **Does it fit you?**: Yes. The core is software, agents and security, which matches your background, and it overlaps with Direction 4 (a trust layer for agents, Agent 信任层) and Direction 2 (verifiable AI) in the [two kinds of opportunities](../two_kinds_of_opportunities.md) document
* **What would make it wrong**: Epic or the big insurers set the standard themselves; regulators push a different solution

**2. Auditable Medical AI Decisions**
* At the heart of the WISeR controversy is this: "An AI denied you, and nobody can explain why." Regulators, hospitals and patients all need records of AI decisions that can be inspected and reproduced. This is where Direction 2 lands concretely in healthcare

**3. AI Enhanced Primary Care**
* **Secret**: nonmetropolitan areas face a physician shortage as high as 58 percent, while nurse practitioners will be in surplus. A "nurse practitioner plus AI" clinic might bring primary care to places short of doctors at a lower cost
* **Barriers**: states set different rules on nurse practitioners' scope of practice (执业范围), and the model needs healthcare operations experience and capital. It is not a good first project, but it is worth watching

**4. Low Cost Care for People Losing Insurance**
* Several million people are losing their insurance, and they still need care. Bundling AI triage, telemedicine, low priced drugs from TrumpRx and tests at cash prices could create a new consumer brand
* The risk is that policy changes quickly, and demand may shift with the next policy adjustment

**5. Home Care and Remote Monitoring**
* This combines population aging, over the counter (OTC, 非处方) continuous glucose monitors (CGM, 连续血糖仪) and noninvasive brain computer interface rehabilitation (see Direction 6 in the two kinds of opportunities document). It suits your ECE background

**6. Faster Clinical Trials (临床试验)**
* Clinical trials are where drug makers spend the most money, and slow patient recruitment is a common problem. The speed at which Chinese drug makers move through clinical trials is one reason they can out license so many drugs. Using AI for patient matching and trial operations is an area where drug makers are willing to pay a premium

---

## 8. Signals to Watch Next

* Third quarter earnings reports (财报) from UnitedHealth and other insurers (from mid October)
* Open enrollment for 2027 ACA plans, starting in November: premiums and enrollment numbers
* Medicaid work requirements formally taking effect in January 2027
* Evaluations of the WISeR model by KFF and others
* The implementation details of PBM reform
* Updates to China's national reimbursement drug list (医保目录) and innovative drug licensing deals
* How widely Epic's AI agents are actually adopted

**Sources worth following over the long term**: KFF (the most authoritative nonprofit research organization on US health policy), Health Affairs, STAT News, Fierce Healthcare and Healthcare Dive; for the drug distribution channel, read Drug Channels.

---

## References

* [National health care spending increased 7.2% in 2024 (Health Affairs)](https://www.healthaffairs.org/doi/10.1377/hlthaff.2025.01683)
* [US health spending reached $5.3T in 2024 (Healthcare Dive)](https://www.healthcaredive.com/news/us-healthcare-spending-2024-cms-health-affairs/809578/)
* [National Health Expenditure Projections 2025 to 2034 (CMS)](https://www.cms.gov/files/document/national-health-expenditure-projections-results-presentation.pdf)
* [Six trends reshaping US drug spending (Drug Channels)](https://www.drugchannels.net/2026/02/latest-cms-data-reveal-six-trends.html)
* [Administrative expenses in the US health care system (JAMA)](https://jamanetwork.com/journals/jama/fullarticle/2785479)
* [Administrative simplification and the potential for saving a quarter trillion dollars (JAMA)](https://jamanetwork.com/journals/jama/fullarticle/2785480)
* [Medical billing denial statistics 2026](https://www.gomedicalbilling.com/medical-billing-denial-statistics-2026)
* [Hospital performance improves in June, but lags 2025 (Fierce Healthcare, August 2026)](https://www.fiercehealthcare.com/providers/hospital-performance-improves-june-lags-2025)
* [UnitedHealth Group Q2 2026 earnings release (SEC)](https://www.sec.gov/Archives/edgar/data/0000731766/000073176626000191/earningsrelease2q26_7152.htm)
* [How has ACA marketplace enrollment changed in 2026 (KFF)](https://www.kff.org/affordable-care-act/how-has-aca-marketplace-enrollment-changed-across-states-in-2026/)
* [9% of ACA enrollees go uninsured after subsidies expire (CNBC)](https://www.cnbc.com/2026/03/19/aca-enrollees-uninsured.html)
* [ACA marketplace deductibles surge in 2026 (AJMC)](https://www.ajmc.com/view/aca-marketplace-enrollment-and-affordability-take-historic-hit-as-enhanced-tax-credits-expire)
* [Hospitals brace for federal Medicaid cuts (HFMA)](https://www.hfma.org/finance-and-business-strategy/hospitals-brace-for-looming-federal-cuts-in-medicaid-and-elsewhere/)
* [How the OBBBA undermines healthcare (Chartis)](https://www.chartis.com/insights/how-obbba-undermines-healthcare-and-harms-america)
* [Examining the potential impact of Medicare's WISeR model (KFF)](https://www.kff.org/medicare/examining-the-potential-impact-of-medicares-new-wiser-model/)
* [CMS launches WISeR model (DLA Piper)](https://www.dlapiper.com/en/insights/publications/2026/01/cms-wiser-model)
* [Epic unveils AI agents (Healthcare IT News)](https://www.healthcareitnews.com/news/epic-unveils-ai-agents-showcases-new-foundational-models)
* [Epic is letting health systems build their own agents (MedCity News)](https://medcitynews.com/2026/03/epic-hospital-ai-agent/)
* [OpenEvidence raises $250M at $12B valuation (SiliconANGLE)](https://siliconangle.com/2026/01/21/healthcare-ai-startup-openevidence-raises-250m-12b-valuation/)
* [Trump announces deals with Lilly, Novo to cut weight loss drug prices (AJMC)](https://www.ajmc.com/view/trump-announces-deals-with-eli-lilly-novo-nordisk-for-lower-weight-loss-drug-prices)
* [PBM reforms signed into law (AJMC)](https://www.ajmc.com/view/pbm-reforms-signed-into-law-reshaping-medicare-part-d-drug-pricing-transparency)
* [Congress has more work to do before PBM reform reaches consumers (ProMarket)](https://www.promarket.org/2026/10/06/congress-has-more-work-to-do-before-pbm-reform-reaches-consumers/)
* [The Big 3 PBMs: market share (IntuitionLabs)](https://intuitionlabs.ai/articles/big-three-pbms-market-share)
* [State of the US health care workforce 2025 (HRSA)](https://bhw.hrsa.gov/sites/default/files/bureau-health-workforce/data-research/State-of-US-Health-Care-Workforce-2025.pdf)
* [Physician shortage could reach 86,000 (AAMC via Chief Healthcare Executive)](https://www.chiefhealthcareexecutive.com/view/physician-shortage-could-reach-86-000-aamc-projects)
* [Value of China's innovative drug out licensing deals hit new high in H1 (Xinhua)](https://english.news.cn/20260720/f4f0de6f4d10466abadf953f156cedc8/c.html)
* [China innovative drug out licensing reaches new high (Yahoo Finance, Reuters)](https://finance.yahoo.com/healthcare/articles/china-innovative-drug-licensing-deal-074952473.html)
* [China medtech 2026 (Simon Kucher)](https://www.simon-kucher.com/en/insights/china-medtech-2026-new-era-innovations-and-complexity)
* [China's NHSA regulations on DRG/DIP payment (CMS Law)](https://cms.law/en/chn/legal-updates/china-s-nhsa-issued-the-regulations-on-drg-dip-healthcare-security-payment-mechanism)
* [Health financing growth in China (Frontiers in Public Health)](https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2025.1633222/full)
* [Medicare's new adventure: the Part D drug benefit (Commonwealth Fund, March 2006)](https://www.commonwealthfund.org/publications/fund-reports/2006/mar/medicares-new-adventure-part-d-drug-benefit)
* [KLAS 2026 EHR market share report (HIT Consultant, May 14 2026)](https://hitconsultant.net/2026/05/14/klas-2026-ehr-market-share-report/)
* [2024 China health statistical bulletin (Xinhua, December 2 2025)](https://www.news.cn/politics/20251202/c879035250804e9995ccb8d284656f67/c.html)
* [2025 national healthcare security statistical bulletin (NHSA, July 16 2026)](https://www.nhsa.gov.cn/art/2026/7/16/art_7_21451.html)
