---
title: 'Module: ai_scientist/treesearch/parallel_agent.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/parallel_agent.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.parallel_agent`/
symbols:
  ParallelAgent._process_node_wrapper: ParallelAgent#_process_node_wrapper().
  ParallelAgent.step: ParallelAgent#step().
  ParallelAgent._run_plot_aggregation: ParallelAgent#_run_plot_aggregation().
  ParallelAgent._run_multi_seed_evaluation: ParallelAgent#_run_multi_seed_evaluation().
  ParallelAgent._select_parallel_nodes: ParallelAgent#_select_parallel_nodes().
  logger: logger.
  MinimalAgent.parse_exec_result: MinimalAgent#parse_exec_result().
  MinimalAgent._debug: MinimalAgent#_debug().
  MinimalAgent._analyze_plots_with_vlm: MinimalAgent#_analyze_plots_with_vlm().
  MinimalAgent._draft: MinimalAgent#_draft().
  MinimalAgent._improve: MinimalAgent#_improve().
  ParallelAgent._generate_hyperparam_tuning_idea: ParallelAgent#_generate_hyperparam_tuning_idea().
  ParallelAgent._generate_ablation_idea: ParallelAgent#_generate_ablation_idea().
  MinimalAgent._generate_node_summary: MinimalAgent#_generate_node_summary().
  MinimalAgent._generate_hyperparam_tuning_node: MinimalAgent#_generate_hyperparam_tuning_node().
  MinimalAgent._generate_ablation_node: MinimalAgent#_generate_ablation_node().
  ParallelAgent.cfg: ParallelAgent#cfg.
  MinimalAgent._determine_datasets_successfully_tested: MinimalAgent#_determine_datasets_successfully_tested().
  ParallelAgent.plan_and_code_query: ParallelAgent#plan_and_code_query().
  MinimalAgent.cfg: MinimalAgent#cfg.
  ParallelAgent.gpu_manager: ParallelAgent#gpu_manager.
  MinimalAgent._generate_plotting_code: MinimalAgent#_generate_plotting_code().
  ParallelAgent._define_global_metrics: ParallelAgent#_define_global_metrics().
  ParallelAgent._generate_seed_eval_aggregation_node: ParallelAgent#_generate_seed_eval_aggregation_node().
  ParallelAgent._update_hyperparam_tuning_state: ParallelAgent#_update_hyperparam_tuning_state().
  ParallelAgent._update_ablation_state: ParallelAgent#_update_ablation_state().
  MinimalAgent.plan_and_code_query: MinimalAgent#plan_and_code_query().
  ParallelAgent.journal: ParallelAgent#journal.
  ParallelAgent.stage_name: ParallelAgent#stage_name.
  MinimalAgent._generate_seed_node: MinimalAgent#_generate_seed_node().
  ParallelAgent.cleanup: ParallelAgent#cleanup().
  ParallelAgent.num_gpus: ParallelAgent#num_gpus.
  review_func_spec: review_func_spec.
  vlm_feedback_spec: vlm_feedback_spec.
  metric_parse_spec: metric_parse_spec.
  plot_selection_spec: plot_selection_spec.
  ParallelAgent.num_workers: ParallelAgent#num_workers.
  ParallelAgent._aggregate_seed_eval_results: ParallelAgent#_aggregate_seed_eval_results().
  ParallelAgent.timeout: ParallelAgent#timeout.
  ParallelAgent._get_leaves: ParallelAgent#_get_leaves().
  MinimalAgent.stage_name: MinimalAgent#stage_name.
  MinimalAgent._prompt_impl_guideline: MinimalAgent#_prompt_impl_guideline().
  ParallelAgent.executor: ParallelAgent#executor.
  MinimalAgent.task_desc: MinimalAgent#task_desc.
  GPUManager.gpu_assignments: GPUManager#gpu_assignments.
  GPUManager.acquire_gpu: GPUManager#acquire_gpu().
  GPUManager.release_gpu: GPUManager#release_gpu().
  _parse_keyword_prefix_response: _parse_keyword_prefix_response().
  GPUManager.available_gpus: GPUManager#available_gpus.
  ParallelAgent.__init__: ParallelAgent#__init__().
  ParallelAgent.evaluation_metrics: ParallelAgent#evaluation_metrics.
  AblationIdea: AblationIdea#
  AblationIdea.name: AblationIdea#name.
  HyperparamTuningIdea: HyperparamTuningIdea#
  HyperparamTuningIdea.name: HyperparamTuningIdea#name.
  MinimalAgent.memory_summary: MinimalAgent#memory_summary.
  ParallelAgent.best_stage3_node: ParallelAgent#best_stage3_node.
  ParallelAgent.best_stage1_node: ParallelAgent#best_stage1_node.
  ExecCallbackType: ExecCallbackType.
  _safe_pickle_test: _safe_pickle_test().
  MinimalAgent._prompt_resp_fmt: MinimalAgent#_prompt_resp_fmt().
  ParallelAgent: ParallelAgent#
  ParallelAgent.task_desc: ParallelAgent#task_desc.
  ParallelAgent._ablation_state: ParallelAgent#_ablation_state.
  ParallelAgent._hyperparam_tuning_state: ParallelAgent#_hyperparam_tuning_state.
  AblationConfig.__init__: AblationConfig#__init__().
  ParallelAgent.__exit__: ParallelAgent#__exit__().
  MinimalAgent.evaluation_metrics: MinimalAgent#evaluation_metrics.
  MinimalAgent.data_preview: MinimalAgent#data_preview.
  ParallelAgent.best_stage2_node: ParallelAgent#best_stage2_node.
  ParallelAgent._is_shutdown: ParallelAgent#_is_shutdown.
  AblationIdea.description: AblationIdea#description.
  HyperparamTuningIdea.description: HyperparamTuningIdea#description.
  MinimalAgent: MinimalAgent#
  MinimalAgent._prompt_environment: MinimalAgent#_prompt_environment().
  MinimalAgent._prompt_metricparse_resp_fmt: MinimalAgent#_prompt_metricparse_resp_fmt().
  MinimalAgent._prompt_debug_resp_fmt: MinimalAgent#_prompt_debug_resp_fmt().
  MinimalAgent._prompt_hyperparam_tuning_resp_fmt: MinimalAgent#_prompt_hyperparam_tuning_resp_fmt().
  MinimalAgent._prompt_ablation_resp_fmt: MinimalAgent#_prompt_ablation_resp_fmt().
  MinimalAgent.encode_image_to_base64: MinimalAgent#encode_image_to_base64().
  GPUManager: GPUManager#
  get_gpu_count: get_gpu_count().
  AblationConfig: AblationConfig#
  AblationConfig.name: AblationConfig#name.
  AblationConfig.description: AblationConfig#description.
  AblationConfig.code: AblationConfig#code.
  AblationConfig.base_node: AblationConfig#base_node.
  AblationConfig.attempts: AblationConfig#attempts.
  AblationConfig.max_attempts: AblationConfig#max_attempts.
  AblationConfig.last_error: AblationConfig#last_error.
  AblationConfig.completed: AblationConfig#completed.
  AblationConfig.current_node: AblationConfig#current_node.
  AblationIdea.__init__: AblationIdea#__init__().
  HyperparamTuningIdea.__init__: HyperparamTuningIdea#__init__().
  MinimalAgent.__init__: MinimalAgent#__init__().
  GPUManager.__init__: GPUManager#__init__().
  GPUManager.num_gpus: GPUManager#num_gpus.
  ParallelAgent.data_preview: ParallelAgent#data_preview.
  ParallelAgent.__enter__: ParallelAgent#__enter__().
