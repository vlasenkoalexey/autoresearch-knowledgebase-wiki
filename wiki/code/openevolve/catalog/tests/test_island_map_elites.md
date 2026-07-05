---
title: 'Module: tests/test_island_map_elites.py'
type: catalog
provenance: extracted
module: tests/test_island_map_elites.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_map_elites`/TestIslandMapElites#
symbols:
  TestIslandMapElites.db: db.
  TestIslandMapElites.test_checkpoint_serialization_preserves_island_maps: test_checkpoint_serialization_preserves_island_maps().
  TestIslandMapElites._create_test_program: _create_test_program().
  TestIslandMapElites.test_better_program_replaces_in_island_feature_map: test_better_program_replaces_in_island_feature_map().
  TestIslandMapElites.setUp: setUp().
  TestIslandMapElites.test_feature_coordinate_isolation: test_feature_coordinate_isolation().
  TestIslandMapElites.test_global_best_program_tracks_across_islands: test_global_best_program_tracks_across_islands().
  TestIslandMapElites.test_program_added_to_correct_island_feature_map: test_program_added_to_correct_island_feature_map().
  TestIslandMapElites.test_no_migrant_suffix_generation: test_no_migrant_suffix_generation().
  TestIslandMapElites.test_island_feature_maps_initialization: test_island_feature_maps_initialization().
  TestIslandMapElites: ''
---
# Module: [`tests/test_island_map_elites.py`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py)

## Classes
### `TestIslandMapElites`  ·  implements/extends TestCase
- def: [`tests/test_island_map_elites.py:15`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L15)
- doc: Tests for per-island MAP-Elites implementation
- signature: `class TestIslandMapElites(unittest.TestCase):`
- members:
  - `_create_test_program(self, program_id: str, score: float, features: list, island: int = 0)` — [`L26`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L26) — Helper to create a test program with specific features
  - `setUp(self)` — [`L18`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L18) — Set up test database with multiple islands
  - `test_better_program_replaces_in_island_feature_map(self)` — [`L94`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L94) — Test that a better program replaces existing program in same island's cell
  - `test_checkpoint_serialization_preserves_island_maps(self)` — [`L173`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L173) — Test that saving/loading preserves island feature maps correctly
  - `test_feature_coordinate_isolation(self)` — [`L77`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L77) — Test that same feature coordinates in different islands don't conflict
  - `test_global_best_program_tracks_across_islands(self)` — [`L140`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L140) — Test that global best program is tracked correctly across all islands
  - `test_island_feature_maps_initialization(self)` — [`L39`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L39) — Test that each island gets its own feature map
  - `test_no_migrant_suffix_generation(self)` — [`L156`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L156) — Test that no programs with _migrant suffixes are created
  - `test_program_added_to_correct_island_feature_map(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L49) — Test that programs are added to their island's specific feature map
  - `db` — [`L24`](../../../../../raw/code/openevolve/tests/test_island_map_elites.py#L24)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`load`](../openevolve/database.md#ProgramDatabase.load), [`save`](../openevolve/database.md#ProgramDatabase.save), [`island_feature_maps`](../openevolve/database.md#ProgramDatabase.island_feature_maps), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`get_best_program`](../openevolve/database.md#ProgramDatabase.get_best_program), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get`](../openevolve/database.md#ProgramDatabase.get), [`feature_bins`](../openevolve/config.md#DatabaseConfig.feature_bins)

