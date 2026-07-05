---
title: 'Module: rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.example.eval.playground-series-s4e9.grade`/
symbols:
  thresholds: thresholds.
  score: score.
  InvalidSubmissionError: InvalidSubmissionError#
  prepare_for_metric: prepare_for_metric().
  grade: grade().
  submission: submission.
  answers: answers.
  submission_path: submission_path.
  gt_submission_path: gt_submission_path.
---
# Module: [`rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py)

## Classes
### `InvalidSubmissionError`  ·  implements/extends Exception
- def: [`rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py:9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L9)
- doc: A custom exception for when the agent submission cannot be graded.
- signature: `class InvalidSubmissionError(Exception):`
- used by: (1 test-only callers)

## Functions
- `grade(submission: pd.DataFrame, answers: pd.DataFrame)` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L42)
- `prepare_for_metric(submission: pd.DataFrame, answers: pd.DataFrame)` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L17)

## Module values
- `answers` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L51)
- `gt_submission_path` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L49)
- `score` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L52)
- `submission` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L50)
- `submission_path` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L48)
- `thresholds` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/example/eval/playground-series-s4e9/grade.py#L56)

