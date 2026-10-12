# 产业深挖二：医疗健康

写于 2026年10月12日 · 世界产业地图系列 · 上一篇：[能源与电力](energy_power.md)

这一篇以美国为主，因为美国是全世界医疗花钱最多的国家，你也在美国；每一节会附上中国的对照。

---

## 0. 一句话看懂这个产业

医疗是一个"**看病的人、治病的人、付钱的人、卖药卖设备的人**"分别是四拨人的产业。

在大多数产业里，用产品的人自己付钱，所以价格和质量会被市场调节。医疗不是这样：病人通常不知道价格，医生不直接承担费用，保险公司不直接看病。**大部分的低效和机会，都藏在这四拨人之间的交接里**：预约、授权、记录、开账单、审核、拒付、申诉。

---

## 1. 产业链

| 角色 | 做什么 | 美国代表 | 中国代表 |
| :--- | :--- | :--- | :--- |
| 患者 | 看病，付一部分钱（自付额、共付额） | | |
| 医疗服务方 | 医院、诊所、医生提供诊疗 | HCA、凯撒医疗、各地医疗系统 | 公立医院占绝对主导 |
| 付款方 | 收保费，替病人付医疗费 | 商业保险：UnitedHealth、Elevance、Cigna、CVS 旗下的 Aetna、Humana；政府：Medicare（老人）、Medicaid（低收入人群） | 国家医保局管理的基本医保，覆盖绝大多数人口 |
| 药企 | 研发和生产药品 | 礼来、强生、默沙东、辉瑞、艾伯维；海外的诺和诺德、罗氏、阿斯利康 | 恒瑞、百济神州、石药 |
| 药品中间商 | 批发、药房、药品福利管理（PBM） | 批发：McKesson、Cencora、Cardinal；PBM：Express Scripts、CVS Caremark、Optum Rx，三家处理约 80% 的处方 | 医药流通企业 |
| 器械与诊断 | 设备、耗材、检测 | 美敦力、雅培、直觉外科 | 迈瑞、联影 |
| 信息系统 | 电子病历、计费系统 | Epic（据报道占美国急症医院电子病历市场约 42%）、Oracle Health | |
| 监管 | 审批药品器械、制定支付规则 | FDA、CMS | 国家药监局、国家医保局、国家卫健委 |

**PBM 是什么**：PBM 替保险公司和雇主管理处方药福利，决定哪些药能报销、报多少，并和药企谈回扣。它站在药企、药房和保险公司中间，是美国药价不透明的重要原因之一。

---

## 2. 钱怎么流

### 2.1 美国：每年 5.3 万亿美元流向哪里

2024 年美国医疗总支出约 **5.28 万亿美元**，占 GDP 的 18%。CMS 预计到 2034 年达到 9 万亿美元，占 GDP 的 20.6%。

**钱花在哪里**
* 医院：约 1.63 万亿美元，占 31%
* 医生和诊所：约 1.1 万亿美元，占 21%
* 零售处方药：约 4,670 亿美元，占 8.8%；医院内使用的药另外再占 4% 到 5%

**谁在付钱**
* 商业保险：约 1.6 万亿美元，占 31%
* Medicare：约 1.1 万亿美元，占 21%
* 另外还有 Medicaid、患者自付和其他政府项目

**有多少花在了"管理"上**
* 一篇 JAMA 文章估计，行政管理支出占美国医疗总支出的 15% 到 25%；2019 年非临床的行政职能花了约 9,500 亿美元
* 另一篇 JAMA 研究估计，美国医疗每年的浪费在 7,600 亿到 9,350 亿美元之间，其中**"行政复杂度"是最大的一类，约 2,656 亿美元**
* 这就是为什么医疗里很多创业机会不在"治病"，而在"处理文件"

### 2.2 理赔这场游戏

