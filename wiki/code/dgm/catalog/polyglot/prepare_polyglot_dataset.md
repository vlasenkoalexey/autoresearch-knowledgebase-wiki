---
title: 'Module: polyglot/prepare_polyglot_dataset.py'
type: catalog
provenance: extracted
module: polyglot/prepare_polyglot_dataset.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.prepare_polyglot_dataset`/
symbols:
  main: main().
  extract_task_metadata: extract_task_metadata().
  generate_dataset_metadata: generate_dataset_metadata().
  generate_dataset_metadata.process_task_dir: generate_dataset_metadata().process_task_dir().
  register_git: register_git().
  register_git.init_git_repo: register_git().init_git_repo().
  modify_cmake_file: modify_cmake_file().
---
# Module: [`polyglot/prepare_polyglot_dataset.py`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py)

## Functions
- `extract_task_metadata(task_dir, all_commits)` — [`L31`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L31) — Extract metadata for a single task directory
- `generate_dataset_metadata(benchmark_dir, all_commits)` — [`L111`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L111) — Generate metadata for all tasks in the benchmark directory
- `init_git_repo(practice_dir)` — [`L160`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L160)
- `main()` — [`L229`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L229)
- `modify_cmake_file(cmake_file_path, new_exercise_value)` — [`L13`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L13)
- `process_task_dir(lang_dir)` — [`L120`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L120)
- `register_git(benchmark_path)` — [`L137`](../../../../../raw/code/dgm/polyglot/prepare_polyglot_dataset.py#L137) — Initialize git repositories for each practice exercise folder if not already a git repo

