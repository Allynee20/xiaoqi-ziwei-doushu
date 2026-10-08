# KNOWLEDGE_GAP Protocol

Status: `ACCEPTED_CORE`

When a required Primitive, Grammar, Context, Exception or active-Profile rule is missing, conflicting without a permitted resolution, or insufficient for the requested claim, the Reasoner must stop that claim and emit:

```json
{
  "event_type": "KNOWLEDGE_GAP",
  "gap_id": "stable-id",
  "topic": "topic-or-dimension",
  "missing_knowledge": "what is missing",
  "current_evidence": ["traceable evidence already present"],
  "why_not_enough": "why the available evidence cannot support the claim",
  "profile": "V4_DEFAULT_SANHE_COMPATIBLE_PROFILE",
  "external_research_needed": "YES"
}
```

`external_research_needed` is `YES` only after local Canonical/Archive paths have been checked and the issue is locally absent or irreducibly conflicting. Default Web access remains OFF. The event is machine-readable and may coexist with supported conclusions on other dimensions, but the unsupported claim itself must stop.

