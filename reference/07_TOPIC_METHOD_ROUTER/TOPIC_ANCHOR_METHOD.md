# Topic Anchor Method

Status: `REQUIRED_ROUTING_METHOD`

`TOPIC_ANCHOR` 决定当前问题的主线结构；`SUPPORTING_STRUCTURES` 提供条件、资源、成本、留存、关系与时间背景。

硬规则：

```text
TOPIC_ANCHOR != SOLE_EVIDENCE
SUPPORTING_STRUCTURE != REPLACEMENT_ANCHOR
```

## Public v1 default route

默认分析范围为 `PERSON / WORK_VALUE_CREATION / RELATIONSHIP`，仅使用本命结构。先按用户问题选取与这三个模块有关的 Topic 和子问题；财富相关信息只有在能独立支持本人收入或价值转收入时，才作为 Work 模块的补充，不生成强制财富章节。大运、流年、人生阶段和 Dynamic Facts 不属于默认路由（均为 `OFF`）。

| Topic | Anchor | Supporting structures |
|---|---|---|
| `CAREER` | Career structure | Life / Body、Wealth、Mobility、Fortune、Composition、Transform、Timing |
| `WEALTH` | Wealth structure | Career formation、Asset / Property、Family resource、Spouse-side resource、Retention、Timing |
| `MARRIAGE` | Spouse structure | Life / Body、Fortune、Resource、Reality formalization、Timing |

Anchor 不是单宫独断。Reasoner 必须从 Anchor 建立问题接口，再用至少一条合法组合链解释 Supporting Structure 如何支持、限制或改变它。Supporting Structure 不能越权成为另一个 Topic 的现实事实；相同 evidence identity 只消费一次。默认路由限制用户报告主题，不修改任何结构知识或可选的内部方法。
