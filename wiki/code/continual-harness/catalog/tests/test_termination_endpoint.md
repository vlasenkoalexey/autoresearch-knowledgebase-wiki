---
title: 'Module: tests/test_termination_endpoint.py'
type: catalog
provenance: extracted
module: tests/test_termination_endpoint.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_termination_endpoint`/
symbols:
  success: success.
  run_standalone_test: run_standalone_test().
  TestTerminationEndpoint: TestTerminationEndpoint#
  TestTerminationEndpoint.server: TestTerminationEndpoint#server().
  TestTerminationEndpoint.test_endpoint_exists: TestTerminationEndpoint#test_endpoint_exists().
  TestTerminationEndpoint.test_gym_badge_count_default: TestTerminationEndpoint#test_gym_badge_count_default().
  TestTerminationEndpoint.test_gym_badge_count_custom_threshold: TestTerminationEndpoint#test_gym_badge_count_custom_threshold().
  TestTerminationEndpoint.test_gym_badge_count_high_threshold: TestTerminationEndpoint#test_gym_badge_count_high_threshold().
  TestTerminationEndpoint.test_unknown_condition_type: TestTerminationEndpoint#test_unknown_condition_type().
  TestTerminationEndpoint.test_badge_names_included: TestTerminationEndpoint#test_badge_names_included().
---
# Module: [`tests/test_termination_endpoint.py`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py)

## Classes
### `TestTerminationEndpoint`
- def: [`tests/test_termination_endpoint.py:23`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L23)
- doc: Test class for /termination_condition endpoint
- signature: `class TestTerminationEndpoint:`
- members:
  - `server(self)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L27) — Start server and yield, then cleanup
  - `test_badge_names_included(self, server)` — [`L165`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L165) — Test that badge_names is included for gym_badge_count
  - `test_endpoint_exists(self, server)` — [`L88`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L88) — Test that /termination_condition endpoint exists
  - `test_gym_badge_count_custom_threshold(self, server)` — [`L123`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L123) — Test gym_badge_count with custom threshold
  - `test_gym_badge_count_default(self, server)` — [`L94`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L94) — Test default gym_badge_count condition (threshold=1)
  - `test_gym_badge_count_high_threshold(self, server)` — [`L137`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L137) — Test gym_badge_count with threshold higher than current badges
  - `test_unknown_condition_type(self, server)` — [`L153`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L153) — Test that unknown condition types return error

## Functions
- `run_standalone_test()` — [`L175`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L175) — Run a standalone test without pytest (for quick manual testing)

## Module values
- `success` — [`L230`](../../../../../raw/code/continual-harness/tests/test_termination_endpoint.py#L230)

