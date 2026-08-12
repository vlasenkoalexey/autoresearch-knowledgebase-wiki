---
title: 'Module: utils/run_artifact_cleanup.py'
type: catalog
provenance: extracted
module: utils/run_artifact_cleanup.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.run_artifact_cleanup`/
symbols:
  run_run_artifact_cleanup: run_run_artifact_cleanup().
  CleanupResult.as_dict: CleanupResult#as_dict().
  CleanupResult.warnings: CleanupResult#warnings.
  embedded_date_from_dir_name: embedded_date_from_dir_name().
  CleanupResult.success: CleanupResult#success.
  CleanupResult.error: CleanupResult#error.
  CleanupResult.sample_removed_dirs: CleanupResult#sample_removed_dirs.
  CleanupResult.sample_deleted_files: CleanupResult#sample_deleted_files.
  _safe_roots: _safe_roots().
  CleanupResult.dry_run: CleanupResult#dry_run.
  CleanupResult.files_deleted: CleanupResult#files_deleted.
  CleanupResult.files_would_delete: CleanupResult#files_would_delete.
  CleanupResult.dirs_removed: CleanupResult#dirs_removed.
  CleanupResult.dirs_would_remove: CleanupResult#dirs_would_remove.
  CleanupResult: CleanupResult#
  CleanupResult.repo_root: CleanupResult#repo_root.
  CleanupResult.file_mtime_on_or_after: CleanupResult#file_mtime_on_or_after.
  CleanupResult.directory_embedded_date_on_or_after: CleanupResult#directory_embedded_date_on_or_after.
  DEFAULT_ROOTS: DEFAULT_ROOTS.
  _EMBEDDED_DATE: _EMBEDDED_DATE.
  _RUN_EMBEDDED_DATE: _RUN_EMBEDDED_DATE.
  repo_root_from_utils: repo_root_from_utils().
  _parse_file_mtime_cutoff: _parse_file_mtime_cutoff().
  _parse_embedded_date_int: _parse_embedded_date_int().
  run_run_artifact_cleanup.on_walk_error: run_run_artifact_cleanup().on_walk_error().
---
# Module: [`utils/run_artifact_cleanup.py`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py)

## Classes
### `CleanupResult`
- def: [`utils/run_artifact_cleanup.py:87`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L87)
- signature: `class CleanupResult:`
- members:
  - `as_dict(self)` — [`L102`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L102)
  - `directory_embedded_date_on_or_after` — [`L93`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L93)
  - `dirs_removed` — [`L96`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L96)
  - `dirs_would_remove` — [`L97`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L97)
  - `dry_run` — [`L89`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L89)
  - `error` — [`L90`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L90)
  - `file_mtime_on_or_after` — [`L92`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L92)
  - `files_deleted` — [`L94`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L94)
  - `files_would_delete` — [`L95`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L95)
  - `repo_root` — [`L91`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L91)
  - `sample_deleted_files` — [`L99`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L99)
  - `sample_removed_dirs` — [`L98`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L98)
  - `success` — [`L88`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L88)
  - `warnings` — [`L100`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L100)
- used by: [`run_run_artifact_cleanup`](run_artifact_cleanup.md#run_run_artifact_cleanup), [`_execute_subagent_cleanup_run_artifacts`](../agents/PokeAgent.md#PokeAgent._execute_subagent_cleanup_run_artifacts)

## Functions
- `_parse_embedded_date_int(s: str)` — [`L48`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L48)
- `_parse_file_mtime_cutoff(s: str)` — [`L34`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L34)
- `_safe_roots(repo_root: Path, roots: Optional[List[str]])` — [`L71`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L71)
- `embedded_date_from_dir_name(name: str)` — [`L61`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L61)
- `on_walk_error(exc: OSError)` — [`L213`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L213)
- `repo_root_from_utils()` — [`L29`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L29) — Repository root (parent of ``utils/``).
- `run_run_artifact_cleanup(*, repo_root: Optional[Path] = None, reasoning: str = "", dry_run: bool = True, file_mtime_on_or_after: Optional[str] = None, directory_embedded_date_on_or_after: Optional[str] = None, roots: Optional[List[str]] = None, max_path_samples: int = 80)` — [`L122`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L122) — Apply cleanup rules. At least one of *file_mtime_on_or_after* or

## Module values
- `DEFAULT_ROOTS` — [`L23`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L23)
- `_EMBEDDED_DATE` — [`L25`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L25)
- `_RUN_EMBEDDED_DATE` — [`L26`](../../../../../raw/code/continual-harness/utils/run_artifact_cleanup.py#L26)

