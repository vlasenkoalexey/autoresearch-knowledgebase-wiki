---
title: 'Module: rdagent/app/finetune/llm/conf.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.conf`/
symbols:
  FT_RD_SETTING: FT_RD_SETTING.
  LLMFinetunePropSetting.file_path: LLMFinetunePropSetting#file_path.
  LLMFinetunePropSetting.base_model: LLMFinetunePropSetting#base_model.
  LLMFinetunePropSetting.force_think_token: LLMFinetunePropSetting#force_think_token.
  LLMFinetunePropSetting: LLMFinetunePropSetting#
  LLMFinetunePropSetting.dataset: LLMFinetunePropSetting#dataset.
  LLMFinetunePropSetting.full_timeout: LLMFinetunePropSetting#full_timeout.
  LLMFinetunePropSetting.user_target_scenario: LLMFinetunePropSetting#user_target_scenario.
  LLMFinetunePropSetting.target_benchmark: LLMFinetunePropSetting#target_benchmark.
  LLMFinetunePropSetting.upper_data_size_limit: LLMFinetunePropSetting#upper_data_size_limit.
  LLMFinetunePropSetting.data_processing_timeout: LLMFinetunePropSetting#data_processing_timeout.
  LLMFinetunePropSetting.benchmark_description: LLMFinetunePropSetting#benchmark_description.
  LLMFinetunePropSetting.benchmark_timeout: LLMFinetunePropSetting#benchmark_timeout.
  LLMFinetunePropSetting.judge_api_key: LLMFinetunePropSetting#judge_api_key.
  LLMFinetunePropSetting.judge_api_base: LLMFinetunePropSetting#judge_api_base.
  LLMFinetunePropSetting.debug_data_processing_timeout: LLMFinetunePropSetting#debug_data_processing_timeout.
  LLMFinetunePropSetting.micro_batch_timeout: LLMFinetunePropSetting#micro_batch_timeout.
  LLMFinetunePropSetting.judge_model: LLMFinetunePropSetting#judge_model.
  LLMFinetunePropSetting.judge_retry: LLMFinetunePropSetting#judge_retry.
  LLMFinetunePropSetting.strong_models: LLMFinetunePropSetting#strong_models.
  LLMFinetunePropSetting.weak_models: LLMFinetunePropSetting#weak_models.
  LLMFinetunePropSetting.docker_enable_cache: LLMFinetunePropSetting#docker_enable_cache.
  LLMFinetunePropSetting.data_sample_count: LLMFinetunePropSetting#data_sample_count.
  LLMFinetunePropSetting.api_max_workers: LLMFinetunePropSetting#api_max_workers.
  LLMFinetunePropSetting.coder_max_loop: LLMFinetunePropSetting#coder_max_loop.
  LLMFinetunePropSetting.model_config: LLMFinetunePropSetting#model_config.
  LLMFinetunePropSetting.scen: LLMFinetunePropSetting#scen.
  LLMFinetunePropSetting.hypothesis_gen: LLMFinetunePropSetting#hypothesis_gen.
  LLMFinetunePropSetting.coder: LLMFinetunePropSetting#coder.
  LLMFinetunePropSetting.runner: LLMFinetunePropSetting#runner.
  LLMFinetunePropSetting.summarizer: LLMFinetunePropSetting#summarizer.
  LLMFinetunePropSetting.coder_on_whole_pipeline: LLMFinetunePropSetting#coder_on_whole_pipeline.
  LLMFinetunePropSetting.app_tpl: LLMFinetunePropSetting#app_tpl.
  LLMFinetunePropSetting.benchmark_limit: LLMFinetunePropSetting#benchmark_limit.
  LLMFinetunePropSetting.benchmark_num_runs: LLMFinetunePropSetting#benchmark_num_runs.
  LLMFinetunePropSetting.benchmark_pass_k: LLMFinetunePropSetting#benchmark_pass_k.
  LLMFinetunePropSetting.show_nan_columns: LLMFinetunePropSetting#show_nan_columns.
  LLMFinetunePropSetting.sample_data_by_LLM: LLMFinetunePropSetting#sample_data_by_LLM.
  LLMFinetunePropSetting.embedding_models: LLMFinetunePropSetting#embedding_models.
---
# Module: [`rdagent/app/finetune/llm/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py)

