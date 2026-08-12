---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.interpreters.python`/
symbols:
  PythonInterpreter.run: PythonInterpreter#run().
  main: main().
  PythonInterpreter.process: PythonInterpreter#process.
  PythonInterpreter.working_dir: PythonInterpreter#working_dir.
  PythonInterpreter.data_dir: PythonInterpreter#data_dir.
  PythonInterpreter.event_outq: PythonInterpreter#event_outq.
  PythonInterpreter.cleanup_session: PythonInterpreter#cleanup_session().
  PythonInterpreter.logger: PythonInterpreter#logger.
  PythonInterpreter.timeout: PythonInterpreter#timeout.
  PythonInterpreter._run_session: PythonInterpreter#_run_session().
  PythonInterpreter.result_outq: PythonInterpreter#result_outq.
  PythonInterpreter.child_proc_setup: PythonInterpreter#child_proc_setup().
  PythonInterpreter: PythonInterpreter#
  RedirectQueue.write: RedirectQueue#write().
  log: log.
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
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py)

## Classes
### `PythonInterpreter`  ·  implements/extends Interpreter
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py:86`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L86)
- signature: `class PythonInterpreter(Interpreter):`
- members:
  - `__init__(self, cfg: PythonInterpreterConfig, data_dir: Path | None = None)` — [`L90`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L90) — Simulates a standalone Python REPL with an execution time limit.
  - `_run_session(self, code_inq: Queue, result_outq: Queue, event_outq: Queue)` — [`L146`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L146) — Main loop running in the child process.
  - `child_proc_setup(self, result_outq: Queue)` — [`L128`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L128) — Pre-execution setup in the child process:
  - `cleanup_session(self)` — [`L222`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L222) — Terminate the child process if it's still running, with escalation (terminate -> kill -> sigkill).
  - `create_process(self)` — [`L205`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L205) — Spawns the child process that will run Python code in an isolated environment.
  - `fetch_file(self, path: str)` — [`L247`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L247)
  - `run(self, code: str, reset_session: bool = True, persist_file: bool = False, file_name: str = "runfile.py", execute_code: bool = True, include_exec_time: bool = True)` — [`L255`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L255) — Execute the provided Python code in a separate process and return its output.
  - `code_inq` — [`L213`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L213)
  - `data_dir` — [`L110`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L110)
  - `event_outq` — [`L215`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L215)
  - `factory` — [`L88`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L88)
  - `local` — [`L87`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L87)
  - `logger` — [`L102`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L102)
  - `process` — [`L126`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L126)
  - `result_outq` — [`L214`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L214)
  - `timeout` — [`L125`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L125)
  - `working_dir` — [`L103`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L103)
- uses (calls/refs, reference-scoped): [`LogEvent`](../../utils/logger.md#LogEvent), [`get_logger`](../../utils/logger.md#get_logger), [`ExecutionResult`](base.md#ExecutionResult), [`INTERPRETER`](../../utils/logger.md#LogEvent.INTERPRETER), [`copy_contents`](utils.md#copy_contents), [`exec_time`](base.md#ExecutionResult.exec_time), [`exit_code`](base.md#ExecutionResult.exit_code), [`term_out`](base.md#ExecutionResult.term_out), [`Interpreter`](base.md#Interpreter), [`PythonInterpreterConfig`](../../config_dataclasses/interpreter/python.md#PythonInterpreterConfig), [`log`](python.md#log), [`eval_return`](base.md#ExecutionResult.eval_return), [`RedirectQueue`](python.md#RedirectQueue), [`exception_summary`](python.md#exception_summary), [`timeout`](../../config_dataclasses/interpreter/base.md#InterpreterConfig.timeout), [`use_symlinks`](../../config_dataclasses/interpreter/python.md#PythonInterpreterConfig.use_symlinks), [`working_dir`](../../config_dataclasses/interpreter/base.md#InterpreterConfig.working_dir)
- used by: [`main`](python.md#main), [`Interpreter`](base.md#Interpreter), [`run`](base.md#Interpreter.run), [`_materialize`](../../config_dataclasses/interpreter/__init__.md#_LazyInterpreterMap._materialize), [`cleanup_session`](base.md#Interpreter.cleanup_session)

### `RedirectQueue`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py:69`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L69)
- doc: A file-like object that writes to a multiprocessing Queue.
- signature: `class RedirectQueue:`
- members:
  - `flush(self)` — [`L82`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L82)
  - `write(self, msg: str)` — [`L76`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L76)
  - `queue` — [`L73`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L73)
  - `timeout` — [`L74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L74)
- protocol/private: `__init__`[`L72`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L72)
- used by: [`child_proc_setup`](python.md#PythonInterpreter.child_proc_setup)

## Functions
- `exception_summary(e: BaseException, working_dir: Path, exec_file_name: str)` — [`L44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L44) — Generates a string that summarizes an exception and its stack trace.
- `main()` — [`L390`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L390)

## Module values
- `log` — [`L41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/python.py#L41)

