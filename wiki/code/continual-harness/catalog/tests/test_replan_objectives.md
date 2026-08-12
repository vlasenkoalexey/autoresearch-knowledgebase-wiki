---
title: 'Module: tests/test_replan_objectives.py'
type: catalog
provenance: extracted
module: tests/test_replan_objectives.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_replan_objectives`/
symbols:
  _obj: _obj().
  _make_manager: _make_manager().
  TestSequenceExhaustion.test_story_exhaustion_appends_fallback: TestSequenceExhaustion#test_story_exhaustion_appends_fallback().
  TestReplanCategoryHappyPath.test_modify_existing_objective: TestReplanCategoryHappyPath#test_modify_existing_objective().
  TestSequenceExhaustion.test_fallback_not_duplicated_on_repeated_calls: TestSequenceExhaustion#test_fallback_not_duplicated_on_repeated_calls().
  TestServerEndpointSimulation.test_replan_does_not_affect_completed_objectives: TestServerEndpointSimulation#test_replan_does_not_affect_completed_objectives().
  TestJsonUtilsReplanProtobuf.test_replan_category_accepts_string_index_after_normalize: TestJsonUtilsReplanProtobuf#test_replan_category_accepts_string_index_after_normalize().
  TestReplanCategoryHappyPath.test_append_new_objective: TestReplanCategoryHappyPath#test_append_new_objective().
  TestReplanCategoryHappyPath.test_delete_existing_objective: TestReplanCategoryHappyPath#test_delete_existing_objective().
  TestReplanCategoryHappyPath.test_mixed_operations: TestReplanCategoryHappyPath#test_mixed_operations().
  TestReplanCategoryHappyPath.test_replan_adds_objective_after_create_placeholder: TestReplanCategoryHappyPath#test_replan_adds_objective_after_create_placeholder().
  TestReplanCategoryHappyPath.test_delete_current_objective_adjusts_index: TestReplanCategoryHappyPath#test_delete_current_objective_adjusts_index().
  TestReplanCategoryHappyPath.test_battling_category: TestReplanCategoryHappyPath#test_battling_category().
  TestGetFullSequenceSnapshot.test_snapshot_structure: TestGetFullSequenceSnapshot#test_snapshot_structure().
  TestSequenceExhaustion.test_fallback_not_appended_when_objectives_remain: TestSequenceExhaustion#test_fallback_not_appended_when_objectives_remain().
  TestReplanCategoryHappyPath.test_replan_empty_dynamics_sequence: TestReplanCategoryHappyPath#test_replan_empty_dynamics_sequence().
  TestReplanCategoryValidation.test_invalid_category: TestReplanCategoryValidation#test_invalid_category().
  TestReplanCategoryValidation.test_too_many_edits: TestReplanCategoryValidation#test_too_many_edits().
  TestReplanCategoryValidation.test_index_below_current: TestReplanCategoryValidation#test_index_below_current().
  TestReplanCategoryValidation.test_non_contiguous_append: TestReplanCategoryValidation#test_non_contiguous_append().
  TestReplanCategoryValidation.test_delete_nonexistent_index: TestReplanCategoryValidation#test_delete_nonexistent_index().
  TestReplanCategoryValidation.test_missing_index_field: TestReplanCategoryValidation#test_missing_index_field().
  TestReplanCategoryValidation.test_edits_not_a_list: TestReplanCategoryValidation#test_edits_not_a_list().
  TestReplanCategoryHappyPath.test_append_multiple_contiguous: TestReplanCategoryHappyPath#test_append_multiple_contiguous().
  TestReplanCategoryHappyPath.test_delete_with_empty_dict: TestReplanCategoryHappyPath#test_delete_with_empty_dict().
  TestReplanCategoryHappyPath.test_no_op_empty_edits: TestReplanCategoryHappyPath#test_no_op_empty_edits().
  TestServerEndpointSimulation.test_replan_valid_request: TestServerEndpointSimulation#test_replan_valid_request().
  TestServerEndpointSimulation.test_replan_validation_error_returns_cleanly: TestServerEndpointSimulation#test_replan_validation_error_returns_cleanly().
  TestServerEndpointSimulation.test_full_sequence_is_json_serializable: TestServerEndpointSimulation#test_full_sequence_is_json_serializable().
  TestGetFullSequenceSnapshot.test_snapshot_empty_sequences: TestGetFullSequenceSnapshot#test_snapshot_empty_sequences().
  TestSequenceExhaustion.test_empty_story_sequence_returns_none: TestSequenceExhaustion#test_empty_story_sequence_returns_none().
  TestJsonUtilsReplanProtobuf.test_convert_protobuf_sequence_before_mapping: TestJsonUtilsReplanProtobuf#test_convert_protobuf_sequence_before_mapping().
  TestJsonUtilsReplanProtobuf.test_convert_protobuf_sequence_before_mapping.ProtoList: TestJsonUtilsReplanProtobuf#test_convert_protobuf_sequence_before_mapping().ProtoList#
  TestJsonUtilsReplanProtobuf.test_coerce_string_digit_index: TestJsonUtilsReplanProtobuf#test_coerce_string_digit_index().
  TestJsonUtilsReplanProtobuf.test_coerce_float_index: TestJsonUtilsReplanProtobuf#test_coerce_float_index().
  TestJsonUtilsReplanProtobuf.test_coerce_invalid_string_unchanged: TestJsonUtilsReplanProtobuf#test_coerce_invalid_string_unchanged().
  TestJsonUtilsReplanProtobuf.test_normalize_replan_edits_coerces_indices: TestJsonUtilsReplanProtobuf#test_normalize_replan_edits_coerces_indices().
  TestReplanCategoryValidation: TestReplanCategoryValidation#
  TestReplanCategoryHappyPath: TestReplanCategoryHappyPath#
  TestGetFullSequenceSnapshot: TestGetFullSequenceSnapshot#
  TestSequenceExhaustion: TestSequenceExhaustion#
  TestServerEndpointSimulation: TestServerEndpointSimulation#
  TestJsonUtilsReplanProtobuf: TestJsonUtilsReplanProtobuf#
---
# Module: [`tests/test_replan_objectives.py`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py)

## Classes
### `ProtoList`  ·  implements/extends list
- def: [`tests/test_replan_objectives.py:376`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L376)
- signature: `class ProtoList(list):`
- used by: (1 test-only callers)

### `TestGetFullSequenceSnapshot`
- def: [`tests/test_replan_objectives.py:220`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L220)
- signature: `class TestGetFullSequenceSnapshot:`
- members:
  - `test_snapshot_empty_sequences(self)` — [`L239`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L239)
  - `test_snapshot_structure(self)` — [`L221`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L221)
- uses (calls/refs, reference-scoped): [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed), [`get_full_sequence_snapshot`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.get_full_sequence_snapshot)  (2 test-only)

### `TestJsonUtilsReplanProtobuf`
- def: [`tests/test_replan_objectives.py:355`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L355)
- signature: `class TestJsonUtilsReplanProtobuf:`
- members:
  - `test_coerce_float_index(self)` — [`L360`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L360)
  - `test_coerce_invalid_string_unchanged(self)` — [`L363`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L363)
  - `test_coerce_string_digit_index(self)` — [`L356`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L356)
  - `test_convert_protobuf_sequence_before_mapping(self)` — [`L373`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L373) — Repeated-like protobuf must become a list, not a merged dict.
  - `test_normalize_replan_edits_coerces_indices(self)` — [`L366`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L366)
  - `test_replan_category_accepts_string_index_after_normalize(self)` — [`L384`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L384)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`replan_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.replan_category), [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`convert_protobuf_value`](../utils/json_utils.md#convert_protobuf_value), [`normalize_replan_edits`](../utils/json_utils.md#normalize_replan_edits), [`coerce_replan_edit_index`](../utils/json_utils.md#coerce_replan_edit_index)  (3 test-only)

### `TestReplanCategoryHappyPath`
- def: [`tests/test_replan_objectives.py:103`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L103)
- signature: `class TestReplanCategoryHappyPath:`
- members:
  - `test_append_multiple_contiguous(self)` — [`L124`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L124)
  - `test_append_new_objective(self)` — [`L114`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L114)
  - `test_battling_category(self)` — [`L206`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L206)
  - `test_delete_current_objective_adjusts_index(self)` — [`L197`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L197)
  - `test_delete_existing_objective(self)` — [`L133`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L133)
  - `test_delete_with_empty_dict(self)` — [`L141`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L141)
  - `test_mixed_operations(self)` — [`L154`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L154) — Modify one objective, delete another, and append a new one.
  - `test_modify_existing_objective(self)` — [`L104`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L104)
  - `test_no_op_empty_edits(self)` — [`L147`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L147)
  - `test_replan_adds_objective_after_create_placeholder(self)` — [`L177`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L177)
  - `test_replan_empty_dynamics_sequence(self)` — [`L168`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L168)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`action_type`](../agents/objectives/objective_types.md#DirectObjective.action_type), [`replan_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.replan_category), [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`battling_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.battling_sequence), [`story_index`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_index), [`dynamics_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.dynamics_sequence)  (2 test-only)

### `TestReplanCategoryValidation`
- def: [`tests/test_replan_objectives.py:48`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L48)
- signature: `class TestReplanCategoryValidation:`
- members:
  - `test_delete_nonexistent_index(self)` — [`L79`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L79)
  - `test_edits_not_a_list(self)` — [`L91`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L91)
  - `test_index_below_current(self)` — [`L62`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L62)
  - `test_invalid_category(self)` — [`L49`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L49)
  - `test_missing_index_field(self)` — [`L85`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L85)
  - `test_non_contiguous_append(self)` — [`L71`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L71)
  - `test_too_many_edits(self)` — [`L55`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L55)
- uses (calls/refs, reference-scoped): [`replan_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.replan_category)  (2 test-only)

### `TestSequenceExhaustion`
- def: [`tests/test_replan_objectives.py:252`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L252)
- signature: `class TestSequenceExhaustion:`
- members:
  - `test_empty_story_sequence_returns_none(self)` — [`L292`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L292) — An empty story sequence (no objectives loaded at all) should return None,
  - `test_fallback_not_appended_when_objectives_remain(self)` — [`L270`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L270) — The fallback should NOT appear when there are still uncompleted objectives.
  - `test_fallback_not_duplicated_on_repeated_calls(self)` — [`L280`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L280) — Calling _get_current_objective_for_category twice after exhaustion
  - `test_story_exhaustion_appends_fallback(self)` — [`L253`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L253) — When all story objectives are completed and index reaches the end,
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`description`](../agents/objectives/objective_types.md#DirectObjective.description), [`action_type`](../agents/objectives/objective_types.md#DirectObjective.action_type), [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`_get_current_objective_for_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager._get_current_objective_for_category), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed)  (2 test-only)

### `TestServerEndpointSimulation`
- def: [`tests/test_replan_objectives.py:305`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L305)
- doc: Simulate the shape of MCP endpoint handlers to verify the contract.
- signature: `class TestServerEndpointSimulation:`
- members:
  - `test_full_sequence_is_json_serializable(self)` — [`L326`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L326)
  - `test_replan_does_not_affect_completed_objectives(self)` — [`L335`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L335) — Replanning must not change the completed status of earlier objectives.
  - `test_replan_valid_request(self)` — [`L308`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L308)
  - `test_replan_validation_error_returns_cleanly(self)` — [`L318`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L318)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`replan_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.replan_category), [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed), [`get_full_sequence_snapshot`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.get_full_sequence_snapshot)  (2 test-only)

## Functions
- `_make_manager(story_objs=None, battling_objs=None, dynamics_objs=None, story_idx=0, battling_idx=0, dynamics_idx=0)` — [`L12`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L12) — Helper to build a minimal DirectObjectiveManager in categorized mode.
- `_obj(id_: str, desc: str = "test", **kwargs)` — [`L33`](../../../../../raw/code/continual-harness/tests/test_replan_objectives.py#L33)

