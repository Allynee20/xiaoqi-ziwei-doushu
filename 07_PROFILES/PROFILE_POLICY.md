# Profile Policy

1. Every run records `profile_id` and `transform_table_id`.
2. One run uses one profile and one transform table.
3. A profile may consume only rules explicitly assigned to it.
4. Missing profile knowledge produces `KNOWLEDGE_GAP`; it is not silently borrowed from another profile.
5. Brightness is raw provenance only unless the selected profile explicitly enables semantic consumption.
6. `SMALL_LIMIT = OFF` and `FLYING_TRANSFORM = OFF` in the default profile.
7. Named/school-specific rules never become Core by repetition or popularity.

