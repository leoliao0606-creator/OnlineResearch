# 产业深挖一：能源与电力

写于 2026年10月12日 · 世界产业地图系列 · 上一篇：[世界产业地图（全景）](../world_industry_map.md)

---

## 0. 一句话看懂这个产业

能源产业做的事情，是把自然界的能量（石油、天然气、煤、铀、阳光、风、地热）变成人能用的形式，并在**正确的时间**送到**正确的地方**。

其中最难的是电力。电几乎不能大量储存，**发电和用电必须在每一秒都保持平衡**，否则电网（power grid）就会崩溃。理解了这一点，你就能理解这个产业里大部分的规则、价格和矛盾。

---

## 1. 产业链（industry value chain）

### 1.1 电力

| 环节 | 做什么 | 代表公司 | 怎么赚钱 |
| :--- | :--- | :--- | :--- |
| 燃料与资源 | 提供天然气、煤、铀；阳光和风本身免费 | 油气公司、煤矿、铀矿 | 卖燃料 |
| 发电设备 | 造燃气轮机（gas turbine）、光伏（solar PV）组件、风机、电池、逆变器（inverter）、变压器（transformer） | 燃气轮机：GE Vernova、西门子能源、三菱重工；光伏：隆基、晶科、天合；电池：宁德时代、比亚迪；逆变器：阳光电源、华为、Enphase | 卖设备 |
| 发电 | 运营电厂，把能量变成电 | 美国：NextEra、Vistra、Constellation；中国：五大发电集团、三峡集团 | 卖电，或者从受监管的投资中获得回报 |
| 输电（transmission） | 用高压线把电从电厂送到城市 | 中国：国家电网（State Grid）、南方电网（China Southern Power Grid）；美国：几百家电力公司（utility）各管一段，由区域电网运营机构（如 PJM、ERCOT）统一调度 | 受监管的投资回报（return on investment, ROI） |
| 配电（distribution） | 把电从变电站送进千家万户 | 地方电力公司 | 受监管的投资回报 |
| 售电与用户 | 卖电给家庭、工厂、数据中心（data center） | 电力公司、售电公司 | 电费 |
| 灵活性 | 在用电高峰和低谷之间"搬运"电，平衡电网 | 储能（energy storage）电站、虚拟电厂（virtual power plant, VPP）、需求响应（demand response）公司 | 峰谷价差、容量费（capacity payment）、辅助服务费 |

### 1.2 油气

| 环节 | 做什么 | 代表公司 |
| :--- | :--- | :--- |
| 上游 | 勘探和开采石油、天然气 | 沙特阿美、埃克森美孚、雪佛龙、壳牌、道达尔、BP；中石油、中海油 |
| 中游 | 管道、液化天然气（LNG）工厂、油轮和 LNG 船 | 管道公司、卡塔尔能源、美国 LNG 出口商 |
| 下游 | 炼油、化工、加油站 | 中石化、各大炼油厂 |

油价很大程度上由 **OPEC+**（以沙特和俄罗斯为首的产油国联盟）的产量决定，所以油气产业受地缘政治的影响非常大。

---

## 2. 钱怎么流

### 2.1 电力的三种赚钱模式

**模式一：受监管的电网公司，按"投资额"拿回报**

美国大多数电力公司和中国的电网公司，属于"自然垄断（monopoly）"：一个地区只需要一张电网，所以政府允许它垄断，但要管它的价格。

在美国，州政府的监管机构会批准电力公司在投资上获得一个回报率（股本回报率（return on equity, ROE）一般在 9% 到 10% 左右）。这带来一个有意思的激励：**电力公司投资越多，能赚的钱就越多**，所以它们喜欢建新的线路和变电站，而这些成本最终都会进入居民的电费。

这就是今天美国的一个核心矛盾：
* 美国居民电价 2026 年约 18.3 美分每千瓦时，比一年前高约 5%，比 2020 年高约 37%
* 2025 年电力公司提交的涨价申请（rate case）创下纪录
* 标普的判断是，"可负担性（affordability）"已经从背景问题变成了限制电力公司赚钱的硬约束

**模式二：市场化的发电商，在批发市场（wholesale market）里卖电**

