---
title: 'Module: OpenMLE-Gym/tests/test_perceive.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_perceive.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_perceive`/
symbols:
  PerceiveTests.test_empty_fileinfo_preserves_raw_on_delete_request: PerceiveTests#test_empty_fileinfo_preserves_raw_on_delete_request().
  PerceiveTests._node: PerceiveTests#_node().
  PerceiveTests.test_llm_exception_uses_fail_open_exit: PerceiveTests#test_llm_exception_uses_fail_open_exit().
  PerceiveTests.test_saved_substring_from_other_tool_degrades: PerceiveTests#test_saved_substring_from_other_tool_degrades().
  PerceiveTests.test_no_tool_call_uses_fail_open_exit: PerceiveTests#test_no_tool_call_uses_fail_open_exit().
  PerceiveTests.test_filtered_tool_calls_use_fail_open_exit: PerceiveTests#test_filtered_tool_calls_use_fail_open_exit().
  PerceiveTests.test_tool_call_limit_uses_fail_open_exit: PerceiveTests#test_tool_call_limit_uses_fail_open_exit().
  PerceiveTests.test_only_successful_save_tool_message_completes_normally: PerceiveTests#test_only_successful_save_tool_message_completes_normally().
  PerceiveTests.test_truncated_text_preview_is_larger_and_explicitly_one_shot: PerceiveTests#test_truncated_text_preview_is_larger_and_explicitly_one_shot().
  HAS_BUILDER_DEPS: HAS_BUILDER_DEPS.
  PerceiveTests.test_archive_path_traversal_is_rejected: PerceiveTests#test_archive_path_traversal_is_rejected().
  REQUIRED_MODULES: REQUIRED_MODULES.
  PerceiveTests.fail: PerceiveTests#fail().
  PerceiveTests: PerceiveTests#
---
# Module: [`OpenMLE-Gym/tests/test_perceive.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py)

## Classes
### `PerceiveTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_perceive.py:22`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L22)
- signature: `class PerceiveTests(unittest.TestCase):`
- members:
  - `fail(_)` — [`L94`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L94)
  - `test_archive_path_traversal_is_rejected(self)` — [`L192`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L192)
  - `test_empty_fileinfo_preserves_raw_on_delete_request(self)` — [`L159`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L159) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_filtered_tool_calls_use_fail_open_exit(self)` — [`L102`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L102) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_llm_exception_uses_fail_open_exit(self)` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L88) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_no_tool_call_uses_fail_open_exit(self)` — [`L76`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L76) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_only_successful_save_tool_message_completes_normally(self)` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L37) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_saved_substring_from_other_tool_degrades(self)` — [`L55`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L55) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_tool_call_limit_uses_fail_open_exit(self)` — [`L123`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L123) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `test_truncated_text_preview_is_larger_and_explicitly_one_shot(self)` — [`L140`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L140)
- protocol/private: `_node`[`L23`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L23)
- uses (calls/refs, reference-scoped): [`todo`](../builder_core/utils/nodes.md#NodeExecutor.todo), [`structure`](../builder_core/utils/nodes.md#NodeExecutor.structure), [`Perceive`](../builder_core/utils/nodes.md#NodeExecutor.Perceive), [`comp_id_dir`](../builder_core/utils/struct.md#Structure.comp_id_dir), [`Next`](../builder_core/utils/nodes.md#NodeExecutor.Next), [`NodeExecutor`](../builder_core/utils/nodes.md#NodeExecutor), [`configure_task_paths`](../builder_core/tools/tools.md#configure_task_paths), [`raw_dir`](../builder_core/utils/struct.md#Structure.raw_dir), [`extract`](../builder_core/utils/nodes.md#NodeExecutor.extract), [`llm_provider_tools`](../builder_core/utils/nodes.md#NodeExecutor.llm_provider_tools), [`read_txt_md`](../builder_core/tools/tools.md#read_txt_md), [`tools`](../builder_core/utils/nodes.md#NodeExecutor.tools), [`Structure`](../builder_core/utils/struct.md#Structure), [`gen_perceiver`](../builder_core/utils/prompts.md#gen_perceiver), [`max_tool_call`](../builder_core/utils/nodes.md#NodeExecutor.max_tool_call), [`delete_raw`](../builder_core/utils/nodes.md#NodeExecutor.delete_raw)

## Module values
- `HAS_BUILDER_DEPS` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L18)
- `REQUIRED_MODULES` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_perceive.py#L11)

