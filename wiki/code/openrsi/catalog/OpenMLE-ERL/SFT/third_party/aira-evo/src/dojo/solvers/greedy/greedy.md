---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.solvers.greedy.greedy`/Greedy#
symbols:
  Greedy.parse_eval_result: parse_eval_result().
  Greedy._draft: _draft().
  Greedy._improve: _improve().
  Greedy.step: step().
  Greedy._debug: _debug().
  Greedy.create_root_node: create_root_node().
  Greedy.__call__: __call__().
  Greedy.state: state.
  Greedy.search_policy: search_policy().
  Greedy.load_checkpoint: load_checkpoint().
  Greedy.journal: journal.
  Greedy._analyze: _analyze().
  Greedy.save_checkpoint: save_checkpoint().
  Greedy.memory_op: memory_op.
  Greedy.setup_operators: setup_operators().
  Greedy.debug_memory_op: debug_memory_op.
  Greedy.draft_fn: draft_fn.
  Greedy.improve_fn: improve_fn.
  Greedy.debug_fn: debug_fn.
  Greedy.update_data_preview: update_data_preview().
  Greedy.lower_is_better: lower_is_better.
  Greedy.task_desc: task_desc.
  Greedy.data_preview: data_preview.
  Greedy.analyze_fn: analyze_fn.
  Greedy: ''
  Greedy.__init__: __init__().
  Greedy.root_node: root_node.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py)

## Classes
### `Greedy`  ·  implements/extends Solver
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py:52`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L52)
- doc: Greedy solver.
- signature: `class Greedy(Solver):`
- members:
  - `__call__(self, task, state)` — [`L144`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L144) — Run the Greedy solver for a specified number of iterations.
  - `__init__(self, cfg: GreedySolverConfig, task_info)` — [`L55`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L55) — Initialize the Greedy solver.
  - `_analyze(self, node: Node)` — [`L337`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L337) — Analyze a node's execution results using the analyze LLM operator.
  - `_debug(self, parent_node: Node)` — [`L306`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L306) — Debug a buggy solution using the debug LLM operator.
  - `_draft(self)` — [`L242`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L242) — Generate a new solution from scratch using the draft LLM operator.
  - `_improve(self, parent_node: Node)` — [`L272`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L272) — Improve an existing solution using the improve LLM operator.
  - `create_root_node(self)` — [`L127`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L127)
  - `load_checkpoint(self)` — [`L87`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L87)
  - `parse_eval_result(self, node: Node, eval_result: Dict[str, Any])` — [`L455`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L455) — Parse evaluation results and update the node accordingly.
  - `save_checkpoint(self)` — [`L76`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L76)
  - `search_policy(self)` — [`L197`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L197) — Determine the next node to work on based on the current state of the journal.
  - `setup_operators(self)` — [`L103`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L103) — Initialize and configure the LLM operators used in the Greedy solver.
  - `step(self, task, state)` — [`L384`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L384) — Execute a single iteration of the Greedy solver process.
  - `update_data_preview(self, state)` — [`L357`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L357) — Generate a data preview to provide context for the LLM operators.
  - `analyze_fn` — [`L125`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L125)
  - `data_preview` — [`L65`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L65)
  - `debug_fn` — [`L124`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L124)
  - `debug_memory_op` — [`L119`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L119)
  - `draft_fn` — [`L122`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L122)
  - `improve_fn` — [`L123`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L123)
  - `journal` — [`L64`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L64)
  - `lower_is_better` — [`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L68)
  - `memory_op` — [`L118`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L118)
  - `root_node` — [`L128`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L128)
  - `state` — [`L74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L74)
  - `task_desc` — [`L67`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/greedy/greedy.py#L67)
- uses (calls/refs, reference-scoped): [`logger`](../../core/solvers/base.md#Solver.logger), [`cfg`](../../core/solvers/base.md#Solver.cfg), [`Node`](../../core/solvers/utils/journal.md#Node), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`from_export_data`](../../core/solvers/utils/journal.md#Journal.from_export_data), [`get_node_data`](../../core/solvers/utils/journal.md#Journal.get_node_data), [`id`](../../core/solvers/utils/journal.md#Node.id), [`parents`](../../core/solvers/utils/journal.md#Node.parents), [`code`](../../core/solvers/utils/journal.md#Node.code), [`Journal`](../../core/solvers/utils/journal.md#Journal), [`nodes`](../../core/solvers/utils/journal.md#Journal.nodes), [`is_buggy`](../../core/solvers/utils/journal.md#Node.is_buggy), [`export_search_results`](../../core/solvers/utils/search_exporter.md#export_search_results), [`plan`](../../core/solvers/utils/journal.md#Node.plan), [`GenericLLM`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM), [`current_step`](../../utils/state.md#GreedyState.current_step), [`create_memory_op`](../../core/solvers/operators/memory.md#create_memory_op), [`absorb_exec_result`](../../core/solvers/utils/journal.md#Node.absorb_exec_result), [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`append`](../../core/solvers/utils/journal.md#Journal.append), [`step`](../../core/solvers/utils/journal.md#Node.step), [`generate`](../../core/solvers/utils/data_preview.md#generate), [`get_complextiy_level`](../utils.md#get_complextiy_level), [`analyze_op`](../../core/solvers/operators/analyze.md#analyze_op), [`get_best_node`](../../core/solvers/utils/journal.md#Journal.get_best_node), [`improve_op`](../../core/solvers/operators/improve.md#improve_op), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`MetricValue`](../../core/solvers/utils/metric.md#MetricValue), [`info`](../../core/solvers/utils/metric.md#MetricValue.info), [`analysis`](../../core/solvers/utils/journal.md#Node.analysis), [`debug_op`](../../core/solvers/operators/debug.md#debug_op), [`execute_op_plan_code`](../../core/solvers/operators/core.md#execute_op_plan_code), [`maximize`](../../core/solvers/utils/metric.md#MetricValue.maximize), [`parse_json_output`](../../utils/code_parsing.md#parse_json_output), [`draft_op`](../../core/solvers/operators/draft.md#draft_op), [`operators_metrics`](../../core/solvers/utils/journal.md#Node.operators_metrics), [`WorstMetricValue`](../../core/solvers/utils/metric.md#WorstMetricValue), [`debug_depth`](../../core/solvers/utils/journal.md#Node.debug_depth), [`operators`](../../config_dataclasses/solver/base.md#SolverConfig.operators), [`extract_code`](../../core/solvers/utils/response.md#extract_code)  (+28 more)
- used by: [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`Solver`](../../core/solvers/base.md#Solver), [`_materialize`](../../config_dataclasses/solver/__init__.md#_LazySolverMap._materialize)

