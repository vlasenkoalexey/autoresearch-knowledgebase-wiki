---
title: 'Module: rdagent/components/coder/data_science/workflow/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/workflow/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.workflow`/Workflow
symbols:
  WorkflowMultiProcessEvolvingStrategy.implement_one_task: MultiProcessEvolvingStrategy#implement_one_task().
  WorkflowCoSTEER.__init__: CoSTEER#__init__().
  WorkflowCoSTEER: CoSTEER#
  WorkflowMultiProcessEvolvingStrategy: MultiProcessEvolvingStrategy#
  WorkflowMultiProcessEvolvingStrategy.assign_code_list_to_evo: MultiProcessEvolvingStrategy#assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/data_science/workflow/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py)

## Classes
### `WorkflowCoSTEER`  ·  implements/extends DSCoSTEER
- def: [`rdagent/components/coder/data_science/workflow/__init__.py:111`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py#L111)
- signature: `class WorkflowCoSTEER(DSCoSTEER):`
- protocol/private: `__init__`[`L112`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py#L112)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`Scenario`](../../../../core/scenario.md#Scenario), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`CoSTEERMultiEvaluator`](../../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../CoSTEER/__init__.md#CoSTEER.__init__), [`DSCoderCoSTEERSettings`](../conf.md#DSCoderCoSTEERSettings), [`coder_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_max_loop), [`WorkflowGeneralCaseSpecEvaluator`](eval.md#WorkflowGeneralCaseSpecEvaluator), [`WorkflowMultiProcessEvolvingStrategy`](__init__.md#WorkflowMultiProcessEvolvingStrategy)
- used by: [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`develop_one_competition`](test.md#develop_one_competition), [`workflow_coder`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.workflow_coder)

### `WorkflowMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/data_science/workflow/__init__.py:26`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py#L26)
- signature: `class WorkflowMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L94`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py#L94) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: WorkflowTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/__init__.py#L27)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`CoderError`](../../../../core/exception.md#CoderError), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`CoSTEERQueriedKnowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`PythonAgentOut`](../../../../utils/agent/ret.md#PythonAgentOut), [`scen`](../../../../core/evolving_framework.md#EvolvingStrategy.scen), [`WorkflowTask`](exp.md#WorkflowTask), [`get_spec`](../../../../utils/agent/ret.md#PythonAgentOut.get_spec), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`extract_output`](../../../../utils/agent/ret.md#PythonAgentOut.extract_output), [`get_codes`](../../../../core/experiment.md#FBWorkspace.get_codes)
- used by: [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#WorkflowCoSTEER.__init__)

