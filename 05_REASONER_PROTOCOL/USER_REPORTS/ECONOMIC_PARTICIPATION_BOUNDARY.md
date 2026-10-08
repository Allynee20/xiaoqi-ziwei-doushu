# Economic Participation Boundary

Status: `REQUIRED_ROUTING_BOUNDARY`

```text
CAREER_CAPACITY != CAREER_NECESSITY != CAREER_PARTICIPATION
WEALTH_ACCESS != SELF_EARNED_WEALTH
GENDER != ECONOMIC_PARTICIPATION
```

## Default audience assumption

只有出生资料、没有现实 Context 时，使用 `DEFAULT_REPORT_AUDIENCE = ORDINARY_ADULT_ECONOMIC_PARTICIPANT`。这只是产品视角：描述本人参与工作/专业/项目/经营时可能呈现的工作与个人收入结构；不得写成“此人一定上班或一定以事业为主”。

## Explicit context override

若用户明确说明长期不工作、职业不是生活主线、主要依赖家庭既有财富、主要依赖配偶资源、全职家庭角色、或已退休且不再参与职业，则设置：

```text
CAREER_PRIMARY = NO
```

此时 Career 只按 `CAPABILITY_IF_ACTIVATED` 弱化描述。禁止继续回答靠什么职业发财、将进入什么管理层或哪一运事业做大。报告重点转向已有证据支持的 life operating style、relationship、resource use/retention/erosion 与 decade structural change。

不得从命盘反推不想工作、富二代或一定靠配偶。Participation Context 只能来自 explicit user context；未提供时保持 unknown，并采用默认受众假设。

## Unknown resource context guard

没有 explicit user context 时，以下项目在内部保持 `UNKNOWN`，不得由未知补成肯定或否定结论：

```text
family wealth = UNKNOWN
spouse wealth = UNKNOWN
inheritance = UNKNOWN
passive resource dependence = UNKNOWN
```

`UNKNOWN_RESOURCE_CONTEXT_REMAINS_UNKNOWN = REQUIRED`。普通用户报告只写确有正面支持的本人价值创造与个人收入内容；家庭、配偶、继承及被动资源没有可输出的正面判断时保持静默。禁止把“未知”改写为“没有支持 / 不是来源”，也禁止告诉用户报告默认只分析本人收入。

## Gender guard

女性工作者与男性工作者使用相同 Career/Wealth 方法。男性或女性的非工作/家庭角色都只由显式 participation context 路由。禁止 `female → 少分析事业` 或 `male → 默认事业主线`；真正控制深度的只有 explicit participation context、user question 与 evidence relevance。
