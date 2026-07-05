---
title: 'Module: tests/test_artifacts.py'
type: catalog
provenance: extracted
module: tests/test_artifacts.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_artifacts`/Test
symbols:
  TestDatabaseArtifacts.program: DatabaseArtifacts#program.
  TestDatabaseArtifacts.test_store_small_artifacts: DatabaseArtifacts#test_store_small_artifacts().
  TestDatabaseArtifacts.test_store_large_artifacts: DatabaseArtifacts#test_store_large_artifacts().
  TestDatabaseArtifacts.database: DatabaseArtifacts#database.
  TestEvaluationResult.test_from_dict_compatibility: EvaluationResult#test_from_dict_compatibility().
  TestEvaluationResult.test_evaluation_result_with_artifacts: EvaluationResult#test_evaluation_result_with_artifacts().
  TestEvaluationResult.test_artifact_size_calculation: EvaluationResult#test_artifact_size_calculation().
  TestDatabaseArtifacts.test_store_mixed_artifacts: DatabaseArtifacts#test_store_mixed_artifacts().
  TestDatabaseArtifacts.test_artifacts_disabled: DatabaseArtifacts#test_artifacts_disabled().
  TestEvaluatorArtifacts.test_process_evaluation_result_dict: EvaluatorArtifacts#test_process_evaluation_result_dict().
  TestEvaluatorArtifacts.test_process_evaluation_result_evaluation_result: EvaluatorArtifacts#test_process_evaluation_result_evaluation_result().
  TestPromptArtifacts.sampler: PromptArtifacts#sampler.
  TestEvaluatorArtifacts.evaluator: EvaluatorArtifacts#evaluator.
  TestEvaluatorArtifacts.temp_eval_file: EvaluatorArtifacts#temp_eval_file.
  TestDatabaseArtifacts.temp_dir: DatabaseArtifacts#temp_dir.
  TestEvaluatorArtifacts.loop: EvaluatorArtifacts#loop.
  TestEvaluatorArtifacts.test_pending_artifacts: EvaluatorArtifacts#test_pending_artifacts().
  TestEvaluatorArtifacts.run_test: EvaluatorArtifacts#run_test().
  TestEvaluatorArtifacts.tearDown: EvaluatorArtifacts#tearDown().
  TestPromptArtifacts.test_render_artifacts_all_items: PromptArtifacts#test_render_artifacts_all_items().
  TestPromptArtifacts.test_render_artifacts_generic: PromptArtifacts#test_render_artifacts_generic().
  TestPromptArtifacts.test_render_artifacts_truncation: PromptArtifacts#test_render_artifacts_truncation().
  TestPromptArtifacts.test_render_artifacts_security_filter: PromptArtifacts#test_render_artifacts_security_filter().
  TestPromptArtifacts.test_safe_decode_artifact_string: PromptArtifacts#test_safe_decode_artifact_string().
  TestPromptArtifacts.test_safe_decode_artifact_bytes: PromptArtifacts#test_safe_decode_artifact_bytes().
  TestPromptArtifacts.test_safe_decode_artifact_invalid_bytes: PromptArtifacts#test_safe_decode_artifact_invalid_bytes().
  TestPromptArtifacts.test_build_prompt_with_artifacts: PromptArtifacts#test_build_prompt_with_artifacts().
  TestPromptArtifacts.test_build_prompt_without_artifacts: PromptArtifacts#test_build_prompt_without_artifacts().
  TestEvaluatorArtifacts.test_evaluate_program_backward_compatibility: EvaluatorArtifacts#test_evaluate_program_backward_compatibility().
  TestPromptArtifacts.setUp: PromptArtifacts#setUp().
  TestEvaluationResult: EvaluationResult#
  TestDatabaseArtifacts: DatabaseArtifacts#
  TestDatabaseArtifacts.setUp: DatabaseArtifacts#setUp().
  TestEvaluatorArtifacts: EvaluatorArtifacts#
  TestEvaluatorArtifacts.setUp: EvaluatorArtifacts#setUp().
  TestPromptArtifacts: PromptArtifacts#
---
# Module: [`tests/test_artifacts.py`](../../../../../raw/code/openevolve/tests/test_artifacts.py)

## Classes
### `TestDatabaseArtifacts`  ·  implements/extends TestCase
- def: [`tests/test_artifacts.py:67`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L67)
- doc: Test artifact storage in the database
- signature: `class TestDatabaseArtifacts(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L70`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L70)
  - `test_artifacts_disabled(self)` — [`L122`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L122) — Test that artifacts are skipped when disabled
  - `test_store_large_artifacts(self)` — [`L93`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L93) — Test storing large artifacts to disk
  - `test_store_mixed_artifacts(self)` — [`L108`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L108) — Test storing both small and large artifacts
  - `test_store_small_artifacts(self)` — [`L79`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L79) — Test storing small artifacts in JSON
  - `database` — [`L73`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L73)
  - `program` — [`L76`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L76)
  - `temp_dir` — [`L71`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L71)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`store_artifacts`](../openevolve/database.md#ProgramDatabase.store_artifacts), [`get`](../openevolve/database.md#ProgramDatabase.get), [`get_artifacts`](../openevolve/database.md#ProgramDatabase.get_artifacts), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path), [`artifact_dir`](../openevolve/database.md#Program.artifact_dir), [`artifacts_json`](../openevolve/database.md#Program.artifacts_json)

### `TestEvaluationResult`  ·  implements/extends TestCase
- def: [`tests/test_artifacts.py:18`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L18)
- doc: Test the EvaluationResult dataclass
- signature: `class TestEvaluationResult(unittest.TestCase):`
- members:
  - `test_artifact_size_calculation(self)` — [`L48`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L48) — Test artifact size calculation — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_evaluation_result_with_artifacts(self)` — [`L36`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L36) — Test EvaluationResult with artifacts — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_from_dict_compatibility(self)` — [`L21`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L21) — Test that dict -> EvaluationResult -> dict roundtrip works — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
- uses (calls/refs, reference-scoped): [`metrics`](../openevolve/evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](../openevolve/evaluation_result.md#EvaluationResult), [`artifacts`](../openevolve/evaluation_result.md#EvaluationResult.artifacts), [`has_artifacts`](../openevolve/evaluation_result.md#EvaluationResult.has_artifacts), [`get_total_artifact_size`](../openevolve/evaluation_result.md#EvaluationResult.get_total_artifact_size), [`from_dict`](../openevolve/evaluation_result.md#EvaluationResult.from_dict), [`get_artifact_size`](../openevolve/evaluation_result.md#EvaluationResult.get_artifact_size), [`get_artifact_keys`](../openevolve/evaluation_result.md#EvaluationResult.get_artifact_keys), [`to_dict`](../openevolve/evaluation_result.md#EvaluationResult.to_dict)

### `TestEvaluatorArtifacts`  ·  implements/extends TestCase
- def: [`tests/test_artifacts.py:135`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L135)
- doc: Test artifact handling in the evaluator
- signature: `class TestEvaluatorArtifacts(unittest.TestCase):`
- members:
  - `run_test()` — [`L174`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L174)
  - `setUp(self)` — [`L138`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L138)
  - `tearDown(self)` — [`L159`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L159)
  - `test_evaluate_program_backward_compatibility(self)` — [`L171`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L171) — Test that old evaluators still work unchanged
  - `test_pending_artifacts(self)` — [`L197`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L197) — Test pending artifacts storage and retrieval
  - `test_process_evaluation_result_dict(self)` — [`L181`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L181) — Test processing dict results — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_process_evaluation_result_evaluation_result(self)` — [`L190`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L190) — Test processing EvaluationResult objects — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `evaluator` — [`L157`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L157)
  - `loop` — [`L141`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L141)
  - `temp_eval_file` — [`L147`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L147)
- uses (calls/refs, reference-scoped): [`metrics`](../openevolve/evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](../openevolve/evaluation_result.md#EvaluationResult), [`artifacts`](../openevolve/evaluation_result.md#EvaluationResult.artifacts), [`evaluate_program`](../openevolve/evaluator.md#Evaluator.evaluate_program), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`EvaluatorConfig`](../openevolve/config.md#EvaluatorConfig), [`_process_evaluation_result`](../openevolve/evaluator.md#Evaluator._process_evaluation_result), [`_pending_artifacts`](../openevolve/evaluator.md#Evaluator._pending_artifacts), [`get_pending_artifacts`](../openevolve/evaluator.md#Evaluator.get_pending_artifacts)

### `TestPromptArtifacts`  ·  implements/extends TestCase
- def: [`tests/test_artifacts.py:214`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L214)
- doc: Test artifact rendering in prompts
- signature: `class TestPromptArtifacts(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L217`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L217)
  - `test_build_prompt_with_artifacts(self)` — [`L292`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L292) — Test building prompt with artifacts — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_build_prompt_without_artifacts(self)` — [`L309`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L309) — Test building prompt without artifacts — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_render_artifacts_all_items(self)` — [`L221`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L221) — Test that all artifacts are included using .items() without prioritization
  - `test_render_artifacts_generic(self)` — [`L240`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L240) — Test that all artifacts are included using .items()
  - `test_render_artifacts_security_filter(self)` — [`L261`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L261) — Test that security filter redacts potential tokens
  - `test_render_artifacts_truncation(self)` — [`L250`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L250) — Test artifact truncation for large content
  - `test_safe_decode_artifact_bytes(self)` — [`L278`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L278) — Test safe decoding of bytes artifacts
  - `test_safe_decode_artifact_invalid_bytes(self)` — [`L285`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L285) — Test safe decoding of invalid bytes
  - `test_safe_decode_artifact_string(self)` — [`L272`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L272) — Test safe decoding of string artifacts
  - `sampler` — [`L219`](../../../../../raw/code/openevolve/tests/test_artifacts.py#L219)
- uses (calls/refs, reference-scoped): [`build_prompt`](../openevolve/prompt/sampler.md#PromptSampler.build_prompt), [`PromptSampler`](../openevolve/prompt/sampler.md#PromptSampler), [`_render_artifacts`](../openevolve/prompt/sampler.md#PromptSampler._render_artifacts), [`PromptConfig`](../openevolve/config.md#PromptConfig), [`_safe_decode_artifact`](../openevolve/prompt/sampler.md#PromptSampler._safe_decode_artifact)

