---
title: 'Module: tests/test_iteration_counting.py'
type: catalog
provenance: extracted
module: tests/test_iteration_counting.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_iteration_counting`/
symbols:
  TestIterationCounting.async_test: TestIterationCounting#async_test().
  run_async_test: run_async_test().
  TestIterationCounting.program_file: TestIterationCounting#program_file.
  TestIterationCounting.eval_file: TestIterationCounting#eval_file.
  TestIterationCounting.test_fresh_start_iteration_counting: TestIterationCounting#test_fresh_start_iteration_counting().
  TestIterationCounting.test_resume_iteration_counting: TestIterationCounting#test_resume_iteration_counting().
  result: result.
  TestIterationCounting.test_dir: TestIterationCounting#test_dir.
  TestIterationCounting.tearDown: TestIterationCounting#tearDown().
  TestIterationCounting.test_controller_iteration_behavior: TestIterationCounting#test_controller_iteration_behavior().
  suite: suite.
  TestIterationCounting: TestIterationCounting#
  TestIterationCounting.setUp: TestIterationCounting#setUp().
  TestIterationCounting.program_content: TestIterationCounting#program_content.
  TestIterationCounting.eval_content: TestIterationCounting#eval_content.
  runner: runner.
  TestIterationCounting.test_checkpoint_boundary_conditions: TestIterationCounting#test_checkpoint_boundary_conditions().
---
# Module: [`tests/test_iteration_counting.py`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py)

## Classes
### `TestIterationCounting`  ·  implements/extends TestCase
- def: [`tests/test_iteration_counting.py:19`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L19)
- doc: Tests for correct iteration counting behavior
- signature: `class TestIterationCounting(unittest.TestCase):`
- members:
  - `async_test()` — [`L158`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L158) — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `setUp(self)` — [`L22`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L22) — Set up test environment
  - `tearDown(self)` — [`L45`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L45) — Clean up test environment
  - `test_checkpoint_boundary_conditions(self)` — [`L118`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L118) — Test checkpoint behavior at various boundaries
  - `test_controller_iteration_behavior(self)` — [`L147`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L147) — Test actual controller behavior with iteration counting - requires optillm server
  - `test_fresh_start_iteration_counting(self)` — [`L51`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L51) — Test that fresh start correctly handles iteration 0 as special
  - `test_resume_iteration_counting(self)` — [`L85`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L85) — Test that resume correctly continues from checkpoint
  - `eval_content` — [`L37`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L37)
  - `eval_file` — [`L41`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L41)
  - `program_content` — [`L27`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L27)
  - `program_file` — [`L32`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L32)
  - `test_dir` — [`L24`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L24)
- uses (calls/refs, reference-scoped): [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`llm`](../openevolve/config.md#Config.llm), [`run`](../openevolve/controller.md#OpenEvolve.run), [`database`](../openevolve/controller.md#OpenEvolve.database), [`evaluator`](../openevolve/config.md#Config.evaluator), [`models`](../openevolve/config.md#LLMConfig.models), [`_save_checkpoint`](../openevolve/controller.md#OpenEvolve._save_checkpoint), [`LLMModelConfig`](../openevolve/config.md#LLMModelConfig), [`OpenEvolve`](../openevolve/controller.md#OpenEvolve), [`api_key`](../openevolve/config.md#LLMModelConfig.api_key), [`name`](../openevolve/config.md#LLMModelConfig.name), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`timeout`](../openevolve/config.md#EvaluatorConfig.timeout), [`weight`](../openevolve/config.md#LLMModelConfig.weight), [`max_iterations`](../openevolve/config.md#Config.max_iterations), [`checkpoint_interval`](../openevolve/config.md#Config.checkpoint_interval), [`api_base`](../openevolve/config.md#LLMModelConfig.api_base), [`parallel_evaluations`](../openevolve/config.md#EvaluatorConfig.parallel_evaluations), [`api_base`](../openevolve/config.md#LLMConfig.api_base)
- used by: (2 test-only callers)

## Functions
- `run_async_test()` — [`L227`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L227)

## Module values
- `result` — [`L224`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L224)
- `runner` — [`L223`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L223)
- `suite` — [`L222`](../../../../../raw/code/openevolve/tests/test_iteration_counting.py#L222)

