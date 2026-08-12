---
title: 'Module: pokemon_red_env/red_map_reader.py'
type: catalog
provenance: extracted
module: pokemon_red_env/red_map_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.red_map_reader`/
symbols:
  RedMapReader.get_whole_map_data: RedMapReader#get_whole_map_data().
  RedMapReader.read_map_around_player: RedMapReader#read_map_around_player().
  RedMapReader._read_u8: RedMapReader#_read_u8().
  RedMapReader.format_map_for_llm: RedMapReader#format_map_for_llm().
  RedMapReader._load_map_data: RedMapReader#_load_map_data().
  RedMapReader._load_sprite_names: RedMapReader#_load_sprite_names().
  RedMapReader._ensure_npc_cache: RedMapReader#_ensure_npc_cache().
  RedMapReader.read_sprites: RedMapReader#read_sprites().
  RedMapReader._detect_cleared_obstacles: RedMapReader#_detect_cleared_obstacles().
  logger: logger.
  RedMapReader._cleared_obstacles: RedMapReader#_cleared_obstacles.
  RedMapReader.get_traversability_grid: RedMapReader#get_traversability_grid().
  RedMapReader.read_map_name: RedMapReader#read_map_name().
  RedMapReader.read_player_coords: RedMapReader#read_player_coords().
  RedMapReader._load_map_names: RedMapReader#_load_map_names().
  RedMapReader._hidden_sprites: RedMapReader#_hidden_sprites.
  RedMapReader.get_full_coll_map: RedMapReader#get_full_coll_map().
  RedMapReader._clamp_viewport: RedMapReader#_clamp_viewport().
  RedMapReader._classify_grid_symbol: RedMapReader#_classify_grid_symbol().
  RedMapReader._map_cache: RedMapReader#_map_cache.
  RedMapReader._picked_up_items: RedMapReader#_picked_up_items.
  RedMapReader._sprite_name_cache: RedMapReader#_sprite_name_cache.
  RedMapReader._npc_position_cache: RedMapReader#_npc_position_cache.
  RedMapReader.read_map_id: RedMapReader#read_map_id().
  RedMapReader: RedMapReader#
  RedMapReader.DATA_DIR: RedMapReader#DATA_DIR.
  RedMapReader._map_names: RedMapReader#_map_names.
  RedMapReader.read_map_dimensions: RedMapReader#read_map_dimensions().
  RedMapReader._last_map_name: RedMapReader#_last_map_name.
  RedMapReader._resolve_path_ci: RedMapReader#_resolve_path_ci().
  _WALKABLE_SYMBOLS: _WALKABLE_SYMBOLS.
  _COMPACT_SYMBOL: _COMPACT_SYMBOL.
  _FACING_MAP: _FACING_MAP.
  _OBJECT_EVENT_RE: _OBJECT_EVENT_RE.
  RedMapReader.pyboy: RedMapReader#pyboy.
  RedMapReader._OBSTACLE_SYMBOLS: RedMapReader#_OBSTACLE_SYMBOLS.
  RedMapReader.__init__: RedMapReader#__init__().
---
# Module: [`pokemon_red_env/red_map_reader.py`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py)

## Classes
### `RedMapReader`
- def: [`pokemon_red_env/red_map_reader.py:45`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L45)
- doc: Provides map collision + NPC data for Pokemon Red.
- signature: `class RedMapReader:`
- members:
  - `_clamp_viewport(player_coord, radius, map_size)` — [`L291`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L291) — Return (view_start, view_end) clamped to [0, map_size).
  - `_classify_grid_symbol(symbol: str)` — [`L182`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L182) — Grid symbol → (type_str, collision_int).
  - `_detect_cleared_obstacles(self, grid: list, raw_tile_data: list)` — [`L311`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L311) — Detect cut trees ('t') and opened gates ('G') via wTileMap comparison.
  - `_ensure_npc_cache(self, map_name: str, npc_data: list)` — [`L154`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L154) — Get or initialize NPC position cache for the current map.
  - `_load_map_data(self, map_name: str)` — [`L93`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L93) — Load and cache processed_map/{map_name}.json.
  - `_load_map_names(self)` — [`L66`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L66) — Load map_names.json mapping map_id string → map_name.
  - `_load_sprite_names(self, map_name: str)` — [`L120`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L120) — Get sprite names for this map.
  - `_resolve_path_ci(directory: str, filename: str)` — [`L77`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L77) — Return the real path for *filename* inside *directory*, matching
  - `format_map_for_llm(self, radius: int = 4)` — [`L475`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L475) — Return compact ASCII map of the area around the player (for /stream).
  - `get_full_coll_map(self)` — [`L544`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L544) — Return the complete map data for the current location (for test/debug).
  - `get_traversability_grid(self, radius: int = 4)` — [`L780`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L780) — Return 2D bool grid.  True = walkable.  Clamped to map bounds.
  - `get_whole_map_data(self)` — [`L570`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L570) — Return complete map data for /whole_map endpoint.
  - `read_map_around_player(self, radius: int = 7)` — [`L409`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L409) — Return 2D list of (0, type_str, collision_int, 0) tuples.
  - `read_map_dimensions(self)` — [`L205`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L205) — Return (width_blocks, height_blocks) from wCurMapWidth/Height.
  - `read_map_id(self)` — [`L201`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L201) — Current map ID from wCurMap (0xD35E).
  - `read_map_name(self)` — [`L213`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L213) — Return the current map name string.
  - `read_player_coords(self)` — [`L209`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L209) — Return (player_x, player_y) block coords from wXCoord/wYCoord.
  - `read_sprites(self)` — [`L222`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L222) — Read NPC positions from wSpriteStateData1 (0xC100).
  - `DATA_DIR` — [`L48`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L48)
  - `pyboy` — [`L51`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L51)
- protocol/private: `_OBSTACLE_SYMBOLS`[`L309`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L309), `__init__`[`L50`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L50), `_cleared_obstacles`[`L59`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L59), `_hidden_sprites`[`L57`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L57), `_last_map_name`[`L55`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L55), `_map_cache`[`L53`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L53), `_map_names`[`L52`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L52), `_npc_position_cache`[`L56`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L56), `_picked_up_items`[`L58`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L58), `_read_u8`[`L195`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L195), `_sprite_name_cache`[`L54`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L54)
- uses (calls/refs, reference-scoped): [`RedMetatileBehavior`](utils/red_metatile_behavior.md#RedMetatileBehavior), [`logger`](red_map_reader.md#logger), [`NORMAL`](utils/red_metatile_behavior.md#RedMetatileBehavior.NORMAL), [`_COMPACT_SYMBOL`](red_map_reader.md#_COMPACT_SYMBOL), [`_FACING_MAP`](red_map_reader.md#_FACING_MAP), [`_OBJECT_EVENT_RE`](red_map_reader.md#_OBJECT_EVENT_RE), [`_WALKABLE_SYMBOLS`](red_map_reader.md#_WALKABLE_SYMBOLS)
- used by: [`initialize`](red_emulator.md#RedEmulator.initialize)

## Module values
- `_COMPACT_SYMBOL` — [`L29`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L29)
- `_FACING_MAP` — [`L39`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L39)
- `_OBJECT_EVENT_RE` — [`L42`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L42)
- `_WALKABLE_SYMBOLS` — [`L25`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L25)
- `logger` — [`L20`](../../../../../raw/code/continual-harness/pokemon_red_env/red_map_reader.py#L20)