美国医疗的钱，大部分是通过"理赔"流动的：
1. 医院看完病，把账单（理赔申请）提交给保险公司
2. 有些检查和手术要事先申请"预授权"，保险公司同意了才能做
3. 保险公司审核，可能付钱，也可能拒付
4. 被拒付后，医院可以修改重提，或者申诉

数字感受一下（多来自行业机构和厂商，作为方向参考）：
* 首次提交被拒付的比例约 12%，Medicaid 最高，约 17%
* 美国医院协会估计，医院每年花约 197 亿美元去推翻拒付
* 每重新处理一份被拒的理赔，成本约 57 美元

**一个正在发生的趋势**：理赔双方都在用 AI。医院用 AI 写申诉信、自动编码；保险公司和政府用 AI 审核。这正在变成一场"AI 对 AI"的较量（见 5.3）。

### 2.3 谁赚钱

| 角色 | 赚钱情况 |
| :--- | :--- |
| 医院 | 很薄。2026 年 3 月医院调整后的年内营业利润率中位数约 1.7%，农村医院最困难 |
| 保险公司 | 赚的是保费和赔付之间的差。UnitedHealth 2026 年二季度把 86.7% 的保费用于医疗支出，其余用于运营和利润；它同时拥有 Optum（诊所、PBM、数据），是一家高度纵向整合的公司 |
| 药企 | 创新药利润很高。礼来因为减重药成为全球第一家市值过万亿美元的药企 |
| PBM | 作为中间商控制约 80% 的处方，2026 年成为改革的重点对象 |
| 信息系统 | Epic 是私有公司，但在美国医院里接近垄断，掌握着医生每天的工作流 |

### 2.4 中国的情况

* 2023 年中国卫生总费用约 9.06 万亿元，基本医保基金支出从 1.78 万亿元增长到 2.97 万亿元
* 公立医院占主导，医疗服务价格由政府定
* **集中带量采购（集采）**：国家医保局把同类药品、耗材集中招标，中标价格往往大幅下降。这让仿制药企业的利润被大幅压缩，迫使药企转向创新药
* **按病种付费（DRG/DIP）**：医保不再按项目报销，而是按疾病组给医院一个固定金额，医院花多了自己承担。到 2024 年已覆盖所有统筹地区，占住院医保基金支出的 80% 以上。很多医院的收入只能勉强覆盖支出
* **创新药出海**：2026 年上半年，中国创新药对外授权交易总额约 1,000 亿到 1,100 亿美元，创纪录，已达 2025 年全年的约 80%；全球前十大对外授权交易里有 8 笔来自中国公司

---

## 3. 主要玩家

| 类别 | 全球 | 美国 | 中国 |
| :--- | :--- | :--- | :--- |
| 药企 | 诺和诺德、罗氏、阿斯利康、诺华 | 礼来、强生、默沙东、辉瑞、艾伯维 | 恒瑞、百济神州、石药 |
| 保险 | | UnitedHealth、Elevance、Cigna、Aetna、Humana | 国家医保为主，商业保险为补充 |
| 医院 | | HCA、凯撒医疗、各大学医疗中心 | 公立三甲医院 |
| 器械 | 西门子医疗、飞利浦 | 美敦力、雅培、直觉外科、GE 医疗 | 迈瑞、联影 |
| 医疗信息与 AI | | Epic、Oracle Health；AI 公司 OpenEvidence（估值 120 亿美元）、Abridge（约 53 亿美元）、Hippocratic AI（35 亿美元） | |

---

## 4. 历史上的几次大变革

