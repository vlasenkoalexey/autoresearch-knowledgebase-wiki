---
title: 'Module: rdagent/components/loader/task_loader.py'
type: catalog
provenance: extracted
module: rdagent/components/loader/task_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.loader.task_loader`/
symbols:
  ModelTaskLoader: ModelTaskLoader#
  ModelWsLoader.load: ModelWsLoader#load().
  ModelWsLoader: ModelWsLoader#
  ModelTaskLoaderJson.load: ModelTaskLoaderJson#load().
  FactorTaskLoader: FactorTaskLoader#
  ModelTaskLoaderJson: ModelTaskLoaderJson#
  ModelTaskLoaderJson.json_uri: ModelTaskLoaderJson#json_uri.
  ModelWsLoader.path: ModelWsLoader#path.
  ModelTaskLoaderJson.__init__: ModelTaskLoaderJson#__init__().
  ModelWsLoader.__init__: ModelWsLoader#__init__().
---
# Module: [`rdagent/components/loader/task_loader.py`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py)

## Classes
### `FactorTaskLoader`  ·  implements/extends Loader
- def: [`rdagent/components/loader/task_loader.py:10`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L10)
- signature: `class FactorTaskLoader(Loader[FactorTask]):`
- uses (calls/refs, reference-scoped): [`FactorTask`](../coder/factor_coder/factor.md#FactorTask), [`Loader`](../../core/experiment.md#Loader)
- used by: [`Loader`](../../core/experiment.md#Loader)

### `ModelTaskLoader`  ·  implements/extends Loader
- def: [`rdagent/components/loader/task_loader.py:14`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L14)
- signature: `class ModelTaskLoader(Loader[ModelTask]):`
- uses (calls/refs, reference-scoped): [`ModelTask`](../coder/model_coder/model.md#ModelTask), [`Loader`](../../core/experiment.md#Loader), [`ModelExperimentLoaderFromPDFfiles`](../coder/model_coder/task_loader.md#ModelExperimentLoaderFromPDFfiles), [`ModelTaskLoaderJson`](task_loader.md#ModelTaskLoaderJson), [`ModelExperimentLoaderFromDict`](../coder/model_coder/task_loader.md#ModelExperimentLoaderFromDict)
- used by: [`Loader`](../../core/experiment.md#Loader), [`ModelExperimentLoaderFromPDFfiles`](../coder/model_coder/task_loader.md#ModelExperimentLoaderFromPDFfiles), [`ModelTaskLoaderJson`](task_loader.md#ModelTaskLoaderJson), [`ModelExperimentLoaderFromDict`](../coder/model_coder/task_loader.md#ModelExperimentLoaderFromDict)

### `ModelTaskLoaderJson`  ·  implements/extends ModelTaskLoader
- def: [`rdagent/components/loader/task_loader.py:18`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L18)
- signature: `class ModelTaskLoaderJson(ModelTaskLoader):`
- members:
  - `load(self, *argT, **kwargs)` — [`L48`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L48)
  - `json_uri` — [`L46`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L46)
- protocol/private: `__init__`[`L44`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L44)
- uses (calls/refs, reference-scoped): [`ModelTask`](../coder/model_coder/model.md#ModelTask), [`ModelTaskLoader`](task_loader.md#ModelTaskLoader)
- used by: [`load`](../../core/experiment.md#Loader.load), [`ModelTaskLoader`](task_loader.md#ModelTaskLoader)  (2 test-only)

### `ModelWsLoader`  ·  implements/extends WsLoader
- def: [`rdagent/components/loader/task_loader.py:85`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L85)
- signature: `class ModelWsLoader(WsLoader[ModelTask, ModelFBWorkspace]):`
- members:
  - `load(self, task: ModelTask)` — [`L89`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L89)
  - `path` — [`L87`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L87)
- protocol/private: `__init__`[`L86`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/task_loader.py#L86)
- uses (calls/refs, reference-scoped): [`inject_files`](../../core/experiment.md#FBWorkspace.inject_files), [`ModelTask`](../coder/model_coder/model.md#ModelTask), [`ModelFBWorkspace`](../coder/model_coder/model.md#ModelFBWorkspace), [`name`](../../core/experiment.md#AbsTask.name), [`prepare`](../../core/experiment.md#FBWorkspace.prepare), [`WsLoader`](../../core/experiment.md#WsLoader)
- used by: [`WsLoader`](../../core/experiment.md#WsLoader), [`load`](../../core/experiment.md#WsLoader.load)  (2 test-only)

