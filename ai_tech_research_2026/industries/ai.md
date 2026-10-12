# 产业深挖四：AI 产业

写于 2026年10月12日 · 世界产业地图系列 · 上一篇：[金融](finance.md)

这一篇讲的是 AI 作为一个**产业**的结构和经济学：谁投钱、谁赚钱、钱从哪里来。具体的技术进展（模型、Agent、语音、机器人等）见第一版的 [report.md](../report.md)。

**说明**：我（Claude）是 Anthropic 开发的，下文会写到 Anthropic。相关数据都来自公开报道，我尽量和其他公司用同样的标准对待。

---

## 0. 一句话看懂这个产业

AI 产业是一条从**电力**一直延伸到**应用**的长链条。2026 年的格局是：

* **上游（芯片）**赚得最多：NVIDIA 毛利率（gross margin） 75%
* **中游（大模型（large models）公司）**收入暴涨，但还在大额亏损
* **下游（应用）**用户增长很快，但利润被推理成本（inference cost）吃掉了一大块

整个产业最核心的问题只有一个：**下游最终能不能创造足够的价值，养活上游每年 7,000 多亿美元的投资？**

---

## 1. 产业链（industry value chain）

| 层 | 做什么 | 代表公司 | 2026 年赚钱情况 |
| :--- | :--- | :--- | :--- |
| 1. 电力与数据中心（data center）建设 | 供电、建机房、冷却 | 电力公司（utility）、GE Vernova、建筑商 | 大赚，供不应求（见[能源与电力](energy_power.md)） |
| 2. 芯片制造 | 光刻机（lithography machine）、晶圆代工（foundry）、存储芯片 | ASML（高端光刻机全球唯一供应商）、台积电、SK 海力士、三星、美光 | 大赚。全球存储芯片市场预计增长约 250% |
| 3. 芯片设计 | GPU 和专用 AI 芯片 | NVIDIA、AMD、博通（帮 Google 等设计定制芯片）；Google TPU、亚马逊 Trainium；中国：华为昇腾 | NVIDIA 最赚钱，毛利率 75% |
| 4. 云与算力（compute） | 出租算力 | 亚马逊 AWS、微软 Azure、Google Cloud、甲骨文；新兴算力云 CoreWeave 等 | 收入快速增长，但资本开支（capital expenditure, capex）巨大 |
| 5. 基础模型（foundation model） | 训练和提供大模型 | OpenAI、Anthropic、Google DeepMind、Meta、xAI；中国：DeepSeek、阿里通义、月之暗面、智谱、MiniMax、字节 | 收入暴涨，多数仍在亏损 |
| 6. 工具与基础设施 | Agent 平台、评测、监控、数据接入 | 各大模型公司的 Agent 平台、MCP 生态、大量创业公司 | 竞争激烈，容易被上下游挤压 |
| 7. 应用 | 面向用户的产品 | 编程：Cursor、Claude Code；医疗：OpenEvidence、Abridge；消费：ChatGPT、豆包 | 增长快，毛利率普遍不高 |

---

## 2. 钱怎么流

### 2.1 两个方向的钱

**投资的钱从下往上流**：四大云厂商（亚马逊、Google、微软、Meta）2026 年资本开支约 **7,300 亿美元**，比 2025 年多 78%，其中六成以上花在电力、冷却和建设上。这些钱最终流向 NVIDIA、台积电、存储芯片厂和电力设备商。

**收入的钱从上往下流**：用户和企业付钱给应用，应用付钱调用模型 API，模型公司付钱租算力，云厂商付钱买芯片。

### 2.2 每一层赚多少

| 层 | 2026 年的数字 |
| :--- | :--- |
| 芯片 | NVIDIA 截至 7 月底的季度收入 962 亿美元，同比增长 106%；其中数据中心 890 亿美元；毛利率 75%；下一季度预计 1,080 亿美元 |
| 模型公司 | Anthropic 7 月底的年化收入（annualized revenue）约 650 亿美元（2 月时约 140 亿美元），5 月融资后估值（valuation）约 9,650 亿美元，6 月秘密提交了上市申请；OpenAI 9 月底年化收入约 500 亿美元，目标年底超过 700 亿美元，但据报道 2026 年预计亏损约 140 亿美元，推理成本从 2025 年的 84 亿美元增长到约 141 亿美元。以上数字都来自媒体报道，不是审计数据 |
| 应用 | ICONIQ 的数据显示，AI 原生公司平均毛利率约 52%（传统软件通常在 70% 到 80%）；编程工具类更低，一项调查显示平均只有约 31%，推理成本吃掉了一半以上的收入。据报道，Cursor 2026 年 1 月的毛利率甚至是负的，后来靠自研模型和更便宜的第三方模型，企业客户部分在 4 月转正 |

