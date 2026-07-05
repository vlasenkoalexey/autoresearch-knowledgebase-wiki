---
title: 'Module: rdagent/scenarios/kaggle/developer/runner.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/developer/runner.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.developer.runner`/KG
symbols:
  KGFactorRunner.develop: FactorRunner#develop().
  KGModelRunner.develop: ModelRunner#develop().
  KGCachedRunner.init_develop: CachedRunner#init_develop().
  KGCachedRunner: CachedRunner#
  KGCachedRunner.get_cache_key: CachedRunner#get_cache_key().
  KGCachedRunner.assign_cached_result: CachedRunner#assign_cached_result().
  KGModelRunner: ModelRunner#
  KGFactorRunner: FactorRunner#
---
# Module: [`rdagent/scenarios/kaggle/developer/runner.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py)

## Classes
### `KGCachedRunner`  ·  implements/extends CachedRunner
- def: [`rdagent/scenarios/kaggle/developer/runner.py:17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L17)
- signature: `class KGCachedRunner(CachedRunner[ASpecificExp]):`
- members:
  - `assign_cached_result(self, exp: Experiment, cached_res: Experiment)` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L28)
  - `get_cache_key(self, exp: ASpecificExp)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L18)
  - `init_develop(self, exp: KGFactorExperiment | KGModelExperiment)` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L41) — For the initial development, the experiment serves as a benchmark for feature engineering.
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../core/experiment.md#Experiment), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`result`](../../../core/experiment.md#Experiment.result), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`execute`](../experiment/workspace.md#KGFBWorkspace.execute), [`md5_hash`](../../../utils/__init__.md#md5_hash), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner), [`KGModelExperiment`](../experiment/kaggle_experiment.md#KGModelExperiment), [`ASpecificExp`](../../../core/experiment.md#ASpecificExp), [`KGFactorExperiment`](../experiment/kaggle_experiment.md#KGFactorExperiment), [`get_cache_key`](../../../components/runner/__init__.md#CachedRunner.get_cache_key), [`assign_cached_result`](../../../components/runner/__init__.md#CachedRunner.assign_cached_result), [`KGFactorRunner`](runner.md#KGFactorRunner), [`KGModelRunner`](runner.md#KGModelRunner), [`sub_results`](../../../core/experiment.md#Experiment.sub_results)
- used by: [`develop`](runner.md#KGFactorRunner.develop), [`develop`](runner.md#KGModelRunner.develop), [`CachedRunner`](../../../components/runner/__init__.md#CachedRunner), [`get_cache_key`](../../../components/runner/__init__.md#CachedRunner.get_cache_key), [`assign_cached_result`](../../../components/runner/__init__.md#CachedRunner.assign_cached_result), [`KGFactorRunner`](runner.md#KGFactorRunner), [`KGModelRunner`](runner.md#KGModelRunner)

### `KGFactorRunner`  ·  implements/extends KGCachedRunner
- def: [`rdagent/scenarios/kaggle/developer/runner.py:94`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L94)
- signature: `class KGFactorRunner(KGCachedRunner[KGFactorExperiment]):`
- members:
  - `develop(self, exp: KGFactorExperiment)` — [`L96`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L96) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- uses (calls/refs, reference-scoped): [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`execute`](../../../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`CoderError`](../../../core/exception.md#CoderError), [`result`](../../../core/experiment.md#Experiment.result), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`init_develop`](runner.md#KGCachedRunner.init_develop), [`execute`](../experiment/workspace.md#KGFBWorkspace.execute), [`target_task`](../../../core/experiment.md#Workspace.target_task), [`KGFactorExperiment`](../experiment/kaggle_experiment.md#KGFactorExperiment), [`FactorEmptyError`](../../../core/exception.md#FactorEmptyError), [`KGCachedRunner`](runner.md#KGCachedRunner), [`get_cache_key`](runner.md#KGCachedRunner.get_cache_key), [`assign_cached_result`](runner.md#KGCachedRunner.assign_cached_result), [`data_description`](../experiment/workspace.md#KGFBWorkspace.data_description), [`sub_results`](../../../core/experiment.md#Experiment.sub_results)
- used by: [`develop`](../../../core/developer.md#Developer.develop), [`KGCachedRunner`](runner.md#KGCachedRunner)

### `KGModelRunner`  ·  implements/extends KGCachedRunner
- def: [`rdagent/scenarios/kaggle/developer/runner.py:60`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L60)
- signature: `class KGModelRunner(KGCachedRunner[KGModelExperiment]):`
- members:
  - `develop(self, exp: KGModelExperiment)` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/runner.py#L62)
- uses (calls/refs, reference-scoped): [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`CoderError`](../../../core/exception.md#CoderError), [`result`](../../../core/experiment.md#Experiment.result), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`init_develop`](runner.md#KGCachedRunner.init_develop), [`execute`](../experiment/workspace.md#KGFBWorkspace.execute), [`target_task`](../../../core/experiment.md#Workspace.target_task), [`KGModelExperiment`](../experiment/kaggle_experiment.md#KGModelExperiment), [`ModelEmptyError`](../../../core/exception.md#ModelEmptyError), [`KGCachedRunner`](runner.md#KGCachedRunner), [`get_cache_key`](runner.md#KGCachedRunner.get_cache_key), [`assign_cached_result`](runner.md#KGCachedRunner.assign_cached_result), [`sub_results`](../../../core/experiment.md#Experiment.sub_results)
- used by: [`develop`](../../../core/developer.md#Developer.develop), [`KGCachedRunner`](runner.md#KGCachedRunner)

