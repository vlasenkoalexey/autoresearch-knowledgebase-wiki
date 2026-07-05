---
title: 'Module: examples/symbolic_regression/eval.py'
type: catalog
provenance: extracted
module: examples/symbolic_regression/eval.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.symbolic_regression.eval`/
symbols:
  value: value.
  d_type: d_type.
  score: score.
  metrics_output: metrics_output.
  d: d.
  data_dir_path: data_dir_path.
  scores_for_mean: scores_for_mean.
  data_file_check: data_file_check.
  path_obj: path_obj.
  m_key: m_key.
  problem_name: problem_name.
  f: f.
  result: result.
  results_data: results_data.
  all_scores: all_scores.
  metrics_summary: metrics_summary.
  overall_performance: overall_performance.
  evaluation: evaluation().
  output_results_file: output_results_file.
  program_file_path: program_file_path.
  all_results: all_results.
  stat_name: stat_name.
  evaluation._get_metrics_for_set: evaluation()._get_metrics_for_set().
  subdir_path: subdir_path.
  root_path_arg: root_path_arg.
  evaluation._create_error_return: evaluation()._create_error_return().
  problem_dirs: problem_dirs.
  program_file_check: program_file_check.
  e: e.
  NumpyFloatJSONEncoder.default: NumpyFloatJSONEncoder#default().
  NumpyFloatJSONEncoder: NumpyFloatJSONEncoder#
  compute_output_base_metrics: compute_output_base_metrics().
  objective_function: objective_function().
  metric_keys: metric_keys.
  dataset_types: dataset_types.
  problem: problem.
---
# Module: [`examples/symbolic_regression/eval.py`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py)

## Classes
### `NumpyFloatJSONEncoder`  ·  implements/extends JSONEncoder
- def: [`examples/symbolic_regression/eval.py:20`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L20)
- signature: `class NumpyFloatJSONEncoder(json.JSONEncoder):`
- members:
  - `default(self, obj)` — [`L21`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L21)
- used by: (1 test-only callers)

## Functions
- `_create_error_return(error_message: str)` — [`L164`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L164)
- `_get_metrics_for_set(X_data: np.ndarray, y_data: np.ndarray, set_name: str)` — [`L260`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L260)
- `compute_output_base_metrics(y_pred: np.ndarray, y: np.ndarray)` — [`L31`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L31) — Computes base metrics after filtering NaNs from predictions.
- `evaluation(program_path: str, data_path: str)` — [`L147`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L147) — Evaluates a model by loading it, optimizing its parameters, and testing it.
- `objective_function(params: np.ndarray, model_func: callable, X_matrix: np.ndarray, y_true_vector: np.ndarray)` — [`L123`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L123) — Objective function for scipy.optimize.minimize.

## Module values
- `all_results` — [`L337`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L337)
- `all_scores` — [`L382`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L382)
- `d` — [`L317`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L317)
- `d_type` — [`L379`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L379)
- `data_dir_path` — [`L343`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L343)
- `data_file_check` — [`L303`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L303)
- `dataset_types` — [`L377`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L377)
- `e` — [`L455`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L455)
- `f` — [`L452`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L452)
- `m_key` — [`L381`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L381)
- `metric_keys` — [`L376`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L376)
- `metrics_output` — [`L359`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L359)
- `metrics_summary` — [`L425`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L425)
- `output_results_file` — [`L447`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L447)
- `overall_performance` — [`L374`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L374)
- `path_obj` — [`L297`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L297)
- `problem` — [`L367`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L367)
- `problem_dirs` — [`L298`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L298)
- `problem_name` — [`L339`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L339)
- `program_file_check` — [`L302`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L302)
- `program_file_path` — [`L342`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L342)
- `result` — [`L367`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L367)
- `results_data` — [`L383`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L383)
- `root_path_arg` — [`L296`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L296)
- `score` — [`L386`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L386)
- `scores_for_mean` — [`L410`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L410)
- `stat_name` — [`L430`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L430)
- `subdir_path` — [`L338`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L338)
- `value` — [`L430`](../../../../../../raw/code/openevolve/examples/symbolic_regression/eval.py#L430)

