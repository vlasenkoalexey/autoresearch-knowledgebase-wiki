---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.tabular-playground-series-dec-2021.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  accuracy: accuracy.
  cls: cls.
  f: f.
  y_test_pred: y_test_pred.
  predict_func: predict_func.
  model_l: model_l.
  select_m: select_m.
  submission_result: submission_result.
  max_index: max_index.
  y_valid_pred: y_valid_pred.
  X_test_selected: X_test_selected.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  X_train: X_train.
  X_valid: X_valid.
  SEED: SEED.
  select_python_path: select_python_path.
  X_test: X_test.
  label_encoder: label_encoder.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  model: model.
  y_train: y_train.
  ids: ids.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py)

## Functions
- `import_module_from_path(module_name, module_path)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L17)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L11)
- `X_test` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `X_test_f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L36)
- `X_test_l` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L29)
- `X_test_selected` — [`L79`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L79)
- `X_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `X_train_f` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L34)
- `X_train_l` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L28)
- `X_train_selected` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L58)
- `X_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `X_valid_f` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L35)
- `X_valid_l` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L28)
- `X_valid_selected` — [`L59`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L59)
- `accuracy` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L70)
- `cls` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L32)
- `f` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L31)
- `ids` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `label_encoder` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `m` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L61)
- `max_index` — [`L75`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L75)
- `metrics_all` — [`L66`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L66)
- `model` — [`L67`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L67)
- `model_l` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L54)
- `predict_func` — [`L67`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L67)
- `select_m` — [`L57`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L57)
- `select_python_path` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L56)
- `submission_result` — [`L84`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L84)
- `y_test_pred` — [`L80`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L80)
- `y_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `y_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L25)
- `y_valid_pred` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-dec-2021/train.py#L69)

