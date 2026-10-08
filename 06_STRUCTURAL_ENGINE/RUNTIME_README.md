# Public Natal Runtime

Requires Node.js 20 or later. The committed Natal bundle is self-contained; do not install packages or rebuild it.

## Fixed runtime policy

- Chart engine: pinned `iztro` `2.5.8`.
- Profile: `V4_DEFAULT_SANHE_COMPATIBLE_PROFILE`.
- Transform table: `IZTRO_2_5_8_DEFAULT_TRANSFORM_TABLE`.
- True Solar Time default: `OFF`.
- Brightness semantic consumption: `OFF`.
- Small limit: `OFF`.
- Flying transform: `OFF`.
- DTR: `OFF`.
- Dynamic / Decade / Annual runtime: not included in the Public v1 package; default usage is `OFF`.

## Generate Natal Structured Facts

Convert only the separately supplied birth information into the accepted BirthProfile fields. Keep the temporary input outside this public directory. Run:

```text
node 06_STRUCTURAL_ENGINE/runtime/birth/birth_to_structured_facts.bundle.cjs --input <birth-profile.json> --pretty
```

Validate the output against:

```text
06_STRUCTURAL_ENGINE/contracts/V4_STRUCTURED_NATAL_FACTS_SCHEMA.json
```

The runtime emits chart facts only, never topic interpretation or user-report text. Do not retain temporary input or output in the public package.
