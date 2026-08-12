---
title: 'Module: OpenMLE-Gym/tests/test_common.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_common.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_common`/
symbols:
  CommonTests.test_json_safe_converts_scalar_and_exception: CommonTests#test_json_safe_converts_scalar_and_exception().
  CommonTests.test_atomic_json_replaces_complete_document: CommonTests#test_atomic_json_replaces_complete_document().
  CommonTests.test_task_name_validation_blocks_path_escape: CommonTests#test_task_name_validation_blocks_path_escape().
  CommonTests.test_resolve_task_path_stays_under_root: CommonTests#test_resolve_task_path_stays_under_root().
  CommonTests.test_slug_reader_does_not_sanitize_path_traversal: CommonTests#test_slug_reader_does_not_sanitize_path_traversal().
  _Scalar: _Scalar#
  _Scalar.item: _Scalar#item().
  CommonTests: CommonTests#
---
# Module: [`OpenMLE-Gym/tests/test_common.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py)

## Classes
### `CommonTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_common.py:22`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L22)
- signature: `class CommonTests(unittest.TestCase):`
- members:
  - `test_atomic_json_replaces_complete_document(self)` — [`L50`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L50)
  - `test_json_safe_converts_scalar_and_exception(self)` — [`L45`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L45)
  - `test_resolve_task_path_stays_under_root(self)` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L29)
  - `test_slug_reader_does_not_sanitize_path_traversal(self)` — [`L36`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L36)
  - `test_task_name_validation_blocks_path_escape(self)` — [`L23`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L23)
- uses (calls/refs, reference-scoped): [`atomic_write_json`](../openmle_gym/common.md#atomic_write_json), [`json_safe`](../openmle_gym/common.md#json_safe), [`validate_task_name`](../openmle_gym/common.md#validate_task_name), [`resolve_task_path`](../openmle_gym/common.md#resolve_task_path), [`read_slug_entries`](../openmle_gym/common.md#read_slug_entries)  (1 test-only)

### `_Scalar`
- def: [`OpenMLE-Gym/tests/test_common.py:17`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L17)
- signature: `class _Scalar:`
- members:
  - `item(self)` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_common.py#L18)
- used by: (2 test-only callers)