---
# Module: [`ai_scientist/treesearch/parallel_agent.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py)

## Classes
### `AblationConfig`
- def: [`ai_scientist/treesearch/parallel_agent.py:223`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L223)
- doc: Track state of ablation experiments
- signature: `class AblationConfig:`
- members:
  - `attempts` — [`L231`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L231)
  - `base_node` — [`L230`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L230)
  - `code` — [`L229`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L229)
  - `completed` — [`L234`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L234)
  - `current_node` — [`L235`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L235)
  - `description` — [`L228`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L228)
  - `last_error` — [`L233`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L233)
  - `max_attempts` — [`L232`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L232)
  - `name` — [`L227`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L227)
- protocol/private: `__init__`[`L226`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L226)
- uses (calls/refs, reference-scoped): [`Node`](journal.md#Node)

### `AblationIdea`
- def: [`ai_scientist/treesearch/parallel_agent.py:238`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L238)
- doc: Ablation idea
- signature: `class AblationIdea:`
- members:
  - `description` — [`L243`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L243)
  - `name` — [`L242`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L242)
- protocol/private: `__init__`[`L241`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L241)
- used by: [`step`](parallel_agent.md#ParallelAgent.step), [`_generate_ablation_idea`](parallel_agent.md#ParallelAgent._generate_ablation_idea), [`_generate_ablation_node`](parallel_agent.md#MinimalAgent._generate_ablation_node)

### `GPUManager`
- def: [`ai_scientist/treesearch/parallel_agent.py:1091`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1091)
- doc: Manages GPU allocation across processes
- signature: `class GPUManager:`
- members:
  - `acquire_gpu(self, process_id: str)` — [`L1099`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1099) — Assigns a GPU to a process
  - `release_gpu(self, process_id: str)` — [`L1112`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1112) — Releases GPU assigned to a process
  - `available_gpus` — [`L1096`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1096)
  - `gpu_assignments` — [`L1097`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1097)
  - `num_gpus` — [`L1095`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1095)
- protocol/private: `__init__`[`L1094`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1094)
- used by: [`step`](parallel_agent.md#ParallelAgent.step), [`_run_multi_seed_evaluation`](parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`gpu_manager`](parallel_agent.md#ParallelAgent.gpu_manager), [`cleanup`](parallel_agent.md#ParallelAgent.cleanup)

### `HyperparamTuningIdea`
- def: [`ai_scientist/treesearch/parallel_agent.py:246`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L246)
- doc: Hyperparameter tuning idea
- signature: `class HyperparamTuningIdea:`
- members:
  - `description` — [`L251`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L251)
  - `name` — [`L250`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L250)
- protocol/private: `__init__`[`L249`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L249)
- used by: [`step`](parallel_agent.md#ParallelAgent.step), [`_generate_hyperparam_tuning_idea`](parallel_agent.md#ParallelAgent._generate_hyperparam_tuning_idea), [`_generate_hyperparam_tuning_node`](parallel_agent.md#MinimalAgent._generate_hyperparam_tuning_node)

### `MinimalAgent`
- def: [`ai_scientist/treesearch/parallel_agent.py:254`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L254)
- doc: A minimal agent class that only contains what's needed for processing nodes
- signature: `class MinimalAgent:`
- members:
  - `_analyze_plots_with_vlm(self, node: Node)` — [`L894`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L894) — Analyze experimental plots using VLM — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_determine_datasets_successfully_tested(self, node: Node)` — [`L835`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L835) — Determine which datasets are successfully tested based on VLM feedback — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `_generate_node_summary(self, node: Node)` — [`L1035`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1035) — Generate a summary of the node's experimental findings
  - `_generate_plotting_code(self, node: Node, working_dir: str, plot_code_from_prev_stage: str = None)` — [`L720`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L720) — Generate code for plotting experiment results — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `encode_image_to_base64(image_path)` — [`L902`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L902)
  - `parse_exec_result(self, node: Node, exec_result: ExecutionResult, workspace: str)` — [`L683`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L683) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `plan_and_code_query(self, prompt, retries=3)` — [`L658`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L658) — Generate a natural language plan + code in the same LLM call and split them apart. — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `cfg` — [`L268`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L268) — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `data_preview` — [`L271`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L271)
  - `evaluation_metrics` — [`L269`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L269)
  - `memory_summary` — [`L267`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L267)
  - `stage_name` — [`L270`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L270)
  - `task_desc` — [`L266`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L266)
- protocol/private: `__init__`[`L257`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L257), `_debug`[`L494`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L494), `_draft`[`L453`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L453), `_generate_ablation_node`[`L605`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L605), `_generate_hyperparam_tuning_node`[`L557`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L557), `_generate_seed_node`[`L549`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L549), `_improve`[`L523`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L523), `_prompt_ablation_resp_fmt`[`L442`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L442), `_prompt_debug_resp_fmt`[`L418`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L418), `_prompt_environment`[`L274`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L274), `_prompt_hyperparam_tuning_resp_fmt`[`L430`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L430), `_prompt_impl_guideline`[`L298`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L298), `_prompt_metricparse_resp_fmt`[`L407`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L407), `_prompt_resp_fmt`[`L397`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L397)
- uses (calls/refs, reference-scoped): [`Node`](journal.md#Node), [`logger`](parallel_agent.md#logger), [`metric`](journal.md#Node.metric), [`id`](journal.md#Node.id), [`parent`](journal.md#Node.parent), [`query`](backend/__init__.md#query), [`absorb_exec_result`](journal.md#Node.absorb_exec_result), [`code`](journal.md#Node.code), [`is_buggy`](journal.md#Node.is_buggy), [`plan`](journal.md#Node.plan), [`plot_paths`](journal.md#Node.plot_paths), [`analysis`](journal.md#Node.analysis), [`plot_code`](journal.md#Node.plot_code), [`wrap_code`](utils/response.md#wrap_code), [`plot_selection_spec`](parallel_agent.md#plot_selection_spec), [`review_func_spec`](parallel_agent.md#review_func_spec), [`vlm_feedback_spec`](parallel_agent.md#vlm_feedback_spec), [`vlm_feedback_summary`](journal.md#Node.vlm_feedback_summary), [`term_out`](journal.md#Node.term_out), [`ExecutionResult`](interpreter.md#ExecutionResult), [`extract_code`](utils/response.md#extract_code), [`plot_analyses`](journal.md#Node.plot_analyses), [`ablation_name`](journal.md#Node.ablation_name), [`exec_time_feedback`](journal.md#Node.exec_time_feedback), [`hyperparam_name`](journal.md#Node.hyperparam_name), [`_parse_keyword_prefix_response`](parallel_agent.md#_parse_keyword_prefix_response), [`exc_type`](journal.md#Node.exc_type), [`is_buggy_plots`](journal.md#Node.is_buggy_plots), [`is_seed_node`](journal.md#Node.is_seed_node), [`AblationIdea`](parallel_agent.md#AblationIdea), [`HyperparamTuningIdea`](parallel_agent.md#HyperparamTuningIdea), [`datasets_successfully_tested`](journal.md#Node.datasets_successfully_tested), [`name`](parallel_agent.md#AblationIdea.name), [`name`](parallel_agent.md#HyperparamTuningIdea.name), [`extract_text_up_to_code`](utils/response.md#extract_text_up_to_code), [`plot_plan`](journal.md#Node.plot_plan), [`description`](parallel_agent.md#AblationIdea.description), [`description`](parallel_agent.md#HyperparamTuningIdea.description)
- used by: [`_process_node_wrapper`](parallel_agent.md#ParallelAgent._process_node_wrapper)

### `ParallelAgent`
- def: [`ai_scientist/treesearch/parallel_agent.py:1142`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1142)
- signature: `class ParallelAgent:`
- members:
  - `_aggregate_seed_eval_results(self, seed_nodes: List[Node], parent_node: Node)` — [`L2228`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2228) — Generate aggregated plots from multi-seed evaluation results. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_define_global_metrics(self)` — [`L1194`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1194) — Define eval metric to be used across all experiments
  - `_generate_ablation_idea(self)` — [`L1860`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1860) — Generate the next ablation idea based on what's been done — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `_generate_hyperparam_tuning_idea(self)` — [`L1798`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1798) — Generate the next hyperparam tuning idea based on what's been done. — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `_generate_seed_eval_aggregation_node(self, node: Node, agg_plotting_code: str)` — [`L1248`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1248) — Generate a special aggregation node for seed evaluation results — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_get_leaves(self, node: Node)` — [`L1921`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1921) — Get all leaf nodes in the subtree rooted at node. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_process_node_wrapper(node_data, task_desc, cfg, gpu_id: int = None, memory_summary: str = None, evaluation_metrics=None, stage_name=None, new_ablation_idea=None, new_hyperparam_idea=None, best_stage3_plot_code=None, best_stage2_plot_code=None, best_stage1_plot_code=None, seed_eval=False)` — [`L1410`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1410) — Wrapper function that creates a fresh environment for each process — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_run_multi_seed_evaluation(self, node: Node)` — [`L1261`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1261) — Run multiple seeds of the same node to get statistical metrics. — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_run_plot_aggregation(self, node: Node, seed_nodes: List[Node])` — [`L1332`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1332) — Generate an aggregation node for seed evaluation results — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_select_parallel_nodes(self)` — [`L1931`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1931) — Select N nodes to process in parallel, — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_update_ablation_state(self, result_node: Node)` — [`L2210`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2210) — Update ablation tracking state based on execution results. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_update_hyperparam_tuning_state(self, result_node: Node)` — [`L2192`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2192) — Update hyperparam tuning tracking state based on execution results. — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `cleanup(self)` — [`L2336`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2336) — Cleanup parallel workers and resources
  - `plan_and_code_query(self, prompt, retries=3)` — [`L1224`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1224) — Generate a natural language plan + code in the same LLM call and split them apart. — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `step(self, exec_callback: ExecCallbackType)` — [`L2053`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2053) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `best_stage1_node` — [`L1161`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1161)
  - `best_stage2_node` — [`L1164`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1164)
  - `best_stage3_node` — [`L1158`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1158)
  - `cfg` — [`L1155`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1155) — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `data_preview` — [`L1167`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1167)
  - `evaluation_metrics` — [`L1186`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1186)
  - `executor` — [`L1183`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1183)
  - `gpu_manager` — [`L1176`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1176) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `journal` — [`L1156`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1156) — documented in [ai_scientist-treesearch-parallel_agent](../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `num_gpus` — [`L1169`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1169)
  - `num_workers` — [`L1168`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1168) — documented in [ai_scientist-treesearch-utils-config](../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `stage_name` — [`L1157`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1157)
  - `task_desc` — [`L1154`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1154)
  - `timeout` — [`L1182`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1182)
- protocol/private: `__enter__`[`L2333`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2333), `__exit__`[`L2367`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L2367), `__init__`[`L1143`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1143), `_ablation_state`[`L1187`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1187), `_hyperparam_tuning_state`[`L1190`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1190), `_is_shutdown`[`L1184`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1184)
- uses (calls/refs, reference-scoped): [`to_dict`](journal.md#Node.to_dict), [`Node`](journal.md#Node), [`value`](utils/metric.md#MetricValue.value), [`logger`](parallel_agent.md#logger), [`metric`](journal.md#Node.metric), [`id`](journal.md#Node.id), [`parent`](journal.md#Node.parent), [`query`](backend/__init__.md#query), [`get_best_node`](journal.md#Journal.get_best_node), [`parse_exec_result`](parallel_agent.md#MinimalAgent.parse_exec_result), [`_analyze_plots_with_vlm`](parallel_agent.md#MinimalAgent._analyze_plots_with_vlm), [`_debug`](parallel_agent.md#MinimalAgent._debug), [`from_dict`](journal.md#Node.from_dict), [`_draft`](parallel_agent.md#MinimalAgent._draft), [`_improve`](parallel_agent.md#MinimalAgent._improve), [`Journal`](journal.md#Journal), [`_generate_ablation_node`](parallel_agent.md#MinimalAgent._generate_ablation_node), [`_generate_hyperparam_tuning_node`](parallel_agent.md#MinimalAgent._generate_hyperparam_tuning_node), [`generate_summary`](journal.md#Journal.generate_summary), [`run`](interpreter.md#Interpreter.run), [`good_nodes`](journal.md#Journal.good_nodes), [`code`](journal.md#Node.code), [`agent`](utils/config.md#Config.agent), [`_generate_plotting_code`](parallel_agent.md#MinimalAgent._generate_plotting_code), [`is_buggy`](journal.md#Node.is_buggy), [`plan_and_code_query`](parallel_agent.md#MinimalAgent.plan_and_code_query), [`children`](journal.md#Node.children), [`cleanup_session`](interpreter.md#Interpreter.cleanup_session), [`plan`](journal.md#Node.plan), [`plot_paths`](journal.md#Node.plot_paths), [`_generate_seed_node`](parallel_agent.md#MinimalAgent._generate_seed_node), [`workspace_dir`](utils/config.md#Config.workspace_dir), [`Config`](utils/config.md#Config), [`plot_code`](journal.md#Node.plot_code), [`wrap_code`](utils/response.md#wrap_code), [`MetricValue`](utils/metric.md#MetricValue), [`append`](journal.md#Journal.append), [`buggy_nodes`](journal.md#Journal.buggy_nodes), [`draft_nodes`](journal.md#Journal.draft_nodes), [`metric_parse_spec`](parallel_agent.md#metric_parse_spec)  (+55 more)
- used by: [`run`](agent_manager.md#AgentManager.run), [`_create_agent_for_stage`](agent_manager.md#AgentManager._create_agent_for_stage)

## Functions
- `_parse_keyword_prefix_response(response: str, keyword_prefix1: str, keyword_prefix2: str)` — [`L41`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L41) — Parse the response into name and description based on keyword prefix
- `_safe_pickle_test(obj, name="object")` — [`L31`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L31) — Test if an object can be pickled
- `get_gpu_count()` — [`L1120`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L1120) — Get number of available NVIDIA GPUs without using torch

## Module values
- `ExecCallbackType` — [`L28`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L28)
- `logger` — [`L26`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L26)
- `metric_parse_spec` — [`L135`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L135) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `plot_selection_spec` — [`L205`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L205) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `review_func_spec` — [`L81`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L81) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `vlm_feedback_spec` — [`L103`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/parallel_agent.py#L103) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)

