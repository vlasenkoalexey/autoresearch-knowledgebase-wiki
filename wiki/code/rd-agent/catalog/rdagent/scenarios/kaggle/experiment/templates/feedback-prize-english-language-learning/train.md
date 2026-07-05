---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.feedback-prize-english-language-learning.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  metrics: metrics.
  cls: cls.
  y_test_pred: y_test_pred.
  submission_result: submission_result.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  y_valid_pred: y_valid_pred.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  min_index: min_index.
  X_valid_f: X_valid_f.
  X_test: X_test.
  X_train_selected: X_train_selected.
  X_test_selected: X_test_selected.
  X_train: X_train.
  X_valid: X_valid.
  select_python_path: select_python_path.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  y_valid: y_valid.
  MCRMSE: MCRMSE().
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py)

## Functions
- `MCRMSE(y_true, y_pred)` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L18)
- `import_module_from_path(module_name, module_path)` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L11)

## Module values
- `DIRNAME` — [`L8`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L8)
- `X_test` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L23)
- `X_test_f` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L35)
- `X_test_l` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L27)
- `X_test_selected` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L73)
- `X_train` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L23)
- `X_train_f` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L33)
- `X_train_l` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L26)
- `X_train_selected` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L53)
- `X_valid` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L23)
- `X_valid_f` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L34)
- `X_valid_l` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L26)
- `X_valid_selected` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L54)
- `cls` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L30)
- `f` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L29)
- `m` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L56)
- `metrics` — [`L64`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L64)
- `metrics_all` — [`L60`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L60)
- `min_index` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L69)
- `model` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L61)
- `model_l` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L49)
- `predict_func` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L61)
- `select_m` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L52)
- `select_python_path` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L51)
- `submission_result` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L77)
- `y_test_pred` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L74)
- `y_train` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L23)
- `y_valid` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L23)
- `y_valid_pred` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/train.py#L63)

