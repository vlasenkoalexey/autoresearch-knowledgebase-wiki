---
title: 'Module: rdagent/components/coder/factor_coder/factor.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/factor.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder.factor`/F
symbols:
  FactorFBWorkspace.execute: actorFBWorkspace#execute().
  FactorTask: actorTask#
  FactorFBWorkspace: actorFBWorkspace#
  FactorTask.get_task_information: actorTask#get_task_information().
  FactorExperiment: actorExperiment.
  FactorTask.get_task_information_and_implementation_result: actorTask#get_task_information_and_implementation_result().
  FactorTask.factor_name: actorTask#factor_name.
  FactorTask.variables: actorTask#variables.
  FactorTask.get_task_brief_information: actorTask#get_task_brief_information().
  FactorTask.factor_description: actorTask#factor_description().
  FactorFBWorkspace.hash_func: actorFBWorkspace#hash_func().
  FactorTask.factor_formulation: actorTask#factor_formulation.
  FactorFBWorkspace.__str__: actorFBWorkspace#__str__().
  FactorFBWorkspace.from_folder: actorFBWorkspace#from_folder().
  FactorFBWorkspace.raise_exception: actorFBWorkspace#raise_exception.
  FeatureExperiment: eatureExperiment.
  FactorTask.factor_implementation: actorTask#factor_implementation.
  FactorTask.from_dict: actorTask#from_dict().
  FactorTask.__repr__: actorTask#__repr__().
  FactorFBWorkspace.__init__: actorFBWorkspace#__init__().
  FactorFBWorkspace.__repr__: actorFBWorkspace#__repr__().
  FactorTask.factor_resources: actorTask#factor_resources.
  FactorFBWorkspace.FB_CODE_NOT_SET: actorFBWorkspace#FB_CODE_NOT_SET.
  FactorFBWorkspace.FB_EXECUTION_SUCCEEDED: actorFBWorkspace#FB_EXECUTION_SUCCEEDED.
  FactorFBWorkspace.FB_OUTPUT_FILE_NOT_FOUND: actorFBWorkspace#FB_OUTPUT_FILE_NOT_FOUND.
  FactorFBWorkspace.FB_OUTPUT_FILE_FOUND: actorFBWorkspace#FB_OUTPUT_FILE_FOUND.
  FactorTask.__init__: actorTask#__init__().
  FactorFBWorkspace.FB_EXEC_SUCCESS: actorFBWorkspace#FB_EXEC_SUCCESS.
---
# Module: [`rdagent/components/coder/factor_coder/factor.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py)

## Classes
### `FactorFBWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/components/coder/factor_coder/factor.py:77`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L77) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- doc: This class is used to implement a factor by writing the code to a file.
- signature: `class FactorFBWorkspace(FBWorkspace):`
- members:
  - `execute(self, data_type: str = "Debug")` — [`L107`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L107) — execute the implementation and get the factor value by the following steps: — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `from_folder(task: FactorTask, path: Union[str, Path], **kwargs)` — [`L221`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L221)
  - `hash_func(self, data_type: str = "Debug")` — [`L99`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L99)
  - `FB_CODE_NOT_SET` — [`L85`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L85)
  - `FB_EXECUTION_SUCCEEDED` — [`L86`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L86)
  - `FB_EXEC_SUCCESS` — [`L84`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L84)
  - `FB_OUTPUT_FILE_FOUND` — [`L88`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L88)
  - `FB_OUTPUT_FILE_NOT_FOUND` — [`L87`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L87)
  - `raise_exception` — [`L97`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L97)
