---
title: 'Module: ai_scientist/treesearch/agent_manager.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/agent_manager.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.agent_manager`/
symbols:
  AgentManager.run: AgentManager#run().
  Stage.name: Stage#name.
  AgentManager._check_stage_completion: AgentManager#_check_stage_completion().
  AgentManager._create_initial_stage: AgentManager#_create_initial_stage().
  AgentManager._create_next_substage: AgentManager#_create_next_substage().
  AgentManager._create_next_main_stage: AgentManager#_create_next_main_stage().
  AgentManager._create_agent_for_stage: AgentManager#_create_agent_for_stage().
  AgentManager._generate_substage_goal: AgentManager#_generate_substage_goal().
  AgentManager._gather_stage_metrics: AgentManager#_gather_stage_metrics().
  AgentManager._check_substage_completion: AgentManager#_check_substage_completion().
  AgentManager.current_stage: AgentManager#current_stage.
  AgentManager.cfg: AgentManager#cfg.
  AgentManager.journals: AgentManager#journals.
  AgentManager._save_checkpoint: AgentManager#_save_checkpoint().
  AgentManager._analyze_progress: AgentManager#_analyze_progress().
  AgentManager.task_desc: AgentManager#task_desc.
  AgentManager._get_best_implementation: AgentManager#_get_best_implementation().
  AgentManager._evaluate_stage_progression: AgentManager#_evaluate_stage_progression().
  AgentManager._parse_vlm_feedback: AgentManager#_parse_vlm_feedback().
  AgentManager._identify_issues: AgentManager#_identify_issues().
  logger: logger.
  Stage: Stage#
  AgentManager._create_stage_analysis_prompt: AgentManager#_create_stage_analysis_prompt().
  AgentManager.stages: AgentManager#stages.
  Stage.stage_number: Stage#stage_number.
  stage_completion_eval_spec: stage_completion_eval_spec.
  AgentManager._curate_task_desc: AgentManager#_curate_task_desc().
  stage_progress_eval_spec: stage_progress_eval_spec.
  stage_config_spec: stage_config_spec.
  AgentManager._save_stage_summary: AgentManager#_save_stage_summary().
  Stage.goals: Stage#goals.
  AgentManager.stage_history: AgentManager#stage_history.
  AgentManager._get_response: AgentManager#_get_response().
  AgentManager.workspace_dir: AgentManager#workspace_dir.
  Stage.description: Stage#description.
  Stage.max_iterations: Stage#max_iterations.
  AgentManager.main_stage_goals: AgentManager#main_stage_goals.
  AgentManager._get_max_iterations: AgentManager#_get_max_iterations().
  Stage.num_drafts: Stage#num_drafts.
  AgentManager.parse_stage_names: AgentManager#parse_stage_names().
  AgentManager._get_task_desc_str: AgentManager#_get_task_desc_str().
  StageTransition: StageTransition#
  StageTransition.from_stage: StageTransition#from_stage.
  AgentManager.current_stage_number: AgentManager#current_stage_number.
  StageTransition.to_stage: StageTransition#to_stage.
  StageTransition.reason: StageTransition#reason.
  StageTransition.config_adjustments: StageTransition#config_adjustments.
  AgentManager: AgentManager#
  AgentManager.main_stage_dict: AgentManager#main_stage_dict.
  AgentManager.__init__: AgentManager#__init__().
  AgentManager.completed_stages: AgentManager#completed_stages.
---
# Module: [`ai_scientist/treesearch/agent_manager.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py)