### 2.3 一个好消息和一个坏消息

**好消息（对应用公司）**：同等能力的价格每年下降约 10 倍。H100 GPU 的租金从 2024 年初的每小时 7 美元以上，降到 2026 年的中位数约 3 美元。

**坏消息（对模型公司）**：价格降得这么快，模型公司必须不停地往前沿推，才能维持定价能力；而训练下一代模型的成本越来越高。

### 2.4 泡沫之争

* **看空的理由**：钱在少数几家公司之间循环。比如 NVIDIA 投资 OpenAI，OpenAI 再用这些钱买 NVIDIA 的芯片。据报道，NVIDIA 7 月曾考虑为 OpenAI 在俄亥俄州的数据中心提供 2,500 亿美元担保，消息传出后 NVIDIA 的债券违约保险价格大涨。有人估计这类"循环交易（circular deals）"超过 8,000 亿美元。摩根士丹利估计到 2028 年 AI 数据中心支出可能接近 3 万亿美元
* **看多的理由**：收入是真的，而且在加速。Anthropic 和 OpenAI 的年化收入加起来已超过 1,000 亿美元，NVIDIA 的收入一年翻倍
* **历史的参照**：2000 年前后的电信泡沫，公司铺了大量光纤，很多公司破产了，但这些光纤后来支撑了整个互联网时代。泡沫和真实的技术革命可以同时存在。对创业者来说，重要的不是判断有没有泡沫，而是**不要把公司建立在"融资环境会一直这么好"的假设上**

### 2.5 中国的情况

* **模型**：中国在开源（open source）模型上领先，DeepSeek V4、Kimi K3、GLM 5.2 都是开放权重（open weights）；价格便宜，豆包月活约 3.45 亿
* **芯片**：美国 1 月允许 H200 对华出口改为逐案审批，附带 25% 关税（tariff）和数量上限，约 10 家中国公司获批；但据报道中国海关随后拦截了 H200 入境。NVIDIA 在年报里承认，它实际上已经被挡在中国数据中心市场之外。华为昇腾 910C 今年计划生产约 60 万颗
* **结果**：中美 AI 产业正在形成两套几乎独立的体系，从芯片到模型再到应用

---

## 3. 主要玩家

| 层 | 美国 | 中国 | 其他 |
| :--- | :--- | :--- | :--- |
| 芯片制造 | 美光 | 中芯国际 | 台积电（台湾）、ASML（荷兰）、SK 海力士和三星（韩国） |
| 芯片设计 | NVIDIA、AMD、博通 | 华为海思、寒武纪 | |
| 云 | AWS、Azure、Google Cloud、甲骨文、CoreWeave | 阿里云、华为云、火山引擎、腾讯云 | |
| 模型 | OpenAI、Anthropic、Google、Meta、xAI | DeepSeek、阿里、月之暗面、智谱、MiniMax、字节 | Mistral（法国） |
| 应用 | Cursor、Perplexity、Harvey、OpenEvidence 等 | 豆包、元宝、千问、Kimi 等 | |

---

## 4. 历史上的几次大变革

| 时间 | 发生了什么 | 赢家 | 输家或教训 |
| :--- | :--- | :--- | :--- |
| 1956 | 达特茅斯会议，"人工智能"这个词诞生 | | |
| 1970 年代和 1980 年代末 | 两次"AI 寒冬"：承诺太多，算力和数据不够，资金撤离 | | 炒作过头的代价 |
| 2006 | NVIDIA 推出 CUDA，让 GPU 能用于通用计算 | **NVIDIA**。这个押注花了十几年才兑现，今天成了它最大的护城河（moat） | |
| 2012 | AlexNet 用 GPU 训练深度神经网络，深度学习时代开始 | Google（收购了 AlexNet 团队的公司）、NVIDIA | |
| 2017 | Google 发表 Transformer 论文 | 后来把它商业化得最成功的是 OpenAI | **发明者不一定是赢家** |
| 2020 | GPT 3 和"规模定律（scaling laws）"：模型越大越强 | 有钱买算力的公司 | 从此开始军备竞赛 |
| 2022 | ChatGPT 发布，成为史上增长最快的消费产品之一 | OpenAI、微软 | Google 一度被动 |
| 2025 年 1 月 | DeepSeek 发布便宜的开源推理模型 | 开源阵营、用户 | NVIDIA 单日市值（market cap）蒸发约 6,000 亿美元，市场第一次担心"AI 不需要那么多算力" |
| 2025 到 2026 | 编程 Agent 爆发，资本开支冲到 7,300 亿美元 | 芯片、电力、模型公司 | 待定 |

