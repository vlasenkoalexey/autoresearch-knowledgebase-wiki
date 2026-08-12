---
title: 'Module: tests/test_bootstrap.py'
type: catalog
provenance: extracted
module: tests/test_bootstrap.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_bootstrap`/
symbols:
  _write_store: _write_store().
  TestBootstrapRoundTrip.test_export_then_import: TestBootstrapRoundTrip#test_export_then_import().
  _sample_memory_entry: _sample_memory_entry().
  TestBootstrapExport._make_run_env: TestBootstrapExport#_make_run_env().
  TestBootstrapImport.test_happy_path: TestBootstrapImport#test_happy_path().
  TestBootstrapImport.test_prompt_canonical_found: TestBootstrapImport#test_prompt_canonical_found().
  TestBootstrapImport.test_prompt_sanitization_uses_single_vlm_call: TestBootstrapImport#test_prompt_sanitization_uses_single_vlm_call().
  TestBootstrapImport.test_prompt_sanitization_falls_back_to_normalized_original: TestBootstrapImport#test_prompt_sanitization_falls_back_to_normalized_original().
  TestBootstrapExport.test_creates_bootstrap_directory: TestBootstrapExport#test_creates_bootstrap_directory().
  TestBootstrapExport.test_copies_latest_evolved_prompt: TestBootstrapExport#test_copies_latest_evolved_prompt().
  TestBootstrapExport.test_no_evolved_prompt_still_exports_stores: TestBootstrapExport#test_no_evolved_prompt_still_exports_stores().
  TestBootstrapExport.test_dual_write: TestBootstrapExport#test_dual_write().
  TestRecencyTracking.test_recent_roots_promoted: TestRecencyTracking#test_recent_roots_promoted().
  TestBootstrapImport.test_prompt_steps_fallback: TestBootstrapImport#test_prompt_steps_fallback().
  TestBootstrapImport.test_no_prompt: TestBootstrapImport#test_no_prompt().
  TestRecencyTracking.test_recent_access_tracked: TestRecencyTracking#test_recent_access_tracked().
  TestBootstrapImport.test_missing_store_file: TestBootstrapImport#test_missing_store_file().
  TestBootstrapImport.test_preserves_mutation_history: TestBootstrapImport#test_preserves_mutation_history().
  TestBootstrapImport.test_next_id_reconciliation: TestBootstrapImport#test_next_id_reconciliation().
  TestBootstrapImport.test_merge_with_existing_entries: TestBootstrapImport#test_merge_with_existing_entries().
  TestBootstrapImport.test_id_collision_prefix: TestBootstrapImport#test_id_collision_prefix().
  TestBootstrapImport.test_repath_single_prefix: TestBootstrapImport#test_repath_single_prefix().
  TestBootstrapImport.test_repath_double_prefix: TestBootstrapImport#test_repath_double_prefix().
  TestBootstrapImport.test_repath_empty_path: TestBootstrapImport#test_repath_empty_path().
  TestPromptSeedOverride.test_override_takes_precedence: TestPromptSeedOverride#test_override_takes_precedence().
  TestPromptSeedOverride.test_fallback_to_seed_without_override: TestPromptSeedOverride#test_fallback_to_seed_without_override().
  TestResolvePrompt.test_canonical_first: TestResolvePrompt#test_canonical_first().
  _make_store_json: _make_store_json().
  _sample_skill_entry: _sample_skill_entry().
  TestBootstrapImport.test_empty_source_dir_exits: TestBootstrapImport#test_empty_source_dir_exits().
  TestBootstrapImport.test_nonexistent_source_dir_exits: TestBootstrapImport#test_nonexistent_source_dir_exits().
  TestPromptNormalization.test_strips_optimizer_header: TestPromptNormalization#test_strips_optimizer_header().
  TestPromptNormalization.test_keeps_regular_prompt: TestPromptNormalization#test_keeps_regular_prompt().
  TestResolvePrompt.test_steps_fallback: TestResolvePrompt#test_steps_fallback().
  TestResolvePrompt.test_none_when_empty: TestResolvePrompt#test_none_when_empty().
  TestExtractNumericId.test_standard_ids: TestExtractNumericId#test_standard_ids().
  TestExtractNumericId.test_custom_ids: TestExtractNumericId#test_custom_ids().
  TestExtractNumericId.test_mixed_ids: TestExtractNumericId#test_mixed_ids().
  _sample_subagent_entry: _sample_subagent_entry().
  TestBootstrapImport: TestBootstrapImport#
  TestBootstrapExport: TestBootstrapExport#
  TestBootstrapRoundTrip: TestBootstrapRoundTrip#
  TestPromptSeedOverride: TestPromptSeedOverride#
  TestPromptNormalization: TestPromptNormalization#
  TestResolvePrompt: TestResolvePrompt#
  TestExtractNumericId: TestExtractNumericId#
  TestRecencyTracking: TestRecencyTracking#
---
# Module: [`tests/test_bootstrap.py`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py)

## Classes
### `TestBootstrapExport`
- def: [`tests/test_bootstrap.py:351`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L351)
- doc: Tests for _export_bootstrap_artifacts() in RunDataManager.
- signature: `class TestBootstrapExport:`
- members:
  - `_make_run_env(self, tmp_path)` — [`L354`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L354) — Set up a mock RunDataManager environment.
  - `test_copies_latest_evolved_prompt(self, tmp_path, monkeypatch)` — [`L404`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L404)
  - `test_creates_bootstrap_directory(self, tmp_path, monkeypatch)` — [`L375`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L375)
  - `test_dual_write(self, tmp_path, monkeypatch)` — [`L453`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L453)
  - `test_no_evolved_prompt_still_exports_stores(self, tmp_path, monkeypatch)` — [`L430`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L430)
- uses (calls/refs, reference-scoped): [`run_dir`](../utils/data_persistence/run_data_manager.md#RunDataManager.run_dir), [`RunDataManager`](../utils/data_persistence/run_data_manager.md#RunDataManager), [`run_id`](../utils/data_persistence/run_data_manager.md#RunDataManager.run_id), [`_export_bootstrap_artifacts`](../utils/data_persistence/run_data_manager.md#RunDataManager._export_bootstrap_artifacts)  (4 test-only)

### `TestBootstrapImport`
- def: [`tests/test_bootstrap.py:94`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L94)
- doc: Tests for bootstrap_stores() import function.
- signature: `class TestBootstrapImport:`
- members:
  - `test_empty_source_dir_exits(self, tmp_path)` — [`L140`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L140)
  - `test_happy_path(self, tmp_path)` — [`L97`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L97)
  - `test_id_collision_prefix(self, tmp_path)` — [`L224`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L224) — When a bootstrapped entry ID already exists in target, prefix with bs_.
  - `test_merge_with_existing_entries(self, tmp_path)` — [`L201`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L201)
  - `test_missing_store_file(self, tmp_path)` — [`L124`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L124)
  - `test_next_id_reconciliation(self, tmp_path)` — [`L184`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L184)
  - `test_no_prompt(self, tmp_path)` — [`L272`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L272)
  - `test_nonexistent_source_dir_exits(self, tmp_path)` — [`L148`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L148)
  - `test_preserves_mutation_history(self, tmp_path)` — [`L169`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L169)
  - `test_prompt_canonical_found(self, tmp_path)` — [`L245`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L245)
  - `test_prompt_sanitization_falls_back_to_normalized_original(self, tmp_path)` — [`L319`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L319)
  - `test_prompt_sanitization_uses_single_vlm_call(self, tmp_path)` — [`L284`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L284)
  - `test_prompt_steps_fallback(self, tmp_path)` — [`L258`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L258)
  - `test_repath_double_prefix(self)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L158) — Multi-generation bootstrap: already-bootstrapped entries get double-prefixed.
  - `test_repath_empty_path(self)` — [`L164`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L164)
  - `test_repath_single_prefix(self)` — [`L152`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L152)
