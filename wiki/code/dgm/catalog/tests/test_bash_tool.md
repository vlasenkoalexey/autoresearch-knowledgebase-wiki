---
title: 'Module: tests/test_bash_tool.py'
type: catalog
provenance: extracted
module: tests/test_bash_tool.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `tests.test_bash_tool`/
symbols:
  bash_session: bash_session().
  TestBashTool.test_simple_command: TestBashTool#test_simple_command().
  TestBashTool.test_multiple_commands: TestBashTool#test_multiple_commands().
  TestBashTool.test_command_with_error: TestBashTool#test_command_with_error().
  TestBashTool.test_environment_variables: TestBashTool#test_environment_variables().
  TestBashTool.test_command_output_processing: TestBashTool#test_command_output_processing().
  TestBashTool.test_long_running_command: TestBashTool#test_long_running_command().
  TestBashTool.test_invalid_commands: TestBashTool#test_invalid_commands().
  TestBashTool.test_command_with_special_chars: TestBashTool#test_command_with_special_chars().
  TestBashTool.test_multiple_line_output: TestBashTool#test_multiple_line_output().
  TestBashTool.test_large_output_handling: TestBashTool#test_large_output_handling().
  TestBashTool: TestBashTool#
---
# Module: [`tests/test_bash_tool.py`](../../../../../raw/code/dgm/tests/test_bash_tool.py)

## Classes
### `TestBashTool`
- def: [`tests/test_bash_tool.py:10`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L10)
- signature: `class TestBashTool:`
- members:
  - `test_command_output_processing(self)` — [`L34`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L34) — Test processing of command output.
  - `test_command_with_error(self)` — [`L23`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L23) — Test running a command that produces an error. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_command_with_special_chars(self)` — [`L59`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L59) — Test command with special characters. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_environment_variables(self)` — [`L29`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L29) — Test command with environment variables. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_invalid_commands(self, invalid_command)` — [`L54`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L54) — Test various invalid commands. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_large_output_handling(self)` — [`L73`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L73) — Test handling of large command output. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_long_running_command(self)` — [`L44`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L44) — Test behavior with a long-running command. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_multiple_commands(self)` — [`L17`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L17) — Test running multiple commands in sequence. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_multiple_line_output(self)` — [`L65`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L65) — Test handling of multiple line output. — documented in [tools-bash](../../concepts/tools-bash.md)
  - `test_simple_command(self)` — [`L11`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L11) — Test running a simple command. — documented in [tools-bash](../../concepts/tools-bash.md)
- uses (calls/refs, reference-scoped): [`tool_function`](../tools/bash.md#tool_function)

## Functions
- `bash_session()` — [`L5`](../../../../../raw/code/dgm/tests/test_bash_tool.py#L5) — Create a BashSession instance for testing.

