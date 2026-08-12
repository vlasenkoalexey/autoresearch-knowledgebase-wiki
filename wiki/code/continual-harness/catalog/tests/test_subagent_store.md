---
title: 'Module: tests/test_subagent_store.py'
type: catalog
provenance: extracted
module: tests/test_subagent_store.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_subagent_store`/
symbols:
  TestSubagentEntry.test_defaults: TestSubagentEntry#test_defaults().
  TestPersistence.test_deserialization_defaults: TestPersistence#test_deserialization_defaults().
  TestSubagentEntry.test_roundtrip_via_asdict: TestSubagentEntry#test_roundtrip_via_asdict().
  TestPersistence.test_save_load_roundtrip: TestPersistence#test_save_load_roundtrip().
  TestSubagentEntry.test_name_title_sync_from_name: TestSubagentEntry#test_name_title_sync_from_name().
  TestSubagentEntry.test_name_title_sync_from_title: TestSubagentEntry#test_name_title_sync_from_title().
  TestSubagentEntry.test_created_at_auto: TestSubagentEntry#test_created_at_auto().
  TestBuiltinSeeding.test_does_not_double_seed: TestBuiltinSeeding#test_does_not_double_seed().
  TestTreeOverview.test_empty_custom_store_shows_only_builtins: TestTreeOverview#test_empty_custom_store_shows_only_builtins().
  TestCharCap.test_add_accepts_at_limit: TestCharCap#test_add_accepts_at_limit().
  store: store().
  TestBuiltinSeeding.test_seeds_on_empty_store: TestBuiltinSeeding#test_seeds_on_empty_store().
  TestCharCap.test_add_rejects_oversized_instructions: TestCharCap#test_add_rejects_oversized_instructions().
  TestCharCap.test_add_rejects_oversized_directive: TestCharCap#test_add_rejects_oversized_directive().
  TestCharCap.test_update_rejects_oversized_instructions: TestCharCap#test_update_rejects_oversized_instructions().
  TestCharCap.test_update_rejects_oversized_directive: TestCharCap#test_update_rejects_oversized_directive().
  TestSubagentEntry: TestSubagentEntry#
  TestBuiltinSeeding: TestBuiltinSeeding#
  TestBuiltinSeeding.test_builtin_entries_are_read_only_records: TestBuiltinSeeding#test_builtin_entries_are_read_only_records().
  TestCRUD: TestCRUD#
  TestCRUD.test_add_custom_subagent: TestCRUD#test_add_custom_subagent().
  TestCRUD.test_read_custom_subagent: TestCRUD#test_read_custom_subagent().
  TestCRUD.test_update_custom_subagent: TestCRUD#test_update_custom_subagent().
  TestCRUD.test_delete_custom_subagent: TestCRUD#test_delete_custom_subagent().
  TestDeleteProtection: TestDeleteProtection#
  TestDeleteProtection.test_cannot_delete_builtin: TestDeleteProtection#test_cannot_delete_builtin().
  TestDeleteProtection.test_can_update_builtin_description: TestDeleteProtection#test_can_update_builtin_description().
  TestTreeOverview: TestTreeOverview#
  TestTreeOverview.test_overview_shows_builtins: TestTreeOverview#test_overview_shows_builtins().
  TestTreeOverview.test_overview_shows_custom: TestTreeOverview#test_overview_shows_custom().
  TestDisplayDict: TestDisplayDict#
  TestDisplayDict.test_excludes_sensitive_fields: TestDisplayDict#test_excludes_sensitive_fields().
  TestDisplayDict.test_excludes_internal_fields: TestDisplayDict#test_excludes_internal_fields().
  TestCharCap: TestCharCap#
  TestPersistence: TestPersistence#
---
# Module: [`tests/test_subagent_store.py`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py)

## Classes
### `TestBuiltinSeeding`
- def: [`tests/test_subagent_store.py:67`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L67)
- signature: `class TestBuiltinSeeding:`
- members:
  - `test_builtin_entries_are_read_only_records(self, store)` — [`L82`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L82)
  - `test_does_not_double_seed(self, tmp_path)` — [`L76`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L76)
  - `test_seeds_on_empty_store(self, store)` — [`L68`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L68)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`SubagentStore`](../utils/stores/subagents.md#SubagentStore), [`BUILTIN_SUBAGENT_CONFIGS`](../utils/stores/subagents.md#BUILTIN_SUBAGENT_CONFIGS.BUILTIN_SUBAGENT_CONFIGS)

### `TestCRUD`
- def: [`tests/test_subagent_store.py:93`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L93)
- signature: `class TestCRUD:`
- members:
  - `test_add_custom_subagent(self, store)` — [`L94`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L94)
  - `test_delete_custom_subagent(self, store)` — [`L116`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L116)
  - `test_read_custom_subagent(self, store)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L105)
  - `test_update_custom_subagent(self, store)` — [`L110`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L110)

