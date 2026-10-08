# Transform Table Policy

Status: `ACCEPTED_CORE` policy with a `PROFILE_SPECIFIC` default table.

```text
DEFAULT_TRANSFORM_TABLE_ID = IZTRO_2_5_8_DEFAULT_TRANSFORM_TABLE
```

The default profile uses the same frozen table ID for natal, decade and annual transforms. Any other Profile must declare its own `transform_table_id`. A reasoning run must not mix tables.

This is the Project Default Construction Policy. It does not claim that iztro or this table is the uniquely correct historical version.

