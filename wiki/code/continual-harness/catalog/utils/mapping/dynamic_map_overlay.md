---
title: 'Module: utils/mapping/dynamic_map_overlay.py'
type: catalog
provenance: extracted
module: utils/mapping/dynamic_map_overlay.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.dynamic_map_overlay`/
symbols:
  apply_live_overlay_to_json_map: apply_live_overlay_to_json_map().
  apply_live_metatile_overlay: apply_live_metatile_overlay().
  logger: logger.
  _read_live_tiles: _read_live_tiles().
  is_dynamic_location: is_dynamic_location().
  _build_live_grid: _build_live_grid().
  GBA_MAP_BORDER_OFFSET: GBA_MAP_BORDER_OFFSET.
  DYNAMIC_MAP_LOCATIONS: DYNAMIC_MAP_LOCATIONS.
---
# Module: [`utils/mapping/dynamic_map_overlay.py`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py)

## Functions
- `_build_live_grid(live_raw_tiles: List[List[Any]], location_name: str)` — [`L58`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L58) — Convert raw metatile data into an ASCII symbol grid.
- `_read_live_tiles(memory_reader: Any, width: int, height: int, location_name: str)` — [`L34`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L34) — Read live metatiles from the emulator, returning None on failure.
- `apply_live_metatile_overlay(state: Dict[str, Any], env: Any, location_name: str)` — [`L109`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L109) — Replace porymap grid/raw_tiles in the game *state* dict with live data.
- `apply_live_overlay_to_json_map(json_map: Dict[str, Any], memory_reader: Any, location_name: str)` — [`L73`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L73) — Replace grid/raw_tiles/ascii in a json_map dict with live emulator data.
- `is_dynamic_location(location_name: str)` — [`L29`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L29) — Return True if the given location needs live metatile overlays.

## Module values
- `DYNAMIC_MAP_LOCATIONS` — [`L20`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L20)
- `GBA_MAP_BORDER_OFFSET` — [`L26`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L26)
- `logger` — [`L17`](../../../../../../raw/code/continual-harness/utils/mapping/dynamic_map_overlay.py#L17)

