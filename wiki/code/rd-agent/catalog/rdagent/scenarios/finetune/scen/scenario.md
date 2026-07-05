---
title: 'Module: rdagent/scenarios/finetune/scen/scenario.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/scen/scenario.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.scen.scenario`/LLMFinetuneScen#
symbols:
  LLMFinetuneScen.get_scenario_all_desc: get_scenario_all_desc().
  LLMFinetuneScen.run_baseline_model_evaluation: run_baseline_model_evaluation().
  LLMFinetuneScen._generate_memory_report: _generate_memory_report().
  LLMFinetuneScen._llm_select_datasets: _llm_select_datasets().
  LLMFinetuneScen._validate_and_prepare_environment: _validate_and_prepare_environment().
  LLMFinetuneScen._select_relevant_datasets: _select_relevant_datasets().
  LLMFinetuneScen._prepare_dataset_config: _prepare_dataset_config().
  LLMFinetuneScen.base_model: base_model.
  LLMFinetuneScen.memory_report: memory_report.
  LLMFinetuneScen._initialize_llama_factory: _initialize_llama_factory().
  LLMFinetuneScen.device_info: device_info.
  LLMFinetuneScen.model_info: model_info.
  LLMFinetuneScen.dataset: dataset.
  LLMFinetuneScen: ''
  LLMFinetuneScen.dataset_config: dataset_config.
  LLMFinetuneScen.selected_datasets: selected_datasets.
  LLMFinetuneScen.target_benchmark: target_benchmark.
  LLMFinetuneScen.user_target_scenario: user_target_scenario.
  LLMFinetuneScen.benchmark_description: benchmark_description.
  LLMFinetuneScen.real_full_timeout: real_full_timeout().
  LLMFinetuneScen.__init__: __init__().
  LLMFinetuneScen.gpu_count: gpu_count.
  LLMFinetuneScen.benchmark_hash: benchmark_hash().
  LLMFinetuneScen.timeout_increase_count: timeout_increase_count.
  LLMFinetuneScen.baseline_benchmark_score: baseline_benchmark_score.
  LLMFinetuneScen.baseline_benchmark_score_test: baseline_benchmark_score_test.
  LLMFinetuneScen.metric_direction: metric_direction().
---
# Module: [`rdagent/scenarios/finetune/scen/scenario.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py)

## Classes
### `LLMFinetuneScen`  ·  implements/extends DataScienceScen
- def: [`rdagent/scenarios/finetune/scen/scenario.py:26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L26)
- doc: LLMFinetuneScen Scenario
- signature: `class LLMFinetuneScen(DataScienceScen):`
- members:
  - `__init__(self)` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L29) — Initialize LLM finetune scenario using configuration from FT_RD_SETTING.
  - `_generate_memory_report(self)` — [`L115`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L115) — Generate memory estimation report based on hardware and model.
  - `_initialize_llama_factory(self)` — [`L164`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L164) — Initialize LLaMA Factory information manager
  - `_llm_select_datasets(self)` — [`L201`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L201) — Use LLM to select relevant datasets.
  - `_prepare_dataset_config(self)` — [`L231`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L231) — Generate dataset_info.json configuration.
  - `_select_relevant_datasets(self)` — [`L175`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L175) — Select relevant datasets based on user target scenario using LLM.
  - `_validate_and_prepare_environment(self)` — [`L150`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L150) — Validate FT_FILE_PATH and prepare all registered datasets
  - `benchmark_hash(self, model_name, benchmark_name)` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L74)
  - `get_scenario_all_desc(self, enable_dataset_description: bool = False)` — [`L284`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L284) — Get complete scenario description for LLM fine-tuning.
  - `metric_direction(self)` — [`L280`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L280) — Metric direction for LLM fine-tuning (higher is better)
  - `real_full_timeout(self)` — [`L112`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L112)
  - `run_baseline_model_evaluation(self, model_name, benchmark_name)` — [`L78`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L78) — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `base_model` — [`L38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L38)
  - `baseline_benchmark_score` — [`L70`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L70)
  - `baseline_benchmark_score_test` — [`L72`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L72)
  - `benchmark_description` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L36)
  - `dataset` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L37)
  - `dataset_config` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L47)
  - `device_info` — [`L59`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L59)
  - `gpu_count` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L60)
  - `memory_report` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L64)
  - `model_info` — [`L61`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L61)
  - `selected_datasets` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L50)
  - `target_benchmark` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L35)
  - `timeout_increase_count` — [`L56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L56)
  - `user_target_scenario` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/scenario.py#L34)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`get_ft_env`](../../../components/coder/finetune/conf.md#get_ft_env), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`file_path`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.file_path), [`get_runtime_environment_by_env`](../../shared/get_runtime_info.md#get_runtime_environment_by_env), [`DataScienceScen`](../../data_science/scen/__init__.md#DataScienceScen), [`ensure_ft_assets_exist`](../utils.md#ensure_ft_assets_exist), [`describe_model`](utils.md#FinetuneDatasetDescriptor.describe_model), [`format`](memory_estimator.md#MemoryEstimator.format), [`generate_dataset_info_config`](utils.md#generate_dataset_info_config), [`LLaMAFactory_manager`](llama_factory_manager.md#LLaMAFactory_manager), [`get_info`](llama_factory_manager.md#LLaMAFactoryManager.get_info), [`base_model`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.base_model), [`FTWorkspace`](../experiment/workspace.md#FTWorkspace), [`prepare_all`](../datasets/__init__.md#prepare_all), [`FinetuneDatasetDescriptor`](utils.md#FinetuneDatasetDescriptor), [`dataset`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.dataset), [`full_timeout`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.full_timeout), [`target_benchmark`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.target_benchmark), [`upper_data_size_limit`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.upper_data_size_limit), [`user_target_scenario`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.user_target_scenario), [`from_model_name`](memory_estimator.md#MemoryEstimator.from_model_name), [`MemoryEstimator`](memory_estimator.md#MemoryEstimator), [`benchmark_description`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.benchmark_description), [`data_processing_timeout`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.data_processing_timeout)  (2 test-only)
- used by: [`get_scenario_all_desc`](../../data_science/scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`real_full_timeout`](../../data_science/scen/__init__.md#DataScienceScen.real_full_timeout), [`DataScienceScen`](../../data_science/scen/__init__.md#DataScienceScen), [`__init__`](../proposal/trace.md#FTTrace.__init__), [`__init__`](../proposal/proposal.md#LLMFinetuneExpGen.__init__)  (1 test-only)

