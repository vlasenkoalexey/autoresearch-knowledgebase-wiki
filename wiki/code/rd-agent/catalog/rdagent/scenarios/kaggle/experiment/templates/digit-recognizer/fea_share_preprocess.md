---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.digit-recognizer.fea_share_preprocess`/
symbols:
  preprocess_script: preprocess_script().
  clean_and_impute_data: clean_and_impute_data().
  prepreprocess: prepreprocess().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py)

## Functions
- `clean_and_impute_data(X_train, X_valid, X_test)` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py#L54) — Handles inf and -inf values by replacing them with NaN,
- `prepreprocess()` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py#L9) — This method loads the data, drops the unnecessary columns, and splits it into train and validation sets.
- `preprocess_script()` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/fea_share_preprocess.py#L26) — This method applies the preprocessing steps to the training, validation, and test datasets.

