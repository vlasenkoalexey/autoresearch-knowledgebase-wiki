---
title: 'Module: rdagent/core/experiment.py'
type: catalog
provenance: extracted
module: rdagent/core/experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.experiment`/
symbols:
  FBWorkspace: FBWorkspace#
  FBWorkspace.file_dict: FBWorkspace#file_dict.
  Experiment.experiment_workspace: Experiment#experiment_workspace.
  Experiment: Experiment#
  FBWorkspace.workspace_path: FBWorkspace#workspace_path.
  Task: Task#
  FBWorkspace.inject_files: FBWorkspace#inject_files().
  Workspace: Workspace#
  Experiment.based_experiments: Experiment#based_experiments.
  Experiment.sub_tasks: Experiment#sub_tasks.
  Task.get_task_information: Task#get_task_information().
  Experiment.hypothesis: Experiment#hypothesis.
  FBWorkspace.run: FBWorkspace#run().
  Experiment.result: Experiment#result().
  FBWorkspace.execute: FBWorkspace#execute().
  AbsTask.name: AbsTask#name.
  Experiment.sub_workspace_list: Experiment#sub_workspace_list.
  Workspace.target_task: Workspace#target_task.
  ASpecificExp: ASpecificExp.
  Experiment.set_user_instructions: Experiment#set_user_instructions().
  FBWorkspace.all_codes: FBWorkspace#all_codes().
  Loader.load: Loader#load().
  Loader: Loader#
  Experiment.__init__: Experiment#__init__().
  ExperimentPlan: ExperimentPlan#
  FBWorkspace.create_ws_ckp: FBWorkspace#create_ws_ckp().
  FBWorkspace.inject_code_from_file_dict: FBWorkspace#inject_code_from_file_dict().
  Task.description: Task#description.
  Workspace.running_info: Workspace#running_info.
  FBWorkspace.prepare: FBWorkspace#prepare().
  UserInstructions: UserInstructions#
  Experiment.local_selection: Experiment#local_selection.
  ASpecificTask: ASpecificTask.
  WsLoader: WsLoader#
  FBWorkspace.inject_from_workspace: FBWorkspace#inject_from_workspace().
  FBWorkspace.before_execute: FBWorkspace#before_execute().
  Experiment.create_ws_ckp: Experiment#create_ws_ckp().
  Experiment.recover_ws_ckp: Experiment#recover_ws_ckp().
  WsLoader.load: WsLoader#load().
  RunningInfo.running_time: RunningInfo#running_time.
  FBWorkspace.get_codes: FBWorkspace#get_codes().
  FBWorkspace.recover_ws_ckp: FBWorkspace#recover_ws_ckp().
  TaskOrExperiment: TaskOrExperiment.
  Workspace.feedback: Workspace#feedback.
  FBWorkspace.__init__: FBWorkspace#__init__().
  ASpecificWSForExperiment: ASpecificWSForExperiment.
  Experiment.running_info: Experiment#running_info.
  Task.__init__: Task#__init__().
  FBWorkspace.remove_files: FBWorkspace#remove_files().
  Experiment.prop_dev_feedback: Experiment#prop_dev_feedback.
  Workspace.execute: Workspace#execute().
  Experiment.user_instructions: Experiment#user_instructions.
  ASpecificPlan: ASpecificPlan.
  Workspace.copy: Workspace#copy().
  FBWorkspace.ws_ckp: FBWorkspace#ws_ckp.
  FBWorkspace.clear: FBWorkspace#clear().
  FBWorkspace.__str__: FBWorkspace#__str__().
  ASpecificFeedback: ASpecificFeedback.
  Workspace.create_ws_ckp: Workspace#create_ws_ckp().
  Workspace.recover_ws_ckp: Workspace#recover_ws_ckp().
  ASpecificWS: ASpecificWS.
  FBWorkspace.inject_code_from_folder: FBWorkspace#inject_code_from_folder().
  ASpecificWSForSubTasks: ASpecificWSForSubTasks.
  RunningInfo.result: RunningInfo#result.
  FBWorkspace.DEL_KEY: FBWorkspace#DEL_KEY.
  Experiment.sub_results: Experiment#sub_results.
  AbsTask: AbsTask#
  Workspace.__init__: Workspace#__init__().
  Workspace.all_codes: Workspace#all_codes().
  FBWorkspace.copy: FBWorkspace#copy().
  Experiment.plan: Experiment#plan.
  RunningInfo: RunningInfo#
  AbsTask.get_task_information: AbsTask#get_task_information().
  Task.__repr__: Task#__repr__().
  FBWorkspace.get_files: FBWorkspace#get_files().
  Task.user_instructions: Task#user_instructions.
  FBWorkspace.change_summary: FBWorkspace#change_summary.
  FBWorkspace._format_code_dict: FBWorkspace#_format_code_dict().
  AbsTask.version: AbsTask#version.
  AbsTask.__init__: AbsTask#__init__().
  FBWorkspace.link_all_files_in_folder_to_workspace: FBWorkspace#link_all_files_in_folder_to_workspace().
  UserInstructions.__str__: UserInstructions#__str__().
---
# Module: [`rdagent/core/experiment.py`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py)

## Classes
### `AbsTask`  ·  implements/extends ABC
- def: [`rdagent/core/experiment.py:34`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L34)
- signature: `class AbsTask(ABC):`
- members:
  - `__init__(self, name: str, version: int = 1)` — [`L35`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L35) — The version of the task, default is 1
  - `get_task_information(self)` — [`L45`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L45) — Get the task information string to build the unique key
  - `name` — [`L42`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L42)
  - `version` — [`L41`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L41)
- uses (calls/refs, reference-scoped): [`Task`](experiment.md#Task), [`get_task_information`](experiment.md#Task.get_task_information)
- used by: [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`Task`](experiment.md#Task), [`develop`](../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`evaluate`](../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`implement_one_task`](../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`get_task_information`](experiment.md#Task.get_task_information), [`evaluate`](../components/coder/factor_coder/evaluators.md#FactorEvaluatorForCoder.evaluate), [`_generate_code`](../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`tasks_window`](../log/ui/app.md#tasks_window), [`consume_msg`](../log/ui/web.md#ModelTaskWindow.consume_msg), [`get_task_information`](../components/coder/model_coder/model.md#ModelTask.get_task_information), [`load`](../components/loader/task_loader.md#ModelWsLoader.load), [`get_task_brief_information`](../components/coder/model_coder/model.md#ModelTask.get_task_brief_information), [`get_task_information`](../components/coder/finetune/exp.md#FTTask.get_task_information), [`__init__`](experiment.md#Task.__init__), [`get_task_information`](../components/coder/data_science/model/exp.md#ModelTask.get_task_information), [`__repr__`](../components/coder/model_coder/model.md#ModelTask.__repr__), [`__repr__`](experiment.md#Task.__repr__)  (1 test-only)

### `Experiment`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/experiment.py:396`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L396) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
- doc: The experiment is a sequence of tasks and the implementations of the tasks after generated by the Developer.
- signature: `class Experiment(ABC, Generic[ASpecificTask, ASpecificWSForExperiment, ASpecificWSForSubTasks]):`
- members:
  - `create_ws_ckp(self)` — [`L469`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L469)
  - `recover_ws_ckp(self)` — [`L476`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L476)
  - `result(self)` — [`L461`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L461) — documented in [rdagent-core-experiment](../../../concepts/rdagent-core-experiment.md)
  - `set_user_instructions(self, user_instructions: UserInstructions | None)` — [`L446`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L446)
  - `based_experiments` — [`L419`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L419)
  - `experiment_workspace` — [`L421`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L421) — documented in [rdagent-core-experiment](../../../concepts/rdagent-core-experiment.md)
  - `hypothesis` — [`L410`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L410) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `local_selection` — [`L440`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L440)
  - `plan` — [`L441`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L441)
  - `prop_dev_feedback` — [`L428`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L428)
  - `running_info` — [`L434`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L434)
  - `sub_results` — [`L435`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L435)
  - `sub_tasks` — [`L411`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L411)
  - `sub_workspace_list` — [`L415`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L415)
  - `user_instructions` — [`L444`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L444)
