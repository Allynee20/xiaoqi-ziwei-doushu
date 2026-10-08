# Final Analysis Schema

默认交付给普通用户时，完整内部结构按 `USER_REPORTS/FINAL_USER_REPORT_PROTOCOL.md` 投影为 `FINAL_SIMPLE_USER_REPORT`。内部字段、证据链和五段式验证继续保留，但默认不直接打印；技术版或 Extended Report 才展开。

`FINAL_SIMPLE_USER_REPORT` 使用 positive-evidence-only rendering：内部不确定性仍完整保留，用户正文对 `UNKNOWN / UNRESOLVED / INSUFFICIENT / OUT_OF_SCOPE / NO SUPPORT` 默认静默。审计状态、缺证说明、范围解释、内部 Schema 词和未被正面分析的替代资源路径不得进入用户正文；不得用否定替代路线来“证明”已写出的路线。

## 0. 来源与职责

按需标明 `REFERENCE_KNOWLEDGE / PROJECT_SCHEMA / EXTERNAL_RESEARCH / MODEL_INFERENCE`。Strong Reasoner 负责综合，但必须能回指事实、语法和边界。未预编码组合可在证据充分时标 `REASONER_SYNTHESIS_ALLOWED`；证据不足时保留 `UNRESOLVED / KNOWLEDGE_GAP`。

## 1. 核心判断

直接回答用户的 Topic/Subquestion，并标注支持程度。每条重要结论必须包含：

内部先使用 `CLAIM / WHY / BOUNDARY / OPTIONAL_SOFT_SIGNAL` Claim Card；最终报告写成自然语言，不打印这些字段名。`WHY` 保留 2–4 条独立证据链，`BOUNDARY` 同时包含 nearest cannot-imply 与 miss condition，Soft Signal 仅在有价值时附加且不得补救 Core。

```text
EVIDENCE
REAL_WORLD_DIMENSION
CONTRAST
CANNOT_IMPLY
MISS_CONDITION
```

不要用工程状态词充当正文结论。缺任一字段的句子不能成为主结论。

## 2. 主线结构

解释最关键的宫位角色、星曜功能、四化与关系结构如何共同作用；只保留对问题有用的结构。

机械拓扑必须单列为 `MECHANICAL_ONLY_FACTS`，只说明检索路径；真正使用的物理宫内容、四化、关系、资源与留存路径列为 `INDIVIDUAL_EVIDENCE_USED`。

## 3. 支持因素

列出独立支持、资源、入口、协作与可见度；相关视图不得重复计票。

完整财富分析必须逐项报告 `SELF_EARNED_INCOME / CAREER_DERIVED_WEALTH / FAMILY_OF_ORIGIN_SUPPORT / FAMILY_ASSET_BASE / SPOUSE_RESOURCE / SPOUSE_FAMILY_RESOURCE / PROPERTY_ASSET_TRANSFER`，不得默认财帛宫等于全部财富来源。

完整 `CAREER_WEALTH_SYSTEM` 还必须报告：

```text
CAREER_VEHICLE
CONTROL_LEVEL
RESOURCE_SOURCE
SCALABILITY
RETENTION
NATAL_RESOURCE_BASELINE
DECADE_RESOURCE_BAND
DECADE_DELTA
```

Baseline 使用 `ORDINARY_RESOURCE_STRUCTURE / AFFLUENT_RESOURCE_STRUCTURE / HIGH_WEALTH_CAPACITY_STRUCTURE / UNRESOLVED`，不得打分。仅在另行明确启用阶段分析时，每个大运才需给出 `BUILD / EXPAND / CONSOLIDATE / RESTRUCTURE / HIGH_SCALE_HIGH_RISK / CONTRACT` 之一、相对本命 Band、与上一运 Delta、主要代价与 Miss Condition；Public v1 默认不运行此分析。

## 4. 限制 / 成本 / 冲突

区分成本、修饰、证据依赖与真冲突；说明结果需要哪些现实条件。

## 5. 不确定项

列出 `PARTIAL / CONFLICTED / UNRESOLVED / INSUFFICIENT` 及其影响，不把未知写成坏。

如不足影响用户所问结论，附加符合 `KNOWLEDGE_GAP_PROTOCOL.json` 的机器可读对象，并停止该项结论升级。

派生宫最多一层，默认置信度低于同等级直接宫位一档。`Spouse Career` 只写 spouse's work/social-role structure，并标注 `ONE_DERIVED_LAYER_MAX`，不得写 actual occupation。

`MARRIAGE_SYSTEM` 必须分列 `FORMATION / STABILITY / SATISFACTION / SPOUSE_SIDE_RESOURCE / RESOURCE_TRANSFER / DECADE_DELTA`。`SPOUSE_SIDE_RESOURCE = RESOURCE_STRONG` 必须通过两条独立方向的 Gate；相同物理 evidence 的借宫/对宫重见不得算第二条。

## 6. 综合分析

由强 Reasoner 做主次判断、条件组合和自然语言收束。使用条件式表达，不输出 `STRUCTURAL_MECHANISM_PRESENT` 等 V3 机器措辞，不作医疗、法律、投资或高风险绝断。

发布前执行 Sentence Swap Test。共享句仅在两盘均有真实结构支持时保留并标记 `SHARED_STRUCTURAL`；它不计作区分性命中。区分度不能靠发明差异；相似机制可以产生相似报告。

按实际分析范围执行 Baseline Swap、Decade Curve Swap、Mechanical Topology、Lifecycle Template、Spouse Resource Gate 与 No Domain Reassignment 审计；未启用的 Decade / Lifecycle 分析不得运行或投影到用户报告。任何跨域追认均为 `MISS`。

## 7. Soft Signal Layer（可选，Core 冻结后）

主动输出 `3–5` 条，超过五条为失败。每条必须保存：

```text
signal_id
domain
strength
evidence_summary
independent_evidence_paths
cannot_imply
conflict_status
user_facing_sentence
```

`strength` 仅允许 `CLEAR_TENDENCY / HAS_SIGNAL / AUXILIARY_ONLY`。Soft Signal 不进入 Core 投票，不得修改 `NATAL_RESOURCE_BASELINE / CAREER_WEALTH_SYSTEM / MARRIAGE_SYSTEM / DECADE_RESOURCE_BAND / DECADE_DELTA`。`AUXILIARY_ONLY` 默认隐藏；Core 冲突时以 Core 为准并 suppress 或明确冲突。

`SOFT_SIGNAL_LIBRARY != COMPLETE_LIST`。允许 Reasoner 创建未列出的 soft signal，但仍须满足同一输出字段、强度门槛、evidence identity 去重、mechanical-topology 禁令和 Core 优先级。

## 8. User-facing projection

普通用户版遵守 `USER_REPORTS/DEFAULT_ANALYSIS_SCOPE.md` 与 `ECONOMIC_PARTICIPATION_BOUNDARY.md`，先回答开放式 `VALUE_CREATION_QUESTION`，允许 `ORDINARY_STABLE_OUTCOME`，并禁止默认职业升级路线。只输出 Person、Work / Value Creation、Relationship 三个模块，可选总结不得增加新主张。财富信息只在有独立正面支持时自然放入 Work 模块；不得默认建立财富章节或把 `NATAL_RESOURCE_BASELINE` 显示为 Total Wealth Class。Family Wealth、Health、Timing 等按需/非默认主题不得成为固定栏目或范围免责声明。未知或缺少支持的内容留在内部，不得因保持沉默而补写排除性结论。展示规则见 `USER_REPORTS/FINAL_USER_REPORT_PROTOCOL.md`；这是默认展示/路由层，不修改原有结构知识。
