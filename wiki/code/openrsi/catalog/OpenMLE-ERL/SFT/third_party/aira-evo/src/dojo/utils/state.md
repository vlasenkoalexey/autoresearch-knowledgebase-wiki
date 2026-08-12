---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.utils.state`/
symbols:
  GreedyState.current_step: GreedyState#current_step.
  MCTSState.current_step: MCTSState#current_step.
  EvolutionaryState.current_step: EvolutionaryState#current_step.
  GreedyState.state_dict: GreedyState#state_dict().
  EvolutionaryState.state_dict: EvolutionaryState#state_dict().
  EvolutionaryState.load_state_dict: EvolutionaryState#load_state_dict().
  EvolutionaryState.running_time: EvolutionaryState#running_time.
  GreedyState.running_time: GreedyState#running_time.
  MCTSState.running_time: MCTSState#running_time.
  GreedyState.load_state_dict: GreedyState#load_state_dict().
  MCTSState.state_dict: MCTSState#state_dict().
  MCTSState.load_state_dict: MCTSState#load_state_dict().
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
  GreedyState.current_generation: GreedyState#current_generation.
  BaseState.__init__: BaseState#__init__().
  GreedyState.__init__: GreedyState#__init__().
  MCTSState.__init__: MCTSState#__init__().
  EvolutionaryState.__init__: EvolutionaryState#__init__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py)

## Classes
### `BaseState`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py:8`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L8)
- signature: `class BaseState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L21)
  - `state_dict(self)` — [`L15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L15)
  - `num_starts` — [`L10`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L10)
  - `running_time` — [`L9`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L9)
- protocol/private: `__init__`[`L12`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L12)
- used by: [`load_checkpoint`](../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../core/solvers/base.md#Solver.save_checkpoint), [`state`](../core/solvers/base.md#Solver.state)

### `EvolutionaryState`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py:70`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L70)
- signature: `class EvolutionaryState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L87`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L87)
  - `state_dict(self)` — [`L79`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L79)
  - `current_generation` — [`L73`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L73)
  - `current_step` — [`L71`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L71)
  - `num_starts` — [`L74`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L74)
  - `running_time` — [`L72`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L72)
- protocol/private: `__init__`[`L76`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L76)
- used by: [`search`](../solvers/evo/evo.md#Evolutionary.search), [`_draft`](../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../solvers/evo/evo.md#Evolutionary._improve), [`_crossover`](../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../solvers/evo/evo.md#Evolutionary._debug), [`create_root_node`](../solvers/evo/evo.md#Evolutionary.create_root_node), [`state`](../solvers/evo/evo.md#Evolutionary.state), [`load_checkpoint`](../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`log_journal`](../solvers/evo/evo.md#Evolutionary.log_journal)

### `GreedyState`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py:26`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L26)
- signature: `class GreedyState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L42`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L42)
  - `state_dict(self)` — [`L34`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L34)
  - `current_generation` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L44)
  - `current_step` — [`L27`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L27)
  - `num_starts` — [`L29`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L29)
  - `running_time` — [`L28`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L28)
- protocol/private: `__init__`[`L31`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L31)
- used by: [`_draft`](../solvers/greedy/greedy.md#Greedy._draft), [`_improve`](../solvers/greedy/greedy.md#Greedy._improve), [`step`](../solvers/greedy/greedy.md#Greedy.step), [`_debug`](../solvers/greedy/greedy.md#Greedy._debug), [`create_root_node`](../solvers/greedy/greedy.md#Greedy.create_root_node), [`__call__`](../solvers/greedy/greedy.md#Greedy.__call__), [`state`](../solvers/greedy/greedy.md#Greedy.state), [`load_checkpoint`](../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`_analyze`](../solvers/greedy/greedy.md#Greedy._analyze)

### `MCTSState`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py:49`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L49)
- signature: `class MCTSState:`
- members:
  - `load_state_dict(self, state_dict)` — [`L64`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L64)
  - `state_dict(self)` — [`L57`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L57)
  - `current_step` — [`L50`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L50)
  - `num_starts` — [`L52`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L52)
  - `running_time` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L51)
- protocol/private: `__init__`[`L54`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/state.py#L54)
- used by: [`_expand_leaf_and_backprop`](../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`debug_cycle`](../solvers/mcts/mcts.md#MCTS.debug_cycle), [`_draft`](../solvers/mcts/mcts.md#MCTS._draft), [`_improve`](../solvers/mcts/mcts.md#MCTS._improve), [`__call__`](../solvers/mcts/mcts.md#MCTS.__call__), [`_debug`](../solvers/mcts/mcts.md#MCTS._debug), [`state`](../solvers/mcts/mcts.md#MCTS.state), [`create_root_node`](../solvers/mcts/mcts.md#MCTS.create_root_node), [`step`](../solvers/mcts/mcts.md#MCTS.step), [`load_checkpoint`](../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`log_journal`](../solvers/mcts/mcts.md#MCTS.log_journal), [`remaining_steps`](../solvers/mcts/mcts.md#MCTS.remaining_steps)

