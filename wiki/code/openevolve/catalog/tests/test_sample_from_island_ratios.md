---
title: 'Module: tests/test_sample_from_island_ratios.py'
type: catalog
provenance: extracted
module: tests/test_sample_from_island_ratios.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_sample_from_island_ratios`/TestSampleFromIsland
symbols:
  TestSampleFromIslandRatios.db: Ratios#db.
  TestSampleFromIslandEdgeCases.test_empty_archive_fallback: EdgeCases#test_empty_archive_fallback().
  TestSampleFromIslandEdgeCases.test_island_id_wrapping: EdgeCases#test_island_id_wrapping().
  TestSampleFromIslandRatios.setUp: Ratios#setUp().
  TestSampleFromIslandRatios.test_weighted_mode_favors_high_fitness: Ratios#test_weighted_mode_favors_high_fitness().
  TestSampleFromIslandEdgeCases.test_empty_island_fallback: EdgeCases#test_empty_island_fallback().
  TestSampleFromIslandEdgeCases.test_single_program_island: EdgeCases#test_single_program_island().
  TestSampleFromIslandEdgeCases.db: EdgeCases#db.
  TestSampleFromIslandRatios.test_exploitation_uses_archive: Ratios#test_exploitation_uses_archive().
  TestSampleFromIslandRatios.test_exploration_mode_uniform_distribution: Ratios#test_exploration_mode_uniform_distribution().
  TestSampleFromIslandRatios.test_exploration_exploitation_random_ratios: Ratios#test_exploration_exploitation_random_ratios().
  TestSampleFromIslandEdgeCases.setUp: EdgeCases#setUp().
  TestSampleFromIslandRatios.test_sample_from_island_returns_from_correct_island: Ratios#test_sample_from_island_returns_from_correct_island().
  TestSampleFromIslandRatios.test_sample_from_island_with_different_islands: Ratios#test_sample_from_island_with_different_islands().
  TestSampleFromIslandRatios: Ratios#
  TestSampleFromIslandEdgeCases: EdgeCases#
---
# Module: [`tests/test_sample_from_island_ratios.py`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py)

## Classes
### `TestSampleFromIslandEdgeCases`  ·  implements/extends TestCase
- def: [`tests/test_sample_from_island_ratios.py:213`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L213)
- doc: Tests for edge cases in sample_from_island()
- signature: `class TestSampleFromIslandEdgeCases(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L216`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L216) — Set up test database
  - `test_empty_archive_fallback(self)` — [`L241`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L241) — Test exploitation mode with empty archive
  - `test_empty_island_fallback(self)` — [`L223`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L223) — Test that empty island falls back to sample()
  - `test_island_id_wrapping(self)` — [`L283`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L283) — Test that island_id wraps around correctly
  - `test_single_program_island(self)` — [`L267`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L267) — Test sampling from island with only one program
  - `db` — [`L221`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L221)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`archive`](../openevolve/database.md#ProgramDatabase.archive), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`exploration_ratio`](../openevolve/config.md#DatabaseConfig.exploration_ratio), [`exploitation_ratio`](../openevolve/config.md#DatabaseConfig.exploitation_ratio)

### `TestSampleFromIslandRatios`  ·  implements/extends TestCase
- def: [`tests/test_sample_from_island_ratios.py:14`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L14)
- doc: Tests for sample_from_island() ratio compliance
- signature: `class TestSampleFromIslandRatios(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L17`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L17) — Set up test database with programs
  - `test_exploitation_uses_archive(self)` — [`L140`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L140) — Test that exploitation mode samples from archive
  - `test_exploration_exploitation_random_ratios(self)` — [`L62`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L62) — Test that sample_from_island respects exploration/exploitation/random ratios
  - `test_exploration_mode_uniform_distribution(self)` — [`L157`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L157) — Test that exploration mode uses uniform random sampling
  - `test_sample_from_island_returns_from_correct_island(self)` — [`L108`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L108) — Test that sampled parent is actually from the requested island
  - `test_sample_from_island_with_different_islands(self)` — [`L122`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L122) — Test that different islands return different programs
  - `test_weighted_mode_favors_high_fitness(self)` — [`L186`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L186) — Test that weighted mode favors programs with higher fitness
  - `db` — [`L30`](../../../../../raw/code/openevolve/tests/test_sample_from_island_ratios.py#L30)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size), [`exploration_ratio`](../openevolve/config.md#DatabaseConfig.exploration_ratio), [`exploitation_ratio`](../openevolve/config.md#DatabaseConfig.exploitation_ratio), [`archive_size`](../openevolve/config.md#DatabaseConfig.archive_size)

