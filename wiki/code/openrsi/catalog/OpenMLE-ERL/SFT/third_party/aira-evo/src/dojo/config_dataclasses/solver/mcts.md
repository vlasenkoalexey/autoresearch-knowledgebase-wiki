---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.solver.mcts`/MCTSSolverConfig#
symbols:
  MCTSSolverConfig: ''
  MCTSSolverConfig.validate: validate().
  MCTSSolverConfig.num_children: num_children.
  MCTSSolverConfig.max_debug_depth: max_debug_depth.
  MCTSSolverConfig.uct_c: uct_c.
  MCTSSolverConfig.max_debug_time: max_debug_time.
  MCTSSolverConfig.data_preview: data_preview.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py)

## Classes
### `MCTSSolverConfig`  ·  implements/extends SolverConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py:15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L15)
- signature: `class MCTSSolverConfig(SolverConfig):`
- members:
  - `validate(self)` — [`L33`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L33)
  - `data_preview` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L28)
  - `max_debug_depth` — [`L20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L20)
  - `max_debug_time` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L24)
  - `num_children` — [`L17`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L17)
  - `uct_c` — [`L21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/mcts.py#L21)
- uses (calls/refs, reference-scoped): [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate)
- used by: [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate), [`__init__`](../../solvers/mcts/mcts.md#MCTS.__init__)