- protocol/private: `__init__`[`L404`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L404)
- uses (calls/refs, reference-scoped): [`DSExperiment`](../scenarios/data_science/experiment/experiment.md#DSExperiment), [`Hypothesis`](proposal.md#Hypothesis), [`QlibFactorExperiment`](../scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment), [`Feedback`](evaluation.md#Feedback), [`QlibModelExperiment`](../scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment), [`target_task`](experiment.md#Workspace.target_task), [`KGModelExperiment`](../scenarios/kaggle/experiment/kaggle_experiment.md#KGModelExperiment), [`KGFactorExperiment`](../scenarios/kaggle/experiment/kaggle_experiment.md#KGFactorExperiment), [`EvolvingItem`](../components/coder/CoSTEER/evolvable_subjects.md#EvolvingItem), [`FTExperiment`](../scenarios/finetune/experiment/experiment.md#FTExperiment), [`ExperimentPlan`](experiment.md#ExperimentPlan), [`UserInstructions`](experiment.md#UserInstructions), [`RLExperiment`](../scenarios/rl/experiment/experiment.md#RLExperiment), [`ASpecificTask`](experiment.md#ASpecificTask), [`QlibFactorExperiment`](../scenarios/qlib/experiment/quant_experiment.md#QlibFactorExperiment), [`QlibModelExperiment`](../scenarios/qlib/experiment/quant_experiment.md#QlibModelExperiment), [`set_user_instructions`](../scenarios/data_science/experiment/experiment.md#DSExperiment.set_user_instructions), [`ASpecificWSForExperiment`](experiment.md#ASpecificWSForExperiment), [`ASpecificWSForSubTasks`](experiment.md#ASpecificWSForSubTasks), [`create_ws_ckp`](experiment.md#Workspace.create_ws_ckp), [`recover_ws_ckp`](experiment.md#Workspace.recover_ws_ckp), [`result`](experiment.md#RunningInfo.result), [`RunningInfo`](experiment.md#RunningInfo), [`user_instructions`](experiment.md#Task.user_instructions)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`DSExperiment`](../scenarios/data_science/experiment/experiment.md#DSExperiment), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`develop`](../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`hypothesis_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`_gen_hypothesis`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`_generate_and_run_script`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`direct_exp_gen`](../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`develop`](../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`coding`](../scenarios/data_science/loop.md#DataScienceRDLoop.coding), [`evaluate_one_trace`](../scenarios/data_science/proposal/exp_gen/select/submit.md#evaluate_one_trace), [`gen`](proposal.md#ExpGen.gen), [`_prepare_validation_scripts`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._prepare_validation_scripts), [`process_experiment`](../scenarios/data_science/proposal/exp_gen/select/submit.md#process_experiment), [`develop`](../scenarios/kaggle/developer/runner.md#KGModelRunner.develop), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen), [`hypothesis_rewrite`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`interact`](../scenarios/data_science/interactor/__init__.md#DSInteractor.interact), [`summarize_folder`](../log/mle_summary.md#summarize_folder), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen.gen), [`extract_hypothesis_and_exp_from_reports`](../app/qlib_rd_loop/factor_from_report.md#extract_hypothesis_and_exp_from_reports), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen_MultiTrace.gen), [`get_sota_exp_stat`](../log/ui/utils.md#get_sota_exp_stat), [`process_factor_data`](../scenarios/qlib/developer/utils.md#process_factor_data), [`evolve_iter`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`gen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen.gen)  (+91 more; 2 test-only)

### `ExperimentPlan`  ·  implements/extends dict
- def: [`rdagent/core/experiment.py:390`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L390)
- doc: A plan for the experiment, which is a dictionary that contains the plan to each stage.
- signature: `class ExperimentPlan(dict[str, Any]):`
- uses (calls/refs, reference-scoped): [`DSExperimentPlan`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExperimentPlan)
- used by: [`gen`](../components/proposal/__init__.md#LLMHypothesisGen.gen), [`DSExperimentPlan`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExperimentPlan), [`plan`](../components/workflow/rd_loop.md#RDLoop.plan), [`gen`](proposal.md#HypothesisGen.gen), [`plan`](../app/qlib_rd_loop/quant.md#QuantRDLoop.plan), [`gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.gen), [`ASpecificPlan`](experiment.md#ASpecificPlan), [`plan`](experiment.md#Experiment.plan)

### `FBWorkspace`  ·  implements/extends Workspace
- def: [`rdagent/core/experiment.py:139`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L139) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- doc: File-based task workspace
- signature: `class FBWorkspace(Workspace):`
- members:
  - `_format_code_dict(code_dict: dict[str, str])` — [`L172`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L172) — Helper function to format the code dictionary into a string.
  - `all_codes(self)` — [`L182`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L182) — Get all the code files in the workspace as a single string, excluding test files.
  - `before_execute(self)` — [`L300`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L300) — Before executing the code, we need to prepare the workspace and inject code into the workspace.
  - `clear(self)` — [`L293`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L293) — Clear the workspace
  - `copy(self)` — [`L287`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L287) — copy the workspace from the original one
  - `create_ws_ckp(self)` — [`L324`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L324) — Zip the contents of ``workspace_path`` and persist the archive on
  - `execute(self, env: Env, entry: str)` — [`L307`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L307) — Before each execution, make sure to prepare and inject code. — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)
  - `get_codes(self, pattern: str)` — [`L189`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L189) — Get code files matching a specific pattern as a single string, excluding test files.
  - `get_files(self)` — [`L257`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L257) — Get the environment description.
  - `inject_code_from_file_dict(self, workspace: FBWorkspace)` — [`L275`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L275) — Load the workspace from the file_dict
  - `inject_code_from_folder(self, folder_path: Path)` — [`L266`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L266) — Load the workspace from the folder
  - `inject_files(self, **files: str)` — [`L223`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L223) — Inject the code into the folder. — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `inject_from_workspace(self, workspace: FBWorkspace)` — [`L283`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L283)
  - `link_all_files_in_folder_to_workspace(data_path: Path, workspace_path: Path)` — [`L209`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L209)
  - `prepare(self)` — [`L198`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L198) — Prepare the workspace except the injected code
  - `recover_ws_ckp(self)` — [`L350`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L350) — Restore the workspace directory from the in-memory checkpoint created by
  - `remove_files(self, file_names: str | list[str])` — [`L245`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L245) — Remove specified files from the workspace.
  - `run(self, env: Env, entry: str)` — [`L314`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L314) — Execute the code in the environment and return an EnvResult object (stdout, exit_code, running_time). — documented in [rdagent-core-experiment](../../../concepts/rdagent-core-experiment.md)
  - `DEL_KEY` — [`L221`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L221)
  - `change_summary` — [`L169`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L169)
  - `file_dict` — [`L164`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L164) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `workspace_path` — [`L167`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L167) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `ws_ckp` — [`L168`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L168)
- protocol/private: `__init__`[`L162`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L162), `__str__`[`L380`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L380)
- uses (calls/refs, reference-scoped): [`RD_AGENT_SETTINGS`](conf.md#RD_AGENT_SETTINGS), [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`run`](../utils/env.md#Env.run), [`Workspace`](experiment.md#Workspace), [`stdout`](../utils/env.md#EnvResult.stdout), [`run`](../scenarios/finetune/experiment/workspace.md#FTWorkspace.run), [`execute`](../components/coder/model_coder/model.md#ModelFBWorkspace.execute), [`ModelFBWorkspace`](../components/coder/model_coder/model.md#ModelFBWorkspace), [`execute`](../scenarios/qlib/experiment/workspace.md#QlibFBWorkspace.execute), [`Env`](../utils/env.md#Env), [`run`](../scenarios/rl/experiment/workspace.md#RLWorkspace.run), [`FactorFBWorkspace`](../components/coder/factor_coder/factor.md#FactorFBWorkspace), [`execute`](../scenarios/kaggle/experiment/workspace.md#KGFBWorkspace.execute), [`target_task`](experiment.md#Workspace.target_task), [`QlibFBWorkspace`](../scenarios/qlib/experiment/workspace.md#QlibFBWorkspace), [`EnvResult`](../utils/env.md#EnvResult), [`KGFBWorkspace`](../scenarios/kaggle/experiment/workspace.md#KGFBWorkspace), [`FTWorkspace`](../scenarios/finetune/experiment/workspace.md#FTWorkspace), [`RLWorkspace`](../scenarios/rl/experiment/workspace.md#RLWorkspace), [`__init__`](experiment.md#Workspace.__init__), [`workspace_ckp_size_limit`](conf.md#RDAgentSettings.workspace_ckp_size_limit), [`workspace_ckp_white_list_names`](conf.md#RDAgentSettings.workspace_ckp_white_list_names), [`workspace_path`](conf.md#RDAgentSettings.workspace_path)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`DSExperiment`](../scenarios/data_science/experiment/experiment.md#DSExperiment), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`evaluate`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`develop`](../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`evaluate`](../components/coder/finetune/eval.md#FTCoderEvaluator.evaluate), [`evaluate`](../components/coder/data_science/workflow/eval.md#WorkflowGeneralCaseSpecEvaluator.evaluate), [`_gen_hypothesis`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`implement_data`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`evaluate`](../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`evaluate`](../components/coder/data_science/raw_data_loader/eval.md#DataLoaderCoSTEEREvaluator.evaluate), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`evaluate`](../components/coder/data_science/share/eval.md#ModelDumpEvaluator.evaluate), [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`evaluate`](../components/coder/data_science/ensemble/eval.md#EnsembleCoSTEEREvaluator.evaluate), [`evaluate`](../components/coder/data_science/feature/eval.md#FeatureCoSTEEREvaluator.evaluate), [`implement_one_task`](../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`_generate_and_run_script`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`Workspace`](experiment.md#Workspace), [`evaluate`](../components/coder/finetune/eval.md#FTDataEvaluator.evaluate), [`implement_one_task`](../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llm_feedback`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`develop`](../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`implement_one_task`](../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`_run_micro_batch_test`](../components/coder/finetune/unified_validator.md#LLMConfigValidator._run_micro_batch_test), [`implement_one_task`](../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`_prepare_validation_scripts`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._prepare_validation_scripts), [`process_experiment`](../scenarios/data_science/proposal/exp_gen/select/submit.md#process_experiment)  (+77 more; 10 test-only)

### `Loader`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/experiment.py:495`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L495)
- signature: `class Loader(ABC, Generic[TaskOrExperiment]):`
- members:
  - `load(self, *args: Any, **kwargs: Any)` — [`L497`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L497)
- uses (calls/refs, reference-scoped): [`load`](../scenarios/qlib/factor_experiment_loader/pdf_loader.md#FactorExperimentLoaderFromPDFfiles.load), [`FactorExperimentLoader`](../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](../components/coder/model_coder/task_loader.md#ModelExperimentLoaderFromPDFfiles.load), [`ModelTaskLoader`](../components/loader/task_loader.md#ModelTaskLoader), [`load`](../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromDict.load), [`TaskOrExperiment`](experiment.md#TaskOrExperiment), [`load`](../components/coder/model_coder/task_loader.md#ModelExperimentLoaderFromDict.load), [`load`](../components/loader/task_loader.md#ModelTaskLoaderJson.load), [`FactorTaskLoader`](../components/loader/task_loader.md#FactorTaskLoader), [`ModelExperimentLoader`](../components/loader/experiment_loader.md#ModelExperimentLoader), [`load`](../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonFile.load), [`load`](../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonString.load)
- used by: [`FactorExperimentLoader`](../components/loader/experiment_loader.md#FactorExperimentLoader), [`ModelTaskLoader`](../components/loader/task_loader.md#ModelTaskLoader), [`FactorTaskLoader`](../components/loader/task_loader.md#FactorTaskLoader), [`ModelExperimentLoader`](../components/loader/experiment_loader.md#ModelExperimentLoader)

### `RunningInfo`
- def: [`rdagent/core/experiment.py:82`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L82)
- signature: `class RunningInfo:`
- members:
  - `result` — [`L83`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L83)
  - `running_time` — [`L84`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L84)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`Experiment`](experiment.md#Experiment), [`evaluate`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`result`](experiment.md#Experiment.result), [`develop`](../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`running_info`](experiment.md#Workspace.running_info), [`running_info`](experiment.md#Experiment.running_info)

### `Task`  ·  implements/extends AbsTask
- def: [`rdagent/core/experiment.py:58`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L58) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- signature: `class Task(AbsTask):`
- members:
  - `get_task_information(self)` — [`L70`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L70) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `description` — [`L67`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L67)
  - `user_instructions` — [`L68`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L68)
- protocol/private: `__init__`[`L59`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L59), `__repr__`[`L73`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L73)
- uses (calls/refs, reference-scoped): [`CoSTEERTask`](../components/coder/CoSTEER/task.md#CoSTEERTask), [`name`](experiment.md#AbsTask.name), [`get_task_information`](../components/coder/model_coder/model.md#ModelTask.get_task_information), [`get_task_information`](../components/coder/factor_coder/factor.md#FactorTask.get_task_information), [`UserInstructions`](experiment.md#UserInstructions), [`get_task_information`](../components/coder/finetune/exp.md#FTTask.get_task_information), [`RLTask`](../scenarios/rl/experiment/experiment.md#RLTask), [`get_task_information`](../components/coder/data_science/model/exp.md#ModelTask.get_task_information), [`AbsTask`](experiment.md#AbsTask), [`__init__`](experiment.md#AbsTask.__init__)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`DSExperiment`](../scenarios/data_science/experiment/experiment.md#DSExperiment), [`evaluate`](../components/coder/finetune/eval.md#FTCoderEvaluator.evaluate), [`evaluate`](../components/coder/data_science/workflow/eval.md#WorkflowGeneralCaseSpecEvaluator.evaluate), [`implement_data`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`evaluate`](../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`evaluate`](../components/coder/data_science/raw_data_loader/eval.md#DataLoaderCoSTEEREvaluator.evaluate), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`evaluate`](../components/coder/data_science/share/eval.md#ModelDumpEvaluator.evaluate), [`evaluate`](../components/coder/data_science/ensemble/eval.md#EnsembleCoSTEEREvaluator.evaluate), [`evaluate`](../components/coder/data_science/feature/eval.md#FeatureCoSTEEREvaluator.evaluate), [`implement_one_task`](../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`evaluate`](../components/coder/finetune/eval.md#FTDataEvaluator.evaluate), [`implement_one_task`](../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llm_feedback`](../components/coder/finetune/eval.md#FTDataEvaluator._generate_llm_feedback), [`implement_one_task`](../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`evaluate`](../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`implement_one_task`](../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`get_scenario_all_desc`](scenario.md#Scenario.get_scenario_all_desc), [`CoSTEERTask`](../components/coder/CoSTEER/task.md#CoSTEERTask), [`_generate_code`](../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`evaluate`](../components/coder/model_coder/eva_utils.md#ModelCodeEvaluator.evaluate), [`evaluate`](../components/coder/model_coder/evaluators.md#ModelCoSTEEREvaluator.evaluate), [`gen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen.gen), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorEvaluator.evaluate), [`evaluate`](../components/coder/model_coder/eva_utils.md#ModelFinalEvaluator.evaluate), [`implement_one_task`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`convert`](../components/coder/data_science/share/notebook.md#NotebookConverter.convert), [`tasks_window`](../log/ui/app.md#tasks_window), [`dump_and_wait_for_user_input`](../scenarios/data_science/interactor/__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`evaluate`](../app/finetune/share/eval.md#PrevModelLoadEvaluator.evaluate), [`implement_lf_config`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_lf_config), [`consume_msg`](../log/ui/web.md#ModelTaskWindow.consume_msg), [`get_task_information`](../components/coder/model_coder/model.md#ModelTask.get_task_information), [`set_user_instructions`](experiment.md#Experiment.set_user_instructions), [`evaluate`](../components/coder/rl/costeer.md#RLCoderEvaluator.evaluate)  (+23 more; 2 test-only)

### `UserInstructions`  ·  implements/extends list
- def: [`rdagent/core/experiment.py:51`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L51)
- signature: `class UserInstructions(list[str]):`
- protocol/private: `__str__`[`L52`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L52)
- used by: [`hypothesis_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`hypothesis_rewrite`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`set_user_instructions`](experiment.md#Experiment.set_user_instructions), [`set_user_instructions`](../scenarios/data_science/experiment/experiment.md#DSExperiment.set_user_instructions), [`__init__`](experiment.md#Task.__init__), [`user_instructions`](experiment.md#Experiment.user_instructions)

### `Workspace`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/experiment.py:87`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L87)
- doc: A workspace is a place to store the task implementation. It evolves as the developer implements the task.
- signature: `class Workspace(ABC, Generic[ASpecificTask, ASpecificFeedback]):`
- members:
  - `all_codes(self)` — [`L110`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L110) — Get all the code files in the workspace as a single string.
  - `copy(self)` — [`L104`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L104)
  - `create_ws_ckp(self)` — [`L117`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L117) — Create an in-memory checkpoint of the workspace so it can be restored later.
  - `execute(self, *args: Any, **kwargs: Any)` — [`L99`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L99)
  - `recover_ws_ckp(self)` — [`L123`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L123) — Restore the workspace from the checkpoint created by :py:meth:`create_ws_ckp`.
  - `feedback` — [`L95`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L95)
  - `running_info` — [`L96`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L96)
  - `target_task` — [`L94`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L94) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- protocol/private: `__init__`[`L93`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L93)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](experiment.md#FBWorkspace), [`execute`](experiment.md#FBWorkspace.execute), [`all_codes`](experiment.md#FBWorkspace.all_codes), [`create_ws_ckp`](experiment.md#FBWorkspace.create_ws_ckp), [`ASpecificTask`](experiment.md#ASpecificTask), [`recover_ws_ckp`](experiment.md#FBWorkspace.recover_ws_ckp), [`ASpecificFeedback`](experiment.md#ASpecificFeedback), [`copy`](experiment.md#FBWorkspace.copy), [`RunningInfo`](experiment.md#RunningInfo)
- used by: [`FBWorkspace`](experiment.md#FBWorkspace), [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`evaluate`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorValueEvaluator.evaluate), [`_generate_llm_feedback`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`develop`](../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`evaluate`](../components/coder/factor_coder/evaluators.md#FactorEvaluatorForCoder.evaluate), [`evaluate`](../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`develop`](../scenarios/kaggle/developer/runner.md#KGModelRunner.develop), [`evaluate`](../components/coder/model_coder/eva_utils.md#ModelCodeEvaluator.evaluate), [`evaluate`](../components/coder/model_coder/evaluators.md#ModelCoSTEEREvaluator.evaluate), [`execute`](../components/coder/model_coder/model.md#ModelFBWorkspace.execute), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorEvaluator.evaluate), [`evaluate`](../components/coder/model_coder/eva_utils.md#ModelFinalEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorCodeEvaluator.evaluate), [`summary_window`](../log/ui/app.md#summary_window), [`consume_msg`](../log/ui/web.md#WorkspaceWindow.consume_msg), [`evolving_window`](../log/ui/app.md#evolving_window), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorOutputFormatEvaluator.evaluate), [`set_user_instructions`](experiment.md#Experiment.set_user_instructions), [`get_experiment_info`](../scenarios/finetune/proposal/trace.md#FTTrace.get_experiment_info), [`_get_df`](../components/coder/factor_coder/eva_utils.md#FactorEvaluator._get_df), [`create_ws_ckp`](experiment.md#Experiment.create_ws_ckp), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorCorrelationEvaluator.evaluate), [`recover_ws_ckp`](experiment.md#Experiment.recover_ws_ckp), [`ASpecificWSForExperiment`](experiment.md#ASpecificWSForExperiment), [`__init__`](experiment.md#FBWorkspace.__init__), [`__str__`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.__str__), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorDatetimeDailyEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorEqualValueRatioEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorIndexEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorInfEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorMissingValuesEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorRowCountEvaluator.evaluate), [`evaluate`](../components/coder/factor_coder/eva_utils.md#FactorSingleColumnEvaluator.evaluate), [`__str__`](experiment.md#FBWorkspace.__str__), [`ASpecificWS`](experiment.md#ASpecificWS)  (+1 more; 3 test-only)

### `WsLoader`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/experiment.py:132`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L132)
- signature: `class WsLoader(ABC, Generic[ASpecificTask, ASpecificWS]):`
- members:
  - `load(self, task: ASpecificTask)` — [`L134`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L134)
- uses (calls/refs, reference-scoped): [`load`](../components/loader/task_loader.md#ModelWsLoader.load), [`ASpecificTask`](experiment.md#ASpecificTask), [`ModelWsLoader`](../components/loader/task_loader.md#ModelWsLoader), [`ASpecificWS`](experiment.md#ASpecificWS)
- used by: [`ModelWsLoader`](../components/loader/task_loader.md#ModelWsLoader)

## Module values
- `ASpecificExp` — [`L489`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L489)
- `ASpecificFeedback` — [`L78`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L78)
- `ASpecificPlan` — [`L490`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L490)
- `ASpecificTask` — [`L77`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L77)
- `ASpecificWS` — [`L129`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L129)
- `ASpecificWSForExperiment` — [`L386`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L386)
- `ASpecificWSForSubTasks` — [`L387`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L387)
- `TaskOrExperiment` — [`L492`](../../../../../../raw/code/rd-agent/rdagent/core/experiment.py#L492)

