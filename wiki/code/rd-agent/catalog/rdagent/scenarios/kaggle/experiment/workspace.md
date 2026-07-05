---
title: 'Module: rdagent/scenarios/kaggle/experiment/workspace.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/workspace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.workspace`/KG
symbols:
  KGFBWorkspace.execute: FBWorkspace#execute().
  KGFBWorkspace.generate_preprocess_data: FBWorkspace#generate_preprocess_data().
  KGFBWorkspace: FBWorkspace#
  KGFBWorkspace.data_description: FBWorkspace#data_description.
  KGFBWorkspace.__init__: FBWorkspace#__init__().
  KGFBWorkspace.model_description: FBWorkspace#model_description().
  KG_FEATURE_PREPROCESS_SCRIPT: _FEATURE_PREPROCESS_SCRIPT.
---
# Module: [`rdagent/scenarios/kaggle/experiment/workspace.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py)

## Classes
### `KGFBWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/scenarios/kaggle/experiment/workspace.py:28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L28)
- signature: `class KGFBWorkspace(FBWorkspace):`
- members:
  - `execute(self, run_env: dict = {}, *args, **kwargs)` — [`L72`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L72)
  - `generate_preprocess_data(self)` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L42)
  - `model_description(self)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L35)
  - `data_description` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L32)
- protocol/private: `__init__`[`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L29)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`error`](../../../log/logger.md#RDAgentLog.error), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`prepare`](../../../utils/env.md#DockerEnv.prepare), [`local_data_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`check_output`](../../../utils/env.md#Env.check_output), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`KGDockerEnv`](../../../utils/env.md#KGDockerEnv), [`__init__`](../../../core/experiment.md#FBWorkspace.__init__), [`dump_python_code_run_and_get_results`](../../../utils/env.md#Env.dump_python_code_run_and_get_results), [`inject_code_from_folder`](../../../core/experiment.md#FBWorkspace.inject_code_from_folder), [`KG_FEATURE_PREPROCESS_SCRIPT`](workspace.md#KG_FEATURE_PREPROCESS_SCRIPT)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`develop`](../developer/runner.md#KGFactorRunner.develop), [`develop`](../developer/runner.md#KGModelRunner.develop), [`execute`](../../../core/experiment.md#FBWorkspace.execute), [`develop`](../developer/coder.md#KGModelFeatureSelectionCoder.develop), [`init_develop`](../developer/runner.md#KGCachedRunner.init_develop), [`__init__`](kaggle_experiment.md#KGFactorExperiment.__init__), [`__init__`](kaggle_experiment.md#KGModelExperiment.__init__), [`KGModelExperiment`](kaggle_experiment.md#KGModelExperiment), [`KGFactorExperiment`](kaggle_experiment.md#KGFactorExperiment), [`source_data`](scenario.md#KGScenario.source_data)  (1 test-only)

## Module values
- `KG_FEATURE_PREPROCESS_SCRIPT` — [`L13`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/workspace.py#L13)

