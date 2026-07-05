---
title: 'Module: rdagent/components/runner/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/runner/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.runner`/CachedRunner#
symbols:
  CachedRunner: ''
  CachedRunner.get_cache_key: get_cache_key().
  CachedRunner.assign_cached_result: assign_cached_result().
---
# Module: [`rdagent/components/runner/__init__.py`](../../../../../../../raw/code/rd-agent/rdagent/components/runner/__init__.py)

## Classes
### `CachedRunner`  ·  implements/extends Developer
- def: [`rdagent/components/runner/__init__.py:6`](../../../../../../../raw/code/rd-agent/rdagent/components/runner/__init__.py#L6)
- signature: `class CachedRunner(Developer[ASpecificExp]):`
- members:
  - `assign_cached_result(self, exp: Experiment, cached_res: Experiment)` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/components/runner/__init__.py#L16)
  - `get_cache_key(self, exp: Experiment)` — [`L7`](../../../../../../../raw/code/rd-agent/rdagent/components/runner/__init__.py#L7)
- uses (calls/refs, reference-scoped): [`Experiment`](../../core/experiment.md#Experiment), [`based_experiments`](../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../core/experiment.md#Experiment.sub_tasks), [`Developer`](../../core/developer.md#Developer), [`result`](../../core/experiment.md#Experiment.result), [`md5_hash`](../../utils/__init__.md#md5_hash), [`ASpecificExp`](../../core/experiment.md#ASpecificExp), [`KGCachedRunner`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner), [`get_cache_key`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner.get_cache_key), [`assign_cached_result`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner.assign_cached_result), [`QlibFactorRunner`](../../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner), [`QlibModelRunner`](../../scenarios/qlib/developer/model_runner.md#QlibModelRunner)
- used by: [`develop`](../../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`Developer`](../../core/developer.md#Developer), [`init_develop`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner.init_develop), [`KGCachedRunner`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner), [`get_cache_key`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner.get_cache_key), [`assign_cached_result`](../../scenarios/kaggle/developer/runner.md#KGCachedRunner.assign_cached_result), [`QlibFactorRunner`](../../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner), [`QlibModelRunner`](../../scenarios/qlib/developer/model_runner.md#QlibModelRunner)

