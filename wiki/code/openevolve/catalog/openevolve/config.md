---
title: 'Module: openevolve/config.py'
type: catalog
provenance: extracted
module: openevolve/config.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.config`/
symbols:
  Config: Config#
  Config.database: Config#database.
  Config.llm: Config#llm.
  Config.evaluator: Config#evaluator.
  LLMConfig.models: LLMConfig#models.
  LLMConfig.rebuild_models: LLMConfig#rebuild_models().
  LLMConfig.__post_init__: LLMConfig#__post_init__().
  Config.prompt: Config#prompt.
  Config.from_dict: Config#from_dict().
  LLMModelConfig: LLMModelConfig#
  DatabaseConfig: DatabaseConfig#
  DatabaseConfig.num_islands: DatabaseConfig#num_islands.
  DatabaseConfig.feature_dimensions: DatabaseConfig#feature_dimensions.
  load_config: load_config().
  LLMModelConfig.api_key: LLMModelConfig#api_key.
  LLMModelConfig.name: LLMModelConfig#name.
  DatabaseConfig.in_memory: DatabaseConfig#in_memory.
  EvaluatorConfig.timeout: EvaluatorConfig#timeout.
  EvaluatorConfig.cascade_evaluation: EvaluatorConfig#cascade_evaluation.
  EvaluatorConfig: EvaluatorConfig#
  Config.evolution_trace: Config#evolution_trace.
  LLMModelConfig.weight: LLMModelConfig#weight.
  PromptConfig.programs_as_changes_description: PromptConfig#programs_as_changes_description.
  Config.from_yaml: Config#from_yaml().
  DatabaseConfig.db_path: DatabaseConfig#db_path.
  LLMConfig.evaluator_models: LLMConfig#evaluator_models.
  DatabaseConfig.population_size: DatabaseConfig#population_size.
  PromptConfig: PromptConfig#
  LLMConfig.primary_model: LLMConfig#primary_model.
  DatabaseConfig.exploration_ratio: DatabaseConfig#exploration_ratio.
  DatabaseConfig.feature_bins: DatabaseConfig#feature_bins.
  Config.max_iterations: Config#max_iterations.
  LLMConfig: LLMConfig#
  DatabaseConfig.max_snapshot_artifacts: DatabaseConfig#max_snapshot_artifacts.
  Config.checkpoint_interval: Config#checkpoint_interval.
  LLMConfig.secondary_model_weight: LLMConfig#secondary_model_weight.
  DatabaseConfig.exploitation_ratio: DatabaseConfig#exploitation_ratio.
  Config.language: Config#language.
  Config.early_stopping_patience: Config#early_stopping_patience.
  LLMModelConfig.api_base: LLMModelConfig#api_base.
  LLMModelConfig.random_seed: LLMModelConfig#random_seed.
  LLMConfig.secondary_model: LLMConfig#secondary_model.
  EvaluatorConfig.parallel_evaluations: EvaluatorConfig#parallel_evaluations.
  Config.random_seed: Config#random_seed.
  LLMConfig.api_base: LLMConfig#api_base.
  LLMConfig.temperature: LLMConfig#temperature.
  LLMConfig.update_model_params: LLMConfig#update_model_params().
  PromptConfig.template_dir: PromptConfig#template_dir.
  PromptConfig.initial_changes_description: PromptConfig#initial_changes_description.
  Config.diff_based_evolution: Config#diff_based_evolution.
  Config.early_stopping_metric: Config#early_stopping_metric.
  _resolve_env_var: _resolve_env_var().
  LLMConfig.top_p: LLMConfig#top_p.
  PromptConfig.system_message_changes_description: PromptConfig#system_message_changes_description.
  PromptConfig.num_top_programs: PromptConfig#num_top_programs.
  DatabaseConfig.migration_interval: DatabaseConfig#migration_interval.
  LLMModelConfig.temperature: LLMModelConfig#temperature.
  EvaluatorConfig.max_retries: EvaluatorConfig#max_retries.
  Config.convergence_threshold: Config#convergence_threshold.
  DatabaseConfig.novelty_llm: DatabaseConfig#novelty_llm.
  LLMModelConfig.reasoning_effort: LLMModelConfig#reasoning_effort.
  LLMModelConfig.__post_init__: LLMModelConfig#__post_init__().
  LLMConfig.retries: LLMConfig#retries.
  LLMConfig.reasoning_effort: LLMConfig#reasoning_effort.
  DatabaseConfig.random_seed: DatabaseConfig#random_seed.
  LLMModelConfig.top_p: LLMModelConfig#top_p.
  LLMConfig.timeout: LLMConfig#timeout.
  DatabaseConfig.archive_size: DatabaseConfig#archive_size.
  EvolutionTraceConfig.format: EvolutionTraceConfig#format.
  Config.max_code_length: Config#max_code_length.
  LLMModelConfig.retries: LLMModelConfig#retries.
  LLMConfig.primary_model_weight: LLMConfig#primary_model_weight.
  PromptConfig.diff_summary_max_line_len: PromptConfig#diff_summary_max_line_len.
  PromptConfig.diff_summary_max_lines: PromptConfig#diff_summary_max_lines.
  DatabaseConfig.migration_rate: DatabaseConfig#migration_rate.
  EvaluatorConfig.cascade_thresholds: EvaluatorConfig#cascade_thresholds.
  EvolutionTraceConfig: EvolutionTraceConfig#
  EvolutionTraceConfig.enabled: EvolutionTraceConfig#enabled.
  EvolutionTraceConfig.include_code: EvolutionTraceConfig#include_code.
  EvolutionTraceConfig.include_prompts: EvolutionTraceConfig#include_prompts.
  Config.diff_pattern: Config#diff_pattern.
  LLMModelConfig.init_client: LLMModelConfig#init_client.
  LLMModelConfig.timeout: LLMModelConfig#timeout.
  LLMModelConfig._manual_queue_dir: LLMModelConfig#_manual_queue_dir.
  LLMConfig.max_tokens: LLMConfig#max_tokens.
  LLMConfig.retry_delay: LLMConfig#retry_delay.
  PromptConfig.num_diverse_programs: PromptConfig#num_diverse_programs.
  DatabaseConfig.log_prompts: DatabaseConfig#log_prompts.
  DatabaseConfig.embedding_model: DatabaseConfig#embedding_model.
  DatabaseConfig.similarity_threshold: DatabaseConfig#similarity_threshold.
  Config.file_suffix: Config#file_suffix.
  Config.to_yaml: Config#to_yaml().
  PromptConfig.system_message: PromptConfig#system_message.
  PromptConfig.include_artifacts: PromptConfig#include_artifacts.
  PromptConfig.max_artifact_bytes: PromptConfig#max_artifact_bytes.
  PromptConfig.artifact_security_filter: PromptConfig#artifact_security_filter.
  PromptConfig.include_changes_under_chars: PromptConfig#include_changes_under_chars.
  PromptConfig.concise_implementation_max_lines: PromptConfig#concise_implementation_max_lines.
  PromptConfig.comprehensive_implementation_min_lines: PromptConfig#comprehensive_implementation_min_lines.
  DatabaseConfig.cleanup_old_artifacts: DatabaseConfig#cleanup_old_artifacts.
  DatabaseConfig.artifact_retention_days: DatabaseConfig#artifact_retention_days.
  EvaluatorConfig.llm_feedback_weight: EvaluatorConfig#llm_feedback_weight.
  EvolutionTraceConfig.output_path: EvolutionTraceConfig#output_path.
  EvolutionTraceConfig.buffer_size: EvolutionTraceConfig#buffer_size.
  Config.log_level: Config#log_level.
  Config.log_dir: Config#log_dir.
  Config.max_tasks_per_child: Config#max_tasks_per_child.
  Config.to_dict: Config#to_dict().
  _ENV_VAR_PATTERN: _ENV_VAR_PATTERN.
  LLMConfig.manual_mode: LLMConfig#manual_mode.
  PromptConfig.use_template_stochasticity: PromptConfig#use_template_stochasticity.
  PromptConfig.template_variations: PromptConfig#template_variations.
  PromptConfig.suggest_simplification_after_chars: PromptConfig#suggest_simplification_after_chars.
  PromptConfig.code_length_threshold: PromptConfig#code_length_threshold.
  DatabaseConfig.elite_selection_ratio: DatabaseConfig#elite_selection_ratio.
  EvaluatorConfig.use_llm_feedback: EvaluatorConfig#use_llm_feedback.
  EvolutionTraceConfig.compress: EvolutionTraceConfig#compress.
  LLMModelConfig.system_message: LLMModelConfig#system_message.
  LLMModelConfig.max_tokens: LLMModelConfig#max_tokens.
  LLMModelConfig.retry_delay: LLMModelConfig#retry_delay.
  LLMModelConfig.manual_mode: LLMModelConfig#manual_mode.
  LLMConfig.system_message: LLMConfig#system_message.
  PromptConfig.evaluator_system_message: PromptConfig#evaluator_system_message.
  PromptConfig.use_meta_prompting: PromptConfig#use_meta_prompting.
  PromptConfig.meta_prompt_weight: PromptConfig#meta_prompt_weight.
  DatabaseConfig.diversity_metric: DatabaseConfig#diversity_metric.
  DatabaseConfig.diversity_reference_size: DatabaseConfig#diversity_reference_size.
  DatabaseConfig.artifacts_base_path: DatabaseConfig#artifacts_base_path.
  DatabaseConfig.artifact_size_threshold: DatabaseConfig#artifact_size_threshold.
  EvaluatorConfig.memory_limit_mb: EvaluatorConfig#memory_limit_mb.
  EvaluatorConfig.cpu_limit: EvaluatorConfig#cpu_limit.
  EvaluatorConfig.distributed: EvaluatorConfig#distributed.
  EvaluatorConfig.enable_artifacts: EvaluatorConfig#enable_artifacts.
  EvaluatorConfig.max_artifact_storage: EvaluatorConfig#max_artifact_storage.
---
# Module: [`openevolve/config.py`](../../../../../raw/code/openevolve/openevolve/config.py)

## Classes
### `Config`
- def: [`openevolve/config.py:401`](../../../../../raw/code/openevolve/openevolve/config.py#L401) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- doc: Master configuration for OpenEvolve
- signature: `class Config:`
- members:
  - `from_dict(cls, config_dict: Dict[str, Any])` — [`L450`](../../../../../raw/code/openevolve/openevolve/config.py#L450) — documented in [openevolve-config](../../concepts/openevolve-config.md)
  - `from_yaml(cls, path: Union[str, Path])` — [`L434`](../../../../../raw/code/openevolve/openevolve/config.py#L434) — Load configuration from a YAML file
  - `to_dict(self)` — [`L485`](../../../../../raw/code/openevolve/openevolve/config.py#L485)
  - `to_yaml(self, path: Union[str, Path])` — [`L488`](../../../../../raw/code/openevolve/openevolve/config.py#L488) — Save configuration to a YAML file
  - `checkpoint_interval` — [`L406`](../../../../../raw/code/openevolve/openevolve/config.py#L406)
  - `convergence_threshold` — [`L427`](../../../../../raw/code/openevolve/openevolve/config.py#L427)
  - `database` — [`L416`](../../../../../raw/code/openevolve/openevolve/config.py#L416) — documented in [openevolve-config](../../concepts/openevolve-config.md)
  - `diff_based_evolution` — [`L421`](../../../../../raw/code/openevolve/openevolve/config.py#L421)
  - `diff_pattern` — [`L423`](../../../../../raw/code/openevolve/openevolve/config.py#L423)
  - `early_stopping_metric` — [`L428`](../../../../../raw/code/openevolve/openevolve/config.py#L428)
  - `early_stopping_patience` — [`L426`](../../../../../raw/code/openevolve/openevolve/config.py#L426)
  - `evaluator` — [`L417`](../../../../../raw/code/openevolve/openevolve/config.py#L417) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `evolution_trace` — [`L418`](../../../../../raw/code/openevolve/openevolve/config.py#L418)
  - `file_suffix` — [`L411`](../../../../../raw/code/openevolve/openevolve/config.py#L411)
  - `language` — [`L410`](../../../../../raw/code/openevolve/openevolve/config.py#L410)
  - `llm` — [`L414`](../../../../../raw/code/openevolve/openevolve/config.py#L414) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `log_dir` — [`L408`](../../../../../raw/code/openevolve/openevolve/config.py#L408)
  - `log_level` — [`L407`](../../../../../raw/code/openevolve/openevolve/config.py#L407)
  - `max_code_length` — [`L422`](../../../../../raw/code/openevolve/openevolve/config.py#L422)
  - `max_iterations` — [`L405`](../../../../../raw/code/openevolve/openevolve/config.py#L405)
  - `max_tasks_per_child` — [`L431`](../../../../../raw/code/openevolve/openevolve/config.py#L431)
  - `prompt` — [`L415`](../../../../../raw/code/openevolve/openevolve/config.py#L415) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `random_seed` — [`L409`](../../../../../raw/code/openevolve/openevolve/config.py#L409)
- uses (calls/refs, reference-scoped): [`DatabaseConfig`](config.md#DatabaseConfig), [`EvaluatorConfig`](config.md#EvaluatorConfig), [`programs_as_changes_description`](config.md#PromptConfig.programs_as_changes_description), [`PromptConfig`](config.md#PromptConfig), [`LLMConfig`](config.md#LLMConfig), [`template_dir`](config.md#PromptConfig.template_dir), [`random_seed`](config.md#DatabaseConfig.random_seed), [`EvolutionTraceConfig`](config.md#EvolutionTraceConfig)
- used by: [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`run`](controller.md#OpenEvolve.run), [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker), [`database`](controller.md#OpenEvolve.database), [`run_evolution`](process_parallel.md#ProcessParallelController.run_evolution), [`_serialize_config`](process_parallel.md#ProcessParallelController._serialize_config), [`_warned_about_combined_score`](process_parallel.md#ProcessParallelController._warned_about_combined_score), [`_run_evolution_async`](api.md#_run_evolution_async), [`main_async`](cli.md#main_async), [`_submit_iteration`](process_parallel.md#ProcessParallelController._submit_iteration), [`output_dir`](controller.md#OpenEvolve.output_dir), [`_run_evolution_with_checkpoints`](controller.md#OpenEvolve._run_evolution_with_checkpoints), [`load_config`](config.md#load_config), [`evolution_tracer`](controller.md#OpenEvolve.evolution_tracer), [`_worker_init`](process_parallel.md#_worker_init), [`evaluator_prompt_sampler`](controller.md#OpenEvolve.evaluator_prompt_sampler), [`_lazy_init_worker_components`](process_parallel.md#_lazy_init_worker_components), [`start`](process_parallel.md#ProcessParallelController.start), [`run_evolution`](api.md#run_evolution), [`_setup_manual_mode_queue`](controller.md#OpenEvolve._setup_manual_mode_queue), [`evaluation_file`](controller.md#OpenEvolve.evaluation_file), [`evaluator`](controller.md#OpenEvolve.evaluator), [`initial_program_code`](controller.md#OpenEvolve.initial_program_code), [`file_extension`](controller.md#OpenEvolve.file_extension), [`num_islands`](process_parallel.md#ProcessParallelController.num_islands), [`_setup_logging`](controller.md#OpenEvolve._setup_logging), [`llm_ensemble`](controller.md#OpenEvolve.llm_ensemble), [`llm_evaluator_ensemble`](controller.md#OpenEvolve.llm_evaluator_ensemble), [`num_workers`](process_parallel.md#ProcessParallelController.num_workers), [`prompt_sampler`](controller.md#OpenEvolve.prompt_sampler), [`__init__`](process_parallel.md#ProcessParallelController.__init__), [`__init__`](controller.md#OpenEvolve.__init__)  (145 test-only)

### `DatabaseConfig`
- def: [`openevolve/config.py:295`](../../../../../raw/code/openevolve/openevolve/config.py#L295) — documented in [openevolve-config](../../concepts/openevolve-config.md)
- doc: Configuration for the program database
- signature: `class DatabaseConfig:`
- members:
  - `archive_size` — [`L307`](../../../../../raw/code/openevolve/openevolve/config.py#L307)
  - `artifact_retention_days` — [`L346`](../../../../../raw/code/openevolve/openevolve/config.py#L346)
  - `artifact_size_threshold` — [`L344`](../../../../../raw/code/openevolve/openevolve/config.py#L344)
  - `artifacts_base_path` — [`L343`](../../../../../raw/code/openevolve/openevolve/config.py#L343)
  - `cleanup_old_artifacts` — [`L345`](../../../../../raw/code/openevolve/openevolve/config.py#L345)
  - `db_path` — [`L299`](../../../../../raw/code/openevolve/openevolve/config.py#L299)
  - `diversity_metric` — [`L315`](../../../../../raw/code/openevolve/openevolve/config.py#L315)
  - `diversity_reference_size` — [`L333`](../../../../../raw/code/openevolve/openevolve/config.py#L333)
  - `elite_selection_ratio` — [`L311`](../../../../../raw/code/openevolve/openevolve/config.py#L311)
  - `embedding_model` — [`L352`](../../../../../raw/code/openevolve/openevolve/config.py#L352)
  - `exploitation_ratio` — [`L313`](../../../../../raw/code/openevolve/openevolve/config.py#L313)
  - `exploration_ratio` — [`L312`](../../../../../raw/code/openevolve/openevolve/config.py#L312)
  - `feature_bins` — [`L332`](../../../../../raw/code/openevolve/openevolve/config.py#L332)
  - `feature_dimensions` — [`L322`](../../../../../raw/code/openevolve/openevolve/config.py#L322) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `in_memory` — [`L300`](../../../../../raw/code/openevolve/openevolve/config.py#L300)
  - `log_prompts` — [`L303`](../../../../../raw/code/openevolve/openevolve/config.py#L303)
  - `max_snapshot_artifacts` — [`L347`](../../../../../raw/code/openevolve/openevolve/config.py#L347)
  - `migration_interval` — [`L336`](../../../../../raw/code/openevolve/openevolve/config.py#L336)
  - `migration_rate` — [`L337`](../../../../../raw/code/openevolve/openevolve/config.py#L337)
  - `novelty_llm` — [`L351`](../../../../../raw/code/openevolve/openevolve/config.py#L351)
  - `num_islands` — [`L308`](../../../../../raw/code/openevolve/openevolve/config.py#L308) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `population_size` — [`L306`](../../../../../raw/code/openevolve/openevolve/config.py#L306)
  - `random_seed` — [`L340`](../../../../../raw/code/openevolve/openevolve/config.py#L340)
  - `similarity_threshold` — [`L353`](../../../../../raw/code/openevolve/openevolve/config.py#L353)
- uses (calls/refs, reference-scoped): [`LLMInterface`](llm/base.md#LLMInterface)
- used by: [`add`](database.md#ProgramDatabase.add), [`database`](config.md#Config.database), [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`islands`](database.md#ProgramDatabase.islands), [`migrate_programs`](database.md#ProgramDatabase.migrate_programs), [`load`](database.md#ProgramDatabase.load), [`_serialize_config`](process_parallel.md#ProcessParallelController._serialize_config), [`save`](database.md#ProgramDatabase.save), [`sample_from_island`](database.md#ProgramDatabase.sample_from_island), [`_calculate_feature_coords`](database.md#ProgramDatabase._calculate_feature_coords), [`island_feature_maps`](database.md#ProgramDatabase.island_feature_maps), [`from_dict`](config.md#Config.from_dict), [`island_best_programs`](database.md#ProgramDatabase.island_best_programs), [`_sample_inspirations`](database.md#ProgramDatabase._sample_inspirations), [`island_generations`](database.md#ProgramDatabase.island_generations), [`_enforce_population_limit`](database.md#ProgramDatabase._enforce_population_limit), [`_llm_evaluate`](evaluator.md#Evaluator._llm_evaluate), [`_run_evolution_with_checkpoints`](controller.md#OpenEvolve._run_evolution_with_checkpoints), [`get_best_program`](database.md#ProgramDatabase.get_best_program), [`feature_bins`](database.md#ProgramDatabase.feature_bins), [`_reconstruct_islands`](database.md#ProgramDatabase._reconstruct_islands), [`_sample_from_island_weighted`](database.md#ProgramDatabase._sample_from_island_weighted), [`_worker_init`](process_parallel.md#_worker_init), [`evaluator_prompt_sampler`](controller.md#OpenEvolve.evaluator_prompt_sampler), [`get_top_programs`](database.md#ProgramDatabase.get_top_programs), [`_update_archive`](database.md#ProgramDatabase._update_archive), [`feature_bins_per_dim`](database.md#ProgramDatabase.feature_bins_per_dim), [`_create_database_snapshot`](process_parallel.md#ProcessParallelController._create_database_snapshot), [`get_island_stats`](database.md#ProgramDatabase.get_island_stats), [`last_iteration`](database.md#ProgramDatabase.last_iteration), [`_is_better`](database.md#ProgramDatabase._is_better), [`_sample_parent`](database.md#ProgramDatabase._sample_parent), [`_save_program`](database.md#ProgramDatabase._save_program), [`num_islands`](process_parallel.md#ProcessParallelController.num_islands), [`prompts_by_program`](database.md#ProgramDatabase.prompts_by_program), [`_cleanup_old_artifacts`](database.md#ProgramDatabase._cleanup_old_artifacts), [`log_prompt`](database.md#ProgramDatabase.log_prompt), [`embedding_client`](database.md#ProgramDatabase.embedding_client), [`_create_artifact_dir`](database.md#ProgramDatabase._create_artifact_dir), [`feature_scaling_method`](database.md#ProgramDatabase.feature_scaling_method)  (+3 more; 79 test-only)

### `EvaluatorConfig`
- def: [`openevolve/config.py:357`](../../../../../raw/code/openevolve/openevolve/config.py#L357)
- doc: Configuration for program evaluation
- signature: `class EvaluatorConfig:`
- members:
  - `cascade_evaluation` — [`L370`](../../../../../raw/code/openevolve/openevolve/config.py#L370) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `cascade_thresholds` — [`L371`](../../../../../raw/code/openevolve/openevolve/config.py#L371)
  - `cpu_limit` — [`L367`](../../../../../raw/code/openevolve/openevolve/config.py#L367)
  - `distributed` — [`L376`](../../../../../raw/code/openevolve/openevolve/config.py#L376)
  - `enable_artifacts` — [`L383`](../../../../../raw/code/openevolve/openevolve/config.py#L383)
  - `llm_feedback_weight` — [`L380`](../../../../../raw/code/openevolve/openevolve/config.py#L380)
  - `max_artifact_storage` — [`L384`](../../../../../raw/code/openevolve/openevolve/config.py#L384)
  - `max_retries` — [`L362`](../../../../../raw/code/openevolve/openevolve/config.py#L362)
  - `memory_limit_mb` — [`L366`](../../../../../raw/code/openevolve/openevolve/config.py#L366)
  - `parallel_evaluations` — [`L374`](../../../../../raw/code/openevolve/openevolve/config.py#L374)
  - `timeout` — [`L361`](../../../../../raw/code/openevolve/openevolve/config.py#L361) — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `use_llm_feedback` — [`L379`](../../../../../raw/code/openevolve/openevolve/config.py#L379)
- used by: [`run_evolution`](process_parallel.md#ProcessParallelController.run_evolution), [`evaluate_program`](evaluator.md#Evaluator.evaluate_program), [`evaluator`](config.md#Config.evaluator), [`_warned_about_combined_score`](process_parallel.md#ProcessParallelController._warned_about_combined_score), [`_run_evolution_async`](api.md#_run_evolution_async), [`_cascade_evaluate`](evaluator.md#Evaluator._cascade_evaluate), [`_worker_init`](process_parallel.md#_worker_init), [`_direct_evaluate`](evaluator.md#Evaluator._direct_evaluate), [`_create_cascade_error_context`](evaluator.md#Evaluator._create_cascade_error_context), [`_validate_cascade_configuration`](evaluator.md#Evaluator._validate_cascade_configuration), [`__init__`](evaluator.md#Evaluator.__init__), [`num_workers`](process_parallel.md#ProcessParallelController.num_workers), [`task_pool`](evaluator.md#Evaluator.task_pool)  (26 test-only)

### `EvolutionTraceConfig`
- def: [`openevolve/config.py:388`](../../../../../raw/code/openevolve/openevolve/config.py#L388)
- doc: Configuration for evolution trace logging
- signature: `class EvolutionTraceConfig:`
- members:
  - `buffer_size` — [`L396`](../../../../../raw/code/openevolve/openevolve/config.py#L396)
  - `compress` — [`L397`](../../../../../raw/code/openevolve/openevolve/config.py#L397)
  - `enabled` — [`L391`](../../../../../raw/code/openevolve/openevolve/config.py#L391)
  - `format` — [`L392`](../../../../../raw/code/openevolve/openevolve/config.py#L392)
  - `include_code` — [`L393`](../../../../../raw/code/openevolve/openevolve/config.py#L393)
  - `include_prompts` — [`L394`](../../../../../raw/code/openevolve/openevolve/config.py#L394)
  - `output_path` — [`L395`](../../../../../raw/code/openevolve/openevolve/config.py#L395)
- used by: [`evolution_tracer`](controller.md#OpenEvolve.evolution_tracer), [`evolution_trace`](config.md#Config.evolution_trace), [`evaluation_file`](controller.md#OpenEvolve.evaluation_file)  (2 test-only)

### `LLMConfig`  ·  implements/extends LLMModelConfig
- def: [`openevolve/config.py:92`](../../../../../raw/code/openevolve/openevolve/config.py#L92)
- doc: Configuration for LLM models
- signature: `class LLMConfig(LLMModelConfig):`
- members:
  - `__post_init__(self)` — [`L127`](../../../../../raw/code/openevolve/openevolve/config.py#L127) — Post-initialization to set up model configurations
  - `rebuild_models(self)` — [`L192`](../../../../../raw/code/openevolve/openevolve/config.py#L192) — Rebuild the models list after primary_model/secondary_model field changes
  - `update_model_params(self, args: Dict[str, Any], overwrite: bool = False)` — [`L185`](../../../../../raw/code/openevolve/openevolve/config.py#L185) — Update model parameters for all models
  - `api_base` — [`L96`](../../../../../raw/code/openevolve/openevolve/config.py#L96)
  - `evaluator_models` — [`L113`](../../../../../raw/code/openevolve/openevolve/config.py#L113)
  - `manual_mode` — [`L125`](../../../../../raw/code/openevolve/openevolve/config.py#L125)
  - `max_tokens` — [`L102`](../../../../../raw/code/openevolve/openevolve/config.py#L102)
  - `models` — [`L110`](../../../../../raw/code/openevolve/openevolve/config.py#L110) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `primary_model` — [`L116`](../../../../../raw/code/openevolve/openevolve/config.py#L116)
  - `primary_model_weight` — [`L117`](../../../../../raw/code/openevolve/openevolve/config.py#L117)
  - `reasoning_effort` — [`L122`](../../../../../raw/code/openevolve/openevolve/config.py#L122)
  - `retries` — [`L106`](../../../../../raw/code/openevolve/openevolve/config.py#L106)
  - `retry_delay` — [`L107`](../../../../../raw/code/openevolve/openevolve/config.py#L107)
  - `secondary_model` — [`L118`](../../../../../raw/code/openevolve/openevolve/config.py#L118)
  - `secondary_model_weight` — [`L119`](../../../../../raw/code/openevolve/openevolve/config.py#L119)
  - `system_message` — [`L99`](../../../../../raw/code/openevolve/openevolve/config.py#L99)
  - `temperature` — [`L100`](../../../../../raw/code/openevolve/openevolve/config.py#L100)
  - `timeout` — [`L105`](../../../../../raw/code/openevolve/openevolve/config.py#L105)
  - `top_p` — [`L101`](../../../../../raw/code/openevolve/openevolve/config.py#L101)
- uses (calls/refs, reference-scoped): [`LLMModelConfig`](config.md#LLMModelConfig), [`api_key`](config.md#LLMModelConfig.api_key), [`name`](config.md#LLMModelConfig.name), [`weight`](config.md#LLMModelConfig.weight), [`random_seed`](config.md#LLMModelConfig.random_seed), [`__post_init__`](config.md#LLMModelConfig.__post_init__)
- used by: [`llm`](config.md#Config.llm), [`_serialize_config`](process_parallel.md#ProcessParallelController._serialize_config), [`_run_evolution_async`](api.md#_run_evolution_async), [`main_async`](cli.md#main_async), [`LLMModelConfig`](config.md#LLMModelConfig), [`output_dir`](controller.md#OpenEvolve.output_dir), [`load_config`](config.md#load_config), [`_worker_init`](process_parallel.md#_worker_init), [`_lazy_init_worker_components`](process_parallel.md#_lazy_init_worker_components), [`_setup_manual_mode_queue`](controller.md#OpenEvolve._setup_manual_mode_queue), [`llm_ensemble`](controller.md#OpenEvolve.llm_ensemble), [`llm_evaluator_ensemble`](controller.md#OpenEvolve.llm_evaluator_ensemble)  (31 test-only)

### `LLMModelConfig`
- def: [`openevolve/config.py:51`](../../../../../raw/code/openevolve/openevolve/config.py#L51) — documented in [openevolve-config](../../concepts/openevolve-config.md)
- doc: Configuration for a single LLM model
- signature: `class LLMModelConfig:`
- members:
  - `__post_init__(self)` — [`L86`](../../../../../raw/code/openevolve/openevolve/config.py#L86) — Post-initialization to resolve ${VAR} env var references in api_key
  - `api_base` — [`L55`](../../../../../raw/code/openevolve/openevolve/config.py#L55)
  - `api_key` — [`L56`](../../../../../raw/code/openevolve/openevolve/config.py#L56) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `init_client` — [`L60`](../../../../../raw/code/openevolve/openevolve/config.py#L60) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
  - `manual_mode` — [`L83`](../../../../../raw/code/openevolve/openevolve/config.py#L83)
  - `max_tokens` — [`L69`](../../../../../raw/code/openevolve/openevolve/config.py#L69)
  - `name` — [`L57`](../../../../../raw/code/openevolve/openevolve/config.py#L57)
  - `random_seed` — [`L77`](../../../../../raw/code/openevolve/openevolve/config.py#L77) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
  - `reasoning_effort` — [`L80`](../../../../../raw/code/openevolve/openevolve/config.py#L80)
  - `retries` — [`L73`](../../../../../raw/code/openevolve/openevolve/config.py#L73)
  - `retry_delay` — [`L74`](../../../../../raw/code/openevolve/openevolve/config.py#L74)
  - `system_message` — [`L66`](../../../../../raw/code/openevolve/openevolve/config.py#L66)
  - `temperature` — [`L67`](../../../../../raw/code/openevolve/openevolve/config.py#L67)
  - `timeout` — [`L72`](../../../../../raw/code/openevolve/openevolve/config.py#L72)
  - `top_p` — [`L68`](../../../../../raw/code/openevolve/openevolve/config.py#L68)
  - `weight` — [`L63`](../../../../../raw/code/openevolve/openevolve/config.py#L63) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
- protocol/private: `_manual_queue_dir`[`L84`](../../../../../raw/code/openevolve/openevolve/config.py#L84)
- uses (calls/refs, reference-scoped): [`LLMConfig`](config.md#LLMConfig), [`_resolve_env_var`](config.md#_resolve_env_var)
- used by: [`_serialize_config`](process_parallel.md#ProcessParallelController._serialize_config), [`models`](config.md#LLMConfig.models), [`rebuild_models`](config.md#LLMConfig.rebuild_models), [`__post_init__`](config.md#LLMConfig.__post_init__), [`main_async`](cli.md#main_async), [`output_dir`](controller.md#OpenEvolve.output_dir), [`_worker_init`](process_parallel.md#_worker_init), [`_setup_manual_mode_queue`](controller.md#OpenEvolve._setup_manual_mode_queue), [`evaluator_models`](config.md#LLMConfig.evaluator_models), [`random_state`](llm/ensemble.md#LLMEnsemble.random_state), [`LLMConfig`](config.md#LLMConfig), [`models`](llm/ensemble.md#LLMEnsemble.models), [`weights`](llm/ensemble.md#LLMEnsemble.weights), [`__init__`](llm/ensemble.md#LLMEnsemble.__init__)  (31 test-only)

### `PromptConfig`
- def: [`openevolve/config.py:240`](../../../../../raw/code/openevolve/openevolve/config.py#L240)
- doc: Configuration for prompt generation
- signature: `class PromptConfig:`
- members:
  - `artifact_security_filter` — [`L268`](../../../../../raw/code/openevolve/openevolve/config.py#L268) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `code_length_threshold` — [`L289`](../../../../../raw/code/openevolve/openevolve/config.py#L289) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `comprehensive_implementation_min_lines` — [`L280`](../../../../../raw/code/openevolve/openevolve/config.py#L280) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `concise_implementation_max_lines` — [`L277`](../../../../../raw/code/openevolve/openevolve/config.py#L277) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `diff_summary_max_line_len` — [`L285`](../../../../../raw/code/openevolve/openevolve/config.py#L285)
  - `diff_summary_max_lines` — [`L286`](../../../../../raw/code/openevolve/openevolve/config.py#L286)
  - `evaluator_system_message` — [`L245`](../../../../../raw/code/openevolve/openevolve/config.py#L245)
  - `include_artifacts` — [`L266`](../../../../../raw/code/openevolve/openevolve/config.py#L266) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `include_changes_under_chars` — [`L274`](../../../../../raw/code/openevolve/openevolve/config.py#L274) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `initial_changes_description` — [`L250`](../../../../../raw/code/openevolve/openevolve/config.py#L250)
  - `max_artifact_bytes` — [`L267`](../../../../../raw/code/openevolve/openevolve/config.py#L267) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `meta_prompt_weight` — [`L263`](../../../../../raw/code/openevolve/openevolve/config.py#L263)
  - `num_diverse_programs` — [`L254`](../../../../../raw/code/openevolve/openevolve/config.py#L254) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `num_top_programs` — [`L253`](../../../../../raw/code/openevolve/openevolve/config.py#L253) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `programs_as_changes_description` — [`L248`](../../../../../raw/code/openevolve/openevolve/config.py#L248) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `suggest_simplification_after_chars` — [`L271`](../../../../../raw/code/openevolve/openevolve/config.py#L271) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `system_message` — [`L244`](../../../../../raw/code/openevolve/openevolve/config.py#L244) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `system_message_changes_description` — [`L249`](../../../../../raw/code/openevolve/openevolve/config.py#L249) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `template_dir` — [`L243`](../../../../../raw/code/openevolve/openevolve/config.py#L243) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `template_variations` — [`L258`](../../../../../raw/code/openevolve/openevolve/config.py#L258) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `use_meta_prompting` — [`L262`](../../../../../raw/code/openevolve/openevolve/config.py#L262)
  - `use_template_stochasticity` — [`L257`](../../../../../raw/code/openevolve/openevolve/config.py#L257) — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
- used by: [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`run`](controller.md#OpenEvolve.run), [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker), [`build_prompt`](prompt/sampler.md#PromptSampler.build_prompt), [`prompt`](config.md#Config.prompt), [`template_manager`](prompt/sampler.md#PromptSampler.template_manager), [`from_dict`](config.md#Config.from_dict), [`_submit_iteration`](process_parallel.md#ProcessParallelController._submit_iteration), [`load_config`](config.md#load_config), [`_worker_init`](process_parallel.md#_worker_init), [`_format_evolution_history`](prompt/sampler.md#PromptSampler._format_evolution_history), [`_extract_unique_features`](prompt/sampler.md#PromptSampler._extract_unique_features), [`_format_inspirations_section`](prompt/sampler.md#PromptSampler._format_inspirations_section), [`from_yaml`](config.md#Config.from_yaml), [`_identify_improvement_areas`](prompt/sampler.md#PromptSampler._identify_improvement_areas), [`_render_artifacts`](prompt/sampler.md#PromptSampler._render_artifacts), [`_safe_decode_artifact`](prompt/sampler.md#PromptSampler._safe_decode_artifact), [`_apply_template_variations`](prompt/sampler.md#PromptSampler._apply_template_variations), [`__init__`](prompt/sampler.md#PromptSampler.__init__)  (18 test-only)

## Functions
- `_resolve_env_var(value: Optional[str])` — [`L21`](../../../../../raw/code/openevolve/openevolve/config.py#L21) — Resolve ${VAR} environment variable reference in a string value.
- `load_config(config_path: Optional[Union[str, Path]] = None)` — [`L494`](../../../../../raw/code/openevolve/openevolve/config.py#L494) — Load configuration from a YAML file or use defaults — documented in [openevolve-api](../../concepts/openevolve-api.md)

## Module values
- `_ENV_VAR_PATTERN` — [`L18`](../../../../../raw/code/openevolve/openevolve/config.py#L18)

