---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.new-york-city-taxi-fare-prediction.fea_share_preprocess`/
symbols:
  preprocess_script: preprocess_script().
  prepreprocess: prepreprocess().
  index_name: index_name.
  label_name: label_name.
  clean_and_impute_data: clean_and_impute_data().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py)

## Functions
- `clean_and_impute_data(X_train, X_valid, X_test)` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py#L53) — Handles inf and -inf values by replacing them with NaN,
- `prepreprocess()` — [`L12`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py#L12) — This method loads the data, drops the unnecessary columns, and splits it into train and validation sets.
- `preprocess_script()` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py#L29) — This method applies the preprocessing steps to the training, validation, and test datasets.

## Module values
- `index_name` — [`L8`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py#L8)
- `label_name` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/fea_share_preprocess.py#L9)

