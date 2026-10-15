# 财务 AI 竞品深度调研：选择工作环节与自动化路径

财务 AI 产品定位与设计 · 重点竞品拆解样本

资料核查截至 **2026-10-12**

## 调研结论

- **先确定产品接手哪项财务工作。** Ramp 与合思靠近支出发生，HighRadius 强调收付款等专业流程，FloQast 与 Numeric 从关账切入，Basis 执行会计工作，Rillet 和金蝶承担更广的账务体系，Pigment 连接计划与集团分析。它们在相邻环节交叉，采购与设计时应按具体流程比较。
- **真正影响产品形态的是数据与执行权。** 读取总账后生成解释、向既有 ERP 推送结果、维护正式账簿、修改经营计划模型，分别需要不同的数据模型、复核界面与实施承诺。Numeric 的叠加与 FDP 两条路线尤其能说明这一区别。
- **AI 自动化要按动作拆开。** Ramp 的合格卡交易可以进入自动同步；FloQast 公开要求人工批准入账；Rillet 的 Aura 动作先提案；Basis 因流程及置信度分配人工；Pigment 模型修改可选择 Auto-accept。不能用一个“AI 自动化程度”分数覆盖这些不同责任。
- **对财务 AI 产品设计，优先研究证据、例外与复核如何连起来。** 可借鉴的共同机制是结构化工作单元、来源依据、责任分配、受控执行与结果反馈；国内样本还要把票据、银行回单、凭证及档案关系纳入工作链。下文的设计机会属于分析判断，需用真实客户资料检验。

## 一眼看懂各家接手哪段财务工作

以下按每个样本的主要研究入口归类。产品经常跨越多个环节；该图表达工作关系，不是功能数量、市场份额或成熟度排名。

| 工作环节 | 主要工作 | 重点样本与工作关系 |
| --- | --- | --- |
| 01 支出发生 | 购买申请、消费、费用与票据 | **Ramp · 合思**<br>在花钱和提单时收集用途、制度与责任。 |
| 02 交易处理 | 付款、核销、争议与催收 | **HighRadius**<br>将交易与未结项目匹配，例外进入责任队列。 |
| 03 账务记录 | 核算、分录、账簿与集团口径 | **Rillet · 金蝶 · Numeric FDP**<br>正式财务记录和会计逻辑成为产品核心。 |
| 04 关账复核 | 对账、进度、差异与签核 | **FloQast · Numeric**<br>把准备工作、证据与批准过程连接起来。 |
| 05 经营决策 | 计划、情景、预测与集团合并 | **Pigment**<br>在经营模型中协作并产出预测和集团报告。 |

**Basis 是执行型会计样本。** 它围绕具体会计任务调用资料和工具，覆盖事务所及企业内部工作。其自动推送、暂存与人工复核取决于具体流程，因此放在横跨账务与会计作业的位置。

## 九个样本的工作内容与结果归宿

下面比较的是每家**主要工作单元与结果归宿**。ERP 指企业管理与财务记录系统；这里的“记录系统”特指正式账务保存在何处。表中的覆盖是所选研究单元的公开范围，不代表每项能力在同一套餐或同一地区可用。

| 样本与研究入口 | 从什么走到什么结果 | 记录系统关系 | 重点借鉴机制 |
| --- | --- | --- | --- |
| 01 **Ramp**<br>支出与付款 | 卡/账单/PO/收据 → 受控支出、付款与会计同步 | 主要接入既有 ERP；Stack 另扩展会计工作执行 | 交易发生时收集背景，编码与付款连在一起 |
| 02 **HighRadius**<br>企业财务流程 | 付款说明/未结发票 → 核销、短付处理、催收及 ERP 更新 | 跨 ERP 自动化层；另有 AP、关账、合并与资金套件 | 交易处理改变后续收款与争议状态 |
| 03 **FloQast**<br>关账与会计工作流 | ERP/底稿/清单 → 对账、待审分录、签核及审计证据 | 保留 ERP；工作与控制放在 FloQast | 准备、复核和可重用 Agent 同处会计流程 |
| 04 **Basis**<br>会计任务执行 | 客户 GL/来源/政策 → 底稿、分录、例外与报告 | 连接原账务系统；覆盖事务所及企业会计 | 客户上下文和 Procedures 形成重复工作 |
| 05 **Rillet**<br>新总账与财务 ERP | 合同/发票/付款 → 支持计划、分录、实体及合并报告 | 自身总账是记录系统，替换原 ERP | 业务对象、账务计划和 AI 提案连到同一账簿 |
| 06 **Numeric**<br>关账分析与可选 FDP | ERP/底稿 → 关账与分析；FDP 对象 → 账务结果 | 叠加模块与 ERP Replacement 两条路线 | 证据丰富的关账，逐步扩展记录平台 |
| 07 **Pigment**<br>经营计划与集团合并 | 实际数/假设/模型 → 预算、预测、情景及合并报表 | 经营模型与合并层；现有 ERP 提供实际数 | AI 可建模型，也可在模型上解释和持续报告 |
| 08 **金蝶**<br>集团财务 ERP 与共享 | 业务单据/会计口径 → 审核、支付、核算及集团报表 | 主拆 AI 星瀚财务云；小K内嵌，灵基另列 | 中国集团业财税资、共享与权限控制 |
| 09 **合思**<br>国内费用与票款凭证 | 消费/合同/票 → 审批、付款、ERP 凭证及档案 | 接入既有 ERP，叠加费用、付款和档案层 | 支出来源与票款凭证关系，AI 审核给风险依据 |

## 逐家拆解  由工作结果理解产品

每个样本先显示用户、核心工作和四步流程；展开后可查看模块、AI 与数据、实施、价格、案例及设计启示。模块按工作内容整理，不代表全部独立收费；说明性用例与厂商案例已分别标注。

### 01 Ramp  从支出发生到付款与会计同步，把政策和资料留在每笔交易里

**服务谁**：CFO、Controller、AP 和采购负责人推动购买；员工提交购买与费用，经理审批，AP 处理供应商账单，会计审核编码与同步。Stack 另面向企业会计团队和服务多客户的会计事务所。

**接手的工作**：在购买、刷卡或账单到达时收集上下文，按预算与政策控制支出，将发票、付款、审批和会计编码连成流程，减少关账时重新追收据、重建费用用途和重复录入。全公司平台覆盖卡、费用、AP、采购、银行及更多产品；Stack 是跨账簿和工作簿的独立 AI 工作环境，不能把它等同于普通卡片功能。

**开始条件**：员工发起购买、已清算卡交易或供应商账单到达；下面重点描述支出到 ERP 的会计流程

