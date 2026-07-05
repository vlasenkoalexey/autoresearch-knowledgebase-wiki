---
title: 'Module: tests/test_visualization_sanitization.py'
type: catalog
provenance: extracted
module: tests/test_visualization_sanitization.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_visualization_sanitization`/Test
symbols:
  TestCheckJsonFloat.scripts_path: CheckJsonFloat#scripts_path.
  TestSanitizeProgramForVisualization.scripts_path: SanitizeProgramForVisualization#scripts_path.
  TestCheckJsonFloat.tearDownClass: CheckJsonFloat#tearDownClass().
  TestSanitizeProgramForVisualization.tearDownClass: SanitizeProgramForVisualization#tearDownClass().
  TestCheckJsonFloat: CheckJsonFloat#
  TestCheckJsonFloat.setUpClass: CheckJsonFloat#setUpClass().
  TestCheckJsonFloat.test_valid_positive_float: CheckJsonFloat#test_valid_positive_float().
  TestCheckJsonFloat.test_valid_negative_float: CheckJsonFloat#test_valid_negative_float().
  TestCheckJsonFloat.test_valid_zero: CheckJsonFloat#test_valid_zero().
  TestCheckJsonFloat.test_valid_integer: CheckJsonFloat#test_valid_integer().
  TestCheckJsonFloat.test_invalid_positive_infinity: CheckJsonFloat#test_invalid_positive_infinity().
  TestCheckJsonFloat.test_invalid_negative_infinity: CheckJsonFloat#test_invalid_negative_infinity().
  TestCheckJsonFloat.test_invalid_nan: CheckJsonFloat#test_invalid_nan().
  TestCheckJsonFloat.test_invalid_none: CheckJsonFloat#test_invalid_none().
  TestSanitizeProgramForVisualization: SanitizeProgramForVisualization#
  TestSanitizeProgramForVisualization.setUpClass: SanitizeProgramForVisualization#setUpClass().
  TestSanitizeProgramForVisualization.test_sanitize_negative_infinity_in_metrics: SanitizeProgramForVisualization#test_sanitize_negative_infinity_in_metrics().
  TestSanitizeProgramForVisualization.test_sanitize_positive_infinity_in_metrics: SanitizeProgramForVisualization#test_sanitize_positive_infinity_in_metrics().
  TestSanitizeProgramForVisualization.test_sanitize_nan_in_metrics: SanitizeProgramForVisualization#test_sanitize_nan_in_metrics().
  TestSanitizeProgramForVisualization.test_valid_metrics_unchanged: SanitizeProgramForVisualization#test_valid_metrics_unchanged().
  TestSanitizeProgramForVisualization.test_sanitize_parent_metrics: SanitizeProgramForVisualization#test_sanitize_parent_metrics().
  TestSanitizeProgramForVisualization.test_mixed_valid_and_invalid_values: SanitizeProgramForVisualization#test_mixed_valid_and_invalid_values().
  TestJsonSerialization: JsonSerialization#
  TestJsonSerialization.test_sanitized_data_is_json_serializable: JsonSerialization#test_sanitized_data_is_json_serializable().
  TestJsonSerialization.test_unsanitized_infinity_fails_strict_json: JsonSerialization#test_unsanitized_infinity_fails_strict_json().
  TestJsonSerialization.test_unsanitized_nan_fails_strict_json: JsonSerialization#test_unsanitized_nan_fails_strict_json().
  TestJsonSerialization.test_sanitized_none_works_with_strict_json: JsonSerialization#test_sanitized_none_works_with_strict_json().
---
# Module: [`tests/test_visualization_sanitization.py`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py)

## Classes
### `TestCheckJsonFloat`  ·  implements/extends TestCase
- def: [`tests/test_visualization_sanitization.py:13`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L13)
- doc: Tests for the check_json_float helper function
- signature: `class TestCheckJsonFloat(unittest.TestCase):`
- members:
  - `setUpClass(cls)` — [`L17`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L17) — Add scripts directory to path for importing visualizer
  - `tearDownClass(cls)` — [`L25`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L25) — Remove scripts directory from path
  - `test_invalid_nan(self)` — [`L84`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L84) — Test that NaN is invalid
  - `test_invalid_negative_infinity(self)` — [`L76`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L76) — Test that negative infinity is invalid
  - `test_invalid_none(self)` — [`L92`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L92) — Test that None is invalid (not a number)
  - `test_invalid_positive_infinity(self)` — [`L68`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L68) — Test that positive infinity is invalid
  - `test_valid_integer(self)` — [`L58`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L58) — Test that integers are valid
  - `test_valid_negative_float(self)` — [`L40`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L40) — Test that negative floats are valid
  - `test_valid_positive_float(self)` — [`L30`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L30) — Test that positive floats are valid
  - `test_valid_zero(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L49) — Test that zero is valid
  - `scripts_path` — [`L19`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L19)

### `TestJsonSerialization`  ·  implements/extends TestCase
- def: [`tests/test_visualization_sanitization.py:219`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L219)
- doc: Tests for JSON serialization of sanitized data
- signature: `class TestJsonSerialization(unittest.TestCase):`
- members:
  - `test_sanitized_data_is_json_serializable(self)` — [`L222`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L222) — Test that sanitized data can be JSON serialized
  - `test_sanitized_none_works_with_strict_json(self)` — [`L248`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L248) — Test that sanitized None values work with strict JSON
  - `test_unsanitized_infinity_fails_strict_json(self)` — [`L234`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L234) — Test that unsanitized infinity fails strict JSON serialization
  - `test_unsanitized_nan_fails_strict_json(self)` — [`L241`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L241) — Test that unsanitized NaN fails strict JSON serialization

### `TestSanitizeProgramForVisualization`  ·  implements/extends TestCase
- def: [`tests/test_visualization_sanitization.py:101`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L101)
- doc: Tests for the sanitize_program_for_visualization function
- signature: `class TestSanitizeProgramForVisualization(unittest.TestCase):`
- members:
  - `setUpClass(cls)` — [`L105`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L105) — Add scripts directory to path for importing visualizer
  - `tearDownClass(cls)` — [`L113`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L113) — Remove scripts directory from path
  - `test_mixed_valid_and_invalid_values(self)` — [`L195`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L195) — Test sanitization with mix of valid and invalid values
  - `test_sanitize_nan_in_metrics(self)` — [`L146`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L146) — Test that NaN in metrics is sanitized to None
  - `test_sanitize_negative_infinity_in_metrics(self)` — [`L118`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L118) — Test that -inf in metrics is sanitized to None
  - `test_sanitize_parent_metrics(self)` — [`L175`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L175) — Test that parent_metrics are also sanitized
  - `test_sanitize_positive_infinity_in_metrics(self)` — [`L132`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L132) — Test that +inf in metrics is sanitized to None
  - `test_valid_metrics_unchanged(self)` — [`L160`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L160) — Test that valid metrics are not changed
  - `scripts_path` — [`L107`](../../../../../raw/code/openevolve/tests/test_visualization_sanitization.py#L107)

