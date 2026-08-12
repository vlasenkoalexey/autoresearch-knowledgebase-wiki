---
title: 'Module: OpenMLE-Gym/tests/test_metric_validation.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_metric_validation.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_metric_validation`/MetricValidationTests#
symbols:
  MetricValidationTests.test_imported_metrics_class_is_not_selected: test_imported_metrics_class_is_not_selected().
  MetricValidationTests.test_numpy_scalar_score_is_json_safe: test_numpy_scalar_score_is_json_safe().
  MetricValidationTests.test_non_finite_metric_score_is_rejected: test_non_finite_metric_score_is_rejected().
  MetricValidationTests: ''
---
# Module: [`OpenMLE-Gym/tests/test_metric_validation.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_metric_validation.py)

## Classes
### `MetricValidationTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_metric_validation.py:11`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_metric_validation.py#L11)
- signature: `class MetricValidationTests(unittest.TestCase):`
- members:
  - `test_imported_metrics_class_is_not_selected(self)` — [`L12`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_metric_validation.py#L12)
  - `test_non_finite_metric_score_is_rejected(self)` — [`L57`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_metric_validation.py#L57)
  - `test_numpy_scalar_score_is_json_safe(self)` — [`L35`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_metric_validation.py#L35)
- uses (calls/refs, reference-scoped): [`evaluate_sample_submission`](../openmle_gym/metric_validation.md#evaluate_sample_submission), [`load_metric_class`](../openmle_gym/metric_validation.md#load_metric_class)