[Ramp 当前主页与产品范围](https://ramp.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | 交易明细、收据与说明、历史编码、供应商发票及行项目；AP 还用 PO、收货资料、供应商支付信息和合同背景 |
| 02 处理 | 提取发票、匹配 PO 与收货、检查异常、按规则和历史补充会计字段；按权限路由审批，区分可继续处理与需关注的项目 |
| 03 复核 | 人员处理缺资料、越政策与编码疑问；可修正 AI 建议。AI 编码不覆盖员工、管理员或规则填写的值；自动标记 Ready 和自动同步分别启用 |
| 04 产出与去向 | AP 批准后安排付款并同步账单及支付记录；卡交易自动同步有资格条件，管理文档称夜间美国东部时间午夜执行，不能把所有流程都写成即时同步 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 企业卡与费用 | 发卡、限额与支出控制，收集收据、费用和报销资料<br>[官方依据](https://ramp.com/) | 受控交易及费用证据 |
| 采购与供应商 | 购买申请、审批、PO、供应商合规和合同资料<br>[官方依据](https://ramp.com/pricing) | 可追踪的采购申请与订单；采购为 Plus/Enterprise 加购 |
| AP / Bill Pay | 发票提取、行项目编码、匹配、审批和多渠道付款<br>[官方依据](https://ramp.com/accounts-payable) | 账单、审批状态、付款及 ERP 同步记录 |
| 会计自动化 | 利用交易与历史补充编码，筛出需审核的支出，支持应计与对账<br>[官方依据](https://ramp.com/accounting-automation-software) | 待审核交易、已完成编码及会计同步 |
| 预算与报表 | 预算对实际、定制报告及支出可视化<br>[官方依据](https://ramp.com/pricing) | 预算使用情况与定期导出；功能随方案变化 |
| 银行与应收 | 官网另列资金账户、开票、客户跟进及现金核销<br>[官方依据](https://ramp.com/pricing) | 公司资金及应收相关工作；不等于完整总账 ERP |
| Stack by Ramp | 用连接器和可复用 Skills 执行对账、计划表、应计、分录及月度分析<br>[官方依据](https://ramp.com/stack) | 公式工作簿、待审分录、批准同步与 Session Audit Log |

#### AI 与复核

AP AI 提取与编码，识别异常支付资料，整理供应商/合同/PO 背景并建议批准或拒绝；卡会计 AI 填合格字段并建议下一步。客户设重要性阈值和政策，系统判断高置信合格项目；当前帮助文档称用户不能自定 AI 置信阈值。Stack 产出可审核工作及来源日志，人员批准需判断的内容后发布。

[Ramp Accounting Agent 管理与日常使用文档](https://support.ramp.com/ramp-accounting-agent-enablement-daily-use-admin-guide)

#### 数据与集成

支出记录把供应商、员工、用途、行项目、单据和审批关联在一起；会计产品写回现有 ERP。官网列 30+ 会计系统，而 Bill Pay FAQ 列 10 个 ERP，不能把不同模块接入名单视为同一范围。定价页中 QBO/Xero 属 Free，NetSuite/Sage 等属 Plus，Workday/Oracle Fusion 等属 Enterprise。Stack 连账簿、银行与文档，以源资料、工作簿和分录组织任务；本次证据未表明 Ramp 提供替换整个 ERP 的账务记录系统。

#### 关键特性与比较位置

产品在交易发生前后同时介入：卡限额与购买审批提供控制，支付执行和 ERP 同步完成后续闭环，原生交易上下文有助于会计编码。它的核心入口是花钱与付款，Numeric 的核心起点更接近关账和财务数据分析；当前 Stack 使双方在会计工作执行上出现交叉。

#### 采用与实施

Bill Pay 可单独使用，先连接会计系统并导入供应商、绑定付款账户，配置角色、审批和发票转发；不用同时采用企业卡。复杂企业方案公开列集成验证、组织/实体与角色配置、员工培训和实施服务。建议先在一类有规律支出上验证编码和例外处理，再扩大自动处理范围。这是基于公开流程的实施判断。

#### 价格与合同范围

2026-10-12 英文官网：Free 为 $0 / 用户 / 月；Plus 显示 $15 / 用户 / 月，另加按团队规模计算的平台费，年付可节省 20%；Enterprise 询价且年付。采购是 Plus 或 Enterprise 加购。Stack 页面仅显示免费试用，未查到可核实的长期统一金额；不得把 Plus 价格当 Stack 价格。付款和其他服务成本需按使用方式另核验。

[Ramp Pricing and Plans](https://ramp.com/pricing)

#### 说明性使用例

说明性推演：一张 $500 软件账单到达后，提取行项目，关联供应商及 PO，补上费用编码；金额较历史突增时向审批人显示原因。通过批准后付款并把账单、支付和证据同步 ERP。对公司要求 PO／收货匹配的账单，缺少相应资料时进入待处理队列。本用例依据公开功能编排，未在真实账户执行。

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**Perplexity**：厂商案例称 >97% 的交易自动编码且无人工触碰

正文具体为每月约 7,000-9,000 笔卡交易；由规则和 AI 共同完成，不能解释成所有 AP 或所有会计工作无人处理

[Ramp Perplexity 官方客户案例](https://ramp.com/customers/perplexity)

**Perplexity**：厂商案例称每月自动化 163+ 小时，覆盖关账、编码和管理工作

该案例的工作时间容量口径；不是独立测量，也不是所有客户承诺

[Ramp Perplexity 官方客户案例](https://ramp.com/customers/perplexity)

#### 关键边界与待确认项

- Accounting Agent 功能随账户而异且 AI 编码属 Plus；自动同步卡交易的资格、实体映射与夜间队列需核验，营销页面的实时描述不能替代操作文档。
- 目前不能自定义 AI 置信阈值，也不能查看已提交给 Agent 的反馈集合；不能据此承诺客户拥有完整模型治理面板。
- Bill Pay 的 ERP、PO 导入及摊销支持与全平台不同，例如公开摊销功能明确提到 NetSuite。
- 发卡、银行、支付渠道与地区资格需要单独确认；证据不能证明中国本地税票、支付清算和全部会计准则覆盖。
- Stack 与支出产品的打包方式、长期价格、每连接器写权限及失败回滚机制未在本次公开资料中完整披露。

#### 设计启示  分析判断

- 分析判断：从支出入口收集用途和责任人，可减少月底让 AI 猜原因；对中国产品尤其值得把发票、合同、审批和记账来源关联。
- 分析判断：把可自动处理、需补资料和需人工判断分成清楚的工作队列，并展示为什么，能让用户理解自动化边界。
- 分析判断：标记可发布与真正写入账簿是两道状态，应独立配置并显示同步结果；不要只把一个自动化按钮当作闭环。

### 02 HighRadius  连接企业收款、应付、关账与资金流程，让交易处理与 ERP 更新连续完成

**服务谁**：CFO、全球业务服务/共享服务及财务转型负责人购买；信用、应收、收款核销、催收、扣款争议、AP、总账关账及资金团队使用，IT和银行/ERP管理员参与集成。重点面向中大型与多实体、多 ERP、高交易量组织。

**接手的工作**：把散落在银行、邮件、客户 AP 门户和多个 ERP 的资料汇集起来，完成收款核销、争议和催收等大量重复交易处理，并将结果回写账务系统。全套公司产品还覆盖 AP、关账与对账、合并报表、B2B 支付和资金管理；研究时应按具体套件和业务场景比较，不能以现金核销一个模块代表全部产品。

**开始条件**：银行收到客户款项；以下以 Cash Application 为具体闭环

[HighRadius 当前主页及 CFO 产品套件](https://www.highradius.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | 银行支付数据、邮件/附件/支票/客户门户的付款说明、ERP 未结发票和客户记录、原因码与容差政策 |
| 02 处理 | 提取付款说明，将付款关联客户与未结发票，处理部分付款和折扣，标记或编码短付；缺说明时可请求补充，并分配例外队列 |
| 03 复核 | 现金分析员处理无法确认的匹配和例外，也可按需手动发送 ERP 付款数据；DXP 案例将 Payment Exception Handler 明确列为 Assisted Agent，不能写成所有流程无人复核 |
| 04 产出与去向 | 通过 API 或文件发送 enriched payment 至 ERP，登记收款和清除未结发票；保留待处理付款、扣款原因和核销状态，使催收人员知道哪些发票仍真正未收 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| Order to Cash | 信用、电子发票、现金核销、扣款和催收协同<br>[官方依据](https://www.highradius.com/) | 信用动作、已核销收款、争议与催收任务 |
| Cash Application | 多渠道付款说明提取、付款与发票匹配、短付编码及 ERP 记账<br>[官方依据](https://www.highradius.com/product/cash-application-automation/) | 已登记收款、清账和需要人员处理的例外 |
| Accounts Payable | 供应商接入、发票提取、重复/欺诈检查、三方匹配和付款<br>[官方依据](https://www.highradius.com/) | 审批及供应商支付流程；是单独套件范围 |
| Close & Reconciliation | 现金、PO应计、预付、余额表、收入与往来核对，提前提示异常<br>[官方依据](https://www.highradius.com/software/financial-close-and-reconciliation-software/) | 对账、应计和调整任务、分录及关账状态 |
| Consolidation & Reporting | 总账余额汇总、汇率转换、往来抵销与报表<br>[官方依据](https://www.highradius.com/) | 合并账务结果和财务/管理报表 |
| Treasury & Risk / B2B Payments | 现金头寸与预测、资金付款；另有收单、附加费和交换费优化<br>[官方依据](https://www.highradius.com/) | 资金可视化、预测与支付结果；不是 Cash Application 的同义词 |

#### AI 与复核

在现金流程中，AI/OCR 提取付款说明、建议或执行匹配、推断短付原因、请求缺失说明并将异常交给分析员；可按容差码处理小额差异。关账套件另列异常检测、预付/应计和分录动作。自动与辅助任务要分别看：厂商 DXP 图将超过90%自动化的 Agent 和需要人员的 Assisted Agent 区分；Agent 数量不代表不受政策或审批控制。

[HighRadius Cash Application Software](https://www.highradius.com/product/cash-application-automation/)

#### 数据与集成

现金核销围绕客户-未结发票-收款-付款说明-扣款案例组织数据，而非先生成文字分析。HighRadius 发布的 Sage Intacct 集成说明明确 ERP 继续作为账务记录系统：客户、发票和应收进入 HighRadius，收款、争议和信用更新返回 ERP。关键更新可用 HTTPS API，大量记录可通过 SFTP 批次交换，初始全量后增量。页面同时有实时与每日描述，因此实际频率需确认。它是跨 ERP 的自动化层，不能与 Numeric FDP 的 ERP 替换路线等同。

#### 关键特性与比较位置

强调各专业财务流程之间的连续编排，尤其针对大量款项、短付款、客户门户和多 ERP 环境。现金核销完成后直接影响催收与争议，可避免已付款客户仍被追款；价值指标更接近 DSO、未核销现金、回收率与人员处理能力。和关账单点产品相比，其实施范围往往涉及更多业务规则、客户/银行数据和团队。

#### 采用与实施

应先选流程和 KPI 基线，核对客户/发票/原因码及银行/门户资料，配置容差、例外路由和 ERP 回写，进行试点与用户培训。DXP 案例称 Cash Application、Collections 与 EIPP 跨15+ ERP的一次部署耗时30周，采用先标准功能后增强的方法；这是特定复杂案例，不能泛化为统一周期。结果付费仍须明确收益计算、数据基线和验收方式。

#### 价格与合同范围

询价，无可核实统一订阅金额。当前主页推广 Outcome-Based Pricing；官方公告称该模式实施费为 $0、上线前订阅费为 $0，之后按实际实现收益分成，需双方约定 MASC 基线与目标。原 pricing 页面仍描述通常按年度 SaaS 订阅、按功能使用收费；因此应向销售确认适用合同及分成比例，不能写成产品永久免费或所有客户均只按结果付费。公告未显示可验证发布日期，不从版权年份推断。

[HighRadius Outcome-Based Pricing 官方公告](https://www.highradius.com/about/news/highradius-launches-outcome-based-pricing-for-ocfo-software/)

#### 说明性使用例

说明性推演：客户汇入98,000元、付款说明引用100,000元发票并说明扣除2,000元价格差异。系统关联该付款和发票、编码短付原因，确认可核销部分；有疑问的差额交给争议分析员，结果回写 ERP 后催收队列更新。这是基于现金模块公开能力设计的案例，未在真实环境验证，也不表示未经配置自动认可客户扣款。

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**DXP Enterprises**：厂商案例称现金核销达到90%+ straight-through / automation

15+ ERP、多收购实体和约300Mn美元贸易应收环境；包含明确需要人工的例外处理 Agent，不能当全产品自动化率

[HighRadius DXP 官方案例 PDF](https://pages.highradius.com/hubfs/highradius.com/case-study/Content%20COE%20New/Case%20Studies/dxp_casestudy.pdf)

**DXP Enterprises**：厂商案例称 DSO 降低20天

现金核销、催收和EIPP共同部署的结果；不可全归于某个AI模型，也不是统一承诺

[HighRadius DXP 官方案例 PDF](https://pages.highradius.com/hubfs/highradius.com/case-study/Content%20COE%20New/Case%20Studies/dxp_casestudy.pdf)

#### 关键边界与待确认项

- 50+ ERP、银行或门户数量是厂商覆盖描述，不能证明某个客户配置的读写字段、地区和同步频率。
- 不同产品页的实时、每日、文件批次口径不同；选型必须演示 ERP 接收与错误修复，而不是只展示匹配成功。
- 公开 Cash Application 支持小额容差处理和自动记账，但具体审批、权限隔离、阈值及回滚没有本次端到端实测。
- Outcome-Based Pricing 无公开分成比例与合同范围；旧订阅页与新模式并存，需要确认适用方案。
- 官网性能数字主要是目标、保证措辞或厂商案例；本文未取得独立对照试验，不把跨模块综合收益视为单一 AI 的因果效果。

#### 设计启示  分析判断

- 分析判断：围绕付款、发票、扣款和责任人建结构化工作单元，能让自动核销实际改变催收与争议状态，比单独展示识别结果更有用。
- 分析判断：大中型客户需要跨系统数据与业务码标准化，产品应显式提供映射、例外队列、传输状态和重试。
- 分析判断：ROI 可以用未核销现金、处理时长与回收率衡量，但应保留基线和分母；按收益定价也需要可审计的收益核算。

### 03 FloQast  把关账工作、支持证据与签核放在一起，让 AI 做准备、会计做复核

**服务谁**：Controller、会计负责人、CFO/CAO及财务转型负责人购买；会计准备人与复核人、跨实体团队使用，内控、内审及外审查看控制与证据，IT参与集成。它同时服务日常会计、月末关账与合规，不是只面向 CFO 的问答工具。

**接手的工作**：把每月重复的清单、账户对账、分录、支持文件、审批和问题集中起来，知道谁还未完成、哪些账户未对上、哪些分录未批准。Close Management 提供基本组织和签核；Close AI 在这一基础上加入匹配、自动对账、分录与自定义 Agent；Risk & Compliance 可单独或与关账方案组合。公开定位仍是使用现有 ERP 账务而增强工作执行，未表明要替换完整 ERP。

**开始条件**：期间关账或每日需要执行的对账/应计；以下是账户对账到调整分录的典型路径

[FloQast 当前主页](https://www.floqast.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | ERP 余额与交易、支持工作簿及银行/其他来源资料、账户规则、上期已完成流程和清单 |
| 02 处理 | 清单按实体、责任人与依赖推进，余额与支持资料核对；AI/自动化准备匹配、计划表和分录，发现异常；Transform 可将完成的工作或输入输出描述变为可复用 Agent |
| 03 复核 | 团队检查例外、支持文件与计算逻辑并签核；官网明确入账需要人工批准。分录路由控制准备人不能审自己的工作，批准后条目锁定 |
| 04 产出与去向 | 通过已配置连接发布分录至 ERP，更新关联关账清单状态；保存对账、说明、修改与审批证据，供后续复核及审计 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| Close Checklist / Accounting Operations | 责任、实体、时间、依赖、截止日期及周期滚动；可延伸日常财务工作<br>[官方依据](https://www.floqast.com/close-management) | 全局进度、风险任务与跨部门协同 |
| Account Reconciliations | 余额与资料核对，记录差异、检查覆盖完整性并签核<br>[官方依据](https://www.floqast.com/close-management) | 已复核账户和待解决差额 |
| AI Matching / Automated Reconciliations | 高交易量匹配、三方匹配以及摊销、折旧和分账核对<br>[官方依据](https://www.floqast.com/pricing) | 匹配结果、重复会计计算与例外 |
| Journal Entry Management | 创建、验证、审核、发布、复制及反转分录，关联清单与证据<br>[官方依据](https://www.floqast.com/close-ai/products/journal-entry-management) | 批准后的 ERP 分录及可追溯状态 |
| Transform AI Agents / AI Assistant | 用 Builder、Skills 和预设库执行准备工作；Assistant 回答关账和余额问题<br>[官方依据](https://www.floqast.com/close-ai/products/ai-agents) | 可复用流程、可审核工作及来源/操作证据 |
| Variance / Detect / Close Analytics | 解释差异、捕捉异常与观察关账过程<br>[官方依据](https://www.floqast.com/pricing) | 需审阅的变化及流程分析；套餐和具体能力需逐项确认 |
| Risk & Compliance | 设计、测试、映射控制并跟踪问题整改和审计<br>[官方依据](https://www.floqast.com/pricing) | 控制证据、风险与整改记录；可单独采用 |

#### AI 与复核

Assistant 基于公司关账资料回答并遵守原有权限；Transform 可基于完工流程创建 Agent，由可复用 Skills取试算表、验证数据和准备分录等。Agent需在自身数据上测试并经会计批准，输出带理由和记录。HubSpot案例描述将逻辑转为可重复Python和公式工作簿，这是该案例的技术机制，不代表所有AI动作都采用同一执行方式。最终入账审批留给人。

[FloQast Journal Entry Management](https://www.floqast.com/close-ai/products/journal-entry-management)

#### 数据与集成

主要工作单元是任务、账户对账、分录、支持文件与签核；数据来自 ERP 和业务系统，结果连回关账进度。公开分录说明支持多来源/多ERP、Excel大额复杂分录上传和模板。当前主页列 NetSuite、SAP、Workday、Oracle、Sage、Xero等，但不能从logo推断所有模块均可对每个ERP直接写回。公开 HubSpot 流程使用上传的 Coupa 发票和PO，而非证明所有客户都已采用实时直连。

#### 关键特性与比较位置

强项是把会计责任、证据、复核和自动化放在同一流程中，保留会计熟悉的工作簿，允许从标准关账扩展到自定义准备工作及内控。与 Numeric 相比有明显的关账重合，但 FloQast 当前更突出以现有ERP与会计流程为中心的治理，Numeric FDP另有从业务对象派生账务的替换路线。

#### 采用与实施

先把关账清单、账户支持与审阅责任组织清楚，再配置来源系统、模板和审批；采用 Transform 时可挑一个应计或预付流程做PoC，用自身数据验证计算和证据，再扩展。HubSpot案例描述团队办5小时实操活动学习构建流程；这说明学习和流程整理属于采用工作，不等于安装后所有会计流程即刻自动运行。本次帮助中心访问返回 Internal Error，未获得后台配置手册。

#### 价格与合同范围

当前英文定价页不公布统一金额，全部联系销售；明确无按用户收费，按组织需求、范围和规模定价。当前组合为 Close Management、Close AI、Risk & Compliance，后者可单独或与任一Close组合。不同地区页面仍有 Close Optimization/Transform 等旧命名，本报告按当前英文主站记述，不从第三方估算年费。

[FloQast 当前英文 Pricing](https://www.floqast.com/pricing)

#### 说明性使用例

说明性推演：月末把ERP预付余额与支持工作簿交给流程，按公司摊销逻辑计算并列出不一致账户；准备调整分录及来源资料，复核人检查、批准后发布ERP，清单显示任务完成并保留审计证据。这是公开功能的组合说明，未做真实账户测试，也不代表未经配置AI自动选择会计政策。

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**HubSpot**：厂商案例正文称预付流程由3名员工每月6小时组装15实体工作簿，转为1人每月1.5小时生成合并工作簿

保留原文人员与时间口径，不自行乘算成18小时；同页摘要又写15实体15分钟，存在不一致，需要客户或厂商澄清

[FloQast HubSpot 官方客户案例](https://www.floqast.com/stories/the-hubspot-blueprint-building-an-accounting-led-ai-powerhouse)

**HubSpot**：厂商案例正文预计应计与PO资料增强流程可减少50%准备时间

原文为 projected，不作为已验证成果；同页摘要写成已实现，本文采用正文的预期属性

[FloQast HubSpot 官方客户案例](https://www.floqast.com/stories/the-hubspot-blueprint-building-an-accounting-led-ai-powerhouse)

#### 关键边界与待确认项

- 公开主页明确人工入账批准，但JEM也用auto-certify等措辞；需要演示具体审批/认证含义，不据此推断无人批准过账。
- ERP列表与第三方应用目录不等于各模块均已直连可写；实施前需核实字段、权限、同步频率及失败处理。
- 帮助中心 https://help.floqast.com/ 在2026-10-12本次浏览返回Internal Error；配置与角色粒度未获得完整公开手册。
- HubSpot案例中的1.5小时与15分钟、预计50%与摘要已实现50%存在冲突；不将这些数字直接当统一产品性能。
- 认证及审计准备功能不保证客户通过审计；中国准则、税务、税票和境内部署范围未在此次材料中完整确认。

#### 设计启示  分析判断

- 分析判断：会计用户更容易验证可点击公式、来源资料和审批记录；让AI输出进入熟悉的复核界面，可能比新建聊天入口更容易采用。
- 分析判断：准备者与审核者职责隔离需要体现在权限、状态和记录上，既约束人也约束Agent。
- 分析判断：以做完的工作和清楚的输入输出培养可重复流程，是比空白Agent编辑器更有帮助的起点；上线前测试应覆盖异常和期后更改。

### 04 Basis  按客户政策执行会计准备工作，输出可复核的底稿与分录

**服务谁**：会计事务所合伙人、CAS 业务负责人、创新/技术负责人；企业内部 CFO 和会计负责人也是当前明确服务对象。

负责客户账务和税务准备的会计人员、主管与复核者。审计师仍负责证据充分性与最终结论。

**接手的工作**：把事务所或企业的既有方法、模板、映射与复核标准变成可反复执行的会计工作。它承接准备与处理，输出可以检查的底稿、分录和解释；公开描述显示其可连接原有总账，而不是要求统一迁入新 ERP。

**开始条件**：月末关账、税务项目或会计人员发起具体 Procedure。触发方式按公开能力归纳，统一调度机制未公开。

[Basis - AI Agents for Accounting](https://www.getbasis.ai/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | 连接客户 GL，提供工资报告、发票、银行对账单等来源，并补充该客户的政策、映射、上一期工作与反馈。 |
| 02 处理 | Agent 按既有标准分类交易、准备支持表、比对资料并定位例外；税务流另组织客户材料与工作底稿。 |
| 03 复核 | 人员查看来源、计算、解释和例外。Small Firms 页分录先暂存待审；CAS 页另允许高置信度交易自动推送，低置信度项目进入复核，不能写成统一逐笔审批。 |
| 04 产出与去向 | 企业会计页明确将已批准分录写入 ERP；也生成差异说明和报告包。具体 ERP 可写对象、失败回滚和权限配置需演示确认。 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 交易分类与账务清理 | 为银行、信用卡和已有 GL 活动提出会计处理。<br>[官方依据](https://www.getbasis.ai/solutions/cas-and-advisory) | 分类结果、解释、待复核条目。 |
| 重复关账准备 | 读取支持资料，准备支持表、底稿和分录。<br>[官方依据](https://www.getbasis.ai/solutions/corporate-accounting) | 可审查的关账工作与批准后 ERP 分录。 |
| 对账与报告 | 比对总账、对账单及支持表，归纳期间变化。<br>[官方依据](https://www.getbasis.ai/solutions/cas-and-advisory) | 未匹配例外、差异说明和报告包。 |
| 税务第一轮准备 | 组织客户文件、补资料缺口并形成工作底稿。<br>[官方依据](https://www.getbasis.ai/solutions/tax) | 带引用和开放问题的税务初稿，供人员复核。 |
| 审计工作支持 | 执行测试并为结论保留证据。<br>[官方依据](https://www.getbasis.ai/) | 供审计师评估与负责的工作成果；不等于自动审计意见。 |
| Procedures 与客户上下文 | 使用或创建可共享程序，按客户组织工作。<br>[官方依据](https://www.getbasis.ai/solutions/small-firms) | 可重复执行的方法与延续的客户知识。 |

#### AI 与复核

生成分录与底稿，处理分类和对账，完成税务第一轮，归纳报告。当前范围还包含审计支持。

职责按工作流不同：分类可高置信度自动推送；分录准备页强调先待审；企业会计只明确已批准分录写回。阈值如何设定、自动推送如何关闭及职责分离未在这些页面详述。

可检查不等于准确性已独立验证；税务人员、审计师和企业会计仍承担复核与判断。

[Basis for CAS & Advisory](https://www.getbasis.ai/solutions/cas-and-advisory) · [Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms) · [Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting) · [Basis for Tax](https://www.getbasis.ai/solutions/tax) · [Basis - AI Agents for Accounting](https://www.getbasis.ai/)

#### 数据与集成

公开产品中心是客户/公司上下文、来源材料、Procedures、工作底稿和分录。精确后台对象模型未披露。Small Firms 的多客户组织避免把不同客户的知识混在同一任务中。

公开确认连接 GL、推送分录和分析；企业会计描述保留已有 ERP。当前所读页面没有完整连接器矩阵，不能自行假定所有 ERP 支持同等读写。

CAS 页说明来源、计算、解释、置信度和例外集中可检查；反馈及已批准程序可带到后续期间。

[Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms) · [Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting) · [Basis for CAS & Advisory](https://www.getbasis.ai/solutions/cas-and-advisory)

#### 关键特性与比较位置

从多客户事务所工作切入，同时扩展企业内部会计；同一平台的范围跨 CAS、税务和审计。

Procedures 把客户差异与团队方法转成重复任务。比较时应重点看已有方法迁入后的执行与复核成本。

相对纯关账清单，明确涉及处理资料、准备分录及 ERP 写回；相对新 ERP，其公开产品说明主要连接现有账务环境。

#### 采用与实施

官网引导演示与访问申请。Deployed Intelligence 团队深入客户组织，学习具体上下文并协助围绕 Agent 改造工作方式；这是厂商对服务方式的描述。

应先选择一种重复工作，将企业政策、模板与复核者配置清楚，再验证写回。上线依赖组织方法整理与复核习惯，而不只是开通账号。

未在所读资料中找到统一实施周期或可复用的迁移费表。

#### 价格与合同范围

询价

已检索 getbasis.ai 的公开价格并读首页与产品访问入口，未找到公开金额或套餐计费规则。应通过演示/访问申请取得报价。

basis.so 和 basishq.co 是不同产品，不能使用它们的价格。

[Basis - AI Agents for Accounting](https://www.getbasis.ai/) · [Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms)

#### 说明性使用例

事务所为一家客户处理工资计提：连接客户 GL 并提供工资报告，由程序准备带来源的分录和支持表；会计检查映射及例外后批准，再确认写入该客户 ERP 的结果。

同一任务里展示数据、拟议分录、依据、例外及写回状态，避免复核人员反复跨系统。

[Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms) · [Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting)

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**REDW**：CFO 证言称四个月内关账从 20 天缩短至 15 天；原文为 days，未限定工作日。

Basis 企业会计页发布的客户证言，未独立验证

[Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting)

#### 关键边界与待确认项

- 完整 ERP/税务软件连接矩阵、每对象写权限、推送阈值、失败恢复与职责分离配置未公开验证。
- 税务与审计产品宣传覆盖整个第一轮，不证明所有复杂事项可无人处理，也不证明中国税务/准则适配。
- 缺少统一错误率、例外漏检率及从初稿到复核通过的工时数据。案例效率不能直接推广。
- 所读企业页称不以客户数据训练模型；区域与具体处理商合同仍需逐项核对。
- Boyum 案例正文未被工具提取，已单独标注证据有限。

#### 设计启示  分析判断

- 分析判断：执行型产品应以工作成果与例外队列作为主界面，复核者能迅速知道哪些已做、哪些待判断、哪些已写回。 Basis 的待审分录与置信度分流提供具体参照。
- 分析判断：上下文按客户隔离，政策、上期成果和反馈显式存储，比让用户每月重新写提示更容易形成重复工作。 Procedures 与多客户组织。
- 分析判断：应分别给出自动推送和待审执行的控制方式，不用一个“自主 Agent”标签掩盖职责差异。 CAS 与 Small Firms 描述的控制不同。

### 05 Rillet  保存正式总账与支持计划，Aura 在账内准备提案并交人批准

**服务谁**：CFO、Controller 与财务负责人；官网同时列出会计事务所等角色和不同企业规模。

会计团队准备、检查和批准账务；只读的投资人、董事会及跨部门负责人查看结果。

**接手的工作**：连接收入、支付、费用和人事等业务数据，把合同、发票、账单形成持续更新的分录和支持计划，再由同一账务来源产生财务及经营报告。它不是仅附在现有 ERP 上的分析工具。

**开始条件**：业务系统同步新数据、合同完成/变更、期间关账，或人员发起 Aura 查询和工作流。

[Rillet - The AI-Native ERP](https://www.rillet.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | CRM 合同、发票、账单、付款与企业配置；可通过连接器、文件和 API 导入。 |
| 02 处理 | 生成收入、递延、预付和资产支持计划及分录。Aura 查询实时 GL、安排工作流、识别异常并提出计提。 |
| 03 复核 | 收入页明确先审合同再入 GL；安全页明确 Aura Agent 提案交人批准。按金额分层路由，批准和拒绝留痕；确定性支持计划的自动入账与 AI 提案应分开理解。 |
| 04 产出与去向 | 分录直接进入 Rillet 自身总账，带动支持计划和报表更新；这里的账务结果是记录系统的一部分，不是仅生成供导入旧 ERP 的文件。 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 持续总账与支持计划 | 接收业务对象并生成分录及收入、预付、固定资产支持表。<br>[官方依据](https://www.rillet.com/product/automated-general-ledger) | 统一 GL 和账务支持。 |
| 收入确认与应收 | 从合同服务期间生成收入计划，关联开票、用量和收款。<br>[官方依据](https://www.rillet.com/product/advanced-revenue-recognition) | 收入瀑布、递延收入与客户收入视图。 |
| 对账与关账 | 组织关账清单、银行匹配和 Flux。<br>[官方依据](https://www.rillet.com/product/automated-general-ledger) | 待处理差异、清单进度与变化解释。 |
| 多实体与报告 | 处理多币种、内部往来，查看子公司及合并口径。<br>[官方依据](https://www.rillet.com/product/aura-ai) | 实体/合并报表以及 GAAP 与经营口径。 |
| Aura AI | 实时 GL 问答、重复工作流、异常和计提提案、MCP 读写连接。<br>[官方依据](https://www.rillet.com/product/aura-ai) | 查询答案与可审查的工作提案。 |
| 审批与期间控制 | 角色访问、金额分层审核、实体子账及期间锁定。<br>[官方依据](https://www.rillet.com/product/security-and-permissions) | 批准/拒绝、变更与锁定记录。 |

#### AI 与复核

Aura Assistant 查账；工作流 Agent 安排数据拉取和交接；Continuous AI 提示异常、建议计提；MCP 向外部工具开放受控读写。

安全页明确 Agent 准备、人员授权，未经批准不发布；支持重要性阈值、职责分离和模型变更控制。不能将“零日关账”理解为账务没有复核或任何交易都由模型自行决定。

这些是当前厂商公布的控制行为，尚未对真实账号操作验证；MCP 各对象写范围仍需核对。

[Aura AI by Rillet](https://www.rillet.com/product/aura-ai) · [AI you can audit](https://www.rillet.com/product/security-and-permissions)

#### 数据与集成

总账是账务记录系统；合同、发票、账单驱动原生支持计划。GL 页确认文件可批量创建/更新对象，API 可导入数据；详细对象 schema 未在本轮审阅。

帮助中心明确列出 Salesforce、Stripe、Ramp、Brex、Rippling。其声称可集成 12,000+ 平台，但未逐一验证原生连接与其他接入方式，报告不据此认定同等深度。

官网强调分录追到来源。安全页描述 Agent 查询、提案、批准与拒绝的时间及理由留痕；关闭期间防止未授权变更。

[General Ledger Software with AI Automation](https://www.rillet.com/product/automated-general-ledger) · [Rillet Help Center](https://www.rillet.com/help-center) · [Rillet - The AI-Native ERP](https://www.rillet.com/) · [AI you can audit](https://www.rillet.com/product/security-and-permissions)

#### 关键特性与比较位置

拥有总账、业务对象和原生支持计划，自动化结果进入自身账，而非只管理工作状态。

Aura 与实时 GL 共用数据及公司配置，查询和提案可连接实际账务控制。

从合同、收入计划到客户经营指标的一体路径，对复杂收入企业尤其值得验证；这是基于功能的适用判断。

#### 采用与实施

帮助中心说明云端交付；CPA 和前审计人员提供实施服务，客户主要解释业务流程。

厂商称实施通常 4-6 周，取决于复杂度及历史数据量，不能当统一交付保证。

替换记录系统涉及历史余额与交易迁移、对象映射、收入政策、审批及报表核对；需要用平行关账确认自动化后数值完整。

#### 价格与合同范围

询价

官方帮助中心明确不按席位或收入收费，而按所用功能和企业复杂度报价；未公开固定美元金额与计费周期。

[Rillet Help Center](https://www.rillet.com/help-center)

#### 说明性使用例

一家 SaaS 公司在 CRM 签订年度合同：合同同步后形成收入模式，会计复核服务期等细节并批准；收入及递延支持计划进入 Rillet，总账和客户视图更新。月底 Aura 提示可能遗漏的计提，审批者核查提案后决定是否发布。

明确显示合同→计划→分录→报表的关系，并区分规则生成和模型建议。

[Advanced Revenue Recognition](https://www.rillet.com/product/advanced-revenue-recognition) · [Aura AI by Rillet](https://www.rillet.com/product/aura-ai) · [AI you can audit](https://www.rillet.com/product/security-and-permissions)

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**Smartcar**：厂商案例称单人财务团队每月关账节省 5 个以上工作日，前系统是 QuickBooks。

官方客户案例，未独立验证

[Smartcar's Director of Finance cut 5+ days from monthly close](https://www.rillet.com/case-studies/smartcars-director-of-finance-cut-5-days-from-the-teams-monthly-close-as-a-finance-team-of-one)

**Smartcar**：同页报告 DSO 从约 50 天降至约 30 天；该成果含催收与流程变化，不能全归因于 AI。

官方客户案例，未独立验证

[Smartcar's Director of Finance cut 5+ days from monthly close](https://www.rillet.com/case-studies/smartcars-director-of-finance-cut-5-days-from-the-teams-monthly-close-as-a-finance-team-of-one)

#### 关键边界与待确认项

- “零日关账”是定位目标，客户仍对账并检查自动化；公开页面不构成所有客户零日交付证据。
- 原生连接、定时连接和通用平台覆盖应拆开确认；历史回填、重复记录识别和故障恢复未实测。
- 安全页的 Agent 未批准不入账，与收入计划自动过账描述需按实际工作类型核对，不能相互替代。
- 具体中国会计准则、税票、税务与银行覆盖未由本轮页面证明。
- 无可比较的统一 AI 错误率、审核耗时、实施总费用及公开套餐金额。

#### 设计启示  分析判断

- 分析判断：拥有记录系统时，产品应把来源对象、支持计划、分录与报告串在同一导航关系中，帮助用户检查修改的连带影响。 GL 与收入页面的对象驱动流程。
- 分析判断：会改变账务的 AI 提案应有清晰的金额、依据、审批状态与批准人，不只返回聊天文字。 Aura 的 Propose & Approve。
- 分析判断：对外展示既要说明自动化范围，也要展示实际关账工时与审核负担，避免用零日口号取代操作证据。 定位与 Smartcar 案例仍有人员检查。

### 06 Numeric  以关账和交易分析切入，再扩展到财务数据平台

**服务谁**：会计主管和 Controller 推动；会计人员准备、调查与复核；CFO 使用财务结果。FDP 路线还涉及财务系统与数据人员。

**接手的工作**：把交易、支持资料、关账任务和差异解释连接起来；保留 ERP 时帮助完成关账，采用 FDP 时从完整业务记录生成账务与报表。

**开始条件**：期间关账，或日常交易检查

[Numeric 当前产品与路线](https://www.numeric.io/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | ERP 交易、总账余额、银行流水、支持底稿；FDP 另接合同、发票和用量等完整业务对象 |
| 02 处理 | 比对与监控、匹配现金、定位期间差异、起草 Flux 解释；FDP 用会计规则生成分录和账务计划 |
| 03 复核 | 会计人员补充原因、调查例外、编辑并批准分析；现金分录经过审批；MCP 按用户权限和工具配置运行 |
| 04 产出与去向 | 已复核的对账、差异说明、报告和审计记录；现金模块明确支持批准后发布分录至 NetSuite |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 关账与对账 | 组织责任、截止日期、支持资料和复核；比对余额<br>[官方依据](https://www.numeric.io/product/close-management) | 任务状态、账户差异与签核证据 |
| 交易监控 | 持续检查缺失字段、大额分录等条件<br>[官方依据](https://www.numeric.io/product/transaction-monitors) | 需要处理的交易与提醒 |
| Flux 与自定义报告 | 下钻差异，结合交易和外部资料起草解释<br>[官方依据](https://www.numeric.io/product/variance-analysis) | 可核查的解释初稿与财务报告 |
| 现金管理 | 规则匹配银行与账务，起草分录并批准发布<br>[官方依据](https://www.numeric.io/product/cash-management) | 匹配结果、例外、NetSuite 分录和现金视图 |
| 计费与收入确认 | 合同和用量驱动发票、收入分摊和合同修改处理<br>[官方依据](https://www.numeric.io/product/billing-and-revenue) | 发票、收入计划、递延与未开票收入 |
| FDP 完整平台 | 保存业务对象，以会计逻辑派生借贷记录<br>[官方依据](https://www.numeric.io/financial-data-platform) | 账务系统、业务维度报告和待审核事项 |

#### AI 与复核

Flux 从交易与补充资料生成解释，人员编辑批准；现金匹配结合规则及 AI 建议。MCP 让外部 AI 读取数据、更新任务或说明，继承用户权限，管理员可限制只读或要求写操作批准，每次操作留记录。不要将生成初稿、规则算账和工具写回统一理解为无人记账。

[Numeric MCP 权限与操作](https://help.numeric.io/articles/5446387341-what-is-the-numeric-mcp)

#### 数据与集成

两种路线的区别在数据底座：叠加模式读取既有 ERP 的账务；FDP 保存合同、账单、发票等记录，并派生会计结果。不是所有客户都拥有相同能力。NetSuite Traditional Sync 与 Warehouse Sync 在维度、层级及接入要求上不同，需按连接方案核验。

#### 关键特性与比较位置

同一工作环境关联责任人、交易、资料、分析与审计；允许从关账模块逐步扩展，FDP 路线进一步把业务背景保留到财务结果。App Studio 与 Agentic Subledgers 明确限于 ERP Replacement。

#### 采用与实施

先明确采用现有 ERP 模块还是迁移 FDP；再确认实体、账户、维度、银行连接、规则与复核角色。FDP 涉及数据迁移和会计逻辑，不能按轻量关账工具估算实施工作。

#### 价格与合同范围

当前官方按交易量、席位及业务情况询价，没有统一公开金额；实施与迁移范围需前置约定。关账与分析、现金、计费与收入可组合，完整平台另有边界。

[Numeric 模块与定价](https://www.numeric.io/pricing)

#### 说明性使用例

说明性推演：工资费用上涨时，先找到相关交易，补入 HR 人员与奖金资料，再起草解释；重复计提形成待处理事项，修正并刷新后由复核人批准。此流程是依据公开功能设计的验证用例，未在真实账户执行。

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**Brex**：厂商案例称关账由 6 个工作日缩短到 4 个工作日

关账清单、Flux 与共建的现金模块共同作用；不能全部归因于 AI，也不是统一承诺

[Numeric Brex 客户案例](https://www.numeric.io/cases/brex-x-numeric)

**Built**：厂商案例称计费与收入工作释放约 2 个全职人员的工作容量

2026 年初迁入 FDP 并连接源业务记录；这是工作容量口径，不等于裁员或所有客户的人员收益

[Numeric Built 客户案例](https://www.numeric.io/cases/numeric-x-built)

#### 关键边界与待确认项

- ERP 支持名单不能证明所有字段、币种、实体与写回一致；现金写回公开明确的是 NetSuite。
- 匹配率和解释准确性没有本报告独立测试；缺少业务背景时仍需补充。
- ASC 606 功能说明不能证明中国税票、税务和当地准则覆盖。
- 替换 ERP 范围需逐项确认，不能从名称推断包含生产、库存或全部企业业务。

#### 设计启示  分析判断

- 可借鉴按账户或差异建立证据链，把 AI 解释放到可下钻、可编辑、可批准的工作单元中。
- 模块切入和记录系统替换应提供不同接入路径、承诺和实施计划。
- 让异常处理与后续数据刷新相连，比仅展示一段解释更有产品价值。

### 07 Pigment  把业务数据、假设和计划模型连接起来，支持预测、情景决策与合并分析。

**服务谁**：CFO、FP&A 及业务负责人；组织涉及财务、销售、HR 与供应链。

建模者维护结构与公式，业务部门输入假设和目标，管理层查看计划及结果；合并团队处理抵销、调整和法定报告。

**接手的工作**：将 ERP、CRM 等实际数据与部门计划放入可重算的经营模型，比较实际与目标，预测和模拟不同决策，并协同输出计划及报表。现有 ERP 提供实际数据；公开页面另外支持合并调整分录，不应把它写成完全不涉及会计。

**开始条件**：预算编制、滚动预测、管理层情景问题、合并周期，或定时运行 Analyst Mission。

[Agentic AI for enterprise business planning](https://www.pigment.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | ERP 实际数据、收入与人事信息、业务维度、预算假设及用户定义的模型逻辑。 |
| 02 处理 | 模型按维度和公式计算计划与差异；Modeler 可创建/调整结构；Analyst 下钻、解释驱动并生成报告；合并模块另处理汇率与内部抵销。 |
| 03 复核 | 用户确认假设、逻辑与建议。Modeler 的 Plan & Build 有检查点，可设 Auto-accept，删除仍需确认；Ask 模式不改模型。不能概括为所有 Agent 都只聊天或所有操作必经逐次审批。 |
| 04 产出与去向 | 写入 Pigment 模型、指标和视图；Analyst 可定时把报告写至 Text Metric/Board，并导出 PDF。合并结果含调整分录及财务报表；本轮没有证明其承担日常总账 ERP 或自动向全部外部系统回写。 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 财务与跨部门计划 | 组织预算、预测及 HR、销售、供应链等业务计划。<br>[官方依据](https://www.pigment.com/) | 关联假设、目标与经营视图。 |
| 情景与绩效分析 | 改变假设并比较财务结果、差异与驱动。<br>[官方依据](https://www.pigment.com/) | 情景结果与决策讨论依据；具体模型需配置。 |
| 财务合并 | 导入实际数据，转换币种、抵销内部交易并处理合并调整。<br>[官方依据](https://www.pigment.com/use-case/financial-consolidation) | 合并报表、控制与记录。 |
| Modeler Agent | 创建和修改维度、指标、公式、视图与 Board。<br>[官方依据](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent) | 永久模型变更，按发起人记入历史。 |
| Analyst Agent 与 Missions | 自然语言下钻分析，并保存为可重复的报告任务。<br>[官方依据](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) | 可编辑的文本/图表报告、定时输出与历史。 |
| Frames 与外部 AI 接口 | 当前主页介绍在实时模型上创建交互界面，并通过 MCP 连接外部 AI。<br>[官方依据](https://www.pigment.com/) | 模型上的显示/输入界面；不推断能替代全部内置分析。 |

#### AI 与复核

Modeler 建模和维护；Analyst 下钻及重复报告；当前合并页另介绍支持控制解释的 Consolidation Agent。主页 Planner Agent 仍标 Coming soon，不能按已上线能力描述。

建模 Agent 可实际写模型，并支持自动接受部分动作；删除必须批准。Analyst 权限取决于运行者，报告共享时不重新检查浏览者的原数据权限，导出到 Text Metric 后需另配访问权。

Missions 是计划/报告自动化证据，不证明 AI 自行执行招聘、采购、支付或总账记账。预测与建议质量仍取决于数据、模型和假设。

[Agentic AI for enterprise business planning](https://www.pigment.com/) · [Run the Modeler Agent - updated 2026-09-30](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent) · [Run the Analyst Agent - updated 2026-07-22](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) · [Financial consolidation in Pigment](https://www.pigment.com/use-case/financial-consolidation)

#### 数据与集成

模型以 Dimension/Transaction Lists、Metrics、Properties 及公式关系组织，数据可以按业务维度重算；这是经营模型结构，而非 Rillet 式交易总账。

合并页列出 NetSuite、Sage Intacct、Salesforce、HubSpot、Stripe、Chargebee 的定时数据导入；Carta 案例实际列出 NetSuite、Workday、Google Sheets。

Modeler 变更进入 Application History 并归属发起人；Analyst Missions 有运行历史和报告预览。合并页面另强调审计日志与控制。

[Run the Modeler Agent - updated 2026-09-30](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent) · [Run the Analyst Agent - updated 2026-07-22](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) · [Financial consolidation in Pigment](https://www.pigment.com/use-case/financial-consolidation) · [Carta - French official customer story](https://www.pigment.com/customer-stories/carta)

#### 关键特性与比较位置

围绕多维经营模型而非会计分录组织产品，适合跨财务与业务部门共同解释目标和行动。

AI 同时服务模型构建与模型使用，用户既能询问数据也能让系统改结构；两种权限和风险应分开。

当前把计划、合并实际数据和报告连接，范围超出传统预算表，但仍需区分合并调整与日常账务记录。

#### 采用与实施

应梳理指标、部门维度、假设责任及数据接入。许可证按权限区分查看、输入和建模，角色配置也影响商业成本。

Carta 官方案例标注实施 12 周；它是个案，不能直接作为当前全部实施周期。

先实现一个预算/预测或合并模型，再验证计算与访问边界；Modeler 能省配置工作，但公开材料不证明无需业务建模和治理。

#### 价格与合同范围

询价

官方许可证页说明平台费、许可证数量和功能构成报价；许可证有 Explorer、Contributor、Editor，由权限决定。未公开统一金额。

当前 AI credits 按工作区和合同年度授予，周年日重置、未用完不结转；Agent 消耗随任务复杂度，Predictions 每条时间序列 0.1 credit。超额可限制功能，旧/定制合同另论。

[Pigment License Types - updated 2026-05-12](https://kb.pigment.com/docs/pigment-license-types) · [Manage your AI credits - updated 2026-09-17](https://kb.pigment.com/v1/docs/ai-credits)

#### 说明性使用例

FP&A 团队评估新增销售岗位：导入实际收入与人事资料，定义岗位成本和收入假设，Modeler 按人员、月份创建或修改模型；业务负责人核查假设，再比较现金与利润情景；Analyst 将每周实际对计划分析保存为 Mission。

界面同时显示假设、计算依赖、版本和结果，让讨论围绕经营选择，并控制共享报告的可见范围。

[Run the Modeler Agent - updated 2026-09-30](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent) · [Run the Analyst Agent - updated 2026-07-22](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) · [Agentic AI for enterprise business planning](https://www.pigment.com/)

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**Carta**：所读官方法语案例页称每位成员每周 ARR 报告节省约 2 小时，初稿由 Analyst Agent 生成。

厂商客户案例，未独立验证

[Carta - French official customer story](https://www.pigment.com/customer-stories/carta)

**Carta**：同页称部门深入分析每月节省 10-15 小时；未给出完整投入/产出方法。

厂商客户案例，未独立验证

[Carta - French official customer story](https://www.pigment.com/customer-stories/carta)

#### 关键边界与待确认项

- 不能把计划平台的模型写入当作 ERP 入账；合并调整分录与原系统日常交易分录的责任范围需单独核对。
- 共享 Analyst 报告的权限不会自动随每个浏览者重算，输出层必须设计访问控制。
- Modeler 在 Test & Deploy 的 managed Applications 当前仅 Ask 模式，Build 可用范围受环境限制。
- 首页对 Carta 周 ARR 报告写 5 小时，所读法语案例正文写约 2 小时；本文件保留正文口径并记录差异，不混用。
- Planner Agent 当前仍在预告；AI 金额、配额、复杂度计费和真实模型准确性需合同及试点确认。

#### 设计启示  分析判断

- 分析判断：计划产品应以假设→公式依赖→情景→经营结果为主线，让使用者知道改变哪一项会影响哪些结果。 多维模型与 Modeler 结构修改。
- 分析判断：把建模 Agent 和分析 Agent 的动作范围分开，分别展示改模型、只读问答及重复报告的状态。 Modeler 永久修改与 Analyst Mission。
- 分析判断：执行权限与输出分享权限应分别设计；不能假定共享输出已继承原数据的访问限制，应按接收者另行配置输出权限。 Analyst 文档关于输出访问权的明确边界。

### 08 金蝶  以集团财务体系连接共享作业、核算、资金与报告

**服务谁**：集团 CFO、财务负责人及数字化/IT负责人；业务负责人和共享中心参与流程与数据标准建设。

业务报账人员、业务财务、共享费用/应收/应付/总账小组、出纳、集团预算与报表管理人员。角色并不共享同一处理权限。

由官方集团定位与工作流角色归纳。

**接手的工作**：把集团分散的财务作业、核算、资金与管理口径接入一个可共享、可组装的体系，支持标准化处理及集团资源配置。相比关账单点工具，ERP、业务单据及会计政策本身就是产品范围的一部分。

**开始条件**：业务发生后提报费用，或采购验收后申请应付/付款；月底进行集团账务和报表处理。以下工作链依据 2023 年官方财务共享方案归纳，当前 SKU 与配置须另行确认。

[Kingdee 官方全球首页](https://www.kingdee.com/global)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | 业务单据及附件、核算组织/账簿/科目/维度、企业会计政策、预算与支付信息。 |
| 02 处理 | 共享任务池按规则分派；可组合规则审核、AI风险审核及附件理解，按核算模板处理业务。 |
| 03 复核 | 业务部门与业务财务先审，共享人员检查合规性并可预览凭证；不是一切付款与入账均由模型自主批准。 |
| 04 产出与去向 | 审批通过后下推付款单，银企结算，按智能核算方案生成账务；结果进入集团报告。具体接口、失败重试和跨 ERP 写回必须以实施方案验证。 |

#### 金蝶产品线范围

金蝶云·星瀚在 2025 年升级为金蝶 AI 星瀚；V8.0 官方发布明确融合小K、Data Cloud 与苍穹 AI 平台。小K是跨业务场景的智能体品牌，不能视作一个只做财务的独立 SaaS。

星瀚：央国企及大型企业套件，本记录只主拆其财务云。

AI套件：面向大、中型企业的另一套件产品线。

金蝶云·星空：中型企业管理云；官网存在星空与 AI 星空两种命名，不把星空功能直接归入星瀚。

AI星辰：小型、小微企业财税及经营 SaaS。

AI苍穹：企业级 AI / PaaS 技术平台，与财务业务应用分层。

灵基（Lingee）：2026 年发布的企业智能体操作系统，单独列在官网产品导航中；其内部实践不等于星瀚全部客户的能力或成效。

[金蝶 AI 财务云](https://www.kingdee.com/products/financial_cloud.html) · [金蝶 AI 星瀚 V8.0 重磅发布](https://www.kingdee.com/resources/articles/1445843916024042177) · [金蝶云·星瀚财务共享：智能驱动，赋能业务](https://www.kingdee.com/article/1737774452831248385.html) · [金蝶的财务部，怎么用灵基AI？以AI原生重塑财务生产力](https://www.kingdee.com/resources/articles/1554808863620117377)

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 财务会计与核算 | 总账及账簿/维度控制；会计政策驱动的凭证生成与期末处理。不要把模板生成凭证一律叫大模型记账。<br>[官方依据](https://www.kingdee.com/products/financial_cloud.html) | 凭证、账簿与期末结果 |
| 财务中台/共享 | 统一接单与共享作业，使专业小组承担审核、处理和质量管理。<br>[官方依据](https://www.kingdee.com/products/cosmic_finance.html) | 共享任务、审核状态与处理证据 |
| 企业绩效管理 | 包含合并报表与全面预算；预算从目标、编制审批到执行、调整及分析，合并使用多维数据能力。<br>[官方依据](https://www.kingdee.com/products/cosmic_finance.html) | 预算、合并报表及分析 |
| 司库 | 资金及金融资源管理是财务云独立领域，与共享付款环节相连接。<br>[官方依据](https://www.kingdee.com/products/financial_cloud.html) | 资金与结算信息 |
| 管理会计/分析 | 经营分析与资源配置属于集团财务体系；AI可辅助填单、审单、报告和分析。<br>[官方依据](https://www.kingdee.com/products/financial_cloud.html) | 经营分析与资源配置信息 |
| 税、票、费用与档案 | 财务产品目录包括税务、发票、人人费用及电子档案；是否购买与实施并非由套件名称自动决定。<br>[官方依据](https://www.kingdee.com/products/financial_cloud.html) | 税票、费用及档案记录 |

#### AI 与复核

小K在星瀚 V8.0 的财税等管理场景中提供增强能力；官方发布的场景数属于全套件，不能全部算作财务功能。

共享审核明确区分规则引擎、AI+大数据、GPT附件审核；后者理解非结构化附件并提示重点，辅助财务识别风险。

灵基是独立 AIOS 对照：官方内部实践展示 HR取数、按规则计提部门活动费、生成凭证并写入 ERP；这里只证明该具体内部场景。

公开流程保留业务审核和人工检查。确定性核算、派单及支付控制与模型理解应分别评估。灵基官方强调权限、规则和责任约束，但通用产品权限矩阵、每项任务的审批阈值及回滚机制仍需演示。

[金蝶 AI 星瀚 V8.0 重磅发布](https://www.kingdee.com/resources/articles/1445843916024042177) · [金蝶云·星瀚财务共享：智能驱动，赋能业务](https://www.kingdee.com/article/1737774452831248385.html) · [金蝶的财务部，怎么用灵基AI？以AI原生重塑财务生产力](https://www.kingdee.com/resources/articles/1554808863620117377)

#### 数据与集成

组织、会计账簿、科目、币别与核算维度承载账务口径；数据并非只有一份上传的表格。V8.0 技术资料记录了按账簿设置公共维度、查询/导出权限分开、已结账期间逆操作控制等细节。

星瀚基于苍穹平台，发布版又连接 Data Cloud。可组装财务中台支持与业务、核算、税务、资金搭配。集团采用星瀚与 EAS 共存的案例，说明不是所有上线都要求一次替换全部旧系统。

可成为新的 ERP/财务主干，也可分阶段接入集团已有体系。与 Numeric 的关账/分析叠加方案相比实施范围更广；Numeric FDP 的记录系统替换路线应另行对照。

[金蝶 AI 星瀚 V8.0 重磅发布](https://www.kingdee.com/resources/articles/1445843916024042177) · [金蝶云·星瀚财务共享：智能驱动，赋能业务](https://www.kingdee.com/article/1737774452831248385.html) · [携手迈向世界一流！金蝶云·星瀚标杆客户案例大集结](https://www.kingdee.com/resources/articles/1396813829714935745) · [【金蝶云·星瀚V8.0】新特性-财务云](https://vip.kingdee.com/article/769491123282183168)

#### 关键特性与比较位置

大型集团、共享财务、EPM、司库与中国企业管理情境是主要覆盖面。

优势候选是从业务事件到集团报表的统一控制与口径，而不是聊天入口。其复杂性也意味着上线成本与收益要按所选模块估算，不能与轻量关账工具直接比订阅价。

[金蝶 AI 财务云](https://www.kingdee.com/products/financial_cloud.html) · [金蝶 AI 星瀚财务云](https://www.kingdee.com/products/cosmic_finance.html)

#### 采用与实施

2023 年共享解决方案说明苍穹底座适配公有云、私有云、混合云及国产信创环境；这是当时的方案说明，现行部署资格需重新确认。

分析判断：多组织主数据、会计政策、流程责任、银行接口和历史数据决定实施范围；应先选一条可验证业务链，再确认集团扩展，不宜假设即开即用。

#### 价格与合同范围

询价

截至研究日，已读官网首页、产品和方案资料未提供星瀚财务云的现行完整套餐/单位/周期价表；官方入口是预约演示或联系销售。未使用代理商报价、星辰/星空价格或应用市场插件价格替代星瀚价格。

分析建议：分别索取业务模块、组织/用户授权、部署、实施迁移、银行及外围接口、AI用量、运维升级费用。

[Kingdee 官方全球首页](https://www.kingdee.com/global) · [金蝶 AI 星瀚财务云](https://www.kingdee.com/products/cosmic_finance.html)

#### 说明性使用例

集团总部需要在月结前完成一家子公司的采购付款：验收单与发票进入共享池，规则检查金额/预算，模型读取附件并标出疑点，共享应付人员检查并预览凭证，审批后由出纳结算，再进入核算及集团报表。

分别制造币种不一致、漏附件、已结账期间调账和重复付款；检查规则拦截、AI建议、人工权限及失败反馈是否各有证据，而不是仅评估回复是否流畅。

[金蝶云·星瀚财务共享：智能驱动，赋能业务](https://www.kingdee.com/article/1737774452831248385.html) · [【金蝶云·星瀚V8.0】新特性-财务云](https://vip.kingdee.com/article/769491123282183168)

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**招商局集团**：官方 2024 案例介绍：把星瀚与 EAS 财务系统引入招商云平台，构建财务共享、合并报表与司库应用。

两套系统共同建设的集团数字化案例；非独立小K或灵基的因果效果，原文未在该段提供统一量化基准。

[携手迈向世界一流！金蝶云·星瀚标杆客户案例大集结](https://www.kingdee.com/resources/articles/1396813829714935745)

#### 关键边界与待确认项

- 星瀚、小K、苍穹、灵基分别处于应用、智能体、平台与AIOS层；必须向厂商问清合同中的实际 SKU 和上线能力。
- 当前菜单仍出现“金蝶云·星空”，部分页面使用“AI星空”；保留官方命名差异，避免静态产品表误导。
- 中国主站部分产品页全文获取失败，已读官方索引正文；不把未展示的页面或下载材料算作已验证。
- 公开资料未给出财务 AI 在陌生企业数据上的误报/漏报分母、结论证据质量或所有写回任务的审计日志示例。
- V8.0 社区技术文为官方域名托管的作者分享，适合揭示系统复杂性，不用其单独承诺标准版本全部功能。

#### 设计启示  分析判断

- 分析判断：产品设计应先把“业务对象-账务口径-责任人-状态”串起来，模型输出才能进入生产流程。
- 分析判断：单据、凭证与支付分别展示风险依据及审批责任；把自动化、AI建议、人工签核显式分开。
- 分析判断：可借鉴灵基的任务入口，但MVP应以一个有结果回写与异常处理的任务为单位，而不是同时仿造全集团 ERP。

### 09 合思  连接因公消费、审核、付款、ERP 凭证与电子档案

**服务谁**：CFO、财务负责人/共享中心、采购或商旅管理负责人；IT与内控人员影响集成及部署。

员工提单和消费，主管/项目负责人审批，财务审核、出纳付款，档案及经营管理人员查阅。

由产品工作流及多级授权角色归纳。

**接手的工作**：把因公支出从申请、发生、票据、审核、付款，到 ERP 凭证和归档接成一条证据链；由事后人工报销转向消费过程管控。AI审核是嵌入这条链的具体能力，价值不能仅用 OCR 识别速度代表。

**开始条件**：员工出差/日常费用申请，或采购合同及付款计划触发报账。

[合思官方首页](https://hosecloud.com/)

| 步骤 | 工作内容 |
| --- | --- |
| 01 输入 | 消费订单、发票/水单/非标附件、预算与费用规则、合同台账、核算和审批组织。 |
| 02 处理 | 按制度进行预算与差标校验；票据采集、查验及费用关联；AI读取附件并给出风险建议，对公流程按票款/合同关系处理。 |
| 03 复核 | 按分级授权提交审批，财务查看风险点、依据和处理建议；保留人机共审，异常与最终付款责任不能由宣传语替代。 |
| 04 产出与去向 | 批准单据驱动付款；银企接口回传进度/回单；字段映射生成 ERP 凭证并回写凭证号；凭证、票据、回单进入档案，费用进入经营分析。 |

#### 模块及交付结果

| 模块 | 具体工作 | 产出 |
| --- | --- | --- |
| 费控及报销 | 移动申请、借款、报销、多级授权；预算与费用标准在事前、事中、事后执行。<br>[官方依据](https://hosecloud.com/expense.html) | 已审批费用及财务单据 |
| 商旅/企业消费 | 商城与易商卡衔接消费数据，覆盖企业统一结算的无需报销场景。它依赖消费资源与制度配置，不是所有费用都自动消失。<br>[官方依据](https://hosecloud.com/) | 消费订单与结算资料 |
| 发票 | 数电票采集、查验、查重、复核及电子源文件管理，与报销、入账和归档相连。票据查验与OCR需和大模型判断分开。<br>[官方依据](https://hosecloud.com/expense.html) | 已查验票据和电子原文件 |
| 对公付款 | 合同模板、变更、付款计划、收票和应付台账协同；支持先款后票、先票后款及供应商对账。<br>[官方依据](https://hosecloud.com/) | 应付台账、付款计划与支付状态 |
| 电子会计档案 | 接收结构化数据及原文件，按可视化关联规则组档，进行四性/业务检测，并建立凭证与原始资料的穿透关系。<br>[官方依据](https://hosecloud.com/archiving.html) | 关联档案与凭证原件关系 |
| BI经营分析 | 文件/数据库/API接入数据，按项目和合同配置指标，看板支持钻取，分析费用及全链路数字化程度。常规报表与自动订阅不自动等于生成式AI。<br>[官方依据](https://www.hosecloud.com/bi/bi.html) | 经营看板与钻取结果 |
| AI财务审核专家 | 自然语言规则、非标材料理解与跨单据校验，输出风险依据/建议，定位人机共审。<br>[官方依据](https://hosecloud.com/aifinancialapproval.html) | 风险点、依据和处理建议 |

#### AI 与复核

AI审核专家可通过自然语言编辑规则并导入制度，以真实历史数据离线调优；理解非标凭证、费用事项与类型、发票/支付水单/事前事项之间的关系。

结果中展示风险点、依据和建议；主页还列出填单、海外票据、商旅及档案智能体，但本记录不以智能体数量推断所有模块成熟度。

付款产品页明确 AI提取合同信息及风险审查；这是辅助判断，不能推导为自动法律结论或付款批准。

预算额度、审批分支、科目映射、凭证生成、档案组装等存在明确规则引擎；AI补充材料理解及建议。官方未公开统一的置信度阈值/自动放行矩阵或审单准确率分母。

[合思官方首页](https://hosecloud.com/) · [合思费控](https://hosecloud.com/expense.html) · [合思付款](https://www.hosecloud.com/ap/) · [合思档案](https://hosecloud.com/archiving.html) · [AI财务审核专家](https://hosecloud.com/aifinancialapproval.html)

#### 数据与集成

单据/费用、组织角色、项目台账、合同和付款计划、发票、会计凭证及回单是关键对象；以对象关系还原支出证据，而不是只保存报销PDF。

官方连接方案明确 ERP 字段映射与凭证号回写、OpenAPI 双向同步、组织/权限及单点登录联通；银企付款后回单回传。具体银行、ERP版本和自研接口须逐项确认。

主路径是接入现有 ERP 后自动生成凭证，属于费用/支付/档案层叠加；公开资料不足以认定它完整替代集团总账、制造成本或合并报表 ERP。

[合思费控](https://hosecloud.com/expense.html) · [合思付款](https://www.hosecloud.com/ap/) · [合思档案](https://hosecloud.com/archiving.html) · [合思广泛连接解决方案](https://hosecloud.com/solutionsr/connect.html)

#### 关键特性与比较位置

从消费资源、前置费控，延伸到票、款、凭证及档案；突出广泛连接和无需报销。

相对关账分析工具，它更靠近支出发生和审批现场；消费/银行/ERP连接形成真实闭环，可能比单独审票更减少人员交接。适用于流程分散的连锁、共享中心及跨组织支出情境。

[合思官方首页](https://hosecloud.com/) · [合思广泛连接解决方案](https://hosecloud.com/solutionsr/connect.html) · [合思×新发现：120+门店，0增人，AI智能审核破解连锁扩张财务困局](https://hosecloud.com/cases/76.html)

#### 采用与实施

AI审核产品页支持全私有化本地部署及企业专属规则，不把这一选项自动外推到所有消费和商旅模块。

分析判断：必须梳理预算/差标、部门项目与合同台账、审批人、ERP映射和银行权限；用真实附件做离线验收。客户新发现案例还说明纸质附件拍照会影响识别，取消重复打印后才改善数据输入。

#### 价格与合同范围

询价

现行核心产品页以免费试用/预约演示为入口，没有可直接比较的现行单位、套餐与周期完整价格。需要核实费控、消费服务、档案、接口、AI审核及部署分别如何计费。

[合思官方首页](https://hosecloud.com/) · [合思费控](https://hosecloud.com/expense.html) · [AI财务审核专家](https://hosecloud.com/aifinancialapproval.html)

#### 说明性使用例

门店同时提报采购食材、维修费和运费：把附件、申请、合同及发票关联到单据，规则判断额度，AI辅助分类并比较材料内容，财务检查异常后审批；批准付款和生成ERP凭证，最后以档案链穿透到原始资料。

植入费用类目错误、同票重复使用、无票额度累计超限及已付款但回单缺失，检查系统在哪一步阻断、谁能覆盖、哪些金额/字段被写回。不能只用一张干净发票验证整个产品。

[合思费控](https://hosecloud.com/expense.html) · [合思档案](https://hosecloud.com/archiving.html) · [合思广泛连接解决方案](https://hosecloud.com/solutionsr/connect.html) · [合思×新发现：120+门店，0增人，AI智能审核破解连锁扩张财务困局](https://hosecloud.com/cases/76.html)

#### 客户案例  厂商披露

这些结果未独立验证，也不能全部归因于 AI。

**新发现餐饮**：厂商案例原口径：审核周期从“超1个月”压缩至“1周内”。

120余门店、3名财务审核人员，餐饮场景定制AI审核；不是所有企业的平均结果。

[合思×新发现：120+门店，0增人，AI智能审核破解连锁扩张财务困局](https://hosecloud.com/cases/76.html)

**新发现餐饮**：同页首屏称年节省人力成本20万元；正文写15-20万元，源自扩张中无需增加1名审核人员的方案。

保留首屏与正文的口径差异，不改写成已经裁员或现金支出净节省；未见独立实验或完整成本计算。

[合思×新发现：120+门店，0增人，AI智能审核破解连锁扩张财务困局](https://hosecloud.com/cases/76.html)

#### 关键边界与待确认项

- 官网首页智能体数量在不同段落出现7与8，规模数字亦可能受页面动画/抓取影响；本记录不用这些数字做竞争力依据。
- 规则校验、税务查验、OCR与大模型材料判断属于不同技术，营销中的智能一词不足以证明AI。
- 数电票与档案本地化能力应连同电子原文件、验签及查阅权限一起验收；厂商合规宣传不等于对具体企业法律合规的结论。
- AI准确率、两周上线、风险拦截等页面概括数字未给统一口径，不用作横向实测排名。
- ERP写回的失败重试、冲正、权限分离、银行支付签核以及AI自动放行阈值需要实际配置与日志验证。

#### 设计启示  分析判断

- 分析判断：从一笔支出展示申请、消费、票、审批、款、凭证、档案的关系，让用户知道哪份材料缺失及由谁补齐。
- 分析判断：风险提示应给出规则/制度依据、关联材料位置与处理动作；把AI建议转成可复核任务。
- 分析判断：将输入质量和组织规则作为产品的一部分，以离线真实单据测试校准，再逐步扩展自动化范围。
- 分析判断：国内产品设计需要保留票据原件、多人授权、银行签核和ERP回写状态，不能照搬海外纯总账分析界面。

## 哪些样本应该放在一起比较

### FloQast 与 Numeric 适合比较关账如何完成

共同入口是任务、账户、支持资料、差异和复核。比较时让两家完成同一次关账：账户对不上时如何追到交易，AI 解释能否显示证据，准备和复核怎样签核，ERP 修正后状态怎样更新。Numeric FDP 的记录系统替换要另做比较，不能混入关账模块的价格和实施范围。

### Rillet 与 Numeric FDP 适合比较新的账务底座

重点从“读了多少数据”转为“保存什么业务对象、怎样生成并修正会计结果”。考察实体、币种、期间锁定、分录与业务源关联、历史迁移、合并和收入计划。金蝶星瀚提供大型集团和更广业财体系的对照；客户复杂度、所选模块和迁移边界应先对齐。

### Basis 与各家的 Agent 适合比较可委派的工作

可委派对象应是一个具有输入、可验收结果和责任人的任务。用同一份原始资料检查取数、计算、工作底稿、写回提案及错误处理。Basis、FloQast Transform、Ramp Stack、Rillet Aura、Numeric MCP 的产品机制和执行范围不同，不能只比较聊天界面或模型回答。

### Ramp 与合思适合比较支出到会计的证据链

两家都靠近员工、购买、单据、审批和支付。可以比较消费信息是否一次采集、风险是否在付款前出现、会计字段和材料是否一起回到 ERP。Ramp 的发卡和金融渠道，合思的票档与本地连接分别是重要环境条件，不能直接照搬价格或流程。

### HighRadius 适合研究高交易量的专业流程

用收款与未结发票核销、短付争议和催收的连续状态观察价值。产品设计可借鉴跨系统工作单元、业务原因码、例外路由与传输结果；是否需要整套企业财务范围，应按目标客户和交易复杂度判断。

### Pigment 适合研究财务数据如何进入决策

比较重点是驱动模型、业务协作、情景与预测，以及当前提供的集团合并。Numeric 等工具的实际财务变化解释，与 Pigment 的计划模型修改属于不同结果。需分别评估计划版本、假设来源、模型变更和共享输出权限。

## AI 执行与人工审批的关键区别

审批要看**具体动作**：准备材料、修改模型、安排付款、发布分录和写回 ERP 不是同一权限。以下均来自公开产品或操作说明，未在登录账户验证；“待确认”表示本次证据不足，不能读成产品一定没有该能力。

| 产品 | AI 接手的工作 | 是否实际执行 | 人工与控制边界 |
| --- | --- | --- | --- |
| Ramp | 编码、AP 资料理解；Stack 准备会计工作 | 合格卡交易可自动入队及夜间同步；Ready 与 Sync 分开启用 | 金额/资料/政策/置信度限制，异常交人；AI 不覆盖人员或规则填值<br>[官方依据](https://support.ramp.com/ramp-accounting-agent-enablement-daily-use-admin-guide) |
| HighRadius | 付款说明、核销、短付与缺资料跟进 | 核销结果可通过 API/文件进入 ERP；例外 Agent 有 Assisted 类型 | 按容差与业务码配置；具体审批、失败和回滚需演示<br>[官方依据](https://www.highradius.com/product/cash-application-automation/) |
| FloQast | 匹配、底稿、分录与可复用 Agent | 公开说明最终入账需要人工批准 | 准备人不能审自己的分录，批准后锁定，保留支持与审批记录<br>[官方依据](https://www.floqast.com/close-ai/products/journal-entry-management)<br>[FloQast 当前主页](https://www.floqast.com/) |
| Basis | 分类、底稿、分录、税务与审计准备 | CAS 高置信度交易可推送；Small Firms 分录先待审；企业会计页明确已批准分录写回 | 自动推送阈值、关闭开关与职责隔离需按具体流程确认<br>[官方依据](https://www.getbasis.ai/solutions/cas-and-advisory)<br>[Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms)<br>[Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting) |
| Rillet | Aura 查账、异常、计提与工作流提案 | Aura Agent 先提案，人工批准后进入 Rillet 账务 | 金额路由、角色和期间锁定留痕；规则支持计划另行区分<br>[官方依据](https://www.rillet.com/product/security-and-permissions) |
| Numeric | Flux 解释、匹配辅助、MCP 工具操作 | Flux 编辑批准；现金批准发布；MCP 按用户及工具配置读写 | 可只读或要求写操作批准；FDP 规则核算与 AI 解释分开看<br>[官方依据](https://help.numeric.io/articles/5446387341-what-is-the-numeric-mcp)<br>[Numeric Flux Analysis](https://www.numeric.io/product/variance-analysis)<br>[Numeric Cash Management](https://www.numeric.io/product/cash-management) |
| Pigment | Modeler 改模型；Analyst 分析与 Mission 报告 | 模型可永久修改，Plan & Build 可 Auto-accept；删除需确认 | 输出报告需单独设置共享权限；Planner 仍为预告<br>[官方依据](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent)<br>[Agentic AI for enterprise business planning](https://www.pigment.com/)<br>[Run the Analyst Agent - updated 2026-07-22](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) |
| 金蝶 | 小K与共享附件理解、风险辅助；灵基另属 AIOS | 共享链保留业务与财务审核，规则驱动核算与支付流程 | 通用 AI 阈值/回滚需确认；内部灵基实践不能当星瀚通用控制<br>[官方依据](https://www.kingdee.com/article/1737774452831248385.html) |
| 合思 | 非标材料理解、跨单据风险建议、合同提取 | 人机共审，分级授权后付款并按映射生成 ERP 凭证 | 风险依据可复核；统一自动放行阈值与银行签核需验证<br>[官方依据](https://hosecloud.com/aifinancialapproval.html) |

## 价格模型与实施工作量需要一起看

公开订阅金额只能作为商业模式线索。报价还受模块、企业复杂度、连接、部署和实施影响；表内“询价”表示本次已读页面未提供可直接比较的完整现行价表，并不表示免费。不能把用户月费与结果分成或 ERP 迁移项目费直接换成同一排名。

| 产品 | 已读公开定价 | 范围与计费条件 | 实施重点 |
| --- | --- | --- | --- |
| Ramp | Free $0/用户/月；Plus 页面显示 $15/用户/月＋平台费；Enterprise 询价<br>[官方依据](https://ramp.com/pricing) | 年付可省20%；采购另加购；Stack长期价格未核验 | 审批/供应商/实体/ERP 配置；发卡与金融服务地区资格 |
| HighRadius | 询价；年度 SaaS 说明与 Outcome-Based Pricing 并存<br>[官方依据](https://www.highradius.com/about/news/highradius-launches-outcome-based-pricing-for-ocfo-software/) | 结果付费宣传零实施费、上线前零订阅，之后收益分成；比例及适用合同未公开 | ERP/银行/门户、业务码与 KPI 基线，复杂个案30周不作统一周期 |
| FloQast | 按组织需求、范围和规模询价；官网称不按用户收费<br>[官方依据](https://www.floqast.com/pricing) | Close Management、Close AI、Risk & Compliance 范围不同 | 清单/账户/模板/审批配置，Agent 在自身资料上测试 |
| Basis | 询价；所读官网未给公开金额与完整计费规则<br>[官方依据](https://www.getbasis.ai/) | 部署团队学习客户方法；不使用同名产品的价格 | 客户政策、映射、Procedures、复核标准及连接写权 |
| Rillet | 按功能与复杂度询价；官网称不按席位或收入收费<br>[官方依据](https://www.rillet.com/help-center) | 厂商称通常4-6周，取决于复杂度及历史量；不作统一保证 | 迁移账务、合同政策、实体币种、期间与平行核对 |
| Numeric | 按交易量、席位和业务情况询价<br>[官方依据](https://www.numeric.io/pricing) | 模块叠加与 FDP 迁移的范围、成本分别约定 | ERP 深度、底稿/银行连接、规则；FDP 另含迁移与会计逻辑 |
| Pigment | 平台费＋按权限分型的许可证＋功能；询价<br>[官方依据](https://kb.pigment.com/docs/pigment-license-types) | 年度 AI credits，未用完不结转，复杂度影响消耗；旧合同可能不同 | 维度/驱动/模型、数据导入、权限；个案12周不作统一周期 |
| 金蝶 | 星瀚财务云询价；未取得现行完整价表<br>[官方依据](https://www.kingdee.com/products/cosmic_finance.html) | 模块、部署、授权、接口、AI用量及实施分别核价；不拿星辰价格替代 | 集团主数据、账簿、会计政策、共享、银行和历史数据 |
| 合思 | 询价；未取得完整现行套餐/单位/周期金额<br>[官方依据](https://hosecloud.com/aifinancialapproval.html) | 费控、消费、档案、接口、AI审核与部署分别核价；排除低可信旧报价 | 制度/审批/项目合同、ERP/银行映射、原票与历史单据调优 |

## 从竞品机制推导四个值得验证的设计方向

### 1 围绕例外建立工作台

将缺资料、匹配失败、跨期、重复记录和业务原因不明分别形成工作卡。每张卡显示金额、实体、期间、源单据、风险依据、责任人、下一动作与处理状态；动作执行后展示 ERP 或银行返回结果。Ramp 与 HighRadius 的资格和例外队列、FloQast 与 Numeric 的复核状态提供了可借鉴机制。

**需要验证**：用户是否能从发现问题走到修正与关闭；是否减少跨系统追问；自动处理后是否仍有未被呈现的残留问题。这是产品机会假设，不是已证明的市场空白。

### 2 把 AI 解释嵌入证据与复核

让每个原因关联到交易或业务材料，并区分确定金额、业务推断与仍缺的资料。用户可以修改原因、追问负责人、保存版本并批准。Numeric Flux 的上下文、FloQast 的支持工作簿、合思的风险依据说明了可信工作结果需要怎样呈现。

**需要验证**：最终批准前的人工修改量、找证据所用时间、关键遗漏和错误；仅衡量第一段草稿生成时间不能说明流程收益。

### 3 以可验收任务提供会计 Agent

从一个明确任务开始，例如预付支持底稿或银行未匹配交易。先提供示范输入、结果格式、测试样本和审核方式，再扩展到工具调用。把取数、计算、暂存、批准与发布分别呈现，保留重试、撤回和重复执行保护的设计。Basis、FloQast Transform 和 Ramp Stack 是主要机制样本；Rillet Aura 与 Numeric MCP 提供执行权边界对照。

**需要验证**：不同客户的科目、规则和来源变化后，任务是否仍可重用；审阅者能否理解计算与操作；工具失败是否停在正确位置。

### 4 在国内支出场景保留完整票款凭证关系

把合同、消费、发票原件、审批、支付回单、ERP 凭证和档案串到同一工作单元。模型辅助理解非标材料，确定性规则负责额度、状态与字段映射，最终责任体现在角色和操作中。合思适合研究前端费用链，金蝶星瀚适合研究共享与集团口径。

**需要验证**：缺票、红冲、部分付款、错科目和回单缺失时，是否仍能形成可追溯结果；本地化覆盖需逐项验收，不能只靠识票演示推断。

## 按目标工作选择重点拆解顺序

这是基于产品机制的研究顺序，不是市场排名或采购结论。定位前，应选择一个明确用户、一个现有痛点和一份实际产出；“财务 AI”这一名称本身不足以确定产品边界。

| 目标方向 | 先研究的样本 | 先要得到的产品结果 | 核心约束 |
| --- | --- | --- | --- |
| 企业关账与财务例外 | Numeric、FloQast，再看 Basis | 已核查差异、待办例外及复核证据 | 交易/底稿可接入，修正与刷新能闭环 |
| 会计事务所或外包工作 | Basis，再看 FloQast Transform 与 Ramp Stack | 可重用且可审核的会计任务 | 多客户隔离、工作底稿、工具权限和复核成本 |
| 国内费用审核与支出 | 合思、Ramp，再看金蝶共享 | 批准单据、支付状态、凭证及档案 | 票据原件、组织制度、银行和 ERP 接口 |
| 收款核销与催收 | HighRadius；Numeric 现金仅作银行/账务匹配子步骤对照 | 已核销收款、争议分工和更新的应收状态 | 付款说明、原因码、多系统映射及回写 |
| 新账务记录平台 | Rillet、Numeric FDP、金蝶星瀚 | 可维护的正式账簿和业务来源关系 | 迁移、期间控制、实体币种、会计规则和本地适配 |
| 计划与经营协作 | Pigment，再看金蝶 EPM | 可解释的模型、情景和集团结果 | 驱动定义、版本、假设、模型变更与输出权限 |

## 四组可复用的深度验证样本

以下是为后续实操建立的**说明性测试样本**，不是本报告已经跑过的试验，也不证明任一产品一定支持全部步骤。每家按适用模块运行，并使用同一份人工核查答案与失败条件。

### T01 支出到凭证与档案

**适用样本**：Ramp · 合思 · 金蝶；HighRadius AP 可作专项对照

**准备资料**：购买申请、合同/PO、收货资料、发票、费用规则、付款记录

**植入例外**：重复发票、缺收货、超标准、部分付款、付款成功但回单缺失

**期望结果**：说明问题与依据，交正确角色；批准后返回支付和 ERP 凭证状态，保持材料关联

**测量项**：总处理时间、补资料次数、审核修改量、写回失败及重复记录

### T02 工资变动与月结例外

**适用样本**：Numeric · FloQast · Basis；Rillet 按账务模块对照

**准备资料**：两期总账、工资明细、HR 人数变动、奖金和计提底稿

**植入例外**：新增人员、一次性奖金、重复计提、跨期和缺业务背景

**期望结果**：量化变化并分开已证实原因与假设，定位需修正项目，复核后留完整证据

**测量项**：关键原因遗漏、错误说明、人工补写量、从发现到批准的总工时

### T03 收款核销与短付争议

**适用样本**：HighRadius 为主；Numeric 现金仅作银行流水/账务匹配子步骤对照，AR 发票核销及催收待确认

**准备资料**：付款、未结发票、付款说明、容差和扣款原因政策

**植入例外**：一款多票、多款一票、短付、缺说明、重复回写

**期望结果**：只核销已确认部分，例外交负责人；ERP 清账状态和催收状态一致

**测量项**：正确无人工核销比例、误匹配、例外时间、ERP 接收与重试结果

### T04 经营计划与集团合并

**适用样本**：Pigment · 金蝶 EPM；账务平台提供实际数对照

**准备资料**：已确认实际数、组织口径、预算驱动、内部交易及汇率

**植入例外**：口径不一致、未授权模型修改、抵销缺项、共享报告权限不匹配

**期望结果**：说明假设并形成可复核情景；合并调整与来源相连；变更及共享范围受控

**测量项**：模型/口径修复工时、未发现差异、批准修改量和权限验证结果

### 测量要以最终结果为单位

- **总工时**：资料准备、连接、配置、自动处理、补充、复核和返工分别记录；不要只测 AI 生成速度。
- **正确自动完成比例**：无需人工介入且核查正确的适用项目数 ÷ 全部适用项目数。单据、卡交易、核销和解释分别统计，不能混成同一分母。
- **错误与遗漏**：用人工核查答案标出误处理、关键遗漏及误拦截，记录对财务结果的影响；厂商未公开错误率时保持未知。
- **闭环结果**：核对外部系统是否真正接收，后续修正是否刷新，失败是否可见，重试是否重复入账。
- **采用成本**：同时记录字段映射、规则维护、权限配置、培训及长期复核负担，收益与这些投入一起判断。

## 研究范围与证据边界

本报告服务于财务 AI 产品定位与设计，按统一框架建立 9 个主样本。国外样本为 Ramp、HighRadius、FloQast、Basis、Rillet、Numeric、Pigment；国内样本为金蝶 AI 星瀚财务云及合思。金蝶按明确产品线拆解，未把全公司能力计入同一产品。

资料核查截至 **2026 年 10 月 12 日**，以当前官方产品、操作/帮助文档、定价、官方托管技术资料和客户案例为主。金蝶部分主站全文超时，使用官方索引正文，具体读取方式保留在来源列表；旧资料标明适用时间。厂商公告和案例证明其公开表述，不等于独立效果验证。

未登录各家生产账户、取得销售合同、访谈实际客户或执行同题实测。因此功能、权限和写回范围属于公开证据；设计机会、样本顺序和说明性用例属于本报告的分析与建议。未找到完整价格、准确率、失败回滚或具体接入覆盖时保留待确认。

**术语**：ERP 是企业资源计划系统；GL 是总账；AP 是应付；AR 是应收；O2C 是从客户交易到收款；R2R 是从账务记录到报告；FP&A 是财务规划与分析；FTE 是全职人员工作容量；Agent 指能调用工具执行任务的智能体；MCP 是 AI 与业务工具受控连接的接口协议。

**补充术语**：CAS 是客户会计服务；PO 是采购订单；DSO 是应收账款周转天数，常用于衡量收款速度；SKU 在本报告中指实际售卖的产品模块；FDP 是 Numeric 完整财务数据平台。

### 样本定义与证据口径

**Ramp · 样本与范围**：Ramp 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**Ramp**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**HighRadius · 样本与范围**：HighRadius 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**HighRadius**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**FloQast · 样本与范围**：FloQast 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**FloQast**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**Basis · 样本与范围**：Basis 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**Basis**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**Basis**：部分材料仅取得官方索引正文或案例标题；读取限制保留在来源记录中。

**Rillet · 样本与范围**：Rillet 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**Rillet**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**Numeric · 样本与范围**：Numeric 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**Numeric**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**Pigment · 样本与范围**：Pigment 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**Pigment**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**金蝶 · 样本与范围**：金蝶 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**金蝶**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**金蝶**：部分材料仅取得官方索引正文或案例标题；读取限制保留在来源记录中。

**合思 · 样本与范围**：合思 的公开产品工作机制，边界取决于模块、连接与配置。案例数值是厂商披露，不是横向标准化测量。

**合思**：来自公开厂商产品、操作说明及案例；未登录实测，案例不视为独立效果测量。

**合思**：部分材料仅取得官方索引正文或案例标题；读取限制保留在来源记录中。

## 官方来源与读取范围

### Ramp

- [Ramp 当前主页与产品范围](https://ramp.com/) - 支出、付款、银行、Stack；发卡及银行服务范围提示
- [Ramp Pricing and Plans](https://ramp.com/pricing) - Free/Plus/Enterprise 当前金额、平台费、年付、模块与 ERP 方案边界
- [Ramp Accounting Automation](https://ramp.com/accounting-automation-software) - 支出到同步工作流、应计和对账、编码解释；不同 ERP 接入
- [Ramp Accounts Payable / Bill Pay](https://ramp.com/accounts-payable) - 发票、PO匹配、审批、支付、独立采用和具体 ERP 范围
- [Ramp Accounting Agent 管理与日常使用文档](https://support.ramp.com/ramp-accounting-agent-enablement-daily-use-admin-guide) - 字段覆盖、Ready与同步开关、夜间批次、重要性与置信度边界
- [Stack by Ramp](https://ramp.com/stack) - 跨系统 Skills、工作簿与分录、审核、日志和免费试用；未公开完整价格
- [Ramp Perplexity 官方客户案例](https://ramp.com/customers/perplexity) - >97% 卡交易自动编码和每月163+小时厂商案例口径

### HighRadius

- [HighRadius 当前主页及 CFO 产品套件](https://www.highradius.com/) - O2C、AP、关账、合并、资金与B2B支付的全套范围；结果定价定位
- [HighRadius Cash Application Software](https://www.highradius.com/product/cash-application-automation/) - 付款说明、匹配、例外、容差和API/文件ERP记账闭环
- [HighRadius Close and Reconciliation Suite](https://www.highradius.com/software/financial-close-and-reconciliation-software/) - 现金/PO/预付应计、异常、余额表、收入及往来核对
- [HighRadius Sage Intacct AR 集成技术说明](https://www.highradius.com/product/accounts-receivable-software/erp/sage/) - ERP保持记录系统、双向数据、HTTPS API/SFTP和增量批次；频率描述边界
- [HighRadius Pricing](https://www.highradius.com/pricing/) - 未公开统一金额、通常年度SaaS订阅说明
- [HighRadius DXP 官方案例 PDF](https://pages.highradius.com/hubfs/highradius.com/case-study/Content%20COE%20New/Case%20Studies/dxp_casestudy.pdf) - 90%+现金核销、DSO降20天、辅助Agent、人机边界和30周实施；未从文件时间推断发布日期
- [HighRadius Outcome-Based Pricing 官方公告](https://www.highradius.com/about/news/highradius-launches-outcome-based-pricing-for-ocfo-software/) - 零实施费、上线前零订阅、收益分成与MASC；无公开分成比例

### FloQast

- [FloQast 当前主页](https://www.floqast.com/) - 会计工作流定位、ERP配合、入账需人工批准与AI审计记录
- [FloQast 当前英文 Pricing](https://www.floqast.com/pricing) - 三种当前组合、模块边界、无按用户收费和询价
- [FloQast Close Management](https://www.floqast.com/close-management) - 任务、对账、签核、日常会计与AI Assistant权限
- [FloQast Transform AI Agents](https://www.floqast.com/close-ai/products/ai-agents) - Builder/Skills/Library、自身数据验证、审核与可复用工作
- [FloQast Journal Entry Management](https://www.floqast.com/close-ai/products/journal-entry-management) - 创建验证审核发布、批准锁定、职责隔离、清单关联
- [FloQast 当前产品页所链接的 JEM Solution Overview PDF](https://7800846.fs1.hubspotusercontent-na1.net/hubfs/7800846/Assets/FloQast_Solution%20Overview_FloQast%20Journal%20Entry%20Management_August%202024.pdf) - 多ERP与Excel输入、模板、支持文件、审批控制；文件名日期不作为产品发布日期
- [FloQast HubSpot 官方客户案例](https://www.floqast.com/stories/the-hubspot-blueprint-building-an-accounting-led-ai-powerhouse) - Coupa上传、Python与公式工作簿、PoC/学习活动、原始时间与预期收益口径及页内冲突

### Basis

- [Basis - AI Agents for Accounting](https://www.getbasis.ai/) - 当前事务所与企业会计范围；审计工作支持；演示入口与无公开金额观察
- [Basis for CAS & Advisory](https://www.getbasis.ai/solutions/cas-and-advisory) - 分类、对账、报告；置信度分流与自动推送；来源和计算可检查
- [Basis for Tax](https://www.getbasis.ai/solutions/tax) - 客户材料与税务第一轮；人员判断与复核
- [Basis for Small Firms](https://www.getbasis.ai/solutions/small-firms) - 待审分录；GL 连接；Procedures 与多客户组织；无公开金额观察
- [Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting) - 企业会计；已批准分录写入 ERP；REDW 20→15 天证言；客户数据训练声明
- [Introducing Deployed Intelligence](https://www.getbasis.ai/blogs/introducing-deployed-intelligence) - 客户部署服务及工作方式改造
- [How Boyum Barenscheer cut CAS preparation time by 75% to 92% to create capacity for growth](https://www.getbasis.ai/blogs/how-boyum-barenscheer-cut-cas-preparation-time-by-75-to-92-to-create-capacity-for-growth) - 官方客户故事标题与发布日期；正文未提取

### Rillet

- [Rillet - The AI-Native ERP](https://www.rillet.com/) - 当前定位；总账记录系统；模块范围与来源可追溯
- [Rillet Help Center](https://www.rillet.com/help-center) - 替换原 ERP；具体集成；4-6 周实施；按功能和复杂度定价
- [General Ledger Software with AI Automation](https://www.rillet.com/product/automated-general-ledger) - 原生支持计划；数据到总账的流程；文件和 API
- [Advanced Revenue Recognition](https://www.rillet.com/product/advanced-revenue-recognition) - 合同审批；收入与递延计划；客户视图和合同变更
- [Aura AI by Rillet](https://www.rillet.com/product/aura-ai) - 实时 GL 问答；Agent 工作流；连续检查与 MCP；模块概览
- [AI you can audit](https://www.rillet.com/product/security-and-permissions) - Agent 提案与人工授权；审计记录；分层审批、角色和期间锁定
- [Smartcar's Director of Finance cut 5+ days from monthly close](https://www.rillet.com/case-studies/smartcars-director-of-finance-cut-5-days-from-the-teams-monthly-close-as-a-finance-team-of-one) - QuickBooks 迁移；关账节省 5+ 工作日；DSO 约50→约30天

### Numeric

- [Numeric 当前产品与路线](https://www.numeric.io/) - 当前定位、模块与 ERP Replacement 专属范围
- [Numeric Financial Data Platform](https://www.numeric.io/financial-data-platform) - 业务对象、会计规则和完整记录系统
- [Numeric Close Management](https://www.numeric.io/product/close-management) - 关账责任、对账和审计记录
- [Numeric Flux Analysis](https://www.numeric.io/product/variance-analysis) - 交易与外部资料生成解释及编辑批准
- [Numeric Cash Management](https://www.numeric.io/product/cash-management) - 匹配规则、分录审批和 NetSuite 发布
- [Numeric Billing and Revenue](https://www.numeric.io/product/billing-and-revenue) - 合同用量、发票及收入确认
- [Numeric 模块与定价](https://www.numeric.io/pricing) - 按模块和完整平台采用、询价
- [Numeric Transaction Monitors](https://www.numeric.io/product/transaction-monitors) - 交易检查内容与提示边界
- [Numeric Brex 客户案例](https://www.numeric.io/cases/brex-x-numeric) - 6 到 4 个工作日及流程组合
- [Numeric Built 客户案例](https://www.numeric.io/cases/numeric-x-built) - FDP 迁移及计费收入工作容量口径
- [Numeric MCP 权限与操作](https://help.numeric.io/articles/5446387341-what-is-the-numeric-mcp) - 读写工具、继承权限、批准配置与记录
- [Numeric NetSuite 集成限制](https://help.numeric.io/articles/8191329356-suiteanalaytics-connect) - Traditional 与 Warehouse 连接差异

### Pigment

- [Agentic AI for enterprise business planning](https://www.pigment.com/) - 计划定位与跨部门范围；Frames/MCP；Planner Coming soon；Carta 首页口径差异
- [Financial consolidation in Pigment](https://www.pigment.com/use-case/financial-consolidation) - actuals 导入；币种、抵销与调整分录；审计及报表；集成与合并 Agent
- [Run the Modeler Agent - updated 2026-09-30](https://kb.pigment.com/docs/configure-and-run-the-modeler-agent) - 永久模型写入与历史；Ask/Build/Plan & Build；自动接受与删除审批；Test & Deploy 限制；模型对象
- [Run the Analyst Agent - updated 2026-07-22](https://kb.pigment.com/docs/configure-and-run-the-conversational-analyst-agent) - 下钻分析；可编辑报告与 PDF；Missions 调度、预览、写 Text Metric；输出权限边界
- [Pigment License Types - updated 2026-05-12](https://kb.pigment.com/docs/pigment-license-types) - 平台费、许可证和功能；三类许可证；权限影响许可证与成本
- [Manage your AI credits - updated 2026-09-17](https://kb.pigment.com/v1/docs/ai-credits) - 年度额度、到期重置；按复杂度消耗；限额与旧合同边界
- [Carta - French official customer story](https://www.pigment.com/customer-stories/carta) - 12 周实施；NetSuite/Workday/Google Sheets；每人每周约2小时及每月10-15小时节省

### 金蝶

- [Kingdee 官方全球首页](https://www.kingdee.com/global) - 企业管理 AI 公司定位；Request A Demo / 联系销售入口。读取：网页全文；www.kingdee.com 自动跳转全球站。
- [金蝶 AI 财务云](https://www.kingdee.com/products/financial_cloud.html) - 星瀚财务领域清单；AI套件、星辰与企业规模分层。读取：官方索引正文；全文打开超时。
- [金蝶 AI 星瀚财务云](https://www.kingdee.com/products/cosmic_finance.html) - 大型企业财务云定位；中台、EPM合并、全面预算与管理会计；填单、审单、报告与分析 AI 场景；预约演示。读取：官方索引正文；全文打开超时。
- [金蝶 AI 星瀚 V8.0 重磅发布](https://www.kingdee.com/resources/articles/1445843916024042177) - 2025-11-18版本发布；星瀚升级命名；小K、Data Cloud、苍穹AI平台关系。读取：官方索引正文；全文打开超时。
- [金蝶云·星瀚财务共享：智能驱动，赋能业务](https://www.kingdee.com/article/1737774452831248385.html) - 当前导航中的产品线与独立灵基；规则/AI/GPT审核分工；采购与费用审核-付款-记账闭环；苍穹部署选项。读取：网页全文；正文发布于2023-12-21，产品导航为研究日页面。
- [携手迈向世界一流！金蝶云·星瀚标杆客户案例大集结](https://www.kingdee.com/resources/articles/1396813829714935745) - 招商局集团星瀚与EAS共同建设案例。读取：官方索引正文；正文发布于2024-07-15。
- [金蝶的财务部，怎么用灵基AI？以AI原生重塑财务生产力](https://www.kingdee.com/resources/articles/1554808863620117377) - 灵基AIOS独立产品及2026发布；金蝶内部HR取数-活动费计提-ERP写回实践；权限规则责任边界。读取：网页全文；正文发布于2026-09-29。
- [【金蝶云·星瀚V8.0】新特性-财务云](https://vip.kingdee.com/article/769491123282183168) - 账簿维度及查询导出权限；出纳币种金额控制；已结账期间控制；实施/升级复杂性。读取：官方社区托管全文，作者Etoakor的笔记分享；非独立合同承诺。

### 合思

- [合思官方首页](https://hosecloud.com/) - 当前产品矩阵与消费/付款定位；AI Partner任务列表；免费试用/预约演示。读取：网页全文。
- [合思费控](https://hosecloud.com/expense.html) - 预算费用标准；单据与分级授权；数电票及ERP凭证；移动审批。读取：网页全文。
- [合思付款](https://www.hosecloud.com/ap/) - 合同付款全生命周期；付款计划与到票；AI合同提取和风险辅助。读取：官方索引正文；全文打开超时。
- [合思档案](https://hosecloud.com/archiving.html) - 电子源文件采集；关联组装及字段回写；四性与业务检测；档案证据链。读取：网页全文。
- [合思BI](https://www.hosecloud.com/bi/bi.html) - 文件数据库API接入；分组及计算指标；仪表板钻取；全链路看板。读取：网页全文。
- [合思广泛连接解决方案](https://hosecloud.com/solutionsr/connect.html) - ERP凭证字段映射与凭证号回写；银企付款回单；组织权限同步；OpenAPI双向同步。读取：网页全文。
- [AI财务审核专家](https://hosecloud.com/aifinancialapproval.html) - 自然语言规则与制度导入；离线真实数据调优；风险依据建议与人机共审；AI审核私有化部署。读取：网页全文。
- [合思×新发现：120+门店，0增人，AI智能审核破解连锁扩张财务困局](https://hosecloud.com/cases/76.html) - 官方客户案例；餐饮混合附件与单价场景；周期及人力成本原口径；无纸化对AI输入质量的影响。读取：网页全文。
