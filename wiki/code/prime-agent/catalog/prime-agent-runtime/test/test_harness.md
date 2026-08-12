---
title: 'Module: prime-agent-runtime/test/test_harness.py'
type: catalog
provenance: extracted
module: prime-agent-runtime/test/test_harness.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `prime-agent-runtime.test.test_harness`/
symbols:
  PYTHON_REFERENCE: PYTHON_REFERENCE.
  HarnessStateTest.test_crud_for_all_entry_kinds: HarnessStateTest#test_crud_for_all_entry_kinds().
  HarnessStateTest.test_persists_entries_and_refinements: HarnessStateTest#test_persists_entries_and_refinements().
  HarnessStateTest.test_update_skill_preserves_omitted_arguments: HarnessStateTest#test_update_skill_preserves_omitted_arguments().
  HarnessStateTest.test_update_skill_without_reference_preserves_contract: HarnessStateTest#test_update_skill_without_reference_preserves_contract().
  HarnessStateTest.test_explicit_create_and_update_enforce_entry_existence: HarnessStateTest#test_explicit_create_and_update_enforce_entry_existence().
  HarnessStateTest: HarnessStateTest#
  HarnessStateTest.test_load_ignores_unknown_json_keys: HarnessStateTest#test_load_ignores_unknown_json_keys().
  HarnessStateTest.test_skill_arguments_are_first_class: HarnessStateTest#test_skill_arguments_are_first_class().
  HarnessStateTest.test_skill_references_must_be_python: HarnessStateTest#test_skill_references_must_be_python().
  HarnessStateTest.test_load_tolerates_corrupt_or_non_object_state: HarnessStateTest#test_load_tolerates_corrupt_or_non_object_state().
  HarnessStateTest.test_update_preserves_omitted_path: HarnessStateTest#test_update_preserves_omitted_path().
  HarnessStateTest.test_in_memory_state_never_touches_disk: HarnessStateTest#test_in_memory_state_never_touches_disk().
  HarnessStateTest.test_in_memory_state_global_flag_uses_global_env_store: HarnessStateTest#test_in_memory_state_global_flag_uses_global_env_store().
  HarnessStateTest.test_in_memory_state_global_flag_uses_default_global_store: HarnessStateTest#test_in_memory_state_global_flag_uses_default_global_store().
  HarnessStateTest.test_reloads_external_writes_before_mutating: HarnessStateTest#test_reloads_external_writes_before_mutating().
  HarnessStateTest.test_create_detects_externally_written_entry: HarnessStateTest#test_create_detects_externally_written_entry().
  HarnessStateTest.test_explicit_state_dir_cache_uses_harness_state_file: HarnessStateTest#test_explicit_state_dir_cache_uses_harness_state_file().
  HarnessStateTest.test_explicit_state_dir_global_flag_uses_matching_state_file: HarnessStateTest#test_explicit_state_dir_global_flag_uses_matching_state_file().
  HarnessStateTest.test_env_default_state_keeps_env_global_target_after_explicit_dir_cache_hit: HarnessStateTest#test_env_default_state_keeps_env_global_target_after_explicit_dir_cache_hit().
  HarnessStateTest.test_local_state_requires_local_path: HarnessStateTest#test_local_state_requires_local_path().
  HarnessStateTest.test_default_state_uses_global_harness_env_dir: HarnessStateTest#test_default_state_uses_global_harness_env_dir().
  HarnessStateTest.test_global_scope_default_state_uses_global_harness_env_dir: HarnessStateTest#test_global_scope_default_state_uses_global_harness_env_dir().
  HarnessStateTest.test_default_state_is_local_and_global_flag_targets_global_store: HarnessStateTest#test_default_state_is_local_and_global_flag_targets_global_store().
  HarnessStateTest.test_global_kwarg_must_be_boolean: HarnessStateTest#test_global_kwarg_must_be_boolean().
  HarnessStateTest.test_state_cache_keeps_scope_distinct_when_local_and_global_share_a_file: HarnessStateTest#test_state_cache_keeps_scope_distinct_when_local_and_global_share_a_file().
  HarnessStateTest.test_scope_prefixed_ids_route_to_the_displayed_scope: HarnessStateTest#test_scope_prefixed_ids_route_to_the_displayed_scope().
  HarnessStateTest.test_create_with_prefixed_id_does_not_mint_literal_id: HarnessStateTest#test_create_with_prefixed_id_does_not_mint_literal_id().
  HarnessStateTest.test_module_harness_binds_lazily_to_env_set_after_import: HarnessStateTest#test_module_harness_binds_lazily_to_env_set_after_import().
  HarnessStateTest.test_module_harness_without_env_raises_on_local_writes_and_reads_work: HarnessStateTest#test_module_harness_without_env_raises_on_local_writes_and_reads_work().
  HarnessStateTest.test_module_harness_without_env_still_routes_global_writes: HarnessStateTest#test_module_harness_without_env_still_routes_global_writes().
  HarnessStateTest.test_import_rlm_without_env_does_not_raise: HarnessStateTest#test_import_rlm_without_env_does_not_raise().
  HarnessStateTest.test_empty_local_state_dir_env_is_treated_as_unset: HarnessStateTest#test_empty_local_state_dir_env_is_treated_as_unset().
  HarnessStateTest.test_explicit_dir_aliasing_env_local_dir_keeps_env_global_target: HarnessStateTest#test_explicit_dir_aliasing_env_local_dir_keeps_env_global_target().
  HarnessStateTest.test_callable_rlm_exposes_harness_state_helpers: HarnessStateTest#test_callable_rlm_exposes_harness_state_helpers().
  HarnessStateTest.test_record_refinement_accepts_single_change_string: HarnessStateTest#test_record_refinement_accepts_single_change_string().
  HarnessStateTest.test_unknown_kind_rejected: HarnessStateTest#test_unknown_kind_rejected().
