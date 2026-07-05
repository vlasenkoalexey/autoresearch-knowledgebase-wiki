---
title: 'Module: rdagent/components/coder/data_science/model/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/model/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.model`/
symbols:
  ModelMultiProcessEvolvingStrategy.implement_one_task: ModelMultiProcessEvolvingStrategy#implement_one_task().
  ModelCoSTEER.__init__: ModelCoSTEER#__init__().
  ModelCoSTEER: ModelCoSTEER#
  ModelMultiProcessEvolvingStrategy: ModelMultiProcessEvolvingStrategy#
  DIRNAME: DIRNAME.
  ModelMultiProcessEvolvingStrategy.assign_code_list_to_evo: ModelMultiProcessEvolvingStrategy#assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/data_science/model/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py)

## Classes
### `ModelCoSTEER`  ·  implements/extends DSCoSTEER
- def: [`rdagent/components/coder/data_science/model/__init__.py:150`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L150)
- signature: `class ModelCoSTEER(DSCoSTEER):`
- protocol/private: `__init__`[`L151`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L151)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`Scenario`](../../../../core/scenario.md#Scenario), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`CoSTEERMultiEvaluator`](../../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../CoSTEER/__init__.md#CoSTEER.__init__), [`DSCoderCoSTEERSettings`](../conf.md#DSCoderCoSTEERSettings), [`coder_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_max_loop), [`ModelGeneralCaseSpecEvaluator`](eval.md#ModelGeneralCaseSpecEvaluator), [`ModelMultiProcessEvolvingStrategy`](__init__.md#ModelMultiProcessEvolvingStrategy)
- used by: [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`develop_one_competition`](test.md#develop_one_competition), [`model_coder`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.model_coder)

### `ModelMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/data_science/model/__init__.py:30`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L30)
- signature: `class ModelMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L133`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L133) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: ModelTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L31`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L31)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`CoderError`](../../../../core/exception.md#CoderError), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`CoSTEERQueriedKnowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`name`](../../../../core/experiment.md#AbsTask.name), [`scen`](../../../../core/evolving_framework.md#EvolvingStrategy.scen), [`ModelTask`](exp.md#ModelTask), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`PythonBatchEditOut`](../../../../utils/agent/ret.md#PythonBatchEditOut), [`get_codes`](../../../../core/experiment.md#FBWorkspace.get_codes), [`get_spec`](../../../../utils/agent/ret.md#PythonBatchEditOut.get_spec), [`get_task_information`](exp.md#ModelTask.get_task_information), [`extract_output`](../../../../utils/agent/ret.md#PythonBatchEditOut.extract_output), [`DIRNAME`](__init__.md#DIRNAME)
- used by: [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#ModelCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/__init__.py#L27)

