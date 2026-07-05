---
title: 'Module: rdagent/scenarios/qlib/developer/factor_runner.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/developer/factor_runner.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.developer.factor_runner`/
symbols:
  QlibFactorRunner.develop: QlibFactorRunner#develop().
  QlibFactorRunner: QlibFactorRunner#
  QlibFactorRunner.deduplicate_new_factors: QlibFactorRunner#deduplicate_new_factors().
  QlibFactorRunner.calculate_information_coefficient: QlibFactorRunner#calculate_information_coefficient().
  DIRNAME: DIRNAME.
  DIRNAME_local: DIRNAME_local.
---
# Module: [`rdagent/scenarios/qlib/developer/factor_runner.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py)

## Classes
### `QlibFactorRunner`  ·  implements/extends CachedRunner
- def: [`rdagent/scenarios/qlib/developer/factor_runner.py:25`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L25)
- doc: Docker run
- signature: `class QlibFactorRunner(CachedRunner[QlibFactorExperiment]):`
- members:
  - `calculate_information_coefficient(self, concat_feature: pd.DataFrame, SOTA_feature_column_size: int, new_feature_columns_size: int)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L35)
  - `deduplicate_new_factors(self, SOTA_feature: pd.DataFrame, new_feature: pd.DataFrame)` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L46)
  - `develop(self, exp: QlibFactorExperiment)` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L64) — Generate the experiment by processing and combining factor data,
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`error`](../../../log/logger.md#RDAgentLog.error), [`result`](../../../core/experiment.md#Experiment.result), [`QlibFactorExperiment`](../experiment/factor_experiment.md#QlibFactorExperiment), [`process_factor_data`](utils.md#process_factor_data), [`execute`](../experiment/workspace.md#QlibFBWorkspace.execute), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`QlibModelExperiment`](../experiment/model_experiment.md#QlibModelExperiment), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner), [`FactorEmptyError`](../../../core/exception.md#FactorEmptyError), [`get_cache_key`](../../../components/runner/__init__.md#CachedRunner.get_cache_key), [`model_type`](../../../components/coder/model_coder/model.md#ModelTask.model_type), [`assign_cached_result`](../../../components/runner/__init__.md#CachedRunner.assign_cached_result), [`FactorBasePropSetting`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting), [`base_features`](../experiment/factor_experiment.md#QlibFactorExperiment.base_features), [`training_hyperparameters`](../../../components/coder/model_coder/model.md#ModelTask.training_hyperparameters), [`test_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.test_end), [`base_feature_codes`](../experiment/factor_experiment.md#QlibFactorExperiment.base_feature_codes), [`test_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.test_start), [`train_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.train_end), [`train_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.train_start), [`valid_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.valid_end), [`valid_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.valid_start), [`stdout`](../experiment/factor_experiment.md#QlibFactorExperiment.stdout)
- used by: [`develop`](../../../core/developer.md#Developer.develop), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner)

## Module values
- `DIRNAME` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L19)
- `DIRNAME_local` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/factor_runner.py#L20)