---
# Module: [`prime-agent-runtime/test/test_harness.py`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py)

## Classes
### `HarnessStateTest`  ·  implements/extends TestCase
- def: [`prime-agent-runtime/test/test_harness.py:23`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L23)
- signature: `class HarnessStateTest(unittest.TestCase):`
- members:
  - `test_callable_rlm_exposes_harness_state_helpers(self)` — [`L907`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L907)
  - `test_create_detects_externally_written_entry(self)` — [`L438`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L438)
  - `test_create_with_prefixed_id_does_not_mint_literal_id(self)` — [`L711`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L711)
  - `test_crud_for_all_entry_kinds(self)` — [`L24`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L24)
  - `test_default_state_is_local_and_global_flag_targets_global_store(self)` — [`L594`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L594)
  - `test_default_state_uses_global_harness_env_dir(self)` — [`L557`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L557)
  - `test_empty_local_state_dir_env_is_treated_as_unset(self)` — [`L846`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L846)
  - `test_env_default_state_keeps_env_global_target_after_explicit_dir_cache_hit(self)` — [`L499`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L499)
  - `test_explicit_create_and_update_enforce_entry_existence(self)` — [`L454`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L454)
  - `test_explicit_dir_aliasing_env_local_dir_keeps_env_global_target(self)` — [`L876`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L876)
  - `test_explicit_state_dir_cache_uses_harness_state_file(self)` — [`L470`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L470)
  - `test_explicit_state_dir_global_flag_uses_matching_state_file(self)` — [`L478`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L478)
  - `test_global_kwarg_must_be_boolean(self)` — [`L635`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L635)
  - `test_global_scope_default_state_uses_global_harness_env_dir(self)` — [`L571`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L571)
  - `test_import_rlm_without_env_does_not_raise(self)` — [`L833`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L833)
  - `test_in_memory_state_global_flag_uses_default_global_store(self)` — [`L383`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L383)
  - `test_in_memory_state_global_flag_uses_global_env_store(self)` — [`L360`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L360)
  - `test_in_memory_state_never_touches_disk(self)` — [`L334`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L334)
  - `test_load_ignores_unknown_json_keys(self)` — [`L137`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L137)
  - `test_load_tolerates_corrupt_or_non_object_state(self)` — [`L268`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L268)
  - `test_local_state_requires_local_path(self)` — [`L539`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L539)
  - `test_module_harness_binds_lazily_to_env_set_after_import(self)` — [`L739`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L739)
  - `test_module_harness_without_env_raises_on_local_writes_and_reads_work(self)` — [`L770`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L770)
  - `test_module_harness_without_env_still_routes_global_writes(self)` — [`L802`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L802)
  - `test_persists_entries_and_refinements(self)` — [`L88`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L88)
  - `test_record_refinement_accepts_single_change_string(self)` — [`L911`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L911)
  - `test_reloads_external_writes_before_mutating(self)` — [`L413`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L413)
  - `test_scope_prefixed_ids_route_to_the_displayed_scope(self)` — [`L673`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L673)
  - `test_skill_arguments_are_first_class(self)` — [`L198`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L198)
  - `test_skill_references_must_be_python(self)` — [`L245`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L245)
  - `test_state_cache_keeps_scope_distinct_when_local_and_global_share_a_file(self)` — [`L642`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L642)
  - `test_unknown_kind_rejected(self)` — [`L920`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L920)
  - `test_update_preserves_omitted_path(self)` — [`L321`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L321)
  - `test_update_skill_preserves_omitted_arguments(self)` — [`L282`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L282)
  - `test_update_skill_without_reference_preserves_contract(self)` — [`L301`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L301)
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Module values
- `PYTHON_REFERENCE` — [`L15`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_harness.py#L15)