## Classes
### `AgentManager`
- def: [`ai_scientist/treesearch/agent_manager.py:123`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L123)
- signature: `class AgentManager:`
- members:
  - `_analyze_progress(self, journal: Journal)` — [`L1127`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L1127) — Analyze progress and convergence in the current stage — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_check_stage_completion(self, stage: Stage)` — [`L410`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L410) — Check if current stage is complete based on criteria — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_check_substage_completion(self, current_substage: Stage, journal: Journal)` — [`L343`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L343) — Check if the current sub-stage is complete — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_create_agent_for_stage(self, stage: Stage)` — [`L274`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L274) — Create a ParallelAgent configured for the given stage — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_create_initial_stage(self)` — [`L200`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L200) — Create the initial stage configuration — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_create_next_substage(self, current_substage: Stage, journal: Journal, substage_feedback: str)` — [`L638`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L638) — Create the next sub-stage. Ask LLM to come up with the next sub-stage name and goals — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_create_stage_analysis_prompt(self, previous_stages: List[Stage], previous_results: Optional[Dict[str, Any]], is_initial_stage: bool)` — [`L831`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L831) — Create detailed prompt to determine next stage configuration — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_evaluate_stage_progression(self, current_stage: Stage, previous_results: Dict[str, Any])` — [`L1151`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L1151) — Evaluate whether experiment is ready for next stage — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_gather_stage_metrics(self, journal: Journal)` — [`L1041`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L1041) — Gather detailed metrics and analysis from the stage's nodes — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_generate_substage_goal(self, main_stage_goal: str, journal: Journal)` — [`L552`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L552) — Generate the next sub-stage goal based on what has been done so far. — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_get_best_implementation(self, stage_name: str)` — [`L538`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L538) — Get the best implementation from a completed stage — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_get_max_iterations(self, stage_number: int)` — [`L171`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L171) — Get max iterations for a stage from config or default
  - `_get_response(self, prompt: str)` — [`L978`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L978) — Get structured response from LLM for stage configuration.
  - `_identify_issues(self, journal: Journal)` — [`L1084`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L1084) — Identify systemic issues and challenges from the current stage's results — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
  - `_parse_vlm_feedback(self, node: Node)` — [`L331`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L331) — Parse the feedback from the VLM — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_save_checkpoint(self)` — [`L249`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L249) — Save the current state of the experiment — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `_save_stage_summary(self, current_results: Dict[str, Any], evaluation: Dict[str, Any])` — [`L943`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L943) — Save comprehensive stage completion summary
  - `parse_stage_names(self, stage_name: str)` — [`L927`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L927) — Parse stage name into main stage number, main stage name,
  - `run(self, exec_callback, step_callback=None)` — [`L692`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L692) — Run the experiment through generated stages — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `cfg` — [`L135`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L135)
  - `completed_stages` — [`L142`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L142)
  - `current_stage` — [`L139`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L139) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `current_stage_number` — [`L137`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L137)
  - `journals` — [`L140`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L140) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `main_stage_dict` — [`L143`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L143)
  - `main_stage_goals` — [`L149`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L149)
  - `stage_history` — [`L141`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L141)
  - `stages` — [`L138`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L138) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `task_desc` — [`L125`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L125)
  - `workspace_dir` — [`L136`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L136)
- protocol/private: `__init__`[`L124`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L124), `_create_next_main_stage`[`L664`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L664), `_curate_task_desc`[`L216`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L216), `_get_task_desc_str`[`L179`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L179)
- uses (calls/refs, reference-scoped): [`step`](parallel_agent.md#ParallelAgent.step), [`Node`](journal.md#Node), [`name`](agent_manager.md#Stage.name), [`value`](utils/metric.md#MetricValue.value), [`_run_plot_aggregation`](parallel_agent.md#ParallelAgent._run_plot_aggregation), [`_run_multi_seed_evaluation`](parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`metric`](journal.md#Node.metric), [`id`](journal.md#Node.id), [`parent`](journal.md#Node.parent), [`query`](backend/__init__.md#query), [`get_best_node`](journal.md#Journal.get_best_node), [`nodes`](journal.md#Journal.nodes), [`Journal`](journal.md#Journal), [`good_nodes`](journal.md#Journal.good_nodes), [`FunctionSpec`](backend/utils.md#FunctionSpec), [`is_buggy`](journal.md#Node.is_buggy), [`logger`](agent_manager.md#logger), [`Stage`](agent_manager.md#Stage), [`children`](journal.md#Node.children), [`stage_number`](agent_manager.md#Stage.stage_number), [`analysis`](journal.md#Node.analysis), [`name`](backend/utils.md#FunctionSpec.name), [`stage_completion_eval_spec`](agent_manager.md#stage_completion_eval_spec), [`append`](journal.md#Journal.append), [`buggy_nodes`](journal.md#Journal.buggy_nodes), [`json_schema`](backend/utils.md#FunctionSpec.json_schema), [`stage_progress_eval_spec`](agent_manager.md#stage_progress_eval_spec), [`description`](backend/utils.md#FunctionSpec.description), [`vlm_feedback_summary`](journal.md#Node.vlm_feedback_summary), [`goals`](agent_manager.md#Stage.goals), [`maximize`](utils/metric.md#MetricValue.maximize), [`name`](utils/metric.md#MetricValue.name), [`plot_analyses`](journal.md#Node.plot_analyses), [`description`](agent_manager.md#Stage.description), [`exec_time_feedback`](journal.md#Node.exec_time_feedback), [`max_iterations`](agent_manager.md#Stage.max_iterations), [`is_leaf`](journal.md#Node.is_leaf), [`datasets_successfully_tested`](journal.md#Node.datasets_successfully_tested), [`exec_time`](journal.md#Node.exec_time), [`num_drafts`](agent_manager.md#Stage.num_drafts)  (+6 more)
- used by: [`perform_experiments_bfts`](perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts)

### `Stage`
- def: [`ai_scientist/treesearch/agent_manager.py:104`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L104) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
- signature: `class Stage:`
- members:
  - `description` — [`L106`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L106)
  - `goals` — [`L107`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L107)
  - `max_iterations` — [`L108`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L108)
  - `name` — [`L105`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L105) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `num_drafts` — [`L109`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L109)
  - `stage_number` — [`L110`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L110) — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
- used by: [`run`](agent_manager.md#AgentManager.run), [`_check_stage_completion`](agent_manager.md#AgentManager._check_stage_completion), [`_create_initial_stage`](agent_manager.md#AgentManager._create_initial_stage), [`_create_next_main_stage`](agent_manager.md#AgentManager._create_next_main_stage), [`_create_next_substage`](agent_manager.md#AgentManager._create_next_substage), [`_create_agent_for_stage`](agent_manager.md#AgentManager._create_agent_for_stage), [`_check_substage_completion`](agent_manager.md#AgentManager._check_substage_completion), [`current_stage`](agent_manager.md#AgentManager.current_stage), [`_save_checkpoint`](agent_manager.md#AgentManager._save_checkpoint), [`_evaluate_stage_progression`](agent_manager.md#AgentManager._evaluate_stage_progression), [`_parse_vlm_feedback`](agent_manager.md#AgentManager._parse_vlm_feedback), [`_create_stage_analysis_prompt`](agent_manager.md#AgentManager._create_stage_analysis_prompt), [`stages`](agent_manager.md#AgentManager.stages), [`_curate_task_desc`](agent_manager.md#AgentManager._curate_task_desc), [`_save_stage_summary`](agent_manager.md#AgentManager._save_stage_summary)

### `StageTransition`
- def: [`ai_scientist/treesearch/agent_manager.py:114`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L114)
- doc: Records transition between stages and the reasoning
- signature: `class StageTransition:`
- members:
  - `config_adjustments` — [`L120`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L120)
  - `from_stage` — [`L117`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L117)
  - `reason` — [`L119`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L119)
  - `to_stage` — [`L118`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L118)
- used by: [`run`](agent_manager.md#AgentManager.run), [`stage_history`](agent_manager.md#AgentManager.stage_history)

## Module values
- `logger` — [`L18`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L18)
- `stage_completion_eval_spec` — [`L78`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L78) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `stage_config_spec` — [`L21`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L21) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `stage_progress_eval_spec` — [`L49`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/agent_manager.py#L49) — documented in [ai_scientist-treesearch-backend-utils](../../../concepts/ai_scientist-treesearch-backend-utils.md)

