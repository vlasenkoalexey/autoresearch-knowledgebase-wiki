---
title: 'Module: tests/test_memory.py'
type: catalog
provenance: extracted
module: tests/test_memory.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_memory`/
symbols:
  TestMemoryEntrySerde.test_defaults: TestMemoryEntrySerde#test_defaults().
  sys_path: sys_path.
  TestMemoryEntrySerde.test_coordinates_stored_as_tuple: TestMemoryEntrySerde#test_coordinates_stored_as_tuple().
  TestMigration.test_auto_migrates_knowledge_base_to_memory: TestMigration#test_auto_migrates_knowledge_base_to_memory().
  TestMemoryStore.test_update_entry: TestMemoryStore#test_update_entry().
  TestMemoryStore.test_clear: TestMemoryStore#test_clear().
  TestMemoryStore.test_source_and_step_fields: TestMemoryStore#test_source_and_step_fields().
  TestMemoryEntrySerde.test_path_field_replaces_category: TestMemoryEntrySerde#test_path_field_replaces_category().
  TestMemoryStore.test_add_with_path: TestMemoryStore#test_add_with_path().
  TestMemoryStore.test_add_with_category_backward_compat: TestMemoryStore#test_add_with_category_backward_compat().
  TestMemoryStore.test_save_and_reload: TestMemoryStore#test_save_and_reload().
  TestMemoryStore.test_remove_entry: TestMemoryStore#test_remove_entry().
  TestMemoryStore.test_coordinates_round_trip: TestMemoryStore#test_coordinates_round_trip().
  TestMigration.test_category_migrated_to_path: TestMigration#test_category_migrated_to_path().
  TestMemoryStore.test_search_by_path_prefix: TestMemoryStore#test_search_by_path_prefix().
  TestMemoryStore.test_search_backward_compat_category_kwarg: TestMemoryStore#test_search_backward_compat_category_kwarg().
  TestMemoryStore.test_summary_with_entries: TestMemoryStore#test_summary_with_entries().
  TestMemoryStore.test_tree_overview: TestMemoryStore#test_tree_overview().
  TestMemoryStore.test_get_all_by_path: TestMemoryStore#test_get_all_by_path().
  TestMigration.test_no_migration_when_memory_already_exists: TestMigration#test_no_migration_when_memory_already_exists().
  TestMigration.test_migration_preserves_next_id: TestMigration#test_migration_preserves_next_id().
  TestMigration.test_deserialization_handles_mixed_category_and_path: TestMigration#test_deserialization_handles_mixed_category_and_path().
  TestMemoryEntrySerde.test_backward_compat_alias: TestMemoryEntrySerde#test_backward_compat_alias().
  TestMemoryStore.test_summary_empty: TestMemoryStore#test_summary_empty().
  TestMemoryStore.test_backward_compat_class_alias: TestMemoryStore#test_backward_compat_class_alias().
  TestGetMemoryStore.test_returns_same_instance: TestGetMemoryStore#test_returns_same_instance().
  TestMigration._write_legacy_kb: TestMigration#_write_legacy_kb().
  TestMemoryEntrySerde: TestMemoryEntrySerde#
  TestMemoryStore: TestMemoryStore#
  TestMigration: TestMigration#
  TestGetMemoryStore: TestGetMemoryStore#
---
# Module: [`tests/test_memory.py`](../../../../../raw/code/continual-harness/tests/test_memory.py)

## Classes
### `TestGetMemoryStore`
- def: [`tests/test_memory.py:263`](../../../../../raw/code/continual-harness/tests/test_memory.py#L263)
- signature: `class TestGetMemoryStore:`
- members:
  - `test_returns_same_instance(self, tmp_path)` — [`L264`](../../../../../raw/code/continual-harness/tests/test_memory.py#L264)
- uses (calls/refs, reference-scoped): [`get_memory_store`](../utils/stores/memory.md#get_memory_store), [`_memory_store`](../utils/stores/memory.md#_memory_store._memory_store)

### `TestMemoryEntrySerde`
- def: [`tests/test_memory.py:23`](../../../../../raw/code/continual-harness/tests/test_memory.py#L23)
- signature: `class TestMemoryEntrySerde:`
- members:
  - `test_backward_compat_alias(self)` — [`L32`](../../../../../raw/code/continual-harness/tests/test_memory.py#L32)
  - `test_coordinates_stored_as_tuple(self)` — [`L35`](../../../../../raw/code/continual-harness/tests/test_memory.py#L35)
  - `test_defaults(self)` — [`L24`](../../../../../raw/code/continual-harness/tests/test_memory.py#L24)
  - `test_path_field_replaces_category(self)` — [`L39`](../../../../../raw/code/continual-harness/tests/test_memory.py#L39)
- uses (calls/refs, reference-scoped): [`MemoryEntry`](../utils/stores/memory.md#MemoryEntry), [`path`](../utils/stores/memory.md#MemoryEntry.path), [`coordinates`](../utils/stores/memory.md#MemoryEntry.coordinates), [`KnowledgeEntry`](../utils/stores/memory.md#KnowledgeEntry), [`content`](../utils/stores/memory.md#MemoryEntry.content), [`created_at`](../utils/stores/memory.md#MemoryEntry.created_at), [`importance`](../utils/stores/memory.md#MemoryEntry.importance), [`title`](../utils/stores/memory.md#MemoryEntry.title), [`id`](../utils/stores/memory.md#MemoryEntry.id), [`last_modified_step`](../utils/stores/memory.md#MemoryEntry.last_modified_step), [`source`](../utils/stores/memory.md#MemoryEntry.source), [`mutation_history`](../utils/stores/memory.md#MemoryEntry.mutation_history)

### `TestMemoryStore`
- def: [`tests/test_memory.py:50`](../../../../../raw/code/continual-harness/tests/test_memory.py#L50)
- signature: `class TestMemoryStore:`
- members:
  - `test_add_with_category_backward_compat(self, tmp_path)` — [`L57`](../../../../../raw/code/continual-harness/tests/test_memory.py#L57)
  - `test_add_with_path(self, tmp_path)` — [`L51`](../../../../../raw/code/continual-harness/tests/test_memory.py#L51)
  - `test_backward_compat_class_alias(self, tmp_path)` — [`L125`](../../../../../raw/code/continual-harness/tests/test_memory.py#L125)
  - `test_clear(self, tmp_path)` — [`L118`](../../../../../raw/code/continual-harness/tests/test_memory.py#L118)
  - `test_coordinates_round_trip(self, tmp_path)` — [`L141`](../../../../../raw/code/continual-harness/tests/test_memory.py#L141)
  - `test_get_all_by_path(self, tmp_path)` — [`L150`](../../../../../raw/code/continual-harness/tests/test_memory.py#L150)
  - `test_remove_entry(self, tmp_path)` — [`L112`](../../../../../raw/code/continual-harness/tests/test_memory.py#L112)
  - `test_save_and_reload(self, tmp_path)` — [`L77`](../../../../../raw/code/continual-harness/tests/test_memory.py#L77)
  - `test_search_backward_compat_category_kwarg(self, tmp_path)` — [`L71`](../../../../../raw/code/continual-harness/tests/test_memory.py#L71)
  - `test_search_by_path_prefix(self, tmp_path)` — [`L62`](../../../../../raw/code/continual-harness/tests/test_memory.py#L62)
  - `test_source_and_step_fields(self, tmp_path)` — [`L128`](../../../../../raw/code/continual-harness/tests/test_memory.py#L128)
  - `test_summary_empty(self, tmp_path)` — [`L86`](../../../../../raw/code/continual-harness/tests/test_memory.py#L86)
  - `test_summary_with_entries(self, tmp_path)` — [`L90`](../../../../../raw/code/continual-harness/tests/test_memory.py#L90)
  - `test_tree_overview(self, tmp_path)` — [`L97`](../../../../../raw/code/continual-harness/tests/test_memory.py#L97)
  - `test_update_entry(self, tmp_path)` — [`L106`](../../../../../raw/code/continual-harness/tests/test_memory.py#L106)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`Memory`](../utils/stores/memory.md#Memory), [`get_tree_overview`](../utils/stores/base_store.md#BaseStore.get_tree_overview), [`add`](../utils/stores/memory.md#Memory.add), [`get`](../utils/stores/base_store.md#BaseStore.get), [`search`](../utils/stores/memory.md#Memory.search), [`update`](../utils/stores/base_store.md#BaseStore.update), [`remove`](../utils/stores/base_store.md#BaseStore.remove), [`clear`](../utils/stores/base_store.md#BaseStore.clear), [`get_summary`](../utils/stores/memory.md#Memory.get_summary), [`path`](../utils/stores/memory.md#MemoryEntry.path), [`next_id`](../utils/stores/base_store.md#BaseStore.next_id), [`get_all`](../utils/stores/memory.md#Memory.get_all), [`coordinates`](../utils/stores/memory.md#MemoryEntry.coordinates), [`KnowledgeBase`](../utils/stores/memory.md#KnowledgeBase), [`content`](../utils/stores/memory.md#MemoryEntry.content), [`last_modified_step`](../utils/stores/memory.md#MemoryEntry.last_modified_step), [`source`](../utils/stores/memory.md#MemoryEntry.source)

### `TestMigration`
- def: [`tests/test_memory.py:164`](../../../../../raw/code/continual-harness/tests/test_memory.py#L164)
- signature: `class TestMigration:`
- members:
  - `_write_legacy_kb(self, cache_dir: Path)` — [`L165`](../../../../../raw/code/continual-harness/tests/test_memory.py#L165) — Write a knowledge_base.json in the legacy format (with category field).
  - `test_auto_migrates_knowledge_base_to_memory(self, tmp_path)` — [`L199`](../../../../../raw/code/continual-harness/tests/test_memory.py#L199)
  - `test_category_migrated_to_path(self, tmp_path)` — [`L212`](../../../../../raw/code/continual-harness/tests/test_memory.py#L212)
  - `test_deserialization_handles_mixed_category_and_path(self, tmp_path)` — [`L231`](../../../../../raw/code/continual-harness/tests/test_memory.py#L231) — Entries with both category and path fields — path wins.
  - `test_migration_preserves_next_id(self, tmp_path)` — [`L226`](../../../../../raw/code/continual-harness/tests/test_memory.py#L226)
  - `test_no_migration_when_memory_already_exists(self, tmp_path)` — [`L218`](../../../../../raw/code/continual-harness/tests/test_memory.py#L218)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`Memory`](../utils/stores/memory.md#Memory), [`path`](../utils/stores/memory.md#MemoryEntry.path), [`next_id`](../utils/stores/base_store.md#BaseStore.next_id), [`coordinates`](../utils/stores/memory.md#MemoryEntry.coordinates), [`last_modified_step`](../utils/stores/memory.md#MemoryEntry.last_modified_step), [`source`](../utils/stores/memory.md#MemoryEntry.source)

## Module values
- `sys_path` — [`L11`](../../../../../raw/code/continual-harness/tests/test_memory.py#L11)

