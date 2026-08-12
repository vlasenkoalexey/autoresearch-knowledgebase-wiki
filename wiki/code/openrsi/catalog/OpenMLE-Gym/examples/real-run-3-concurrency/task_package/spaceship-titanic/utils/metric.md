---
title: 'Module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.examples.real-run-3-concurrency.task_package.spaceship-titanic.utils.metric`/SpaceshipTitanicMetrics#
symbols:
  SpaceshipTitanicMetrics.value: value.
  SpaceshipTitanicMetrics._parse_bool: _parse_bool().
  SpaceshipTitanicMetrics.evaluate: evaluate().
  SpaceshipTitanicMetrics.validate_submission: validate_submission().
  SpaceshipTitanicMetrics.convert: convert().
  SpaceshipTitanicMetrics: ''
  SpaceshipTitanicMetrics.__init__: __init__().
  SpaceshipTitanicMetrics.higher_is_better: higher_is_better.
---
# Module: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py)

## Classes
### `SpaceshipTitanicMetrics`
- def: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py:5`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L5)
- doc: Metric class for Spaceship Titanic competition using Classification Accuracy.
- signature: `class SpaceshipTitanicMetrics:`
- members:
  - `_parse_bool(self, series: pd.Series)` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L12) — Convert string or boolean values to consistent boolean.
  - `convert(val)` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L14)
  - `evaluate(self, y_true: pd.DataFrame = None, y_pred: pd.DataFrame = None)` — [`L23`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L23) — Calculate classification accuracy between predictions and true labels.
  - `validate_submission(self, submission: Any, ground_truth: Any)` — [`L47`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L47)
  - `higher_is_better` — [`L9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L9)
  - `value` — [`L10`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L10)
- protocol/private: `__init__`[`L8`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/spaceship-titanic/utils/metric.py#L8)

