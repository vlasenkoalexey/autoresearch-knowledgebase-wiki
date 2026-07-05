---
title: 'Module: rdagent/scenarios/qlib/developer/model_runner.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/developer/model_runner.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.developer.model_runner`/QlibModelRunner#
symbols:
  QlibModelRunner.develop: develop().
  QlibModelRunner: ''
---
# Module: [`rdagent/scenarios/qlib/developer/model_runner.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/model_runner.py)

## Classes
### `QlibModelRunner`  ·  implements/extends CachedRunner
- def: [`rdagent/scenarios/qlib/developer/model_runner.py:14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/model_runner.py#L14)
- doc: Docker run
- signature: `class QlibModelRunner(CachedRunner[QlibModelExperiment]):`
- members:
  - `develop(self, exp: QlibModelExperiment)` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/model_runner.py#L28)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`error`](../../../log/logger.md#RDAgentLog.error), [`result`](../../../core/experiment.md#Experiment.result), [`QlibFactorExperiment`](../experiment/factor_experiment.md#QlibFactorExperiment), [`process_factor_data`](utils.md#process_factor_data), [`execute`](../experiment/workspace.md#QlibFBWorkspace.execute), [`name`](../../../core/experiment.md#AbsTask.name), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`QlibModelExperiment`](../experiment/model_experiment.md#QlibModelExperiment), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner), [`ModelEmptyError`](../../../core/exception.md#ModelEmptyError), [`get_cache_key`](../../../components/runner/__init__.md#CachedRunner.get_cache_key), [`model_type`](../../../components/coder/model_coder/model.md#ModelTask.model_type), [`assign_cached_result`](../../../components/runner/__init__.md#CachedRunner.assign_cached_result), [`ModelBasePropSetting`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting), [`training_hyperparameters`](../../../components/coder/model_coder/model.md#ModelTask.training_hyperparameters), [`base_features`](../experiment/model_experiment.md#QlibModelExperiment.base_features), [`test_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.test_end), [`test_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.test_start), [`train_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.train_end), [`train_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.train_start), [`valid_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.valid_end), [`valid_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.valid_start), [`stdout`](../experiment/model_experiment.md#QlibModelExperiment.stdout)
- used by: [`develop`](../../../core/developer.md#Developer.develop), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner)

