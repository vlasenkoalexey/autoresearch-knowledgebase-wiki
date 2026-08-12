---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.solver.greedy`/GreedySolverConfig#
symbols:
  GreedySolverConfig: ''
  GreedySolverConfig.validate: validate().
  GreedySolverConfig.improvement_steps: improvement_steps.
  GreedySolverConfig.data_preview: data_preview.
  GreedySolverConfig.max_debug_depth: max_debug_depth.
  GreedySolverConfig.debug_prob: debug_prob.
  GreedySolverConfig.num_drafts: num_drafts.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py)

## Classes
### `GreedySolverConfig`  ·  implements/extends SolverConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L15)
- signature: `class GreedySolverConfig(SolverConfig):`
- members:
  - `validate(self)` — [`L59`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L59)
  - `data_preview` — [`L25`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L25)
  - `debug_prob` — [`L42`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L42)
  - `improvement_steps` — [`L17`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L17)
  - `max_debug_depth` — [`L34`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L34)
  - `num_drafts` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/greedy.py#L51)
- uses (calls/refs, reference-scoped): [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate)
- used by: [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate), [`__init__`](../../solvers/greedy/greedy.md#Greedy.__init__)

