---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.meta_tpl_deprecated.model.model_nn`/
symbols:
  FeatureInteractionModel.forward: FeatureInteractionModel#forward().
  fit: fit().
  device: device.
  FeatureInteractionModel.__init__: FeatureInteractionModel#__init__().
  predict: predict().
  FeatureInteractionModel: FeatureInteractionModel#
  FeatureInteractionModel.fc1: FeatureInteractionModel#fc1.
  FeatureInteractionModel.bn1: FeatureInteractionModel#bn1.
  FeatureInteractionModel.fc2: FeatureInteractionModel#fc2.
  FeatureInteractionModel.bn2: FeatureInteractionModel#bn2.
  FeatureInteractionModel.fc3: FeatureInteractionModel#fc3.
  FeatureInteractionModel.dropout: FeatureInteractionModel#dropout.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py)

## Classes
### `FeatureInteractionModel`
- def: [`rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py:13`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L13)
- signature: `class FeatureInteractionModel(nn.Module):`
- members:
  - `forward(self, x)` — [`L23`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L23)
  - `bn1` — [`L17`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L17)
  - `bn2` — [`L19`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L19)
  - `dropout` — [`L21`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L21)
  - `fc1` — [`L16`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L16)
  - `fc2` — [`L18`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L18)
  - `fc3` — [`L20`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L20)
- protocol/private: `__init__`[`L14`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L14)
- used by: [`fit`](model_nn.md#fit)

## Functions
- `fit(X_train, y_train, X_valid, y_valid)` — [`L32`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L32)
- `predict(model, X)` — [`L67`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L67)

## Module values
- `device` — [`L9`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_nn.py#L9)