在美国的很多地区，发电厂在一个批发市场里竞价卖电。除了卖电量，还有一种很重要的收入叫"**容量费**"：电网运营机构提前几年拍卖，付钱给电厂，让它们保证在需要的时候能发电。

美国最大的电网区域 PJM（覆盖华盛顿、费城、芝加哥等 13 个州）的容量拍卖（capacity auction），是看懂这个产业的一个窗口：
* 2025 年 12 月针对 2027 到 2028 年的拍卖，价格直接撞到上限（每兆瓦每天 333 美元），总成本 164 亿美元，创纪录，连续第三次触顶
* 即便如此，仍比可靠性要求少了约 6.5 GW
* 市场监督机构估计，其中约 63 亿到 65 亿美元是数据中心带来的
* 一份 NRDC 的预测是，按这个趋势，到 2028 年普通家庭每月电费可能多出约 70 美元

**模式三：卖设备和工程**

现在是卖方市场。最典型的是燃气轮机和变压器：
* GE Vernova 的燃气轮机积压订单（backlog）加预留产能，2026 年二季度达到 116 GW，年底预计至少 125 GW；而它每年只能造约 20 GW，重型燃气轮机的交货基本排满到 2028 年
* 大型变压器的交期（lead time）最长要 4 年；发电厂用的升压变压器交期超过 160 周

**中国的情况**：中国过去是电网"统购统销"，电价由政府定。现在正在推进市场化：2025 年 6 月 1 日起，新的风电和光伏项目从固定电价转向市场定价；到 2026 年 9 月，已有 11 个省级电力现货市场（spot market）正式运行；目标是 2030 年基本建成全国统一电力市场。

### 2.2 油气：价格决定一切

油气公司的利润主要取决于油价，而油价主要取决于地缘政治和 OPEC+。2026 年是一个极端的例子：
* 2 月底伊朗战争爆发，霍尔木兹海峡（Strait of Hormuz）关闭，布伦特原油 3 月底一度到 118 美元左右
* 8 月底，因为重新开放的希望，一度跌到 86 美元左右
* 到 9 月，各机构对四季度油价的预测从 77 美元到 105 美元不等

天然气受的冲击更大。全球约 20% 的 LNG 要经过霍尔木兹海峡，卡塔尔的主要 LNG 设施在 3 月遭到无人机袭击停产，亚洲 LNG 价格在两天内翻倍。

### 2.3 利润现在在哪里

* **赚钱的**：手握积压订单的设备商（GE Vernova），拥有稀缺电源的发电商（尤其是核电），以及创纪录投资的电网公司。国家电网 2026 到 2030 年计划投资 4 万亿元人民币，比上一个五年多约 40%；美国电力公司 2025 到 2029 年计划投资约 1.1 万亿美元
* **不赚钱的**：中国光伏制造商。产能严重过剩，龙头企业已经连续约 10 个季度亏损，多晶硅库存超过 54 万吨。这是"完全竞争（perfect competition）"的教科书案例：产品越来越便宜、越来越普及，但造它的公司赚不到钱

---

## 3. 主要玩家

| 类别 | 全球 | 美国 | 中国 |
| :--- | :--- | :--- | :--- |
| 油气 | 沙特阿美、壳牌、道达尔、BP | 埃克森美孚、雪佛龙 | 中石油、中石化、中海油 |
| 电网 | 意大利国家电力、伊维尔德罗拉、法国电力 | 几百家电力公司，较大的有 NextEra、Duke、Southern | 国家电网（全球最大的电力公司）、南方电网 |
| 发电 | | NextEra、Vistra、Constellation（核电最多） | 华能、大唐、华电、国家电投、国家能源集团、三峡集团 |
| 燃气轮机 | 西门子能源、三菱重工 | GE Vernova | 东方电气、上海电气 |
| 光伏 | | First Solar（美国本土） | 隆基、晶科、天合、晶澳、通威 |
| 电池 | LG 新能源、三星 SDI | 特斯拉（储能） | 宁德时代、比亚迪 |
| 新一代电源 | | Fervo（增强型地热（enhanced geothermal））、Commonwealth Fusion Systems（核聚变（nuclear fusion），就在马萨诸塞州）、Oklo、Kairos、X energy（小型核反应堆（small modular reactor, SMR）） | 中核、中广核 |

