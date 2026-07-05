---
title: 'Module: rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.spaceship-titanic_template.train`/
symbols:
  y_test_pred: y_test_pred.
  X_test_f: X_test_f.
  m: m.
  y_valid_pred: y_valid_pred.
  metrics: metrics.
  weight: weight.
  j: j.
  cls: cls.
  test_pred_list: test_pred_list.
  imputer: imputer.
  predict_func: predict_func.
  select_m: select_m.
  X_train: X_train.
  X_valid: X_valid.
  X_test: X_test.
  f: f.
  submission_result: submission_result.
  X_train_f: X_train_f.
  model_l: model_l.
  X_valid_selected: X_valid_selected.
  max_index: max_index.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  X_test_selected: X_test_selected.
  valid_pred_list: valid_pred_list.
  SEED: SEED.
  select_python_path: select_python_path.
  metrics_all: metrics_all.
  passenger_ids: passenger_ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  model: model.
  DIRNAME: DIRNAME.
  weight_list: weight_list.
  searched_set: searched_set.
  y_valid: y_valid.
  compute_metrics_for_classification: compute_metrics_for_classification().
  y_train: y_train.
  i: i.
---
# Module: [`rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L18) — Compute accuracy metric for classification.
- `import_module_from_path(module_name, module_path)` — [`L24`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L24)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L11)
- `X_test` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `X_test_f` — [`L43`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L43)
- `X_test_l` — [`L36`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L36)
- `X_test_selected` — [`L129`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L129)
- `X_train` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `X_train_f` — [`L41`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L41)
- `X_train_l` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L35)
- `X_train_selected` — [`L80`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L80)
- `X_valid` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `X_valid_f` — [`L42`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L42)
- `X_valid_l` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L35)
- `X_valid_selected` — [`L81`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L81)
- `cls` — [`L39`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L39)
- `f` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L38)
- `i` — [`L106`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L106)
- `imputer` — [`L63`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L63)
- `j` — [`L113`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L113)
- `m` — [`L83`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L83)
- `max_index` — [`L122`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L122)
- `metrics` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L116)
- `metrics_all` — [`L103`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L103)
- `model` — [`L98`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L98)
- `model_l` — [`L76`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L76)
- `passenger_ids` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `predict_func` — [`L98`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L98)
- `searched_set` — [`L105`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L105)
- `select_m` — [`L79`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L79)
- `select_python_path` — [`L78`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L78)
- `submission_result` — [`L138`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L138)
- `test_pred_list` — [`L127`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L127)
- `valid_pred_list` — [`L97`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L97)
- `weight` — [`L107`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L107)
- `weight_list` — [`L104`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L104)
- `y_test_pred` — [`L130`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L130)
- `y_train` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `y_valid` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L32)
- `y_valid_pred` — [`L100`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/spaceship-titanic_template/train.py#L100)

