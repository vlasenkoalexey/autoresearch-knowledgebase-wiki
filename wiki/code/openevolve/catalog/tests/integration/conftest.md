---
title: 'Module: tests/integration/conftest.py'
type: catalog
provenance: extracted
module: tests/integration/conftest.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.conftest`/
symbols:
  optillm_server: optillm_server().
  evolution_config: evolution_config().
  test_program_file: test_program_file().
  test_evaluator_file: test_evaluator_file().
  temp_workspace: temp_workspace().
  evolution_output_dir: evolution_output_dir().
---
# Module: [`tests/integration/conftest.py`](../../../../../../raw/code/openevolve/tests/integration/conftest.py)

## Functions
- `evolution_config(optillm_server)` — [`L53`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L53) — Get config for evolution tests
- `evolution_output_dir(temp_workspace)` — [`L84`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L84) — Create output directory for evolution tests
- `optillm_server()` — [`L27`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L27) — Start optillm server for the test session
- `temp_workspace()` — [`L60`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L60) — Create a temporary workspace for test files
- `test_evaluator_file(temp_workspace)` — [`L76`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L76) — Create a test evaluator file
- `test_program_file(temp_workspace)` — [`L68`](../../../../../../raw/code/openevolve/tests/integration/conftest.py#L68) — Create a test program file

