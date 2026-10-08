# Public Reference Map

Status: `PUBLIC_REFERENCE_READY`

本目录是公开 Reference 的紧凑导航层。它连接既有 Canonical 知识、项目方法和运行协议，不复制整套 Stage 文档，也不把 V4 改造成确定性断命引擎。

## Product contract

- `REFERENCE_NOT_RULE_ENGINE`：Reference 教强 Reasoner 如何合法推理，不预计算每个结果。
- `REASONER_AUTONOMY_PRESERVED`：证据主次、冲突处理、语境、软象、自然语言和不确定性由 Strong Reasoner 综合。
- `FREEZE GRAMMAR, NOT EVERY RESULT`：未知组合允许 `UNRESOLVED / REASONER_SYNTHESIS_ALLOWED`。
- `COMPOSITE_FIRST` 是组合原则，不是要求枚举所有双星或多星组合。
- Pattern 框架是推理辅助，不是格局穷举引擎。
- `SOFT_SIGNAL_LIBRARY != COMPLETE_LIST`。
- 仁怀 518,400 生成语料若被使用，只能作为覆盖、回归、措辞、模式和缺例发现用的 generated combinatorial reference corpus；不得嵌入全部语料或作为 lookup predictor。

## Knowledge provenance

每个重要判断应区分：

1. `REFERENCE_KNOWLEDGE`：本仓库 Canonical 知识或明确 Profile。
2. `PROJECT_SCHEMA`：项目自建的分析、认识论或输出框架，不冒充传统命理共识。
3. `EXTERNAL_RESEARCH`：可选实时检索所得资料；必须注明来源、学派和不确定性。
4. `MODEL_INFERENCE`：Reasoner 基于前述材料的综合，必须可回指证据和边界。

实时 Web 只用于传统出处、流派差异、罕见术语、未决机制或当前研究，不得用于看过现实后的事后合理化。

## Public v1 reading path

Follow only the path selected in the root `README.md`; do not recursively browse this tree. The default path is:

1. [`01_SYSTEM_AND_CHART`](01_SYSTEM_AND_CHART/README.md)
2. [`02_PRIMITIVE_SEMANTICS`](02_PRIMITIVE_SEMANTICS/README.md)
3. [`03_QUESTION_AND_ROLE`](03_QUESTION_AND_ROLE/README.md)
4. [`04_STRUCTURAL_MODIFIERS`](04_STRUCTURAL_MODIFIERS/README.md)
5. [`05_COMPOSITION_AND_RELATIONS`](05_COMPOSITION_AND_RELATIONS/README.md)
6. [`06_SYNTHESIS_METHOD`](06_SYNTHESIS_METHOD/README.md)
7. [`07_TOPIC_METHOD_ROUTER`](07_TOPIC_METHOD_ROUTER/README.md)
8. [`09_VARIANTS_AND_UNRESOLVED`](09_VARIANTS_AND_UNRESOLVED/README.md)
9. [`10_RUNTIME_PROTOCOL`](10_RUNTIME_PROTOCOL/README.md)

Timing/dynamic materials are not part of this Public v1 release path. Local V4 retains its internal timing methods and runtime assets.

只沿根 README 明确列出的路径阅读；不要递归加载未链接资料或内部档案。
