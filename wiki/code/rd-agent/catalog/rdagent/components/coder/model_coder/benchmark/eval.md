---
title: 'Module: rdagent/components/coder/model_coder/benchmark/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.eval`/
symbols:
  ModelImpValEval.evaluate: ModelImpValEval#evaluate().
  ModelImpValEval: ModelImpValEval#
  ModelImpValEval.norm: ModelImpValEval#norm().
  get_data_conf: get_data_conf().
---
# Module: [`rdagent/components/coder/model_coder/benchmark/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/eval.py)

## Classes
### `ModelImpValEval`
- def: [`rdagent/components/coder/model_coder/benchmark/eval.py:17`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/eval.py#L17)
- doc: Evaluate the similarity of the model structure by changing the input and observe the output.
- signature: `class ModelImpValEval:`
- members:
  - `evaluate(self, gt: ModelFBWorkspace, gen: ModelFBWorkspace)` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/eval.py#L35)
  - `norm(x)` — [`L60`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/eval.py#L60)
- uses (calls/refs, reference-scoped): [`execute`](../model.md#ModelFBWorkspace.execute), [`ModelFBWorkspace`](../model.md#ModelFBWorkspace)
- used by: (3 test-only callers)

## Functions
- `get_data_conf(init_val)` — [`L7`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/eval.py#L7)

