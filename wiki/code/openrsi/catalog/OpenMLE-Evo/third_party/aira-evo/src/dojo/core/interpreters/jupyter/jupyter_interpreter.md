---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.jupyter.jupyter_interpreter`/
symbols:
  JupyterInterpreter.run: JupyterInterpreter#run().
  JupyterInterpreter.jupyter_server: JupyterInterpreter#jupyter_server.
  JupyterInterpreter.create_process: JupyterInterpreter#create_process().
  JupyterInterpreter.fetch_file: JupyterInterpreter#fetch_file().
  JupyterInterpreterFactory.instance: JupyterInterpreterFactory#instance().
  JupyterInterpreter.code_executor: JupyterInterpreter#code_executor.
  JupyterInterpreterFactory.run: JupyterInterpreterFactory#run().
  JupyterInterpreter.env: JupyterInterpreter#env.
  JupyterInterpreter.close: JupyterInterpreter#close().
  JupyterInterpreter.data_dir: JupyterInterpreter#data_dir.
  JupyterInterpreterFactory.data_dir: JupyterInterpreterFactory#data_dir.
  JupyterInterpreterFactory.reset_session: JupyterInterpreterFactory#reset_session().
  JupyterInterpreter.working_dir: JupyterInterpreter#working_dir.
  log: log.
  JupyterInterpreter.cleanup_session: JupyterInterpreter#cleanup_session().
  JupyterInterpreter.timeout: JupyterInterpreter#timeout.
  JupyterInterpreterFactory: JupyterInterpreterFactory#
  JupyterInterpreterFactory._instance: JupyterInterpreterFactory#_instance.
  JupyterInterpreterFactory.fetch_file: JupyterInterpreterFactory#fetch_file().
  JupyterInterpreter: JupyterInterpreter#
  JupyterInterpreter.strip_ansi: JupyterInterpreter#strip_ansi.
  JupyterInterpreter.superimage_directory: JupyterInterpreter#superimage_directory.
  JupyterInterpreter.superimage_version: JupyterInterpreter#superimage_version.
  JupyterInterpreter.read_only_overlays: JupyterInterpreter#read_only_overlays.
  JupyterInterpreter.read_only_binds: JupyterInterpreter#read_only_binds.
  JupyterInterpreter.cleanup_line: JupyterInterpreter#cleanup_line().
  JupyterInterpreterFactory.working_dir: JupyterInterpreterFactory#working_dir.
  JupyterInterpreter.__init__: JupyterInterpreter#__init__().
  JupyterInterpreterFactory.__init__: JupyterInterpreterFactory#__init__().
  JupyterInterpreterFactory.timeout: JupyterInterpreterFactory#timeout.
  JupyterInterpreterFactory.strip_ansi: JupyterInterpreterFactory#strip_ansi.
  JupyterInterpreterFactory.suerimage_directory: JupyterInterpreterFactory#suerimage_directory.
  JupyterInterpreterFactory.superimage_version: JupyterInterpreterFactory#superimage_version.
  JupyterInterpreterFactory.read_only_overlays: JupyterInterpreterFactory#read_only_overlays.
  JupyterInterpreterFactory.read_only_binds: JupyterInterpreterFactory#read_only_binds.
  JupyterInterpreterFactory.env: JupyterInterpreterFactory#env.
  JupyterInterpreterFactory.cleanup_session: JupyterInterpreterFactory#cleanup_session().
  JupyterInterpreterFactory.close: JupyterInterpreterFactory#close().
  JupyterInterpreterFactory.cfg: JupyterInterpreterFactory#cfg.
  JupyterInterpreter.local: JupyterInterpreter#local.
  JupyterInterpreter.factory: JupyterInterpreter#factory.
  JupyterInterpreterFactory.local: JupyterInterpreterFactory#local.
  JupyterInterpreterFactory.factory: JupyterInterpreterFactory#factory.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py)

## Classes
### `JupyterInterpreter`  ·  implements/extends Interpreter
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py:23`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L23)
- signature: `class JupyterInterpreter(Interpreter):`
- members:
  - `cleanup_line(self, line: str)` — [`L93`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L93)
  - `cleanup_session(self)` — [`L139`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L139)
  - `close(self)` — [`L146`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L146)
  - `create_process(self)` — [`L64`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L64)
  - `fetch_file(self, path: str)` — [`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L68)
  - `run(self, code: str, reset_session: bool = True, persist_file: bool = False, file_name: str = "runfile.py", execute_code: bool = True, include_exec_time: bool = True)` — [`L98`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L98)
  - `code_executor` — [`L62`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L62)
  - `data_dir` — [`L48`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L48)
  - `env` — [`L40`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L40)
  - `factory` — [`L25`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L25)
  - `jupyter_server` — [`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L54)
  - `local` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L24)
  - `read_only_binds` — [`L39`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L39)
  - `read_only_overlays` — [`L38`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L38)
  - `strip_ansi` — [`L33`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L33)
  - `superimage_directory` — [`L36`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L36)
  - `superimage_version` — [`L37`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L37)
  - `timeout` — [`L32`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L32)
  - `working_dir` — [`L34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L34)
- protocol/private: `__init__`[`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L27)
- uses (calls/refs, reference-scoped): [`execute_code`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code), [`fetch_file`](jupyter_code_executor.md#JupyterCodeExecutor.fetch_file), [`ExecutionResult`](../base.md#ExecutionResult), [`stop`](jupyter_code_executor.md#JupyterCodeExecutor.stop), [`Interpreter`](../base.md#Interpreter), [`exec_time`](../base.md#ExecutionResult.exec_time), [`exit_code`](../base.md#ExecutionResult.exit_code), [`term_out`](../base.md#ExecutionResult.term_out), [`stop`](apptainer_jupyter_server.md#ApptainerJupyterServer.stop), [`timed_out`](../base.md#ExecutionResult.timed_out), [`JupyterInterpreterConfig`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig), [`log`](jupyter_interpreter.md#log), [`JupyterCodeExecutor`](jupyter_code_executor.md#JupyterCodeExecutor), [`eval_return`](../base.md#ExecutionResult.eval_return), [`ApptainerJupyterServer`](apptainer_jupyter_server.md#ApptainerJupyterServer), [`superimage_directory`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.superimage_directory), [`timeout`](../../../config_dataclasses/interpreter/base.md#InterpreterConfig.timeout), [`working_dir`](../../../config_dataclasses/interpreter/base.md#InterpreterConfig.working_dir), [`superimage_version`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.superimage_version), [`env`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.env), [`read_only_binds`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.read_only_binds), [`read_only_overlays`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.read_only_overlays), [`strip_ansi`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.strip_ansi)
- used by: [`Interpreter`](../base.md#Interpreter), [`instance`](jupyter_interpreter.md#JupyterInterpreterFactory.instance), [`run`](../base.md#Interpreter.run), [`run`](jupyter_interpreter.md#JupyterInterpreterFactory.run), [`reset_session`](jupyter_interpreter.md#JupyterInterpreterFactory.reset_session), [`cleanup_session`](../base.md#Interpreter.cleanup_session), [`fetch_file`](jupyter_interpreter.md#JupyterInterpreterFactory.fetch_file)

### `JupyterInterpreterFactory`  ·  implements/extends Interpreter
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py:151`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L151)
- signature: `class JupyterInterpreterFactory(Interpreter):`
- members:
  - `cleanup_session(self)` — [`L220`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L220)
  - `close(self)` — [`L223`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L223)
  - `fetch_file(self, path: str)` — [`L193`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L193)
  - `instance(self)` — [`L188`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L188)
  - `reset_session(self)` — [`L180`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L180)
  - `run(self, code: str, reset_session: bool = True, persist_file: bool = False, file_name: str = "runfile.py", execute_code: bool = True, include_exec_time: bool = True)` — [`L199`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L199)
  - `cfg` — [`L160`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L160)
  - `data_dir` — [`L165`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L165)
  - `env` — [`L176`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L176)
  - `factory` — [`L153`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L153)
  - `local` — [`L152`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L152)
  - `read_only_binds` — [`L175`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L175)
  - `read_only_overlays` — [`L174`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L174)
  - `strip_ansi` — [`L171`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L171)
  - `suerimage_directory` — [`L172`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L172)
  - `superimage_version` — [`L173`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L173)
  - `timeout` — [`L170`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L170)
  - `working_dir` — [`L162`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L162)
- protocol/private: `__init__`[`L155`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L155), `_instance`[`L178`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L178)
- uses (calls/refs, reference-scoped): [`run`](jupyter_interpreter.md#JupyterInterpreter.run), [`ExecutionResult`](../base.md#ExecutionResult), [`Interpreter`](../base.md#Interpreter), [`fetch_file`](jupyter_interpreter.md#JupyterInterpreter.fetch_file), [`close`](jupyter_interpreter.md#JupyterInterpreter.close), [`JupyterInterpreterConfig`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig), [`JupyterInterpreter`](jupyter_interpreter.md#JupyterInterpreter), [`superimage_directory`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.superimage_directory), [`timeout`](../../../config_dataclasses/interpreter/base.md#InterpreterConfig.timeout), [`working_dir`](../../../config_dataclasses/interpreter/base.md#InterpreterConfig.working_dir), [`superimage_version`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.superimage_version), [`env`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.env), [`read_only_binds`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.read_only_binds), [`read_only_overlays`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.read_only_overlays), [`strip_ansi`](../../../config_dataclasses/interpreter/jupyter.md#JupyterInterpreterConfig.strip_ansi)
- used by: [`Interpreter`](../base.md#Interpreter), [`run`](../base.md#Interpreter.run), [`_materialize`](../../../config_dataclasses/interpreter/__init__.md#_LazyInterpreterMap._materialize), [`cleanup_session`](../base.md#Interpreter.cleanup_session)

## Module values
- `log` — [`L20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_interpreter.py#L20)

