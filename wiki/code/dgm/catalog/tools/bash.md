---
title: 'Module: tools/bash.py'
type: catalog
provenance: extracted
module: tools/bash.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `tools.bash`/
symbols:
  BashSession.run: BashSession#run().
  tool_function: tool_function().
  tool_function_call: tool_function_call().
  BashSession._process: BashSession#_process.
  result: result.
  BashSession._started: BashSession#_started.
  BashSession.start: BashSession#start().
  BashSession.stop: BashSession#stop().
  BashSession: BashSession#
  BashSession._timed_out: BashSession#_timed_out.
  BashSession._timeout: BashSession#_timeout.
  BashSession._sentinel: BashSession#_sentinel.
  BashSession._output_delay: BashSession#_output_delay.
  filter_error: filter_error().
  input_command: input_command.
  tool_info: tool_info().
  BashSession.__init__: BashSession#__init__().
---
# Module: [`tools/bash.py`](../../../../../raw/code/dgm/tools/bash.py)

## Classes
### `BashSession`
- def: [`tools/bash.py:27`](../../../../../raw/code/dgm/tools/bash.py#L27) — documented in [tools-bash](../../concepts/tools-bash.md)
- doc: A session of a bash shell.
- signature: `class BashSession:`
- members:
  - `run(self, command)` — [`L58`](../../../../../raw/code/dgm/tools/bash.py#L58) — documented in [tools-bash](../../concepts/tools-bash.md)
  - `start(self)` — [`L37`](../../../../../raw/code/dgm/tools/bash.py#L37) — documented in [tools-bash](../../concepts/tools-bash.md)
  - `stop(self)` — [`L50`](../../../../../raw/code/dgm/tools/bash.py#L50) — documented in [tools-bash](../../concepts/tools-bash.md)
- protocol/private: `__init__`[`L29`](../../../../../raw/code/dgm/tools/bash.py#L29), `_output_delay`[`L35`](../../../../../raw/code/dgm/tools/bash.py#L35), `_process`[`L31`](../../../../../raw/code/dgm/tools/bash.py#L31), `_sentinel`[`L34`](../../../../../raw/code/dgm/tools/bash.py#L34), `_started`[`L30`](../../../../../raw/code/dgm/tools/bash.py#L30), `_timed_out`[`L32`](../../../../../raw/code/dgm/tools/bash.py#L32), `_timeout`[`L33`](../../../../../raw/code/dgm/tools/bash.py#L33)
- used by: [`tool_function_call`](bash.md#tool_function_call)  (1 test-only)

## Functions
- `filter_error(error)` — [`L108`](../../../../../raw/code/dgm/tools/bash.py#L108) — documented in [tools-bash](../../concepts/tools-bash.md)
- `tool_function(command)` — [`L150`](../../../../../raw/code/dgm/tools/bash.py#L150) — documented in [tools-bash](../../concepts/tools-bash.md)
- `tool_function_call(command)` — [`L131`](../../../../../raw/code/dgm/tools/bash.py#L131) — Execute a command in the bash shell. — documented in [tools-bash](../../concepts/tools-bash.md)
- `tool_info()` — [`L4`](../../../../../raw/code/dgm/tools/bash.py#L4)

## Module values
- `input_command` — [`L162`](../../../../../raw/code/dgm/tools/bash.py#L162)
- `result` — [`L164`](../../../../../raw/code/dgm/tools/bash.py#L164) — documented in [tools-bash](../../concepts/tools-bash.md)