**从历史里能学到的四点**：
1. **基础设施的押注要很久才兑现。** CUDA 花了十几年
2. **发明者不一定是赢家。** Transformer 是 Google 发明的，但最先用它做出爆款产品的是 OpenAI。赢家往往是最会把技术变成产品、并且抢到分发渠道的公司
3. **炒作周期是真实存在的。** AI 已经经历过两次寒冬
4. **便宜的开源可以突然改变整个产业的定价。** DeepSeek 就是例子

---

## 5. 2026 年正在发生的变化

### 5.1 收入真的来了，但利润分布极不均衡
见第 2 节：芯片毛利率 75%，模型公司亏损，应用公司毛利率被推理成本压低。

### 5.2 企业落地仍然很难
* MIT 2025 年的研究：只有约 5% 的企业级 AI 试点进入生产环境
* 普华永道的 CEO 调查：56% 的公司表示 AI 既没有带来更多收入，也没有降低成本
* 毕马威 2026 年二季度：只有 7% 的企业领导者说已经看到明确的投资回报（return on investment, ROI）
* 麦肯锡：约 6% 的公司是"高绩效者"，能把 5% 以上的利润归功于 AI
* **这意味着**：技术已经够用了，瓶颈在于数据接入、流程改造、权限、安全和信任。这些"脏活"正是创业公司的机会

### 5.3 中美分化
芯片出口管制（export controls）反复，中国在开源模型上领先，两边的产业链越来越独立（见 2.5）。

### 5.4 电力成为瓶颈
数据中心"什么时候能通电"已经成为选址的第一标准，燃气轮机（gas turbine）和变压器（transformer）都排起了长队（见[能源与电力](energy_power.md)）。

### 5.5 监管
* **美国**：联邦层面统一 AI 规则的努力停滞；总统行政令（executive order）要求司法部挑战州的 AI 法律，但行政令本身不能取代州法。2025 年有 38 个州通过了 145 部 AI 相关法律；加州 SB 53 和德州的 TRAIGA 从 2026 年 1 月起生效；科罗拉多州的 AI 法案被大幅修改，推迟到 2027 年 1 月生效
* **欧盟**：AI 法案的透明度义务（transparency obligations） 2026 年 8 月生效，高风险义务推迟到 2027 年 12 月
* **中国**：AIGC 强制标识（mandatory labeling）

### 5.6 对就业的影响，尤其是新人
这一点和你直接相关。
* 斯坦福的研究发现，在受 AI 影响大的岗位（比如软件开发）上，22 到 25 岁年轻人的就业自 2022 年底以来相对下降了约 16%
* 纽约联储的数据：2026 年二季度，应届大学毕业生失业率约 5.6%，"大材小用"的比例约 42%
* 但也有不同的证据：另一项研究认为没有明确证据表明 AI 把应届生挤出了劳动力市场；美国大学雇主协会的数据显示 2026 届的招聘需求增长了 5.6%；IBM 宣布把入门级招聘提高到原来的三倍
* **结论**：入门级岗位确实在变弱，尤其是软件；但 AI 是不是主要原因，学界还在争论

### 5.7 最强的能力开始受限开放
Anthropic 的 Mythos 和 Google 的 Gemini 4 Argon 都只向少数网络安全合作方开放；OpenAI 因为安全问题取消了 GPT 6.1 Astra 的发布（见第一版报告）。

---

## 6. 一线从业者最常抱怨的问题

| 谁 | 最头疼的事 |
| :--- | :--- |
| 应用创业者 | 推理成本吃掉利润；依赖模型公司，而模型公司随时可能推出竞争功能；模型更新太快，评测跟不上 |
| 企业 | 试点很多，上线很少；数据接入难；安全（比如提示注入（prompt injection）攻击）；说不清投资回报 |
| 模型公司 | 算力贵且不够；人才争夺；电力；监管和安全 |
| 云和数据中心 | 拿不到电，买不到变压器，招不到电工 |
| 开发者 | 模型不稳定，会编造内容；Agent 出错的方式难以预测；成本难以预估 |
| 学生和新人 | 入门级岗位在减少 |

