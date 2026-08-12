---
title: 'Module: utils/stores/bootstrap.py'
type: catalog
provenance: extracted
module: utils/stores/bootstrap.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.stores.bootstrap`/
symbols:
  bootstrap_stores: bootstrap_stores().
  SANITIZED_PROMPT_FILENAME: SANITIZED_PROMPT_FILENAME.
  _preprocess_bootstrap_prompt: _preprocess_bootstrap_prompt().
  _materialize_prompt_override: _materialize_prompt_override().
  logger: logger.
  _resolve_prompt: _resolve_prompt().
  _extract_numeric_id: _extract_numeric_id().
  PROMPT_CANONICAL: PROMPT_CANONICAL.
  _normalize_prompt_text: _normalize_prompt_text().
  _repath_entries: _repath_entries().
  _merge_into_target: _merge_into_target().
  STORE_FILES: STORE_FILES.
  _STEPS_PATTERN: _STEPS_PATTERN.
---
# Module: [`utils/stores/bootstrap.py`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py)

## Functions
- `_extract_numeric_id(entry_id: str)` — [`L160`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L160) — Extract the numeric suffix from auto-generated IDs like ``mem_0042``.
- `_materialize_prompt_override(source_dir: str, target_cache_dir: str, backend: Optional[str] = None, model_name: Optional[str] = None)` — [`L124`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L124) — Resolve and optionally preprocess the bootstrap prompt into the target cache.
- `_merge_into_target(source_data: dict, target_file: str)` — [`L179`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L179) — Merge bootstrapped entries into an existing target store file.
- `_normalize_prompt_text(prompt_text: str)` — [`L46`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L46) — Normalize prompt text so downstream prompt assembly is clean.
- `_preprocess_bootstrap_prompt(prompt_text: str, backend: Optional[str], model_name: Optional[str])` — [`L57`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L57) — Use one VLM call to conservatively strip run-specific strategy/objective text.
- `_repath_entries(data: dict)` — [`L166`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L166) — Mutate entries in-place: prefix paths with ``bootstrapped/``, tag source.
- `_resolve_prompt(source_dir: str)` — [`L27`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L27) — Find the evolved orchestrator policy in *source_dir*.
- `bootstrap_stores(source_dir: str, target_cache_dir: str, prompt_backend: Optional[str] = None, prompt_model_name: Optional[str] = None)` — [`L223`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L223) — Load stores from *source_dir*, re-path under ``bootstrapped/``, write to *target_cache_dir*.

## Module values
- `PROMPT_CANONICAL` — [`L22`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L22)
- `SANITIZED_PROMPT_FILENAME` — [`L23`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L23)
- `STORE_FILES` — [`L20`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L20)
- `_STEPS_PATTERN` — [`L24`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L24)
- `logger` — [`L18`](../../../../../../raw/code/continual-harness/utils/stores/bootstrap.py#L18)

