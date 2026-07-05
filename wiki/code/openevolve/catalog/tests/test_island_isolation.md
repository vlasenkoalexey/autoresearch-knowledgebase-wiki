---
title: 'Module: tests/test_island_isolation.py'
type: catalog
provenance: extracted
module: tests/test_island_isolation.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_isolation`/TestIsland
symbols:
  TestIslandIsolation.test_island_distribution_in_batch: Isolation#test_island_distribution_in_batch().
  TestIslandIsolation.test_submit_iteration_uses_correct_island: Isolation#test_submit_iteration_uses_correct_island().
  TestIslandIsolation.test_database_current_island_restoration: Isolation#test_database_current_island_restoration().
  TestIslandIsolation.config: Isolation#config.
  TestIslandIsolation.database: Isolation#database.
  TestIslandMigration.test_migration_preserves_island_structure: Migration#test_migration_preserves_island_structure().
  TestIslandMigration.config: Migration#config.
  TestIslandMigration.database: Migration#database.
  TestIslandIsolation.test_island_isolation_during_evolution: Isolation#test_island_isolation_during_evolution().
  TestIslandIsolation.mock_sample_from_island: Isolation#mock_sample_from_island().
  TestIslandIsolation.evaluation_file: Isolation#evaluation_file.
  TestIslandIsolation.mock_submit_iteration: Isolation#mock_submit_iteration().
  TestIslandIsolation: Isolation#
  TestIslandIsolation.setUp: Isolation#setUp().
  TestIslandMigration: Migration#
  TestIslandMigration.setUp: Migration#setUp().
---
# Module: [`tests/test_island_isolation.py`](../../../../../raw/code/openevolve/tests/test_island_isolation.py)

## Classes
### `TestIslandIsolation`  ·  implements/extends TestCase
- def: [`tests/test_island_isolation.py:14`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L14)
- doc: Test that workers are properly pinned to islands
- signature: `class TestIslandIsolation(unittest.TestCase):`
- members:
  - `mock_sample_from_island(island_id, num_inspirations=None)` — [`L71`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L71)
  - `mock_submit_iteration(iteration, island_id=None)` — [`L133`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L133)
  - `setUp(self)` — [`L17`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L17) — Set up test environment
  - `test_database_current_island_restoration(self)` — [`L89`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L89) — Test that database current_island is properly restored after sampling
  - `test_island_distribution_in_batch(self)` — [`L116`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L116) — Test that initial batch is distributed across islands — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_island_isolation_during_evolution(self)` — [`L64`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L64) — Test that parallel workers maintain island isolation
  - `test_submit_iteration_uses_correct_island(self)` — [`L27`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L27) — Test that _submit_iteration samples from the specified island
  - `config` — [`L19`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L19)
  - `database` — [`L24`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L24)
  - `evaluation_file` — [`L25`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L25)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`run_evolution`](../openevolve/process_parallel.md#ProcessParallelController.run_evolution), [`evaluator`](../openevolve/config.md#Config.evaluator), [`current_island`](../openevolve/database.md#ProgramDatabase.current_island), [`_submit_iteration`](../openevolve/process_parallel.md#ProcessParallelController._submit_iteration), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`start`](../openevolve/process_parallel.md#ProcessParallelController.start), [`ProcessParallelController`](../openevolve/process_parallel.md#ProcessParallelController), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size), [`stop`](../openevolve/process_parallel.md#ProcessParallelController.stop), [`parallel_evaluations`](../openevolve/config.md#EvaluatorConfig.parallel_evaluations)

### `TestIslandMigration`  ·  implements/extends TestCase
- def: [`tests/test_island_isolation.py:159`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L159)
- doc: Test that migration still works with island pinning
- signature: `class TestIslandMigration(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L162`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L162) — Set up test environment
  - `test_migration_preserves_island_structure(self)` — [`L170`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L170) — Test that migration works correctly with pinned workers
  - `config` — [`L164`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L164)
  - `database` — [`L168`](../../../../../raw/code/openevolve/tests/test_island_isolation.py#L168)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`migrate_programs`](../openevolve/database.md#ProgramDatabase.migrate_programs), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`migration_interval`](../openevolve/config.md#DatabaseConfig.migration_interval), [`migration_rate`](../openevolve/config.md#DatabaseConfig.migration_rate)

