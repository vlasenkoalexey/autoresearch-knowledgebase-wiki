---
title: 'Module: rdagent/components/coder/data_science/pipeline/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/pipeline/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.pipeline`/
symbols:
  PipelineMultiProcessEvolvingStrategy.implement_one_task: PipelineMultiProcessEvolvingStrategy#implement_one_task().
  PipelineCoSTEER.__init__: PipelineCoSTEER#__init__().
  PipelineCoSTEER: PipelineCoSTEER#
  PipelineMultiProcessEvolvingStrategy: PipelineMultiProcessEvolvingStrategy#
  DIRNAME: DIRNAME.
  PipelineMultiProcessEvolvingStrategy.assign_code_list_to_evo: PipelineMultiProcessEvolvingStrategy#assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/data_science/pipeline/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py)

## Classes
### `PipelineCoSTEER`  ·  implements/extends DSCoSTEER
- def: [`rdagent/components/coder/data_science/pipeline/__init__.py:133`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L133)
- signature: `class PipelineCoSTEER(DSCoSTEER):`
- protocol/private: `__init__`[`L134`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L134)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`Scenario`](../../../../core/scenario.md#Scenario), [`import_class`](../../../../core/utils.md#import_class), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`CoSTEERMultiEvaluator`](../../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../CoSTEER/__init__.md#CoSTEER.__init__), [`DSCoderCoSTEERSettings`](../conf.md#DSCoderCoSTEERSettings), [`ModelDumpEvaluator`](../share/eval.md#ModelDumpEvaluator), [`coder_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_max_loop), [`PipelineCoSTEEREvaluator`](eval.md#PipelineCoSTEEREvaluator), [`enable_model_dump`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_model_dump), [`PipelineMultiProcessEvolvingStrategy`](__init__.md#PipelineMultiProcessEvolvingStrategy), [`extra_eval`](../conf.md#DSCoderCoSTEERSettings.extra_eval), [`extra_evaluator`](../conf.md#DSCoderCoSTEERSettings.extra_evaluator)
- used by: [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`pipeline_coder`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.pipeline_coder)

### `PipelineMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/data_science/pipeline/__init__.py:54`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L54)
- signature: `class PipelineMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L116) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: PipelineTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L55`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L55) — documented in [rdagent-app-data_science-conf](../../../../../../concepts/rdagent-app-data_science-conf.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`CoderError`](../../../../core/exception.md#CoderError), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`CoSTEERQueriedKnowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`PythonAgentOut`](../../../../utils/agent/ret.md#PythonAgentOut), [`get_runtime_environment`](../../../../core/scenario.md#Scenario.get_runtime_environment), [`scen`](../../../../core/evolving_framework.md#EvolvingStrategy.scen), [`PipelineTask`](exp.md#PipelineTask), [`get_spec`](../../../../utils/agent/ret.md#PythonAgentOut.get_spec), [`sample_data_by_LLM`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.sample_data_by_LLM), [`extract_output`](../../../../utils/agent/ret.md#PythonAgentOut.extract_output), [`enable_notebook_conversion`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_notebook_conversion), [`enable_model_dump`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_model_dump), [`package_info`](exp.md#PipelineTask.package_info)
- used by: [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`__init__`](__init__.md#PipelineCoSTEER.__init__), [`assign_code_list_to_evo`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo)

## Module values
- `DIRNAME` — [`L51`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/__init__.py#L51)

