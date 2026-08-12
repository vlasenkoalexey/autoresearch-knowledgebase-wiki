---
title: 'Module: tests/test_base_store.py'
type: catalog
provenance: extracted
module: tests/test_base_store.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_base_store`/
symbols:
  DummyStore: DummyStore#
  TestPersistence.test_save_load_roundtrip: TestPersistence#test_save_load_roundtrip().
  TestPersistence.test_auto_save_after_update: TestPersistence#test_auto_save_after_update().
  TestPersistence.test_auto_save_after_remove: TestPersistence#test_auto_save_after_remove().
  TestPersistence.test_sync_to_run_data: TestPersistence#test_sync_to_run_data().
  DummyEntry.__post_init__: DummyEntry#__post_init__().
  DummyStore.__init__: DummyStore#__init__().
  TestPersistence.test_empty_file_starts_fresh: TestPersistence#test_empty_file_starts_fresh().
  TestPersistence.test_corrupt_json_starts_fresh: TestPersistence#test_corrupt_json_starts_fresh().
  TestPersistence.test_no_file_starts_fresh: TestPersistence#test_no_file_starts_fresh().
  TestPersistence.test_auto_save_after_add: TestPersistence#test_auto_save_after_add().
  DummyEntry.created_at: DummyEntry#created_at.
  DummyStore.entry_class: DummyStore#entry_class.
  store: store().
  DummyEntry: DummyEntry#
  DummyEntry.updated_at: DummyEntry#updated_at.
  DummyEntry.title: DummyEntry#title.
  DummyEntry.id: DummyEntry#id.
  DummyEntry.path: DummyEntry#path.
  DummyEntry.content: DummyEntry#content.
  DummyEntry.importance: DummyEntry#importance.
  DummyEntry.mutation_history: DummyEntry#mutation_history.
  DummyStore.file_name: DummyStore#file_name.
  DummyStore.id_prefix: DummyStore#id_prefix.
  DummyStore.store_label: DummyStore#store_label.
  DummyStore.empty_message: DummyStore#empty_message.
  TestCRUD: TestCRUD#
  TestCRUD.test_add_returns_id: TestCRUD#test_add_returns_id().
  TestCRUD.test_add_increments_ids: TestCRUD#test_add_increments_ids().
  TestCRUD.test_get_returns_entry: TestCRUD#test_get_returns_entry().
  TestCRUD.test_get_missing_returns_none: TestCRUD#test_get_missing_returns_none().
  TestCRUD.test_get_multiple: TestCRUD#test_get_multiple().
  TestCRUD.test_update: TestCRUD#test_update().
  TestCRUD.test_update_missing_returns_false: TestCRUD#test_update_missing_returns_false().
  TestCRUD.test_remove: TestCRUD#test_remove().
  TestCRUD.test_remove_missing_returns_false: TestCRUD#test_remove_missing_returns_false().
  TestCRUD.test_clear: TestCRUD#test_clear().
  TestCRUD.test_get_all: TestCRUD#test_get_all().
  TestPersistence: TestPersistence#
  TestTreeOverview: TestTreeOverview#
  TestTreeOverview.test_empty_store: TestTreeOverview#test_empty_store().
  TestTreeOverview.test_single_entry: TestTreeOverview#test_single_entry().
  TestTreeOverview.test_nested_paths: TestTreeOverview#test_nested_paths().
  TestTreeOverview.test_max_display_cap: TestTreeOverview#test_max_display_cap().
  TestTreeOverview.test_deep_path_flattened_at_4: TestTreeOverview#test_deep_path_flattened_at_4().
  TestTreeOverview.test_uncategorized_default: TestTreeOverview#test_uncategorized_default().
  TestTreeOverview.test_unicode_in_titles: TestTreeOverview#test_unicode_in_titles().
  TestCacheInvalidation: TestCacheInvalidation#
  TestCacheInvalidation.test_add_invalidates_cache: TestCacheInvalidation#test_add_invalidates_cache().
  TestCacheInvalidation.test_update_invalidates_cache: TestCacheInvalidation#test_update_invalidates_cache().
  TestCacheInvalidation.test_remove_invalidates_cache: TestCacheInvalidation#test_remove_invalidates_cache().
  TestCacheInvalidation.test_clear_invalidates_cache: TestCacheInvalidation#test_clear_invalidates_cache().
  TestCacheInvalidation.test_repeated_read_uses_cache: TestCacheInvalidation#test_repeated_read_uses_cache().
  TestDisplayFilter: TestDisplayFilter#
  TestDisplayFilter.test_omits_internal_fields: TestDisplayFilter#test_omits_internal_fields().
---
# Module: [`tests/test_base_store.py`](../../../../../raw/code/continual-harness/tests/test_base_store.py)

## Classes
### `DummyEntry`
- def: [`tests/test_base_store.py:19`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L19)
- signature: `class DummyEntry:`
- members:
  - `content` — [`L23`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L23)
  - `created_at` — [`L25`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L25)
  - `id` — [`L20`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L20)
  - `importance` — [`L24`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L24)
  - `mutation_history` — [`L27`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L27)
  - `path` — [`L21`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L21)
  - `title` — [`L22`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L22)
  - `updated_at` — [`L26`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L26)
- protocol/private: `__post_init__`[`L29`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L29)
- used by: (3 test-only callers)

### `DummyStore`  ·  implements/extends BaseStore
- def: [`tests/test_base_store.py:37`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L37)
- signature: `class DummyStore(BaseStore[DummyEntry]):`
- members:
  - `empty_message` — [`L41`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L41)
  - `entry_class` — [`L42`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L42)
  - `file_name` — [`L38`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L38)
  - `id_prefix` — [`L39`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L39)
  - `store_label` — [`L40`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L40)
- protocol/private: `__init__`[`L44`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L44)
- uses (calls/refs, reference-scoped): [`load`](../utils/stores/base_store.md#BaseStore.load), [`BaseStore`](../utils/stores/base_store.md#BaseStore), [`__init__`](../utils/stores/base_store.md#BaseStore.__init__)  (1 test-only)
- used by: [`BaseStore`](../utils/stores/base_store.md#BaseStore)  (11 test-only)

### `TestCRUD`
- def: [`tests/test_base_store.py:62`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L62)
- signature: `class TestCRUD:`
- members:
  - `test_add_increments_ids(self, store)` — [`L68`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L68)
  - `test_add_returns_id(self, store)` — [`L63`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L63)
  - `test_clear(self, store)` — [`L108`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L108)
  - `test_get_all(self, store)` — [`L115`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L115)
  - `test_get_missing_returns_none(self, store)` — [`L80`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L80)
  - `test_get_multiple(self, store)` — [`L83`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L83)
  - `test_get_returns_entry(self, store)` — [`L74`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L74)
  - `test_remove(self, store)` — [`L99`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L99)
  - `test_remove_missing_returns_false(self, store)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L105)
  - `test_update(self, store)` — [`L89`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L89)
  - `test_update_missing_returns_false(self, store)` — [`L96`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L96)

