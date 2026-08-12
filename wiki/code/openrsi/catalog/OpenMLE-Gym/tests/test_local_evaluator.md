---
title: 'Module: OpenMLE-Gym/tests/test_local_evaluator.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_local_evaluator.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_local_evaluator`/
symbols:
  _make_task: _make_task().
  LocalEvaluatorTests.test_llm_failure_is_not_reported_as_not_recommended: LocalEvaluatorTests#test_llm_failure_is_not_reported_as_not_recommended().
  LocalEvaluatorTests.test_structure_validation_uses_csv_records_and_alignment: LocalEvaluatorTests#test_structure_validation_uses_csv_records_and_alignment().
  LocalEvaluatorTests.test_structural_mismatch_is_a_deterministic_failure: LocalEvaluatorTests#test_structural_mismatch_is_a_deterministic_failure().
  LocalEvaluatorTests.test_metric_owns_submission_answer_schema_and_identifier_alignment: LocalEvaluatorTests#test_metric_owns_submission_answer_schema_and_identifier_alignment().
  LocalEvaluatorTests.test_online_hard_gate_does_not_call_quality_judge: LocalEvaluatorTests#test_online_hard_gate_does_not_call_quality_judge().
  LocalEvaluatorTests.test_local_only_performs_no_quality_scoring: LocalEvaluatorTests#test_local_only_performs_no_quality_scoring().
  LocalEvaluatorTests.test_quality_result_is_validated_and_recomputed: LocalEvaluatorTests#test_quality_result_is_validated_and_recomputed().
  LocalEvaluatorTests.test_major_issue_requires_structured_evidence: LocalEvaluatorTests#test_major_issue_requires_structured_evidence().
  LocalEvaluatorTests.test_prompt_documents_random_submission_and_holdout_contract: LocalEvaluatorTests#test_prompt_documents_random_submission_and_holdout_contract().
  _judge_result: _judge_result().
  LocalEvaluatorTests.test_csv_inspection_counts_logical_records_and_labels_preview: LocalEvaluatorTests#test_csv_inspection_counts_logical_records_and_labels_preview().
  METRIC_CODE: METRIC_CODE.
  LocalEvaluatorTests: LocalEvaluatorTests#
---
# Module: [`OpenMLE-Gym/tests/test_local_evaluator.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py)

## Classes
### `LocalEvaluatorTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_local_evaluator.py:85`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L85)
- signature: `class LocalEvaluatorTests(unittest.TestCase):`
- members:
  - `test_csv_inspection_counts_logical_records_and_labels_preview(self)` — [`L86`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L86)
  - `test_llm_failure_is_not_reported_as_not_recommended(self)` — [`L194`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L194)
  - `test_local_only_performs_no_quality_scoring(self)` — [`L180`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L180)
  - `test_major_issue_requires_structured_evidence(self)` — [`L228`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L228)
  - `test_metric_owns_submission_answer_schema_and_identifier_alignment(self)` — [`L131`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L131)
  - `test_online_hard_gate_does_not_call_quality_judge(self)` — [`L151`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L151)
  - `test_prompt_documents_random_submission_and_holdout_contract(self)` — [`L234`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L234)
  - `test_quality_result_is_validated_and_recomputed(self)` — [`L220`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L220)
  - `test_structural_mismatch_is_a_deterministic_failure(self)` — [`L117`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L117)
  - `test_structure_validation_uses_csv_records_and_alignment(self)` — [`L99`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L99)
- uses (calls/refs, reference-scoped): [`_evaluate_with_ai`](../openmle_gym/local_evaluator.md#_evaluate_with_ai), [`analyze_task_structure`](../openmle_gym/local_evaluator.md#analyze_task_structure), [`_evaluate_task`](../openmle_gym/local_evaluator.md#_evaluate_task), [`_inspect_csv`](../openmle_gym/local_evaluator.md#_inspect_csv), [`_validate_ai_quality`](../openmle_gym/local_evaluator.md#_validate_ai_quality), [`evaluation_has_task_failures`](../openmle_gym/local_evaluator.md#evaluation_has_task_failures)  (2 test-only)

## Functions
- `_judge_result()` — [`L69`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L69)
- `_make_task(root: Path, name: str = "fixture")` — [`L26`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L26)

## Module values
- `METRIC_CODE` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_local_evaluator.py#L19)

