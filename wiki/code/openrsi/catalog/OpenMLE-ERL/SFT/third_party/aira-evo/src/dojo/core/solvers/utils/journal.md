---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.journal`/
symbols:
  Node: Node#
  Node.metric: Node#metric.
  Journal.from_export_data: Journal#from_export_data().
  Journal.get_node_data: Journal#get_node_data().
  Node.id: Node#id.
  Node.parents: Node#parents.
  Node.code: Node#code.
  Journal: Journal#
  Journal.nodes: Journal#nodes.
  Node.is_buggy: Node#is_buggy.
  Node.children: Node#children.
  Node.plan: Node#plan.
  Node.absorb_exec_result: Node#absorb_exec_result().
  Journal.generate_summary: Journal#generate_summary().
  Node.step: Node#step.
  Journal.append: Journal#append().
  Journal.is_root_node: Journal#is_root_node().
  Journal.get_best_node: Journal#get_best_node().
  Node.analysis: Node#analysis.
  Node.operators_metrics: Node#operators_metrics.
  Node.debug_depth: Node#debug_depth().
  Node.operators_used: Node#operators_used.
  Node.term_out: Node#term_out().
  Node.exec_time: Node#exec_time.
  Journal.draft_nodes: Journal#draft_nodes().
  Journal.good_nodes: Journal#good_nodes().
  Node._term_out: Node#_term_out.
  Node.stage_name: Node#stage_name().
  Journal.buggy_nodes: Journal#buggy_nodes().
  Journal.export_data: Journal#export_data().
  InteractiveSession.append: InteractiveSession#append().
  Node.exit_code: Node#exit_code.
  Node.is_leaf: Node#is_leaf().
  Journal.node_list: Journal#node_list().
  Journal.get_metric_history: Journal#get_metric_history().
  Node.ctime: Node#ctime.
  Node.attach_to_parents: Node#attach_to_parents().
  Node.remove_child: Node#remove_child().
  Node.__eq__: Node#__eq__().
  Node.__gt__: Node#__gt__().
  Journal.__getitem__: Journal#__getitem__().
  InteractiveSession.nodes: InteractiveSession#nodes.
  Node.__post_init__: Node#__post_init__().
  Node.__hash__: Node#__hash__().
  Node.extra_metrics_to_log: Node#extra_metrics_to_log().
  Journal.__len__: Journal#__len__().
  log: log.
  InteractiveSession: InteractiveSession#
  InteractiveSession.completed: InteractiveSession#completed.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py)

## Classes
### `InteractiveSession`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py:153`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L153)
- doc: A collection of nodes for an interactive search session.
- signature: `class InteractiveSession(DataClassJsonMixin):`
- members:
  - `append(self, node: Node)` — [`L159`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L159)
  - `completed` — [`L157`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L157)
  - `nodes` — [`L156`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L156)
