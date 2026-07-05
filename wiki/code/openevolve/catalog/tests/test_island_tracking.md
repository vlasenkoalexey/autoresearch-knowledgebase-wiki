---
title: 'Module: tests/test_island_tracking.py'
type: catalog
provenance: extracted
module: tests/test_island_tracking.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_tracking`/TestIslandTracking#
symbols:
  TestIslandTracking.db: db.
  TestIslandTracking._create_test_program: _create_test_program().
  TestIslandTracking.test_migration_updates_island_best: test_migration_updates_island_best().
  TestIslandTracking.test_island_best_with_combined_score: test_island_best_with_combined_score().
  TestIslandTracking.test_island_best_with_missing_program: test_island_best_with_missing_program().
  TestIslandTracking.test_sample_inspirations_from_island: test_sample_inspirations_from_island().
  TestIslandTracking.test_get_top_programs_island_specific: test_get_top_programs_island_specific().
  TestIslandTracking.setUp: setUp().
  TestIslandTracking.test_first_program_becomes_island_best: test_first_program_becomes_island_best().
  TestIslandTracking.test_better_program_updates_island_best: test_better_program_updates_island_best().
  TestIslandTracking.test_worse_program_does_not_update_island_best: test_worse_program_does_not_update_island_best().
  TestIslandTracking.test_island_isolation_in_best_tracking: test_island_isolation_in_best_tracking().
  TestIslandTracking.test_island_status_logging: test_island_status_logging().
  TestIslandTracking.test_island_best_persistence: test_island_best_persistence().
  TestIslandTracking.test_initial_island_best_tracking: test_initial_island_best_tracking().
  TestIslandTracking.test_invalid_island_index_handling: test_invalid_island_index_handling().
  TestIslandTracking.test_empty_island_top_programs: test_empty_island_top_programs().
  TestIslandTracking: ''
---
# Module: [`tests/test_island_tracking.py`](../../../../../raw/code/openevolve/tests/test_island_tracking.py)

## Classes
### `TestIslandTracking`  ·  implements/extends TestCase
- def: [`tests/test_island_tracking.py:10`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L10)
- doc: Tests for island best program tracking in program database
- signature: `class TestIslandTracking(unittest.TestCase):`
- members:
  - `_create_test_program(self, program_id: str, score: float, island: int)` — [`L20`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L20) — Helper to create a test program
  - `setUp(self)` — [`L13`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L13) — Set up test database with multiple islands
  - `test_better_program_updates_island_best(self)` — [`L50`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L50) — Test that a better program replaces the island best
  - `test_empty_island_top_programs(self)` — [`L260`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L260) — Test getting top programs from empty island
  - `test_first_program_becomes_island_best(self)` — [`L38`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L38) — Test that the first program added to an island becomes the best
  - `test_get_top_programs_island_specific(self)` — [`L118`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L118) — Test getting top programs from a specific island
  - `test_initial_island_best_tracking(self)` — [`L31`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L31) — Test initial state of island best program tracking
  - `test_invalid_island_index_handling(self)` — [`L254`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L254) — Test handling of invalid island indices
  - `test_island_best_persistence(self)` — [`L230`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L230) — Test that island best programs are maintained across operations
  - `test_island_best_with_combined_score(self)` — [`L147`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L147) — Test island best tracking with combined_score metric
  - `test_island_best_with_missing_program(self)` — [`L173`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L173) — Test island best tracking when best program is removed
  - `test_island_isolation_in_best_tracking(self)` — [`L76`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L76) — Test that island best tracking is isolated between islands
  - `test_island_status_logging(self)` — [`L215`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L215) — Test island status logging functionality
  - `test_migration_updates_island_best(self)` — [`L92`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L92) — Test that migration can update island best programs
  - `test_sample_inspirations_from_island(self)` — [`L190`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L190) — Test that inspiration sampling respects island boundaries
  - `test_worse_program_does_not_update_island_best(self)` — [`L62`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L62) — Test that a worse program does not replace the island best
  - `db` — [`L18`](../../../../../raw/code/openevolve/tests/test_island_tracking.py#L18)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`island_best_programs`](../openevolve/database.md#ProgramDatabase.island_best_programs), [`_sample_inspirations`](../openevolve/database.md#ProgramDatabase._sample_inspirations), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get_top_programs`](../openevolve/database.md#ProgramDatabase.get_top_programs), [`log_island_status`](../openevolve/database.md#ProgramDatabase.log_island_status)

