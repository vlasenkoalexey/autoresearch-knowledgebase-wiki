---
title: 'Module: rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.factor_experiment_loader.json_loader`/Factor
symbols:
  FactorTestCaseLoaderFromJsonFile.load: TestCaseLoaderFromJsonFile#load().
  FactorExperimentLoaderFromDict.load: ExperimentLoaderFromDict#load().
  FactorExperimentLoaderFromDict: ExperimentLoaderFromDict#
  FactorExperimentLoaderFromJsonFile.load: ExperimentLoaderFromJsonFile#load().
  FactorExperimentLoaderFromJsonString.load: ExperimentLoaderFromJsonString#load().
  FactorExperimentLoaderFromJsonFile: ExperimentLoaderFromJsonFile#
  FactorExperimentLoaderFromJsonString: ExperimentLoaderFromJsonString#
  FactorTestCaseLoaderFromJsonFile: TestCaseLoaderFromJsonFile#
---
# Module: [`rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py)

## Classes
### `FactorExperimentLoaderFromDict`  ·  implements/extends FactorExperimentLoader
- def: [`rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py:15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L15)
- signature: `class FactorExperimentLoaderFromDict(FactorExperimentLoader):`
- members:
  - `load(self, factor_dict: dict)` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L16) — Load data from a dict.
- uses (calls/refs, reference-scoped): [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`QlibFactorExperiment`](../experiment/factor_experiment.md#QlibFactorExperiment), [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader)
- used by: [`load`](pdf_loader.md#FactorExperimentLoaderFromPDFfiles.load), [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](../../../core/experiment.md#Loader.load), [`load`](json_loader.md#FactorExperimentLoaderFromJsonFile.load), [`load`](json_loader.md#FactorExperimentLoaderFromJsonString.load)

### `FactorExperimentLoaderFromJsonFile`  ·  implements/extends FactorExperimentLoader
- def: [`rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py:31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L31)
- signature: `class FactorExperimentLoaderFromJsonFile(FactorExperimentLoader):`
- members:
  - `load(self, json_file_path: Path)` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L32)
- uses (calls/refs, reference-scoped): [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](json_loader.md#FactorExperimentLoaderFromDict.load), [`FactorExperimentLoaderFromDict`](json_loader.md#FactorExperimentLoaderFromDict)
- used by: [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](../../../core/experiment.md#Loader.load)

### `FactorExperimentLoaderFromJsonString`  ·  implements/extends FactorExperimentLoader
- def: [`rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py:38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L38)
- signature: `class FactorExperimentLoaderFromJsonString(FactorExperimentLoader):`
- members:
  - `load(self, json_string: str)` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L39)
- uses (calls/refs, reference-scoped): [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](json_loader.md#FactorExperimentLoaderFromDict.load), [`FactorExperimentLoaderFromDict`](json_loader.md#FactorExperimentLoaderFromDict)
- used by: [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](../../../core/experiment.md#Loader.load)

### `FactorTestCaseLoaderFromJsonFile`
- def: [`rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py:46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L46)
- signature: `class FactorTestCaseLoaderFromJsonFile:`
- members:
  - `load(self, json_file_path: Path)` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/json_loader.py#L47)
- uses (calls/refs, reference-scoped): [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`FactorFBWorkspace`](../../../components/coder/factor_coder/factor.md#FactorFBWorkspace)  (3 test-only)
- used by: (1 test-only callers)

