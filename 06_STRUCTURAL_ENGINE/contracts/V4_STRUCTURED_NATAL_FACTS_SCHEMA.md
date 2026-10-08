# V4 Structured Natal Facts Schema

Machine authority: `V4_STRUCTURED_NATAL_FACTS_SCHEMA.json`  
Status: `ACCEPTED_CORE`

## Pipeline

```text
BirthProfile
→ Workbench normalizeBirth
→ iztro 2.5.8
→ V4_STRUCTURED_NATAL_FACTS
```

The adapter keeps only deterministic semantic input: explicit Profile/table/policy IDs; stable calendar facts; Life/Body palaces; five-phase bureau; 12 physical palaces and their stems/branches; all stars by category; natal transform binding; raw brightness with provider/table provenance; opposite/sanfang topology; borrow eligibility and complete opposite main-star group; source identity; decade data.

Excluded fields include copyright year, timestamps, UI metadata, runtime notices and query-date-dependent output. Annual or finer dynamic facts require a separately fixed `as_of` and are not smuggled into natal facts.

## Source identity rules

- each star has one deterministic `star_id` under its physical palace;
- `physical_palace_id` and `source_star_id` remain unchanged in relation/borrow views;
- `relocated` is always false;
- transforms and raw brightness remain star/source-bound;
- an empty palace keeps local stars and facts while borrowing the complete opposite main-star group as a view.

## Default interpretation switches

Brightness semantics, flying transform/DTR and small limit are all OFF. Their raw facts or archived material cannot be consumed without an explicit compatible Profile.

