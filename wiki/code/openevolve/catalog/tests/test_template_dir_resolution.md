---
title: 'Module: tests/test_template_dir_resolution.py'
type: catalog
provenance: extracted
module: tests/test_template_dir_resolution.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_template_dir_resolution`/TestTemplateDirResolution#
symbols:
  TestTemplateDirResolution.test_relative_template_dir_resolved_to_config_location: test_relative_template_dir_resolved_to_config_location().
  TestTemplateDirResolution.test_absolute_template_dir_unchanged: test_absolute_template_dir_unchanged().
  TestTemplateDirResolution.test_null_template_dir_unchanged: test_null_template_dir_unchanged().
  TestTemplateDirResolution.test_nested_relative_template_dir: test_nested_relative_template_dir().
  TestTemplateDirResolution.test_real_example_config: test_real_example_config().
  TestTemplateDirResolution: ''
---
# Module: [`tests/test_template_dir_resolution.py`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py)

## Classes
### `TestTemplateDirResolution`  ·  implements/extends TestCase
- def: [`tests/test_template_dir_resolution.py:13`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L13)
- doc: Test that template_dir paths are resolved relative to config file location
- signature: `class TestTemplateDirResolution(unittest.TestCase):`
- members:
  - `test_absolute_template_dir_unchanged(self)` — [`L39`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L39) — Absolute paths in template_dir should remain unchanged
  - `test_nested_relative_template_dir(self)` — [`L78`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L78) — Nested relative paths should resolve correctly
  - `test_null_template_dir_unchanged(self)` — [`L59`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L59) — Null template_dir should remain None
  - `test_real_example_config(self)` — [`L100`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L100) — Test with real example config file
  - `test_relative_template_dir_resolved_to_config_location(self)` — [`L16`](../../../../../raw/code/openevolve/tests/test_template_dir_resolution.py#L16) — Relative paths in template_dir should resolve relative to config file
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`prompt`](../openevolve/config.md#Config.prompt), [`from_yaml`](../openevolve/config.md#Config.from_yaml), [`template_dir`](../openevolve/config.md#PromptConfig.template_dir)

