---
title: 'Module: utils/mapping/map_formatter.py'
type: catalog
provenance: extracted
module: utils/mapping/map_formatter.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.map_formatter`/
symbols:
  format_tile_to_symbol: format_tile_to_symbol().
  _get_behavior_enum: _get_behavior_enum().
  is_tile_walkable: is_tile_walkable().
  format_map_grid: format_map_grid().
  format_map_for_llm: format_map_for_llm().
  generate_dynamic_legend: generate_dynamic_legend().
  format_map_for_display: format_map_for_display().
  _FallbackEnum: _FallbackEnum#
  _FallbackEnum.name: _FallbackEnum#name.
  get_symbol_legend: get_symbol_legend().
  _FallbackEnum.__new__: _FallbackEnum#__new__().
---
# Module: [`utils/mapping/map_formatter.py`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py)

## Classes
### `_FallbackEnum`  ·  implements/extends int
- def: [`utils/mapping/map_formatter.py:13`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L13)
- signature: `class _FallbackEnum(int):`
- members:
  - `name` — [`L14`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L14)
- protocol/private: `__new__`[`L16`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L16)

## Functions
- `_get_behavior_enum()` — [`L28`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L28) — Return the appropriate behavior enum for the current game type.
- `format_map_for_display(raw_tiles, player_facing="South", title="Map", npcs=None, player_coords=None)` — [`L431`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L431) — Format raw tiles into a complete display string with headers and legend.
- `format_map_for_llm(raw_tiles, player_facing="South", npcs=None, player_coords=None, location_name=None)` — [`L577`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L577) — Format raw tiles into LLM-friendly grid format with detailed NPC information.
- `format_map_grid(raw_tiles, player_facing="South", npcs=None, player_coords=None, trim_padding=True, location_name=None)` — [`L326`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L326) — Format raw tile data into a traversability grid with NPCs.
- `format_tile_to_symbol(tile, x=None, y=None, location_name=None, player_pos=None, stairs_pos=None, raw_tiles=None)` — [`L166`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L166) — Convert a single tile to its display symbol.
- `generate_dynamic_legend(grid)` — [`L524`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L524) — Generate a legend based on symbols that actually appear in the grid.
- `get_symbol_legend()` — [`L477`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L477) — Get the complete symbol legend for map displays.
- `is_tile_walkable(tile)` — [`L47`](../../../../../../raw/code/continual-harness/utils/mapping/map_formatter.py#L47) — Determine if a tile is walkable based on its behavior and collision.

