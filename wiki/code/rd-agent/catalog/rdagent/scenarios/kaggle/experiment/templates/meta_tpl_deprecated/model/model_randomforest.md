---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.meta_tpl_deprecated.model.model_randomforest`/
symbols:
  select: select().
  fit: fit().
  predict: predict().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py)

## Functions
- `fit(X_train: pd.DataFrame, y_train: pd.Series, X_valid: pd.DataFrame, y_valid: pd.Series)` — [`L21`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py#L21) — Define and train the Random Forest model. Merge feature selection into the pipeline.
- `predict(model, X)` — [`L43`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py#L43) — Keep feature selection's consistency and make predictions.
- `select(X: pd.DataFrame)` — [`L13`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/model/model_randomforest.py#L13) — Select relevant features. To be used in fit & predict function.

