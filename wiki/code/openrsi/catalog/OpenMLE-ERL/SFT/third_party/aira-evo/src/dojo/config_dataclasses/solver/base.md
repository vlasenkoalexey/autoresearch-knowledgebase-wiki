---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.solver.base`/SolverConfig#
symbols:
  SolverConfig: ''
  SolverConfig.operators: operators.
  SolverConfig.time_limit_secs: time_limit_secs.
  SolverConfig.validate: validate().
  SolverConfig.checkpoint_path: checkpoint_path.
  SolverConfig.max_llm_call_retries: max_llm_call_retries.
  SolverConfig.step_limit: step_limit.
  SolverConfig.use_complexity: use_complexity.
  SolverConfig.memory: memory.
  SolverConfig.debug_memory: debug_memory.
  SolverConfig.use_test_score: use_test_score.
  SolverConfig.available_packages: available_packages.
  SolverConfig.exp_name: exp_name.
  SolverConfig.execution_timeout: execution_timeout.
  SolverConfig.export_search_results: export_search_results.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py)

## Classes
### `SolverConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py:18`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L18)
- signature: `class SolverConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L135`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L135)
  - `available_packages` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L27)
  - `checkpoint_path` — [`L101`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L101)
  - `debug_memory` — [`L60`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L60)
  - `execution_timeout` — [`L78`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L78)
  - `exp_name` — [`L69`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L69)
  - `export_search_results` — [`L92`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L92)
  - `max_llm_call_retries` — [`L126`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L126)
  - `memory` — [`L53`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L53)
  - `operators` — [`L46`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L46)
  - `step_limit` — [`L19`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L19)
  - `time_limit_secs` — [`L85`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L85)
  - `use_complexity` — [`L118`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L118)
  - `use_test_score` — [`L110`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/base.py#L110)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`MemoryOpConfig`](../operators/memory.md#MemoryOpConfig), [`OperatorConfig`](../operators/base.md#OperatorConfig), [`EvolutionarySolverConfig`](evo.md#EvolutionarySolverConfig), [`GreedySolverConfig`](greedy.md#GreedySolverConfig), [`MCTSSolverConfig`](mcts.md#MCTSSolverConfig), [`validate`](evo.md#EvolutionarySolverConfig.validate), [`validate`](greedy.md#GreedySolverConfig.validate), [`validate`](mcts.md#MCTSSolverConfig.validate)
- used by: [`search`](../../solvers/evo/evo.md#Evolutionary.search), [`_main`](../../main_run.md#_main), [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`parse_eval_result`](../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`_draft`](../../solvers/greedy/greedy.md#Greedy._draft), [`_expand_leaf_and_backprop`](../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`_draft`](../../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../../solvers/evo/evo.md#Evolutionary._improve), [`_improve`](../../solvers/greedy/greedy.md#Greedy._improve), [`_crossover`](../../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../../solvers/evo/evo.md#Evolutionary._debug), [`_debug`](../../solvers/greedy/greedy.md#Greedy._debug), [`debug_cycle`](../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`_draft`](../../solvers/mcts/mcts.md#MCTS._draft), [`_improve`](../../solvers/mcts/mcts.md#MCTS._improve), [`__call__`](../../solvers/greedy/greedy.md#Greedy.__call__), [`__call__`](../../solvers/mcts/mcts.md#MCTS.__call__), [`_debug`](../../solvers/mcts/mcts.md#MCTS._debug), [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`load_checkpoint`](../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`save_checkpoint`](../../solvers/evo/evo.md#Evolutionary.save_checkpoint), [`save_checkpoint`](../../solvers/greedy/greedy.md#Greedy.save_checkpoint), [`save_checkpoint`](../../solvers/mcts/mcts.md#MCTS.save_checkpoint), [`remaining_steps`](../../solvers/mcts/mcts.md#MCTS.remaining_steps), [`memory_op`](../../solvers/evo/evo.md#Evolutionary.memory_op), [`memory_op`](../../solvers/greedy/greedy.md#Greedy.memory_op), [`memory_op`](../../solvers/mcts/mcts.md#MCTS.memory_op), [`debug_memory_op`](../../solvers/evo/evo.md#Evolutionary.debug_memory_op), [`debug_memory_op`](../../solvers/greedy/greedy.md#Greedy.debug_memory_op), [`debug_memory_op`](../../solvers/mcts/mcts.md#MCTS.debug_memory_op), [`setup_operators`](../../solvers/evo/evo.md#Evolutionary.setup_operators), [`setup_operators`](../../solvers/greedy/greedy.md#Greedy.setup_operators), [`setup_operators`](../../solvers/mcts/mcts.md#MCTS.setup_operators), [`solver`](../run.md#RunConfig.solver)  (+8 more)

