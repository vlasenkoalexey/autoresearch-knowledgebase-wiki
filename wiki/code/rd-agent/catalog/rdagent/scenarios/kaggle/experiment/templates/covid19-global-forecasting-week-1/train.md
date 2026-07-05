---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.covid19-global-forecasting-week-1.train`/
symbols:
  X_test_f: X_test_f.
  m: m.
  cls: cls.
  imputer: imputer.
  rmsle_avg: rmsle_avg.
  X_train: X_train.
  X_valid: X_valid.
  rmsle_fatalities: rmsle_fatalities.
  X_test: X_test.
  predict_func: predict_func.
  f: f.
  model_l: model_l.
  select_m: select_m.
  y_valid_pred: y_valid_pred.
  y_test_pred: y_test_pred.
  min_index: min_index.
  rmsle_cases: rmsle_cases.
  X_test_selected: X_test_selected.
  submission_result: submission_result.
  X_train_f: X_train_f.
  X_valid_selected: X_valid_selected.
  X_valid_f: X_valid_f.
  X_train_selected: X_train_selected.
  y_valid_cases: y_valid_cases.
  y_pred_cases: y_pred_cases.
  SEED: SEED.
  select_python_path: select_python_path.
  epsilon: epsilon.
  forecast_ids: forecast_ids.
  import_module_from_path: import_module_from_path().
  X_test_l: X_test_l.
  metrics_all: metrics_all.
  y_valid: y_valid.
  X_train_l: X_train_l.
  X_valid_l: X_valid_l.
  DIRNAME: DIRNAME.
  compute_rmsle: compute_rmsle().
  y_train: y_train.
  model: model.
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py)

## Functions
- `compute_rmsle(y_true, y_pred)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L17) — Compute Root Mean Squared Logarithmic Error for regression.
- `import_module_from_path(module_name, module_path)` — [`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L22)

## Module values
- `DIRNAME` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L14)
- `SEED` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L11)
- `X_test` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `X_test_f` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L41)
- `X_test_l` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L34)
- `X_test_selected` — [`L108`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L108)
- `X_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `X_train_f` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L39)
- `X_train_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L33)
- `X_train_selected` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L77)
- `X_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `X_valid_f` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L40)
- `X_valid_l` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L33)
- `X_valid_selected` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L78)
- `cls` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L37)
- `epsilon` — [`L91`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L91)
- `f` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L36)
- `forecast_ids` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `imputer` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L61)
- `m` — [`L80`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L80)
- `metrics_all` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L85)
- `min_index` — [`L104`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L104)
- `model` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L86)
- `model_l` — [`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L73)
- `predict_func` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L86)
- `rmsle_avg` — [`L99`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L99)
- `rmsle_cases` — [`L95`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L95)
- `rmsle_fatalities` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L96)
- `select_m` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L76)
- `select_python_path` — [`L75`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L75)
- `submission_result` — [`L112`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L112)
- `y_pred_cases` — [`L93`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L93)
- `y_test_pred` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L109)
- `y_train` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `y_valid` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L30)
- `y_valid_cases` — [`L92`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L92)
- `y_valid_pred` — [`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/covid19-global-forecasting-week-1/train.py#L88)

