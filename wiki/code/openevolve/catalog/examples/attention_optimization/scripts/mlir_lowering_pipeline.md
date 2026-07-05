---
title: 'Module: examples/attention_optimization/scripts/mlir_lowering_pipeline.py'
type: catalog
provenance: extracted
module: examples/attention_optimization/scripts/mlir_lowering_pipeline.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.attention_optimization.scripts.mlir_lowering_pipeline`/
symbols:
  MLIRLoweringPipeline.process_file: MLIRLoweringPipeline#process_file().
  main: main().
  MLIRLoweringPipeline.test_lowering_passes: MLIRLoweringPipeline#test_lowering_passes().
  MLIRLoweringPipeline.__init__: MLIRLoweringPipeline#__init__().
  MLIRLoweringPipeline: MLIRLoweringPipeline#
  MLIRLoweringPipeline.verify_tools: MLIRLoweringPipeline#verify_tools().
  MLIRLoweringPipeline.find_available_passes: MLIRLoweringPipeline#find_available_passes().
  MLIRLoweringPipeline.test_pass_sequence: MLIRLoweringPipeline#test_pass_sequence().
  MLIRLoweringPipeline.create_lowered_file: MLIRLoweringPipeline#create_lowered_file().
---
# Module: [`examples/attention_optimization/scripts/mlir_lowering_pipeline.py`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py)

## Classes
### `MLIRLoweringPipeline`
- def: [`examples/attention_optimization/scripts/mlir_lowering_pipeline.py:13`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L13)
- signature: `class MLIRLoweringPipeline:`
- members:
  - `create_lowered_file(self, input_file, output_file, pass_sequence)` — [`L141`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L141) — Create a fully lowered MLIR file
  - `find_available_passes(self)` — [`L25`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L25) — Find what lowering passes are available
  - `process_file(self, input_file)` — [`L192`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L192) — Complete pipeline to lower an MLIR file
  - `test_lowering_passes(self, input_file)` — [`L58`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L58) — Test different lowering pass combinations
  - `test_pass_sequence(self, input_file, passes)` — [`L104`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L104) — Test a specific sequence of passes
  - `verify_tools(self)` — [`L17`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L17) — Verify required MLIR tools
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L14)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L227`](../../../../../../../raw/code/openevolve/examples/attention_optimization/scripts/mlir_lowering_pipeline.py#L227)

