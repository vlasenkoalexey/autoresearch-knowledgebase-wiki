---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.examples.nature_bench.build_tasks`/
symbols:
  build_tasks: build_tasks().
  _resource_line_map: _resource_line_map().
  _line_value: _line_value().
  _plain: _plain().
  _merge_resource_line_specs: _merge_resource_line_specs().
  REPO_ROOT: REPO_ROOT.
  _visible_data_analysis_for_task: _visible_data_analysis_for_task().
  _task_names_from_cfg: _task_names_from_cfg().
  _task_set_resource_map: _task_set_resource_map().
  _normalize_scm_roots: _normalize_scm_roots().
  _remote_task_records: _remote_task_records().
  main: main().
  _read_optional: _read_optional().
  _task_set_ids: _task_set_ids().
  _sanitize_task_name: _sanitize_task_name().
  _task_set_ids_from_host: _task_set_ids_from_host().
  _resolve_resource_line_task_set_path: _resolve_resource_line_task_set_path().
  _legacy_resource_line: _legacy_resource_line().
  _resource_from_metadata: _resource_from_metadata().
  _public_user_prompt: _public_user_prompt().
  _task_family_guidance: _task_family_guidance().
  OFFICIAL_RESOURCE_LINE_DEFAULTS.OFFICIAL_RESOURCE_LINE_DEFAULTS: OFFICIAL_RESOURCE_LINE_DEFAULTS.OFFICIAL_RESOURCE_LINE_DEFAULTS.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py)

## Functions
- `_legacy_resource_line(resource: str)` — [`L220`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L220)
- `_line_value(line_spec: dict[str, Any], data_cfg: Any, key: str, default: Any = None)` — [`L226`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L226)
- `_merge_resource_line_specs(data_cfg: Any)` — [`L145`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L145)
- `_normalize_scm_roots(value: Any)` — [`L250`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L250)
- `_plain(value: Any)` — [`L54`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L54)
- `_public_user_prompt()` — [`L317`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L317)
- `_read_optional(path: Path)` — [`L24`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L24)
- `_remote_task_records(data_cfg: Any, task_names: list[str])` — [`L261`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L261)
- `_resolve_resource_line_task_set_path(spec: dict[str, Any], *, naturebench_root: Path, data_cfg: Any)` — [`L158`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L158)
- `_resource_from_metadata(metadata: dict[str, Any])` — [`L237`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L237)
- `_resource_line_map(data_cfg: Any, naturebench_root: Path)` — [`L177`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L177)
- `_sanitize_task_name(task_name: str)` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L20)
- `_task_family_guidance(metadata: dict[str, Any])` — [`L330`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L330)
- `_task_names_from_cfg(data_cfg: Any, tasks_root: Path)` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L89)
- `_task_set_ids(path: Path)` — [`L108`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L108)
- `_task_set_ids_from_host(host: str, path: str)` — [`L118`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L118)
- `_task_set_resource_map(naturebench_root: Path)` — [`L207`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L207)
- `_visible_data_analysis_for_task(data_cfg: Any, task_name: str)` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L28)
- `build_tasks(config_path: Path, output_root: Path | None = None)` — [`L351`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L351)
- `main()` — [`L493`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L493)

## Module values
- `OFFICIAL_RESOURCE_LINE_DEFAULTS` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L58)
- `REPO_ROOT` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/build_tasks.py#L15)

