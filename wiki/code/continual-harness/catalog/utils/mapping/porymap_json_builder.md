---
title: 'Module: utils/mapping/porymap_json_builder.py'
type: catalog
provenance: extracted
module: utils/mapping/porymap_json_builder.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.porymap_json_builder`/
symbols:
  build_json_map: build_json_map().
  json_map: json_map.
  output_path: output_path.
  build_json_map_for_llm: build_json_map_for_llm().
  args: args.
  parser: parser.
  pokeemerald_root: pokeemerald_root.
  tile_to_symbol: tile_to_symbol().
  save_json_map: save_json_map().
  output_dir: output_dir.
  _build_json_map_for_llm_cached: _build_json_map_for_llm_cached().
---
# Module: [`utils/mapping/porymap_json_builder.py`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py)

## Functions
- `_build_json_map_for_llm_cached(map_name: str, pokeemerald_root_str: str, badge_count: int)` — [`L547`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L547) — Cache static porymap builds to avoid repeated filesystem parsing.
- `build_json_map(map_name: str, pokeemerald_root: Path, include_grid: bool = True, include_ascii: bool = True, badge_count: int = 0)` — [`L38`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L38) — Build a complete JSON map structure from porymap data.
- `build_json_map_for_llm(map_name: str, pokeemerald_root: Path, badge_count: int = 0)` — [`L562`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L562) — Build a JSON map optimized for LLM consumption.
- `save_json_map(map_name: str, pokeemerald_root: Path, output_path: Path)` — [`L591`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L591) — Build and save a JSON map to file.
- `tile_to_symbol(tile_tuple: Tuple[int, Any, int, int], location_name: str = "")` — [`L31`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L31) — Proxy to shared formatter so behaviour-based symbols stay in sync.

## Module values
- `args` — [`L627`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L627)
- `json_map` — [`L631`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L631)
- `output_dir` — [`L643`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L643)
- `output_path` — [`L645`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L645)
- `parser` — [`L621`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L621)
- `pokeemerald_root` — [`L629`](../../../../../../raw/code/continual-harness/utils/mapping/porymap_json_builder.py#L629)

