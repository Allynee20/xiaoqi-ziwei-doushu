# Zi Wei Strong Reasoner Reference

## What this repository is

This is a compact public reference for using a strong reasoning model to interpret Zi Wei Dou Shu charts. It does not encode every possible chart combination or replace reasoning with lookup tables. It provides deterministic natal chart facts, primitive semantics, composition boundaries, inference guards, and a user-report protocol. The Strong Reasoner performs synthesis, evidence weighting, conflict handling, and final language.

## Default public scope

Public v1 focuses on a person's stable natal operating mechanisms. The default report contains only:

1. How the person naturally operates.
2. How they work and create value.
3. How they operate in intimate relationships.

An optional 2–4 sentence summary may only compress those three sections. Money-related information belongs inside the work/value section only when it has distinct positive support; a separate wealth chapter is not forced.

Future decade prediction, annual prediction, lifecycle analysis, health diagnosis, family wealth classification, exact occupation, exact income or net worth, marriage count, and exact marriage timing are not part of the default public product scope. This is a default-scope boundary, not a claim that every such topic is permanently impossible.

## START HERE — Fresh Strong Reasoner reading path

Read in this order. Do not recursively browse the repository or load unrelated archives.

1. This `README.md`.
2. [`FRESH_WINDOW_RUN_INSTRUCTIONS.md`](FRESH_WINDOW_RUN_INSTRUCTIONS.md).
3. [`reference/README.md`](reference/README.md), then its linked public path in order: `01_SYSTEM_AND_CHART` → `02_PRIMITIVE_SEMANTICS` → `03_QUESTION_AND_ROLE` → `04_STRUCTURAL_MODIFIERS` → `05_COMPOSITION_AND_RELATIONS` → `06_SYNTHESIS_METHOD` → `07_TOPIC_METHOD_ROUTER` → `09_VARIANTS_AND_UNRESOLVED` → `10_RUNTIME_PROTOCOL`.
4. The applicable linked canonical knowledge and report protocols; do not expand to unrelated topics.
5. The default Profile and Natal runtime instructions/schema only when chart facts must be generated: `07_PROFILES/PROFILE_POLICY.md`, `07_PROFILES/V4_DEFAULT_SANHE_COMPATIBLE_PROFILE.json`, `06_STRUCTURAL_ENGINE/RUNTIME_README.md`, and `06_STRUCTURAL_ENGINE/contracts/V4_STRUCTURED_NATAL_FACTS_SCHEMA.json`.
6. The separately supplied birth input.

The public runtime generates Natal facts only. Dynamic / decade / annual runtime is intentionally not included in this default path.
