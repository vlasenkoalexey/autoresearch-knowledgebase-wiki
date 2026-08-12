---
title: 'Module: utils/data_persistence/backup_manager.py'
type: catalog
provenance: extracted
module: utils/data_persistence/backup_manager.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.data_persistence.backup_manager`/
symbols:
  logger: logger.
  create_cache_backup: create_cache_backup().
  restore_cache_from_backup: restore_cache_from_backup().
  create_cli_agent_termination_backup: create_cli_agent_termination_backup().
  _cleanup_old_backups: _cleanup_old_backups().
  list_backups: list_backups().
  _load_metrics_summary: _load_metrics_summary().
  create_cache_backup.on_walk_error: create_cache_backup().on_walk_error().
---
# Module: [`utils/data_persistence/backup_manager.py`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py)

## Functions
- `_cleanup_old_backups(backup_base_dir: Path, max_run_dirs: int = 50)` — [`L155`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L155) — Remove old run backup directories to prevent excessive disk usage.
- `_load_metrics_summary(path: Path)` — [`L19`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L19)
- `create_cache_backup(objective_id: str, objective_description: str, cache_dir: str = None, backup_base_dir: str = "backups")` — [`L35`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L35) — Create a zip backup of the .pokeagent_cache directory.
- `create_cli_agent_termination_backup(run_id: str, reason: str, cache_dir: str = None, backup_base_dir: str = "backups")` — [`L127`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L127) — Create a backup of the CLI agent cache on termination (condition met or user interrupt).
- `list_backups(backup_dir: str = "backups", limit: int = 20)` — [`L282`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L282) — List available backups (now organized in run-specific subdirectories).
- `on_walk_error(err: OSError)` — [`L93`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L93)
- `restore_cache_from_backup(backup_file: str, cache_dir: str = None, create_backup_of_current: bool = True)` — [`L187`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L187) — Restore .pokeagent_cache from a backup zip file.

## Module values
- `logger` — [`L16`](../../../../../../raw/code/continual-harness/utils/data_persistence/backup_manager.py#L16)

