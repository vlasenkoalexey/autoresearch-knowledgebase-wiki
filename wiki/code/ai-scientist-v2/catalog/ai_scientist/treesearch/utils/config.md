---
title: 'Module: ai_scientist/treesearch/utils/config.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/config.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.config`/
symbols:
  prep_cfg: prep_cfg().
  Config.agent: Config#agent.
  prep_agent_workspace: prep_agent_workspace().
  load_task_desc: load_task_desc().
  Config.log_dir: Config#log_dir.
  Config.workspace_dir: Config#workspace_dir.
  Config: Config#
  save_run: save_run().
  AgentConfig.code: AgentConfig#code.
  load_cfg: load_cfg().
  StageConfig: StageConfig#
  Config.exp_name: Config#exp_name.
  StageConfig.model: StageConfig#model.
  StageConfig.temp: StageConfig#temp.
  Config.data_dir: Config#data_dir.
  AgentConfig.summary: AgentConfig#summary.
  Config.exec: Config#exec.
  Config.desc_file: Config#desc_file.
  logger: logger.
  Config.goal: Config#goal.
  AgentConfig.search: AgentConfig#search.
  _load_cfg: _load_cfg().
  Config.eval: Config#eval.
  StageConfig.thinking: StageConfig#thinking.
  AgentConfig.feedback: AgentConfig#feedback.
  AgentConfig.vlm_feedback: AgentConfig#vlm_feedback.
  AgentConfig.select_node: AgentConfig#select_node.
  Config.report: Config#report.
  Config.experiment: Config#experiment.
  Config.debug: Config#debug.
  print_cfg: print_cfg().
  SearchConfig.num_drafts: SearchConfig#num_drafts.
  ExecConfig.timeout: ExecConfig#timeout.
  _get_next_logindex: _get_next_logindex().
  ThinkingConfig: ThinkingConfig#
  SearchConfig: SearchConfig#
  SearchConfig.max_debug_depth: SearchConfig#max_debug_depth.
  SearchConfig.debug_prob: SearchConfig#debug_prob.
  DebugConfig: DebugConfig#
  AgentConfig: AgentConfig#
  AgentConfig.steps: AgentConfig#steps.
  AgentConfig.num_workers: AgentConfig#num_workers.
  AgentConfig.multi_seed_eval: AgentConfig#multi_seed_eval.
  ExecConfig: ExecConfig#
  ExecConfig.agent_file_name: ExecConfig#agent_file_name.
  ExecConfig.format_tb_ipython: ExecConfig#format_tb_ipython.
  ExperimentConfig: ExperimentConfig#
  Config.preprocess_data: Config#preprocess_data.
  Config.copy_data: Config#copy_data.
  Config.generate_report: Config#generate_report.
  ThinkingConfig.budget_tokens: ThinkingConfig#budget_tokens.
  StageConfig.betas: StageConfig#betas.
  StageConfig.max_tokens: StageConfig#max_tokens.
  DebugConfig.stage4: DebugConfig#stage4.
  AgentConfig.stages: AgentConfig#stages.
  AgentConfig.k_fold_validation: AgentConfig#k_fold_validation.
  AgentConfig.expose_prediction: AgentConfig#expose_prediction.
  AgentConfig.data_preview: AgentConfig#data_preview.
  ExperimentConfig.num_syn_datasets: ExperimentConfig#num_syn_datasets.
---
# Module: [`ai_scientist/treesearch/utils/config.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py)

## Classes
### `AgentConfig`
- def: [`ai_scientist/treesearch/utils/config.py:57`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L57) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- signature: `class AgentConfig:`
- members:
  - `code` — [`L64`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L64)
  - `data_preview` — [`L62`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L62)
  - `expose_prediction` — [`L61`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L61)
  - `feedback` — [`L65`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L65)
  - `k_fold_validation` — [`L60`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L60)
  - `multi_seed_eval` — [`L71`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L71)
  - `num_workers` — [`L69`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L69)
  - `search` — [`L68`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L68)
  - `select_node` — [`L74`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L74)
  - `stages` — [`L59`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L59)
  - `steps` — [`L58`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L58)
  - `summary` — [`L73`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L73)
  - `vlm_feedback` — [`L66`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L66)
