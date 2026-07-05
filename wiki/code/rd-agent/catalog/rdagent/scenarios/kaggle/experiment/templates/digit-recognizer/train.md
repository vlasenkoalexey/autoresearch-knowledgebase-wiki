---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.digit-recognizer.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  cls: cls.
  accuracy: accuracy.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  X_test: X_test.
  X_valid_selected: X_valid_selected.
  max_index: max_index.
  y_valid_pred: y_valid_pred.
  y_test_pred: y_test_pred.
  submission_result: submission_result.
  X_train_f: X_train_f.
  X_valid_f: X_valid_f.
  X_train: X_train.
  X_valid: X_valid.
  X_train_selected: X_train_selected.
  ids: ids.
  SEED: SEED.
  select_python_path: select_python_path.
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
# Module: [`rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L17) — Compute accuracy for classification.
- `import_module_from_path(module_name, module_path)` — [`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L22)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L11)
- `X_test` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L30)
- `X_test_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L41)
- `X_test_l` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L34)
- `X_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L30)
- `X_train_f` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L39)
- `X_train_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L33)
- `X_train_selected` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L62)
- `X_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L30)
- `X_valid_f` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L40)
- `X_valid_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L33)
- `X_valid_selected` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L63)
- `accuracy` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L73)
- `cls` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L37)
- `f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L36)
- `ids` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L82)
- `m` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L65)
- `max_index` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L78)
- `metrics_all` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L69)
- `model` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L70)
- `model_l` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L58)
- `predict_func` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L70)
- `select_m` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L61)
- `select_python_path` — [`L60`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L60)
- `submission_result` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L87)
- `y_test_pred` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L86)
- `y_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L30)
- `y_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L30)
- `y_valid_pred` — [`L72`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/digit-recognizer/train.py#L72)

