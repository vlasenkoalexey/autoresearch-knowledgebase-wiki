---
title: 'Module: utils/mapping/porymap_state.py'
type: catalog
provenance: extracted
module: utils/mapping/porymap_state.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.porymap_state`/
symbols:
  _format_porymap_info: _format_porymap_info().
  logger: logger.
  PorymapResult: PorymapResult#
  PorymapResult.json_map: PorymapResult#json_map.
  PorymapResult.context_parts: PorymapResult#context_parts.
  ROM_TO_PORYMAP_MAP: ROM_TO_PORYMAP_MAP.
  _format_porymap_info._is_connector: _format_porymap_info()._is_connector().
  _is_npc_object_event: _is_npc_object_event().
  _object_ascii_marker: _object_ascii_marker().
  _get_pokeemerald_root: _get_pokeemerald_root().
  _get_porymap_map_name: _get_porymap_map_name().
  _agent_debug_log: _agent_debug_log().
  _format_porymap_info._get_elev: _format_porymap_info()._get_elev().
  _get_runtime_xy: _get_runtime_xy().
  _normalize_local_id: _normalize_local_id().
  _is_item_object_event: _is_item_object_event().
  _format_porymap_info.normalize_for_matching: _format_porymap_info().normalize_for_matching().
  _graphics_ids_compatible: _graphics_ids_compatible().
  NON_NPC_GRAPHICS_KEYWORDS: NON_NPC_GRAPHICS_KEYWORDS.
---
# Module: [`utils/mapping/porymap_state.py`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py)

## Classes
### `PorymapResult`
- def: [`utils/mapping/porymap_state.py:15`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L15)
- signature: `class PorymapResult:`
- members:
  - `context_parts` — [`L16`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L16)
  - `json_map` — [`L17`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L17)
- used by: [`get_comprehensive_state`](../../server/app.md#get_comprehensive_state), [`_format_porymap_info`](porymap_state.md#_format_porymap_info), [`_format_map_info`](../state_formatter.md#_format_map_info)  (6 test-only)

## Functions
- `_agent_debug_log(hypothesis_id: str, location: str, message: str, data: Dict[str, Any], run_id: str = "run1")` — [`L20`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L20)
- `_format_porymap_info(location_name: Optional[str], player_coords: Optional[Tuple[int, int]] = None, badge_count: int = 0, memory_reader: Any = None, runtime_object_events: Optional[List[Dict[str, Any]]] = None)` — [`L538`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L538) — Format porymap ground truth data (JSON and ASCII map) for the agent.
- `_get_elev(tx, ty)` — [`L701`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L701)
- `_get_pokeemerald_root()` — [`L39`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L39) — Get the pokeemerald root directory path. Delegates to centralized resolver.
- `_get_porymap_map_name(location_name: Optional[str])` — [`L455`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L455) — Convert ROM location name to porymap map name.
- `_get_runtime_xy(runtime_obj: Dict[str, Any])` — [`L468`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L468)
- `_graphics_ids_compatible(static_gid: Any, runtime_gid: Any)` — [`L474`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L474) — Return True when graphics IDs are comparable and match, or unknown.
- `_is_connector(cx, cy)` — [`L707`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L707) — Check if a tile is an elevation connector (E0, stair, door, ladder).
- `_is_item_object_event(obj: Dict[str, Any])` — [`L490`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L490) — Best-effort item object detection.
- `_is_npc_object_event(obj: Dict[str, Any])` — [`L502`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L502) — Best-effort NPC detection without assuming unknowns are items.
- `_normalize_local_id(value: Any)` — [`L462`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L462)
- `_object_ascii_marker(obj: Dict[str, Any])` — [`L529`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L529) — Choose ASCII marker for reconciled object events.
- `normalize_for_matching(name: str)` — [`L583`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L583) — Normalize location name for fuzzy matching.

## Module values
- `NON_NPC_GRAPHICS_KEYWORDS` — [`L485`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L485)
- `ROM_TO_PORYMAP_MAP` — [`L46`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L46)
- `logger` — [`L11`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_state.py#L11)

