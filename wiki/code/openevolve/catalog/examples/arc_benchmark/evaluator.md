---
title: 'Module: examples/arc_benchmark/evaluator.py'
type: catalog
provenance: extracted
module: examples/arc_benchmark/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.arc_benchmark.evaluator`/
symbols:
  evaluate: evaluate().
  pass_at_2_accuracy_multi_test: pass_at_2_accuracy_multi_test().
  extract_failure_artifacts: extract_failure_artifacts().
  TASK_FILE: TASK_FILE.
  TASK_NUM: TASK_NUM.
  DATA_ROOT: DATA_ROOT.
  pass_at_2_accuracy_single: pass_at_2_accuracy_single().
---
# Module: [`examples/arc_benchmark/evaluator.py`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py)

## Functions
- `evaluate(program_path)` — [`L113`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L113) — Evaluate the program by running it multiple times and checking how close — documented in [openevolve-evaluation_result](../../../concepts/openevolve-evaluation_result.md)
- `extract_failure_artifacts(diagnostics)` — [`L93`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L93) — Extract failure artifacts from diagnostics for a given example.
- `pass_at_2_accuracy_multi_test(all_attempts: List[List[np.ndarray]], all_gt: List[np.ndarray])` — [`L70`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L70) — Compute pass@2 accuracy across multiple ARC test cases.
- `pass_at_2_accuracy_single(attempts: List[np.ndarray], gt: np.ndarray)` — [`L14`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L14) — Compute pass@2 accuracy for a single ARC test case.

## Module values
- `DATA_ROOT` — [`L11`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L11)
- `TASK_FILE` — [`L9`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L9)
- `TASK_NUM` — [`L10`](../../../../../../raw/code/openevolve/examples/arc_benchmark/evaluator.py#L10)

