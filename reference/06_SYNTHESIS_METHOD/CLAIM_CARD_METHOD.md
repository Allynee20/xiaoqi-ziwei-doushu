# User-facing Claim Card Method

Status: `REQUIRED_INTERNAL_SCHEMA`  
Schema type: `PROJECT_SCHEMA`

每条 Important Claim 在内部先整理为：

```text
CLAIM
WHY
BOUNDARY
OPTIONAL_SOFT_SIGNAL
```

- `CLAIM`：用户真正需要知道的一句话，必须落到当前现实维度。
- `WHY`：2–4 条真正参与判断、可回指 source identity 的证据链；相关视图不可重复计数。
- `BOUNDARY`：合并 nearest cannot-imply 与可观察 miss condition；说明什么没有被证明、什么现实出现时应降级。
- `OPTIONAL_SOFT_SIGNAL`：仅在增加区分度且通过 Soft Signal Guard 时加入；不得补救 Core 证据不足。

Claim Card 是内部组织方式。最终用户报告不得机械打印字段名，应把四部分写成自然语言。Anti-Barnum 五段式仍作为验证记录：`WHY` 承载 Evidence/Dimension/Contrast，`BOUNDARY` 承载 Cannot Imply/Miss Condition；两套协议不得丢字段。
