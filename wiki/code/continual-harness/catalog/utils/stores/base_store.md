---
title: 'Module: utils/stores/base_store.py'
type: catalog
provenance: extracted
module: utils/stores/base_store.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.stores.base_store`/
symbols:
  BaseStore.entries: BaseStore#entries.
  BaseStore.add: BaseStore#add().
  BaseStore.get_tree_overview: BaseStore#get_tree_overview().
  BaseStore.get: BaseStore#get().
  BaseStore.load: BaseStore#load().
  BaseStore: BaseStore#
  BaseStore.update: BaseStore#update().
  BaseStore.save: BaseStore#save().
  BaseStore.remove: BaseStore#remove().
  BaseStore.clear: BaseStore#clear().
  logger: logger.
  BaseStore._deserialize_entry: BaseStore#_deserialize_entry().
  BaseStore.store_file: BaseStore#store_file.
  BaseStore.next_id: BaseStore#next_id.
  BaseStore.to_display_dict: BaseStore#to_display_dict().
  T: T.
  BaseStore.sync_to_run_data: BaseStore#sync_to_run_data().
  BaseStore.get_multiple: BaseStore#get_multiple().
  BaseStore.get_all: BaseStore#get_all().
  BaseStore._invalidate_cache: BaseStore#_invalidate_cache().
  BaseStore._recent_access_ids: BaseStore#_recent_access_ids.
  BaseStore.file_name: BaseStore#file_name.
  BaseStore._cached_tree: BaseStore#_cached_tree.
  BaseStore.__init__: BaseStore#__init__().
  BaseStore.store_label: BaseStore#store_label.
  BaseStore._format_tree_leaf: BaseStore#_format_tree_leaf().
  BaseStore._render_tree: BaseStore#_render_tree().
  BaseStore._compute_recent_roots: BaseStore#_compute_recent_roots().
  BaseStore._serialize_entry: BaseStore#_serialize_entry().
  _INTERNAL_FIELDS: _INTERNAL_FIELDS.
  BaseStore.id_prefix: BaseStore#id_prefix.
  BaseStore.entry_class: BaseStore#entry_class.
  BaseStore.empty_message: BaseStore#empty_message.
  BaseStore.cache_dir: BaseStore#cache_dir.
  StoreEntry: StoreEntry#
  StoreEntry.id: StoreEntry#id.
  StoreEntry.path: StoreEntry#path.
  StoreEntry.title: StoreEntry#title.
  StoreEntry.importance: StoreEntry#importance.
  StoreEntry.mutation_history: StoreEntry#mutation_history.
  StoreEntry.created_at: StoreEntry#created_at.
  StoreEntry.updated_at: StoreEntry#updated_at.
---
# Module: [`utils/stores/base_store.py`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py)

## Classes
### `BaseStore`  ·  implements/extends Generic
- def: [`utils/stores/base_store.py:44`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L44) — documented in [utils-stores-subagents](../../../concepts/utils-stores-subagents.md)
- doc: Persistent JSON store with tree overview and CRUD.
- signature: `class BaseStore(Generic[T]):`
- members:
  - `_compute_recent_roots(self, entries: list)` — [`L243`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L243) — Return root path segments that contain recently-accessed entries.
  - `_deserialize_entry(self, entry_dict: dict)` — [`L344`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L344) — Reconstruct an entry from a JSON dict.
  - `_format_tree_leaf(self, entry: T)` — [`L258`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L258) — Format a single entry for the tree overview. Override in subclasses.
  - `_serialize_entry(self, entry: T)` — [`L299`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L299) — Convert an entry to a JSON-safe dict.
  - `add(self, **fields)` — [`L82`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L82) — Create a new entry. Returns the entry ID. — documented in [utils-stores-base_store](../../../concepts/utils-stores-base_store.md)
  - `clear(self)` — [`L174`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L174)
  - `get(self, entry_id: str)` — [`L145`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L145) — Look up by ID first, then fall back to name/title match.
  - `get_all(self)` — [`L171`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L171)
  - `get_multiple(self, ids: List[str], max_count: int = 3)` — [`L161`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L161) — Return up to *max_count* entries by ID (order preserved).
  - `get_tree_overview(self, max_display: int = 200)` — [`L185`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L185) — Render a hierarchical tree of entries grouped by path.
  - `load(self)` — [`L318`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L318)
  - `remove(self, entry_id: str)` — [`L135`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L135) — Delete an entry. Returns False if not found.
  - `save(self)` — [`L306`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L306)
  - `sync_to_run_data(self, dest_dir: str)` — [`L355`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L355) — Copy the store file to *dest_dir* (e.g. run_data agent_scratch_space).
  - `to_display_dict(self, entry: T)` — [`L286`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L286) — Return only orchestrator-visible fields for a read response.
  - `update(self, entry_id: str, **fields)` — [`L110`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L110) — Update fields on an existing entry. Returns False if not found.
  - `cache_dir` — [`L69`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L69)
  - `empty_message` — [`L61`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L61)
  - `entries` — [`L73`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L73)
  - `entry_class` — [`L62`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L62)
  - `file_name` — [`L58`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L58)
  - `id_prefix` — [`L59`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L59)
  - `next_id` — [`L74`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L74)
  - `store_file` — [`L70`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L70)
  - `store_label` — [`L60`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L60)
- protocol/private: `__init__`[`L64`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L64), `_cached_tree`[`L75`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L75), `_invalidate_cache`[`L279`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L279), `_recent_access_ids`[`L76`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L76), `_render_tree`[`L263`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L263)
- uses (calls/refs, reference-scoped): [`Memory`](memory.md#Memory), [`get_cache_directory`](../data_persistence/run_data_manager.md#get_cache_directory), [`add`](memory.md#Memory.add), [`SubagentStore`](subagents.md#SubagentStore), [`SkillStore`](skills.md#SkillStore), [`logger`](base_store.md#logger), [`_format_tree_leaf`](skills.md#SkillStore._format_tree_leaf), [`T`](base_store.md#T), [`add`](subagents.md#SubagentStore.add), [`get_all`](memory.md#Memory.get_all), [`remove`](subagents.md#SubagentStore.remove), [`update`](subagents.md#SubagentStore.update), [`load`](subagents.md#SubagentStore.load), [`to_display_dict`](subagents.md#SubagentStore.to_display_dict), [`_deserialize_entry`](memory.md#Memory._deserialize_entry), [`_INTERNAL_FIELDS`](base_store.md#_INTERNAL_FIELDS), [`_deserialize_entry`](skills.md#SkillStore._deserialize_entry), [`_deserialize_entry`](subagents.md#SubagentStore._deserialize_entry)  (1 test-only)
- used by: [`Memory`](memory.md#Memory), [`_evolve_subagents`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_subagents), [`_execute_custom_subagent_inner`](../../agents/subagents/utils/executor.md#SubagentExecutor._execute_custom_subagent_inner), [`_evolve_skills`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_skills), [`_evolve_memory`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_memory), [`_execute_builtin_subagent_by_registry_id`](../../agents/PokeAgent.md#PokeAgent._execute_builtin_subagent_by_registry_id), [`add`](memory.md#Memory.add), [`process_memory_direct`](../../server/game_tools.md#process_memory_direct), [`process_skill_direct`](../../server/game_tools.md#process_skill_direct), [`process_subagent_direct`](../../server/game_tools.md#process_subagent_direct), [`SubagentStore`](subagents.md#SubagentStore), [`search`](memory.md#Memory.search), [`SkillStore`](skills.md#SkillStore), [`_execute_run_skill`](../../agents/PokeAgent.md#PokeAgent._execute_run_skill), [`get_summary`](memory.md#Memory.get_summary), [`_migrate_if_needed`](memory.md#Memory._migrate_if_needed), [`_seed_builtins`](subagents.md#SubagentStore._seed_builtins), [`add`](subagents.md#SubagentStore.add), [`get_all`](memory.md#Memory.get_all), [`get_memory_overview_direct`](../../server/game_tools.md#get_memory_overview_direct), [`remove`](subagents.md#SubagentStore.remove), [`get_skill_overview_direct`](../../server/game_tools.md#get_skill_overview_direct), [`get_subagent_overview_direct`](../../server/game_tools.md#get_subagent_overview_direct), [`__init__`](memory.md#Memory.__init__), [`update`](subagents.md#SubagentStore.update), [`load`](subagents.md#SubagentStore.load), [`__init__`](skills.md#SkillStore.__init__), [`__init__`](subagents.md#SubagentStore.__init__)  (39 test-only)

### `StoreEntry`  ·  implements/extends Protocol
- def: [`utils/stores/base_store.py:20`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L20)
- doc: Minimum fields every store entry must expose.
- signature: `class StoreEntry(Protocol):`
- members:
  - `created_at` — [`L27`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L27)
  - `id` — [`L22`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L22)
  - `importance` — [`L25`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L25)
  - `mutation_history` — [`L26`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L26)
  - `path` — [`L23`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L23)
  - `title` — [`L24`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L24)
  - `updated_at` — [`L28`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L28)

## Module values
- `T` — [`L31`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L31)
- `_INTERNAL_FIELDS` — [`L35`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L35)
- `logger` — [`L17`](../../../../../../raw/code/continual-harness/utils/stores/base_store.py#L17)

