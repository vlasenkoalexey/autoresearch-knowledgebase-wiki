---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.new-york-city-taxi-fare-prediction.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  cls: cls.
  rmse: rmse.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  submission_result: submission_result.
  min_index: min_index.
  y_valid_pred: y_valid_pred.
  X_test_selected: X_test_selected.
  y_test_pred: y_test_pred.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train: X_train.
  X_valid: X_valid.
  X_train_selected: X_train_selected.
  X_test: X_test.
  SEED: SEED.
  select_python_path: select_python_path.
  ids: ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  y_train: y_train.
  model: model.
  compute_metrics_for_classification: compute_metrics_for_classification().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L17) — Compute MCC for classification.
- `import_module_from_path(module_name, module_path)` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L23)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L11)
- `X_test` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `X_test_f` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L42)
- `X_test_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L35)
- `X_test_selected` — [`L83`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L83)
- `X_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `X_train_f` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L40)
- `X_train_l` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L34)
- `X_train_selected` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L63)
- `X_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `X_valid_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L41)
- `X_valid_l` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L34)
- `X_valid_selected` — [`L64`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L64)
- `cls` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L38)
- `f` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L37)
- `ids` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `m` — [`L66`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L66)
- `metrics_all` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L70)
- `min_index` — [`L79`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L79)
- `model` — [`L71`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L71)
- `model_l` — [`L59`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L59)
- `predict_func` — [`L71`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L71)
- `rmse` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L74)
- `select_m` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L62)
- `select_python_path` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L61)
- `submission_result` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L88)
- `y_test_pred` — [`L84`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L84)
- `y_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `y_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L31)
- `y_valid_pred` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/new-york-city-taxi-fare-prediction/train.py#L73)

