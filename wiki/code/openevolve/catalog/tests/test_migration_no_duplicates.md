---
title: 'Module: tests/test_migration_no_duplicates.py'
type: catalog
provenance: extracted
module: tests/test_migration_no_duplicates.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_migration_no_duplicates`/TestMigrationNoDuplicates#
symbols:
  TestMigrationNoDuplicates.db: db.
  TestMigrationNoDuplicates.test_migration_uses_map_elites_deduplication: test_migration_uses_map_elites_deduplication().
  TestMigrationNoDuplicates.test_migrated_program_content_preserved: test_migrated_program_content_preserved().
  TestMigrationNoDuplicates.test_migration_skips_duplicate_code_on_target_island: test_migration_skips_duplicate_code_on_target_island().
  TestMigrationNoDuplicates.test_multiple_migration_rounds_no_exponential_growth: test_multiple_migration_rounds_no_exponential_growth().
  TestMigrationNoDuplicates.test_migration_target_islands_are_different: test_migration_target_islands_are_different().
  TestMigrationNoDuplicates._create_test_program: _create_test_program().
  TestMigrationNoDuplicates.test_no_duplicate_program_ids_across_all_islands: test_no_duplicate_program_ids_across_all_islands().
  TestMigrationNoDuplicates.test_migration_with_feature_map_conflicts_resolved_cleanly: test_migration_with_feature_map_conflicts_resolved_cleanly().
  TestMigrationNoDuplicates.setUp: setUp().
  TestMigrationNoDuplicates.test_migration_creates_clean_uuid_ids: test_migration_creates_clean_uuid_ids().
  TestMigrationNoDuplicates: ''
  TestMigrationNoDuplicates._is_valid_uuid: _is_valid_uuid().
---
# Module: [`tests/test_migration_no_duplicates.py`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py)

## Classes
### `TestMigrationNoDuplicates`  ·  implements/extends TestCase
- def: [`tests/test_migration_no_duplicates.py:16`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L16)
- doc: Tests for migration without creating duplicate program chains
- signature: `class TestMigrationNoDuplicates(unittest.TestCase):`
- members:
  - `_create_test_program(self, program_id: str, score: float, features: list, island: int, generation: int = 1)` — [`L29`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L29) — Helper to create a test program
  - `_is_valid_uuid(self, test_string: str)` — [`L41`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L41) — Check if a string is a valid UUID
  - `setUp(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L19) — Set up test database with migration enabled
  - `test_migrated_program_content_preserved(self)` — [`L123`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L123) — Test that migrated programs preserve original content and metrics
  - `test_migration_creates_clean_uuid_ids(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L49) — Test that migration creates programs with clean UUID IDs, not _migrant suffixes
  - `test_migration_skips_duplicate_code_on_target_island(self)` — [`L337`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L337) — Test that migration skips programs if target island already has identical code
  - `test_migration_target_islands_are_different(self)` — [`L159`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L159) — Test that programs migrate to different islands, not same island
  - `test_migration_uses_map_elites_deduplication(self)` — [`L256`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L256) — Test that migrants go through MAP-Elites deduplication (same cell = keep better) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_migration_with_feature_map_conflicts_resolved_cleanly(self)` — [`L230`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L230) — Test that when migrants compete for same feature cell, resolution is clean
  - `test_multiple_migration_rounds_no_exponential_growth(self)` — [`L83`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L83) — Test that multiple migration rounds don't create exponential program growth
  - `test_no_duplicate_program_ids_across_all_islands(self)` — [`L198`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L198) — Test that no program ID appears in multiple islands simultaneously
  - `db` — [`L27`](../../../../../raw/code/openevolve/tests/test_migration_no_duplicates.py#L27)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`migrate_programs`](../openevolve/database.md#ProgramDatabase.migrate_programs), [`_calculate_feature_coords`](../openevolve/database.md#ProgramDatabase._calculate_feature_coords), [`island_feature_maps`](../openevolve/database.md#ProgramDatabase.island_feature_maps), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`island_generations`](../openevolve/database.md#ProgramDatabase.island_generations), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get`](../openevolve/database.md#ProgramDatabase.get), [`feature_bins`](../openevolve/config.md#DatabaseConfig.feature_bins), [`migration_interval`](../openevolve/config.md#DatabaseConfig.migration_interval), [`_feature_coords_to_key`](../openevolve/database.md#ProgramDatabase._feature_coords_to_key), [`migration_rate`](../openevolve/config.md#DatabaseConfig.migration_rate)