- protocol/private: `__init__`[`L90`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L90), `__repr__`[`L217`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L217), `__str__`[`L212`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L212)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`FactorTask`](factor.md#FactorTask), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`FACTOR_COSTEER_SETTINGS`](config.md#FACTOR_COSTEER_SETTINGS), [`target_task`](../../../core/experiment.md#Workspace.target_task), [`local_data_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`md5_hash`](../../../utils/__init__.md#md5_hash), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`before_execute`](../../../core/experiment.md#FBWorkspace.before_execute), [`CustomRuntimeError`](../../../core/exception.md#CustomRuntimeError), [`__init__`](../../../core/experiment.md#FBWorkspace.__init__), [`data_folder_debug`](config.md#FactorCoSTEERSettings.data_folder_debug), [`NoOutputError`](../../../core/exception.md#NoOutputError), [`data_folder`](config.md#FactorCoSTEERSettings.data_folder), [`CodeFormatError`](../../../core/exception.md#CodeFormatError), [`file_based_execution_timeout`](config.md#FactorCoSTEERSettings.file_based_execution_timeout), [`link_all_files_in_folder_to_workspace`](../../../core/experiment.md#FBWorkspace.link_all_files_in_folder_to_workspace), [`python_bin`](config.md#FactorCoSTEERSettings.python_bin)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`develop`](../../../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`QlibFactorExperiment`](../../../scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment), [`execute`](../../../core/experiment.md#FBWorkspace.execute), [`consume_msg`](../../../log/ui/web.md#EvolvingWindow.consume_msg), [`summary_window`](../../../log/ui/app.md#summary_window), [`consume_msg`](../../../log/ui/web.md#WorkspaceWindow.consume_msg), [`evolving_window`](../../../log/ui/app.md#evolving_window), [`KGFactorExperiment`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGFactorExperiment), [`_build_execute_calls`](../../../scenarios/qlib/developer/utils.md#_build_execute_calls), [`load`](../../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorTestCaseLoaderFromJsonFile.load), [`_build_base_feature_workspaces`](../../../scenarios/qlib/developer/utils.md#_build_base_feature_workspaces), [`QlibFactorExperiment`](../../../scenarios/qlib/experiment/quant_experiment.md#QlibFactorExperiment), [`assign_code_list_to_evo`](evolving_strategy.md#FactorMultiProcessEvolvingStrategy.assign_code_list_to_evo)  (1 test-only)

### `FactorTask`  ·  implements/extends CoSTEERTask
- def: [`rdagent/components/coder/factor_coder/factor.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L20) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- signature: `class FactorTask(CoSTEERTask):`
- members:
  - `factor_description(self)` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L44) — for compatibility
  - `from_dict(dict)` — [`L70`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L70)
  - `get_task_brief_information(self)` — [`L54`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L54)
  - `get_task_information(self)` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L48) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `get_task_information_and_implementation_result(self)` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L60)
  - `factor_formulation` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L37)
  - `factor_implementation` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L40)
  - `factor_name` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L34)
  - `factor_resources` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L39)
  - `variables` — [`L38`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L38)
- protocol/private: `__init__`[`L23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L23), `__repr__`[`L73`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L73)
- uses (calls/refs, reference-scoped): [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask), [`description`](../../../core/experiment.md#Task.description), [`__init__`](../CoSTEER/task.md#CoSTEERTask.__init__)
- used by: [`_obj_to_json`](../../../log/ui/storage.md#WebStorage._obj_to_json), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`evaluate`](evaluators.md#FactorEvaluatorForCoder.evaluate), [`implement_one_task`](evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask), [`QlibFactorExperiment`](../../../scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment), [`extract_hypothesis_and_exp_from_reports`](../../../app/qlib_rd_loop/factor_from_report.md#extract_hypothesis_and_exp_from_reports), [`evaluate`](eva_utils.md#FactorCodeEvaluator.evaluate), [`summary_window`](../../../log/ui/app.md#summary_window), [`tasks_window`](../../../log/ui/app.md#tasks_window), [`consume_msg`](../../../log/ui/web.md#ResearchWindow.consume_msg), [`error_summary`](evolving_strategy.md#FactorMultiProcessEvolvingStrategy.error_summary), [`evolving_window`](../../../log/ui/app.md#evolving_window), [`__init__`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGFactorExperiment.__init__), [`__init__`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGModelExperiment.__init__), [`convert_response`](../../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`consume_msg`](../../../log/ui/web.md#FactorTaskWindow.consume_msg), [`evaluate`](eva_utils.md#FactorFinalDecisionEvaluator.evaluate), [`KGFactorExperiment`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGFactorExperiment), [`convert_feature_experiment`](../../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_feature_experiment), [`load`](../../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorTestCaseLoaderFromJsonFile.load), [`_build_base_feature_workspaces`](../../../scenarios/qlib/developer/utils.md#_build_base_feature_workspaces), [`QlibFactorExperiment`](../../../scenarios/qlib/experiment/quant_experiment.md#QlibFactorExperiment), [`load`](../../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromDict.load), [`from_folder`](factor.md#FactorFBWorkspace.from_folder), [`FactorTaskLoader`](../../loader/task_loader.md#FactorTaskLoader)

## Module values
- `FactorExperiment` — [`L230`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L230)
- `FeatureExperiment` — [`L231`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/factor.py#L231)

