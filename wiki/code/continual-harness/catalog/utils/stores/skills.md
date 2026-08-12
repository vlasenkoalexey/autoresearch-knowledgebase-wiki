---
title: 'Module: utils/stores/skills.py'
type: catalog
provenance: extracted
module: utils/stores/skills.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.stores.skills`/
symbols:
  SkillStore: SkillStore#
  get_skill_store: get_skill_store().
  SkillStore._format_tree_leaf: SkillStore#_format_tree_leaf().
  SkillEntry.name: SkillEntry#name.
  SkillEntry: SkillEntry#
  SkillEntry.__post_init__: SkillEntry#__post_init__().
  _skill_store._skill_store: _skill_store._skill_store.
  SkillEntry.title: SkillEntry#title.
  SkillEntry.id: SkillEntry#id.
  SkillStore.__init__: SkillStore#__init__().
  SkillEntry.created_at: SkillEntry#created_at.
  SkillEntry.effectiveness: SkillEntry#effectiveness.
  SkillStore.entry_class: SkillStore#entry_class.
  SkillStore._deserialize_entry: SkillStore#_deserialize_entry().
  SkillEntry.path: SkillEntry#path.
  SkillEntry.code: SkillEntry#code.
  SkillEntry.updated_at: SkillEntry#updated_at.
  SkillEntry.source: SkillEntry#source.
  SkillEntry.importance: SkillEntry#importance.
  SkillEntry.mutation_history: SkillEntry#mutation_history.
  logger: logger.
  SkillEntry.description: SkillEntry#description.
  SkillStore.file_name: SkillStore#file_name.
  SkillStore.id_prefix: SkillStore#id_prefix.
  SkillStore.store_label: SkillStore#store_label.
  SkillStore.empty_message: SkillStore#empty_message.
---
# Module: [`utils/stores/skills.py`](../../../../../../raw/code/continual-harness/utils/stores/skills.py)

## Classes
### `SkillEntry`
- def: [`utils/stores/skills.py:18`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L18)
- doc: A single entry in the skill library.
- signature: `class SkillEntry:`
- members:
  - `code` — [`L24`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L24)
  - `created_at` — [`L27`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L27)
  - `description` — [`L23`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L23)
  - `effectiveness` — [`L25`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L25)
  - `id` — [`L20`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L20)
  - `importance` — [`L29`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L29)
  - `mutation_history` — [`L30`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L30)
  - `name` — [`L22`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L22)
  - `path` — [`L21`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L21)
  - `source` — [`L26`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L26)
  - `title` — [`L31`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L31)
  - `updated_at` — [`L28`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L28)
- protocol/private: `__post_init__`[`L33`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L33)
- used by: [`SkillStore`](skills.md#SkillStore), [`_execute_run_skill`](../../agents/PokeAgent.md#PokeAgent._execute_run_skill), [`_format_tree_leaf`](skills.md#SkillStore._format_tree_leaf), [`_deserialize_entry`](skills.md#SkillStore._deserialize_entry), [`entry_class`](skills.md#SkillStore.entry_class)  (7 test-only)

### `SkillStore`  ·  implements/extends BaseStore
- def: [`utils/stores/skills.py:45`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L45) — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)
- doc: Persistent skill library.
- signature: `class SkillStore(BaseStore[SkillEntry]):`
- members:
  - `_format_tree_leaf(self, entry: SkillEntry)` — [`L58`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L58) — Annotate executable skills so the agent knows to call run_skill.
  - `empty_message` — [`L51`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L51)
  - `entry_class` — [`L52`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L52)
  - `file_name` — [`L48`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L48)
  - `id_prefix` — [`L49`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L49)
  - `store_label` — [`L50`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L50)
- protocol/private: `__init__`[`L54`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L54), `_deserialize_entry`[`L65`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L65)
- uses (calls/refs, reference-scoped): [`load`](base_store.md#BaseStore.load), [`BaseStore`](base_store.md#BaseStore), [`name`](skills.md#SkillEntry.name), [`SkillEntry`](skills.md#SkillEntry), [`title`](skills.md#SkillEntry.title), [`__init__`](base_store.md#BaseStore.__init__), [`id`](skills.md#SkillEntry.id), [`code`](skills.md#SkillEntry.code)
- used by: [`BaseStore`](base_store.md#BaseStore), [`get_skill_store`](skills.md#get_skill_store), [`_deserialize_entry`](base_store.md#BaseStore._deserialize_entry), [`_skill_store`](skills.md#_skill_store._skill_store), [`_format_tree_leaf`](base_store.md#BaseStore._format_tree_leaf)  (10 test-only)

## Functions
- `get_skill_store()` — [`L82`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L82) — Get or create the global SkillStore instance.

## Module values
- `_skill_store` — [`L79`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L79)
- `logger` — [`L14`](../../../../../../raw/code/continual-harness/utils/stores/skills.py#L14)

