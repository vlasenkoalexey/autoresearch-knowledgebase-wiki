---
title: 'Module: test/notebook/test_notebook_converter.py'
type: catalog
provenance: extracted
module: test/notebook/test_notebook_converter.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.notebook.test_notebook_converter`/
symbols:
  TestNotebookConverter.test_convert: TestNotebookConverter#test_convert().
  TestNotebookConverter.test_convert_2: TestNotebookConverter#test_convert_2().
  TestNotebookConverter.converter: TestNotebookConverter#converter.
  TestNotebookConverter.test_validation_pass: TestNotebookConverter#test_validation_pass().
  TestNotebookConverter.test_validation_missing_main_fn: TestNotebookConverter#test_validation_missing_main_fn().
  TestNotebookConverter.test_validation_missing_sections: TestNotebookConverter#test_validation_missing_sections().
  test_files_dir: test_files_dir.
  TestNotebookConverter.test_argparse_happy_path: TestNotebookConverter#test_argparse_happy_path().
  TestNotebookConverter.test_argparse_with_dupe_sys: TestNotebookConverter#test_argparse_with_dupe_sys().
  normalize_nb_json_for_comparison: normalize_nb_json_for_comparison().
  TestNotebookConverter: TestNotebookConverter#
  TestNotebookConverter.__init__: TestNotebookConverter#__init__().
---
# Module: [`test/notebook/test_notebook_converter.py`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py)

## Classes
### `TestNotebookConverter`  ·  implements/extends TestCase
- def: [`test/notebook/test_notebook_converter.py:18`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L18)
- signature: `class TestNotebookConverter(unittest.TestCase):`
- members:
  - `test_argparse_happy_path(self)` — [`L48`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L48)
  - `test_argparse_with_dupe_sys(self)` — [`L96`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L96)
  - `test_convert(self)` — [`L149`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L149)
  - `test_convert_2(self)` — [`L166`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L166)
  - `test_validation_missing_main_fn(self)` — [`L30`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L30)
  - `test_validation_missing_sections(self)` — [`L39`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L39)
  - `test_validation_pass(self)` — [`L24`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L24)
  - `converter` — [`L21`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L21)
- protocol/private: `__init__`[`L19`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L19)
- uses (calls/refs, reference-scoped): [`convert`](../../rdagent/components/coder/data_science/share/notebook.md#NotebookConverter.convert), [`validate_code_format`](../../rdagent/components/coder/data_science/share/notebook.md#NotebookConverter.validate_code_format), [`NotebookConverter`](../../rdagent/components/coder/data_science/share/notebook.md#NotebookConverter)  (2 test-only)

## Functions
- `normalize_nb_json_for_comparison(nb_json_str)` — [`L10`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L10)

## Module values
- `test_files_dir` — [`L7`](../../../../../../raw/code/rd-agent/test/notebook/test_notebook_converter.py#L7)

