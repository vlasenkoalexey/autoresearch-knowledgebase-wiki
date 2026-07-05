---
title: 'Module: tests/test_valid_configs.py'
type: catalog
provenance: extracted
module: tests/test_valid_configs.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_valid_configs`/TestConfigValidity#
symbols:
  TestConfigValidity.test_import_config_files: test_import_config_files().
  TestConfigValidity.collect_files: collect_files().
  TestConfigValidity: ''
---
# Module: [`tests/test_valid_configs.py`](../../../../../raw/code/openevolve/tests/test_valid_configs.py)

## Classes
### `TestConfigValidity`  ·  implements/extends TestCase
- def: [`tests/test_valid_configs.py:13`](../../../../../raw/code/openevolve/tests/test_valid_configs.py#L13)
- doc: Tests that all config files in the configs/ and examples/ directories are valid
- signature: `class TestConfigValidity(unittest.TestCase):`
- members:
  - `collect_files(self)` — [`L16`](../../../../../raw/code/openevolve/tests/test_valid_configs.py#L16) — Collect all config/*config*.yaml and examples/**/*config*.yaml files
  - `test_import_config_files(self)` — [`L28`](../../../../../raw/code/openevolve/tests/test_valid_configs.py#L28) — Attempt to import all config files
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`llm`](../openevolve/config.md#Config.llm), [`models`](../openevolve/config.md#LLMConfig.models), [`load_config`](../openevolve/config.md#load_config)