### `TestCharCap`
- def: [`tests/test_subagent_store.py:193`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L193)
- signature: `class TestCharCap:`
- members:
  - `test_add_accepts_at_limit(self, store)` — [`L218`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L218)
  - `test_add_rejects_oversized_directive(self, store)` — [`L201`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L201)
  - `test_add_rejects_oversized_instructions(self, store)` — [`L194`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L194)
  - `test_update_rejects_oversized_directive(self, store)` — [`L213`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L213)
  - `test_update_rejects_oversized_instructions(self, store)` — [`L208`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L208)
- uses (calls/refs, reference-scoped): [`MAX_DIRECTIVE_LEN`](../utils/stores/subagents.md#MAX_DIRECTIVE_LEN), [`MAX_INSTRUCTIONS_LEN`](../utils/stores/subagents.md#MAX_INSTRUCTIONS_LEN)

### `TestDeleteProtection`
- def: [`tests/test_subagent_store.py:126`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L126)
- signature: `class TestDeleteProtection:`
- members:
  - `test_can_update_builtin_description(self, store)` — [`L134`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L134) — Built-ins can be updated (e.g. description) but not deleted.
  - `test_cannot_delete_builtin(self, store)` — [`L127`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L127)

### `TestDisplayDict`
- def: [`tests/test_subagent_store.py:170`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L170)
- signature: `class TestDisplayDict:`
- members:
  - `test_excludes_internal_fields(self, store)` — [`L181`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L181)
  - `test_excludes_sensitive_fields(self, store)` — [`L171`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L171)

### `TestPersistence`
- def: [`tests/test_subagent_store.py:231`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L231)
- signature: `class TestPersistence:`
- members:
  - `test_deserialization_defaults(self, tmp_path)` — [`L242`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L242) — Entries missing optional fields get defaults from _deserialize_entry.
  - `test_save_load_roundtrip(self, tmp_path)` — [`L232`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L232)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`get`](../utils/stores/base_store.md#BaseStore.get), [`SubagentStore`](../utils/stores/subagents.md#SubagentStore), [`add`](../utils/stores/subagents.md#SubagentStore.add), [`name`](../utils/stores/subagents.md#SubagentEntry.name), [`title`](../utils/stores/subagents.md#SubagentEntry.title), [`available_tools`](../utils/stores/subagents.md#SubagentEntry.available_tools), [`is_builtin`](../utils/stores/subagents.md#SubagentEntry.is_builtin), [`max_turns`](../utils/stores/subagents.md#SubagentEntry.max_turns), [`handler_type`](../utils/stores/subagents.md#SubagentEntry.handler_type)

### `TestSubagentEntry`
- def: [`tests/test_subagent_store.py:30`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L30)
- signature: `class TestSubagentEntry:`
- members:
  - `test_created_at_auto(self)` — [`L47`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L47)
  - `test_defaults(self)` — [`L31`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L31)
  - `test_name_title_sync_from_name(self)` — [`L39`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L39)
  - `test_name_title_sync_from_title(self)` — [`L43`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L43)
  - `test_roundtrip_via_asdict(self)` — [`L52`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L52)
- uses (calls/refs, reference-scoped): [`SubagentEntry`](../utils/stores/subagents.md#SubagentEntry), [`name`](../utils/stores/subagents.md#SubagentEntry.name), [`title`](../utils/stores/subagents.md#SubagentEntry.title), [`available_tools`](../utils/stores/subagents.md#SubagentEntry.available_tools), [`created_at`](../utils/stores/subagents.md#SubagentEntry.created_at), [`is_builtin`](../utils/stores/subagents.md#SubagentEntry.is_builtin), [`max_turns`](../utils/stores/subagents.md#SubagentEntry.max_turns), [`updated_at`](../utils/stores/subagents.md#SubagentEntry.updated_at), [`handler_type`](../utils/stores/subagents.md#SubagentEntry.handler_type), [`id`](../utils/stores/subagents.md#SubagentEntry.id), [`path`](../utils/stores/subagents.md#SubagentEntry.path), [`source`](../utils/stores/subagents.md#SubagentEntry.source)

### `TestTreeOverview`
- def: [`tests/test_subagent_store.py:148`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L148)
- signature: `class TestTreeOverview:`
- members:
  - `test_empty_custom_store_shows_only_builtins(self, tmp_path)` — [`L159`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L159)
  - `test_overview_shows_builtins(self, store)` — [`L149`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L149)
  - `test_overview_shows_custom(self, store)` — [`L154`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L154)
- uses (calls/refs, reference-scoped): [`get_tree_overview`](../utils/stores/base_store.md#BaseStore.get_tree_overview), [`SubagentStore`](../utils/stores/subagents.md#SubagentStore)

## Functions
- `store(tmp_path)` — [`L22`](../../../../../raw/code/continual-harness/tests/test_subagent_store.py#L22)

