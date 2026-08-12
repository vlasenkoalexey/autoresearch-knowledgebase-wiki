---
title: 'Module: src/arc3/tools.py'
type: catalog
provenance: extracted
module: src/arc3/tools.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.tools`/P
symbols:
  PythonTool.run: ythonTool#run().
  PythonTool.spec: ythonTool#spec().
  PythonArgs: ythonArgs#
  PythonTool: ythonTool#
  PythonTool.python_path: ythonTool#python_path.
  PythonArgs.timeout: ythonArgs#timeout.
  PythonTool.max_tool_chars: ythonTool#max_tool_chars.
  PYTHON_DESCRIPTION: YTHON_DESCRIPTION.
  PythonArgs.code: ythonArgs#code.
  PythonTool.workspace: ythonTool#workspace.
  PythonTool.__init__: ythonTool#__init__().
---
# Module: [`src/arc3/tools.py`](../../../../../../raw/code/Retrodict/src/arc3/tools.py)

## Classes
### `PythonArgs`
- def: [`src/arc3/tools.py:30`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L30)
- doc: Arguments for python.
- signature: `class PythonArgs(StrictArgs):`
- members:
  - `code` — [`L33`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L33)
  - `timeout` — [`L34`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L34)
- used by: [`run`](tools.md#PythonTool.run), [`containment_check`](runner.md#containment_check), [`spec`](tools.md#PythonTool.spec)

### `PythonTool`
- def: [`src/arc3/tools.py:37`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L37)
- doc: Direct argv exec of python code in the analysis interpreter.
- signature: `class PythonTool:`
- members:
  - `run(self, args: PythonArgs | dict)` — [`L51`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L51) — Run one python script in the analysis interpreter.
  - `spec(self)` — [`L47`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L47) — Return the python tool spec.
  - `max_tool_chars` — [`L45`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L45)
  - `python_path` — [`L44`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L44)
  - `workspace` — [`L41`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L41)
- protocol/private: `__init__`[`L40`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L40)
- uses (calls/refs, reference-scoped): [`PythonArgs`](tools.md#PythonArgs), [`timeout`](tools.md#PythonArgs.timeout), [`PYTHON_DESCRIPTION`](tools.md#PYTHON_DESCRIPTION), [`code`](tools.md#PythonArgs.code)
- used by: [`containment_check`](runner.md#containment_check), [`harness`](runner.md#ThinAgentClient.harness)

## Module values
- `PYTHON_DESCRIPTION` — [`L23`](../../../../../../raw/code/Retrodict/src/arc3/tools.py#L23)

