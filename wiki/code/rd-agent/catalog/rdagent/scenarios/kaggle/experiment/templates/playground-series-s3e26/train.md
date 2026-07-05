---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.playground-series-s3e26.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  logloss: logloss.
  cls: cls.
  imputer: imputer.
  submission_result: submission_result.
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
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  SEED: SEED.
  select_python_path: select_python_path.
  class_labels: class_labels.
  test_ids: test_ids.
  import_module_from_path: import_module_from_path().
  metrics_all: metrics_all.
  DIRNAME: DIRNAME.
  X_test_l: X_test_l.
  y_valid: y_valid.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  compute_metrics_for_classification: compute_metrics_for_classification().
  y_train: y_train.
  status_encoder: status_encoder.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L18) — Compute log loss for classification.
- `import_module_from_path(module_name, module_path)` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L25)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L11)
- `X_test` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `X_test_f` — [`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L45)
- `X_test_l` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L38)
- `X_test_selected` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L102)
- `X_train` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `X_train_f` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L43)
- `X_train_l` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L37)
- `X_train_selected` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L82)
- `X_valid` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `X_valid_f` — [`L44`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L44)
- `X_valid_l` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L37)
- `X_valid_selected` — [`L83`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L83)
- `class_labels` — [`L105`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L105)
- `cls` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L41)
- `f` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L40)
- `imputer` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L65)
- `logloss` — [`L93`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L93)
- `m` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L85)
- `metrics_all` — [`L89`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L89)
- `min_index` — [`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L98)
- `model` — [`L90`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L90)
- `model_l` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L78)
- `predict_func` — [`L90`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L90)
- `select_m` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L81)
- `select_python_path` — [`L80`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L80)
- `status_encoder` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `submission_result` — [`L107`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L107)
- `test_ids` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `y_test_pred` — [`L103`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L103)
- `y_train` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `y_valid` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L33)
- `y_valid_pred` — [`L92`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/playground-series-s3e26/train.py#L92)

