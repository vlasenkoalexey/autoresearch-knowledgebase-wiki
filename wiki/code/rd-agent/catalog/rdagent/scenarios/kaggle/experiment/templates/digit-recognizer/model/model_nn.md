---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.digit-recognizer.model.model_nn`/
symbols:
  NeuralNetwork.forward: NeuralNetwork#forward().
  device: device.
  fit: fit().
  NeuralNetwork.__init__: NeuralNetwork#__init__().
  predict: predict().
  NeuralNetwork: NeuralNetwork#
  NeuralNetwork.conv1: NeuralNetwork#conv1.
  NeuralNetwork.dropout1: NeuralNetwork#dropout1.
  NeuralNetwork.conv2: NeuralNetwork#conv2.
  NeuralNetwork.dropout2: NeuralNetwork#dropout2.
  NeuralNetwork.flatten: NeuralNetwork#flatten.
  NeuralNetwork.fc1: NeuralNetwork#fc1.
  NeuralNetwork.fc2: NeuralNetwork#fc2.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py)

## Classes
### `NeuralNetwork`
- def: [`rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py:12`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L12)
- signature: `class NeuralNetwork(nn.Module):`
- members:
  - `forward(self, x)` — [`L23`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L23)
  - `conv1` — [`L15`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L15)
  - `conv2` — [`L17`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L17)
  - `dropout1` — [`L16`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L16)
  - `dropout2` — [`L18`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L18)
  - `fc1` — [`L20`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L20)
  - `fc2` — [`L21`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L21)
  - `flatten` — [`L19`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L19)
- protocol/private: `__init__`[`L13`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L13)
- used by: [`fit`](model_nn.md#fit)

## Functions
- `fit(X_train: pd.DataFrame, y_train: pd.DataFrame, X_valid: pd.DataFrame, y_valid: pd.DataFrame)` — [`L34`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L34)
- `predict(model, X)` — [`L82`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L82)

## Module values
- `device` — [`L8`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/model/model_nn.py#L8)