---

## 4. 历史上的几次大变革

| 时间 | 发生了什么 | 赢家 | 输家 |
| :--- | :--- | :--- | :--- |
| 1973 和 1979 | 两次石油危机，OPEC 拿到定价权 | 产油国；法国借机大建核电，至今约七成电力来自核能 | 石油进口国 |
| 1990 年代 | 很多国家把发电和电网拆开，建立电力批发市场 | 高效的发电商 | 2000 到 2001 年加州电力危机，2001 年安然破产，说明市场设计出错代价很大 |
| 2008 到 2015 | 美国页岩革命：水平钻井加压裂，让美国成为全球最大的油气生产国 | 美国消费者，天然气变便宜 | 煤电；很多页岩公司自己也在油价下跌时破产，产量很大，回报却很差 |
| 2010 年代 | 光伏和电池成本暴跌，中国主导制造 | 用电的人；中国在产量上全面领先 | 欧美光伏制造业；中国厂商自己也陷入价格战（price war） |
| 2011 | 福岛核事故 | 天然气和可再生能源 | 核电，德国决定全面退出核电 |
| 2022 | 俄乌战争，欧洲天然气危机 | LNG 出口国，尤其是美国和卡塔尔 | 依赖俄罗斯天然气的欧洲工业 |
| 2024 到 2026 | AI 用电暴增，加上 2026 年伊朗战争 | 设备商、核电、电网公司 | 电费上涨的居民；依赖霍尔木兹海峡的进口国 |

**从历史里能学到的三点**：
1. **技术降本会让产品普及，但不一定让制造商赚钱。** 页岩油和光伏都是如此。用 Thiel 的话说，它们创造了巨大的价值，但没能留住价值
2. **每次能源危机都会重塑政策。** 战略储备、核电、LNG 基础设施，都是危机之后建起来的
3. **市场规则决定谁赚钱。** 安然和加州危机、PJM 的容量拍卖，都说明规则设计本身就是一门大生意

---

## 5. 现在正在发生的变化

### 5.1 需求重新开始增长

在过去十几年里，发达国家的用电量基本是平的。现在变了：
* 全球用电 2025 年增长 3%，IEA 预计 2026 到 2030 年每年增长 3.6%
* 美国用电 2026 年预计创下 42,880 亿千瓦时的新纪录，大约一半的增长来自数据中心
* 全球数据中心用电从 2025 年的 485 太瓦时，预计到 2030 年翻倍到 950 太瓦时；2025 年 AI 数据中心的用电增长了 50%
* 除了数据中心，电动车、空调、工业电气化也在推高用电

### 5.2 拿不到电：并网排队（interconnection queue）

新电厂要接入电网，得先排队等电网公司做研究、批准、升级线路。美国劳伦斯伯克利国家实验室的数据：
* 到 2025 年底，排队中的发电和储能项目约 **2,061 GW**，比美国现有的全部装机容量还多
* 2025 年建成的项目，从申请到投运的中位时间**超过 5 年**
* 2000 到 2020 年申请的项目，只有 **13%** 最终建成，75% 退出了
* 2025 年新申请里，天然气项目增加了 86%，光伏、风电、储能都在减少

### 5.3 设备和人都不够

* 燃气轮机交货基本排满到 2028 年，大型变压器最长要等 4 年
* 美国每年需要约 8.1 万名新电工；59% 的电力公司说招不到线路工人
* 电气工程占数据中心建设成本的 45% 到 70%；微软总裁说电工短缺是美国数据中心扩张的头号难题

### 5.4 美国政策在剧烈调整

* **税收抵免（tax credit）削减**：2025 年 7 月通过的《大而美法案》规定，2026 年 7 月 4 日之后才开工的风电和光伏项目，必须在 2027 年底前投运，否则拿不到联邦税收抵免
* **逆变器禁令**：7 月 FCC 禁止外国制造的联网逆变器新型号进入，要求美国本土含量（domestic content）至少 65%（详见 [personal_fit.md](../personal_fit.md)）
* **大型负荷（load）接入**：能源部要求 FERC 制定数据中心等大型负荷接入电网的规则。FERC 6 月向六个区域电网运营机构发出命令，要求修改或解释现行规则，但正式规则还没出台

