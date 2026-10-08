# Composition and Pattern Method

Status: `REQUIRED_REASONING_GRAMMAR`  
Schema type: `PROJECT_SCHEMA`

本文件提供 Strong Reasoner 可现场应用的方法，不建立 Pattern Enumeration Engine。

## 1. Composite First

当两颗或多颗星形成稳定共同结构时，先理解组合后的共同机制，再依次进入：

```text
COMPOSITE_MECHANISM
→ PALACE_ROLE
→ TRANSFORM
→ LOCAL_MODIFIER
→ SANFANG / OPPOSITE / BORROW
→ TOPIC_CONTEXT
```

禁止：

```text
STAR_A_TEXT + STAR_B_TEXT = COMPOSITE_MEANING
```

Reasoner 必须说明共同作用、相互牵制或职责分工，而不是拼接两段单星词典。Reference 没有现成组合时，若 Primitive、Palace、Modifier、Relation 和 Topic 边界足够，可标 `REASONER_SYNTHESIS_ALLOWED` 并现场综合；否则标 `UNRESOLVED`。缺少预编码组合不得迫使整个分析停止，也不得成为发明新传统规则的许可。

本 Stage 只使用当前 V4 已有的明确组合知识，不导入或穷举 Renhuai123 双星规则。

## 2. Pattern condition layers

| Layer | Definition | Use |
|---|---|---|
| `REQUIRED` | 候选结构成立必需的条件 | 缺少时不得输出完整结构结论 |
| `REINFORCING` | 已成立结构的增强条件 | 只说明增强，不作为独立投票累加 |
| `BREAKING` | 削弱、限制、改变或破坏现实表现的因素 | 说明改变机制；不自动等于完全反向 |

同一 physical/source evidence 的不同视图不得同时充当多个条件层的独立票。

## 3. Pattern completeness

| Status | Gate | Allowed output |
|---|---|---|
| `COMPLETE` | Required 完整，且无主导 Breaking | 可使用条件式完整结构描述；仍不保证现实结果 |
| `PARTIAL` | 有明显结构，但 Required 不完整 | 只写“有这个象 / partial candidate”；不得套用完整格结果 |
| `BROKEN` | 主体存在，但 Breaking 显著改变其表现 | 同时写原始结构与破坏机制；不得当作 Complete |
| `INACTIVE` | Required 不成立 | 不得因为名称或排列相似而使用该格结论 |

`PARTIAL != COMPLETE`，`BROKEN != COMPLETE`，`BREAKING != REVERSE_RESULT`。

## 4. Boundary

这是一套 Reasoning Grammar，不是传统格局全集。不得穷举所有格局、星曜排列或结果。遇到新组合时，Strong Reasoner 应现场应用 Required / Reinforcing / Breaking / Completeness，并保留来源、冲突、边界和不确定性。
