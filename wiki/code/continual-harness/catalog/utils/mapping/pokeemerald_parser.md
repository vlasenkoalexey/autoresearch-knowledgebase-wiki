---
title: 'Module: utils/mapping/pokeemerald_parser.py'
type: catalog
provenance: extracted
module: utils/mapping/pokeemerald_parser.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.pokeemerald_parser`/
symbols:
  PokeemeraldLayoutParser.get_metatiles_with_behavior: PokeemeraldLayoutParser#get_metatiles_with_behavior().
  PokeemeraldLayoutParser.layout_lookup: PokeemeraldLayoutParser#layout_lookup.
  PokeemeraldLayoutParser._load_tileset_attributes: PokeemeraldLayoutParser#_load_tileset_attributes().
  PokeemeraldLayoutParser.parse_map_bin: PokeemeraldLayoutParser#parse_map_bin().
  PokeemeraldMapLoader.maps_dir: PokeemeraldMapLoader#maps_dir.
  PokeemeraldLayoutParser.tilesets_dir: PokeemeraldLayoutParser#tilesets_dir.
  PokeemeraldMapLoader: PokeemeraldMapLoader#
  PokeemeraldLayoutParser.get_layout_info: PokeemeraldLayoutParser#get_layout_info().
  PokeemeraldMapLoader.load_map: PokeemeraldMapLoader#load_map().
  PokeemeraldLayoutParser.layouts_dir: PokeemeraldLayoutParser#layouts_dir.
  PokeemeraldMapLoader.get_layout_name_from_map: PokeemeraldMapLoader#get_layout_name_from_map().
  PokeemeraldLayoutParser.root: PokeemeraldLayoutParser#root.
  PokeemeraldLayoutParser._tileset_attributes_cache: PokeemeraldLayoutParser#_tileset_attributes_cache.
  PokeemeraldLayoutParser: PokeemeraldLayoutParser#
  PokeemeraldLayoutParser.tileset_to_dir: PokeemeraldLayoutParser#tileset_to_dir.
  PokeemeraldLayoutParser.layouts_data: PokeemeraldLayoutParser#layouts_data.
  PokeemeraldLayoutParser._parse_binary_file: PokeemeraldLayoutParser#_parse_binary_file().
  PokeemeraldLayoutParser.unpack_metatile: PokeemeraldLayoutParser#unpack_metatile().
  PokeemeraldMapLoader.root: PokeemeraldMapLoader#root.
  MetatileBehavior.NORMAL: MetatileBehavior#NORMAL.
  PokeemeraldLayoutParser.__init__: PokeemeraldLayoutParser#__init__().
  PokeemeraldMapLoader.__init__: PokeemeraldMapLoader#__init__().
  PokeemeraldMapLoader.map_groups: PokeemeraldMapLoader#map_groups.
---
# Module: [`utils/mapping/pokeemerald_parser.py`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py)

## Classes
### `PokeemeraldLayoutParser`
- def: [`utils/mapping/pokeemerald_parser.py:27`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L27)
- doc: Parse pokeemerald layout binary files (map.bin) and tileset attributes
- signature: `class PokeemeraldLayoutParser:`
- members:
  - `_load_tileset_attributes(self, tileset_name: str)` — [`L246`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L246) — Load metatile_attributes.bin for a tileset and extract behavior values.
  - `_parse_binary_file(self, file_path: Path, width: int, height: int)` — [`L198`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L198) — Parse a binary file containing metatile data.
  - `get_layout_info(self, layout_name_or_id: str)` — [`L130`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L130) — Get layout information by name or ID.
  - `get_metatiles_with_behavior(self, layout_name_or_id: str)` — [`L306`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L306) — Parse map.bin and return metatiles with actual behavior from tileset attributes.
  - `parse_map_bin(self, layout_name_or_id: str)` — [`L177`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L177) — Parse map.bin file for a given layout.
  - `unpack_metatile(self, metatile_value: int)` — [`L231`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L231) — Unpack a metatile value into its components.
  - `layout_lookup` — [`L44`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L44)
  - `layouts_data` — [`L41`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L41)
  - `layouts_dir` — [`L32`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L32)
  - `root` — [`L31`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L31)
  - `tileset_to_dir` — [`L52`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L52)
  - `tilesets_dir` — [`L33`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L33)
- protocol/private: `__init__`[`L30`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L30), `_tileset_attributes_cache`[`L128`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L128)
- uses (calls/refs, reference-scoped): [`MetatileBehavior`](../../pokemon_env/enums.md#MetatileBehavior)
- used by: [`build_json_map`](porymap_json_builder.md#build_json_map)

### `PokeemeraldMapLoader`
- def: [`utils/mapping/pokeemerald_parser.py:389`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L389)
- doc: Load and parse pokeemerald map data from JSON files
- signature: `class PokeemeraldMapLoader:`
- members:
  - `get_layout_name_from_map(self, map_name: str)` — [`L413`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L413) — Get the layout name from a map JSON
  - `load_map(self, map_name: str)` — [`L404`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L404) — Load a specific map's JSON data
  - `map_groups` — [`L402`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L402)
  - `maps_dir` — [`L394`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L394)
  - `root` — [`L393`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L393)
- protocol/private: `__init__`[`L392`](../../../../../../raw/code/continual-harness/utils/mapping/pokeemerald_parser.py#L392)
- used by: [`_format_porymap_info`](porymap_state.md#_format_porymap_info), [`get_whole_map`](../../server/app.md#get_whole_map), [`build_json_map`](porymap_json_builder.md#build_json_map)

