---
title: 'Module: rdagent/components/coder/data_science/raw_data_loader/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/raw_data_loader/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.raw_data_loader`/D
symbols:
  DataLoaderMultiProcessEvolvingStrategy.implement_one_task: ataLoaderMultiProcessEvolvingStrategy#implement_one_task().
  DataLoaderCoSTEER.develop: ataLoaderCoSTEER#develop().
  DataLoaderCoSTEER.__init__: ataLoaderCoSTEER#__init__().
  DataLoaderCoSTEER: ataLoaderCoSTEER#
  DataLoaderMultiProcessEvolvingStrategy: ataLoaderMultiProcessEvolvingStrategy#
  DIRNAME: IRNAME.
  DataLoaderMultiProcessEvolvingStrategy.assign_code_list_to_evo: ataLoaderMultiProcessEvolvingStrategy#assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/data_science/raw_data_loader/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py)

## Classes
### `DataLoaderCoSTEER`  ·  implements/extends DSCoSTEER
- def: [`rdagent/components/coder/data_science/raw_data_loader/__init__.py:198`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L198)
- signature: `class DataLoaderCoSTEER(DSCoSTEER):`
- members:
  - `develop(self, exp)` — [`L222`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L222)
- protocol/private: `__init__`[`L199`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L199)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../../core/scenario.md#Scenario), [`get_ds_env`](../conf.md#get_ds_env), [`develop`](../../CoSTEER/__init__.md#CoSTEER.develop), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`local_data_path`](../../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`CoSTEERMultiEvaluator`](../../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../CoSTEER/__init__.md#CoSTEER.__init__), [`DSCoderCoSTEERSettings`](../conf.md#DSCoderCoSTEERSettings), [`scen`](../../../../core/developer.md#Developer.scen), [`coder_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_max_loop), [`DataLoaderCoSTEEREvaluator`](eval.md#DataLoaderCoSTEEREvaluator), [`DataLoaderMultiProcessEvolvingStrategy`](__init__.md#DataLoaderMultiProcessEvolvingStrategy)
- used by: [`coding`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.coding), [`develop`](../../CoSTEER/__init__.md#CoSTEER.develop), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`develop_one_competition`](test.md#develop_one_competition), [`data_loader_coder`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.data_loader_coder)

### `DataLoaderMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/data_science/raw_data_loader/__init__.py:58`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L58)
- signature: `class DataLoaderMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L181`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L181) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: DataLoaderTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L59`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L59)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`CoderError`](../../../../core/exception.md#CoderError), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`build_chat_completion`](../../../../oai/backend/base.md#ChatSession.build_chat_completion), [`CoSTEERQueriedKnowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`PythonAgentOut`](../../../../utils/agent/ret.md#PythonAgentOut), [`get_runtime_environment`](../../../../core/scenario.md#Scenario.get_runtime_environment), [`scen`](../../../../core/evolving_framework.md#EvolvingStrategy.scen), [`build_chat_session`](../../../../oai/backend/base.md#APIBackend.build_chat_session), [`DataLoaderTask`](exp.md#DataLoaderTask), [`get_spec`](../../../../utils/agent/ret.md#PythonAgentOut.get_spec), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`extract_output`](../../../../utils/agent/ret.md#PythonAgentOut.extract_output), [`DIRNAME`](__init__.md#DIRNAME)
- used by: [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#DataLoaderCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L55`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/__init__.py#L55)

