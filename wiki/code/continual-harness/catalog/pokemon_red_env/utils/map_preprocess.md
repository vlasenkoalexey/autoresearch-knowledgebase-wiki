---
title: 'Module: pokemon_red_env/utils/map_preprocess.py'
type: catalog
provenance: extracted
module: pokemon_red_env/utils/map_preprocess.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.utils.map_preprocess`/
symbols:
  main: main().
  _GRID_SYMBOL_TO_BEHAVIOR._GRID_SYMBOL_TO_BEHAVIOR: _GRID_SYMBOL_TO_BEHAVIOR._GRID_SYMBOL_TO_BEHAVIOR.
  parse_door_tile_ids_asm: parse_door_tile_ids_asm().
  parse_warp_tile_ids_asm: parse_warp_tile_ids_asm().
  game_code_dir: game_code_dir.
  _HEX_RE: _HEX_RE.
  _norm_tileset: _norm_tileset().
  parse_card_key_coords_asm: parse_card_key_coords_asm().
  parse_collision_tile_ids_asm: parse_collision_tile_ids_asm().
  parse_pair_collision_tile_ids_asm: parse_pair_collision_tile_ids_asm().
  parse_warp_pad_hole_tile_ids_asm: parse_warp_pad_hole_tile_ids_asm().
  parse_bookshelf_tile_ids_asm: parse_bookshelf_tile_ids_asm().
  parse_warp_carpet_tile_ids_asm: parse_warp_carpet_tile_ids_asm().
  main.in_bounds: main().in_bounds().
  env_dir: env_dir.
  parse_collision_tile_ids_asm.label_to_tile_type: parse_collision_tile_ids_asm().label_to_tile_type().
  parse_hidden_objects: parse_hidden_objects().
  classify_hidden_object: classify_hidden_object().
  classify_sign: classify_sign().
  parse_ledge_tiles_asm: parse_ledge_tiles_asm().
  parse_pair_collision_tile_ids_asm.normalize_ttype: parse_pair_collision_tile_ids_asm().normalize_ttype().
  load_map_constants_constants_asm: load_map_constants_constants_asm().
  parse_blk: parse_blk().
  parse_blocks_from_bst: parse_blocks_from_bst().
  build_tile_id_map: build_tile_id_map().
  parse_map_objects_asm: parse_map_objects_asm().
  _CARD_KEY_MAP_CONST_TO_NAME._CARD_KEY_MAP_CONST_TO_NAME: _CARD_KEY_MAP_CONST_TO_NAME._CARD_KEY_MAP_CONST_TO_NAME.
  _WARP_EXCLUSIONS._WARP_EXCLUSIONS: _WARP_EXCLUSIONS._WARP_EXCLUSIONS.
---
# Module: [`pokemon_red_env/utils/map_preprocess.py`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py)

## Functions
- `_norm_tileset(raw: str)` — [`L342`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L342)
- `build_tile_id_map(blk, blocks, map_width_blocks, map_height_blocks)` — [`L565`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L565)
- `classify_hidden_object(func_name: str)` — [`L184`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L184) — Map hidden event function name to grid symbol (matching map_formatter.py).
- `classify_sign(text_id: str)` — [`L204`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L204) — Map a sign text_id (from bg_event TEXT_xxx) to a grid symbol.
- `in_bounds(cx_, cy_)` — [`L919`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L919)
- `label_to_tile_type(label)` — [`L112`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L112)
- `load_map_constants_constants_asm(constants_asm_path)` — [`L532`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L532)
- `main()` — [`L632`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L632)
- `normalize_ttype(tt: str)` — [`L302`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L302)
- `parse_blk(path)` — [`L548`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L548)
- `parse_blocks_from_bst(path)` — [`L552`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L552)
- `parse_bookshelf_tile_ids_asm(path)` — [`L493`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L493) — Parse data/tilesets/bookshelf_tile_ids.asm.
- `parse_card_key_coords_asm(path: str)` — [`L74`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L74) — Parse card_key_coords.asm → {map_name: [(x, y), ...]}.
- `parse_collision_tile_ids_asm(collision_asm_path)` — [`L94`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L94) — Parses the file `data/tilesets/collision_tile_ids.asm` to extract
- `parse_door_tile_ids_asm(path)` — [`L361`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L361) — Parse data/tilesets/door_tile_ids.asm.
- `parse_hidden_objects(asm_text)` — [`L153`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L153) — Parse hidden_events.asm into {MAP_LABEL: {(x,y): description, ...}, ...}.
- `parse_ledge_tiles_asm(ledge_tiles_asm_path)` — [`L234`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L234) — Parses the file `ledge_tiles.asm` in the following format:
- `parse_map_objects_asm(root_dir, map_name)` — [`L581`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L581)
- `parse_pair_collision_tile_ids_asm(path)` — [`L280`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L280) — Reads the file `pair_collision_tile_ids.asm` and collects
- `parse_warp_carpet_tile_ids_asm(path)` — [`L513`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L513) — Parse data/tilesets/warp_carpet_tile_ids.asm.
- `parse_warp_pad_hole_tile_ids_asm(path)` — [`L470`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L470) — Parse data/tilesets/warp_pad_hole_tile_ids.asm.
- `parse_warp_tile_ids_asm(path)` — [`L409`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L409) — Parse data/tilesets/warp_tile_ids.asm.

## Module values
- `_CARD_KEY_MAP_CONST_TO_NAME` — [`L54`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L54)
- `_GRID_SYMBOL_TO_BEHAVIOR` — [`L26`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L26)
- `_HEX_RE` — [`L339`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L339)
- `_WARP_EXCLUSIONS` — [`L70`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L70)
- `env_dir` — [`L20`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L20)
- `game_code_dir` — [`L21`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/map_preprocess.py#L21)