## Classes
### `LLMFinetunePropSetting`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/app/finetune/llm/conf.py:8`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L8) — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
- doc: LLM Fine-tune dedicated property settings.
- signature: `class LLMFinetunePropSetting(ExtendedBaseSettings):`
- members:
  - `api_max_workers` — [`L111`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L111) — ---
  - `app_tpl` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L51)
  - `base_model` — [`L90`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L90) — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `benchmark_description` — [`L89`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L89)
  - `benchmark_limit` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L71) — ---
  - `benchmark_num_runs` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L74) — ---
  - `benchmark_pass_k` — [`L77`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L77) — ---
  - `benchmark_timeout` — [`L55`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L55) — ---
  - `coder` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L24) — ---
  - `coder_max_loop` — [`L115`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L115)
  - `coder_on_whole_pipeline` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L50)
  - `data_processing_timeout` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L42) — ---
  - `data_sample_count` — [`L108`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L108)
  - `dataset` — [`L91`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L91)
  - `debug_data_processing_timeout` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L44) — ---
  - `docker_enable_cache` — [`L104`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L104) — ---
  - `embedding_models` — [`L101`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L101)
  - `file_path` — [`L81`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L81) — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `force_think_token` — [`L118`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L118) — --- — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `full_timeout` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L40) — ---
  - `hypothesis_gen` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L21) — ---
  - `judge_api_base` — [`L65`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L65) — ---
  - `judge_api_key` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L62) — ---
  - `judge_model` — [`L59`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L59) — ---
  - `judge_retry` — [`L68`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L68) — ---
  - `micro_batch_timeout` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L46) — ---
  - `model_config` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L15)
  - `runner` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L29) — ---
  - `sample_data_by_LLM` — [`L83`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L83)
  - `scen` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L18) — ---
  - `show_nan_columns` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L82)
  - `strong_models` — [`L95`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L95) — ---
  - `summarizer` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L34) — ---
  - `target_benchmark` — [`L87`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L87) — ---
  - `upper_data_size_limit` — [`L92`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L92)
  - `user_target_scenario` — [`L86`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L86)
  - `weak_models` — [`L98`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L98) — ---
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings)
- used by: [`FT_RD_SETTING`](conf.md#FT_RD_SETTING), [`_gen_hypothesis`](../../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`implement_data`](../../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`generate_feedback`](../../../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings), [`get_ft_env`](../../../components/coder/finetune/conf.md#get_ft_env), [`_generate_llamafactory_config_with_llm`](../../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`_generate_llm_feedback`](../../../components/coder/finetune/eval.md#FTDataEvaluator._generate_llm_feedback), [`get_benchmark_env`](../../../components/coder/finetune/conf.md#get_benchmark_env), [`_generate_llm_feedback`](../../../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`get_scenario_all_desc`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.get_scenario_all_desc), [`describe_dataset_folder`](../../../scenarios/finetune/scen/utils.md#FinetuneDatasetDescriptor.describe_dataset_folder), [`main`](loop.md#main), [`run_baseline_model_evaluation`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.run_baseline_model_evaluation), [`__init__`](../../../components/coder/finetune/__init__.md#LLMFinetuneCoSTEER.__init__), [`gen`](../../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen.gen), [`ensure_ft_assets_exist`](../../../scenarios/finetune/utils.md#ensure_ft_assets_exist), [`prepare`](../../../scenarios/finetune/datasets/__init__.md#prepare), [`_get_dataset_info`](../../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._get_dataset_info), [`_prepare_dataset_config`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen._prepare_dataset_config), [`_validate_and_prepare_environment`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen._validate_and_prepare_environment), [`get_data_processing_env`](../../../components/coder/finetune/conf.md#get_data_processing_env), [`describe_model`](../../../scenarios/finetune/scen/utils.md#FinetuneDatasetDescriptor.describe_model), [`base_model`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.base_model), [`cache_dir`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactoryManager.cache_dir), [`datasets`](../../../components/coder/finetune/conf.md#FTPathConfig.datasets), [`download_model`](../../../scenarios/finetune/download/hf.md#download_model), [`_get_standard_ft_volumes`](../../../components/coder/finetune/conf.md#_get_standard_ft_volumes), [`models`](../../../components/coder/finetune/conf.md#FTPathConfig.models), [`dataset`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.dataset), [`target_benchmark`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.target_benchmark), [`benchmark_description`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.benchmark_description), [`user_target_scenario`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.user_target_scenario), [`real_full_timeout`](../../../scenarios/finetune/scen/scenario.md#LLMFinetuneScen.real_full_timeout), [`model`](../../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.model), [`__init__`](../../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.__init__), [`dataset`](../../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.dataset)  (3 test-only)

## Module values
- `FT_RD_SETTING` — [`L125`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/conf.py#L125) — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)