| 时间 | 发生了什么 | 赢家 | 输家 |
| :--- | :--- | :--- | :--- |
| 1965 | 美国建立 Medicare 和 Medicaid | 老人和低收入人群；政府成了最大的付款方 | |
| 1983 | Medicare 改为按诊断分组付费（DRG），按病种给医院固定金额 | 控制成本的医院 | 住院天数长、效率低的医院。中国今天推行的 DRG 正是借鉴了这一模式 |
| 1990 年代 | 管理式医疗（HMO）兴起，保险公司开始控制医生能做什么 | 保险公司 | 医生的自主权；后来引发了公众反弹 |
| 2003 | Medicare 开始覆盖处方药 | PBM 迅速壮大 | |
| 2009 | 美国政府拿出数百亿美元补贴医院采用电子病历 | **Epic**，借此在美国医院里接近垄断 | 医生：文书负担大增，成为今天职业倦怠的主要原因之一 |
| 2010 | 《平价医疗法案》（ACA），建立保险交易所，扩大 Medicaid | 新增的数千万参保人；大型保险公司借机纵向整合 | |
| 2018 | 中国成立国家医保局，推行集采 | 患者，药价大幅下降 | 仿制药企业 |
| 2020 | 新冠疫情 | 远程医疗、mRNA 疫苗企业 | |
| 2023 到 2026 | GLP 1 减重药爆发 | 礼来、诺和诺德 | 部分食品和零售企业（见世界产业地图） |
| 2025 到 2026 | 美国医保政策大调整（见第 5 节） | 待定 | 失去保险的人群，农村医院 |

**从历史里能学到的三点**：
1. **支付规则决定行为。** 按项目付费，医院就多做项目；按病种付费，医院就控制成本；补贴电子病历，所有医院就都装了电子病历
2. **谁控制了"决策点"，谁就能拿走价值。** 保险公司靠预授权，PBM 靠决定哪些药能报销，Epic 靠控制医生每天使用的系统
3. **监管会制造赢家。** Epic 的地位很大程度上来自 2009 年的补贴政策。这对创业者是一个提醒：在医疗里，读懂政策往往比读懂技术更重要

---

## 5. 2026 年正在发生的变化

### 5.1 美国：参保人群在缩小

* **ACA 增强补贴在 2025 年底到期**：2026 年开放注册的人数为 2,310 万，比 2025 年少 4.9%；但 KFF 预计实际缴费的人数会下降约 21.5%，降到 1,750 万左右。平均每位参保人的保费翻了一倍多；约 9% 的去年参保人已经完全没有保险
* **Medicaid 削减**：《大而美法案》规定从 2027 年 1 月起实行工作要求，2026 年底起每半年重新审核一次资格。一家咨询公司估计将有 780 万人失去 Medicaid；CBO 估计到 2034 年未参保人数将增加约 1,000 万
* **对医院的影响**：坏账和慈善医疗在增加；有 432 家农村医院面临关闭风险；法案也设立了 500 亿美元的农村医疗转型基金

### 5.2 AI 进入核心工作流

* 29% 的美国医生在用 AI 语音写病历
* Epic 在 2026 年 3 月推出三个 AI Agent：Art 负责写病历和临床支持，Penny 负责计费、预授权和申诉，Emmie 负责回答患者问题和预约。Epic 说 85% 以上的客户已经在用它的 AI 工具（这些数字多来自 Epic 及其合作方）
* FDA 1 月放宽了对临床决策支持软件的监管；已授权的 AI 医疗器械超过 1,600 个
* 医疗 AI 公司估值很高：OpenEvidence 120 亿美元，Abridge 约 53 亿美元

### 5.3 预授权变成"AI 对 AI"

* 2026 年 1 月起，CMS 在亚利桑那、新泽西、俄亥俄、俄克拉何马、德克萨斯、华盛顿六个州，对传统 Medicare 的 15 类服务试行由私营科技公司用 AI 做预授权审核（WISeR 模型），而这些公司可以**从被拒绝的服务节省下来的钱里分成**。这引发了很大争议
* 讽刺的是，CMS 宣布这个模型，是在各大保险公司公开承诺减少预授权的四天之后（2025 年 6 月）
* 与此同时，医院一方在用 Epic 的 Penny 等工具自动写申诉。一边用 AI 拒，一边用 AI 申诉

### 5.4 药价政治