### `TestCacheInvalidation`
- def: [`tests/test_base_store.py:233`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L233)
- signature: `class TestCacheInvalidation:`
- members:
  - `test_add_invalidates_cache(self, store)` — [`L234`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L234)
  - `test_clear_invalidates_cache(self, store)` — [`L257`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L257)
  - `test_remove_invalidates_cache(self, store)` — [`L250`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L250)
  - `test_repeated_read_uses_cache(self, store)` — [`L263`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L263)
  - `test_update_invalidates_cache(self, store)` — [`L242`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L242)

### `TestDisplayFilter`
- def: [`tests/test_base_store.py:274`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L274)
- signature: `class TestDisplayFilter:`
- members:
  - `test_omits_internal_fields(self, store)` — [`L275`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L275)

### `TestPersistence`
- def: [`tests/test_base_store.py:125`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L125)
- signature: `class TestPersistence:`
- members:
  - `test_auto_save_after_add(self, tmp_path)` — [`L152`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L152)
  - `test_auto_save_after_remove(self, tmp_path)` — [`L165`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L165)
  - `test_auto_save_after_update(self, tmp_path)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L158)
  - `test_corrupt_json_starts_fresh(self, tmp_path)` — [`L142`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L142)
  - `test_empty_file_starts_fresh(self, tmp_path)` — [`L136`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L136)
  - `test_no_file_starts_fresh(self, tmp_path)` — [`L148`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L148)
  - `test_save_load_roundtrip(self, tmp_path)` — [`L126`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L126)
  - `test_sync_to_run_data(self, tmp_path)` — [`L172`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L172)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`add`](../utils/stores/base_store.md#BaseStore.add), [`get`](../utils/stores/base_store.md#BaseStore.get), [`update`](../utils/stores/base_store.md#BaseStore.update), [`remove`](../utils/stores/base_store.md#BaseStore.remove), [`next_id`](../utils/stores/base_store.md#BaseStore.next_id), [`sync_to_run_data`](../utils/stores/base_store.md#BaseStore.sync_to_run_data)  (2 test-only)

### `TestTreeOverview`
- def: [`tests/test_base_store.py:184`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L184)
- signature: `class TestTreeOverview:`
- members:
  - `test_deep_path_flattened_at_4(self, store)` — [`L211`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L211)
  - `test_empty_store(self, store)` — [`L185`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L185)
  - `test_max_display_cap(self, store)` — [`L205`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L205)
  - `test_nested_paths(self, store)` — [`L195`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L195)
  - `test_single_entry(self, store)` — [`L188`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L188)
  - `test_uncategorized_default(self, store)` — [`L218`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L218)
  - `test_unicode_in_titles(self, store)` — [`L223`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L223)

## Functions
- `store(tmp_path)` — [`L54`](../../../../../raw/code/continual-harness/tests/test_base_store.py#L54)

