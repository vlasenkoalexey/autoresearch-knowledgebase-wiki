---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.tabular-playground-series-may-2022.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  auroc: auroc.
  cls: cls.
  f: f.
  model_name: model_name.
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
  SEED: SEED.
  select_python_path: select_python_path.
  X_train: X_train.
  X_valid: X_valid.
  ids: ids.
  predict_func: predict_func.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  sub_submission: sub_submission.
  metrics_all: metrics_all.
  X_test: X_test.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  model: model.
  y_train: y_train.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py)

## Functions
- `import_module_from_path(module_name, module_path)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L17)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L11)
- `X_test` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `X_test_f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L36)
- `X_test_l` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L29)
- `X_test_selected` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L77)
- `X_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `X_train_f` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L34)
- `X_train_l` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L28)
- `X_train_selected` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L53)
- `X_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `X_valid_f` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L35)
- `X_valid_l` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L28)
- `X_valid_selected` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L54)
- `auroc` — [`L66`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L66)
- `cls` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L32)
- `f` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L31)
- `ids` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `m` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L56)
- `max_index` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L73)
- `metrics_all` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L62)
- `model` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L63)
- `model_l` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L49)
- `model_name` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L63)
- `predict_func` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L63)
- `select_m` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L52)
- `select_python_path` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L51)
- `sub_submission` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L61)
- `submission_result` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L82)
- `y_test_pred` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L78)
- `y_train` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `y_valid` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L25)
- `y_valid_pred` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/tabular-playground-series-may-2022/train.py#L65)

