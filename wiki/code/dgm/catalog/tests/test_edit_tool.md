---
title: 'Module: tests/test_edit_tool.py'
type: catalog
provenance: extracted
module: tests/test_edit_tool.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `tests.test_edit_tool`/
symbols:
  TestEditorTool.test_view_file: TestEditorTool#test_view_file().
  TestEditorTool.test_create_file: TestEditorTool#test_create_file().
  TestEditorTool.test_create_existing_file: TestEditorTool#test_create_existing_file().
  TestEditorTool.test_edit_file: TestEditorTool#test_edit_file().
  TestEditorTool.test_edit_nonexistent_file: TestEditorTool#test_edit_nonexistent_file().
  TestEditorTool.test_view_directory: TestEditorTool#test_view_directory().
  TestEditorTool.test_invalid_path: TestEditorTool#test_invalid_path().
  TestEditorTool.test_invalid_commands: TestEditorTool#test_invalid_commands().
  temp_dir: temp_dir().
  sample_file: sample_file().
  TestEditorTool: TestEditorTool#
---
# Module: [`tests/test_edit_tool.py`](../../../../../raw/code/dgm/tests/test_edit_tool.py)

## Classes
### `TestEditorTool`
- def: [`tests/test_edit_tool.py:20`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L20)
- signature: `class TestEditorTool:`
- members:
  - `test_create_existing_file(self, sample_file)` — [`L36`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L36) — Test attempting to create an already existing file.
  - `test_create_file(self, temp_dir)` — [`L28`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L28) — Test creating a new file.
  - `test_edit_file(self, sample_file)` — [`L42`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L42) — Test editing an existing file.
  - `test_edit_nonexistent_file(self, temp_dir)` — [`L49`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L49) — Test attempting to edit a nonexistent file.
  - `test_invalid_commands(self, command, sample_file)` — [`L82`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L82) — Test various invalid commands.
  - `test_invalid_path(self)` — [`L71`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L71) — Test operations with invalid path.
  - `test_view_directory(self, temp_dir)` — [`L56`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L56) — Test viewing directory contents.
  - `test_view_file(self, sample_file)` — [`L21`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L21) — Test viewing entire file content.
- uses (calls/refs, reference-scoped): [`tool_function`](../tools/edit.md#tool_function)

## Functions
- `sample_file(temp_dir)` — [`L13`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L13) — Create a sample file with content for testing.
- `temp_dir()` — [`L7`](../../../../../raw/code/dgm/tests/test_edit_tool.py#L7) — Create a temporary directory for test files.

