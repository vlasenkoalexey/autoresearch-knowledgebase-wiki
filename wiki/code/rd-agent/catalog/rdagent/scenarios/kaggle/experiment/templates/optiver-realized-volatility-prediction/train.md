---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.optiver-realized-volatility-prediction.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  metrics: metrics.
  cls: cls.
  imputer: imputer.
  X_train: X_train.
  X_valid: X_valid.
  X_test: X_test.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  min_index: min_index.
  y_valid_pred: y_valid_pred.
  X_test_selected: X_test_selected.
  y_test_pred: y_test_pred.
  submission_result: submission_result.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
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
  compute_rmspe: compute_rmspe().
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py)

## Functions
- `compute_rmspe(y_true, y_pred)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L17) — Compute Root Mean Squared Percentage Error (RMSPE) for regression.
- `import_module_from_path(module_name, module_path)` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L23)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L11)
- `X_test` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `X_test_f` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L43)
- `X_test_l` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L36)
- `X_test_selected` — [`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L98)
- `X_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `X_train_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L41)
- `X_train_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L35)
- `X_train_selected` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L78)
- `X_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `X_valid_f` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L42)
- `X_valid_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L35)
- `X_valid_selected` — [`L79`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L79)
- `cls` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L39)
- `f` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L38)
- `ids` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `imputer` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L61)
- `m` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L81)
- `metrics` — [`L89`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L89)
- `metrics_all` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L85)
- `min_index` — [`L94`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L94)
- `model` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L86)
- `model_l` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L74)
- `predict_func` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L86)
- `select_m` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L77)
- `select_python_path` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L76)
- `submission_result` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L101)
- `y_test_pred` — [`L99`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L99)
- `y_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `y_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L31)
- `y_valid_pred` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/optiver-realized-volatility-prediction/train.py#L88)