* **GLP 1 最惠国价格协议**（2025 年 11 月）：礼来和诺和诺德同意，Medicare 和 Medicaid 支付的价格降到每月 245 美元，Medicare 患者每月自付 50 美元，Medicare 首次覆盖肥胖症用药
* **TrumpRx**：政府推出的药品直购网站，减重药现金价格每月约 149 到 350 美元
* **PBM 改革**：2026 年 2 月签署的法律要求 PBM 把回扣全部转给客户，禁止在 Medicare 处方药计划里赚差价，并把 PBM 的收费和药品标价脱钩；联邦贸易委员会先后和 Express Scripts、CVS Caremark 达成和解，Optum Rx 也在转向按服务收费

### 5.5 保险公司在收缩

* UnitedHealth 2026 年主动退出不赚钱的 Medicare Advantage 计划，预计会员减少约 110 万
* 商业保险的医疗成本增速超过 11%

### 5.6 人手不够

* 美国卫生资源和服务管理局（HRSA）预计，到 2038 年医生缺口约 14.1 万人，非城市地区缺口高达 58%
* 注册护士缺口约 10.9 万人；但执业护士（Nurse Practitioner）反而会过剩约 7.3 万人，可以部分弥补基层医生的不足

### 5.7 中国

* 创新药对外授权创纪录，中国正在成为全球新药研发的重要来源
* DRG/DIP 全面铺开，集采继续，医院的成本压力很大
* 全球首个商用脑机接口获批，脑机接口有了医保收费项目
* 司美格鲁肽专利到期，国产仿制药即将上市

---

## 6. 一线从业者最常抱怨的问题

以下根据报道整理，不是直接访谈。

| 谁 | 最头疼的事 |
| :--- | :--- |
| 医生 | 写病历占用大量时间，被预授权卡住，职业倦怠 |
| 医院财务部门 | 拒付和申诉；没有保险的病人越来越多，坏账上升；利润率只有约 2% |
| 保险公司 | 医疗使用量和成本持续上涨，减重药的费用压力 |
| 患者 | ACA 参保人的保费翻倍，平均起付额创纪录（约 3,786 美元），账单看不懂，约不上医生 |
| 药企 | 药价被压，被 PBM 这样的中间商分走利润 |
| 中国医院 | 按病种付费的预算压力，集采降价，医生工作量大 |

---

## 7. 机会

### 7.1 第一类：风口

| 机会 | 为什么现在 | 退潮信号 |
| :--- | :--- | :--- |
| 专科 AI 病历：口腔、心理咨询、康复理疗、兽医等 Epic 覆盖不到的小诊所 | 大医院已被 Epic 和大公司占领，小专科还没有 | 通用 AI 病历工具降价进入 |
| 小诊所的拒付申诉和预授权代办，按追回的金额分成 | 拒付率上升，AI 写申诉已经可行 | 理赔规则改革，或者大平台免费提供 |
| 帮医院找回"失去保险"的病人的保险资格（资格筛查、重新参保、慈善医疗申请） | ACA 和 Medicaid 变化导致坏账上升 | 政策再次调整 |
| 减重药伴随服务 | Medicare 开始覆盖，TrumpRx 降价 | 大平台推出同类服务 |
| 现金支付患者的药价和服务比价 | 现金价格越来越多，越来越透明 | 政府网站和保险公司自己做好了 |

### 7.2 第二类：可能长出垄断的方向

