---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.base`/Solver#
symbols:
  Solver.logger: logger.
  Solver.cfg: cfg.
  Solver.load_checkpoint: load_checkpoint().
  Solver.save_checkpoint: save_checkpoint().
  Solver: ''
  Solver.__init__: __init__().
  Solver.state: state.
  Solver.task_info: task_info.
  Solver.start_time: start_time.
  Solver.__call__: __call__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py)

## Classes
### `Solver`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py:20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L20)
- signature: `class Solver(ABC):`
- members:
  - `load_checkpoint(self)` — [`L41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L41)
  - `save_checkpoint(self)` — [`L34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L34)
  - `cfg` — [`L22`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L22)
  - `logger` — [`L23`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L23)
  - `start_time` — [`L25`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L25)
  - `state` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L28)
  - `task_info` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L24)
- protocol/private: `__call__`[`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L31), `__init__`[`L21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/base.py#L21)
- uses (calls/refs, reference-scoped): [`SolverConfig`](../../config_dataclasses/solver/base.md#SolverConfig), [`load_checkpoint`](../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`save_checkpoint`](../../solvers/evo/evo.md#Evolutionary.save_checkpoint), [`save_checkpoint`](../../solvers/greedy/greedy.md#Greedy.save_checkpoint), [`save_checkpoint`](../../solvers/mcts/mcts.md#MCTS.save_checkpoint), [`get_logger`](../../utils/logger.md#get_logger), [`checkpoint_path`](../../config_dataclasses/solver/base.md#SolverConfig.checkpoint_path), [`load_state_dict`](../../utils/state.md#BaseState.load_state_dict), [`state_dict`](../../utils/state.md#BaseState.state_dict), [`Evolutionary`](../../solvers/evo/evo.md#Evolutionary), [`Greedy`](../../solvers/greedy/greedy.md#Greedy), [`MCTS`](../../solvers/mcts/mcts.md#MCTS), [`num_starts`](../../utils/state.md#BaseState.num_starts), [`BaseState`](../../utils/state.md#BaseState)
- used by: [`search`](../../solvers/evo/evo.md#Evolutionary.search), [`parse_eval_result`](../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`_draft`](../../solvers/greedy/greedy.md#Greedy._draft), [`_expand_leaf_and_backprop`](../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`_draft`](../../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../../solvers/evo/evo.md#Evolutionary._improve), [`_improve`](../../solvers/greedy/greedy.md#Greedy._improve), [`step`](../../solvers/greedy/greedy.md#Greedy.step), [`_crossover`](../../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../../solvers/evo/evo.md#Evolutionary._debug), [`_debug`](../../solvers/greedy/greedy.md#Greedy._debug), [`debug_cycle`](../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`create_root_node`](../../solvers/greedy/greedy.md#Greedy.create_root_node), [`_draft`](../../solvers/mcts/mcts.md#MCTS._draft), [`_improve`](../../solvers/mcts/mcts.md#MCTS._improve), [`debug_cycle`](../../solvers/evo/evo.md#Evolutionary.debug_cycle), [`__call__`](../../solvers/greedy/greedy.md#Greedy.__call__), [`__call__`](../../solvers/mcts/mcts.md#MCTS.__call__), [`_build_solution_database_from_journal`](../../solvers/evo/evo.md#Evolutionary._build_solution_database_from_journal), [`_debug`](../../solvers/mcts/mcts.md#MCTS._debug), [`__call__`](../../solvers/evo/evo.md#Evolutionary.__call__), [`search_policy`](../../solvers/greedy/greedy.md#Greedy.search_policy), [`step`](../../solvers/mcts/mcts.md#MCTS.step), [`load_checkpoint`](../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`_analyze`](../../solvers/greedy/greedy.md#Greedy._analyze), [`search_policy`](../../solvers/mcts/mcts.md#MCTS.search_policy), [`log_journal`](../../solvers/evo/evo.md#Evolutionary.log_journal), [`log_journal`](../../solvers/mcts/mcts.md#MCTS.log_journal), [`_analyze`](../../solvers/evo/evo.md#Evolutionary._analyze), [`_analyze`](../../solvers/mcts/mcts.md#MCTS._analyze), [`save_checkpoint`](../../solvers/evo/evo.md#Evolutionary.save_checkpoint), [`save_checkpoint`](../../solvers/greedy/greedy.md#Greedy.save_checkpoint), [`save_checkpoint`](../../solvers/mcts/mcts.md#MCTS.save_checkpoint), [`remaining_steps`](../../solvers/mcts/mcts.md#MCTS.remaining_steps), [`crossover_fn`](../../solvers/evo/evo.md#Evolutionary.crossover_fn), [`debug_fn`](../../solvers/evo/evo.md#Evolutionary.debug_fn)  (+30 more)

