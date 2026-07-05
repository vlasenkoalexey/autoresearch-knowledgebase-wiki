---
title: 'Module: rdagent/scenarios/data_science/scen/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/scen/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.scen`/
symbols:
  DataScienceScen.get_scenario_all_desc: DataScienceScen#get_scenario_all_desc().
  DataScienceScen.real_full_timeout: DataScienceScen#real_full_timeout().
  DataScienceScen.get_competition_full_desc: DataScienceScen#get_competition_full_desc().
  DataScienceScen.background: DataScienceScen#background().
  DataScienceScen: DataScienceScen#
  DataScienceScen._get_description: DataScienceScen#_get_description().
  DataScienceScen.__init__: DataScienceScen#__init__().
  DataScienceScen.reanalyze_competition_description: DataScienceScen#reanalyze_competition_description().
  DataScienceScen._analysis_competition_description: DataScienceScen#_analysis_competition_description().
  DataScienceScen._get_data_folder_description: DataScienceScen#_get_data_folder_description().
  DataScienceScen.real_debug_timeout: DataScienceScen#real_debug_timeout().
  DataScienceScen.competition: DataScienceScen#competition.
  KaggleScen: KaggleScen#
  DataScienceScen.rich_style_description: DataScienceScen#rich_style_description().
  KaggleScen._get_description: KaggleScen#_get_description().
  DataScienceScen.coder_longer_time_limit_required: DataScienceScen#coder_longer_time_limit_required.
  DataScienceScen.runner_longer_time_limit_required: DataScienceScen#runner_longer_time_limit_required.
  DataScienceScen.debug_path: DataScienceScen#debug_path.
  KaggleScen.__init__: KaggleScen#__init__().
  KaggleScen.rich_style_description: KaggleScen#rich_style_description().
  DataScienceScen.processed_data_folder_description: DataScienceScen#processed_data_folder_description.
  DataScienceScen._get_direction: DataScienceScen#_get_direction().
  DataScienceScen.get_runtime_environment: DataScienceScen#get_runtime_environment().
  DataScienceScen.raw_description: DataScienceScen#raw_description.
  DataScienceScen.metric_direction_guess: DataScienceScen#metric_direction_guess.
  DataScienceScen.recommend_debug_timeout: DataScienceScen#recommend_debug_timeout().
  DataScienceScen.recommend_full_timeout: DataScienceScen#recommend_full_timeout().
  DataScienceScen.metric_direction: DataScienceScen#metric_direction.
  DataScienceScen.metric_description: DataScienceScen#metric_description.
  DataScienceScen.timeout_increase_count: DataScienceScen#timeout_increase_count.
  KaggleScen._get_direction: KaggleScen#_get_direction().
  DataScienceScen.increase_timeout: DataScienceScen#increase_timeout().
  DataScienceScen.metric_name: DataScienceScen#metric_name.
  DataScienceScen.submission_specifications: DataScienceScen#submission_specifications.
  DataScienceScen.task_type: DataScienceScen#task_type.
  DataScienceScen.data_type: DataScienceScen#data_type.
  DataScienceScen.brief_description: DataScienceScen#brief_description.
  DataScienceScen.dataset_description: DataScienceScen#dataset_description.
  DataScienceScen.model_output_channel: DataScienceScen#model_output_channel.
---
# Module: [`rdagent/scenarios/data_science/scen/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py)

