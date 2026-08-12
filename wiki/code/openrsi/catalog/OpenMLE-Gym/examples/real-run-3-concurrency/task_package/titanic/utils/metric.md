---
title: 'Module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.examples.real-run-3-concurrency.task_package.titanic.utils.metric`/TitanicMetrics#
symbols:
  TitanicMetrics.value: value.
  TitanicMetrics.id_column: id_column.
  TitanicMetrics.evaluate: evaluate().
  TitanicMetrics.validate_submission: validate_submission().
  TitanicMetrics: ''
  TitanicMetrics.__init__: __init__().
  TitanicMetrics.higher_is_better: higher_is_better.
---
# Module: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py)

## Classes
### `TitanicMetrics`
- def: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py:6`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L6)
- doc: Metric class for Titanic - Machine Learning from Disaster competition using Accuracy.
- signature: `class TitanicMetrics:`
- members:
  - `evaluate(self, y_true: pd.DataFrame = None, y_pred: pd.DataFrame = None)` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L14) — Calculate accuracy between the predictions and the true labels.
  - `validate_submission(self, submission: Any, ground_truth: Any)` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L33)
  - `higher_is_better` — [`L10`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L10)
  - `id_column` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L12)
  - `value` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L11)
- protocol/private: `__init__`[`L9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/titanic/utils/metric.py#L9)

