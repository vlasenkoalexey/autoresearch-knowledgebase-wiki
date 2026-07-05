---
title: 'Module: tests/test_island_child_placement.py'
type: catalog
provenance: extracted
module: tests/test_island_child_placement.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_child_placement`/Test
symbols:
  TestEmptyIslandChildPlacement.db: EmptyIslandChildPlacement#db.
  TestEmptyIslandChildPlacement.test_child_should_go_to_target_island_not_parent_island: EmptyIslandChildPlacement#test_child_should_go_to_target_island_not_parent_island().
  TestEmptyIslandChildPlacement.test_explicit_target_island_overrides_parent_inheritance: EmptyIslandChildPlacement#test_explicit_target_island_overrides_parent_inheritance().
  TestIslandChildPlacement.test_child_inherits_parent_island_when_no_target_specified: IslandChildPlacement#test_child_inherits_parent_island_when_no_target_specified().
  TestIslandChildPlacement.test_child_placed_in_target_island_when_specified: IslandChildPlacement#test_child_placed_in_target_island_when_specified().
  TestIslandPopulationGrowth.test_islands_should_all_get_populated: IslandPopulationGrowth#test_islands_should_all_get_populated().
  TestRegressionOldBehavior.test_without_target_island_child_inherits_parent: RegressionOldBehavior#test_without_target_island_child_inherits_parent().
  TestRegressionOldBehavior.test_with_target_island_child_goes_to_target: RegressionOldBehavior#test_with_target_island_child_goes_to_target().
  TestIslandChildPlacement.db: IslandChildPlacement#db.
  TestRegressionOldBehavior.db: RegressionOldBehavior#db.
  TestIslandChildPlacement.setUp: IslandChildPlacement#setUp().
  TestEmptyIslandChildPlacement.setUp: EmptyIslandChildPlacement#setUp().
  TestIslandPopulationGrowth.setUp: IslandPopulationGrowth#setUp().
  TestRegressionOldBehavior.setUp: RegressionOldBehavior#setUp().
  TestIslandPopulationGrowth.db: IslandPopulationGrowth#db.
  TestEmptyIslandChildPlacement.test_sample_from_empty_island_returns_fallback_parent: EmptyIslandChildPlacement#test_sample_from_empty_island_returns_fallback_parent().
  TestIslandChildPlacement: IslandChildPlacement#
  TestEmptyIslandChildPlacement: EmptyIslandChildPlacement#
  TestIslandPopulationGrowth: IslandPopulationGrowth#
  TestRegressionOldBehavior: RegressionOldBehavior#
---
# Module: [`tests/test_island_child_placement.py`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py)

## Classes
### `TestEmptyIslandChildPlacement`  ·  implements/extends TestCase
- def: [`tests/test_island_child_placement.py:76`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L76)
- doc: Test the critical bug: when sampling from an empty island falls back to
- signature: `class TestEmptyIslandChildPlacement(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L82`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L82) — Set up test database with programs only in island 0
  - `test_child_should_go_to_target_island_not_parent_island(self)` — [`L114`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L114) — CRITICAL TEST: This tests the fix for issue #391.
  - `test_explicit_target_island_overrides_parent_inheritance(self)` — [`L151`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L151) — Test that explicit target_island works even with fallback parent
  - `test_sample_from_empty_island_returns_fallback_parent(self)` — [`L104`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L104) — Test that sampling from empty island falls back to available programs
  - `db` — [`L87`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L87)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size)

### `TestIslandChildPlacement`  ·  implements/extends TestCase
- def: [`tests/test_island_child_placement.py:14`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L14)
- doc: Test that child programs are placed in the correct island
- signature: `class TestIslandChildPlacement(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L17`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L17) — Set up test database with multiple islands
  - `test_child_inherits_parent_island_when_no_target_specified(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L24) — Test that child inherits parent's island when no target_island is given
  - `test_child_placed_in_target_island_when_specified(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L49) — Test that child is placed in target_island when explicitly specified
  - `db` — [`L22`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L22)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size)

### `TestIslandPopulationGrowth`  ·  implements/extends TestCase
- def: [`tests/test_island_child_placement.py:176`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L176)
- doc: Test that simulates multiple evolution iterations and checks
- signature: `class TestIslandPopulationGrowth(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L182`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L182) — Set up test database
  - `test_islands_should_all_get_populated(self)` — [`L189`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L189) — Simulate evolution and verify all islands get programs.
  - `db` — [`L187`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L187)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size)

### `TestRegressionOldBehavior`  ·  implements/extends TestCase
- def: [`tests/test_island_child_placement.py:245`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L245)
- doc: Regression tests to ensure we don't revert to the old buggy behavior.
- signature: `class TestRegressionOldBehavior(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L251`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L251) — Set up test database
  - `test_with_target_island_child_goes_to_target(self)` — [`L293`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L293) — Verify that WITH explicit target_island, child goes to target island.
  - `test_without_target_island_child_inherits_parent(self)` — [`L258`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L258) — Verify that without explicit target_island, child inherits parent's island.
  - `db` — [`L256`](../../../../../raw/code/openevolve/tests/test_island_child_placement.py#L256)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`metadata`](../openevolve/database.md#Program.metadata), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size)

