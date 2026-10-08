# Soft Signal Output Schema

Each stored signal is one structured record with exactly these required fields:

```yaml
signal_id: <representative library ID or a concise new traceable ID>
domain: <CAREER | WEALTH | MARRIAGE | DECADE>
strength: <CLEAR_TENDENCY | HAS_SIGNAL | AUXILIARY_ONLY>
evidence_summary: <concise physical/source-layer facts>
independent_evidence_paths:
  - path_id: <stable evidence path>
    source_identity: <physical/source identity>
cannot_imply: <nearest forbidden upgrade>
conflict_status: <NONE | CORE_PRIORITY_SUPPRESSED | CONFLICT_DISCLOSED>
user_facing_sentence: <conditional, non-inevitable sentence>
```

Validation requirements:

- `independent_evidence_paths` contains no duplicate source identity;
- `CLEAR_TENDENCY` has at least two paths;
- `HAS_SIGNAL` has at least one path and must not be phrased as inevitable;
- `AUXILIARY_ONLY` is hidden unless the user explicitly asks the domain;
- mechanical topology cannot appear as a path;
- no signal may change a Core classification or be counted back into Core;
- proactive Natal output contains no more than five records.
- an ID absent from the representative library must still be defined by its evidence in this record; it does not create a reusable Core rule.
