---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.tabular-playground-series-dec-2021.fea_share_preprocess`/
symbols:
  preprocess_script: preprocess_script().
  index_col_name: index_col_name.
  prepreprocess: prepreprocess().
  clean_and_impute_data: clean_and_impute_data().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py)

## Functions
- `clean_and_impute_data(X_train, X_valid, X_test)` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py#L62) — Handles inf and -inf values by replacing them with NaN,
- `prepreprocess()` — [`L12`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py#L12) — This method loads the data, drops the unnecessary columns, and splits it into train and validation sets.
- `preprocess_script()` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py#L29) — This method applies the preprocessing steps to the training, validation, and test datasets.

## Module values
- `index_col_name` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/fea_share_preprocess.py#L9)

