---
title: 'Module: utils/stores/memory.py'
type: catalog
provenance: extracted
module: utils/stores/memory.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.stores.memory`/
symbols:
  Memory: Memory#
  Memory.add: Memory#add().
  Memory.search: Memory#search().
  get_memory_store: get_memory_store().
  MemoryEntry: MemoryEntry#
  Memory.get_summary: Memory#get_summary().
  MemoryEntry.path: MemoryEntry#path.
  Memory._migrate_if_needed: Memory#_migrate_if_needed().
  Memory.get_all: Memory#get_all().
  _memory_store._memory_store: _memory_store._memory_store.
  MemoryEntry.__post_init__: MemoryEntry#__post_init__().
  Memory.__init__: Memory#__init__().
  MemoryEntry.coordinates: MemoryEntry#coordinates.
  KnowledgeEntry: KnowledgeEntry.
  KnowledgeBase: KnowledgeBase.
  Memory._deserialize_entry: Memory#_deserialize_entry().
  MemoryEntry.title: MemoryEntry#title.
  MemoryEntry.content: MemoryEntry#content.
  MemoryEntry.created_at: MemoryEntry#created_at.
  MemoryEntry.importance: MemoryEntry#importance.
  get_knowledge_base: get_knowledge_base.
  MemoryEntry.id: MemoryEntry#id.
  MemoryEntry.tags: MemoryEntry#tags.
  MemoryEntry.updated_at: MemoryEntry#updated_at.
  MemoryEntry.source: MemoryEntry#source.
  MemoryEntry.last_modified_step: MemoryEntry#last_modified_step.
  Memory.entry_class: Memory#entry_class.
  logger: logger.
  Memory._migrate_category_to_path: Memory#_migrate_category_to_path().
  MemoryEntry.location: MemoryEntry#location.
  MemoryEntry.mutation_history: MemoryEntry#mutation_history.
  Memory.file_name: Memory#file_name.
  Memory.id_prefix: Memory#id_prefix.
  Memory.store_label: Memory#store_label.
  Memory.empty_message: Memory#empty_message.
---
# Module: [`utils/stores/memory.py`](../../../../../../raw/code/continual-harness/utils/stores/memory.py)

## Classes
### `Memory`  ·  implements/extends BaseStore
- def: [`utils/stores/memory.py:50`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L50) — documented in [utils-stores-memory](../../../concepts/utils-stores-memory.md)
- doc: Persistent long-term memory store.
- signature: `class Memory(BaseStore[MemoryEntry]):`
- members:
  - `_migrate_category_to_path(entry_dict: dict)` — [`L88`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L88) — Convert a legacy ``category`` field to ``path``, removing it.
  - `_migrate_if_needed(self)` — [`L68`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L68) — Auto-migrate from knowledge_base.json -> memory.json,
  - `add(self, **fields)` — [`L113`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L113)
  - `get_all(self, path: Optional[str] = None, category: Optional[str] = None)` — [`L156`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L156) — Return all entries, optionally filtered by path prefix.
  - `get_summary(self, max_entries: int = 20, min_importance: int = 3)` — [`L163`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L163) — Legacy summary format — retained for backward compat.
  - `search(self, path: Optional[str] = None, location: Optional[str] = None, tags: Optional[List[str]] = None, query: Optional[str] = None, min_importance: int = 1, category: Optional[str] = None)` — [`L124`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L124)
  - `empty_message` — [`L56`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L56)
  - `entry_class` — [`L57`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L57)
  - `file_name` — [`L53`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L53)
  - `id_prefix` — [`L54`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L54)
  - `store_label` — [`L55`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L55)
- protocol/private: `__init__`[`L59`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L59), `_deserialize_entry`[`L99`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L99)
- uses (calls/refs, reference-scoped): [`entries`](base_store.md#BaseStore.entries), [`add`](base_store.md#BaseStore.add), [`load`](base_store.md#BaseStore.load), [`BaseStore`](base_store.md#BaseStore), [`MemoryEntry`](memory.md#MemoryEntry), [`path`](memory.md#MemoryEntry.path), [`store_file`](base_store.md#BaseStore.store_file), [`__init__`](base_store.md#BaseStore.__init__), [`content`](memory.md#MemoryEntry.content), [`importance`](memory.md#MemoryEntry.importance), [`title`](memory.md#MemoryEntry.title), [`tags`](memory.md#MemoryEntry.tags), [`updated_at`](memory.md#MemoryEntry.updated_at), [`logger`](memory.md#logger), [`cache_dir`](base_store.md#BaseStore.cache_dir), [`location`](memory.md#MemoryEntry.location)
- used by: [`add`](base_store.md#BaseStore.add), [`_evolve_memory`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_memory), [`process_memory_direct`](../../server/game_tools.md#process_memory_direct), [`BaseStore`](base_store.md#BaseStore), [`get_memory_store`](memory.md#get_memory_store), [`_deserialize_entry`](base_store.md#BaseStore._deserialize_entry), [`_memory_store`](memory.md#_memory_store._memory_store), [`add_memory_direct`](../../server/game_tools.md#add_memory_direct), [`get_memory_summary_direct`](../../server/game_tools.md#get_memory_summary_direct), [`search_memory_direct`](../../server/game_tools.md#search_memory_direct), [`get_all`](base_store.md#BaseStore.get_all), [`KnowledgeBase`](memory.md#KnowledgeBase)  (23 test-only)

### `MemoryEntry`
- def: [`utils/stores/memory.py:20`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L20)
- doc: A single entry in long-term memory.
- signature: `class MemoryEntry:`
- members:
  - `content` — [`L25`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L25)
  - `coordinates` — [`L27`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L27)
  - `created_at` — [`L29`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L29)
  - `id` — [`L22`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L22)
  - `importance` — [`L31`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L31)
  - `last_modified_step` — [`L33`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L33)
  - `location` — [`L26`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L26)
  - `mutation_history` — [`L34`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L34)
  - `path` — [`L23`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L23)
  - `source` — [`L32`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L32)
  - `tags` — [`L28`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L28)
  - `title` — [`L24`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L24)
  - `updated_at` — [`L30`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L30)
- protocol/private: `__post_init__`[`L36`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L36)
- used by: [`Memory`](memory.md#Memory), [`search`](memory.md#Memory.search), [`get_summary`](memory.md#Memory.get_summary), [`get_all`](memory.md#Memory.get_all), [`KnowledgeEntry`](memory.md#KnowledgeEntry), [`_deserialize_entry`](memory.md#Memory._deserialize_entry), [`entry_class`](memory.md#Memory.entry_class)  (13 test-only)

## Functions
- `get_memory_store()` — [`L199`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L199) — Get or create the global Memory instance (persistent across runs).

## Module values
- `KnowledgeBase` — [`L193`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L193)
- `KnowledgeEntry` — [`L47`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L47)
- `_memory_store` — [`L196`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L196)
- `get_knowledge_base` — [`L207`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L207)
- `logger` — [`L16`](../../../../../../raw/code/continual-harness/utils/stores/memory.py#L16)

