---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.forest-cover-type-prediction.train_past`/
symbols:
  X_test_f: X_test_f.
  accuracy: accuracy.
  X_val: X_val.
  m: m.
  X_te: X_te.
  imputer: imputer.
  X_tr: X_tr.
  cls: cls.
  predict_func: predict_func.
  f: f.
  submission_result: submission_result.
  y_val: y_val.
  select_m: select_m.
  y_valid_pred: y_valid_pred.
  X_valid_selected: X_valid_selected.
  model_l: model_l.
  final_model: final_model.
  valid_index: valid_index.
  data_df: data_df.
  X_train_f: X_train_f.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  X_test_selected: X_test_selected.
  y_test_pred: y_test_pred.
  X_train: X_train.
  SEED: SEED.
  y_train: y_train.
  select_python_path: select_python_path.
  ids: ids.
  X_test: X_test.
  import_module_from_path: import_module_from_path().
  scaler: scaler.
  model_count: model_count.
  best_accuracy: best_accuracy.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  X_test_l: X_test_l.
  DIRNAME: DIRNAME.
  submission_df: submission_df.
  fold_number: fold_number.
  best: best.
  train_index: train_index.
  model: model.
  y_tr: y_tr.
  accuracies: accuracies.
  y_test_pred_l: y_test_pred_l.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py)

## Functions
- `import_module_from_path(module_name, module_path)` — [`L19`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L19)

## Module values
- `DIRNAME` — [`L16`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L16)
- `SEED` — [`L13`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L13)
- `X_te` — [`L55`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L55)
- `X_test` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L36)
- `X_test_f` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L63)
- `X_test_l` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L52)
- `X_test_selected` — [`L127`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L127)
- `X_tr` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L53)
- `X_train` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L31)
- `X_train_f` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L61)
- `X_train_l` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L52)
- `X_train_selected` — [`L100`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L100)
- `X_val` — [`L53`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L53)
- `X_valid_f` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L62)
- `X_valid_l` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L52)
- `X_valid_selected` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L101)
- `accuracies` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L40)
- `accuracy` — [`L112`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L112)
- `best` — [`L108`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L108)
- `best_accuracy` — [`L107`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L107)
- `cls` — [`L59`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L59)
- `data_df` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L28)
- `f` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L58)
- `final_model` — [`L123`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L123)
- `fold_number` — [`L46`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L46)
- `ids` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L35)
- `imputer` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L81)
- `m` — [`L103`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L103)
- `model` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L109)
- `model_count` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L47)
- `model_l` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L96)
- `predict_func` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L109)
- `scaler` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L42)
- `select_m` — [`L99`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L99)
- `select_python_path` — [`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L98)
- `submission_df` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L34)
- `submission_result` — [`L130`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L130)
- `train_index` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L49)
- `valid_index` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L49)
- `y_test_pred` — [`L128`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L128)
- `y_test_pred_l` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L41)
- `y_tr` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L54)
- `y_train` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L32)
- `y_val` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L54)
- `y_valid_pred` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/forest-cover-type-prediction/train_past.py#L111)

