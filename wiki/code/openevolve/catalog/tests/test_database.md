---
title: 'Module: tests/test_database.py'
type: catalog
provenance: extracted
module: tests/test_database.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_database`/TestProgramDatabase#
symbols:
  TestProgramDatabase.db: db.
  TestProgramDatabase.test_empty_island_initialization_creates_copies: test_empty_island_initialization_creates_copies().
  TestProgramDatabase.test_migration_prevents_re_migration: test_migration_prevents_re_migration().
  TestProgramDatabase.test_no_program_assigned_to_multiple_islands: test_no_program_assigned_to_multiple_islands().
  TestProgramDatabase.test_migration_validation_passes: test_migration_validation_passes().
  TestProgramDatabase.test_multi_island_setup: test_multi_island_setup().
  TestProgramDatabase.test_archive_operations: test_archive_operations().
  TestProgramDatabase.test_feature_coordinates_calculation: test_feature_coordinates_calculation().
  TestProgramDatabase.test_population_limit_enforcement: test_population_limit_enforcement().
  TestProgramDatabase.test_diversity_feature_integration: test_diversity_feature_integration().
  TestProgramDatabase.test_island_operations_basic: test_island_operations_basic().
  TestProgramDatabase.test_feature_map_operations: test_feature_map_operations().
  TestProgramDatabase.test_calculate_diversity_bin_adaptive: test_calculate_diversity_bin_adaptive().
  TestProgramDatabase.test_add_and_get: test_add_and_get().
  TestProgramDatabase.test_get_best_program: test_get_best_program().
  TestProgramDatabase.test_sample: test_sample().
  TestProgramDatabase.test_get_top_programs_with_metrics: test_get_top_programs_with_metrics().
  TestProgramDatabase.test_best_program_tracking: test_best_program_tracking().
  TestProgramDatabase.test_calculate_complexity_bin_adaptive: test_calculate_complexity_bin_adaptive().
  TestProgramDatabase.test_calculate_complexity_bin_cold_start: test_calculate_complexity_bin_cold_start().
  TestProgramDatabase.test_calculate_diversity_bin_cold_start: test_calculate_diversity_bin_cold_start().
  TestProgramDatabase.test_calculate_diversity_bin_identical_programs: test_calculate_diversity_bin_identical_programs().
  TestProgramDatabase.setUp: setUp().
  TestProgramDatabase.test_fast_code_diversity_function: test_fast_code_diversity_function().
  TestProgramDatabase: ''
---
# Module: [`tests/test_database.py`](../../../../../raw/code/openevolve/tests/test_database.py)

## Classes
### `TestProgramDatabase`  ·  implements/extends TestCase
- def: [`tests/test_database.py:11`](../../../../../raw/code/openevolve/tests/test_database.py#L11)
- doc: Tests for program database
- signature: `class TestProgramDatabase(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_database.py#L14) — Set up test database
  - `test_add_and_get(self)` — [`L20`](../../../../../raw/code/openevolve/tests/test_database.py#L20) — Test adding and retrieving a program
  - `test_archive_operations(self)` — [`L233`](../../../../../raw/code/openevolve/tests/test_database.py#L233) — Test archive functionality
  - `test_best_program_tracking(self)` — [`L253`](../../../../../raw/code/openevolve/tests/test_database.py#L253) — Test absolute best program tracking
  - `test_calculate_complexity_bin_adaptive(self)` — [`L297`](../../../../../raw/code/openevolve/tests/test_database.py#L297) — Test adaptive complexity binning with multiple programs
  - `test_calculate_complexity_bin_cold_start(self)` — [`L331`](../../../../../raw/code/openevolve/tests/test_database.py#L331) — Test complexity binning during cold start (< 2 programs)
  - `test_calculate_diversity_bin_adaptive(self)` — [`L347`](../../../../../raw/code/openevolve/tests/test_database.py#L347) — Test adaptive diversity binning with multiple programs
  - `test_calculate_diversity_bin_cold_start(self)` — [`L383`](../../../../../raw/code/openevolve/tests/test_database.py#L383) — Test diversity binning during cold start (< 2 programs)
  - `test_calculate_diversity_bin_identical_programs(self)` — [`L399`](../../../../../raw/code/openevolve/tests/test_database.py#L399) — Test diversity binning when all programs have identical diversity
  - `test_diversity_feature_integration(self)` — [`L434`](../../../../../raw/code/openevolve/tests/test_database.py#L434) — Test diversity feature calculation in feature coordinates
  - `test_empty_island_initialization_creates_copies(self)` — [`L514`](../../../../../raw/code/openevolve/tests/test_database.py#L514) — Test that empty islands are initialized with copies, not shared references — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_fast_code_diversity_function(self)` — [`L414`](../../../../../raw/code/openevolve/tests/test_database.py#L414) — Test the _fast_code_diversity function
  - `test_feature_coordinates_calculation(self)` — [`L127`](../../../../../raw/code/openevolve/tests/test_database.py#L127) — Test MAP-Elites feature coordinate calculation
  - `test_feature_map_operations(self)` — [`L147`](../../../../../raw/code/openevolve/tests/test_database.py#L147) — Test per-island feature map operations for MAP-Elites
  - `test_get_best_program(self)` — [`L37`](../../../../../raw/code/openevolve/tests/test_database.py#L37) — Test getting the best program
  - `test_get_top_programs_with_metrics(self)` — [`L207`](../../../../../raw/code/openevolve/tests/test_database.py#L207) — Test get_top_programs with specific metrics
  - `test_island_operations_basic(self)` — [`L84`](../../../../../raw/code/openevolve/tests/test_database.py#L84) — Test basic island operations
  - `test_migration_prevents_re_migration(self)` — [`L463`](../../../../../raw/code/openevolve/tests/test_database.py#L463) — Test that programs marked as migrants don't migrate again — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_migration_validation_passes(self)` — [`L597`](../../../../../raw/code/openevolve/tests/test_database.py#L597) — Test that migration validation passes after our fixes
  - `test_multi_island_setup(self)` — [`L102`](../../../../../raw/code/openevolve/tests/test_database.py#L102) — Test database with multiple islands
  - `test_no_program_assigned_to_multiple_islands(self)` — [`L554`](../../../../../raw/code/openevolve/tests/test_database.py#L554) — Test that programs are never assigned to multiple islands — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_population_limit_enforcement(self)` — [`L275`](../../../../../raw/code/openevolve/tests/test_database.py#L275) — Test population size limit enforcement
  - `test_sample(self)` — [`L60`](../../../../../raw/code/openevolve/tests/test_database.py#L60) — Test sampling from the database
  - `db` — [`L18`](../../../../../raw/code/openevolve/tests/test_database.py#L18)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`migrate_programs`](../openevolve/database.md#ProgramDatabase.migrate_programs), [`_calculate_feature_coords`](../openevolve/database.md#ProgramDatabase._calculate_feature_coords), [`island_feature_maps`](../openevolve/database.md#ProgramDatabase.island_feature_maps), [`best_program_id`](../openevolve/database.md#ProgramDatabase.best_program_id), [`island_best_programs`](../openevolve/database.md#ProgramDatabase.island_best_programs), [`feature_dimensions`](../openevolve/config.md#DatabaseConfig.feature_dimensions), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`island_generations`](../openevolve/database.md#ProgramDatabase.island_generations), [`parent_id`](../openevolve/database.md#Program.parent_id), [`archive`](../openevolve/database.md#ProgramDatabase.archive), [`get_best_program`](../openevolve/database.md#ProgramDatabase.get_best_program), [`feature_bins`](../openevolve/database.md#ProgramDatabase.feature_bins), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get_top_programs`](../openevolve/database.md#ProgramDatabase.get_top_programs), [`get`](../openevolve/database.md#ProgramDatabase.get), [`sample`](../openevolve/database.md#ProgramDatabase.sample), [`_validate_migration_results`](../openevolve/database.md#ProgramDatabase._validate_migration_results), [`_calculate_complexity_bin`](../openevolve/database.md#ProgramDatabase._calculate_complexity_bin), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size), [`_calculate_diversity_bin`](../openevolve/database.md#ProgramDatabase._calculate_diversity_bin), [`exploration_ratio`](../openevolve/config.md#DatabaseConfig.exploration_ratio), [`exploitation_ratio`](../openevolve/config.md#DatabaseConfig.exploitation_ratio), [`set_current_island`](../openevolve/database.md#ProgramDatabase.set_current_island), [`migration_interval`](../openevolve/config.md#DatabaseConfig.migration_interval), [`_fast_code_diversity`](../openevolve/database.md#ProgramDatabase._fast_code_diversity), [`archive_size`](../openevolve/config.md#DatabaseConfig.archive_size)

