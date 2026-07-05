---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.sf-crime.model.model_randomforest`/
symbols:
  fit: fit().
  predict: predict().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py)

## Functions
- `fit(X_train: pd.DataFrame, y_train: pd.Series, X_valid: pd.DataFrame, y_valid: pd.Series)` — [`L12`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py#L12) — Define and train the Random Forest model. Merge feature selection into the pipeline.
- `predict(model, X)` — [`L25`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/model/model_randomforest.py#L25) — Keep feature selection's consistency and make predictions.

