---
title: 'Module: OpenMLE-Gym/openmle_gym/common.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/common.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.common`/
symbols:
  atomic_write_json: atomic_write_json().
  atomic_write_text: atomic_write_text().
  validate_task_name: validate_task_name().
  json_safe: json_safe().
  resolve_task_path: resolve_task_path().
  read_slugs_file: read_slugs_file().
  read_slug_entries: read_slug_entries().
  ensure_parent: ensure_parent().
  normalize_slugs: normalize_slugs().
  normalize_slug: normalize_slug().
  read_task_list: read_task_list().
  collect_task_dirs: collect_task_dirs().
  TASK_NAME_PATTERN: TASK_NAME_PATTERN.
---
# Module: [`OpenMLE-Gym/openmle_gym/common.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py)

## Functions
- `atomic_write_json(path: str | Path, value: Any)` — [`L144`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L144) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `atomic_write_text(path: str | Path, content: str, encoding: str = "utf-8")` — [`L121`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L121) — Atomically replace a text file without exposing a partial result. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- `collect_task_dirs(root: str | Path)` — [`L151`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L151)
- `ensure_parent(path: str | Path)` — [`L158`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L158) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `json_safe(value: Any)` — [`L93`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L93) — Recursively convert common scientific-Python values to strict JSON data. — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `normalize_slug(value: str)` — [`L15`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L15) — Return a Kaggle competition slug from a slug, URL, or path-like value.
- `normalize_slugs(values: Iterable[str])` — [`L30`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L30)
- `read_slug_entries(path: str | Path)` — [`L48`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L48) — Read slug inputs without deduplicating so callers can report duplicates.
- `read_slugs_file(path: str | Path)` — [`L44`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L44)
- `read_task_list(path: str | Path)` — [`L63`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L63)
- `resolve_task_path(root: str | Path, task_name: str)` — [`L81`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L81) — Resolve a task directory and enforce containment within root.
- `validate_task_name(value: str)` — [`L71`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L71) — Return a safe task identifier that cannot escape a batch directory.

## Module values
- `TASK_NAME_PATTERN` — [`L12`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/common.py#L12)

