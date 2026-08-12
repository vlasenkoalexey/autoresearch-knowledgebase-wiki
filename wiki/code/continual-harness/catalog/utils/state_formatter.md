---
title: 'Module: utils/state_formatter.py'
type: catalog
provenance: extracted
module: utils/state_formatter.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.state_formatter`/
symbols:
  format_state_for_llm: format_state_for_llm().
  _format_map_info: _format_map_info().
  _format_state_detailed: _format_state_detailed().
  _build_stitched_world_map: _build_stitched_world_map().
  get_movement_preview: get_movement_preview().
  LAST_TRANSITION: LAST_TRANSITION.
  clear_persistent_world_map: clear_persistent_world_map().
  detect_dialogue_on_frame: detect_dialogue_on_frame().
  CURRENT_LOCATION: CURRENT_LOCATION.
  LAST_LOCATION: LAST_LOCATION.
  _add_local_map_fallback: _add_local_map_fallback().
  format_state: format_state().
  MAP_STITCHER_INSTANCE: MAP_STITCHER_INSTANCE.
  logger: logger.
  _format_world_map_display: _format_world_map_display().
  _get_location_connections_from_cache: _get_location_connections_from_cache().
  _format_red_map_info: _format_red_map_info().
  _get_map_stitcher_instance: _get_map_stitcher_instance().
  _format_game_state: _format_game_state().
  format_movement_preview_for_llm: format_movement_preview_for_llm().
  MAP_STITCHER_SAVE_CALLBACK: MAP_STITCHER_SAVE_CALLBACK.
  format_state_summary: format_state_summary().
  format_state_for_debug: format_state_for_debug().
  _get_player_position: _get_player_position().
  _format_party_info: _format_party_info().
  _format_inventory_info: _format_inventory_info().
  save_persistent_world_map: save_persistent_world_map().
  load_persistent_world_map: load_persistent_world_map().
  _format_state_summary: _format_state_summary().
  _format_debug_info: _format_debug_info().
  format_action_history: format_action_history().
  _get_party_size: _get_party_size().
  _format_stitched_map_info: _format_stitched_map_info().
  get_movement_options: get_movement_options().
  get_party_health_summary: get_party_health_summary().
---
# Module: [`utils/state_formatter.py`](../../../../../raw/code/continual-harness/utils/state_formatter.py)

## Functions
- `_add_local_map_fallback(context_parts, map_info, include_npcs, location_name=None)` — [`L944`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L944) — Helper function to add local map display as fallback
- `_build_stitched_world_map(stitched_data, full_state_data=None)` — [`L1011`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1011) — Build map display using MapStitcher
- `_format_debug_info(state_data)` — [`L1376`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1376) — Format additional debug information.
- `_format_game_state(game_data, state_data=None, include_movement_preview=True)` — [`L1320`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1320) — Format game state information (for non-battle mode).
- `_format_inventory_info(player_data, game_data, include_only_pockets=None, header=None)` — [`L660`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L660) — Format bag inventory information from structured player/game state.
- `_format_map_info(map_info, player_data=None, include_debug_info=False, include_npcs=True, full_state_data=None, memory_reader=None)` — [`L701`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L701) — Format map and traversability information using MapStitcher.
- `_format_party_info(player_data, game_data)` — [`L616`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L616) — Format pokemon party information.
- `_format_red_map_info(location_name: Optional[str], player_coords: Optional[Tuple[int, int]], map_info: dict)` — [`L868`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L868) — Format Red's native map data for the agent (equivalent to _format_porymap_info for Emerald).
- `_format_state_detailed(state_data, include_debug_info=False, include_npcs=True, include_movement_preview=True, action_history=None)` — [`L336`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L336) — Internal function to create detailed multi-line state format for LLM prompts.
- `_format_state_summary(state_data)` — [`L224`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L224) — Internal function to create a concise one-line summary of the current state.
- `_format_stitched_map_info(map_info)` — [`L1307`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1307) — Format stitched map information for the agent
- `_format_world_map_display(stitched_data, full_state_data=None)` — [`L968`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L968) — Format location-specific map display
- `_get_location_connections_from_cache()` — [`L37`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L37) — Read location connections from MapStitcher's cache file
- `_get_map_stitcher_instance()` — [`L978`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L978) — Get the MapStitcher instance - always reload from cache for multiprocess compatibility
- `_get_party_size(party_data)` — [`L608`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L608) — Get party size from party data regardless of format.
- `_get_player_position(player_data)` — [`L595`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L595) — Extract player position from various possible locations in player data.
- `clear_persistent_world_map()` — [`L995`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L995) — Clear the MapStitcher's data for testing
- `detect_dialogue_on_frame(screenshot_base64=None, frame_array=None)` — [`L50`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L50) — Detect if dialogue is visible on the game frame by analyzing the lower portion.
- `format_action_history(action_history, max_actions=10)` — [`L1831`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1831) — Format action history with starting and ending positions.
- `format_movement_preview_for_llm(state_data)` — [`L1761`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1761) — Format movement preview in a concise format suitable for LLM prompts.
- `format_state(state_data, format_type="summary", include_debug_info=False, include_npcs=True, include_movement_preview=True, action_history=None)` — [`L174`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L174) — Format comprehensive state data into readable text.
- `format_state_for_debug(state_data)` — [`L553`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L553) — Format state data for detailed debugging output.
- `format_state_for_llm(state_data, include_debug_info=False, include_npcs=True, include_movement_preview=True, action_history=None)` — [`L196`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L196) — Format comprehensive state data into a readable context for the VLM. — documented in [utils-state_formatter](../../concepts/utils-state_formatter.md)
- `format_state_summary(state_data)` — [`L212`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L212) — Create a concise one-line summary of the current state for logging.
- `get_movement_options(state_data)` — [`L1401`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1401) — Extract movement options from traversability data.
- `get_movement_preview(state_data)` — [`L1442`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1442) — Get detailed preview of what happens with each directional movement.
- `get_party_health_summary(state_data)` — [`L1907`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L1907) — Get a summary of party health status.
- `load_persistent_world_map(file_path=None)` — [`L990`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L990) — Deprecated - MapStitcher handles all persistence now
- `save_persistent_world_map(file_path=None)` — [`L985`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L985) — Deprecated - MapStitcher handles all persistence now

## Module values
- `CURRENT_LOCATION` — [`L31`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L31)
- `LAST_LOCATION` — [`L32`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L32)
- `LAST_TRANSITION` — [`L33`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L33)
- `MAP_STITCHER_INSTANCE` — [`L35`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L35)
- `MAP_STITCHER_SAVE_CALLBACK` — [`L34`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L34)
- `logger` — [`L28`](../../../../../raw/code/continual-harness/utils/state_formatter.py#L28)

