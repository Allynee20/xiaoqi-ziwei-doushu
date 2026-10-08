# Family Wealth Scope Guard

Status: `REQUIRED_DEFAULT_GUARD`

> Current V4 cannot reliably infer ordinary / affluent / very wealthy / ultra-wealthy family-of-origin levels from the subject's natal chart alone.

默认用户报告禁止把以下内容作为强结论：

- 你出生在普通家庭；
- 你家属于中产；
- 你家比较富；
- 你家是高资源家庭；
- 你父母财富很强。

Family / Parents 结构仍可在用户按需询问时描述 support mechanism、resource-access candidate、institutional/educational support 与 relationship mechanism，但必须同时保留：

```text
SUPPORT != FAMILY WEALTH
RESOURCE SIGNAL != WEALTH LEVEL
CHILD CHART != RELIABLE PARENT NET-WORTH ESTIMATOR
WEALTH ACCESS != SELF_EARNED WEALTH
```

`NATAL_RESOURCE_BASELINE != DEFAULT USER-FACING TOTAL WEALTH CLASS`。内部的 `ORDINARY_RESOURCE_STRUCTURE / AFFLUENT_RESOURCE_STRUCTURE / HIGH_WEALTH_CAPACITY_STRUCTURE` 继续保留作项目推理 Schema，但 Simple Report 不得将其翻译成“本命财富普通、小富或高资源”。默认改写为本人收入路径、价值创造、留存/侵蚀候选和对职业参与的依赖。

没有明确用户背景或独立、正面可用的结论时，家庭财富、配偶财富、继承及被动资源依赖在内部保留为 `UNKNOWN`。该未知状态不得渲染为“没有家庭支持 / 配偶资源 / 继承”，也不以“本报告不判断家庭财富”等话语向用户解释；相关内容默认完全省略。只有用户主动询问且已有正面可输出内容时，才按问题范围作答。
