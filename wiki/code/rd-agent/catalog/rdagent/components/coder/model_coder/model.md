---
title: 'Module: rdagent/components/coder/model_coder/model.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/model.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.model`/Model
symbols:
  ModelTask: Task#
  ModelFBWorkspace.execute: FBWorkspace#execute().
  ModelFBWorkspace: FBWorkspace#
  ModelTask.get_task_information: Task#get_task_information().
  ModelExperiment: Experiment.
  ModelTask.model_type: Task#model_type.
  ModelTask.get_task_brief_information: Task#get_task_brief_information().
  ModelFBWorkspace.hash_func: FBWorkspace#hash_func().
  ModelTask.formulation: Task#formulation.
  ModelTask.training_hyperparameters: Task#training_hyperparameters.
  ModelTask.architecture: Task#architecture.
  ModelTask.variables: Task#variables.
  ModelTask.hyperparameters: Task#hyperparameters.
  ModelTask.from_dict: Task#from_dict().
  ModelTask.__repr__: Task#__repr__().
  ModelTask.__init__: Task#__init__().
---
# Module: [`rdagent/components/coder/model_coder/model.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py)

## Classes
### `ModelFBWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/components/coder/model_coder/model.py:69`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L69) — documented in [rdagent-log-ui-web](../../../../../concepts/rdagent-log-ui-web.md)
- doc: It is a Pytorch model implementation task;
- signature: `class ModelFBWorkspace(FBWorkspace):`
- members:
  - `execute(self, batch_size: int = 8, num_features: int = 10, num_timesteps: int = 4, num_edges: int = 20, input_value: float = 1, param_init_value: float = 1)` — [`L105`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L105)
  - `hash_func(self, batch_size: int = 8, num_features: int = 10, num_timesteps: int = 4, num_edges: int = 20, input_value: float = 1, param_init_value: float = 1)` — [`L90`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L90)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`target_task`](../../../core/experiment.md#Workspace.target_task), [`md5_hash`](../../../utils/__init__.md#md5_hash), [`prepare`](../../../utils/env.md#QTDockerEnv.prepare), [`QTDockerEnv`](../../../utils/env.md#QTDockerEnv), [`QlibCondaEnv`](../../../utils/env.md#QlibCondaEnv), [`QlibCondaConf`](../../../utils/env.md#QlibCondaConf), [`MODEL_COSTEER_SETTINGS`](conf.md#MODEL_COSTEER_SETTINGS), [`before_execute`](../../../core/experiment.md#FBWorkspace.before_execute), [`env_type`](conf.md#ModelCoSTEERSettings.env_type), [`KGDockerEnv`](../../../utils/env.md#KGDockerEnv), [`dump_python_code_run_and_get_results`](../../../utils/env.md#Env.dump_python_code_run_and_get_results)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`execute`](../../../core/experiment.md#FBWorkspace.execute), [`evaluate`](eva_utils.md#ModelCodeEvaluator.evaluate), [`evaluate`](evaluators.md#ModelCoSTEEREvaluator.evaluate), [`evaluate`](eva_utils.md#ModelFinalEvaluator.evaluate), [`consume_msg`](../../../log/ui/web.md#EvolvingWindow.consume_msg), [`summary_window`](../../../log/ui/app.md#summary_window), [`QlibModelExperiment`](../../../scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment), [`consume_msg`](../../../log/ui/web.md#WorkspaceWindow.consume_msg), [`evolving_window`](../../../log/ui/app.md#evolving_window), [`develop`](one_shot/__init__.md#ModelCodeWriter.develop), [`KGModelExperiment`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGModelExperiment), [`load`](../../loader/task_loader.md#ModelWsLoader.load), [`QlibModelExperiment`](../../../scenarios/qlib/experiment/quant_experiment.md#QlibModelExperiment), [`ModelWsLoader`](../../loader/task_loader.md#ModelWsLoader), [`assign_code_list_to_evo`](evolving_strategy.md#ModelMultiProcessEvolvingStrategy.assign_code_list_to_evo)  (1 test-only)

### `ModelTask`  ·  implements/extends CoSTEERTask
- def: [`rdagent/components/coder/model_coder/model.py:15`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L15) — documented in [rdagent-log-ui-web](../../../../../concepts/rdagent-log-ui-web.md)
- signature: `class ModelTask(CoSTEERTask):`
- members:
  - `from_dict(dict)` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L62)
  - `get_task_brief_information(self)` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L51)
  - `get_task_information(self)` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L39)
  - `architecture` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L30)
  - `formulation` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L29)
  - `hyperparameters` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L32)
  - `model_type` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L34)
  - `training_hyperparameters` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L33)
  - `variables` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L31)
- protocol/private: `__init__`[`L16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L16), `__repr__`[`L65`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L65)
- uses (calls/refs, reference-scoped): [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask), [`name`](../../../core/experiment.md#AbsTask.name), [`description`](../../../core/experiment.md#Task.description), [`__init__`](../CoSTEER/task.md#CoSTEERTask.__init__)
- used by: [`_obj_to_json`](../../../log/ui/storage.md#WebStorage._obj_to_json), [`develop`](../../../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../../../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask), [`implement_one_task`](evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`evaluate`](eva_utils.md#ModelCodeEvaluator.evaluate), [`evaluate`](evaluators.md#ModelCoSTEEREvaluator.evaluate), [`evaluate`](eva_utils.md#ModelFinalEvaluator.evaluate), [`QlibModelExperiment`](../../../scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment), [`tasks_window`](../../../log/ui/app.md#tasks_window), [`consume_msg`](../../../log/ui/web.md#ResearchWindow.consume_msg), [`develop`](../../../scenarios/kaggle/developer/coder.md#KGModelFeatureSelectionCoder.develop), [`convert_model_experiment`](../../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_model_experiment), [`KGModelExperiment`](../../../scenarios/kaggle/experiment/kaggle_experiment.md#KGModelExperiment), [`consume_msg`](../../../log/ui/web.md#ModelTaskWindow.consume_msg), [`convert_response`](../../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.convert_response), [`ModelTaskLoader`](../../loader/task_loader.md#ModelTaskLoader), [`load`](../../loader/task_loader.md#ModelWsLoader.load), [`QlibModelExperiment`](../../../scenarios/qlib/experiment/quant_experiment.md#QlibModelExperiment), [`ModelWsLoader`](../../loader/task_loader.md#ModelWsLoader), [`load`](task_loader.md#ModelExperimentLoaderFromDict.load), [`load`](../../loader/task_loader.md#ModelTaskLoaderJson.load)

## Module values
- `ModelExperiment` — [`L163`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/model.py#L163)

