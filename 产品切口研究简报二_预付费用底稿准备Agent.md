# 预付费用底稿准备 Agent 产品研究简报

面向财务 AI 产品立项团队  重点官方资料核查 2026年10月14日

**建议继续调研从原始材料和上期已复核底稿生成本期预付支持表的 Agent。** 首个任务覆盖合同与新增事项整理、变更确认、按客户政策重算、与总账核对及待审分录差额。费用计提作为后续相邻任务。这个方向的成败取决于减少取数、变更与复核，而不只是算出摊销金额。

该方向与月结费用解释的结果不同：解释任务回答实际变化为何发生；准备任务按企业已采用的政策形成支持账务的底稿。两者可用同一份合同与费用资料研究，但底稿计算正确不代表业务原因已证实，说明获批也不等于分录获批。

## 为什么将准备任务列为第二方向

Basis、FloQast Transform 与 Ramp Stack 都已公开描述可复用会计任务，输出支持表、分录或报告并保留复核。这使单项任务具备可检查的产品参照。选择一个合同类型、一个期间和一份已完成底稿，可以先验证产物，再扩展连接和执行范围。[\[1\]](https://www.getbasis.ai/solutions/corporate-accounting)[\[7\]](https://www.floqast.com/close-ai/products/ai-agents)[\[4\]](https://ramp.com/stack)

主要替代是已有 ERP 的支持计划与定时凭证、Excel公式、宏及 RPA。Ramp 普通 Plus 摊销功能已可按日期、预付账户和费用科目安排分录，NetSuite 与其他合格系统采用不同机制。静态摊销计算本身的产品空间有限，应首先比较客户配置既有功能的成本。[\[6\]](https://support.ramp.com/ramp-amortization-with-accounting-integrations/)

## 目标客户与首个任务

初始客户假设为已有 ERP、仍在表格中滚动预付底稿的企业核算团队，或服务多个客户且已有统一方法的会计服务机构。第一轮先选其中一类，避免同时承担企业与事务所的产品、权限和交付要求。

会计准备，核算主管复核，采购或合同负责人提供变更，财务或共享负责人决定预算。值得接触的客户应有可提供的上期已复核底稿和政策，本期仍反复整理新增合同、续约、退款、提前终止或部门变更。若工作只有少量固定公式，优先采用现有工具。

| **候选切口** | **本轮判断** | **主要前提与限制** |
| --- | --- | --- |
| 预付支持表滚动与总账核对 | 首选验证 | 来源和政策明确；需要处理新项目、变更、核对与待审结果 |
| 合同或 PO 驱动费用计提 | 第二步 | 还需收货或服务完成、已入账资料和客户估计；不能只凭未付款认定漏计提 |
| 银行对账例外 | 条件型备选 | 结果可验收，但匹配、底稿与 ERP 清账状态必须分开 |
| 通用会计 Agent 编辑器 | 暂缓 | 把流程设计交给用户，范围与复核成本难统一；先证明一个模板任务可复用 |

## 把任务拆成可检查的工作

一个任务由主体、期间、支持表版本、企业政策和复核人共同定义。源资料包括合同及变更、发票、上期底稿、期初未摊余额和本期相关总账。合同金额、发票金额与可摊金额可能不同，服务期间及税务口径需按客户确认的政策处理，不由模型自行决定。

| **步骤** | **Agent 的准备工作** | **可以验收的结果** |
| --- | --- | --- |
| 读入方法 | 识别上期已复核文件、政策与字段映射 | 规则、期间、科目及来源版本由人员确认 |
| 识别变化 | 查找新增合同、续约、终止、退款等事件 | 原文件位置、变更前后字段、待确认项 |
| 更新支持表 | 调用确定性规则滚动和重算 | 可编辑公式、分项计划、期末未摊余额 |
| 核对总账 | 关联已入账与支持表，计算差额 | 期初加新增减摊销及调整等于期末；与 GL 差异单列 |
| 准备交审 | 形成分录差额草稿和例外材料 | 借贷方向、期间、科目、来源及未解事项可查 |
| 复用与重跑 | 保存批准规则，输入更新后重算 | 新旧版本变化清楚，不重复计入已处理项目 |

语言模型适合识别材料、提出映射、说明计算和列出缺口；会计政策选择及计算结果通过可重算规则、核对和人员批准约束。尤其要区分未取得资料、疑似遗漏和已确认差错。两期总账无法单独证明费用完整性。

## 竞品的任务与执行边界

**Basis 提供公司方法与执行结果的参照。** 企业会计页描述政策、映射、支持表、输入与计算、例外，以及已批准分录写回 ERP。CAS 页的高置信自动推送特指银行或卡交易编码，不能外推成全部调整分录自主过账。演示要看当前客户政策如何进入任务、哪些工作是实施配置、复核人如何定位原文件及计算。[\[1\]](https://www.getbasis.ai/solutions/corporate-accounting)[\[2\]](https://www.getbasis.ai/solutions/cas-and-advisory)

**FloQast Transform 提供从既有成果建立任务的参照。** 2026年9月16日的官方文章描述用上一期输入和已审核输出构建流程，在旧数据上按列与实体核验，并由团队设定人工确认节点。这支持先取得真实完成样本；它不证明新期退款或冲突材料已经通过。JEM 的分录批准和发布是另一个流程对象，应分别核验权限。[\[7\]](https://www.floqast.com/close-ai/products/ai-agents)[\[8\]](https://www.floqast.com/blog/transform-builds-from-last-months-close)[\[9\]](https://www.floqast.com/close-ai/products/journal-entry-management)

**Ramp Stack 的主页与具体记账文档要并列阅读。** 主页描述跨系统 Skills、公式工作簿、待审分录与批准同步；《Stack for bookkeeping》则以标准 QBO 流程为主，列支持表滚动与同步前审改拒，说明不改已有 QBO 交易、不支持多币种，合格多实体设置另需确认。不能用主页系统名单作为每种任务可写的证明。[\[4\]](https://ramp.com/stack)[\[5\]](https://support.ramp.com/stack-for-bookkeeping)

该操作文档还说明银行对账能生成底稿并同步清理交易，但不能在 QBO 中标为已对账，受其 API 限制。因此如果把银行对账换成首个切口，验收必须核对外部状态，不能只看匹配比例。[\[5\]](https://support.ramp.com/stack-for-bookkeeping)

**Rillet Aura 用于对照执行权，不能替代既有 ERP 叠加路线。** 它在自身账务平台中给 Agent 动作生成提案，人员批准后才过账并留日志；规则支持计划另有机制。第一版可借鉴提案与权限，但不需先承诺替换客户总账系统。[\[11\]](https://www.rillet.com/product/security-and-permissions)[\[14\]](https://www.rillet.com/help-center)[\[15\]](https://www.rillet.com/product/automated-general-ledger)

## 案例与定价不能代替任务验收

Basis 企业页的 REDW 证言披露四个月内关账从20天至15天、59%的清单先由 Basis 处理。这是整体任务组合的厂商证言，days 未限定工作日，不能归因单一预付任务或作为我们的效益目标。[\[1\]](https://www.getbasis.ai/solutions/corporate-accounting)

FloQast HubSpot 案例展示自建预付和应计流程，但正文预付耗时与摘要不同，应计50%的收益在正文为预计、摘要为已实现。该案例可用于追问工作簿和流程构建方式，不能合并数字来预测价格或节省人时。[\[12\]](https://www.floqast.com/stories/the-hubspot-blueprint-building-an-accounting-led-ai-powerhouse)

| **产品** | **当前公开商业边界** | **评价时必须固定的范围** |
| --- | --- | --- |
| Basis | 条款由订单规定价格、账期及订阅期限；没有统一公开金额[\[3\]](https://www.getbasis.ai/legal/product-terms) | 任务模板、客户政策、实体、连接写权、实施及持续服务 |
| FloQast | Close AI 等方案询价，不按用户收费；能力合同范围需核价[\[10\]](https://www.floqast.com/pricing) | Transform、底稿与 JEM 的授权和接入、实施、交易实体范围 |
| Ramp Stack | 当前主页引导联系 Ramp 团队；操作页有 credits 使用，计划需问代表[\[4\]](https://ramp.com/stack)[\[5\]](https://support.ramp.com/stack-for-bookkeeping) | Stack 订阅及用量、任务复杂度、资格、支持服务；不套用 Plus 用户价[\[13\]](https://ramp.com/pricing) |

候选收费单位可先按一类任务、服务主体及期间约定有限试点，而非按对话次数展示价值。客户净价值取决于完整准备与审核工时、接入及维护、实际替代支出和产品费用。供给端还需记录推理、交付和持续人工支持成本；下一期或第二客户仍逐笔由专家加工时，应按服务交付核算。

## 第一版范围与差异化假设

限定单实体、单功能币和一种经客户确认的预付处理方法。输入采用上传文件和人工映射，优先支持已有已复核底稿。每个项目有稳定标识和来源版本，输出公式支持表、与 GL 的核对差异、待审分录文件及例外清单。

- 承接上期方法：读取并确认字段、会计规则、取数范围和审核标准；长期规则的更新需明确批准。

- 处理本期变化：识别新增、续约、提前终止、退款和部门变更；材料冲突或日期不明时形成待确认项。

- 形成可检查产物：可编辑公式、分项计划、金额核对、期末余额及待审差额；已入账金额仍纳入支持表与核对，不重复形成分录。

- 管理复核与重复执行：保留输入、方法、运行和批准版本；重跑展示差异，防重复计入；正式账务由原 ERP 执行。

可验证的优势是把杂乱原资料、合同变更和已采用方法连到可重算结果，减少每期取数、核对与返工。若客户既有 ERP 计划或一张维护成本很低的 Excel 已能稳定完成，应停止这个切口，避免把公式包装成 Agent。

## 下一轮研究与停止条件

建议在企业核算或会计服务两个客户群中选一个，访谈6至8家，再取2至3家连续期间资料。需要同一次月结的合同与变更、上期底稿、采用政策、当期总账、审核意见和最终入账结果。样本数量是拟定研究安排。

问操作者：上期底稿从什么材料得到，除了计算还做了哪些取数和判断，本期新增或变更在哪里漏过？

问审核者：逐项核对哪些字段和公式，什么情况必须退回；如何确认前期余额和已入账金额？

问负责人：原 ERP 为什么没有解决，配置一次是否更划算；哪份产物能正式验收，试点如何进入采购？

先复现一个已完成期间，再用新期间及测试副本验证合同冲突、服务期不明、退款、重复单据、前期更正和重复运行。比较旧方法及可配置的 ERP 或 Excel 基线。由会计与复核人确认参考答案；记录输入准备、变更、计算、核对、审核及返工总工时，金额与政策错误，第二期配置改动量和逐笔人工支持。

**继续投入**：除了公式确有重复准备负担，支持材料可取得，产物可核验，下一期主要复用且完整审核负担下降，买家能给出验收和预算路径。**收窄或停止**：现有功能配置即可解决，每个项目都需重新判断政策，Agent 核查更费时，或第二期及第二客户持续逐笔定制。隐藏差额、未经批准改变规则、重跑重复计入和已批准旧结果失效未提示，必须先修复并重测。

若此任务的复用和净收益证据强于费用解释，应提升它的优先级。若静态准备已足够自动化，而主要损耗仍是业务原因与审核追问，则把它作为现有系统能力，主攻第一份简报的解释与处理。

## 来源与核查范围

基准材料为用户提供的《财务 AI 竞品深度调研》，38 页，原核查截止 2026 年 10 月 12 日。以下为重点产品的增补官方来源。公开操作说明支持工作机制；客户案例保留具体范围，实际收益以目标客户试点确认。

\[1\] [Basis for Corporate Accounting](https://www.getbasis.ai/solutions/corporate-accounting)  核查 2026-10-14

企业政策、底稿、例外、批准分录与 REDW 证言。

\[2\] [Basis for CAS & Advisory](https://www.getbasis.ai/solutions/cas-and-advisory)  核查 2026-10-14

CAS 分类、报告、自动推送与待审的流程区别。

\[3\] [Basis Product Terms](https://www.getbasis.ai/legal/product-terms)  核查 2026-10-14

订单规定价格、账期和期限，公开金额未列。

\[4\] [Ramp Stack product](https://ramp.com/stack)  核查 2026-10-14

跨系统 Skills、公式工作簿、复核与同步。

\[5\] [Stack for bookkeeping — Ramp Help Center](https://support.ramp.com/stack-for-bookkeeping)  核查 2026-10-14

具体记账操作及适用条件，主要以标准 QBO 流程为对象。

多系统平台宣传不应替代具体流程的接入与动作验收。

\[6\] [Ramp amortization with accounting integrations](https://support.ramp.com/ramp-amortization-with-accounting-integrations/)  核查 2026-10-14

普通 Ramp 原生摊销及不同 ERP 的计划机制。

普通 Ramp 摊销功能，不是 Stack 独有的 Agent 功能。

\[7\] [FloQast Transform AI Agents](https://www.floqast.com/close-ai/products/ai-agents)  核查 2026-10-14

Transform 会计工作流构建与测试。

\[8\] [Skip the Blank Page. Transform Builds From Last Month's Close.](https://www.floqast.com/blog/transform-builds-from-last-months-close)  核查 2026-10-14

从上一期输入与已审核输出建立流程，旧期核验与人工确认。

官方文章发布日期 2026-09-16，核查日 2026-10-14；旧期核验通过仍需测试新期变更与例外。

\[9\] [FloQast Journal Entry Management](https://www.floqast.com/close-ai/products/journal-entry-management)  核查 2026-10-14

分录准备、审批、职责隔离及发布。

\[10\] [FloQast Pricing](https://www.floqast.com/pricing)  核查 2026-10-14

当前方案、计费方式与询价。

\[11\] [AI you can audit — Rillet](https://www.rillet.com/product/security-and-permissions)  核查 2026-10-14

Aura 提案批准、日志及控制。

\[12\] [The HubSpot Blueprint: Building an Accounting-Led AI Powerhouse](https://www.floqast.com/stories/the-hubspot-blueprint-building-an-accounting-led-ai-powerhouse)  核查 2026-10-14

HubSpot 自建预付与应计流程案例。

正文预付耗时与摘要不同，预期应计收益与摘要不同；不采用该案例数字估算本产品 ROI。

\[13\] [Ramp Pricing and Plans](https://ramp.com/pricing)  核查 2026-10-14

普通 Ramp 定价，不能替代 Stack 报价。

\[14\] [Rillet Help Center](https://www.rillet.com/help-center)  核查 2026-10-14

自身 ERP 定位及商业和实施 FAQ。

\[15\] [Rillet automated general ledger](https://www.rillet.com/product/automated-general-ledger)  核查 2026-10-14

原生支持计划及分录机制，与 Agent 提案分别理解。
