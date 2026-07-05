---
title: 'Module: tests/test_island_migration.py'
type: catalog
provenance: extracted
module: tests/test_island_migration.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_migration`/TestIslandMigration#
symbols:
  TestIslandMigration.db: db.
  TestIslandMigration.test_migration_creates_proper_copies: test_migration_creates_proper_copies().
  TestIslandMigration._create_test_program: _create_test_program().
  TestIslandMigration.test_no_migration_with_single_island: test_no_migration_with_single_island().
  TestIslandMigration.test_migration_rate_respected: test_migration_rate_respected().
  TestIslandMigration.test_migration_ring_topology: test_migration_ring_topology().
  TestIslandMigration.test_migration_preserves_best_programs: test_migration_preserves_best_programs().
  TestIslandMigration.setUp: setUp().
  TestIslandMigration.test_program_island_assignment: test_program_island_assignment().
  TestIslandMigration.test_migration_updates_generations: test_migration_updates_generations().
  TestIslandMigration.test_migration_with_empty_islands: test_migration_with_empty_islands().
  TestIslandMigration.test_initial_island_setup: test_initial_island_setup().
  TestIslandMigration.test_should_migrate_logic: test_should_migrate_logic().
  TestIslandMigration: ''
---
# Module: [`tests/test_island_migration.py`](../../../../../raw/code/openevolve/tests/test_island_migration.py)

## Classes
### `TestIslandMigration`  ·  implements/extends TestCase
- def: [`tests/test_island_migration.py:10`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L10)
- doc: Tests for island migration in program database
- signature: `class TestIslandMigration(unittest.TestCase):`
- members:
  - `_create_test_program(self, program_id: str, score: float, island: int)` — [`L22`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L22) — Helper to create a test program
  - `setUp(self)` — [`L13`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L13) — Set up test database with multiple islands
  - `test_initial_island_setup(self)` — [`L33`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L33) — Test that islands are properly initialized
  - `test_migration_creates_proper_copies(self)` — [`L214`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L214) — Test that migration creates proper program copies
  - `test_migration_preserves_best_programs(self)` — [`L153`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L153) — Test that migration selects the best programs for migration
  - `test_migration_rate_respected(self)` — [`L117`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L117) — Test that migration rate is properly applied
  - `test_migration_ring_topology(self)` — [`L81`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L81) — Test that migration follows ring topology
  - `test_migration_updates_generations(self)` — [`L183`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L183) — Test that migration updates the last migration generation
  - `test_migration_with_empty_islands(self)` — [`L199`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L199) — Test that migration handles empty islands gracefully
  - `test_no_migration_with_single_island(self)` — [`L256`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L256) — Test that migration is skipped with single island
  - `test_program_island_assignment(self)` — [`L47`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L47) — Test that programs are assigned to correct islands
  - `test_should_migrate_logic(self)` — [`L68`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L68) — Test the migration timing logic
  - `db` — [`L20`](../../../../../raw/code/openevolve/tests/test_island_migration.py#L20)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`migrate_programs`](../openevolve/database.md#ProgramDatabase.migrate_programs), [`island_feature_maps`](../openevolve/database.md#ProgramDatabase.island_feature_maps), [`island_best_programs`](../openevolve/database.md#ProgramDatabase.island_best_programs), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`island_generations`](../openevolve/database.md#ProgramDatabase.island_generations), [`parent_id`](../openevolve/database.md#Program.parent_id), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get`](../openevolve/database.md#ProgramDatabase.get), [`last_migration_generation`](../openevolve/database.md#ProgramDatabase.last_migration_generation), [`should_migrate`](../openevolve/database.md#ProgramDatabase.should_migrate), [`migration_interval`](../openevolve/config.md#DatabaseConfig.migration_interval), [`migration_rate`](../openevolve/config.md#DatabaseConfig.migration_rate)

