---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.sf-crime.train`/
symbols:
  X_test_f: X_test_f.
  y_test_pred: y_test_pred.
  m: m.
  y_valid_pred: y_valid_pred.
  metrics: metrics.
  weight: weight.
  test_ids: test_ids.
  X_train: X_train.
  X_valid: X_valid.
  j: j.
  cls: cls.
  test_pred_list: test_pred_list.
  X_test: X_test.
  imputer: imputer.
  predict_func: predict_func.
  select_m: select_m.
  submission_result: submission_result.
  f: f.
  X_train_f: X_train_f.
  model_l: model_l.
  X_valid_selected: X_valid_selected.
  min_index: min_index.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  X_test_selected: X_test_selected.
  valid_pred_list: valid_pred_list.
  y_valid: y_valid.
  SEED: SEED.
  select_python_path: select_python_path.
  metrics_all: metrics_all.
  y_train: y_train.
  class_labels: class_labels.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  model: model.
  DIRNAME: DIRNAME.
  weight_list: weight_list.
  searched_set: searched_set.
  compute_metrics_for_classification: compute_metrics_for_classification().
  category_encoder: category_encoder.
  i: i.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L18) — Compute log loss for classification.
- `import_module_from_path(module_name, module_path)` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L25)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L11)
- `X_test` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `X_test_f` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L50)
- `X_test_l` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L43)
- `X_test_selected` — [`L134`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L134)
- `X_train` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `X_train_f` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L48)
- `X_train_l` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L42)
- `X_train_selected` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L86)
- `X_valid` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `X_valid_f` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L49)
- `X_valid_l` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L42)
- `X_valid_selected` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L87)
- `category_encoder` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `class_labels` — [`L144`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L144)
- `cls` — [`L46`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L46)
- `f` — [`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L45)
- `i` — [`L110`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L110)
- `imputer` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L70)
- `j` — [`L117`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L117)
- `m` — [`L89`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L89)
- `metrics` — [`L121`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L121)
- `metrics_all` — [`L107`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L107)
- `min_index` — [`L127`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L127)
- `model` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L102)
- `model_l` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L82)
- `predict_func` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L102)
- `searched_set` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L109)
- `select_m` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L85)
- `select_python_path` — [`L84`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L84)
- `submission_result` — [`L146`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L146)
- `test_ids` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `test_pred_list` — [`L132`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L132)
- `valid_pred_list` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L101)
- `weight` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L111)
- `weight_list` — [`L108`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L108)
- `y_test_pred` — [`L135`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L135)
- `y_train` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `y_valid` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L33)
- `y_valid_pred` — [`L104`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/sf-crime/train.py#L104)