### 5.5 中国：从拼装机量到拼市场

* 2025 年中国新增光伏创纪录，约 315 GW；但 2026 年上半年只有 72 GW，同比下降 66%，原因是新项目改为市场定价，收益不再确定
* 政府在推动"反内卷（anti involution）"，希望减产提价，但到 9 月多晶硅价格仍然疲软
* 国家电网的投资创纪录，2026 到 2030 年计划新建 15 条特高压（ultra high voltage, UHV）线路
* 电力现货市场在各省铺开

### 5.6 新技术开始兑现

| 技术 | 2026 年进展 |
| :--- | :--- |
| 储能 | 2025 年电池包均价跌到 108 美元每千瓦时；储能用电池跌了 45%，到 70 美元，首次成为最便宜的细分 |
| 虚拟电厂 | 美国已登记约 38 到 40 GW；能源部的目标是 2030 年达到 80 到 160 GW；9 月 9 日，加州 14 万户家用电池在一个晚上一起向电网送出了 580 MW |
| 增强型地热 | Fervo 在犹他州的 Cape Station 于 9 月 24 日首次发电，是全球第一个实现发电的商业规模增强型地热电站；和 Google 签了 396 MW 的购电协议（power purchase agreement, PPA）；5 月在纳斯达克上市 |
| 核聚变 | 马萨诸塞州的 Commonwealth Fusion Systems，SPARC 装置约八成完工，首次等离子体从 2026 年推迟到 2027 年 |
| 核电重启 | 密歇根州的 Palisades 核电站重启一再推迟，到 10 月仍未完成 |
| 固态变压器（solid state transformer） | Heron Power 2 月融资 1.4 亿美元，DG Matrix 融资 6,000 万美元，Amperesand 融资 8,000 万美元 |
| 柔性数据中心 | Emerald AI 的试点在用电高峰时让数据中心降低 25% 用电，估值（valuation） 10.5 亿美元 |

---

## 6. 一线从业者最常抱怨的问题

以下是根据行业报道整理的，不是我直接访谈得来的。如果你要验证某个方向，最好的办法是直接去问这些人。

| 谁 | 最头疼的事 |
| :--- | :--- |
| 电站开发商 | 并网（interconnection）要等五年以上，而且不知道最后要花多少钱升级电网；四分之三的项目最后放弃 |
| 电力公司 | 负荷预测失灵：同一个数据中心项目会同时向好几家电力公司申请，真假难辨；设备买不到；招不到人；监管机构不愿意批准涨价 |
| 数据中心开发商 | "什么时候能通电"已经成为选址的第一标准；电工短缺 |
| 居民和小企业 | 电费持续上涨，账单看不懂 |
| 中国光伏制造商 | 产能过剩（overcapacity），连续亏损 |
| 政策制定者 | 可靠、便宜、低碳三个目标很难同时满足 |

---

## 7. 机会

### 7.1 第一类：风口（hot trend），快进快出

| 机会 | 为什么现在 | 退潮信号 |
| :--- | :--- | :--- |
| 帮数据中心找电：选址、"什么时候能通电"的数据服务和咨询 | 通电时间成了选址第一标准 | 大电网运营机构公开透明的接入数据，或者负荷增长放缓 |
| 并网申请的文件准备和流程代办 | 2,000 多 GW 在排队，流程复杂 | 并网改革简化了流程 |
| 电工和电网技工的培训、招聘平台 | 严重短缺，薪资上涨 | 数据中心建设降温 |
| 中小企业电费分析、需求响应报名 | 电价持续上涨 | 电力公司自己提供类似工具 |
| 长交期设备的二手和翻新撮合 | 变压器等要等好几年 | 产能追上需求 |
| 阳台光伏、家用储能的销售和安装 | 各州相继立法，电价上涨 | 价格战，大品牌进入 |

### 7.2 第二类：可能长出垄断的方向

