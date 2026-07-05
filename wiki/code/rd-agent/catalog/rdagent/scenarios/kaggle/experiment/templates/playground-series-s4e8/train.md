---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.playground-series-s4e8.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  metrics: metrics.
  cls: cls.
  imputer: imputer.
  y_valid_pred: y_valid_pred.
  y_test_pred: y_test_pred.
  X_train: X_train.
  X_valid: X_valid.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  X_test: X_test.
  max_index: max_index.
  X_test_selected: X_test_selected.
  submission_result: submission_result.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  SEED: SEED.
  select_python_path: select_python_path.
  y_test_pred_labels: y_test_pred_labels.
  ids: ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  compute_metrics_for_classification: compute_metrics_for_classification().
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L18) — Compute MCC for classification.
- `import_module_from_path(module_name, module_path)` — [`L24`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L24)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L11)
- `X_test` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `X_test_f` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L43)
- `X_test_l` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L36)
- `X_test_selected` — [`L95`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L95)
- `X_train` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `X_train_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L41)
- `X_train_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L35)
- `X_train_selected` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L74)
- `X_valid` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `X_valid_f` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L42)
- `X_valid_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L35)
- `X_valid_selected` — [`L75`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L75)
- `cls` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L39)
- `f` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L38)
- `ids` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `imputer` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L58)
- `m` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L77)
- `max_index` — [`L91`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L91)
- `metrics` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L86)
- `metrics_all` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L81)
- `model` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L82)
- `model_l` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L70)
- `predict_func` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L82)
- `select_m` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L73)
- `select_python_path` — [`L72`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L72)
- `submission_result` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L102)
- `y_test_pred` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L96)
- `y_test_pred_labels` — [`L99`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L99)
- `y_train` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `y_valid` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L32)
- `y_valid_pred` — [`L84`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s4e8/train.py#L84)

