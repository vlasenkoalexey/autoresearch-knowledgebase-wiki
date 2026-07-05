---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.meta_tpl_deprecated.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  cls: cls.
  predict_func: predict_func.
  m_pred: m_pred.
  imputer: imputer.
  mcc: mcc.
  X_train: X_train.
  X_valid: X_valid.
  X_test: X_test.
  submission_result: submission_result.
  model_l: model_l.
  y_valid_pred: y_valid_pred.
  y_test_pred: y_test_pred.
  f: f.
  X_train_f: X_train_f.
  X_valid_f: X_valid_f.
  SEED: SEED.
  y_test_pred_l: y_test_pred_l.
  y_test_pred_labels: y_test_pred_labels.
  passenger_ids: passenger_ids.
  DIRNAME: DIRNAME.
  compute_metrics_for_classification: compute_metrics_for_classification().
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  y_valid_pred_l: y_valid_pred_l.
  y_valid: y_valid.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py)

## Functions
- `compute_metrics_for_classification(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L18) — Compute accuracy metric for classification.
- `import_module_from_path(module_name, module_path)` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L30)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L11)
- `X_test` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `X_test_f` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L50)
- `X_test_l` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L43)
- `X_train` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `X_train_f` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L48)
- `X_train_l` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L42)
- `X_valid` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `X_valid_f` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L49)
- `X_valid_l` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L42)
- `cls` — [`L46`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L46)
- `f` — [`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L45)
- `imputer` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L69)
- `m` — [`L83`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L83)
- `m_pred` — [`L105`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L105)
- `mcc` — [`L97`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L97)
- `model` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L88)
- `model_l` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L81)
- `passenger_ids` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `predict_func` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L88)
- `submission_result` — [`L113`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L113)
- `y_test_pred` — [`L108`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L108)
- `y_test_pred_l` — [`L104`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L104)
- `y_test_pred_labels` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L111)
- `y_train` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `y_valid` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L39)
- `y_valid_pred` — [`L94`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L94)
- `y_valid_pred_l` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/meta_tpl_deprecated/train.py#L87)

