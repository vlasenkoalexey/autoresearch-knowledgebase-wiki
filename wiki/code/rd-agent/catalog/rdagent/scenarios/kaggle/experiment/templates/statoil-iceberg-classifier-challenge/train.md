---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.statoil-iceberg-classifier-challenge.train`/
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
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L18) — Compute log loss for classification.
- `import_module_from_path(module_name, module_path)` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L23)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L11)
- `X_test` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `X_test_f` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L43)
- `X_test_l` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L36)
- `X_test_selected` — [`L100`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L100)
- `X_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `X_train_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L41)
- `X_train_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L35)
- `X_train_selected` — [`L80`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L80)
- `X_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `X_valid_f` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L42)
- `X_valid_l` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L35)
- `X_valid_selected` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L81)
- `cls` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L39)
- `f` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L38)
- `imputer` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L62)
- `m` — [`L83`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L83)
- `metrics` — [`L91`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L91)
- `metrics_all` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L87)
- `min_index` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L96)
- `model` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L88)
- `model_l` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L76)
- `predict_func` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L88)
- `select_m` — [`L79`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L79)
- `select_python_path` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L78)
- `submission_result` — [`L105`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L105)
- `test_ids` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `y_test_pred` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L101)
- `y_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `y_valid` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L31)
- `y_valid_pred` — [`L90`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/statoil-iceberg-classifier-challenge/train.py#L90)

