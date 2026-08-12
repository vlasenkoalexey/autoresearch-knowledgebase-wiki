---
title: 'Module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.examples.real-run-3-concurrency.task_package.house-prices-advanced-regression-techniques.utils.metric`/AmesHousingMetrics#
symbols:
  AmesHousingMetrics.value: value.
  AmesHousingMetrics.evaluate: evaluate().
  AmesHousingMetrics.validate_submission: validate_submission().
  AmesHousingMetrics: ''
  AmesHousingMetrics.__init__: __init__().
  AmesHousingMetrics.higher_is_better: higher_is_better.
---
# Module: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py)

## Classes
### `AmesHousingMetrics`
- def: [`OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py:6`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L6)
- doc: Metric class for Ames Housing Price Prediction using RMSLE.
- signature: `class AmesHousingMetrics:`
- members:
  - `evaluate(self, y_true: pd.DataFrame = None, y_pred: pd.DataFrame = None)` — [`L13`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L13) — Calculate RMSE between log of predicted and log of actual SalePrice.
  - `validate_submission(self, submission: Any, ground_truth: Any)` — [`L32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L32)
  - `higher_is_better` — [`L10`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L10)
  - `value` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L11)
- protocol/private: `__init__`[`L9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Gym/examples/real-run-3-concurrency/task_package/house-prices-advanced-regression-techniques/utils/metric.py#L9)

