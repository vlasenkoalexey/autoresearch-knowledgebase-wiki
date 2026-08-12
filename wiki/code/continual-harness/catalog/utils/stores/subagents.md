---
title: 'Module: utils/stores/subagents.py'
type: catalog
provenance: extracted
module: utils/stores/subagents.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.stores.subagents`/
symbols:
  SubagentStore: SubagentStore#
  get_subagent_store: get_subagent_store().
  SubagentEntry: SubagentEntry#
  SubagentStore._seed_builtins: SubagentStore#_seed_builtins().
  SubagentEntry.name: SubagentEntry#name.
  SubagentEntry.__post_init__: SubagentEntry#__post_init__().
  SubagentStore.add: SubagentStore#add().
  SubagentStore.remove: SubagentStore#remove().
  SubagentEntry.title: SubagentEntry#title.
  _validate_char_caps: _validate_char_caps().
  SubagentStore.update: SubagentStore#update().
  _subagent_store._subagent_store: _subagent_store._subagent_store.
  MAX_INSTRUCTIONS_LEN: MAX_INSTRUCTIONS_LEN.
  MAX_DIRECTIVE_LEN: MAX_DIRECTIVE_LEN.
  SubagentStore.load: SubagentStore#load().
  SubagentStore.to_display_dict: SubagentStore#to_display_dict().
  SubagentEntry.available_tools: SubagentEntry#available_tools.
  SubagentEntry.created_at: SubagentEntry#created_at.
  SubagentStore.__init__: SubagentStore#__init__().
  BUILTIN_SUBAGENT_CONFIGS.BUILTIN_SUBAGENT_CONFIGS: BUILTIN_SUBAGENT_CONFIGS.BUILTIN_SUBAGENT_CONFIGS.
  _SUBAGENT_DISPLAY_EXCLUDE: _SUBAGENT_DISPLAY_EXCLUDE.
  logger: logger.
  SubagentEntry.max_turns: SubagentEntry#max_turns.
  SubagentEntry.is_builtin: SubagentEntry#is_builtin.
  SubagentEntry.updated_at: SubagentEntry#updated_at.
  SubagentStore.entry_class: SubagentStore#entry_class.
  SubagentStore._deserialize_entry: SubagentStore#_deserialize_entry().
  SubagentEntry.id: SubagentEntry#id.
  SubagentEntry.handler_type: SubagentEntry#handler_type.
  SubagentEntry.path: SubagentEntry#path.
  SubagentEntry.system_instructions: SubagentEntry#system_instructions.
  SubagentEntry.directive: SubagentEntry#directive.
  SubagentEntry.return_condition: SubagentEntry#return_condition.
  SubagentEntry.source: SubagentEntry#source.
  SubagentEntry.description: SubagentEntry#description.
  SubagentEntry.importance: SubagentEntry#importance.
  SubagentEntry.mutation_history: SubagentEntry#mutation_history.
  SubagentStore.file_name: SubagentStore#file_name.
  SubagentStore.id_prefix: SubagentStore#id_prefix.
  SubagentStore.store_label: SubagentStore#store_label.
  SubagentStore.empty_message: SubagentStore#empty_message.
---
# Module: [`utils/stores/subagents.py`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py)

## Classes
### `SubagentEntry`
- def: [`utils/stores/subagents.py:27`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L27) — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)
- doc: A single entry in the subagent registry.
- signature: `class SubagentEntry:`
- members:
  - `available_tools` — [`L36`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L36)
  - `created_at` — [`L43`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L43)
  - `description` — [`L33`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L33)
  - `directive` — [`L38`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L38)
  - `handler_type` — [`L34`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L34)
  - `id` — [`L30`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L30)
  - `importance` — [`L40`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L40)
  - `is_builtin` — [`L42`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L42)
  - `max_turns` — [`L35`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L35)
  - `mutation_history` — [`L45`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L45)
  - `name` — [`L32`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L32)
  - `path` — [`L31`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L31)
  - `return_condition` — [`L39`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L39)
  - `source` — [`L41`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L41)
  - `system_instructions` — [`L37`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L37)
  - `title` — [`L46`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L46)
  - `updated_at` — [`L44`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L44)
- protocol/private: `__post_init__`[`L48`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L48)
- used by: [`_execute_custom_subagent_inner`](../../agents/subagents/utils/executor.md#SubagentExecutor._execute_custom_subagent_inner), [`_execute_builtin_subagent_by_registry_id`](../../agents/PokeAgent.md#PokeAgent._execute_builtin_subagent_by_registry_id), [`SubagentStore`](subagents.md#SubagentStore), [`to_display_dict`](subagents.md#SubagentStore.to_display_dict), [`_deserialize_entry`](subagents.md#SubagentStore._deserialize_entry), [`entry_class`](subagents.md#SubagentStore.entry_class)  (8 test-only)

### `SubagentStore`  ·  implements/extends BaseStore
- def: [`utils/stores/subagents.py:159`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L159) — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)
- doc: Persistent subagent registry.
- signature: `class SubagentStore(BaseStore[SubagentEntry]):`
- members:
  - `_seed_builtins(self)` — [`L176`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L176) — Populate built-in entries if none exist yet. — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)
  - `add(self, **fields)` — [`L200`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L200)
  - `load(self)` — [`L172`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L172)
  - `remove(self, entry_id: str)` — [`L208`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L208)
  - `to_display_dict(self, entry: SubagentEntry)` — [`L215`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L215)
  - `update(self, entry_id: str, **fields)` — [`L204`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L204)
  - `empty_message` — [`L165`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L165)
  - `entry_class` — [`L166`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L166)
  - `file_name` — [`L162`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L162)
  - `id_prefix` — [`L163`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L163)
  - `store_label` — [`L164`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L164)
- protocol/private: `__init__`[`L168`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L168), `_deserialize_entry`[`L223`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L223)
- uses (calls/refs, reference-scoped): [`entries`](base_store.md#BaseStore.entries), [`add`](base_store.md#BaseStore.add), [`load`](base_store.md#BaseStore.load), [`BaseStore`](base_store.md#BaseStore), [`update`](base_store.md#BaseStore.update), [`remove`](base_store.md#BaseStore.remove), [`SubagentEntry`](subagents.md#SubagentEntry), [`_validate_char_caps`](subagents.md#_validate_char_caps), [`__init__`](base_store.md#BaseStore.__init__), [`BUILTIN_SUBAGENT_CONFIGS`](subagents.md#BUILTIN_SUBAGENT_CONFIGS.BUILTIN_SUBAGENT_CONFIGS), [`_SUBAGENT_DISPLAY_EXCLUDE`](subagents.md#_SUBAGENT_DISPLAY_EXCLUDE), [`logger`](subagents.md#logger)
- used by: [`add`](base_store.md#BaseStore.add), [`_evolve_subagents`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_subagents), [`process_subagent_direct`](../../server/game_tools.md#process_subagent_direct), [`load`](base_store.md#BaseStore.load), [`BaseStore`](base_store.md#BaseStore), [`update`](base_store.md#BaseStore.update), [`remove`](base_store.md#BaseStore.remove), [`get_subagent_store`](subagents.md#get_subagent_store), [`_deserialize_entry`](base_store.md#BaseStore._deserialize_entry), [`to_display_dict`](base_store.md#BaseStore.to_display_dict), [`_subagent_store`](subagents.md#_subagent_store._subagent_store)  (9 test-only)

## Functions
- `_validate_char_caps(**fields)` — [`L143`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L143) — Raise ValueError if system_instructions or directive exceed caps.
- `get_subagent_store()` — [`L245`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L245) — Get or create the global SubagentStore instance. — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)

## Module values
- `BUILTIN_SUBAGENT_CONFIGS` — [`L61`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L61)
- `MAX_DIRECTIVE_LEN` — [`L18`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L18)
- `MAX_INSTRUCTIONS_LEN` — [`L17`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L17)
- `_SUBAGENT_DISPLAY_EXCLUDE` — [`L20`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L20)
- `_subagent_store` — [`L242`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L242)
- `logger` — [`L15`](../../../../../../raw/code/continual-harness/utils/stores/subagents.py#L15)

