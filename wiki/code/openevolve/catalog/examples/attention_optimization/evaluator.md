---
title: 'Module: examples/attention_optimization/evaluator.py'
type: catalog
provenance: extracted
module: examples/attention_optimization/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.attention_optimization.evaluator`/
symbols:
  MLIRAttentionEvaluator.evaluate: MLIRAttentionEvaluator#evaluate().
  result: result.
  evaluate: evaluate().
  MLIRAttentionEvaluator.mlir_file: MLIRAttentionEvaluator#mlir_file.
  MLIRAttentionEvaluator.baseline_mlir: MLIRAttentionEvaluator#baseline_mlir.
  MLIRAttentionEvaluator.baseline_metrics: MLIRAttentionEvaluator#baseline_metrics.
  MLIRAttentionEvaluator.load_baseline_mlir: MLIRAttentionEvaluator#load_baseline_mlir().
  evaluator: evaluator.
  MLIRAttentionEvaluator.__init__: MLIRAttentionEvaluator#__init__().
  MLIRAttentionEvaluator.analyze_ir_complexity: MLIRAttentionEvaluator#analyze_ir_complexity().
  MLIRAttentionEvaluator: MLIRAttentionEvaluator#
  MLIRAttentionEvaluator.verify_tools: MLIRAttentionEvaluator#verify_tools().
  MLIRAttentionEvaluator.estimate_performance_from_ir: MLIRAttentionEvaluator#estimate_performance_from_ir().
  MLIRAttentionEvaluator.apply_optimizations: MLIRAttentionEvaluator#apply_optimizations().
  test_params: test_params().
---
# Module: [`examples/attention_optimization/evaluator.py`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py)

## Classes
### `MLIRAttentionEvaluator`
- def: [`examples/attention_optimization/evaluator.py:17`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L17)
- signature: `class MLIRAttentionEvaluator:`
- members:
  - `analyze_ir_complexity(self, mlir_content)` — [`L44`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L44) — Analyze MLIR IR for performance-relevant characteristics
  - `apply_optimizations(self, mlir_content, params)` — [`L146`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L146) — Apply MLIR optimization passes based on parameters
  - `estimate_performance_from_ir(self, optimized_metrics, baseline_metrics, params)` — [`L95`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L95) — Estimate performance based on IR analysis
  - `evaluate(self, optimize_attention_input)` — [`L193`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L193) — Main evaluation function called by OpenEvolve
  - `load_baseline_mlir(self)` — [`L33`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L33) — Load baseline MLIR from file
  - `verify_tools(self)` — [`L25`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L25) — Verify MLIR tools are available
  - `baseline_metrics` — [`L23`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L23)
  - `baseline_mlir` — [`L22`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L22)
  - `mlir_file` — [`L20`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L20)
- protocol/private: `__init__`[`L18`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L18)
- used by: (2 test-only callers)

## Functions
- `evaluate(optimize_attention)` — [`L289`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L289) — Entry point for OpenEvolve
- `test_params()` — [`L296`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L296)

## Module values
- `evaluator` — [`L287`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L287)
- `result` — [`L306`](../../../../../../raw/code/openevolve/examples/attention_optimization/evaluator.py#L306)

