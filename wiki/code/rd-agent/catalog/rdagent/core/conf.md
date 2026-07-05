---
title: 'Module: rdagent/core/conf.py'
type: catalog
provenance: extracted
module: rdagent/core/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.conf`/
symbols:
  RD_AGENT_SETTINGS: RD_AGENT_SETTINGS.
  ExtendedBaseSettings: ExtendedBaseSettings#
  RDAgentSettings.get_max_parallel: RDAgentSettings#get_max_parallel().
  RDAgentSettings.multi_proc_n: RDAgentSettings#multi_proc_n.
  ExtendedBaseSettings.base_iter: ExtendedBaseSettings#base_iter().
  RDAgentSettings.is_force_subproc: RDAgentSettings#is_force_subproc().
  RDAgentSettings.app_tpl: RDAgentSettings#app_tpl.
  RDAgentSettings.enable_mlflow: RDAgentSettings#enable_mlflow.
  RDAgentSettings.step_semaphore: RDAgentSettings#step_semaphore.
  RDAgentSettings: RDAgentSettings#
  RDAgentSettings.azure_document_intelligence_key: RDAgentSettings#azure_document_intelligence_key.
  RDAgentSettings.azure_document_intelligence_endpoint: RDAgentSettings#azure_document_intelligence_endpoint.
  RDAgentSettings.max_input_duplicate_factor_group: RDAgentSettings#max_input_duplicate_factor_group.
  RDAgentSettings.workspace_ckp_size_limit: RDAgentSettings#workspace_ckp_size_limit.
  RDAgentSettings.workspace_ckp_white_list_names: RDAgentSettings#workspace_ckp_white_list_names.
  ExtendedBaseSettings.settings_customise_sources: ExtendedBaseSettings#settings_customise_sources().
  RDAgentSettings.workspace_path: RDAgentSettings#workspace_path.
  RDAgentSettings.pickle_cache_folder_path_str: RDAgentSettings#pickle_cache_folder_path_str.
  RDAgentSettings.max_output_duplicate_factor_group: RDAgentSettings#max_output_duplicate_factor_group.
  RDAgentSettings.max_kmeans_group_number: RDAgentSettings#max_kmeans_group_number.
  RDAgentSettings.cache_with_pickle: RDAgentSettings#cache_with_pickle.
  RDAgentSettings.use_file_lock: RDAgentSettings#use_file_lock.
  RDAgentSettings.stdout_context_len: RDAgentSettings#stdout_context_len.
  RDAgentSettings.stdout_line_len: RDAgentSettings#stdout_line_len.
  RDAgentSettings.subproc_step: RDAgentSettings#subproc_step.
  RDAgentSettings.initial_fator_library_size: RDAgentSettings#initial_fator_library_size.
---
# Module: [`rdagent/core/conf.py`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py)

## Classes
### `ExtendedBaseSettings`  ·  implements/extends BaseSettings
- def: [`rdagent/core/conf.py:13`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L13) — documented in [rdagent-app-data_science-conf](../../../concepts/rdagent-app-data_science-conf.md)
- signature: `class ExtendedBaseSettings(BaseSettings):`
- members:
  - `base_iter(settings_cls: type[ExtendedBaseSettings])` — [`L25`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L25) — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
  - `settings_customise_sources(cls, settings_cls: type[BaseSettings], init_settings: PydanticBaseSettingsSource, env_settings: PydanticBaseSettingsSource, dotenv_settings: PydanticBaseSettingsSource, file_secret_settings: PydanticBaseSettingsSource)` — [`L16`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L16)
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../components/coder/CoSTEER/config.md#CoSTEERSettings), [`BasePropSetting`](../components/workflow/conf.md#BasePropSetting), [`EnvConf`](../utils/env.md#EnvConf), [`KaggleBasePropSetting`](../app/kaggle/conf.md#KaggleBasePropSetting), [`LLMSettings`](../oai/llm_conf.md#LLMSettings), [`LLMFinetunePropSetting`](../app/finetune/llm/conf.md#LLMFinetunePropSetting), [`AutoRLBenchSettings`](../scenarios/rl/autorl_bench/conf.md#AutoRLBenchSettings), [`DSFinetuneScen`](../app/finetune/data_science/conf.md#DSFinetuneScen), [`LogSettings`](../log/conf.md#LogSettings), [`RDAgentSettings`](conf.md#RDAgentSettings), [`RLPostTrainingPropSetting`](../app/rl/conf.md#RLPostTrainingPropSetting), [`UIBasePropSetting`](../log/ui/conf.md#UIBasePropSetting)  (1 test-only)
- used by: [`CoSTEERSettings`](../components/coder/CoSTEER/config.md#CoSTEERSettings), [`download_data`](../scenarios/kaggle/kaggle_crawler.md#download_data), [`BasePropSetting`](../components/workflow/conf.md#BasePropSetting), [`EnvConf`](../utils/env.md#EnvConf), [`KaggleBasePropSetting`](../app/kaggle/conf.md#KaggleBasePropSetting), [`LLMSettings`](../oai/llm_conf.md#LLMSettings), [`LLMFinetunePropSetting`](../app/finetune/llm/conf.md#LLMFinetunePropSetting), [`AutoRLBenchSettings`](../scenarios/rl/autorl_bench/conf.md#AutoRLBenchSettings), [`DSFinetuneScen`](../app/finetune/data_science/conf.md#DSFinetuneScen), [`LogSettings`](../log/conf.md#LogSettings), [`RDAgentSettings`](conf.md#RDAgentSettings), [`RLPostTrainingPropSetting`](../app/rl/conf.md#RLPostTrainingPropSetting), [`UIBasePropSetting`](../log/ui/conf.md#UIBasePropSetting)  (1 test-only)

### `RDAgentSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/core/conf.py:46`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L46) — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
- signature: `class RDAgentSettings(ExtendedBaseSettings):`
- members:
  - `get_max_parallel(self)` — [`L92`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L92) — Based on the setting of semaphore, return the maximum number of parallel loops — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
  - `is_force_subproc(self)` — [`L102`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L102)
  - `app_tpl` — [`L106`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L106)
  - `azure_document_intelligence_endpoint` — [`L50`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L50)
  - `azure_document_intelligence_key` — [`L49`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L49)
  - `cache_with_pickle` — [`L69`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L69)
  - `enable_mlflow` — [`L83`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L83)
  - `initial_fator_library_size` — [`L85`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L85)
  - `max_input_duplicate_factor_group` — [`L52`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L52)
  - `max_kmeans_group_number` — [`L54`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L54)
  - `max_output_duplicate_factor_group` — [`L53`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L53)
  - `multi_proc_n` — [`L66`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L66) — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
  - `pickle_cache_folder_path_str` — [`L70`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L70)
  - `stdout_context_len` — [`L80`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L80)
  - `stdout_line_len` — [`L81`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L81)
  - `step_semaphore` — [`L88`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L88) — --- — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
  - `subproc_step` — [`L100`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L100)
  - `use_file_lock` — [`L73`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L73) — ---
  - `workspace_ckp_size_limit` — [`L58`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L58)
  - `workspace_ckp_white_list_names` — [`L59`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L59) — ---
  - `workspace_path` — [`L57`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L57)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](conf.md#ExtendedBaseSettings)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`workspace_path`](experiment.md#FBWorkspace.workspace_path), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`RD_AGENT_SETTINGS`](conf.md#RD_AGENT_SETTINGS), [`ExtendedBaseSettings`](conf.md#ExtendedBaseSettings), [`direct_exp_gen`](../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`run`](../utils/workflow/loop.md#LoopBase.run), [`log_workflow_state`](../utils/workflow/tracking.md#WorkflowTracker.log_workflow_state), [`process_factor_data`](../scenarios/qlib/developer/utils.md#process_factor_data), [`evolve_iter`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`evaluate_iter`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator.evaluate_iter), [`direct_exp_gen`](../app/qlib_rd_loop/quant.md#QuantRDLoop.direct_exp_gen), [`direct_exp_gen`](../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`cached_run`](../utils/env.md#Env.cached_run), [`__deduplicate_factor_dict`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#__deduplicate_factor_dict), [`async_gen`](proposal.md#ExpGen.async_gen), [`load_from_documents`](../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.load_from_documents), [`kickoff_loop`](../utils/workflow/loop.md#LoopBase.kickoff_loop), [`_get_truncated_stdout`](../utils/env.md#EnvResult._get_truncated_stdout), [`execute_loop`](../utils/workflow/loop.md#LoopBase.execute_loop), [`extract_factors_from_report_dict`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#extract_factors_from_report_dict), [`mlflow`](../utils/workflow/tracking.md#mlflow), [`update_settings`](../app/finetune/data_science/conf.md#update_settings), [`create_ws_ckp`](experiment.md#FBWorkspace.create_ws_ckp), [`__init__`](../scenarios/finetune/experiment/workspace.md#FTWorkspace.__init__), [`load_content`](../utils/agent/tpl.md#load_content), [`cache_wrapper`](utils.md#cache_with_pickle.cache_decorator.cache_wrapper), [`check_factor_viability`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#check_factor_viability), [`check_factor_relevance`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#check_factor_relevance), [`load_and_process_pdfs_by_azure_document_intelligence`](../components/document_reader/document_reader.md#load_and_process_pdfs_by_azure_document_intelligence), [`get_semaphore`](../utils/workflow/loop.md#LoopBase.get_semaphore), [`deduplicate_factors_by_llm`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#deduplicate_factors_by_llm), [`is_enabled`](../utils/workflow/tracking.md#WorkflowTracker.is_enabled)  (2 test-only)

## Module values
- `RD_AGENT_SETTINGS` — [`L109`](../../../../../../raw/code/rd-agent/rdagent/core/conf.py#L109) — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)

