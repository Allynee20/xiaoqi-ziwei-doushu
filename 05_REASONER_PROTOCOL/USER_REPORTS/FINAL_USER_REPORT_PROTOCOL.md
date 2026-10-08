# Final User Report Protocol

Status: `REQUIRED_DEFAULT_USER_OUTPUT`

本协议冻结 Public v1 的默认用户展示层，不改变 Core、Career–Wealth、Marriage、Natal Baseline、Decade 或 Soft Signal 的既有内部知识与方法。默认范围见 `DEFAULT_ANALYSIS_SCOPE.md`。

默认产品范围以 `DEFAULT_ANALYSIS_SCOPE.md` 为准，参与路由以 `ECONOMIC_PARTICIPATION_BOUNDARY.md` 为准，家庭财富禁区以 `FAMILY_WEALTH_SCOPE_GUARD.md` 为准。

## Internal / user separation

内部可以继续保存 `CAREER_VEHICLE / CONTROL_LEVEL / SCALABILITY / RETENTION / NATAL_RESOURCE_BASELINE / DECADE_RESOURCE_BAND / DECADE_DELTA`。普通用户版默认将它们翻译成可观察现实语言，不堆 Schema 名称、星曜清单或工程状态词。需要审计时另给 Extended Report。

## Positive-evidence-only user rendering

```text
POSITIVE_EVIDENCE_ONLY_USER_RENDERING = REQUIRED
UNKNOWN_CONTENT_USER_RENDERING = SILENT
OUT_OF_SCOPE_USER_RENDERING = SILENT
NEGATIVE_EXCLUSION_SENTENCE = FORBIDDEN_BY_DEFAULT
INTERNAL_AUDIT_SEPARATED_FROM_USER_REPORT = REQUIRED
```

内部继续保留 `SUPPORTED / UNRESOLVED / UNKNOWN / INSUFFICIENT_EVIDENCE / FORBIDDEN_INFERENCE / OUT_OF_SCOPE`，但它们不是用户正文。只把已有正面支持、且对用户问题有用的内容写进报告；未知、未解决、缺少支持和关闭主题默认不写，也不解释“为什么没说”。

默认禁止研究或审计式表达，包括“没有足够证据”“没有独立证据”“不足以推出”“无法判断”“本报告不判断 / 不分析”“没有看到明显”“不能据此认为”“尚不足以支持”“不作为本报告主线”等。也不以排除未被正面分析的路线来证明另一条路线，例如“靠本人工作，而不是家庭或伴侣”“适合专业工作，而不是创业”。普通概率限定词（如“更容易”“更偏向”“通常”）可以保留。只有省略限定会实质误导一条已输出的核心判断时，才可用简短自然语言限定该判断；仍不得暴露内部状态、缺证过程或未讨论的资源来源。

`ABSENCE OF EVIDENCE != EVIDENCE OF ABSENCE`；内部的未知资源状态不得转写为“没有家庭 / 配偶资源”。涉及 Family Origin、配偶财富、继承或被动资源而没有正面可输出结论时，整项静默，不写正向或排除性判断。

## Default user report structure

用户版只按以下顺序组织；不得先铺陈星曜清单、内部字段或十几个术语：

### 1. 你这个人怎么运转

将核心运行机制、自然优势、过量使用后的常见代价合在一起，写清遇事时较自然的判断与行动方式。

### 2. 你怎么工作、怎么创造价值

先回答开放的 `VALUE_CREATION_QUESTION`，再写有支持的工作环境、责任范围、自主空间、工作节奏与消耗。只有本人收入/价值转收入/资金使用或沉淀存在明显独立正面信息时，才把它自然写入本节；不另设默认财富章节。

### 3. 你在亲密关系里怎么运转

写有支持的长期关系需求、互动方式、冲突反应和较适合的相处结构。默认不推断伴侣的具体职业、长相、财富、家庭财富、婚姻次数或精确婚期。

### 可选：最后总结

仅可用 2–4 句话压缩前三节。逐句检查每个判断是否已在前三节出现；任何新主张都必须删除。

每节只保留真正有结构差异的内容。若去掉姓名、出生信息和星曜名称后主结论仍可大量交换给不同结构，标 `NON_DISCRIMINATIVE` 并重写；若结构机制相似，则允许报告相似，不得为区分而发明差异。

## Default analysis gates

```text
DEFAULT_DECADE_ANALYSIS = OFF
DEFAULT_LIFECYCLE_ANALYSIS = OFF
DEFAULT_FUTURE_STAGE_ANALYSIS = OFF
DEFAULT_ANNUAL_ANALYSIS = OFF
DEFAULT_DYNAMIC_FACTS_USAGE = OFF
WEALTH_SECTION = OPTIONAL_WITHIN_WORK_MODULE
SUMMARY_NEW_CLAIMS = FORBIDDEN
```

以上关闭状态作用于 Public v1 默认路径；不得为填满版面而生成阶段/流年内容。相关内部方法不因本协议而删除。Soft Signal 只有在提升三个默认模块的区分度且不改写 Core 时才可加入，不得凑数或补救 Core。

Parents/Family Origin、Family Environment/Wealth、Siblings、Children、Health、Detailed Property 与 Detailed Social Network 均为 `ON_DEMAND_TOPIC`，不作为默认固定栏目。

关闭主题只影响内部路由；用户版不列出空栏目、不添加范围说明或结尾免责声明。若用户主动询问某项，再按该问题决定是否有可用内容。

## Length and language

普通用户版默认使用大白话和现实语言；不要堆 Schema 名称、星曜清单、审计状态或分析过程。只写三项默认模块以及可选总结。星曜和内部术语只在用户主动要求技术版时展开。
