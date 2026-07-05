---
title: 'Module: rdagent/components/loader/experiment_loader.py'
type: catalog
provenance: extracted
module: rdagent/components/loader/experiment_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.loader.experiment_loader`/
symbols:
  FactorExperimentLoader: FactorExperimentLoader#
  ModelExperimentLoader: ModelExperimentLoader#
---
# Module: [`rdagent/components/loader/experiment_loader.py`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/experiment_loader.py)

## Classes
### `FactorExperimentLoader`  ·  implements/extends Loader
- def: [`rdagent/components/loader/experiment_loader.py:5`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/experiment_loader.py#L5)
- signature: `class FactorExperimentLoader(Loader[FactorExperiment]):`
- uses (calls/refs, reference-scoped): [`Loader`](../../core/experiment.md#Loader), [`FactorExperiment`](../coder/factor_coder/factor.md#FactorExperiment), [`FactorExperimentLoaderFromDict`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromDict), [`FactorExperimentLoaderFromPDFfiles`](../../scenarios/qlib/factor_experiment_loader/pdf_loader.md#FactorExperimentLoaderFromPDFfiles), [`FactorExperimentLoaderFromJsonFile`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonFile), [`FactorExperimentLoaderFromJsonString`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonString)
- used by: [`Loader`](../../core/experiment.md#Loader), [`FactorExperimentLoaderFromDict`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromDict), [`FactorExperimentLoaderFromPDFfiles`](../../scenarios/qlib/factor_experiment_loader/pdf_loader.md#FactorExperimentLoaderFromPDFfiles), [`FactorExperimentLoaderFromJsonFile`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonFile), [`FactorExperimentLoaderFromJsonString`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromJsonString)

### `ModelExperimentLoader`  ·  implements/extends Loader
- def: [`rdagent/components/loader/experiment_loader.py:9`](../../../../../../../raw/code/rd-agent/rdagent/components/loader/experiment_loader.py#L9)
- signature: `class ModelExperimentLoader(Loader[FactorExperiment]):`
- uses (calls/refs, reference-scoped): [`Loader`](../../core/experiment.md#Loader), [`FactorExperiment`](../coder/factor_coder/factor.md#FactorExperiment)
- used by: [`Loader`](../../core/experiment.md#Loader)