**1. 机器对机器的理赔基础设施**
* **秘密**：预授权和理赔正在从"人对人"变成"Agent 对 Agent"。医院这边有 Epic 的 Penny，保险和政府那边有 AI 审核公司。当双方都是机器时，需要一个中立的协议、一套可审计的记录，以及一个大家都认可的"规则引擎"。谁成为这一层的标准，谁就站在了每年数万亿美元资金流动的中间
* **垄断从哪来**：双边网络效应（医院和保险公司都接入）、标准地位、监管认可
* **参照**：现在的理赔清算所（例如 Change Healthcare、Availity）已经是这样的中间层。2024 年 Change Healthcare 遭到勒索软件攻击，全美大量理赔停摆，说明这一层有多关键
* **适合你吗**：适合。核心是软件、Agent 和安全，正好对应你的背景，也和"两类机会"里的方向 4（Agent 信任层）、方向 2（可验证的 AI）重叠
* **会错的情况**：Epic 或大保险公司直接定标准；监管推动的是另一套方案

**2. 可审计的医疗 AI 决策**
* WISeR 引发的争议，核心是"AI 拒绝了你，但没人能说清为什么"。监管机构、医院、患者都需要能被检查和复现的 AI 决策记录。这是方向 2 在医疗里的具体落点

**3. AI 增强的基层医疗**
* **秘密**：非城市地区医生缺口高达 58%，但执业护士会过剩。"执业护士加 AI"的诊所，可能用更低的成本把基层医疗带到缺医生的地方
* **门槛**：各州对执业护士的执业范围规定不同，需要医疗运营经验和资本，不适合作为第一个项目，但值得关注

**4. 面向失去保险人群的低价医疗**
* 几百万人正在失去保险，他们仍然需要看病。把 AI 分诊、远程医疗、TrumpRx 的低价药和现金价格的检查打包，可能形成一个新的消费品牌
* 风险在于政策变化很快，需求可能随着下一次政策调整而变化

**5. 居家照护和远程监测**
* 结合人口老龄化、非处方 CGM、非侵入式脑机接口康复（见两类机会文档的方向 6）。适合你的 ECE 背景

**6. 临床试验加速**
* 药企在临床试验上花钱最多，招募患者慢是普遍问题。中国药企在临床推进速度上的优势，是它们能大量对外授权的原因之一。用 AI 做患者匹配、试验运营，是药企愿意付高价的领域

---

## 8. 接下来值得关注的信号

* UnitedHealth 等保险公司的三季度财报（10 月中旬起）
* 11 月开始的 2027 年 ACA 开放注册：保费和参保人数
* 2027 年 1 月 Medicaid 工作要求正式实施
* KFF 等机构对 WISeR 模型的评估
* PBM 改革的落地细节
* 中国的医保目录调整和创新药授权交易
* Epic 的 AI Agent 实际被采用的程度

**适合长期跟踪的信息源**：KFF（美国医疗政策最权威的非营利研究机构）、Health Affairs、STAT News、Fierce Healthcare、Healthcare Dive；药品渠道方面可以看 Drug Channels。

---

## 参考来源

* [National health care spending increased 7.2% in 2024 (Health Affairs)](https://www.healthaffairs.org/doi/10.1377/hlthaff.2025.01683)
* [US health spending reached $5.3T in 2024 (Healthcare Dive)](https://www.healthcaredive.com/news/us-healthcare-spending-2024-cms-health-affairs/809578/)
* [National Health Expenditure Projections 2025 to 2034 (CMS)](https://www.cms.gov/files/document/national-health-expenditure-projections-results-presentation.pdf)
* [Six trends reshaping US drug spending (Drug Channels)](https://www.drugchannels.net/2026/02/latest-cms-data-reveal-six-trends.html)
* [Administrative expenses in the US health care system (JAMA)](https://jamanetwork.com/journals/jama/fullarticle/2785479)
* [Administrative simplification and the potential for saving a quarter trillion dollars (JAMA)](https://jamanetwork.com/journals/jama/fullarticle/2785480)
* [Medical billing denial statistics 2026](https://www.gomedicalbilling.com/medical-billing-denial-statistics-2026)
* [Kaufman Hall National Hospital Flash Report, April 2026 metrics](https://www.kaufmanhall.com/sites/default/files/2026-06/KH-NHFR_Report-April-2026-Metrics.pdf)
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