**1. 用 AI 加速并网研究**
* **秘密**：并网排队慢，一个重要原因是电网公司要为每个项目做复杂的电力系统仿真（潮流计算（power flow analysis）、稳定性分析），人手不够，一做就是几个月到几年。如果能用 AI 和高性能仿真把它缩短到几天，并且结果被监管机构和电网公司接受，这个工具就会成为行业基础设施
* **垄断从哪来**：被监管接受后的标准地位，加上越积越多的电网模型数据
* **适合你吗**：很适合。需要电力系统知识（ECE）加机器学习
* **会错的情况**：电网公司不愿意把关键研究交给外部工具；数据拿不到

**2. 柔性负荷调度**
* 两类机会文档里的方向 7。美国已经有 Emerald AI，可以考虑更小的切口：中小型数据中心、边缘算力（compute）、工业用户

**3. 电力电子（power electronics）：固态变压器和美国本土逆变器**
* 固态变压器用半导体替代传统的铁芯和线圈，体积更小、可控性更好，而且能绕开传统变压器的供应链（supply chain）瓶颈。已有几家公司拿到大额融资，可以找它们没覆盖的细分场景，比如电动车车队充电站、校园微电网、插电式光伏
* 美国本土逆变器的机会，见 [personal_fit.md](../personal_fit.md) 里的"新 A"

**4. 家庭能源的"操作系统"**
* **秘密**：家里的电池、电动车、热泵、阳台光伏，正在变成一个个小电厂。谁能把它们聚合起来调度，谁就站在了家庭和电网之间，形成双边网络效应（two sided network effects）
* **竞争**：特斯拉、Base Power 等已经在做。可以从租房者和多户住宅这些被忽略的人群切入

**5. 电网资产的数据层**
* 美国很多变压器和线路已经用了几十年，故障预测、寿命评估、"电网数字孪生"都有需求。谁积累了最多的设备运行数据，谁的预测就最准

**6. 下一代稳定电源（增强型地热、核聚变、小型核反应堆）**
* 这些是十年以上的硬科技，需要巨额资本，学生创业很难。更现实的路径是去这类公司实习或工作。Commonwealth Fusion Systems 就在马萨诸塞州的 Devens，离你不远

---

## 8. 接下来值得关注的信号

* PJM 下一次容量拍卖的结果，以及电价的政治反弹
* FERC 关于大型负荷接入的正式规则
* 霍尔木兹海峡能否完全重新开放
* GE Vernova 的积压订单是否继续增长
* 中国多晶硅是否真的减产，光伏装机能否回暖
* 马萨诸塞州的插电式光伏法案能否通过
* Commonwealth Fusion Systems 2027 年的首次等离子体

**适合长期跟踪的信息源**：IEA 的年度电力报告、劳伦斯伯克利国家实验室的 Queued Up 报告，以及 Utility Dive、Canary Media、Latitude Media 这几个行业媒体。

---

## 参考来源

