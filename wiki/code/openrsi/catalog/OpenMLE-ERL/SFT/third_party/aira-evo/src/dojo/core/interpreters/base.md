---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.interpreters.base`/
symbols:
  ExecutionResult.get_empty: ExecutionResult#get_empty().
  ExecutionResult: ExecutionResult#
  ExecutionResult.term_out: ExecutionResult#term_out.
  ExecutionResult.exec_time: ExecutionResult#exec_time.
  ExecutionResult.exit_code: ExecutionResult#exit_code.
  Interpreter: Interpreter#
  Interpreter.run: Interpreter#run().
  ExecutionResult.eval_return: ExecutionResult#eval_return.
  ExecutionResult.timed_out: ExecutionResult#timed_out.
  Interpreter.cleanup_session: Interpreter#cleanup_session().
  Interpreter.__init__: Interpreter#__init__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py)

## Classes
### `ExecutionResult`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py:21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L21)
- doc: Result of executing a code snippet in the interpreter.
- signature: `class ExecutionResult(DataClassJsonMixin):`
- members:
  - `get_empty()` — [`L34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L34)
  - `eval_return` — [`L30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L30)
  - `exec_time` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L28)
  - `exit_code` — [`L29`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L29)
  - `term_out` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L27)
  - `timed_out` — [`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L31)
- used by: [`step_task`](../../tasks/mlebench/task.md#MLEBenchTask.step_task), [`run`](python.md#PythonInterpreter.run), [`absorb_exec_result`](../solvers/utils/journal.md#Node.absorb_exec_result), [`main`](python.md#main), [`run`](base.md#Interpreter.run)

### `Interpreter`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py:44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L44)
- doc: An abstract base class defining the interface for a code interpreter that:
- signature: `class Interpreter(ABC):`
- members:
  - `__init__(self, working_dir: Path | str, data_dir: Path | str = None, timeout: int = 3600)` — [`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L54) — Initializes the interpreter with a working directory, execution timeout,
  - `cleanup_session(self)` — [`L100`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L100) — Cleans up resources, such as terminating the subprocess or closing open handles.
  - `run(self, code: str, reset_session: bool = True, persist_file: bool = False, file_name: str = "runfile.py", execute_code: bool = True)` — [`L71`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/base.py#L71) — Execute the provided code in the environment managed by this interpreter.
- uses (calls/refs, reference-scoped): [`run`](python.md#PythonInterpreter.run), [`cleanup_session`](python.md#PythonInterpreter.cleanup_session), [`ExecutionResult`](base.md#ExecutionResult), [`PythonInterpreter`](python.md#PythonInterpreter)
- used by: [`evaluate_fitness`](../../tasks/mlebench/task.md#MLEBenchTask.evaluate_fitness), [`PythonInterpreter`](python.md#PythonInterpreter)

