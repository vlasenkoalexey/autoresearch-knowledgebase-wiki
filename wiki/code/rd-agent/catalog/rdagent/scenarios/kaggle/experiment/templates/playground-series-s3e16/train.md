---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.playground-series-s3e16.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  cls: cls.
  metrics: metrics.
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
  X_train_selected: X_train_selected.
  select_python_path: select_python_path.
  X_train: X_train.
  X_valid: X_valid.
  X_train_l: X_train_l.
  ids: ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_test: X_test.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py)

## Functions
- `import_module_from_path(module_name, module_path)` — [`L12`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L12)

## Module values
- `DIRNAME` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L9)
- `X_test` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `X_test_f` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L31)
- `X_test_l` — [`L24`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L24)
- `X_test_selected` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L69)
- `X_train` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `X_train_f` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L29)
- `X_train_l` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L23)
- `X_train_selected` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L49)
- `X_valid` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `X_valid_f` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L30)
- `X_valid_l` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L23)
- `X_valid_selected` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L50)
- `cls` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L27)
- `f` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L26)
- `ids` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `m` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L52)
- `metrics` — [`L60`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L60)
- `metrics_all` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L56)
- `min_index` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L65)
- `model` — [`L57`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L57)
- `model_l` — [`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L45)
- `predict_func` — [`L57`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L57)
- `select_m` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L48)
- `select_python_path` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L47)
- `submission_result` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L73)
- `y_test_pred` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L70)
- `y_train` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `y_valid` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L20)
- `y_valid_pred` — [`L59`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e16/train.py#L59)