---

## 7. 机会

### 7.1 先用 Thiel 的框架看 AI 创业

大部分 AI 创业公司都处在和模型公司的竞争之中：今天你在模型之上做的功能，明天模型公司可能就直接内置了。所以在 AI 里，能形成垄断（monopoly）的通常不是"技术本身"，而是下面这几种东西：
1. **专有数据和反馈循环**：在某个垂直领域里，用户越多，数据越多，产品越好
2. **成为"记录系统（system of record）"**：比如 Epic 之于医院，客户的核心数据和流程都在你这里，换掉你的成本很高
3. **网络效应（network effects）**：协议、市场、多方参与的平台
4. **分发和品牌**：先占住用户的心智
5. **信任和验证**：当 AI 做的事越来越多，谁能证明它做对了，谁就有价值

### 7.2 第一类：风口（hot trend）

| 机会 | 为什么现在 | 退潮信号 |
| :--- | :--- | :--- |
| 帮中小企业落地 AI 和 Agent 的实施服务 | 绝大多数企业试点没有进入生产环境 | 大厂推出开箱即用的方案 |
| Agent 模板、技能包、MCP 连接器 | 高消费用户愿意为提效付钱 | 平台推出官方市场 |
| AI 评测和质量保证服务 | 模型更新太快，企业不知道该用哪个 | 评测工具标准化 |
| AI 使用培训（企业和个人） | 需求大，供给少 | 培训内容免费化 |

### 7.3 第二类：可能长出垄断的方向

**1. 验证层：证明 AI 做对了**
* 两类机会文档的方向 2。AI 生成的代码、文件、决策越来越多，验证成了瓶颈。这个方向在医疗（可审计的 AI 决策）、金融（可验证的规则）、能源（并网（interconnection）研究）里都出现了，是一条横跨多个产业的线

**2. Agent 信任层：身份、权限、责任**
* 两类机会文档的方向 4。在金融篇里它是"了解你的 Agent"，在医疗篇里它是"机器对机器的理赔（claim）"。这也是一条横跨多个产业的线

**3. 没有被数字化的行业的"记录系统"**
* 建筑、养老、小型制造这些行业，很多数据还在纸上和微信群里。过去软件进不去，是因为录入数据太麻烦；现在 AI 可以自动从照片、语音、文件里提取数据，让这些行业第一次有机会拥有自己的"Epic"

**4. 企业 AI 落地的"最后一公里"：数据接入和权限**
* 企业 AI 落地难，很大程度上卡在把旧系统的数据安全地接给 Agent。见第一版的产品卡 D

**5. 物理世界的数据**
* 两类机会文档的方向 1。语言模型的数据已经快被用完了，但机器人、工厂、医院里的真实交互数据才刚开始积累

**6. AI 时代的新人培养**
* **可能的秘密**：如果企业因为 AI 少招新人，五到十年后就会缺资深的人，因为资深的人都是从新人成长起来的。谁能建立"AI 时代的学徒制"（让新人和 AI Agent 一起在真实项目里快速成长，并把这种成长过程变成可信的能力证明），谁就可能掌握未来的人才供应链（supply chain）
* **适合你吗**：你本身就是这个问题的亲历者，又是 AI 的重度用户。这可能是你最容易获得"一线观察"的方向
* **会错的情况**：AI 发展到资深的人也不太需要了；或者企业很快恢复招新人

---

## 8. 接下来值得关注的信号

* OpenAI 和 Anthropic 的收入增长和上市进展
* NVIDIA 下一季度能否达到 1,080 亿美元的指引
* "循环交易"和数据中心融资是否出现问题
* 企业 AI 投资回报的新调查
* 中美芯片管制的变化
* 美国联邦是否统一 AI 规则
* 应届生就业数据
* GPU 租金走势（反映算力的供需）

**适合长期跟踪的信息源**：Stratechery（商业模式（business model）分析）、SemiAnalysis（芯片和算力）、Epoch AI（AI 趋势数据）、Import AI 周刊、Latent Space（播客和通讯）；中文可以看晚点 LatePost 和量子位。

---

## 参考来源

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
