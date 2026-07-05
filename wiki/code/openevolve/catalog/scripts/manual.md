---
title: 'Module: scripts/manual.py'
type: catalog
provenance: extracted
module: scripts/manual.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `scripts.manual`/
symbols:
  create_manual_blueprint.api_tasks: create_manual_blueprint().api_tasks().
  _list_tasks: _list_tasks().
  create_manual_blueprint.api_task_detail: create_manual_blueprint().api_task_detail().
  create_manual_blueprint.api_task_answer: create_manual_blueprint().api_task_answer().
  _queue_dir: _queue_dir().
  _write_answer: _write_answer().
  _resolve_run_root: _resolve_run_root().
  TaskItem: TaskItem#
  TaskItem.id: TaskItem#id.
  TaskItem.created_at: TaskItem#created_at.
  TaskItem.model: TaskItem#model.
  TaskItem.has_answer: TaskItem#has_answer.
  create_manual_blueprint: create_manual_blueprint().
  QUEUE_DIRNAME: QUEUE_DIRNAME.
  _read_task: _read_task().
  _normalize_newlines: _normalize_newlines().
  create_manual_blueprint.manual_page: create_manual_blueprint().manual_page().
---
# Module: [`scripts/manual.py`](../../../../../raw/code/openevolve/scripts/manual.py)

## Classes
### `TaskItem`
- def: [`scripts/manual.py:57`](../../../../../raw/code/openevolve/scripts/manual.py#L57)
- signature: `class TaskItem:`
- members:
  - `created_at` — [`L59`](../../../../../raw/code/openevolve/scripts/manual.py#L59)
  - `has_answer` — [`L61`](../../../../../raw/code/openevolve/scripts/manual.py#L61)
  - `id` — [`L58`](../../../../../raw/code/openevolve/scripts/manual.py#L58)
  - `model` — [`L60`](../../../../../raw/code/openevolve/scripts/manual.py#L60)
- used by: [`api_tasks`](manual.md#create_manual_blueprint.api_tasks), [`_list_tasks`](manual.md#_list_tasks)

## Functions
- `_list_tasks(qdir: Path)` — [`L64`](../../../../../raw/code/openevolve/scripts/manual.py#L64)
- `_normalize_newlines(text: str)` — [`L107`](../../../../../raw/code/openevolve/scripts/manual.py#L107) — Normalize CRLF/CR newlines to LF
- `_queue_dir(run_root: Path)` — [`L52`](../../../../../raw/code/openevolve/scripts/manual.py#L52)
- `_read_task(qdir: Path, task_id: str)` — [`L97`](../../../../../raw/code/openevolve/scripts/manual.py#L97)
- `_resolve_run_root(path_str: str)` — [`L26`](../../../../../raw/code/openevolve/scripts/manual.py#L26) — Resolve run root from a path that may point to:
- `_write_answer(qdir: Path, task_id: str, answer_text: str)` — [`L116`](../../../../../raw/code/openevolve/scripts/manual.py#L116)
- `api_task_answer(task_id: str)` — [`L160`](../../../../../raw/code/openevolve/scripts/manual.py#L160)
- `api_task_detail(task_id: str)` — [`L145`](../../../../../raw/code/openevolve/scripts/manual.py#L145)
- `api_tasks()` — [`L137`](../../../../../raw/code/openevolve/scripts/manual.py#L137)
- `create_manual_blueprint(get_visualizer_path: Callable[[], str])` — [`L128`](../../../../../raw/code/openevolve/scripts/manual.py#L128)
- `manual_page()` — [`L133`](../../../../../raw/code/openevolve/scripts/manual.py#L133)

## Module values
- `QUEUE_DIRNAME` — [`L23`](../../../../../raw/code/openevolve/scripts/manual.py#L23)

