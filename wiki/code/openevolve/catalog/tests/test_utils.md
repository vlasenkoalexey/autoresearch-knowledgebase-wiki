---
title: 'Module: tests/test_utils.py'
type: catalog
provenance: extracted
module: tests/test_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_utils`/
symbols:
  get_integration_config: get_integration_config().
  start_test_server: start_test_server().
  is_server_running: is_server_running().
  DEFAULT_BASE_URL: DEFAULT_BASE_URL.
  TEST_MODEL: TEST_MODEL.
  DEFAULT_PORT: DEFAULT_PORT.
  setup_test_env: setup_test_env().
  get_test_client: get_test_client().
  stop_test_server: stop_test_server().
  get_evolution_test_program: get_evolution_test_program().
  get_evolution_test_evaluator: get_evolution_test_evaluator().
  find_free_port: find_free_port().
  get_simple_test_messages: get_simple_test_messages().
---
# Module: [`tests/test_utils.py`](../../../../../raw/code/openevolve/tests/test_utils.py)

## Functions
- `find_free_port(start_port: int = 8000, max_tries: int = 100)` — [`L21`](../../../../../raw/code/openevolve/tests/test_utils.py#L21) — Find a free port starting from start_port
- `get_evolution_test_evaluator()` — [`L160`](../../../../../raw/code/openevolve/tests/test_utils.py#L160) — Get a simple evaluator for evolution testing
- `get_evolution_test_program()` — [`L152`](../../../../../raw/code/openevolve/tests/test_utils.py#L152) — Get a simple program for evolution testing
- `get_integration_config(port: int = DEFAULT_PORT)` — [`L113`](../../../../../raw/code/openevolve/tests/test_utils.py#L113) — Get config for integration tests with optillm
- `get_simple_test_messages()` — [`L145`](../../../../../raw/code/openevolve/tests/test_utils.py#L145) — Get simple test messages for basic validation
- `get_test_client(base_url: str = DEFAULT_BASE_URL)` — [`L40`](../../../../../raw/code/openevolve/tests/test_utils.py#L40) — Get OpenAI client configured for local optillm
- `is_server_running(port: int = DEFAULT_PORT)` — [`L105`](../../../../../raw/code/openevolve/tests/test_utils.py#L105) — Check if optillm server is running on the given port
- `setup_test_env()` — [`L35`](../../../../../raw/code/openevolve/tests/test_utils.py#L35) — Set up test environment with local inference
- `start_test_server(model: str = TEST_MODEL, port: Optional[int] = None)` — [`L44`](../../../../../raw/code/openevolve/tests/test_utils.py#L44) — Start optillm server for testing
- `stop_test_server(proc: subprocess.Popen)` — [`L96`](../../../../../raw/code/openevolve/tests/test_utils.py#L96) — Stop the test server

## Module values
- `DEFAULT_BASE_URL` — [`L19`](../../../../../raw/code/openevolve/tests/test_utils.py#L19)
- `DEFAULT_PORT` — [`L18`](../../../../../raw/code/openevolve/tests/test_utils.py#L18)
- `TEST_MODEL` — [`L17`](../../../../../raw/code/openevolve/tests/test_utils.py#L17)