- uses (calls/refs, reference-scoped): [`Node`](journal.md#Node), [`step`](journal.md#Node.step), [`attach_to_parents`](journal.md#Node.attach_to_parents)

### `Journal`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py:166`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L166)
- doc: A collection of nodes representing the solution tree.
- signature: `class Journal(DataClassJsonMixin):`
- members:
  - `__len__(self)` — [`L174`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L174) — Return the number of nodes in the journal.
  - `append(self, node: Node)` — [`L178`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L178) — Append a new node to the journal.
  - `buggy_nodes(self)` — [`L204`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L204) — Return a list of nodes that are considered buggy by the agent.
  - `draft_nodes(self)` — [`L194`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L194) — Return a list of nodes representing intial coding drafts
  - `export_data(self)` — [`L312`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L312) — Gather data into a dictionary structure.
  - `from_export_data(cls, export_data: dict)` — [`L334`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L334) — Reconstruct a Journal object from exported search data.
  - `generate_summary(self, include_code: bool = False, include_buggy_nodes: bool = False, only_plans: bool = False)` — [`L234`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L234) — Generate a summary of the journal for the agent.
  - `get_best_node(self, only_good: bool = True)` — [`L217`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L217) — Return the node with the best validation metric, or ``None`` if none exist.
  - `get_metric_history(self)` — [`L213`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L213) — Return a list of all metric values in the journal.
  - `get_node_data(self, idx: int)` — [`L256`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L256)
  - `good_nodes(self)` — [`L209`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L209) — Return a list of nodes that are not considered buggy by the agent.
  - `is_root_node(self, node: Node)` — [`L185`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L185) — Check if the node is a root node (no parents).
  - `node_list(self)` — [`L422`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L422) — Gather data into a dictionary structure.
  - `nodes` — [`L169`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L169)
- protocol/private: `__getitem__`[`L171`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L171)
- uses (calls/refs, reference-scoped): [`Node`](journal.md#Node), [`metric`](journal.md#Node.metric), [`id`](journal.md#Node.id), [`value`](metric.md#MetricValue.value), [`parents`](journal.md#Node.parents), [`code`](journal.md#Node.code), [`is_buggy`](journal.md#Node.is_buggy), [`children`](journal.md#Node.children), [`plan`](journal.md#Node.plan), [`step`](journal.md#Node.step), [`MetricValue`](metric.md#MetricValue), [`info`](metric.md#MetricValue.info), [`analysis`](journal.md#Node.analysis), [`maximize`](metric.md#MetricValue.maximize), [`operators_metrics`](journal.md#Node.operators_metrics), [`WorstMetricValue`](metric.md#WorstMetricValue), [`operators_used`](journal.md#Node.operators_used), [`term_out`](journal.md#Node.term_out), [`exec_time`](journal.md#Node.exec_time), [`_term_out`](journal.md#Node._term_out), [`exit_code`](journal.md#Node.exit_code), [`attach_to_parents`](journal.md#Node.attach_to_parents), [`ctime`](journal.md#Node.ctime), [`log`](journal.md#log)
- used by: [`search`](../../../solvers/evo/evo.md#Evolutionary.search), [`test_export_and_reconstruct_search_data`](search_exporter.md#test_export_and_reconstruct_search_data), [`_draft`](../../../solvers/greedy/greedy.md#Greedy._draft), [`_expand_leaf_and_backprop`](../../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`step`](../../../solvers/greedy/greedy.md#Greedy.step), [`debug_cycle`](../../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`create_root_node`](../../../solvers/greedy/greedy.md#Greedy.create_root_node), [`cfg_to_tree_struct`](tree_export.md#cfg_to_tree_struct), [`create_root_node`](../../../solvers/evo/evo.md#Evolutionary.create_root_node), [`calculate_tree_statistics`](../../../analysis_utils/meta_tree_analysis.md#calculate_tree_statistics), [`__call__`](../../../solvers/greedy/greedy.md#Greedy.__call__), [`__call__`](../../../solvers/mcts/mcts.md#MCTS.__call__), [`_build_solution_database_from_journal`](../../../solvers/evo/evo.md#Evolutionary._build_solution_database_from_journal), [`export_search_results`](search_exporter.md#export_search_results), [`write_tree_reports`](../../../analysis_utils/meta_tree_analysis.md#write_tree_reports), [`__call__`](../../../solvers/evo/evo.md#Evolutionary.__call__), [`create_root_node`](../../../solvers/mcts/mcts.md#MCTS.create_root_node), [`create_memory_op`](../operators/memory.md#create_memory_op), [`search_policy`](../../../solvers/greedy/greedy.md#Greedy.search_policy), [`step`](../../../solvers/mcts/mcts.md#MCTS.step), [`improve_op`](../operators/improve.md#improve_op), [`load_checkpoint`](../../../solvers/evo/evo.md#Evolutionary.load_checkpoint), [`load_checkpoint`](../../../solvers/greedy/greedy.md#Greedy.load_checkpoint), [`load_checkpoint`](../../../solvers/mcts/mcts.md#MCTS.load_checkpoint), [`journal`](../../../solvers/evo/evo.md#Evolutionary.journal), [`journal`](../../../solvers/greedy/greedy.md#Greedy.journal), [`debug_op`](../operators/debug.md#debug_op), [`log_journal`](../../../solvers/evo/evo.md#Evolutionary.log_journal), [`log_journal`](../../../solvers/mcts/mcts.md#MCTS.log_journal), [`crossover_op`](../operators/crossover.md#crossover_op), [`draft_op`](../operators/draft.md#draft_op), [`generate_journal_summary`](../operators/memory.md#generate_journal_summary), [`save_checkpoint`](../../../solvers/evo/evo.md#Evolutionary.save_checkpoint), [`save_checkpoint`](../../../solvers/greedy/greedy.md#Greedy.save_checkpoint), [`save_checkpoint`](../../../solvers/mcts/mcts.md#MCTS.save_checkpoint), [`journal`](../../../solvers/mcts/mcts.md#MCTS.journal), [`gather_and_export_search_results`](search_exporter.md#SearchExporter.gather_and_export_search_results), [`generate_journal_report`](../../../analysis_utils/meta_tree_analysis.md#generate_journal_report), [`generate`](tree_export.md#generate), [`journal_into_tree`](../../../analysis_utils/journal_to_tree.md#journal_into_tree)  (+8 more)

### `Node`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py:41`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L41)
- doc: A single node in the solution tree. Contains code, execution results, and evaluation information.
- signature: `class Node(DataClassJsonMixin):`
- members:
  - `absorb_exec_result(self, exec_result: ExecutionResult)` — [`L103`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L103) — Absorb the result of executing the code from this node.
  - `attach_to_parents(self)` — [`L80`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L80)
  - `debug_depth(self)` — [`L133`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L133) — Length of the current debug path
  - `extra_metrics_to_log(self)` — [`L148`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L148)
  - `is_leaf(self)` — [`L119`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L119) — Check if the node is a leaf node in the solution tree.
  - `remove_child(self, child: Node)` — [`L87`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L87)
  - `stage_name(self)` — [`L92`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L92) — Return the stage of the node:
  - `term_out(self)` — [`L112`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L112) — Get the terminal output of the code execution (after truncating it).
  - `analysis` — [`L66`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L66)
  - `children` — [`L53`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L53)
  - `code` — [`L45`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L45)
  - `ctime` — [`L51`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L51)
  - `exec_time` — [`L61`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L61)
  - `exit_code` — [`L62`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L62)
  - `id` — [`L50`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L50)
  - `is_buggy` — [`L70`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L70)
  - `metric` — [`L67`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L67)
  - `operators_metrics` — [`L57`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L57)
  - `operators_used` — [`L56`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L56)
  - `parents` — [`L52`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L52)
  - `plan` — [`L46`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L46)
  - `step` — [`L49`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L49)
- protocol/private: `__eq__`[`L123`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L123), `__gt__`[`L126`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L126), `__hash__`[`L129`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L129), `__post_init__`[`L72`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L72), `_term_out`[`L60`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L60)
- uses (calls/refs, reference-scoped): [`MetricValue`](metric.md#MetricValue), [`MCTSNode`](../../../solvers/mcts/mcts.md#MCTSNode), [`get_empty`](../../interpreters/base.md#ExecutionResult.get_empty), [`ExecutionResult`](../../interpreters/base.md#ExecutionResult), [`exec_time`](../../interpreters/base.md#ExecutionResult.exec_time), [`exit_code`](../../interpreters/base.md#ExecutionResult.exit_code), [`term_out`](../../interpreters/base.md#ExecutionResult.term_out), [`extra_metrics_to_log`](../../../solvers/mcts/mcts.md#MCTSNode.extra_metrics_to_log), [`trim_long_string`](response.md#trim_long_string)
- used by: [`search`](../../../solvers/evo/evo.md#Evolutionary.search), [`test_export_and_reconstruct_search_data`](search_exporter.md#test_export_and_reconstruct_search_data), [`from_export_data`](journal.md#Journal.from_export_data), [`get_node_data`](journal.md#Journal.get_node_data), [`parse_eval_result`](../../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`_draft`](../../../solvers/greedy/greedy.md#Greedy._draft), [`_expand_leaf_and_backprop`](../../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`_draft`](../../../solvers/evo/evo.md#Evolutionary._draft), [`_improve`](../../../solvers/evo/evo.md#Evolutionary._improve), [`_improve`](../../../solvers/greedy/greedy.md#Greedy._improve), [`step`](../../../solvers/greedy/greedy.md#Greedy.step), [`_crossover`](../../../solvers/evo/evo.md#Evolutionary._crossover), [`_debug`](../../../solvers/evo/evo.md#Evolutionary._debug), [`_debug`](../../../solvers/greedy/greedy.md#Greedy._debug), [`add_nodes_to_islands`](../../../solvers/evo/evo.md#SolutionsDatabase.add_nodes_to_islands), [`debug_cycle`](../../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`create_root_node`](../../../solvers/greedy/greedy.md#Greedy.create_root_node), [`cfg_to_tree_struct`](tree_export.md#cfg_to_tree_struct), [`create_root_node`](../../../solvers/evo/evo.md#Evolutionary.create_root_node), [`sample_in_context`](../../../solvers/evo/evo.md#SolutionsDatabase.sample_in_context), [`nodes`](journal.md#Journal.nodes), [`calculate_tree_statistics`](../../../analysis_utils/meta_tree_analysis.md#calculate_tree_statistics), [`debug_cycle`](../../../solvers/evo/evo.md#Evolutionary.debug_cycle), [`__call__`](../../../solvers/greedy/greedy.md#Greedy.__call__), [`__call__`](../../../solvers/mcts/mcts.md#MCTS.__call__), [`_build_solution_database_from_journal`](../../../solvers/evo/evo.md#Evolutionary._build_solution_database_from_journal), [`__call__`](../../../solvers/evo/evo.md#Evolutionary.__call__), [`create_root_node`](../../../solvers/mcts/mcts.md#MCTS.create_root_node), [`register_node_in_island`](../../../solvers/evo/evo.md#Island.register_node_in_island), [`create_memory_op`](../operators/memory.md#create_memory_op), [`generate_summary`](journal.md#Journal.generate_summary), [`search_policy`](../../../solvers/greedy/greedy.md#Greedy.search_policy), [`append`](journal.md#Journal.append), [`only_keep_best`](../../../solvers/evo/evo.md#Island.only_keep_best), [`get_complextiy_level`](../../../solvers/utils.md#get_complextiy_level), [`is_root_node`](journal.md#Journal.is_root_node), [`analyze_op`](../operators/analyze.md#analyze_op), [`get_best_node`](journal.md#Journal.get_best_node)  (+39 more)

## Module values
- `log` — [`L36`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/journal.py#L36)