- uses (calls/refs, reference-scoped): [`StageConfig`](config.md#StageConfig), [`SearchConfig`](config.md#SearchConfig)
- used by: [`step`](../parallel_agent.md#ParallelAgent.step), [`_run_multi_seed_evaluation`](../parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`_select_parallel_nodes`](../parallel_agent.md#ParallelAgent._select_parallel_nodes), [`perform_experiments_bfts`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts), [`_generate_ablation_idea`](../parallel_agent.md#ParallelAgent._generate_ablation_idea), [`_generate_hyperparam_tuning_idea`](../parallel_agent.md#ParallelAgent._generate_hyperparam_tuning_idea), [`agent`](config.md#Config.agent), [`plan_and_code_query`](../parallel_agent.md#ParallelAgent.plan_and_code_query), [`_define_global_metrics`](../parallel_agent.md#ParallelAgent._define_global_metrics), [`step_callback`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts.step_callback), [`num_workers`](../parallel_agent.md#ParallelAgent.num_workers)

### `Config`  ·  implements/extends Hashable
- def: [`ai_scientist/treesearch/utils/config.py:89`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L89) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- signature: `class Config(Hashable):`
- members:
  - `agent` — [`L107`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L107) — documented in [ai_scientist-treesearch-parallel_agent](../../../../concepts/ai_scientist-treesearch-parallel_agent.md)
  - `copy_data` — [`L100`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L100) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `data_dir` — [`L90`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L90) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `debug` — [`L109`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L109)
  - `desc_file` — [`L91`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L91) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `eval` — [`L94`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L94) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `exec` — [`L104`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L104)
  - `exp_name` — [`L102`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L102) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `experiment` — [`L108`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L108)
  - `generate_report` — [`L105`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L105)
  - `goal` — [`L93`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L93) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `log_dir` — [`L96`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L96) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `preprocess_data` — [`L99`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L99) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
  - `report` — [`L106`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L106)
  - `workspace_dir` — [`L97`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L97) — documented in [ai_scientist-treesearch-parallel_agent](../../../../concepts/ai_scientist-treesearch-parallel_agent.md)
- uses (calls/refs, reference-scoped): [`StageConfig`](config.md#StageConfig), [`AgentConfig`](config.md#AgentConfig), [`DebugConfig`](config.md#DebugConfig), [`ExecConfig`](config.md#ExecConfig), [`ExperimentConfig`](config.md#ExperimentConfig)
- used by: [`step`](../parallel_agent.md#ParallelAgent.step), [`_run_plot_aggregation`](../parallel_agent.md#ParallelAgent._run_plot_aggregation), [`_run_multi_seed_evaluation`](../parallel_agent.md#ParallelAgent._run_multi_seed_evaluation), [`_select_parallel_nodes`](../parallel_agent.md#ParallelAgent._select_parallel_nodes), [`perform_experiments_bfts`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts), [`_generate_ablation_idea`](../parallel_agent.md#ParallelAgent._generate_ablation_idea), [`_generate_hyperparam_tuning_idea`](../parallel_agent.md#ParallelAgent._generate_hyperparam_tuning_idea), [`prep_cfg`](config.md#prep_cfg), [`plan_and_code_query`](../parallel_agent.md#ParallelAgent.plan_and_code_query), [`prep_agent_workspace`](config.md#prep_agent_workspace), [`_define_global_metrics`](../parallel_agent.md#ParallelAgent._define_global_metrics), [`step_callback`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts.step_callback), [`load_task_desc`](config.md#load_task_desc), [`save_run`](config.md#save_run), [`generate_live`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts.generate_live), [`num_workers`](../parallel_agent.md#ParallelAgent.num_workers), [`load_cfg`](config.md#load_cfg), [`timeout`](../parallel_agent.md#ParallelAgent.timeout), [`__init__`](../parallel_agent.md#ParallelAgent.__init__), [`_load_cfg`](config.md#_load_cfg), [`cleanup`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts.cleanup), [`print_cfg`](config.md#print_cfg)

### `DebugConfig`
- def: [`ai_scientist/treesearch/utils/config.py:52`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L52)
- signature: `class DebugConfig:`
- members:
  - `stage4` — [`L53`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L53)
- used by: [`debug`](config.md#Config.debug)

### `ExecConfig`
- def: [`ai_scientist/treesearch/utils/config.py:77`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L77)
- signature: `class ExecConfig:`
- members:
  - `agent_file_name` — [`L79`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L79)
  - `format_tb_ipython` — [`L80`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L80)
  - `timeout` — [`L78`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L78)
- used by: [`_run_plot_aggregation`](../parallel_agent.md#ParallelAgent._run_plot_aggregation), [`timeout`](../parallel_agent.md#ParallelAgent.timeout), [`exec`](config.md#Config.exec)

### `ExperimentConfig`
- def: [`ai_scientist/treesearch/utils/config.py:84`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L84)
- signature: `class ExperimentConfig:`
- members:
  - `num_syn_datasets` — [`L85`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L85)
- used by: [`experiment`](config.md#Config.experiment)

### `SearchConfig`
- def: [`ai_scientist/treesearch/utils/config.py:45`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L45)
- signature: `class SearchConfig:`
- members:
  - `debug_prob` — [`L47`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L47)
  - `max_debug_depth` — [`L46`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L46)
  - `num_drafts` — [`L48`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L48)
- used by: [`_select_parallel_nodes`](../parallel_agent.md#ParallelAgent._select_parallel_nodes), [`search`](config.md#AgentConfig.search)

### `StageConfig`
- def: [`ai_scientist/treesearch/utils/config.py:36`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L36)
- signature: `class StageConfig:`
- members:
  - `betas` — [`L40`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L40)
  - `max_tokens` — [`L41`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L41)
  - `model` — [`L37`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L37)
  - `temp` — [`L38`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L38)
  - `thinking` — [`L39`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L39)
- uses (calls/refs, reference-scoped): [`ThinkingConfig`](config.md#ThinkingConfig)
- used by: [`step`](../parallel_agent.md#ParallelAgent.step), [`_generate_ablation_idea`](../parallel_agent.md#ParallelAgent._generate_ablation_idea), [`_generate_hyperparam_tuning_idea`](../parallel_agent.md#ParallelAgent._generate_hyperparam_tuning_idea), [`plan_and_code_query`](../parallel_agent.md#ParallelAgent.plan_and_code_query), [`_define_global_metrics`](../parallel_agent.md#ParallelAgent._define_global_metrics), [`journal2report`](../journal2report.md#journal2report), [`step_callback`](../perform_experiments_bfts_with_agentmanager.md#perform_experiments_bfts.step_callback), [`code`](config.md#AgentConfig.code), [`summary`](config.md#AgentConfig.summary), [`feedback`](config.md#AgentConfig.feedback), [`report`](config.md#Config.report), [`select_node`](config.md#AgentConfig.select_node), [`vlm_feedback`](config.md#AgentConfig.vlm_feedback)

### `ThinkingConfig`
- def: [`ai_scientist/treesearch/utils/config.py:30`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L30)
- signature: `class ThinkingConfig:`
- members:
  - `budget_tokens` — [`L32`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L32)
- used by: [`thinking`](config.md#StageConfig.thinking)

## Functions
- `_get_next_logindex(dir: Path)` — [`L112`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L112) — Get the next available index for a log directory. — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `_load_cfg(path: Path = Path(__file__).parent / "config.yaml", use_cli_args=False)` — [`L125`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L125)
- `load_cfg(path: Path = Path(__file__).parent / "config.yaml")` — [`L134`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L134) — Load config from .yaml file and CLI args, and set up logging directory. — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `load_task_desc(cfg: Config)` — [`L183`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L183) — Load task description from markdown file or config str. — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `prep_agent_workspace(cfg: Config)` — [`L209`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L209) — Setup the agent's workspace and preprocess data if necessary. — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `prep_cfg(cfg: Config)` — [`L139`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L139) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `print_cfg(cfg: Config)` — [`L179`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L179)
- `save_run(cfg: Config, journal, stage_name: str = None)` — [`L219`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L219)

## Module values
- `logger` — [`L22`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/config.py#L22) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)

