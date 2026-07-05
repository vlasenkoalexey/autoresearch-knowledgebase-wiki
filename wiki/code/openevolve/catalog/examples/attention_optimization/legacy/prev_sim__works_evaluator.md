---
title: 'Module: examples/attention_optimization/legacy/prev_sim__works_evaluator.py'
type: catalog
provenance: extracted
module: examples/attention_optimization/legacy/prev_sim__works_evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.attention_optimization.legacy.prev_sim__works_evaluator`/
symbols:
  evaluate: evaluate().
  MLIRAttentionEvaluator.get_reference_performance: MLIRAttentionEvaluator#get_reference_performance().
  MLIRAttentionEvaluator.load_base_mlir: MLIRAttentionEvaluator#load_base_mlir().
  MLIRAttentionEvaluator.compile_mlir_with_optimizations: MLIRAttentionEvaluator#compile_mlir_with_optimizations().
  MLIRAttentionEvaluator.benchmark_implementation: MLIRAttentionEvaluator#benchmark_implementation().
  MLIRAttentionEvaluator.test_configs: MLIRAttentionEvaluator#test_configs.
  MLIRAttentionEvaluator.reference_performance: MLIRAttentionEvaluator#reference_performance.
  MLIRAttentionEvaluator.base_mlir_file: MLIRAttentionEvaluator#base_mlir_file.
  MLIRAttentionEvaluator: MLIRAttentionEvaluator#
  MLIRAttentionEvaluator.create_baseline_mlir: MLIRAttentionEvaluator#create_baseline_mlir().
  MLIRAttentionEvaluator.apply_optimizations: MLIRAttentionEvaluator#apply_optimizations().
  MLIRAttentionEvaluator.simulate_mlir_compilation: MLIRAttentionEvaluator#simulate_mlir_compilation().
  MLIRAttentionEvaluator.calculate_speedup_factor: MLIRAttentionEvaluator#calculate_speedup_factor().
  MLIRAttentionEvaluator.__init__: MLIRAttentionEvaluator#__init__().
---
# Module: [`examples/attention_optimization/legacy/prev_sim__works_evaluator.py`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py)

## Classes
### `MLIRAttentionEvaluator`
- def: [`examples/attention_optimization/legacy/prev_sim__works_evaluator.py:262`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L262)
- doc: Evaluates MLIR attention optimizations
- signature: `class MLIRAttentionEvaluator:`
- members:
  - `apply_optimizations(self, base_mlir, params)` — [`L322`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L322) — Apply optimization parameters to base MLIR
  - `benchmark_implementation(self, optimized_mlir, test_config)` — [`L357`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L357) — Benchmark the optimized implementation
  - `calculate_speedup_factor(self, optimized_mlir)` — [`L377`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L377) — Calculate speedup factor based on applied optimizations
  - `compile_mlir_with_optimizations(self, base_mlir, optimization_params)` — [`L308`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L308) — Apply optimizations and compile MLIR
  - `create_baseline_mlir(self)` — [`L286`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L286) — Create a simple baseline MLIR attention implementation
  - `get_reference_performance(self)` — [`L412`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L412) — Get baseline performance for comparison
  - `load_base_mlir(self)` — [`L277`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L277) — Load the baseline MLIR implementation
  - `simulate_mlir_compilation(self, mlir_code)` — [`L342`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L342) — Simulate MLIR compilation success
  - `base_mlir_file` — [`L267`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L267)
  - `reference_performance` — [`L268`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L268)
  - `test_configs` — [`L271`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L271)
- protocol/private: `__init__`[`L265`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L265)
- used by: (1 test-only callers)

## Functions
- `evaluate(program_path)` — [`L427`](../../../../../../../raw/code/openevolve/examples/attention_optimization/legacy/prev_sim__works_evaluator.py#L427) — Main evaluation function called by OpenEvolve.

