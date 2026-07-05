---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.sf-crime.fea_share_preprocess`/prepr
symbols:
  preprocess_script: ocess_script().
  prepreprocess: eprocess().
  preprocess_transform: ocess_transform().
  prepreprocess.feature_engineering: eprocess().feature_engineering().
  preprocess_fit: ocess_fit().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py)

## Functions
- `feature_engineering(data)` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py#L32)
- `prepreprocess()` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py#L11) — This method loads the data, drops the unnecessary columns, and splits it into train and validation sets.
- `preprocess_fit(X_train: pd.DataFrame)` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py#L69) — Fits the preprocessor on the training data and returns the fitted preprocessor.
- `preprocess_script()` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py#L101) — This method applies the preprocessing steps to the training, validation, and test datasets.
- `preprocess_transform(X: pd.DataFrame, preprocessor)` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/fea_share_preprocess.py#L88) — Transforms the given DataFrame using the fitted preprocessor.

