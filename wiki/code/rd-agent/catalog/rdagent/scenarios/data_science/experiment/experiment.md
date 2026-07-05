---
title: 'Module: rdagent/scenarios/data_science/experiment/experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/experiment/experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.experiment.experiment`/
symbols:
  DSExperiment: DSExperiment#
  DSExperiment.pending_tasks_list: DSExperiment#pending_tasks_list.
  DSExperiment.set_user_instructions: DSExperiment#set_user_instructions().
  DSExperiment.__init__: DSExperiment#__init__().
  COMPONENT: COMPONENT.
  DSExperiment.is_ready_to_run: DSExperiment#is_ready_to_run().
  DSExperiment.set_local_selection: DSExperiment#set_local_selection().
  DSExperiment.hypothesis_candidates: DSExperiment#hypothesis_candidates.
  DSExperiment.format_check_result: DSExperiment#format_check_result.
---
# Module: [`rdagent/scenarios/data_science/experiment/experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py)

## Classes
### `DSExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/data_science/experiment/experiment.py:11`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L11) — documented in [rdagent-core-experiment](../../../../../concepts/rdagent-core-experiment.md)
- signature: `class DSExperiment(Experiment[Task, FBWorkspace, FBWorkspace]):`
- members:
  - `is_ready_to_run(self)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L35) — ready to run does not indicate the experiment is runnable
  - `set_local_selection(self, local_selection: tuple[int, ...])` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L42)
  - `set_user_instructions(self, user_instructions: UserInstructions | None)` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L27)
  - `format_check_result` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L23)
  - `hypothesis_candidates` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L21)
  - `pending_tasks_list` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L20)
- protocol/private: `__init__`[`L12`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L12)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../core/experiment.md#Experiment), [`Task`](../../../core/experiment.md#Task), [`set_user_instructions`](../../../core/experiment.md#Experiment.set_user_instructions), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`UserInstructions`](../../../core/experiment.md#UserInstructions), [`local_selection`](../../../core/experiment.md#Experiment.local_selection)
- used by: [`record`](../loop.md#DataScienceRDLoop.record), [`_obj_to_json`](../../../log/ui/storage.md#WebStorage._obj_to_json), [`Experiment`](../../../core/experiment.md#Experiment), [`async_gen`](../proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`hypothesis_gen`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`gen`](../proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`gen`](../proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`gen`](../proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`_generate_and_run_script`](../proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`gen`](../proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`_prepare_validation_scripts`](../proposal/exp_gen/select/submit.md#ValidationSelector._prepare_validation_scripts), [`process_experiment`](../proposal/exp_gen/select/submit.md#process_experiment), [`gen`](../proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen), [`hypothesis_rewrite`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`interact`](../interactor/__init__.md#DSInteractor.interact), [`summarize_folder`](../../../log/mle_summary.md#summarize_folder), [`gen`](../proposal/exp_gen/merge.md#MergeExpGen.gen), [`gen`](../proposal/exp_gen/merge.md#MergeExpGen_MultiTrace.gen), [`get_sota_exp_stat`](../../../log/ui/utils.md#get_sota_exp_stat), [`task_gen`](../proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.task_gen), [`gen`](../proposal/exp_gen/naive.md#NaiveExpGen.gen), [`identify_feedback_problem`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.identify_feedback_problem), [`identify_scenario_problem`](../proposal/exp_gen/proposal.md#DSProposalV2ExpGen.identify_scenario_problem), [`feedback`](../loop.md#DataScienceRDLoop.feedback), [`get_sota_exp_to_submit`](../proposal/exp_gen/select/submit.md#AutoSOTAexpSelector.get_sota_exp_to_submit), [`dump_and_wait_for_user_input`](../interactor/__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`hist`](../proposal/exp_gen/base.md#DSTrace.hist), [`get_sota_exp_to_submit`](../proposal/exp_gen/select/submit.md#ValidationSelector.get_sota_exp_to_submit), [`develop_one_competition`](../../../components/coder/data_science/model/test.md#develop_one_competition), [`develop_one_competition`](../../../components/coder/data_science/workflow/test.md#develop_one_competition), [`experiment_and_feedback_list_after_init`](../proposal/exp_gen/base.md#DSTrace.experiment_and_feedback_list_after_init), [`sota_experiment_fb`](../proposal/exp_gen/base.md#DSTrace.sota_experiment_fb), [`save_grade_info`](../../../log/mle_summary.md#save_grade_info), [`running`](../loop.md#DataScienceRDLoop.running), [`collect_sota_candidates`](../proposal/exp_gen/select/submit.md#BestValidSelector.collect_sota_candidates)  (+25 more)

## Module values
- `COMPONENT` — [`L8`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/experiment/experiment.py#L8)

