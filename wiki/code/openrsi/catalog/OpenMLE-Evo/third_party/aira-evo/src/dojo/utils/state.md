---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.utils.state`/
symbols:
  GreedyState.current_step: GreedyState#current_step.
  MCTSState.current_step: MCTSState#current_step.
  EvolutionaryState.current_step: EvolutionaryState#current_step.
  EvolutionaryState.running_time: EvolutionaryState#running_time.
  GreedyState.state_dict: GreedyState#state_dict().
  GreedyState.running_time: GreedyState#running_time.
  MCTSState.running_time: MCTSState#running_time.
  GreedyState.load_state_dict: GreedyState#load_state_dict().
  MCTSState.state_dict: MCTSState#state_dict().
  MCTSState.load_state_dict: MCTSState#load_state_dict().
  EvolutionaryState.state_dict: EvolutionaryState#state_dict().
  EvolutionaryState.load_state_dict: EvolutionaryState#load_state_dict().
  BaseState.state_dict: BaseState#state_dict().
  BaseState.load_state_dict: BaseState#load_state_dict().
  EvolutionaryState.current_generation: EvolutionaryState#current_generation.
  BaseState.num_starts: BaseState#num_starts.
  BaseState: BaseState#
  BaseState.running_time: BaseState#running_time.
  GreedyState: GreedyState#
  GreedyState.num_starts: GreedyState#num_starts.
  MCTSState: MCTSState#
  MCTSState.num_starts: MCTSState#num_starts.
  EvolutionaryState: EvolutionaryState#
  EvolutionaryState.num_starts: EvolutionaryState#num_starts.
  BaseState.__init__: BaseState#__init__().
  GreedyState.__init__: GreedyState#__init__().
  MCTSState.__init__: MCTSState#__init__().
  EvolutionaryState.__init__: EvolutionaryState#__init__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py)

## Classes
### `BaseState`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py:8`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L8)
- signature: `class BaseState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L21)
  - `state_dict(self)` — [`L15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L15)
  - `num_starts` — [`L10`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L10)
  - `running_time` — [`L9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L9)
- protocol/private: `__init__`[`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L12)
- used by: [`load_checkpoint`](../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../core/solvers/base.md#Solver.save_checkpoint), [`state`](../core/solvers/base.md#Solver.state)

### `EvolutionaryState`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py:68`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L68)
- signature: `class EvolutionaryState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L84`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L84)
  - `state_dict(self)` — [`L77`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L77)
  - `current_generation` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L71)
  - `current_step` — [`L69`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L69)
  - `num_starts` — [`L72`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L72)
  - `running_time` — [`L70`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L70)
- protocol/private: `__init__`[`L74`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L74)
- used by: [`search`](../solvers/evo/evo.md#Evolutionary.search), [`_draft`](../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../solvers/evo/evo.md#Evolutionary._improve), [`_crossover`](../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../solvers/evo/evo.md#Evolutionary._debug), [`root_node`](../solvers/evo/evo.md#Evolutionary.root_node), [`_next_async_work_item`](../solvers/evo/evo.md#Evolutionary._next_async_work_item), [`create_root_node`](../solvers/evo/evo.md#Evolutionary.create_root_node), [`_commit_async_node`](../solvers/evo/evo.md#Evolutionary._commit_async_node), [`state`](../solvers/evo/evo.md#Evolutionary.state), [`_should_stop_async_search`](../solvers/evo/evo.md#Evolutionary._should_stop_async_search), [`_append_evaluated_node`](../solvers/evo/evo.md#Evolutionary._append_evaluated_node), [`load_checkpoint`](../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`log_journal`](../solvers/evo/evo.md#Evolutionary.log_journal)

### `GreedyState`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py:26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L26)
- signature: `class GreedyState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L41)
  - `state_dict(self)` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L34)
  - `current_step` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L27)
  - `num_starts` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L29)
  - `running_time` — [`L28`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L28)
- protocol/private: `__init__`[`L31`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L31)
- used by: [`_draft`](../solvers/greedy/greedy.md#Greedy._draft), [`_improve`](../solvers/greedy/greedy.md#Greedy._improve), [`step`](../solvers/greedy/greedy.md#Greedy.step), [`_debug`](../solvers/greedy/greedy.md#Greedy._debug), [`create_root_node`](../solvers/greedy/greedy.md#Greedy.create_root_node), [`__call__`](../solvers/greedy/greedy.md#Greedy.__call__), [`state`](../solvers/greedy/greedy.md#Greedy.state), [`load_checkpoint`](../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`_analyze`](../solvers/greedy/greedy.md#Greedy._analyze)

### `MCTSState`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py:47`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L47)
- signature: `class MCTSState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L62)
  - `state_dict(self)` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L55)
  - `current_step` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L48)
  - `num_starts` — [`L50`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L50)
  - `running_time` — [`L49`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L49)
- protocol/private: `__init__`[`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/state.py#L52)
- used by: [`_expand_leaf_and_backprop`](../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`debug_cycle`](../solvers/mcts/mcts.md#MCTS.debug_cycle), [`_draft`](../solvers/mcts/mcts.md#MCTS._draft), [`_improve`](../solvers/mcts/mcts.md#MCTS._improve), [`__call__`](../solvers/mcts/mcts.md#MCTS.__call__), [`_debug`](../solvers/mcts/mcts.md#MCTS._debug), [`state`](../solvers/mcts/mcts.md#MCTS.state), [`create_root_node`](../solvers/mcts/mcts.md#MCTS.create_root_node), [`step`](../solvers/mcts/mcts.md#MCTS.step), [`load_checkpoint`](../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`log_journal`](../solvers/mcts/mcts.md#MCTS.log_journal), [`remaining_steps`](../solvers/mcts/mcts.md#MCTS.remaining_steps)

