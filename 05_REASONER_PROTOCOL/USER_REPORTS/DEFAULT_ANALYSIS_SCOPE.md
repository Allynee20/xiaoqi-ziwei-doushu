# Default Analysis Scope

Status: `REQUIRED_DEFAULT_SCOPE`

```text
DEFAULT_REPORT_AUDIENCE = ORDINARY_ADULT_ECONOMIC_PARTICIPANT
```

这表示默认产品主要面向通过本人工作、专业、项目或小规模经营参与现实经济生活的普通成年人；它不是命理判断“此人一定工作”。参与程度由显式用户 Context 控制，不由性别控制。

## Public v1 product contract

```text
ZIWEI_PUBLIC_REFERENCE_VERSION = v1
PUBLIC_PRODUCT_SCOPE = NATAL_STRUCTURAL_ANALYSIS
DEFAULT_MODULES = PERSON, WORK_VALUE_CREATION, RELATIONSHIP
DEFAULT_DECADE_ANALYSIS = OFF
DEFAULT_LIFECYCLE_ANALYSIS = OFF
DEFAULT_FUTURE_STAGE_ANALYSIS = OFF
DEFAULT_ANNUAL_ANALYSIS = OFF
DEFAULT_DYNAMIC_FACTS_USAGE = OFF
```

Public v1 用紫微命盘理解成年人的相对稳定运行机制。默认只呈现以下三个模块；第四项总结可选，且只能压缩前三项。

## Default Core Output

### 1. Person / Life Operating Style

回答这个人遇事时最自然的判断与行动方式。把核心机制、自然优势，以及同一机制过量使用时的代价写在一起；只保留 1–3 个最有区分度的主轴，不生成大而全性格词典。

### 2. Work / Value Creation

回答开放问题：现实里最自然靠什么创造价值、换取收入？说明更容易发挥能力的问题类型、自然的价值创造方式、适合的工作环境、自主空间、完整结果或局部执行、稳定流程或复杂变化，以及主要工作消耗。不得默认沿执行→项目→管理→平台升级。

钱不单独成为默认章节。只有对本人收入形成、价值转成收入或资金使用/沉淀机制存在明显且独立的正面信息时，才自然写入本节；不得把 `NATAL_RESOURCE_BASELINE` 当作总财富等级。

### 3. Intimate Relationship

回答长期关系里真正需要什么、自然如何表达和处理关系、舒服的互动方式、容易消耗的关系模式、冲突时的自然反应，以及有助于长期稳定的相处结构。默认只描述命主自身的关系运行方式，不输出配偶职业、长相、本人/配偶家庭财富、婚姻次数、精确婚期或必然离婚。

### Optional summary

允许 2–4 句话压缩前三个模块，不得添加新判断、领域或未来阶段主张。

## Outside the default public scope

未来大运、人生阶段、流年、健康诊断、家庭财富等级、精确职业、精确收入/净资产、婚姻次数与婚期均不是 Public v1 默认产品范围。它们不进入默认阅读路径、运行时调用或用户报告；本地内部项目保留的相关方法与运行资产不得因此删除。

## On-demand topics

以下知识保留在 KB，但统一标记 `ON_DEMAND_TOPIC`，仅在用户主动询问时分析：

```text
PARENTS / FAMILY ORIGIN
FAMILY ENVIRONMENT
FAMILY WEALTH LEVEL
SIBLINGS
CHILDREN
HEALTH
DETAILED PROPERTY
DETAILED SOCIAL NETWORK
```

默认报告不得固定输出这些栏目，尤其不得输出 Family Wealth Level。

## User-facing omission rule

```text
OUT_OF_SCOPE_USER_RENDERING = SILENT
UNKNOWN_CONTENT_USER_RENDERING = SILENT
```

`ON_DEMAND_TOPIC` 是内部路由，不是用户正文提示。未被主动询问或没有正面可输出内容时，直接省略该主题及其空标题；不得在正文或结尾说明它“未分析”“无法判断”或“不在范围内”。
