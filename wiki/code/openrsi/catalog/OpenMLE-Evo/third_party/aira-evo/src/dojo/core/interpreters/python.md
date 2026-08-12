---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.python`/
symbols:
  PythonInterpreter.run: PythonInterpreter#run().
  main: main().
  PythonInterpreter.process: PythonInterpreter#process.
  PythonInterpreter.working_dir: PythonInterpreter#working_dir.
  PythonInterpreter.data_dir: PythonInterpreter#data_dir.
  PythonInterpreter.event_outq: PythonInterpreter#event_outq.
  PythonInterpreter.cleanup_session: PythonInterpreter#cleanup_session().
  PythonInterpreter.logger: PythonInterpreter#logger.
  PythonInterpreter._run_session: PythonInterpreter#_run_session().
  PythonInterpreter.timeout: PythonInterpreter#timeout.
  PythonInterpreter.result_outq: PythonInterpreter#result_outq.
  PythonInterpreter.child_proc_setup: PythonInterpreter#child_proc_setup().
  PythonInterpreter: PythonInterpreter#
  RedirectQueue.write: RedirectQueue#write().
  log: log.
  PythonInterpreter.format_tb_ipython: PythonInterpreter#format_tb_ipython.
  PythonInterpreter.__init__: PythonInterpreter#__init__().
  PythonInterpreter.code_inq: PythonInterpreter#code_inq.
  exception_summary: exception_summary().
  RedirectQueue: RedirectQueue#
  RedirectQueue.queue: RedirectQueue#queue.
  RedirectQueue.timeout: RedirectQueue#timeout.
  PythonInterpreter.create_process: PythonInterpreter#create_process().
  RedirectQueue.__init__: RedirectQueue#__init__().
  RedirectQueue.flush: RedirectQueue#flush().
  PythonInterpreter.local: PythonInterpreter#local.
  PythonInterpreter.factory: PythonInterpreter#factory.
  PythonInterpreter.fetch_file: PythonInterpreter#fetch_file().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py)

## Classes
### `PythonInterpreter`  ·  implements/extends Interpreter
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py:96`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L96)
- signature: `class PythonInterpreter(Interpreter):`
- members:
  - `__init__(self, cfg: PythonInterpreterConfig, data_dir: Path | None = None)` — [`L100`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L100) — Simulates a standalone Python REPL with an execution time limit.
  - `_run_session(self, code_inq: Queue, result_outq: Queue, event_outq: Queue)` — [`L158`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L158) — Main loop running in the child process.
  - `child_proc_setup(self, result_outq: Queue)` — [`L140`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L140) — Pre-execution setup in the child process:
  - `cleanup_session(self)` — [`L235`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L235) — Terminate the child process if it's still running, with escalation (terminate -> kill -> sigkill).
  - `create_process(self)` — [`L218`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L218) — Spawns the child process that will run Python code in an isolated environment.
  - `fetch_file(self, path: str)` — [`L260`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L260)
  - `run(self, code: str, reset_session: bool = True, persist_file: bool = False, file_name: str = "runfile.py", execute_code: bool = True, include_exec_time: bool = True)` — [`L268`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L268) — Execute the provided Python code in a separate process and return its output.
  - `code_inq` — [`L226`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L226)
  - `data_dir` — [`L121`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L121)
  - `event_outq` — [`L228`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L228)
  - `factory` — [`L98`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L98)
  - `format_tb_ipython` — [`L137`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L137)
  - `local` — [`L97`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L97)
  - `logger` — [`L113`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L113)
  - `process` — [`L138`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L138)
  - `result_outq` — [`L227`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L227)
  - `timeout` — [`L136`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L136)
  - `working_dir` — [`L114`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L114)
- uses (calls/refs, reference-scoped): [`LogEvent`](../../utils/logger.md#LogEvent), [`ExecutionResult`](base.md#ExecutionResult), [`Interpreter`](base.md#Interpreter), [`get_logger`](../../utils/logger.md#get_logger), [`exec_time`](base.md#ExecutionResult.exec_time), [`INTERPRETER`](../../utils/logger.md#LogEvent.INTERPRETER), [`exit_code`](base.md#ExecutionResult.exit_code), [`term_out`](base.md#ExecutionResult.term_out), [`copy_contents`](utils.md#copy_contents), [`eval_return`](base.md#ExecutionResult.eval_return), [`PythonInterpreterConfig`](../../config_dataclasses/interpreter/python.md#PythonInterpreterConfig), [`log`](python.md#log), [`timeout`](../../config_dataclasses/interpreter/base.md#InterpreterConfig.timeout), [`working_dir`](../../config_dataclasses/interpreter/base.md#InterpreterConfig.working_dir), [`RedirectQueue`](python.md#RedirectQueue), [`exception_summary`](python.md#exception_summary), [`format_tb_ipython`](../../config_dataclasses/interpreter/python.md#PythonInterpreterConfig.format_tb_ipython), [`use_symlinks`](../../config_dataclasses/interpreter/python.md#PythonInterpreterConfig.use_symlinks)
- used by: [`main`](python.md#main), [`Interpreter`](base.md#Interpreter), [`run`](base.md#Interpreter.run), [`_materialize`](../../config_dataclasses/interpreter/__init__.md#_LazyInterpreterMap._materialize), [`cleanup_session`](base.md#Interpreter.cleanup_session)

### `RedirectQueue`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py:79`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L79)
- doc: A file-like object that writes to a multiprocessing Queue.
- signature: `class RedirectQueue:`
- members:
  - `flush(self)` — [`L92`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L92)
  - `write(self, msg: str)` — [`L86`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L86)
  - `queue` — [`L83`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L83)
  - `timeout` — [`L84`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L84)
- protocol/private: `__init__`[`L82`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L82)
- used by: [`child_proc_setup`](python.md#PythonInterpreter.child_proc_setup)

## Functions
- `exception_summary(e: BaseException, working_dir: Path, exec_file_name: str, format_tb_ipython: bool)` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L44) — Generates a string that summarizes an exception and its stack trace.
- `main()` — [`L403`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L403)

## Module values
- `log` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/python.py#L41)

