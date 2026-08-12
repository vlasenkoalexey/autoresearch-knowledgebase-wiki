---
title: 'Module: tests/test_tools.py'
type: catalog
provenance: extracted
module: tests/test_tools.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_tools`/
symbols:
  make_tool: make_tool().
  test_runs_code_with_workspace_cwd: test_runs_code_with_workspace_cwd().
  test_numpy_is_available: test_numpy_is_available().
  test_game_engine_imports_fail_in_agent_interpreter: test_game_engine_imports_fail_in_agent_interpreter().
  test_timeout_kills_the_process: test_timeout_kills_the_process().
  test_output_is_capped: test_output_is_capped().
  test_nonzero_exit_reports_stderr: test_nonzero_exit_reports_stderr().
---
# Module: [`tests/test_tools.py`](../../../../../raw/code/Retrodict/tests/test_tools.py)

## Functions
- `make_tool(tmp_path: Path, analysis_python: Path, **kwargs)` — [`L10`](../../../../../raw/code/Retrodict/tests/test_tools.py#L10)
- `test_game_engine_imports_fail_in_agent_interpreter(tmp_path: Path, analysis_python: Path)` — [`L31`](../../../../../raw/code/Retrodict/tests/test_tools.py#L31) — The whole point of the analysis venv: arcengine/arc_agi must not be importable.
- `test_nonzero_exit_reports_stderr(tmp_path: Path, analysis_python: Path)` — [`L59`](../../../../../raw/code/Retrodict/tests/test_tools.py#L59)
- `test_numpy_is_available(tmp_path: Path, analysis_python: Path)` — [`L24`](../../../../../raw/code/Retrodict/tests/test_tools.py#L24)
- `test_output_is_capped(tmp_path: Path, analysis_python: Path)` — [`L52`](../../../../../raw/code/Retrodict/tests/test_tools.py#L52)
- `test_runs_code_with_workspace_cwd(tmp_path: Path, analysis_python: Path)` — [`L16`](../../../../../raw/code/Retrodict/tests/test_tools.py#L16)
- `test_timeout_kills_the_process(tmp_path: Path, analysis_python: Path)` — [`L41`](../../../../../raw/code/Retrodict/tests/test_tools.py#L41)

