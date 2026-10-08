# Analyze Chart Command Template

```yaml
command: ANALYZE_ZIWEI_CHART_WITH_V4_KB
user_question: "<用户原始问题>"
topic: "<WEALTH | CAREER | MARRIAGE | CROSS_TOPIC>"
subquestions:
  - "<具体子问题>"
subject_and_role_context:
  subject_ref: "<本人>"
  economic_participation: "<UNKNOWN_DEFAULT_AUDIENCE | CAREER_PRIMARY_YES | CAREER_PRIMARY_NO>"
  participation_context_source: "<EXPLICIT_USER_CONTEXT | NOT_PROVIDED>"
  known_real_world_objects: []
  unknown_or_unconfirmed_objects: []
chart_input:
  type: "<CONSTRUCTED_NATAL_CHART | STRUCTURED_NATAL_FACTS>"
  facts: "<粘贴或引用结构化事实>"
  conflicts_or_missing_fields: []
knowledge_policy:
  USE_PROJECT_KB_ONLY: YES
  WEB: OFF
  ALLOW_MODEL_MEMORY_TO_FILL_KB_GAPS: NO
  ONE_DERIVED_LAYER_MAX: YES
  MECHANICAL_TOPOLOGY_AS_EVIDENCE: FORBIDDEN
  LIFECYCLE_TEMPLATE: FORBIDDEN
analysis_depth: "<STANDARD | DEEP>"
output_requirements:
  language: "zh-CN"
  schema: "05_REASONER_PROTOCOL/FINAL_ANALYSIS_SCHEMA.md"
  report_mode: "FINAL_SIMPLE_USER_REPORT"
  internal_reasoning_visibility: "PRESERVED_NOT_PRINTED_BY_DEFAULT"
  public_product_scope: "NATAL_STRUCTURAL_ANALYSIS"
  default_modules: [PERSON, WORK_VALUE_CREATION, RELATIONSHIP]
  default_decade_analysis: "OFF"
  default_lifecycle_analysis: "OFF"
  default_future_stage_analysis: "OFF"
  default_annual_analysis: "OFF"
  default_dynamic_facts_usage: "OFF"
  wealth_section: "OPTIONAL_WITHIN_WORK_MODULE_IF_DISTINCT_POSITIVE_EVIDENCE"
  optional_summary: "2_TO_4_SENTENCES; NO_NEW_CLAIMS"
  plain_language: REQUIRED
  value_creation_question: REQUIRED_OPEN_QUESTION
  ordinary_stable_outcome: ALLOWED
  default_career_upgrade: FORBIDDEN
  gender_based_career_routing: FORBIDDEN
  family_origin_default_output: OFF
  family_wealth_level_default_output: OFF
  health_default_output: OFF
  report_sections: [PERSON, WORK_VALUE_CREATION, RELATIONSHIP]
  preserve_uncertainty: true
  trace_level: "KEY_CLAIMS"
  five_part_claim_contract: true
  sentence_swap_test: REQUIRED
  non_discriminative_status: ENABLED
  life_domains:
    career_wealth_system: REQUIRED_WHEN_IN_SCOPE
    natal_resource_baseline: REQUIRED_FOR_COMPLETE_WEALTH
    decade_band_and_delta: REQUIRED_ONLY_IF_EXPLICITLY_ENABLED
    marriage_system: REQUIRED_WHEN_IN_SCOPE
  audits:
    baseline_swap: REQUIRED_FOR_COMPARATIVE_REGRESSION
    decade_curve_swap: REQUIRED_ONLY_IF_STAGE_ANALYSIS_ENABLED
    spouse_resource_gate: REQUIRED
    no_domain_reassignment: REQUIRED
  soft_signal_layer:
    run_after_core_freeze: true
    allowed_strengths: [CLEAR_TENDENCY, HAS_SIGNAL, AUXILIARY_ONLY]
    proactive_output_min: 3
    proactive_output_max: 5
    user_display: OPTIONAL_ONLY_IF_DISCRIMINATIVE
    core_override: FORBIDDEN
    duplicate_source_identity: FORBIDDEN
```

执行要求：先分类问题与角色，再按 Context -> Primitive -> Grammar -> Pattern/Exception -> Conflict/Uncertainty -> Anti-Barnum/Discrimination -> Synthesis 顺序运行。首次报告冻结前不得提供现实经历。若发现 V4 无法支持的理论缺口，输出：

```yaml
status: KNOWLEDGE_GAP
missing_knowledge: "<具体缺口>"
affected_question: "<影响>"
existing_v4_support: "<已有但不足的内容>"
next_action: "COORDINATOR_DECIDES_WHETHER_TO_START_WORKER_BOT_OR_WEB_RESEARCH"
```
