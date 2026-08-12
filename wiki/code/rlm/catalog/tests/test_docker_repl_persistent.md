---
title: 'Module: tests/test_docker_repl_persistent.py'
type: catalog
provenance: extracted
module: tests/test_docker_repl_persistent.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_docker_repl_persistent`/
symbols:
  repl: repl().
  repl_compaction: repl_compaction().
  pytestmark: pytestmark.
  TestDockerProtocol.test_satisfies_persistence_protocol: TestDockerProtocol#test_satisfies_persistence_protocol().
  _docker_available: _docker_available().
  TestDockerProtocol: TestDockerProtocol#
  TestDockerMultiContext: TestDockerMultiContext#
  TestDockerMultiContext.test_add_context_versioning_and_access: TestDockerMultiContext#test_add_context_versioning_and_access().
  TestDockerMultiContext.test_add_context_auto_increment: TestDockerMultiContext#test_add_context_auto_increment().
  TestDockerMultiContext.test_context_alias_points_to_first: TestDockerMultiContext#test_context_alias_points_to_first().
  TestDockerMultiContext.test_dict_context: TestDockerMultiContext#test_dict_context().
  TestDockerMultiHistory: TestDockerMultiHistory#
  TestDockerMultiHistory.test_add_history_versioning: TestDockerMultiHistory#test_add_history_versioning().
  TestDockerMultiHistory.test_history_alias_points_to_first: TestDockerMultiHistory#test_history_alias_points_to_first().
  TestDockerMultiHistory.test_add_history_deep_copy: TestDockerMultiHistory#test_add_history_deep_copy().
  TestDockerUpdateHandlerAddress: TestDockerUpdateHandlerAddress#
  TestDockerUpdateHandlerAddress.test_update_handler_address: TestDockerUpdateHandlerAddress#test_update_handler_address().
  TestDockerCompaction: TestDockerCompaction#
  TestDockerCompaction.test_history_seeded_as_list: TestDockerCompaction#test_history_seeded_as_list().
  TestDockerCompaction.test_append_compaction_entry: TestDockerCompaction#test_append_compaction_entry().
  TestDockerCompaction.test_append_ignored_without_compaction: TestDockerCompaction#test_append_ignored_without_compaction().
  TestDockerCompaction.test_history_survives_model_overwrite: TestDockerCompaction#test_history_survives_model_overwrite().
---
# Module: [`tests/test_docker_repl_persistent.py`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py)

## Classes
### `TestDockerCompaction`
- def: [`tests/test_docker_repl_persistent.py:109`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L109)
- signature: `class TestDockerCompaction:`
- members:
  - `test_append_compaction_entry(self, repl_compaction)` — [`L114`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L114)
  - `test_append_ignored_without_compaction(self, repl)` — [`L123`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L123)
  - `test_history_seeded_as_list(self, repl_compaction)` — [`L110`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L110)
  - `test_history_survives_model_overwrite(self, repl_compaction)` — [`L127`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L127)

### `TestDockerMultiContext`
- def: [`tests/test_docker_repl_persistent.py:51`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L51)
- signature: `class TestDockerMultiContext:`
- members:
  - `test_add_context_auto_increment(self, repl)` — [`L59`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L59)
  - `test_add_context_versioning_and_access(self, repl)` — [`L52`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L52)
  - `test_context_alias_points_to_first(self, repl)` — [`L66`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L66)
  - `test_dict_context(self, repl)` — [`L72`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L72)

### `TestDockerMultiHistory`
- def: [`tests/test_docker_repl_persistent.py:78`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L78)
- signature: `class TestDockerMultiHistory:`
- members:
  - `test_add_history_deep_copy(self, repl)` — [`L93`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L93)
  - `test_add_history_versioning(self, repl)` — [`L79`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L79)
  - `test_history_alias_points_to_first(self, repl)` — [`L88`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L88)

### `TestDockerProtocol`
- def: [`tests/test_docker_repl_persistent.py:46`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L46)
- signature: `class TestDockerProtocol:`
- members:
  - `test_satisfies_persistence_protocol(self, repl)` — [`L47`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L47)
- uses (calls/refs, reference-scoped): [`SupportsPersistence`](../rlm/environments/base_env.md#SupportsPersistence)

### `TestDockerUpdateHandlerAddress`
- def: [`tests/test_docker_repl_persistent.py:102`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L102)
- signature: `class TestDockerUpdateHandlerAddress:`
- members:
  - `test_update_handler_address(self, repl)` — [`L103`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L103)

## Functions
- `_docker_available()` — [`L16`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L16)
- `repl()` — [`L29`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L29)
- `repl_compaction()` — [`L38`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L38)

## Module values
- `pytestmark` — [`L25`](../../../../../raw/code/rlm/tests/test_docker_repl_persistent.py#L25)

