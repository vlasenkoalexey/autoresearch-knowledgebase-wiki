---
title: 'Module: tests/test_file_extension_preservation.py'
type: catalog
provenance: extracted
module: tests/test_file_extension_preservation.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_file_extension_preservation`/TestFileExtensionPreservation#
symbols:
  TestFileExtensionPreservation.config: config.
  TestFileExtensionPreservation.test_evaluator_uses_correct_suffix: test_evaluator_uses_correct_suffix().
  TestFileExtensionPreservation.test_evaluator_temp_file_creation: test_evaluator_temp_file_creation().
  TestFileExtensionPreservation.test_process_parallel_controller_passes_suffix: test_process_parallel_controller_passes_suffix().
  TestFileExtensionPreservation.temp_dir: temp_dir.
  TestFileExtensionPreservation.tearDown: tearDown().
  TestFileExtensionPreservation: ''
  TestFileExtensionPreservation.setUp: setUp().
  TestFileExtensionPreservation.test_controller_preserves_file_extension: test_controller_preserves_file_extension().
  TestFileExtensionPreservation.test_worker_suffix_access: test_worker_suffix_access().
  TestFileExtensionPreservation.test_file_extension_mapping: test_file_extension_mapping().
---
# Module: [`tests/test_file_extension_preservation.py`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py)

## Classes
### `TestFileExtensionPreservation`  ·  implements/extends TestCase
- def: [`tests/test_file_extension_preservation.py:17`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L17)
- doc: Test that file extensions are preserved across iterations
- signature: `class TestFileExtensionPreservation(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L20`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L20) — Set up test fixtures
  - `tearDown(self)` — [`L34`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L34) — Clean up test fixtures
  - `test_controller_preserves_file_extension(self)` — [`L39`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L39) — Test that the controller properly extracts and stores file extension
  - `test_evaluator_temp_file_creation(self)` — [`L130`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L130) — Test that evaluator creates temp files with correct suffix
  - `test_evaluator_uses_correct_suffix(self)` — [`L55`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L55) — Test that the evaluator uses the correct file suffix
  - `test_file_extension_mapping(self)` — [`L113`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L113) — Test that different file extensions are handled correctly
  - `test_process_parallel_controller_passes_suffix(self)` — [`L97`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L97) — Test that ProcessParallelController correctly passes file suffix
  - `test_worker_suffix_access(self)` — [`L81`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L81) — Test that worker can access file suffix from config
  - `config` — [`L25`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L25)
  - `temp_dir` — [`L22`](../../../../../raw/code/openevolve/tests/test_file_extension_preservation.py#L22)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`llm`](../openevolve/config.md#Config.llm), [`evaluator`](../openevolve/config.md#Config.evaluator), [`models`](../openevolve/config.md#LLMConfig.models), [`prompt`](../openevolve/config.md#Config.prompt), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`EvaluatorConfig`](../openevolve/config.md#EvaluatorConfig), [`ProcessParallelController`](../openevolve/process_parallel.md#ProcessParallelController), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size), [`PromptConfig`](../openevolve/config.md#PromptConfig), [`max_iterations`](../openevolve/config.md#Config.max_iterations), [`LLMConfig`](../openevolve/config.md#LLMConfig), [`language`](../openevolve/config.md#Config.language), [`parallel_evaluations`](../openevolve/config.md#EvaluatorConfig.parallel_evaluations), [`program_suffix`](../openevolve/evaluator.md#Evaluator.program_suffix), [`file_suffix`](../openevolve/process_parallel.md#ProcessParallelController.file_suffix)

