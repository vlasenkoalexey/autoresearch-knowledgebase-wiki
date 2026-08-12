---
title: 'Module: tests/test_skills.py'
type: catalog
provenance: extracted
module: tests/test_skills.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_skills`/
symbols:
  TestSkillEntry.test_defaults: TestSkillEntry#test_defaults().
  TestSkillStore.test_save_and_reload: TestSkillStore#test_save_and_reload().
  TestSkillStore.test_update: TestSkillStore#test_update().
  TestSkillStore.test_add_and_get: TestSkillStore#test_add_and_get().
  sys_path: sys_path.
  TestSkillEntry.test_title_synced_from_name: TestSkillEntry#test_title_synced_from_name().
  TestSkillEntry.test_name_synced_from_title: TestSkillEntry#test_name_synced_from_title().
  TestSkillStore.test_remove: TestSkillStore#test_remove().
  TestSkillStore.test_display_dict_omits_internal_fields: TestSkillStore#test_display_dict_omits_internal_fields().
  TestSkillStore.test_tree_overview: TestSkillStore#test_tree_overview().
  TestSkillStore.test_empty_tree: TestSkillStore#test_empty_tree().
  TestGetSkillStore.test_returns_same_instance: TestGetSkillStore#test_returns_same_instance().
  TestSkillEntry: TestSkillEntry#
  TestSkillStore: TestSkillStore#
  TestGetSkillStore: TestGetSkillStore#
---
# Module: [`tests/test_skills.py`](../../../../../raw/code/continual-harness/tests/test_skills.py)

## Classes
### `TestGetSkillStore`
- def: [`tests/test_skills.py:104`](../../../../../raw/code/continual-harness/tests/test_skills.py#L104)
- signature: `class TestGetSkillStore:`
- members:
  - `test_returns_same_instance(self, tmp_path)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_skills.py#L105)
- uses (calls/refs, reference-scoped): [`get_skill_store`](../utils/stores/skills.md#get_skill_store), [`_skill_store`](../utils/stores/skills.md#_skill_store._skill_store)

### `TestSkillEntry`
- def: [`tests/test_skills.py:22`](../../../../../raw/code/continual-harness/tests/test_skills.py#L22)
- signature: `class TestSkillEntry:`
- members:
  - `test_defaults(self)` — [`L23`](../../../../../raw/code/continual-harness/tests/test_skills.py#L23)
  - `test_name_synced_from_title(self)` — [`L35`](../../../../../raw/code/continual-harness/tests/test_skills.py#L35)
  - `test_title_synced_from_name(self)` — [`L31`](../../../../../raw/code/continual-harness/tests/test_skills.py#L31)
- uses (calls/refs, reference-scoped): [`name`](../utils/stores/skills.md#SkillEntry.name), [`SkillEntry`](../utils/stores/skills.md#SkillEntry), [`title`](../utils/stores/skills.md#SkillEntry.title), [`id`](../utils/stores/skills.md#SkillEntry.id), [`created_at`](../utils/stores/skills.md#SkillEntry.created_at), [`effectiveness`](../utils/stores/skills.md#SkillEntry.effectiveness), [`path`](../utils/stores/skills.md#SkillEntry.path), [`importance`](../utils/stores/skills.md#SkillEntry.importance), [`mutation_history`](../utils/stores/skills.md#SkillEntry.mutation_history), [`source`](../utils/stores/skills.md#SkillEntry.source)

### `TestSkillStore`
- def: [`tests/test_skills.py:45`](../../../../../raw/code/continual-harness/tests/test_skills.py#L45)
- signature: `class TestSkillStore:`
- members:
  - `test_add_and_get(self, tmp_path)` — [`L46`](../../../../../raw/code/continual-harness/tests/test_skills.py#L46)
  - `test_display_dict_omits_internal_fields(self, tmp_path)` — [`L91`](../../../../../raw/code/continual-harness/tests/test_skills.py#L91)
  - `test_empty_tree(self, tmp_path)` — [`L73`](../../../../../raw/code/continual-harness/tests/test_skills.py#L73)
  - `test_remove(self, tmp_path)` — [`L85`](../../../../../raw/code/continual-harness/tests/test_skills.py#L85)
  - `test_save_and_reload(self, tmp_path)` — [`L54`](../../../../../raw/code/continual-harness/tests/test_skills.py#L54)
  - `test_tree_overview(self, tmp_path)` — [`L64`](../../../../../raw/code/continual-harness/tests/test_skills.py#L64)
  - `test_update(self, tmp_path)` — [`L77`](../../../../../raw/code/continual-harness/tests/test_skills.py#L77)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`add`](../utils/stores/base_store.md#BaseStore.add), [`get_tree_overview`](../utils/stores/base_store.md#BaseStore.get_tree_overview), [`get`](../utils/stores/base_store.md#BaseStore.get), [`update`](../utils/stores/base_store.md#BaseStore.update), [`SkillStore`](../utils/stores/skills.md#SkillStore), [`remove`](../utils/stores/base_store.md#BaseStore.remove), [`name`](../utils/stores/skills.md#SkillEntry.name), [`next_id`](../utils/stores/base_store.md#BaseStore.next_id), [`to_display_dict`](../utils/stores/base_store.md#BaseStore.to_display_dict), [`effectiveness`](../utils/stores/skills.md#SkillEntry.effectiveness), [`path`](../utils/stores/skills.md#SkillEntry.path)

## Module values
- `sys_path` — [`L10`](../../../../../raw/code/continual-harness/tests/test_skills.py#L10)