## Classes
### `DataScienceScen`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/data_science/scen/__init__.py:27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L27) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
- doc: Data Science Scenario
- signature: `class DataScienceScen(Scenario):`
- members:
  - `background(self)` — [`L184`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L184)
  - `get_competition_full_desc(self)` — [`L203`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L203)
  - `get_runtime_environment(self)` — [`L246`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L246) — Return runtime environment information.
  - `get_scenario_all_desc(self, eda_output=None)` — [`L220`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L220) — eda_output depends on dynamic .md files from current workspace, not fixed. — documented in [rdagent-app-data_science-conf](../../../../../concepts/rdagent-app-data_science-conf.md)
  - `increase_timeout(self)` — [`L179`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L179) — Increase the timeout multiplier for the scenario.
  - `real_debug_timeout(self)` — [`L141`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L141)
  - `real_full_timeout(self)` — [`L155`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L155) — documented in [rdagent-app-data_science-conf](../../../../../concepts/rdagent-app-data_science-conf.md)
  - `reanalyze_competition_description(self)` — [`L70`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L70)
  - `recommend_debug_timeout(self)` — [`L152`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L152)
  - `recommend_full_timeout(self)` — [`L176`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L176)
  - `rich_style_description(self)` — [`L197`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L197)
  - `brief_description` — [`L109`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L109)
  - `coder_longer_time_limit_required` — [`L127`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L127)
  - `competition` — [`L61`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L61)
  - `data_type` — [`L108`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L108)
  - `dataset_description` — [`L110`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L110)
  - `debug_path` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L40)
  - `metric_description` — [`L115`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L115)
  - `metric_direction` — [`L65`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L65)
  - `metric_direction_guess` — [`L119`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L119)
  - `metric_name` — [`L57`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L57)
  - `model_output_channel` — [`L114`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L114)
  - `processed_data_folder_description` — [`L63`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L63)
  - `raw_description` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L62)
  - `runner_longer_time_limit_required` — [`L133`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L133)
  - `submission_specifications` — [`L111`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L111)
  - `task_type` — [`L107`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L107)
  - `timeout_increase_count` — [`L68`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L68)
