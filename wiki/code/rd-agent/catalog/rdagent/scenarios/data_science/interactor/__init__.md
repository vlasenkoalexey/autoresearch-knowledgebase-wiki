---
title: 'Module: rdagent/scenarios/data_science/interactor/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/interactor/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.interactor`/
symbols:
  DSInteractor.interact: DSInteractor#interact().
  FBDSInteractor.dump_and_wait_for_user_input: FBDSInteractor#dump_and_wait_for_user_input().
  DSInteractor.dump_and_wait_for_user_input: DSInteractor#dump_and_wait_for_user_input().
  DSInteractor: DSInteractor#
  FBDSInteractor: FBDSInteractor#
---
# Module: [`rdagent/scenarios/data_science/interactor/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py)

## Classes
### `DSInteractor`  ·  implements/extends Interactor
- def: [`rdagent/scenarios/data_science/interactor/__init__.py:17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py#L17)
- signature: `class DSInteractor(Interactor[DSExperiment]):`
- members:
  - `dump_and_wait_for_user_input(self, scenario_description: str, ds_trace_desc: str, current_code: str, hypothesis_candidates: list[str], target_hypothesis: DSHypothesis, target_hypothesis_index: int, task_description: Task, exp: DSExperiment)` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py#L19)
  - `interact(self, exp: DSExperiment, trace: DSTrace)` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py#L32) — Interact with the experiment to get feedback or confirmation. — documented in [rdagent-app-data_science-conf](../../../../../concepts/rdagent-app-data_science-conf.md)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../app/data_science/conf.md#DS_RD_SETTING), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../experiment/experiment.md#DSExperiment), [`Task`](../../../core/experiment.md#Task), [`DSTrace`](../proposal/exp_gen/base.md#DSTrace), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`dump_and_wait_for_user_input`](__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`DSHypothesis`](../proposal/exp_gen/base.md#DSHypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`experiment_and_feedback_list_after_init`](../proposal/exp_gen/base.md#DSTrace.experiment_and_feedback_list_after_init), [`coder_on_whole_pipeline`](../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`is_selection_new_tree`](../../../core/proposal.md#Trace.is_selection_new_tree), [`Interactor`](../../../core/interactor.md#Interactor), [`pending_tasks_list`](../experiment/experiment.md#DSExperiment.pending_tasks_list), [`FBDSInteractor`](__init__.md#FBDSInteractor), [`hypothesis_candidates`](../experiment/experiment.md#DSExperiment.hypothesis_candidates), [`scen`](../../../core/interactor.md#Interactor.scen)
- used by: [`Interactor`](../../../core/interactor.md#Interactor), [`interact`](../../../core/interactor.md#Interactor.interact), [`FBDSInteractor`](__init__.md#FBDSInteractor)

### `FBDSInteractor`  ·  implements/extends DSInteractor
- def: [`rdagent/scenarios/data_science/interactor/__init__.py:70`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py#L70)
- signature: `class FBDSInteractor(DSInteractor):`
- members:
  - `dump_and_wait_for_user_input(self, scenario_description: str, ds_trace_desc: str, current_code: str, hypothesis_candidates: list[DSHypothesis], target_hypothesis: DSHypothesis, target_hypothesis_index: int, task: Task, exp: DSExperiment)` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/interactor/__init__.py#L71) — documented in [rdagent-app-data_science-conf](../../../../../concepts/rdagent-app-data_science-conf.md)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../app/data_science/conf.md#DS_RD_SETTING), [`DSExperiment`](../experiment/experiment.md#DSExperiment), [`Task`](../../../core/experiment.md#Task), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`DSHypothesis`](../proposal/exp_gen/base.md#DSHypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`user_interaction_mid_folder`](../../../app/data_science/conf.md#DataScienceBasePropSetting.user_interaction_mid_folder), [`pending_tasks_list`](../experiment/experiment.md#DSExperiment.pending_tasks_list), [`set_user_instructions`](../experiment/experiment.md#DSExperiment.set_user_instructions), [`DSInteractor`](__init__.md#DSInteractor), [`user_instructions`](../../../core/experiment.md#Experiment.user_instructions), [`user_interaction_wait_seconds`](../../../app/data_science/conf.md#DataScienceBasePropSetting.user_interaction_wait_seconds)
- used by: [`dump_and_wait_for_user_input`](__init__.md#DSInteractor.dump_and_wait_for_user_input), [`DSInteractor`](__init__.md#DSInteractor)

