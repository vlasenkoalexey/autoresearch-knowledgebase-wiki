---
title: 'Module: server/game_tools.py'
type: catalog
provenance: extracted
module: server/game_tools.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `server.game_tools`/
symbols:
  logger: logger.
  process_memory_direct: process_memory_direct().
  process_skill_direct: process_skill_direct().
  process_subagent_direct: process_subagent_direct().
  navigate_to_direct: navigate_to_direct().
  load_porymap_for_pathfinding: load_porymap_for_pathfinding().
  memory_store: memory_store.
  get_game_state_direct: get_game_state_direct().
  subagent_store: subagent_store.
  add_memory_direct: add_memory_direct().
  search_memory_direct: search_memory_direct().
  get_memory_summary_direct: get_memory_summary_direct().
  get_memory_overview_direct: get_memory_overview_direct().
  skill_store: skill_store.
  get_skill_overview_direct: get_skill_overview_direct().
  get_subagent_overview_direct: get_subagent_overview_direct().
  pathfinder: pathfinder.
  _normalize_process_reasoning: _normalize_process_reasoning().
  _validate_process_entries_list: _validate_process_entries_list().
  _batch_all_succeeded: _batch_all_succeeded().
  add_knowledge_direct: add_knowledge_direct.
  search_knowledge_direct: search_knowledge_direct.
  get_knowledge_summary_direct: get_knowledge_summary_direct.
  get_knowledge_base: get_knowledge_base.
---
# Module: [`server/game_tools.py`](../../../../../raw/code/continual-harness/server/game_tools.py)

## Functions
- `_batch_all_succeeded(results: list)` — [`L527`](../../../../../raw/code/continual-harness/server/game_tools.py#L527) — True only if every per-entry result reports success (batch semantics).
- `_normalize_process_reasoning(reasoning: object)` — [`L510`](../../../../../raw/code/continual-harness/server/game_tools.py#L510) — Return stripped non-empty reasoning string, or None if missing/invalid.
- `_validate_process_entries_list(entries: object)` — [`L518`](../../../../../raw/code/continual-harness/server/game_tools.py#L518) — Return an error message if *entries* is not a non-empty list.
- `add_memory_direct(category=None, title="", content="", location=None, coordinates=None, importance=3, path=None)` — [`L452`](../../../../../raw/code/continual-harness/server/game_tools.py#L452) — Add an entry to long-term memory.
- `get_game_state_direct(env, state_formatter, action_history=None, current_obs=None)` — [`L116`](../../../../../raw/code/continual-harness/server/game_tools.py#L116) — Get game state without HTTP calls.
- `get_memory_overview_direct()` — [`L500`](../../../../../raw/code/continual-harness/server/game_tools.py#L500) — Get compact tree overview of long-term memory ([id] title grouped by path).
- `get_memory_summary_direct(min_importance=3)` — [`L490`](../../../../../raw/code/continual-harness/server/game_tools.py#L490) — Get long-term memory summary (legacy content dump).
- `get_skill_overview_direct()` — [`L623`](../../../../../raw/code/continual-harness/server/game_tools.py#L623) — Get compact tree overview of the skill library ([id] name grouped by path).
- `get_subagent_overview_direct()` — [`L726`](../../../../../raw/code/continual-harness/server/game_tools.py#L726) — Get compact tree overview of the subagent registry ([id] name grouped by path).
- `load_porymap_for_pathfinding(state: dict)` — [`L34`](../../../../../raw/code/continual-harness/server/game_tools.py#L34) — Load porymap data into *state* for pathfinding, with game-state-aware override support.
- `navigate_to_direct(env, x, y, reason: str = "", variance: Optional[str] = None, consider_npcs: bool = True, blocked_coords: Optional[List[Tuple[int, int]]] = None)` — [`L209`](../../../../../raw/code/continual-harness/server/game_tools.py#L209) — Calculate path to coordinates without HTTP calls.
- `process_memory_direct(action: str, entries: list, reasoning: object)` — [`L532`](../../../../../raw/code/continual-harness/server/game_tools.py#L532) — Unified CRUD dispatch for long-term memory.
- `process_skill_direct(action: str, entries: list, reasoning: object)` — [`L633`](../../../../../raw/code/continual-harness/server/game_tools.py#L633) — Unified CRUD dispatch for the skill library.
- `process_subagent_direct(action: str, entries: list, reasoning: object)` — [`L736`](../../../../../raw/code/continual-harness/server/game_tools.py#L736) — Unified CRUD dispatch for the subagent registry.
- `search_memory_direct(category=None, query="", location="", min_importance=1, path=None)` — [`L478`](../../../../../raw/code/continual-harness/server/game_tools.py#L478) — Search long-term memory.

## Module values
- `add_knowledge_direct` — [`L851`](../../../../../raw/code/continual-harness/server/game_tools.py#L851)
- `get_knowledge_base` — [`L854`](../../../../../raw/code/continual-harness/server/game_tools.py#L854)
- `get_knowledge_summary_direct` — [`L853`](../../../../../raw/code/continual-harness/server/game_tools.py#L853)
- `logger` — [`L21`](../../../../../raw/code/continual-harness/server/game_tools.py#L21)
- `memory_store` — [`L25`](../../../../../raw/code/continual-harness/server/game_tools.py#L25)
- `pathfinder` — [`L24`](../../../../../raw/code/continual-harness/server/game_tools.py#L24)
- `search_knowledge_direct` — [`L852`](../../../../../raw/code/continual-harness/server/game_tools.py#L852)
- `skill_store` — [`L26`](../../../../../raw/code/continual-harness/server/game_tools.py#L26)
- `subagent_store` — [`L27`](../../../../../raw/code/continual-harness/server/game_tools.py#L27)