- uses (calls/refs, reference-scoped): [`bootstrap_stores`](../utils/stores/bootstrap.md#bootstrap_stores), [`SANITIZED_PROMPT_FILENAME`](../utils/stores/bootstrap.md#SANITIZED_PROMPT_FILENAME), [`PROMPT_CANONICAL`](../utils/stores/bootstrap.md#PROMPT_CANONICAL), [`_repath_entries`](../utils/stores/bootstrap.md#_repath_entries)  (5 test-only)

### `TestBootstrapRoundTrip`
- def: [`tests/test_bootstrap.py:482`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L482)
- doc: Export then import — verify entries survive the full pipeline.
- signature: `class TestBootstrapRoundTrip:`
- members:
  - `test_export_then_import(self, tmp_path, monkeypatch)` — [`L485`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L485)
- uses (calls/refs, reference-scoped): [`run_dir`](../utils/data_persistence/run_data_manager.md#RunDataManager.run_dir), [`bootstrap_stores`](../utils/stores/bootstrap.md#bootstrap_stores), [`RunDataManager`](../utils/data_persistence/run_data_manager.md#RunDataManager), [`run_id`](../utils/data_persistence/run_data_manager.md#RunDataManager.run_id), [`_export_bootstrap_artifacts`](../utils/data_persistence/run_data_manager.md#RunDataManager._export_bootstrap_artifacts)  (3 test-only)

### `TestExtractNumericId`
- def: [`tests/test_bootstrap.py:634`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L634)
- signature: `class TestExtractNumericId:`
- members:
  - `test_custom_ids(self)` — [`L641`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L641)
  - `test_mixed_ids(self)` — [`L645`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L645)
  - `test_standard_ids(self)` — [`L636`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L636)
- uses (calls/refs, reference-scoped): [`_extract_numeric_id`](../utils/stores/bootstrap.md#_extract_numeric_id)

### `TestPromptNormalization`
- def: [`tests/test_bootstrap.py:598`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L598)
- signature: `class TestPromptNormalization:`
- members:
  - `test_keeps_regular_prompt(self)` — [`L604`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L604)
  - `test_strips_optimizer_header(self)` — [`L599`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L599)
- uses (calls/refs, reference-scoped): [`_normalize_prompt_text`](../utils/stores/bootstrap.md#_normalize_prompt_text)

### `TestPromptSeedOverride`
- def: [`tests/test_bootstrap.py:551`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L551)
- doc: Tests for initial_prompt_override in PromptOptimizer.
- signature: `class TestPromptSeedOverride:`
- members:
  - `test_fallback_to_seed_without_override(self, tmp_path)` — [`L574`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L574)
  - `test_override_takes_precedence(self, tmp_path)` — [`L554`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L554)
- uses (calls/refs, reference-scoped): [`PromptOptimizer`](../agents/utils/prompt_optimizer.md#PromptOptimizer), [`get_current_prompt`](../agents/utils/prompt_optimizer.md#PromptOptimizer.get_current_prompt)

### `TestRecencyTracking`
- def: [`tests/test_bootstrap.py:653`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L653)
- doc: Verify that recently-accessed entries influence tree overview ordering.
- signature: `class TestRecencyTracking:`
- members:
  - `test_recent_access_tracked(self)` — [`L656`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L656)
  - `test_recent_roots_promoted(self)` — [`L665`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L665)
- uses (calls/refs, reference-scoped): [`add`](../utils/stores/base_store.md#BaseStore.add), [`get_tree_overview`](../utils/stores/base_store.md#BaseStore.get_tree_overview), [`get`](../utils/stores/base_store.md#BaseStore.get), [`_invalidate_cache`](../utils/stores/base_store.md#BaseStore._invalidate_cache), [`_recent_access_ids`](../utils/stores/base_store.md#BaseStore._recent_access_ids)  (1 test-only)

### `TestResolvePrompt`
- def: [`tests/test_bootstrap.py:612`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L612)
- doc: Tests for the _resolve_prompt fallback chain.
- signature: `class TestResolvePrompt:`
- members:
  - `test_canonical_first(self, tmp_path)` — [`L615`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L615)
  - `test_none_when_empty(self, tmp_path)` — [`L626`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L626)
  - `test_steps_fallback(self, tmp_path)` — [`L620`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L620)
- uses (calls/refs, reference-scoped): [`_resolve_prompt`](../utils/stores/bootstrap.md#_resolve_prompt), [`PROMPT_CANONICAL`](../utils/stores/bootstrap.md#PROMPT_CANONICAL)

## Functions
- `_make_store_json(entries: dict, next_id: int = 1)` — [`L25`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L25)
- `_sample_memory_entry(eid="mem_0001", path="pokemon/team", title="My Team", source="orchestrator")` — [`L35`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L35)
- `_sample_skill_entry(eid="skill_0001", path="navigation", name="pathfinder")` — [`L51`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L51)
- `_sample_subagent_entry(eid="sa_0001", path="custom", name="battler")` — [`L68`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L68)
- `_write_store(path, entries: dict, next_id: int = 1)` — [`L29`](../../../../../raw/code/continual-harness/tests/test_bootstrap.py#L29)

