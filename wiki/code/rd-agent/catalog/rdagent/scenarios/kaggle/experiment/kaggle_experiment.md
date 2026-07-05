---
title: 'Module: rdagent/scenarios/kaggle/experiment/kaggle_experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/kaggle_experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.kaggle_experiment`/KG
symbols:
  KGModelExperiment.__init__: ModelExperiment#__init__().
  KGFactorExperiment.__init__: FactorExperiment#__init__().
  KGModelExperiment: ModelExperiment#
  KGFactorExperiment: FactorExperiment#
  KG_SELECT_MAPPING: _SELECT_MAPPING.
  KG_MODEL_MAPPING: _MODEL_MAPPING.
  KG_MODEL_TYPE_XGBOOST: _MODEL_TYPE_XGBOOST.
  KG_MODEL_TYPE_RANDOMFOREST: _MODEL_TYPE_RANDOMFOREST.
  KG_MODEL_TYPE_LIGHTGBM: _MODEL_TYPE_LIGHTGBM.
  KG_MODEL_TYPE_NN: _MODEL_TYPE_NN.
---
# Module: [`rdagent/scenarios/kaggle/experiment/kaggle_experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py)

## Classes
### `KGFactorExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/kaggle/experiment/kaggle_experiment.py:61`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L61)
- signature: `class KGFactorExperiment(FeatureExperiment[FactorTask, KGFBWorkspace, FactorFBWorkspace]):`
- protocol/private: `__init__`[`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L62)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`FactorFBWorkspace`](../../../components/coder/factor_coder/factor.md#FactorFBWorkspace), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`get_task_information`](../../../components/coder/factor_coder/factor.md#FactorTask.get_task_information), [`KGFBWorkspace`](workspace.md#KGFBWorkspace), [`data_description`](workspace.md#KGFBWorkspace.data_description), [`FeatureExperiment`](../../../components/coder/factor_coder/factor.md#FeatureExperiment)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`develop`](../developer/runner.md#KGFactorRunner.develop), [`init_develop`](../developer/runner.md#KGCachedRunner.init_develop), [`source_data`](scenario.md#KGScenario.source_data), [`convert_feature_experiment`](../proposal/proposal.md#KGHypothesis2Experiment.convert_feature_experiment), [`KGFactorRunner`](../developer/runner.md#KGFactorRunner)

### `KGModelExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/kaggle/experiment/kaggle_experiment.py:37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L37)
- signature: `class KGModelExperiment(ModelExperiment[ModelTask, KGFBWorkspace, ModelFBWorkspace]):`
- protocol/private: `__init__`[`L38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L38)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`ModelTask`](../../../components/coder/model_coder/model.md#ModelTask), [`ModelFBWorkspace`](../../../components/coder/model_coder/model.md#ModelFBWorkspace), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`ModelExperiment`](../../../components/coder/model_coder/model.md#ModelExperiment), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`get_task_information`](../../../components/coder/factor_coder/factor.md#FactorTask.get_task_information), [`KGFBWorkspace`](workspace.md#KGFBWorkspace), [`data_description`](workspace.md#KGFBWorkspace.data_description)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`develop`](../developer/runner.md#KGModelRunner.develop), [`develop`](../developer/coder.md#KGModelFeatureSelectionCoder.develop), [`init_develop`](../developer/runner.md#KGCachedRunner.init_develop), [`convert_model_experiment`](../proposal/proposal.md#KGHypothesis2Experiment.convert_model_experiment), [`KGModelFeatureSelectionCoder`](../developer/coder.md#KGModelFeatureSelectionCoder), [`KGModelRunner`](../developer/runner.md#KGModelRunner)

## Module values
- `KG_MODEL_MAPPING` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L22)
- `KG_MODEL_TYPE_LIGHTGBM` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L19)
- `KG_MODEL_TYPE_NN` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L20)
- `KG_MODEL_TYPE_RANDOMFOREST` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L18)
- `KG_MODEL_TYPE_XGBOOST` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L17)
- `KG_SELECT_MAPPING` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/kaggle_experiment.py#L29)

