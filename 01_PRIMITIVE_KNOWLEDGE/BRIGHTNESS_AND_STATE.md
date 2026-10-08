# Brightness and State

Status: `ACCEPTED_CORE` for transport policy; semantic interpretation is `PROFILE_SPECIFIC`.

V4 Core stores only raw state and provenance:

```text
raw_state
source
provider
table_version
semantic_consumption = OFF
```

Default policy:

```text
BRIGHTNESS_SEMANTIC_CONSUMPTION = OFF
```

Core does not interpret 庙/旺/得/利/平/不/陷. In particular, it forbids:

```text
庙 = 好
陷 = 坏
庙 = 强
陷 = 弱
```

The seven labels are not an equal-interval scale and cannot be converted into numeric weights. Raw brightness remains bound to its physical source star and source table, including in a borrowed view. It is not consumed again across time or relation views.

Any future semantic use must name a Profile, source/provider and table version. Profiles that disagree remain isolated; their meanings cannot be merged into Core.
