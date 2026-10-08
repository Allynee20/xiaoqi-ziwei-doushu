# Uncertainty Policy

以下是内部分类与处理要求；普通用户呈现另按 `USER_REPORTS/FINAL_USER_REPORT_PROTOCOL.md` 投影。

| 状态 | 内部含义 | 内部处理 |
|---|---|---|
| `SUPPORTED` | 现有 V4 知识与盘面事实形成可追溯支持 | 记录主线、支持与边界 |
| `PARTIAL` | 有部分支持，但覆盖、条件或直接性不完整 | 保留已支持部分；缺口仅记在内部 |
| `CONFLICTED` | 同一问题的相关证据真冲突且无授权解法 | 并列冲突，不强行裁决 |
| `UNRESOLVED` | 旧资产自身未冻结、历史争议未解决或 V4 尚未迁入 | 内部明确停点；必要时生成独立机器可读 Knowledge Gap 事件 |
| `INSUFFICIENT` | 当前盘面输入或所需证据不足 | 不推正面或负面结论 |
| `UNKNOWN` | 资料、背景或观察范围没有确定该项的值 | 保持未知，不转成正面或负面结论 |

补充边界：`NO_EVIDENCE != CONFLICTED`；absence/unknown/no proposition 都不等于 negative。只有明确知识与完整观察范围支持时，才可表达负向判断；V4 Stage 1 不预设封闭世界。

上述状态与处理要求属于内部推理 / 审计层。投影为普通用户报告时，默认按 `USER_REPORTS/FINAL_USER_REPORT_PROTOCOL.md` 静默省略 `UNKNOWN / UNRESOLVED / INSUFFICIENT / OUT_OF_SCOPE / NO SUPPORT`；不得把状态解释、证据缺口或范围关闭转写成用户免责声明。只有为避免误导某条已输出的核心判断时，才允许保留最短的自然语言限定。
