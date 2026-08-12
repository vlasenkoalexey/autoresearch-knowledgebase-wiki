---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.solvers.mcts.mcts`/
symbols:
  MCTS.parse_eval_result: MCTS#parse_eval_result().
  MCTS._expand_leaf_and_backprop: MCTS#_expand_leaf_and_backprop().
  MCTS.debug_cycle: MCTS#debug_cycle().
  MCTS._draft: MCTS#_draft().
  MCTS._improve: MCTS#_improve().
  MCTS.__call__: MCTS#__call__().
  MCTS._debug: MCTS#_debug().
  MCTS.state: MCTS#state.
  MCTS.create_root_node: MCTS#create_root_node().
  MCTS.step: MCTS#step().
  MCTS.load_checkpoint: MCTS#load_checkpoint().
  MCTS.search_policy: MCTS#search_policy().
  MCTS.log_journal: MCTS#log_journal().
  MCTSNode: MCTSNode#
  MCTS.save_checkpoint: MCTS#save_checkpoint().
  MCTS._analyze: MCTS#_analyze().
  MCTS.journal: MCTS#journal.
  MCTS.remaining_steps: MCTS#remaining_steps().
  MCTS.memory_op: MCTS#memory_op.
  MCTS._backprop_step: MCTS#_backprop_step().
  MCTS.setup_operators: MCTS#setup_operators().
  MCTS.debug_memory_op: MCTS#debug_memory_op.
  MCTS.draft_fn: MCTS#draft_fn.
  MCTS.improve_fn: MCTS#improve_fn.
  MCTS.debug_fn: MCTS#debug_fn.
  MCTS.update_data_preview: MCTS#update_data_preview().
  MCTSNode.explore_count: MCTSNode#explore_count.
  MCTS.set_global_q_values: MCTS#set_global_q_values().
  MCTS.task_desc: MCTS#task_desc.
  MCTS.lower_is_better: MCTS#lower_is_better.
  MCTS.data_preview: MCTS#data_preview.
  MCTS.analyze_fn: MCTS#analyze_fn.
  MCTS: MCTS#
  MCTSNode.node_value: MCTSNode#node_value.
  MCTSNode.q_value: MCTSNode#q_value().
  MCTSNode.extra_metrics_to_log: MCTSNode#extra_metrics_to_log().
  MCTS.__init__: MCTS#__init__().
  MCTS.root_node: MCTS#root_node.
  uct_value: uct_value().
  MCTSNode.add_value: MCTSNode#add_value().
  MCTSNode.increment_explore_count: MCTSNode#increment_explore_count().
  MCTS.global_max_q_val: MCTS#global_max_q_val.
  MCTS.global_min_q_val: MCTS#global_min_q_val.
  MCTSNode.set_value: MCTSNode#set_value().
  normalise_q_value: normalise_q_value().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py)

## Classes
### `MCTS`  ·  implements/extends Solver
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py:108`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L108)
- signature: `class MCTS(Solver):`
- members:
  - `__call__(self, task, state)` — [`L201`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L201) — Run the MCTS solver for a specified number of iterations.
  - `__init__(self, cfg: MCTSSolverConfig, task_info)` — [`L109`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L109) — Initialize the MCTS solver.
  - `_analyze(self, node: MCTSNode)` — [`L370`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L370) — Analyze a node's execution results using the analyze LLM operator.
  - `_backprop_step(self, path: List[MCTSNode], value_estimate: float)` — [`L447`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L447) — Backpropagates the reward/score up the path (increasing explore_count
  - `_debug(self, parent_node: MCTSNode)` — [`L340`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L340) — Debug a buggy solution using the debug LLM operator.
  - `_draft(self, parent: Optional[MCTSNode] = None)` — [`L283`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L283) — Generate a new solution from scratch using the draft LLM operator.
  - `_expand_leaf_and_backprop(self, path: List[MCTSNode], state: Any, task: Any)` — [`L472`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L472) — Expand a leaf node and backpropagate results.
  - `_improve(self, parent_node: MCTSNode)` — [`L309`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L309) — Improve an existing solution using the improve LLM operator.
  - `create_root_node(self)` — [`L184`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L184)
  - `debug_cycle(self, state, task, buggy_node: MCTSNode)` — [`L522`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L522)
  - `load_checkpoint(self)` — [`L144`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L144)
  - `log_journal(self)` — [`L456`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L456)
  - `parse_eval_result(self, node: Node, eval_result: Dict[str, Any])` — [`L556`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L556) — Parse evaluation results and update the node accordingly.
  - `remaining_steps(self)` — [`L198`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L198)
  - `save_checkpoint(self)` — [`L133`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L133)
  - `search_policy(self, root_node: MCTSNode)` — [`L252`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L252) — Traverse the tree from root to leaf using UCT selection.
  - `set_global_q_values(self, new_metric_value)` — [`L467`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L467)
  - `setup_operators(self)` — [`L160`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L160) — Initialize and configure the LLM operators used in the MCTS solver.
  - `step(self, task, state)` — [`L416`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L416) — Execute a single iteration of the MCTS solver process.
  - `update_data_preview(self, state)` — [`L389`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L389) — Generate a data preview to provide context for the LLM operators.
  - `analyze_fn` — [`L182`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L182)
  - `data_preview` — [`L119`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L119)
  - `debug_fn` — [`L181`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L181)
  - `debug_memory_op` — [`L176`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L176)
  - `draft_fn` — [`L179`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L179)
  - `global_max_q_val` — [`L130`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L130)
  - `global_min_q_val` — [`L131`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L131)
  - `improve_fn` — [`L180`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L180)
  - `journal` — [`L118`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L118)
  - `lower_is_better` — [`L122`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L122)
  - `memory_op` — [`L175`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L175)
  - `root_node` — [`L185`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L185)
  - `state` — [`L126`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L126)
  - `task_desc` — [`L121`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L121)
- uses (calls/refs, reference-scoped): [`logger`](../../core/solvers/base.md#Solver.logger), [`cfg`](../../core/solvers/base.md#Solver.cfg), [`Node`](../../core/solvers/utils/journal.md#Node), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`from_export_data`](../../core/solvers/utils/journal.md#Journal.from_export_data), [`get_node_data`](../../core/solvers/utils/journal.md#Journal.get_node_data), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`parents`](../../core/solvers/utils/journal.md#Node.parents), [`code`](../../core/solvers/utils/journal.md#Node.code), [`Journal`](../../core/solvers/utils/journal.md#Journal), [`nodes`](../../core/solvers/utils/journal.md#Journal.nodes), [`is_buggy`](../../core/solvers/utils/journal.md#Node.is_buggy), [`export_search_results`](../../core/solvers/utils/search_exporter.md#export_search_results), [`children`](../../core/solvers/utils/journal.md#Node.children), [`GenericLLM`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM), [`create_memory_op`](../../core/solvers/operators/memory.md#create_memory_op), [`absorb_exec_result`](../../core/solvers/utils/journal.md#Node.absorb_exec_result), [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`append`](../../core/solvers/utils/journal.md#Journal.append), [`step`](../../core/solvers/utils/journal.md#Node.step), [`generate`](../../core/solvers/utils/data_preview.md#generate), [`get_complextiy_level`](../utils.md#get_complextiy_level), [`analyze_op`](../../core/solvers/operators/analyze.md#analyze_op), [`get_best_node`](../../core/solvers/utils/journal.md#Journal.get_best_node), [`improve_op`](../../core/solvers/operators/improve.md#improve_op), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`MetricValue`](../../core/solvers/utils/metric.md#MetricValue), [`info`](../../core/solvers/utils/metric.md#MetricValue.info), [`analysis`](../../core/solvers/utils/journal.md#Node.analysis), [`current_step`](../../utils/state.md#MCTSState.current_step), [`debug_op`](../../core/solvers/operators/debug.md#debug_op), [`execute_op_plan_code`](../../core/solvers/operators/core.md#execute_op_plan_code), [`maximize`](../../core/solvers/utils/metric.md#MetricValue.maximize), [`MCTSNode`](mcts.md#MCTSNode), [`parse_json_output`](../../utils/code_parsing.md#parse_json_output), [`draft_op`](../../core/solvers/operators/draft.md#draft_op), [`operators_metrics`](../../core/solvers/utils/journal.md#Node.operators_metrics), [`WorstMetricValue`](../../core/solvers/utils/metric.md#WorstMetricValue), [`debug_depth`](../../core/solvers/utils/journal.md#Node.debug_depth)  (+30 more)
- used by: [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`Solver`](../../core/solvers/base.md#Solver), [`_materialize`](../../config_dataclasses/solver/__init__.md#_LazySolverMap._materialize)

### `MCTSNode`  ·  implements/extends Node
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py:68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L68)
- signature: `class MCTSNode(Node):`
- members:
  - `add_value(self, value: float)` — [`L87`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L87) — Add to the node's cumulative value.
  - `extra_metrics_to_log(self)` — [`L100`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L100)
  - `increment_explore_count(self)` — [`L97`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L97)
  - `q_value(self, lower_is_better: bool = False)` — [`L72`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L72)
  - `set_value(self, value: float)` — [`L83`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L83) — Set the node's value.
  - `explore_count` — [`L69`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L69)
  - `node_value` — [`L70`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L70)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node)
- used by: [`Node`](../../core/solvers/utils/journal.md#Node), [`_expand_leaf_and_backprop`](mcts.md#MCTS._expand_leaf_and_backprop), [`debug_cycle`](mcts.md#MCTS.debug_cycle), [`_draft`](mcts.md#MCTS._draft), [`_improve`](mcts.md#MCTS._improve), [`_debug`](mcts.md#MCTS._debug), [`create_root_node`](mcts.md#MCTS.create_root_node), [`search_policy`](mcts.md#MCTS.search_policy), [`_analyze`](mcts.md#MCTS._analyze), [`_backprop_step`](mcts.md#MCTS._backprop_step), [`extra_metrics_to_log`](../../core/solvers/utils/journal.md#Node.extra_metrics_to_log)

## Functions
- `normalise_q_value(q_value: float, global_max_q_val: float, global_min_q_val: float)` — [`L44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L44)
- `uct_value(q_value: float, explore_count: int, parent_explore_count: int, uct_c: float, global_max_q_val: float, global_min_q_val: float)` — [`L51`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/mcts/mcts.py#L51)

