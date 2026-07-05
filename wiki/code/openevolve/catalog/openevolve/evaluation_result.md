---
title: 'Module: openevolve/evaluation_result.py'
type: catalog
provenance: extracted
module: openevolve/evaluation_result.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.evaluation_result`/EvaluationResult#
symbols:
  EvaluationResult.metrics: metrics.
  EvaluationResult: ''
  EvaluationResult.artifacts: artifacts.
  EvaluationResult.has_artifacts: has_artifacts().
  EvaluationResult.get_total_artifact_size: get_total_artifact_size().
  EvaluationResult.from_dict: from_dict().
  EvaluationResult.get_artifact_size: get_artifact_size().
  EvaluationResult.to_dict: to_dict().
  EvaluationResult.get_artifact_keys: get_artifact_keys().
---
# Module: [`openevolve/evaluation_result.py`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py)

## Classes
### `EvaluationResult`
- def: [`openevolve/evaluation_result.py:11`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L11) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- doc: Result of program evaluation containing both metrics and optional artifacts
- signature: `class EvaluationResult:`
- members:
  - `from_dict(cls, metrics: Dict[str, float])` — [`L31`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L31) — Auto-wrap dict returns for backward compatibility — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `get_artifact_keys(self)` — [`L43`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L43) — Get list of artifact keys — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `get_artifact_size(self, key: str)` — [`L47`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L47) — Get size of a specific artifact in bytes — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `get_total_artifact_size(self)` — [`L60`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L60) — Get total size of all artifacts in bytes — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `has_artifacts(self)` — [`L39`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L39) — Check if this result contains any artifacts — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `to_dict(self)` — [`L35`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L35) — Backward compatibility - return just metrics — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `artifacts` — [`L28`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L28) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `metrics` — [`L27`](../../../../../raw/code/openevolve/openevolve/evaluation_result.py#L27) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- used by: [`evaluate_program`](evaluator.md#Evaluator.evaluate_program), [`_cascade_evaluate`](evaluator.md#Evaluator._cascade_evaluate), [`_llm_evaluate`](evaluator.md#Evaluator._llm_evaluate), [`_process_evaluation_result`](evaluator.md#Evaluator._process_evaluation_result), [`_direct_evaluate`](evaluator.md#Evaluator._direct_evaluate)  (32 test-only)

