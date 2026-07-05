---
title: 'Module: ai_scientist/treesearch/journal.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/journal.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.journal`/
symbols:
  Node.to_dict: Node#to_dict().
  Node: Node#
  Node.metric: Node#metric.
  Node.id: Node#id.
  Node.parent: Node#parent.
  Journal.get_best_node: Journal#get_best_node().
  Node.from_dict: Node#from_dict().
  Journal.nodes: Journal#nodes.
  Journal: Journal#
  Node.absorb_exec_result: Node#absorb_exec_result().
  Journal.generate_summary: Journal#generate_summary().
  Node.absorb_plot_exec_result: Node#absorb_plot_exec_result().
  Journal.good_nodes: Journal#good_nodes().
  Node.code: Node#code.
  Node.is_buggy: Node#is_buggy.
  Node.children: Node#children.
  Journal.generate_summary_old: Journal#generate_summary_old().
  Node.plan: Node#plan.
  Node.plot_paths: Node#plot_paths.
  Journal.save_experiment_notes: Journal#save_experiment_notes().
  Node.plot_code: Node#plot_code.
  Node.analysis: Node#analysis.
  Journal.append: Journal#append().
  Journal.draft_nodes: Journal#draft_nodes().
  Journal.buggy_nodes: Journal#buggy_nodes().
  node_selection_spec: node_selection_spec.
  Node.debug_depth: Node#debug_depth().
  Node.step: Node#step.
  Node.vlm_feedback_summary: Node#vlm_feedback_summary.
  InteractiveSession.generate_nb_trace: InteractiveSession#generate_nb_trace().
  Journal.get_node_by_id: Journal#get_node_by_id().
  Node.term_out: Node#term_out().
  InteractiveSession.nodes: InteractiveSession#nodes.
  InteractiveSession.append: InteractiveSession#append().
  Journal.get_metric_history: Journal#get_metric_history().
  Node.exp_results_dir: Node#exp_results_dir.
  Node.plot_analyses: Node#plot_analyses.
  Node._term_out: Node#_term_out.
  Node.parse_metrics_plan: Node#parse_metrics_plan.
  Node.exec_time_feedback: Node#exec_time_feedback.
  Node.ablation_name: Node#ablation_name.
  Node.hyperparam_name: Node#hyperparam_name.
  Node.__post_init__: Node#__post_init__().
  Node.stage_name: Node#stage_name().
  logger: logger.
  Node.exc_type: Node#exc_type.
  Node.parse_metrics_code: Node#parse_metrics_code.
  Node.parse_term_out: Node#parse_term_out.
  Node.is_buggy_plots: Node#is_buggy_plots.
  Node.plots: Node#plots.
  Node.is_seed_node: Node#is_seed_node.
  Node.__deepcopy__: Node#__deepcopy__().
  Node.__eq__: Node#__eq__().
  Journal.__getitem__: Journal#__getitem__().
  Journal.to_dict: Journal#to_dict().
  Node.is_leaf: Node#is_leaf().
  Node.exec_time: Node#exec_time.
  Node.parse_exc_type: Node#parse_exc_type.
  Node.parse_exc_info: Node#parse_exc_info.
  Node.parse_exc_stack: Node#parse_exc_stack.
  Node.datasets_successfully_tested: Node#datasets_successfully_tested.
  Node.plot_plan: Node#plot_plan.
  Node.exc_info: Node#exc_info.
  Node.exc_stack: Node#exc_stack.
  Node.plot_exc_type: Node#plot_exc_type.
  Node.is_seed_agg_node: Node#is_seed_agg_node.
  Node.__getstate__: Node#__getstate__().
  Node.__hash__: Node#__hash__().
  Journal.__len__: Journal#__len__().
  Node.plot_term_out: Node#plot_term_out.
  Node.overall_plan: Node#overall_plan.
  Node.ctime: Node#ctime.
  Node.plot_exec_time: Node#plot_exec_time.
  Node.plot_exc_info: Node#plot_exc_info.
  Node.plot_exc_stack: Node#plot_exc_stack.
  Node.plot_data: Node#plot_data.
  Node.plots_generated: Node#plots_generated.
  Node.__setstate__: Node#__setstate__().
  InteractiveSession: InteractiveSession#
  InteractiveSession.completed: InteractiveSession#completed.
---
# Module: [`ai_scientist/treesearch/journal.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py)

