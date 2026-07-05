---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.draft.draft`/DSDraft
symbols:
  DSDraftExpGen.gen: ExpGen#gen().
  DSDraftV2ExpGen.gen: V2ExpGen#gen().
  DSDraftV2ExpGen.task_gen: V2ExpGen#task_gen().
  DSDraftExpGen._init_task_gen: ExpGen#_init_task_gen().
  DSDraftV2ExpGen.hypothesis_gen: V2ExpGen#hypothesis_gen().
  DSDraftV2ExpGen.knowledge_gen: V2ExpGen#knowledge_gen().
  DSDraftV2ExpGen.tag_gen: V2ExpGen#tag_gen().
  DSDraftV2ExpGen.supports_response_schema: V2ExpGen#supports_response_schema.
  DSDraftExpGen: ExpGen#
  DSDraftV2ExpGen: V2ExpGen#
  DSDraftV2ExpGen.__init__: V2ExpGen#__init__().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py)

## Classes
### `DSDraftExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py:26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L26)
- signature: `class DSDraftExpGen(ExpGen):`
- members:
  - `gen(self, component: COMPONENT, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L61) — Handle any component using a unified approach. — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
- protocol/private: `_init_task_gen`[`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L27)
- uses (calls/refs, reference-scoped): [`T`](../../../../../utils/agent/tpl.md#T), [`r`](../../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Hypothesis`](../../../../../core/proposal.md#Hypothesis), [`DSTrace`](../base.md#DSTrace), [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`get_scenario_all_desc`](../../../scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`scen`](../../../../../core/proposal.md#Trace.scen), [`DSHypothesis`](../base.md#DSHypothesis), [`DSExperimentPlan`](../planner/__init__.md#DSExperimentPlan), [`retrieve_search_list`](../base.md#DSTrace.retrieve_search_list), [`WorkflowTask`](../../../../../components/coder/data_science/workflow/exp.md#WorkflowTask), [`DataLoaderTask`](../../../../../components/coder/data_science/raw_data_loader/exp.md#DataLoaderTask), [`EnsembleTask`](../../../../../components/coder/data_science/ensemble/exp.md#EnsembleTask), [`FeatureTask`](../../../../../components/coder/data_science/feature/exp.md#FeatureTask), [`ModelTask`](../../../../../components/coder/data_science/model/exp.md#ModelTask), [`inject_code_from_file_dict`](../../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict), [`pending_tasks_list`](../../../experiment/experiment.md#DSExperiment.pending_tasks_list), [`spec_enabled`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`last_successful_exp`](../base.md#DSTrace.last_successful_exp), [`COMPONENT`](../../../experiment/experiment.md#COMPONENT), [`enable_notebook_conversion`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_notebook_conversion), [`exception`](../../../../../core/proposal.md#ExperimentFeedback.exception)
- used by: [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`gen`](../../../../../core/proposal.md#ExpGen.gen), [`draft_exp_in_decomposition`](../proposal.md#draft_exp_in_decomposition)

### `DSDraftV2ExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py:132`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L132)
- signature: `class DSDraftV2ExpGen(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L241`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L241) — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
  - `hypothesis_gen(self, knowledge: str, component_desc: str, scenario_desc: str, failed_exp_feedback_list_desc: str)` — [`L157`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L157)
  - `knowledge_gen(self)` — [`L150`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L150)
  - `tag_gen(self, scenario_desc: str)` — [`L137`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L137)
  - `task_gen(self, component_desc: str, scenario_desc: str, hypothesis: DSHypothesis, pipeline: bool, knowledge: str, failed_exp_feedback_list_desc: str)` — [`L183`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L183)
  - `supports_response_schema` — [`L135`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L135)
- protocol/private: `__init__`[`L133`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/draft/draft.py#L133)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../../utils/agent/tpl.md#T), [`r`](../../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`DSTrace`](../base.md#DSTrace), [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`get_scenario_all_desc`](../../../scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`scen`](../../../../../core/proposal.md#Trace.scen), [`DSHypothesis`](../base.md#DSHypothesis), [`experiment_and_feedback_list_after_init`](../base.md#DSTrace.experiment_and_feedback_list_after_init), [`DSExperimentPlan`](../planner/__init__.md#DSExperimentPlan), [`scen`](../../../../../core/proposal.md#ExpGen.scen), [`get_runtime_environment`](../../../../../core/scenario.md#Scenario.get_runtime_environment), [`WorkflowTask`](../../../../../components/coder/data_science/workflow/exp.md#WorkflowTask), [`coder_on_whole_pipeline`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`component`](../base.md#DSHypothesis.component), [`__init__`](../../../../../core/proposal.md#ExpGen.__init__), [`get_component`](../utils.md#get_component), [`pending_tasks_list`](../../../experiment/experiment.md#DSExperiment.pending_tasks_list), [`supports_response_schema`](../../../../../oai/backend/base.md#APIBackend.supports_response_schema), [`template`](../../../../../utils/agent/tpl.md#RDAT.template), [`last_exp`](../base.md#DSTrace.last_exp), [`CodingSketch`](../utils.md#CodingSketch)
- used by: [`async_gen`](../router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`gen`](../../../../../core/proposal.md#ExpGen.gen), [`draft_exp_gen`](../router/__init__.md#ParallelMultiTraceExpGen.draft_exp_gen)

