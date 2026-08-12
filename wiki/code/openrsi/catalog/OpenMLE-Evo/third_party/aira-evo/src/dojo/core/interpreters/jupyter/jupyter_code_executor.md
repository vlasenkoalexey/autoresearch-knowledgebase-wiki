---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.jupyter.jupyter_code_executor`/
symbols:
  JupyterCodeExecutor.execute_code: JupyterCodeExecutor#execute_code().
  JupyterCodeExecutor.fetch_file: JupyterCodeExecutor#fetch_file().
  log: log.
  JupyterCodeExecutor._kernel_id: JupyterCodeExecutor#_kernel_id.
  JupyterCodeExecutor._jupyter_client: JupyterCodeExecutor#_jupyter_client.
  JupyterCodeExecutor._jupyter_kernel_client: JupyterCodeExecutor#_jupyter_kernel_client.
  JupyterCodeExecutor.stop: JupyterCodeExecutor#stop().
  JupyterCodeExecutor.restart: JupyterCodeExecutor#restart().
  JupyterCodeExecutor._connection_info: JupyterCodeExecutor#_connection_info.
  JupyterCodeExecutor: JupyterCodeExecutor#
  JupyterCodeExecutor.__init__: JupyterCodeExecutor#__init__().
  JupyterCodeExecutor.execute_code_blocks: JupyterCodeExecutor#execute_code_blocks().
  JupyterCodeExecutor._kernel_name: JupyterCodeExecutor#_kernel_name.
  JupyterCodeExecutor.__exit__: JupyterCodeExecutor#__exit__().
  JupyterCodeExecutor.code_extractor: JupyterCodeExecutor#code_extractor().
  JupyterCodeExecutor._wait_timeout: JupyterCodeExecutor#_wait_timeout.
  JupyterCodeExecutor._timeout: JupyterCodeExecutor#_timeout.
  JupyterCodeExecutor._fetch_file_timeout: JupyterCodeExecutor#_fetch_file_timeout.
  JupyterCodeExecutor._output_dir: JupyterCodeExecutor#_output_dir.
  JupyterCodeExecutor.__enter__: JupyterCodeExecutor#__enter__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py)

## Classes
### `JupyterCodeExecutor`  ·  implements/extends CodeExecutor
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py:43`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L43)
- signature: `class JupyterCodeExecutor(CodeExecutor):`
- members:
  - `__init__(self, jupyter_server: Union[JupyterConnectable, JupyterConnectionInfo], kernel_name: str | None = None, timeout: int = 60, output_dir: Union[Path, str] = Path())` — [`L44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L44) — (Experimental) A code executor class that executes code statefully using
  - `code_extractor(self)` — [`L229`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L229) — (Experimental) The code extractor used by this code executor.
  - `execute_code(self, code: str)` — [`L99`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L99)
  - `execute_code_blocks(self, code_blocks: list[CodeBlock])` — [`L233`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L233) — (Experimental) Execute code blocks and return the result.
  - `fetch_file(self, filename: str)` — [`L153`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L153)
  - `restart(self)` — [`L200`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L200) — (Experimental) Restart a new session.
  - `stop(self)` — [`L207`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L207) — Stop the kernel.
- protocol/private: `__enter__`[`L217`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L217), `__exit__`[`L220`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L220), `_connection_info`[`L74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L74), `_fetch_file_timeout`[`L96`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L96), `_jupyter_client`[`L80`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L80), `_jupyter_kernel_client`[`L92`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L92), `_kernel_id`[`L88`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L88), `_kernel_name`[`L90`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L90), `_output_dir`[`L97`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L97), `_timeout`[`L94`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L94), `_wait_timeout`[`L95`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L95)
- uses (calls/refs, reference-scoped): [`execute`](jupyter_client.md#JupyterKernelClient.execute), [`log`](jupyter_code_executor.md#log), [`ExecutionResult`](../base.md#ExecutionResult), [`exec_time`](../base.md#ExecutionResult.exec_time), [`exit_code`](../base.md#ExecutionResult.exit_code), [`interrupt_kernel`](jupyter_client.md#JupyterClient.interrupt_kernel), [`term_out`](../base.md#ExecutionResult.term_out), [`data_items`](jupyter_client.md#JupyterKernelClient.ExecutionResult.data_items), [`get_kernel_client`](jupyter_client.md#JupyterClient.get_kernel_client), [`JupyterConnectionInfo`](base.md#JupyterConnectionInfo), [`timed_out`](../base.md#ExecutionResult.timed_out), [`delete_kernel`](jupyter_client.md#JupyterClient.delete_kernel), [`list_kernel_specs`](jupyter_client.md#JupyterClient.list_kernel_specs), [`restart_kernel`](jupyter_client.md#JupyterClient.restart_kernel), [`start_kernel`](jupyter_client.md#JupyterClient.start_kernel), [`JupyterConnectable`](base.md#JupyterConnectable), [`wait_for_ready`](jupyter_client.md#JupyterKernelClient.wait_for_ready), [`CodeResult`](base.md#CodeResult), [`connection_info`](base.md#JupyterConnectable.connection_info), [`is_ok`](jupyter_client.md#JupyterKernelClient.ExecutionResult.is_ok), [`CodeExecutor`](base.md#CodeExecutor), [`JupyterClient`](jupyter_client.md#JupyterClient), [`output`](jupyter_client.md#JupyterKernelClient.ExecutionResult.output), [`timed_out`](jupyter_client.md#JupyterKernelClient.ExecutionResult.timed_out), [`stop`](jupyter_client.md#JupyterKernelClient.stop), [`CodeBlock`](base.md#CodeBlock), [`data`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem.data), [`CodeExtractor`](base.md#CodeExtractor), [`mime_type`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem.mime_type)
- used by: [`run`](jupyter_interpreter.md#JupyterInterpreter.run), [`create_process`](jupyter_interpreter.md#JupyterInterpreter.create_process), [`fetch_file`](jupyter_interpreter.md#JupyterInterpreter.fetch_file), [`execute_code_blocks`](base.md#CodeExecutor.execute_code_blocks), [`cleanup_session`](jupyter_interpreter.md#JupyterInterpreter.cleanup_session), [`CodeExecutor`](base.md#CodeExecutor), [`code_extractor`](base.md#CodeExecutor.code_extractor), [`restart`](base.md#CodeExecutor.restart)

## Module values
- `log` — [`L40`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_code_executor.py#L40)

