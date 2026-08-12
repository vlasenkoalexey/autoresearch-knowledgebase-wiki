---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.base`/Solver#
symbols:
  Solver.cfg: cfg.
  Solver.logger: logger.
  Solver.load_checkpoint: load_checkpoint().
  Solver.save_checkpoint: save_checkpoint().
  Solver: ''
  Solver.__init__: __init__().
  Solver.state: state.
  Solver.start_time: start_time.
  Solver.task_info: task_info.
  Solver.__call__: __call__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py)

## Classes
### `Solver`  ·  implements/extends ABC
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py:20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L20)
- signature: `class Solver(ABC):`
- members:
  - `load_checkpoint(self)` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L41)
  - `save_checkpoint(self)` — [`L34`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L34)
  - `cfg` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L22)
  - `logger` — [`L23`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L23)
  - `start_time` — [`L25`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L25)
  - `state` — [`L28`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L28)
  - `task_info` — [`L24`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L24)
- protocol/private: `__call__`[`L31`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L31), `__init__`[`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/base.py#L21)
- uses (calls/refs, reference-scoped): [`SolverConfig`](../../config_dataclasses/solver/base.md#SolverConfig), [`load_checkpoint`](../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`save_checkpoint`](../../solvers/evo/evo.md#Evolutionary.save_checkpoint), [`save_checkpoint`](../../solvers/greedy/greedy.md#Greedy.save_checkpoint), [`save_checkpoint`](../../solvers/mcts/mcts.md#MCTS.save_checkpoint), [`get_logger`](../../utils/logger.md#get_logger), [`checkpoint_path`](../../config_dataclasses/solver/base.md#SolverConfig.checkpoint_path), [`load_state_dict`](../../utils/state.md#BaseState.load_state_dict), [`state_dict`](../../utils/state.md#BaseState.state_dict), [`Greedy`](../../solvers/greedy/greedy.md#Greedy), [`MCTS`](../../solvers/mcts/mcts.md#MCTS), [`Evolutionary`](../../solvers/evo/evo.md#Evolutionary), [`num_starts`](../../utils/state.md#BaseState.num_starts), [`BaseState`](../../utils/state.md#BaseState)
- used by: [`search`](../../solvers/evo/evo.md#Evolutionary.search), [`parse_eval_result`](../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`_draft`](../../solvers/greedy/greedy.md#Greedy._draft), [`_expand_leaf_and_backprop`](../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`_draft`](../../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../../solvers/evo/evo.md#Evolutionary._improve), [`_debug_cycle_async`](../../solvers/evo/evo.md#Evolutionary._debug_cycle_async), [`_async_worker_loop`](../../solvers/evo/evo.md#Evolutionary._async_worker_loop), [`_improve`](../../solvers/greedy/greedy.md#Greedy._improve), [`step`](../../solvers/greedy/greedy.md#Greedy.step), [`_crossover`](../../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../../solvers/evo/evo.md#Evolutionary._debug), [`root_node`](../../solvers/evo/evo.md#Evolutionary.root_node), [`_next_async_work_item`](../../solvers/evo/evo.md#Evolutionary._next_async_work_item), [`_debug`](../../solvers/greedy/greedy.md#Greedy._debug), [`debug_cycle`](../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`create_root_node`](../../solvers/greedy/greedy.md#Greedy.create_root_node), [`_draft`](../../solvers/mcts/mcts.md#MCTS._draft), [`debug_cycle`](../../solvers/evo/evo.md#Evolutionary.debug_cycle), [`_improve`](../../solvers/mcts/mcts.md#MCTS._improve), [`_commit_async_node`](../../solvers/evo/evo.md#Evolutionary._commit_async_node), [`__call__`](../../solvers/greedy/greedy.md#Greedy.__call__), [`__call__`](../../solvers/mcts/mcts.md#MCTS.__call__), [`_debug`](../../solvers/mcts/mcts.md#MCTS._debug), [`__call__`](../../solvers/evo/evo.md#Evolutionary.__call__), [`_ensure_node_rich_summary_unlocked`](../../solvers/evo/evo.md#Evolutionary._ensure_node_rich_summary_unlocked), [`_prepare_operator_rich_memory`](../../solvers/evo/evo.md#Evolutionary._prepare_operator_rich_memory), [`_should_stop_async_search`](../../solvers/evo/evo.md#Evolutionary._should_stop_async_search), [`search_policy`](../../solvers/greedy/greedy.md#Greedy.search_policy), [`step`](../../solvers/mcts/mcts.md#MCTS.step), [`load_checkpoint`](../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`_analyze`](../../solvers/greedy/greedy.md#Greedy._analyze), [`search_policy`](../../solvers/mcts/mcts.md#MCTS.search_policy), [`log_journal`](../../solvers/mcts/mcts.md#MCTS.log_journal), [`log_journal`](../../solvers/evo/evo.md#Evolutionary.log_journal), [`save_checkpoint`](../../solvers/evo/evo.md#Evolutionary.save_checkpoint)  (+47 more)

