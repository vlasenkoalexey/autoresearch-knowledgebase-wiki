---
title: 'Module: rdagent/components/coder/data_science/feature/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/feature/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.feature`/
symbols:
  FeatureMultiProcessEvolvingStrategy.implement_one_task: FeatureMultiProcessEvolvingStrategy#implement_one_task().
  FeatureCoSTEER.__init__: FeatureCoSTEER#__init__().
  FeatureCoSTEER: FeatureCoSTEER#
  FeatureMultiProcessEvolvingStrategy: FeatureMultiProcessEvolvingStrategy#
  DIRNAME: DIRNAME.
  FeatureMultiProcessEvolvingStrategy.assign_code_list_to_evo: FeatureMultiProcessEvolvingStrategy#assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/data_science/feature/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py)

## Classes
### `FeatureCoSTEER`  ·  implements/extends DSCoSTEER
- def: [`rdagent/components/coder/data_science/feature/__init__.py:118`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L118)
- signature: `class FeatureCoSTEER(DSCoSTEER):`
- protocol/private: `__init__`[`L119`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L119)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`Scenario`](../../../../core/scenario.md#Scenario), [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`CoSTEERMultiEvaluator`](../../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../CoSTEER/__init__.md#CoSTEER.__init__), [`DSCoderCoSTEERSettings`](../conf.md#DSCoderCoSTEERSettings), [`coder_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_max_loop), [`FeatureCoSTEEREvaluator`](eval.md#FeatureCoSTEEREvaluator), [`FeatureMultiProcessEvolvingStrategy`](__init__.md#FeatureMultiProcessEvolvingStrategy)
- used by: [`DSCoSTEER`](../share/ds_costeer.md#DSCoSTEER), [`develop_one_competition`](test.md#develop_one_competition), [`feature_coder`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.feature_coder)

### `FeatureMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/data_science/feature/__init__.py:28`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L28)
- signature: `class FeatureMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L101`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L101) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: FeatureTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L29)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`CoderError`](../../../../core/exception.md#CoderError), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`CoSTEERQueriedKnowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`PythonAgentOut`](../../../../utils/agent/ret.md#PythonAgentOut), [`scen`](../../../../core/evolving_framework.md#EvolvingStrategy.scen), [`FeatureTask`](exp.md#FeatureTask), [`get_spec`](../../../../utils/agent/ret.md#PythonAgentOut.get_spec), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`extract_output`](../../../../utils/agent/ret.md#PythonAgentOut.extract_output), [`DIRNAME`](__init__.md#DIRNAME)
- used by: [`MultiProcessEvolvingStrategy`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#FeatureCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/feature/__init__.py#L25)

