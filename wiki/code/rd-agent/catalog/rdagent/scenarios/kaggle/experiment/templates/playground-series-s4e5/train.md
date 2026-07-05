---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.playground-series-s4e5.train`/
symbols:
  X_test_f: X_test_f.
  model_name: model_name.
  r2: r2.
  cls: cls.
  predict_func: predict_func.
  imputer: imputer.
  f: f.
  model_l: model_l.
  select_m: select_m.
  max_index: max_index.
  X_train: X_train.
  X_valid: X_valid.
  y_valid_pred: y_valid_pred.
  X_test_selected: X_test_selected.
  y_test_pred: y_test_pred.
  submission_result: submission_result.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_test: X_test.
  X_valid_f: X_valid_f.
  m: m.
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
  compute_r2: compute_r2().
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py)

## Functions
- `compute_r2(y_true, y_pred)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L17) — Compute R² score for regression.
- `import_module_from_path(module_name, module_path)` — [`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L22)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L11)
- `X_test` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `X_test_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L41)
- `X_test_l` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L34)
- `X_test_selected` — [`L94`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L94)
- `X_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `X_train_f` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L39)
- `X_train_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L33)
- `X_train_selected` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L73)
- `X_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `X_valid_f` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L40)
- `X_valid_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L33)
- `X_valid_selected` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L74)
- `cls` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L37)
- `f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L36)
- `ids` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `imputer` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L61)
- `m` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L76)
- `max_index` — [`L90`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L90)
- `metrics_all` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L81)
- `model` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L82)
- `model_l` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L69)
- `model_name` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L77)
- `predict_func` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L82)
- `r2` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L85)
- `select_m` — [`L72`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L72)
- `select_python_path` — [`L71`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L71)
- `submission_result` — [`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L98)
- `y_test_pred` — [`L95`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L95)
- `y_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `y_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L30)
- `y_valid_pred` — [`L84`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e5/train.py#L84)

