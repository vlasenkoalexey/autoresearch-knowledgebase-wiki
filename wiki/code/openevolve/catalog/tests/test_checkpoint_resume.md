---
title: 'Module: tests/test_checkpoint_resume.py'
type: catalog
provenance: extracted
module: tests/test_checkpoint_resume.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_checkpoint_resume`/
symbols:
  TestCheckpointResume.run_test: TestCheckpointResume#run_test().
  TestCheckpointResume.config: TestCheckpointResume#config.
  TestCheckpointResume.test_program_path: TestCheckpointResume#test_program_path.
  TestCheckpointResume.evaluator_path: TestCheckpointResume#evaluator_path.
  MockEvaluator.call_count: MockEvaluator#call_count.
  TestCheckpointResume.test_dir: TestCheckpointResume#test_dir.
  MockEvaluator: MockEvaluator#
  TestCheckpointResume.test_program_content: TestCheckpointResume#test_program_content.
  MockEvaluator.evaluate_program: MockEvaluator#evaluate_program().
  TestCheckpointResume.tearDown: TestCheckpointResume#tearDown().
  TestCheckpointResume.test_fresh_start_adds_initial_program: TestCheckpointResume#test_fresh_start_adds_initial_program().
  TestCheckpointResume.test_checkpoint_resume_skips_initial_program: TestCheckpointResume#test_checkpoint_resume_skips_initial_program().
  TestCheckpointResume.test_non_empty_database_at_iteration_zero: TestCheckpointResume#test_non_empty_database_at_iteration_zero().
  TestCheckpointResume.test_multiple_run_calls_no_pollution: TestCheckpointResume#test_multiple_run_calls_no_pollution().
  TestCheckpointResume.evaluator_content: TestCheckpointResume#evaluator_content.
  MockEvaluator.__init__: MockEvaluator#__init__().
  TestCheckpointResume: TestCheckpointResume#
  TestCheckpointResume.setUp: TestCheckpointResume#setUp().
  TestCheckpointResume.test_duplicate_content_prevention: TestCheckpointResume#test_duplicate_content_prevention().
---
# Module: [`tests/test_checkpoint_resume.py`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py)

## Classes
### `MockEvaluator`
- def: [`tests/test_checkpoint_resume.py:21`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L21)
- doc: Mock evaluator for testing
- signature: `class MockEvaluator:`
- members:
  - `evaluate_program(self, code, program_id)` — [`L27`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L27) — Mock evaluation that returns predictable metrics
  - `call_count` — [`L25`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L25)
- protocol/private: `__init__`[`L24`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L24)
- used by: (1 test-only callers)

### `TestCheckpointResume`  ·  implements/extends TestCase
- def: [`tests/test_checkpoint_resume.py:37`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L37)
- doc: Tests for checkpoint resume functionality
- signature: `class TestCheckpointResume(unittest.TestCase):`
- members:
  - `run_test()` — [`L83`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L83) — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `setUp(self)` — [`L40`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L40) — Set up test environment
  - `tearDown(self)` — [`L74`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L74) — Clean up test environment
  - `test_checkpoint_resume_skips_initial_program(self)` — [`L179`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L179) — Test that initial program is not re-added when resuming from checkpoint
  - `test_duplicate_content_prevention(self)` — [`L129`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L129) — Test that programs with identical content are not added multiple times
  - `test_fresh_start_adds_initial_program(self)` — [`L80`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L80) — Test that initial program is added when starting fresh
  - `test_multiple_run_calls_no_pollution(self)` — [`L295`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L295) — Test that calling run() multiple times doesn't pollute the database
  - `test_non_empty_database_at_iteration_zero(self)` — [`L237`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L237) — Test that initial program is not added when database already has programs at iteration 0
  - `config` — [`L69`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L69)
  - `evaluator_content` — [`L59`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L59)
  - `evaluator_path` — [`L64`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L64)
  - `test_dir` — [`L42`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L42)
  - `test_program_content` — [`L45`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L45)
  - `test_program_path` — [`L54`](../../../../../raw/code/openevolve/tests/test_checkpoint_resume.py#L54)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`run`](../openevolve/controller.md#OpenEvolve.run), [`database`](../openevolve/controller.md#OpenEvolve.database), [`language`](../openevolve/database.md#Program.language), [`OpenEvolve`](../openevolve/controller.md#OpenEvolve), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`iteration_found`](../openevolve/database.md#Program.iteration_found), [`last_iteration`](../openevolve/database.md#ProgramDatabase.last_iteration), [`max_iterations`](../openevolve/config.md#Config.max_iterations), [`checkpoint_interval`](../openevolve/config.md#Config.checkpoint_interval)  (2 test-only)