* [IEA Electricity 2026: Executive summary](https://www.iea.org/reports/electricity-2026/executive-summary)
* [IEA Key Questions on Energy and AI](https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary)
* [US power use expected to reach record highs in 2026, 2027 (Carrier Management, citing EIA)](https://carriermanagement.com/news/2026/10/07/292552.htm)
* [US data center power demand projected to double by 2027 (Goldman Sachs)](https://www.goldmansachs.com/insights/articles/us-data-center-power-demand-projected-to-double-by-2027)
* [Queued Up: 2026 Edition (Lawrence Berkeley National Laboratory)](https://emp.lbl.gov/publications/queued-2026-edition-characteristics)
* [GE Vernova gas turbine backlog climbs to 116 GW (Utility Dive)](https://www.utilitydive.com/news/ge-vernova-gas-turbine-backlog-climbs-to-116-gw/826039/)
* [US transformer lead times extend to four years (pv magazine USA)](https://pv-magazine-usa.com/2026/05/11/u-s-transformer-market-faces-severe-supply-constraints-as-lead-times-extend-to-four-years/)
* [PJM 2027/2028 Base Residual Auction Report](https://www.pjm.com/-/media/DotCom/markets-ops/rpm/rpm-auction-info/2027-2028/2027-2028-bra-report.pdf)
* [PJM capacity prices hit price cap, reserve shortfall grows (Utility Dive)](https://www.utilitydive.com/news/pjm-capacity-auction-price-cap-reserve-shortfall/825282/)
* [PJM's capacity costs hit record (Canary Media)](https://www.canarymedia.com/articles/data-centers/pjm-record-capacity-costs-rising-bills)
* [Electricity rates by state, October 2026 (ElectricChoice)](https://www.electricchoice.com/electricity-prices-by-state/)
* [Record utility rate requests in 2025 amid affordability concerns (S&P Global)](https://www.spglobal.com/market-intelligence/en/news-insights/research/2026/01/record-amount-of-utility-rate-requests-in-2025-amid-affordability-concerns)
* [Impact of the One Big Beautiful Bill on clean energy tax credits (Chapman and Cutler)](https://www.chapman.com/publication-impact-of-one-big-beautiful-bill-on-clean-energy-tax-credits)
* [FERC orders grid operators to revise or justify large load rules (White & Case)](https://www.whitecase.com/insight-alert/ferc-orders-grid-operators-promptly-revise-or-justify-interconnection-rules-data)
* [CPIA: China's H1 2026 solar installations drop 66% (TaiyangNews)](https://taiyangnews.info/markets/cpia-china-h1-2026-solar-pv-istallations-drop-66-percent-yoy)
* [China's anti involution campaign falters (BigGo Finance)](https://finance.biggo.com/news/zFh_-p0B2jrwCtglfL2F)
* [RMI 2026 China Power Market Outlook](https://rmi.org/app/uploads/dlm_uploads/2026/07/rmi-2026-July-2026-China-Power-Market-Outlook-1.pdf)
* [State Grid's record investment plan (Yicai Global)](https://www.yicaiglobal.com/news/chinas-state-grid-to-invest-record-usd5739-billion-over-next-five-years)
* [Lithium ion battery pack prices fall to $108 per kWh (BloombergNEF)](https://about.bnef.com/insights/clean-transport/lithium-ion-battery-pack-prices-fall-to-108-per-kilowatt-hour-despite-rising-metal-prices-bloombergnef/)
* [IEA Gas Market Report, Q3 2026](https://iea.blob.core.windows.net/assets/72079a0a-ec1e-48a1-b8e9-3042160b9378/GasMarketReport,Q3-2026.pdf)
* [International LNG prices rise amid Strait of Hormuz closure (EIA)](https://www.eia.gov/todayinenergy/detail.php?id=67604)
* [Oil price forecasts jump as Hormuz disruption drags on (OilPrice.com)](https://oilprice.com/Energy/Oil-Prices/Oil-Price-Forecasts-Jump-as-Hormuz-Disruption-Drags-On.html)
* [In 2026, virtual power plants must scale (Utility Dive)](https://www.utilitydive.com/news/in-2026-virtual-power-plants-must-scale-or-risk-being-left-behind/810321/)
* [Fervo Energy achieves first power at Cape Station](https://fervoenergy.com/fervo-energy-achieves-first-power-at-cape-station-a-landmark-moment-for-the-future-of-enhanced-geothermal-systems/)
* [Commonwealth Fusion Systems (Wikipedia)](https://en.wikipedia.org/wiki/Commonwealth_Fusion_Systems)
* [Palisades restart status (ANS Nuclear Newswire)](https://www.ans.org/news/2026-07-08/article-8187/palisades-restart-projects-holtec-ipo-lawsuit-dismissal-but-no-restart-date/)
* [Heron Power raises $140M to modernize transformers (Canary Media)](https://www.canarymedia.com/articles/climatetech-finance/heron-power-raises-140m-electrical-transformers)
* [Hyperscale Power challenges transformer tech (TechCrunch)](https://techcrunch.com/2026/03/10/hyperscale-power-is-the-latest-startup-to-challenge-140-year-old-transformer-tech/)
* [Data center rush worsens shortages of grid workers (EnergyNow)](https://energynow.com/2026/05/data-center-rush-worsens-shortages-of-power-grid-workers/)
* [Emerald AI and Nvidia fast pass for grid connections (Fortune)](https://fortune.com/2026/03/31/emerald-ai-nvidia-fast-pass-data-center-grid-connects/)
