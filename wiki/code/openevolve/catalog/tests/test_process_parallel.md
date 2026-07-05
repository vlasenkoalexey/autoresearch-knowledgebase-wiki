---
title: 'Module: tests/test_process_parallel.py'
type: catalog
provenance: extracted
module: tests/test_process_parallel.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_process_parallel`/TestProcessParallel#
symbols:
  TestProcessParallel.config: config.
  TestProcessParallel.run_test: run_test().
  TestProcessParallel.database: database.
  TestProcessParallel.test_controller_start_stop: test_controller_start_stop().
  TestProcessParallel.test_controller_initialization: test_controller_initialization().
  TestProcessParallel.test_request_shutdown: test_request_shutdown().
  TestProcessParallel.test_serializable_result: test_serializable_result().
  TestProcessParallel.eval_file: eval_file.
  TestProcessParallel.test_database_snapshot_creation: test_database_snapshot_creation().
  TestProcessParallel.tearDown: tearDown().
  TestProcessParallel.test_run_evolution_basic: test_run_evolution_basic().
  TestProcessParallel.test_dir: test_dir.
  TestProcessParallel.eval_content: eval_content.
  TestProcessParallel: ''
  TestProcessParallel.setUp: setUp().
---
# Module: [`tests/test_process_parallel.py`](../../../../../raw/code/openevolve/tests/test_process_parallel.py)

## Classes
### `TestProcessParallel`  ·  implements/extends TestCase
- def: [`tests/test_process_parallel.py:21`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L21)
- doc: Tests for process-based parallel controller
- signature: `class TestProcessParallel(unittest.TestCase):`
- members:
  - `run_test()` — [`L109`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L109) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `setUp(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L24) — Set up test environment
  - `tearDown(self)` — [`L60`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L60) — Clean up test environment
  - `test_controller_initialization(self)` — [`L66`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L66) — Test that controller initializes correctly
  - `test_controller_start_stop(self)` — [`L74`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L74) — Test starting and stopping the controller
  - `test_database_snapshot_creation(self)` — [`L87`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L87) — Test creating database snapshot for workers
  - `test_request_shutdown(self)` — [`L156`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L156) — Test graceful shutdown request
  - `test_run_evolution_basic(self)` — [`L106`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L106) — Test basic evolution run
  - `test_serializable_result(self)` — [`L166`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L166) — Test SerializableResult dataclass
  - `config` — [`L29`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L29)
  - `database` — [`L47`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L47)
  - `eval_content` — [`L38`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L38)
  - `eval_file` — [`L42`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L42)
  - `test_dir` — [`L26`](../../../../../raw/code/openevolve/tests/test_process_parallel.py#L26)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`language`](../openevolve/database.md#Program.language), [`run_evolution`](../openevolve/process_parallel.md#ProcessParallelController.run_evolution), [`evaluator`](../openevolve/config.md#Config.evaluator), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`get`](../openevolve/database.md#ProgramDatabase.get), [`_create_database_snapshot`](../openevolve/process_parallel.md#ProcessParallelController._create_database_snapshot), [`start`](../openevolve/process_parallel.md#ProcessParallelController.start), [`timeout`](../openevolve/config.md#EvaluatorConfig.timeout), [`iteration_found`](../openevolve/database.md#Program.iteration_found), [`ProcessParallelController`](../openevolve/process_parallel.md#ProcessParallelController), [`SerializableResult`](../openevolve/process_parallel.md#SerializableResult), [`max_iterations`](../openevolve/config.md#Config.max_iterations), [`executor`](../openevolve/process_parallel.md#ProcessParallelController.executor), [`iteration`](../openevolve/process_parallel.md#SerializableResult.iteration), [`checkpoint_interval`](../openevolve/config.md#Config.checkpoint_interval), [`error`](../openevolve/process_parallel.md#SerializableResult.error), [`stop`](../openevolve/process_parallel.md#ProcessParallelController.stop), [`num_workers`](../openevolve/process_parallel.md#ProcessParallelController.num_workers), [`parallel_evaluations`](../openevolve/config.md#EvaluatorConfig.parallel_evaluations), [`shutdown_event`](../openevolve/process_parallel.md#ProcessParallelController.shutdown_event), [`request_shutdown`](../openevolve/process_parallel.md#ProcessParallelController.request_shutdown), [`child_program_dict`](../openevolve/process_parallel.md#SerializableResult.child_program_dict), [`iteration_time`](../openevolve/process_parallel.md#SerializableResult.iteration_time), [`parent_id`](../openevolve/process_parallel.md#SerializableResult.parent_id)

