---
title: 'Module: tests/test_artifacts_integration.py'
type: catalog
provenance: extracted
module: tests/test_artifacts_integration.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_artifacts_integration`/TestArtifacts
symbols:
  TestArtifactsIntegration.run_test: Integration#run_test().
  TestArtifactsPersistence.test_save_load_artifacts: Persistence#test_save_load_artifacts().
  TestArtifactsIntegration.config: Integration#config.
  TestArtifactsIntegration.evaluator: Integration#evaluator.
  TestArtifactsIntegration.database: Integration#database.
  TestArtifactsPersistence.temp_dir: Persistence#temp_dir.
  TestArtifactsIntegration.test_cascade_evaluation_with_artifacts: Integration#test_cascade_evaluation_with_artifacts().
  TestArtifactsIntegration.loop: Integration#loop.
  TestArtifactsIntegration.prompt_sampler: Integration#prompt_sampler.
  TestArtifactsPersistence.loop: Persistence#loop.
  TestArtifactsIntegration.eval_file: Integration#eval_file.
  TestArtifactsPersistence.database: Persistence#database.
  TestArtifactsIntegration.tearDown: Integration#tearDown().
  TestArtifactsIntegration.test_compile_failure_artifact_capture: Integration#test_compile_failure_artifact_capture().
  TestArtifactsIntegration.test_end_to_end_artifact_flow: Integration#test_end_to_end_artifact_flow().
  TestArtifactsIntegration.test_artifacts_disabled_integration: Integration#test_artifacts_disabled_integration().
  TestArtifactsIntegration.test_successful_evaluation_with_artifacts: Integration#test_successful_evaluation_with_artifacts().
  TestArtifactsPersistence.tearDown: Persistence#tearDown().
  TestArtifactsIntegration.temp_dir: Integration#temp_dir.
  TestArtifactsIntegration: Integration#
  TestArtifactsIntegration.setUp: Integration#setUp().
  TestArtifactsPersistence: Persistence#
  TestArtifactsPersistence.setUp: Persistence#setUp().
---
# Module: [`tests/test_artifacts_integration.py`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py)

## Classes
### `TestArtifactsIntegration`  ·  implements/extends TestCase
- def: [`tests/test_artifacts_integration.py:18`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L18)
- doc: Test full integration of artifacts feature
- signature: `class TestArtifactsIntegration(unittest.TestCase):`
- members:
  - `run_test()` — [`L109`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L109) — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `setUp(self)` — [`L21`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L21)
  - `tearDown(self)` — [`L94`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L94)
  - `test_artifacts_disabled_integration(self)` — [`L212`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L212) — Test that the full system works with artifacts disabled
  - `test_cascade_evaluation_with_artifacts(self)` — [`L181`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L181) — Test cascade evaluation captures artifacts at each stage — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_compile_failure_artifact_capture(self)` — [`L106`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L106) — Test that compilation failures are captured as artifacts
  - `test_end_to_end_artifact_flow(self)` — [`L137`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L137) — Test full flow: eval failure -> artifact -> prompt -> next gen
  - `test_successful_evaluation_with_artifacts(self)` — [`L235`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L235) — Test that successful evaluations can also have artifacts
  - `config` — [`L84`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L84)
  - `database` — [`L90`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L90)
  - `eval_file` — [`L33`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L33)
  - `evaluator` — [`L91`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L91)
  - `loop` — [`L24`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L24)
  - `prompt_sampler` — [`L92`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L92)
  - `temp_dir` — [`L30`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L30)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`metrics`](../openevolve/evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](../openevolve/evaluation_result.md#EvaluationResult), [`artifacts`](../openevolve/evaluation_result.md#EvaluationResult.artifacts), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`language`](../openevolve/database.md#Program.language), [`evaluate_program`](../openevolve/evaluator.md#Evaluator.evaluate_program), [`evaluator`](../openevolve/config.md#Config.evaluator), [`build_prompt`](../openevolve/prompt/sampler.md#PromptSampler.build_prompt), [`prompt`](../openevolve/config.md#Config.prompt), [`_cascade_evaluate`](../openevolve/evaluator.md#Evaluator._cascade_evaluate), [`store_artifacts`](../openevolve/database.md#ProgramDatabase.store_artifacts), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`cascade_evaluation`](../openevolve/config.md#EvaluatorConfig.cascade_evaluation), [`get_artifacts`](../openevolve/database.md#ProgramDatabase.get_artifacts), [`PromptSampler`](../openevolve/prompt/sampler.md#PromptSampler), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path), [`get_pending_artifacts`](../openevolve/evaluator.md#Evaluator.get_pending_artifacts), [`from_dict`](../openevolve/evaluation_result.md#EvaluationResult.from_dict), [`include_artifacts`](../openevolve/config.md#PromptConfig.include_artifacts)

### `TestArtifactsPersistence`  ·  implements/extends TestCase
- def: [`tests/test_artifacts_integration.py:260`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L260)
- doc: Test that artifacts persist correctly across save/load cycles
- signature: `class TestArtifactsPersistence(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L263`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L263)
  - `tearDown(self)` — [`L275`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L275)
  - `test_save_load_artifacts(self)` — [`L286`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L286) — Test that artifacts survive database save/load cycle
  - `database` — [`L273`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L273)
  - `loop` — [`L266`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L266)
  - `temp_dir` — [`L271`](../../../../../raw/code/openevolve/tests/test_artifacts_integration.py#L271)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`load`](../openevolve/database.md#ProgramDatabase.load), [`save`](../openevolve/database.md#ProgramDatabase.save), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`store_artifacts`](../openevolve/database.md#ProgramDatabase.store_artifacts), [`get_artifacts`](../openevolve/database.md#ProgramDatabase.get_artifacts), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path)

