---
title: 'Module: rdagent/components/coder/finetune/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/finetune/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.finetune`/
symbols:
  LLMFinetuneEvolvingStrategy.implement_data: LLMFinetuneEvolvingStrategy#implement_data().
  LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm: LLMFinetuneEvolvingStrategy#_generate_llamafactory_config_with_llm().
  LLMFinetuneEvolvingStrategy.implement_lf_config: LLMFinetuneEvolvingStrategy#implement_lf_config().
  LLMFinetuneCoSTEER.__init__: LLMFinetuneCoSTEER#__init__().
  LLMFinetuneEvolvingStrategy._get_dataset_info: LLMFinetuneEvolvingStrategy#_get_dataset_info().
  LLMFinetuneEvolvingStrategy.llama_factory_manager: LLMFinetuneEvolvingStrategy#llama_factory_manager.
  LLMFinetuneEvolvingStrategy.__init__: LLMFinetuneEvolvingStrategy#__init__().
  LLMFinetuneEvolvingStrategy.implement_func_list: LLMFinetuneEvolvingStrategy#implement_func_list().
  LLMFinetuneCoSTEER: LLMFinetuneCoSTEER#
  LLMFinetuneEvolvingStrategy: LLMFinetuneEvolvingStrategy#
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/finetune/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py)

## Classes
### `LLMFinetuneCoSTEER`  ·  implements/extends CoSTEER
- def: [`rdagent/components/coder/finetune/__init__.py:368`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L368)
- doc: LLM Fine-tuning CoSTEER implementation
- signature: `class LLMFinetuneCoSTEER(CoSTEER):`
- protocol/private: `__init__`[`L371`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L371)
- uses (calls/refs, reference-scoped): [`Scenario`](../../../core/scenario.md#Scenario), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER), [`CoSTEERMultiEvaluator`](../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../CoSTEER/__init__.md#CoSTEER.__init__), [`FTCoderCoSTEERSettings`](conf.md#FTCoderCoSTEERSettings), [`FTDataEvaluator`](eval.md#FTDataEvaluator), [`FTCoderEvaluator`](eval.md#FTCoderEvaluator), [`LLMFinetuneEvolvingStrategy`](__init__.md#LLMFinetuneEvolvingStrategy), [`coder_max_loop`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.coder_max_loop)
- used by: [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER)  (1 test-only)

### `LLMFinetuneEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/finetune/__init__.py:45`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L45)
- doc: LLM Fine-tuning specific evolving strategy
- signature: `class LLMFinetuneEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `_generate_llamafactory_config_with_llm(self, base_model: str, task_info: str = "", queried_former_failed_knowledge: tuple = None, prev_feedback=None, workspace=None)` — [`L288`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L288) — Generate LlamaFactory configuration YAML using LLM — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `_get_dataset_info(self, involving_datasets: list[str], datasets_path: str = None)` — [`L153`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L153) — Read dataset_info.json and return information for specified datasets.
  - `implement_data(self, target_task: Task, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L55`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L55) — Generate data processing script based on task. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `implement_func_list(self)` — [`L52`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L52)
  - `implement_lf_config(self, target_task: Task, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L245`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L245) — Implement a single fine-tuning task by generating LlamaFactory config
  - `llama_factory_manager` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L50)
- protocol/private: `__init__`[`L48`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L48)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`Scenario`](../../../core/scenario.md#Scenario), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Task`](../../../core/experiment.md#Task), [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`error`](../../../log/logger.md#RDAgentLog.error), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`build_chat_completion`](../../../oai/backend/base.md#ChatSession.build_chat_completion), [`CoSTEERQueriedKnowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`describe_dataset_folder`](../../../scenarios/finetune/scen/utils.md#FinetuneDatasetDescriptor.describe_dataset_folder), [`FT_YAML_FILE_NAME`](conf.md#FT_YAML_FILE_NAME), [`file_path`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.file_path), [`scen`](../../../core/evolving_framework.md#EvolvingStrategy.scen), [`build_chat_session`](../../../oai/backend/base.md#APIBackend.build_chat_session), [`FT_PATHS`](conf.md#FT_PATHS), [`FT_DATA_SCRIPT_NAME`](conf.md#FT_DATA_SCRIPT_NAME), [`datasets`](conf.md#FTPathConfig.datasets), [`LLaMAFactory_manager`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactory_manager), [`models`](conf.md#FTPathConfig.models), [`__init__`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.__init__), [`format_method_specific_params`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactoryManager.format_method_specific_params), [`format_shared_params`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactoryManager.format_shared_params), [`source_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.source_feedback), [`workspace`](conf.md#FTPathConfig.workspace), [`force_think_token`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.force_think_token), [`methods`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactoryManager.methods), [`FinetuneDatasetDescriptor`](../../../scenarios/finetune/scen/utils.md#FinetuneDatasetDescriptor), [`FT_TEST_PARAMS_FILE_NAME`](conf.md#FT_TEST_PARAMS_FILE_NAME), [`deepspeed`](conf.md#FTPathConfig.deepspeed), [`api_max_workers`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.api_max_workers)
- used by: [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`__init__`](__init__.md#LLMFinetuneCoSTEER.__init__), [`implement_func_list`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_func_list)

## Module values
- `DIRNAME` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/__init__.py#L42)