## Classes
### `InteractiveSession`
- def: [`ai_scientist/treesearch/journal.py:332`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L332)
- doc: A collection of nodes for an interaction session
- signature: `class InteractiveSession(DataClassJsonMixin):`
- members:
  - `append(self, node: Node)` — [`L341`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L341) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `generate_nb_trace(self, include_prompt, comment_headers=True)` — [`L345`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L345) — Generate a trace of the interactive session in IPython format.
  - `completed` — [`L339`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L339)
  - `nodes` — [`L338`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L338)
- uses (calls/refs, reference-scoped): [`Node`](journal.md#Node), [`code`](journal.md#Node.code), [`step`](journal.md#Node.step), [`term_out`](journal.md#Node.term_out)

### `Journal`
- def: [`ai_scientist/treesearch/journal.py:362`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L362) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
- members:
  - `__len__(self)` — [`L370`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L370) — Return the number of nodes in the journal.
  - `append(self, node: Node)` — [`L374`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L374) — Append a new node to the journal. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `buggy_nodes(self)` — [`L385`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L385) — Return a list of nodes that are considered buggy by the agent. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `draft_nodes(self)` — [`L380`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L380) — Return a list of nodes representing intial coding drafts — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `generate_summary(self, include_code: bool = False, **model_kwargs)` — [`L504`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L504) — Generate a summary of the research progress using LLM, including both successes and failures. — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `generate_summary_old(self, include_code: bool = False)` — [`L550`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L550)
  - `get_best_node(self, only_good=True, use_val_metric_only=False, cfg=None)` — [`L420`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L420) — Return the best solution found so far. — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `get_metric_history(self)` — [`L416`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L416) — Return a list of all metric values in the journal. — documented in [ai_scientist-treesearch-utils-metric](../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `get_node_by_id(self, node_id: str)` — [`L409`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L409) — Get a node by its ID. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `good_nodes(self)` — [`L390`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L390) — Return a list of nodes that are not considered buggy by the agent. — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `save_experiment_notes(self, workspace_dir: str, stage_name: str, cfg: Any)` — [`L565`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L565) — Save experimental notes and summaries to files
  - `to_dict(self)` — [`L561`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L561) — Convert journal to a JSON-serializable dictionary
  - `nodes` — [`L365`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L365) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
- protocol/private: `__getitem__`[`L367`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L367)
- uses (calls/refs, reference-scoped): [`to_dict`](journal.md#Node.to_dict), [`Node`](journal.md#Node), [`value`](utils/metric.md#MetricValue.value), [`metric`](journal.md#Node.metric), [`id`](journal.md#Node.id), [`parent`](journal.md#Node.parent), [`query`](backend/__init__.md#query), [`code`](journal.md#Node.code), [`is_buggy`](journal.md#Node.is_buggy), [`plan`](journal.md#Node.plan), [`analysis`](journal.md#Node.analysis), [`MetricValue`](utils/metric.md#MetricValue), [`node_selection_spec`](journal.md#node_selection_spec), [`debug_depth`](journal.md#Node.debug_depth), [`step`](journal.md#Node.step), [`vlm_feedback_summary`](journal.md#Node.vlm_feedback_summary), [`exc_type`](journal.md#Node.exc_type), [`is_buggy_plots`](journal.md#Node.is_buggy_plots), [`is_seed_node`](journal.md#Node.is_seed_node), [`logger`](journal.md#logger)
- used by: [`_process_node_wrapper`](parallel_agent.md#ParallelAgent._process_node_wrapper), [`cfg_to_tree_struct`](utils/tree_export.md#cfg_to_tree_struct), [`step`](parallel_agent.md#ParallelAgent.step), [`run`](agent_manager.md#AgentManager.run), [`_run_plot_aggregation`](parallel_agent.md#ParallelAgent._run_plot_aggregation), [`_run_multi_seed_evaluation`](parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`_select_parallel_nodes`](parallel_agent.md#ParallelAgent._select_parallel_nodes), [`_check_stage_completion`](agent_manager.md#AgentManager._check_stage_completion), [`_create_initial_stage`](agent_manager.md#AgentManager._create_initial_stage), [`from_dict`](journal.md#Node.from_dict), [`_create_next_main_stage`](agent_manager.md#AgentManager._create_next_main_stage), [`_create_next_substage`](agent_manager.md#AgentManager._create_next_substage), [`_gather_stage_metrics`](agent_manager.md#AgentManager._gather_stage_metrics), [`_generate_substage_goal`](agent_manager.md#AgentManager._generate_substage_goal), [`_check_substage_completion`](agent_manager.md#AgentManager._check_substage_completion), [`journals`](agent_manager.md#AgentManager.journals), [`_analyze_progress`](agent_manager.md#AgentManager._analyze_progress), [`_get_best_implementation`](agent_manager.md#AgentManager._get_best_implementation), [`_identify_issues`](agent_manager.md#AgentManager._identify_issues), [`journal2report`](journal2report.md#journal2report), [`loads_json`](utils/serialize.md#loads_json), [`reconstruct_journal`](log_summarization.md#reconstruct_journal), [`generate`](utils/tree_export.md#generate), [`journal_to_rich_tree`](perform_experiments_bfts_with_agentmanager.md#journal_to_rich_tree), [`dumps_json`](utils/serialize.md#dumps_json), [`get_edges`](utils/tree_export.md#get_edges), [`__init__`](parallel_agent.md#ParallelAgent.__init__)

### `Node`
- def: [`ai_scientist/treesearch/journal.py:44`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L44) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
- doc: A single node in the solution tree. Contains code, execution results, and evaluation information.
- signature: `class Node(DataClassJsonMixin):`
- members:
  - `__getstate__(self)` — [`L145`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L145) — Return state for pickling
  - `__setstate__(self, state)` — [`L153`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L153) — Set state during unpickling
  - `absorb_exec_result(self, exec_result: ExecutionResult)` — [`L170`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L170) — Absorb the result of executing the code from this node. — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `absorb_plot_exec_result(self, plot_exec_result: ExecutionResult)` — [`L178`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L178) — Absorb the result of executing the plotting code from this node.
  - `debug_depth(self)` — [`L203`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L203) — Length of the current debug path
  - `from_dict(cls, data: Dict, journal: Optional[Journal] = None)` — [`L294`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L294) — Create a Node from a dictionary, optionally linking to journal for relationships — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `is_leaf(self)` — [`L192`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L192) — Check if the node is a leaf node in the solution tree.
  - `stage_name(self)` — [`L159`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L159) — Return the stage of the node:
  - `term_out(self)` — [`L187`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L187) — Get the terminal output of the code execution (after truncating it).
  - `to_dict(self)` — [`L214`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L214) — Convert node to dictionary for serialization — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `ablation_name` — [`L111`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L111)
  - `analysis` — [`L87`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L87) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `children` — [`L59`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L59) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `code` — [`L50`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L50) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `ctime` — [`L57`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L57)
  - `datasets_successfully_tested` — [`L105`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L105)
  - `exc_info` — [`L66`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L66)
  - `exc_stack` — [`L67`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L67)
  - `exc_type` — [`L65`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L65)
  - `exec_time` — [`L64`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L64)
  - `exec_time_feedback` — [`L108`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L108)
  - `exp_results_dir` — [`L60`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L60)
  - `hyperparam_name` — [`L114`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L114)
  - `id` — [`L56`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L56) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `is_buggy` — [`L91`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L91) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `is_buggy_plots` — [`L92`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L92)
  - `is_seed_agg_node` — [`L118`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L118)
  - `is_seed_node` — [`L117`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L117)
  - `metric` — [`L88`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L88) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `overall_plan` — [`L49`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L49)
  - `parent` — [`L58`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L58) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `parse_exc_info` — [`L75`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L75)
  - `parse_exc_stack` — [`L76`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L76)
  - `parse_exc_type` — [`L74`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L74)
  - `parse_metrics_code` — [`L71`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L71)
  - `parse_metrics_plan` — [`L70`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L70)
  - `parse_term_out` — [`L73`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L73)
  - `plan` — [`L48`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L48) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `plot_analyses` — [`L103`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L103)
  - `plot_code` — [`L51`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L51) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `plot_data` — [`L95`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L95)
  - `plot_exc_info` — [`L82`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L82)
  - `plot_exc_stack` — [`L83`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L83)
  - `plot_exc_type` — [`L81`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L81)
  - `plot_exec_time` — [`L80`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L80)
  - `plot_paths` — [`L98`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L98) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `plot_plan` — [`L52`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L52)
  - `plot_term_out` — [`L79`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L79)
  - `plots` — [`L97`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L97)
  - `plots_generated` — [`L96`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L96)
  - `step` — [`L55`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L55) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `vlm_feedback_summary` — [`L104`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L104) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
- protocol/private: `__deepcopy__`[`L128`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L128), `__eq__`[`L196`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L196), `__hash__`[`L199`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L199), `__post_init__`[`L120`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L120), `_term_out`[`L63`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L63)
- uses (calls/refs, reference-scoped): [`value`](utils/metric.md#MetricValue.value), [`Journal`](journal.md#Journal), [`MetricValue`](utils/metric.md#MetricValue), [`WorstMetricValue`](utils/metric.md#WorstMetricValue), [`get_node_by_id`](journal.md#Journal.get_node_by_id), [`maximize`](utils/metric.md#MetricValue.maximize), [`ExecutionResult`](interpreter.md#ExecutionResult), [`name`](utils/metric.md#MetricValue.name), [`term_out`](interpreter.md#ExecutionResult.term_out), [`exc_info`](interpreter.md#ExecutionResult.exc_info), [`exc_type`](interpreter.md#ExecutionResult.exc_type), [`description`](utils/metric.md#MetricValue.description), [`exc_stack`](interpreter.md#ExecutionResult.exc_stack), [`exec_time`](interpreter.md#ExecutionResult.exec_time), [`trim_long_string`](utils/response.md#trim_long_string)
- used by: [`_process_node_wrapper`](parallel_agent.md#ParallelAgent._process_node_wrapper), [`cfg_to_tree_struct`](utils/tree_export.md#cfg_to_tree_struct), [`step`](parallel_agent.md#ParallelAgent.step), [`_run_plot_aggregation`](parallel_agent.md#ParallelAgent._run_plot_aggregation), [`_run_multi_seed_evaluation`](parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`_select_parallel_nodes`](parallel_agent.md#ParallelAgent._select_parallel_nodes), [`_check_stage_completion`](agent_manager.md#AgentManager._check_stage_completion), [`get_best_node`](journal.md#Journal.get_best_node), [`parse_exec_result`](parallel_agent.md#MinimalAgent.parse_exec_result), [`_analyze_plots_with_vlm`](parallel_agent.md#MinimalAgent._analyze_plots_with_vlm), [`_debug`](parallel_agent.md#MinimalAgent._debug), [`nodes`](journal.md#Journal.nodes), [`_draft`](parallel_agent.md#MinimalAgent._draft), [`_improve`](parallel_agent.md#MinimalAgent._improve), [`_generate_node_summary`](parallel_agent.md#MinimalAgent._generate_node_summary), [`_gather_stage_metrics`](agent_manager.md#AgentManager._gather_stage_metrics), [`_generate_ablation_node`](parallel_agent.md#MinimalAgent._generate_ablation_node), [`_generate_hyperparam_tuning_node`](parallel_agent.md#MinimalAgent._generate_hyperparam_tuning_node), [`generate_summary`](journal.md#Journal.generate_summary), [`good_nodes`](journal.md#Journal.good_nodes), [`_analyze_progress`](agent_manager.md#AgentManager._analyze_progress), [`_determine_datasets_successfully_tested`](parallel_agent.md#MinimalAgent._determine_datasets_successfully_tested), [`_get_best_implementation`](agent_manager.md#AgentManager._get_best_implementation), [`_parse_vlm_feedback`](agent_manager.md#AgentManager._parse_vlm_feedback), [`_generate_plotting_code`](parallel_agent.md#MinimalAgent._generate_plotting_code), [`_generate_seed_eval_aggregation_node`](parallel_agent.md#ParallelAgent._generate_seed_eval_aggregation_node), [`_identify_issues`](agent_manager.md#AgentManager._identify_issues), [`_update_ablation_state`](parallel_agent.md#ParallelAgent._update_ablation_state), [`_update_hyperparam_tuning_state`](parallel_agent.md#ParallelAgent._update_hyperparam_tuning_state), [`append_rec`](perform_experiments_bfts_with_agentmanager.md#journal_to_rich_tree.append_rec), [`loads_json`](utils/serialize.md#loads_json), [`generate_summary_old`](journal.md#Journal.generate_summary_old), [`_generate_seed_node`](parallel_agent.md#MinimalAgent._generate_seed_node), [`reconstruct_journal`](log_summarization.md#reconstruct_journal), [`save_experiment_notes`](journal.md#Journal.save_experiment_notes), [`append`](journal.md#Journal.append), [`buggy_nodes`](journal.md#Journal.buggy_nodes), [`draft_nodes`](journal.md#Journal.draft_nodes), [`_aggregate_seed_eval_results`](parallel_agent.md#ParallelAgent._aggregate_seed_eval_results), [`generate_nb_trace`](journal.md#InteractiveSession.generate_nb_trace)  (+10 more)

## Module values
- `logger` — [`L21`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L21)
- `node_selection_spec` — [`L23`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/journal.py#L23) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)