- protocol/private: `__init__`[`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L30), `_analysis_competition_description`[`L92`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L92), `_get_data_folder_description`[`L253`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L253), `_get_description`[`L76`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L76), `_get_direction`[`L89`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L89)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`Scenario`](../../../core/scenario.md#Scenario), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`get_ds_env`](../../../components/coder/data_science/conf.md#get_ds_env), [`error`](../../../log/logger.md#RDAgentLog.error), [`RD_Agent_TIMER_wrapper`](../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`get_scenario_all_desc`](../../finetune/scen/scenario.md#LLMFinetuneScen.get_scenario_all_desc), [`local_data_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`remain_time`](../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../log/timer.md#RDAgentTimerWrapper.timer), [`get_runtime_environment_by_env`](../../shared/get_runtime_info.md#get_runtime_environment_by_env), [`all_duration`](../../../log/timer.md#RDAgentTimer.all_duration), [`KaggleScen`](__init__.md#KaggleScen), [`_get_data_folder_description`](../../../app/finetune/data_science/scen.md#DSFinetuneScen._get_data_folder_description), [`sample_data_by_LLM`](../../../app/data_science/conf.md#DataScienceBasePropSetting.sample_data_by_LLM), [`_get_description`](__init__.md#KaggleScen._get_description), [`describe_data_folder_v2`](utils.md#describe_data_folder_v2), [`check_runtime_environment`](../../shared/get_runtime_info.md#check_runtime_environment), [`LLMFinetuneScen`](../../finetune/scen/scenario.md#LLMFinetuneScen), [`create_debug_data`](../debug/data.md#create_debug_data), [`rich_style_description`](__init__.md#KaggleScen.rich_style_description), [`full_timeout`](../../../app/data_science/conf.md#DataScienceBasePropSetting.full_timeout), [`real_full_timeout`](../../finetune/scen/scenario.md#LLMFinetuneScen.real_full_timeout), [`_get_direction`](__init__.md#KaggleScen._get_direction), [`allow_longer_timeout`](../../../app/data_science/conf.md#DataScienceBasePropSetting.allow_longer_timeout), [`debug_timeout`](../../../app/data_science/conf.md#DataScienceBasePropSetting.debug_timeout), [`DSFinetuneScen`](../../../app/finetune/data_science/scen.md#DSFinetuneScen), [`ratio_merge_or_ensemble`](../../../app/data_science/conf.md#DataScienceBasePropSetting.ratio_merge_or_ensemble), [`runner_longer_timeout_multiplier_upper`](../../../app/data_science/conf.md#DataScienceBasePropSetting.runner_longer_timeout_multiplier_upper), [`show_hard_limit`](../../../app/data_science/conf.md#DataScienceBasePropSetting.show_hard_limit), [`show_nan_columns`](../../../app/data_science/conf.md#DataScienceBasePropSetting.show_nan_columns), [`use_raw_description`](../../../app/data_science/conf.md#DataScienceBasePropSetting.use_raw_description), [`coder_enable_llm_decide_longer_timeout`](../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_enable_llm_decide_longer_timeout), [`coder_longer_timeout_multiplier_upper`](../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_longer_timeout_multiplier_upper), [`coder_timeout_increase_stage`](../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_timeout_increase_stage)  (+6 more)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`record`](../loop.md#DataScienceRDLoop.record), [`hypothesis_select_with_llm`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`gen`](../proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`gen`](../proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`DSTrace`](../proposal/exp_gen/base.md#DSTrace), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`gen`](../proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen), [`gen`](../proposal/exp_gen/naive.md#NaiveExpGen.gen), [`observe_feedback`](../proposal/exp_gen/trace_scheduler.md#MCTSScheduler.observe_feedback), [`develop_one_competition`](../../../components/coder/data_science/feature/test.md#develop_one_competition), [`get_runtime_environment`](../../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../../core/scenario.md#Scenario.background), [`rich_style_description`](../../../core/scenario.md#Scenario.rich_style_description), [`KaggleScen`](__init__.md#KaggleScen), [`_get_data_folder_description`](../../../app/finetune/data_science/scen.md#DSFinetuneScen._get_data_folder_description), [`_get_description`](__init__.md#KaggleScen._get_description), [`LLMFinetuneScen`](../../finetune/scen/scenario.md#LLMFinetuneScen), [`__init__`](../proposal/exp_gen/base.md#DSTrace.__init__), [`__init__`](__init__.md#KaggleScen.__init__), [`rich_style_description`](__init__.md#KaggleScen.rich_style_description), [`_get_direction`](__init__.md#KaggleScen._get_direction), [`DSFinetuneScen`](../../../app/finetune/data_science/scen.md#DSFinetuneScen)

### `KaggleScen`  ·  implements/extends DataScienceScen
- def: [`rdagent/scenarios/data_science/scen/__init__.py:259`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L259)
- doc: Kaggle Scenario
- signature: `class KaggleScen(DataScienceScen):`
- members:
  - `rich_style_description(self)` — [`L279`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L279)
- protocol/private: `__init__`[`L268`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L268), `_get_description`[`L272`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L272), `_get_direction`[`L275`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/__init__.py#L275)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../app/data_science/conf.md#DS_RD_SETTING), [`download_data`](../../kaggle/kaggle_crawler.md#download_data), [`local_data_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`DataScienceScen`](__init__.md#DataScienceScen), [`__init__`](__init__.md#DataScienceScen.__init__), [`get_metric_direction`](../../kaggle/kaggle_crawler.md#get_metric_direction), [`competition`](__init__.md#DataScienceScen.competition), [`crawl_descriptions`](../../kaggle/kaggle_crawler.md#crawl_descriptions)
- used by: [`develop_one_competition`](../../../components/coder/data_science/model/test.md#develop_one_competition), [`develop_one_competition`](../../../components/coder/data_science/workflow/test.md#develop_one_competition), [`develop_one_competition`](../../../components/coder/data_science/ensemble/test.md#develop_one_competition), [`develop_one_competition`](../../../components/coder/data_science/feature/test.md#develop_one_competition), [`DataScienceScen`](__init__.md#DataScienceScen), [`_get_description`](__init__.md#DataScienceScen._get_description), [`develop_one_competition`](../../../components/coder/data_science/raw_data_loader/test.md#develop_one_competition), [`rich_style_description`](__init__.md#DataScienceScen.rich_style_description), [`_get_direction`](__init__.md#DataScienceScen._get_direction)

