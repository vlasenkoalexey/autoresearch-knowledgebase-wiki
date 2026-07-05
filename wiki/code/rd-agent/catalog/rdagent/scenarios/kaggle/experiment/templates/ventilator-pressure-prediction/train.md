---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.ventilator-pressure-prediction.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  mae: mae.
  cls: cls.
  f: f.
  predict_func: predict_func.
  model_l: model_l.
  select_m: select_m.
  submission_result: submission_result.
  max_index: max_index.
  y_valid_pred: y_valid_pred.
  X_test_selected: X_test_selected.
  y_test_pred: y_test_pred.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  y_valid_filtered: y_valid_filtered.
  y_valid_pred_filtered: y_valid_pred_filtered.
  X_valid: X_valid.
  SEED: SEED.
  mask: mask.
  select_python_path: select_python_path.
  X_train: X_train.
  ids: ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_test: X_test.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  model: model.
  y_train: y_train.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py)

## Functions
- `import_module_from_path(module_name, module_path)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L17)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L11)
- `X_test` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `X_test_f` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L37)
- `X_test_l` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L30)
- `X_test_selected` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L77)
- `X_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `X_train_f` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L35)
- `X_train_l` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L29)
- `X_train_selected` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L54)
- `X_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `X_valid_f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L36)
- `X_valid_l` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L29)
- `X_valid_selected` — [`L55`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L55)
- `cls` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L33)
- `f` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L32)
- `ids` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `m` — [`L57`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L57)
- `mae` — [`L68`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L68)
- `mask` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L26)
- `max_index` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L73)
- `metrics_all` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L62)
- `model` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L63)
- `model_l` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L50)
- `predict_func` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L63)
- `select_m` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L53)
- `select_python_path` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L52)
- `submission_result` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L82)
- `y_test_pred` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L78)
- `y_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `y_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L25)
- `y_valid_filtered` — [`L66`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L66)
- `y_valid_pred` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L65)
- `y_valid_pred_filtered` — [`L67`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/ventilator-pressure-prediction/train.py#L67)

