---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.jupyter.jupyter_client`/
symbols:
  JupyterKernelClient.execute: JupyterKernelClient#execute().
  JupyterClient._get_api_base_url: JupyterClient#_get_api_base_url().
  JupyterKernelClient._ws_app: JupyterKernelClient#_ws_app.
  log: log.
  JupyterClient._get_headers: JupyterClient#_get_headers().
  JupyterClient.interrupt_kernel: JupyterClient#interrupt_kernel().
  JupyterClient._session: JupyterClient#_session.
  JupyterClient.get_kernel_client: JupyterClient#get_kernel_client().
  JupyterKernelClient.ExecutionResult.data_items: JupyterKernelClient#ExecutionResult#data_items.
  JupyterClient._connection_info: JupyterClient#_connection_info.
  JupyterClient._get_ws_base_url: JupyterClient#_get_ws_base_url().
  JupyterClient.list_kernel_specs: JupyterClient#list_kernel_specs().
  JupyterClient.start_kernel: JupyterClient#start_kernel().
  JupyterClient.delete_kernel: JupyterClient#delete_kernel().
  JupyterClient.restart_kernel: JupyterClient#restart_kernel().
  JupyterClient.list_kernels: JupyterClient#list_kernels().
  JupyterKernelClient._time_cycle: JupyterKernelClient#_time_cycle.
  JupyterKernelClient._send_message: JupyterKernelClient#_send_message().
  JupyterKernelClient.wait_for_ready: JupyterKernelClient#wait_for_ready().
  JupyterKernelClient.ExecutionResult.is_ok: JupyterKernelClient#ExecutionResult#is_ok.
  JupyterKernelClient._thread: JupyterKernelClient#_thread.
  JupyterClient: JupyterClient#
  JupyterKernelClient.ExecutionResult: JupyterKernelClient#ExecutionResult#
  JupyterKernelClient.ExecutionResult.output: JupyterKernelClient#ExecutionResult#output.
  JupyterKernelClient.ExecutionResult.timed_out: JupyterKernelClient#ExecutionResult#timed_out.
  JupyterKernelClient: JupyterKernelClient#
  JupyterKernelClient.stop: JupyterKernelClient#stop().
  JupyterKernelClient._receive_message: JupyterKernelClient#_receive_message().
  JupyterKernelClient.ExecutionResult.DataItem.data: JupyterKernelClient#ExecutionResult#DataItem#data.
  JupyterKernelClient._on_open: JupyterKernelClient#_on_open().
  JupyterKernelClient._on_message: JupyterKernelClient#_on_message().
  JupyterKernelClient.ExecutionResult.DataItem.mime_type: JupyterKernelClient#ExecutionResult#DataItem#mime_type.
  JupyterClient.__init__: JupyterClient#__init__().
  JupyterKernelClient.__exit__: JupyterKernelClient#__exit__().
  JupyterKernelClient.ExecutionResult.DataItem: JupyterKernelClient#ExecutionResult#DataItem#
  JupyterKernelClient._message_queue: JupyterKernelClient#_message_queue.
  JupyterKernelClient._connected_event: JupyterKernelClient#_connected_event.
  JupyterKernelClient._session_id: JupyterKernelClient#_session_id.
  JupyterKernelClient._on_error: JupyterKernelClient#_on_error().
  JupyterKernelClient._on_close: JupyterKernelClient#_on_close().
  JupyterKernelClient.__init__: JupyterKernelClient#__init__().
  JupyterKernelClient.__enter__: JupyterKernelClient#__enter__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py)

## Classes
### `DataItem`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py:134`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L134)
- signature: `class DataItem:`
- members:
  - `data` — [`L136`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L136)
  - `mime_type` — [`L135`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L135)
- used by: [`execute_code`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code), [`execute`](jupyter_client.md#JupyterKernelClient.execute), [`fetch_file`](jupyter_code_executor.md#JupyterCodeExecutor.fetch_file), [`data_items`](jupyter_client.md#JupyterKernelClient.ExecutionResult.data_items)

### `ExecutionResult`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py:132`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L132)
- signature: `class ExecutionResult:`
- members:
  - `data_items` — [`L140`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L140)
  - `is_ok` — [`L138`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L138)
  - `output` — [`L139`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L139)
  - `timed_out` — [`L141`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L141)
- uses (calls/refs, reference-scoped): [`DataItem`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem)
- used by: [`execute_code`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code), [`execute`](jupyter_client.md#JupyterKernelClient.execute), [`fetch_file`](jupyter_code_executor.md#JupyterCodeExecutor.fetch_file)

### `JupyterClient`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py:51`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L51)
- signature: `class JupyterClient:`
- members:
  - `__init__(self, connection_info: JupyterConnectionInfo)` — [`L52`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L52) — (Experimental) A client for communicating with a Jupyter gateway server.
  - `delete_kernel(self, kernel_id: str)` — [`L101`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L101)
  - `get_kernel_client(self, kernel_id: str)` — [`L122`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L122)
  - `interrupt_kernel(self, kernel_id: str)` — [`L113`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L113)
  - `list_kernel_specs(self)` — [`L77`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L77)
  - `list_kernels(self)` — [`L81`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L81)
  - `restart_kernel(self, kernel_id: str)` — [`L107`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L107)
  - `start_kernel(self, kernel_spec_name: str)` — [`L85`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L85) — Start a new kernel.
- protocol/private: `_connection_info`[`L58`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L58), `_get_api_base_url`[`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L68), `_get_headers`[`L63`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L63), `_get_ws_base_url`[`L73`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L73), `_session`[`L59`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L59)
- uses (calls/refs, reference-scoped): [`log`](jupyter_client.md#log), [`JupyterConnectionInfo`](base.md#JupyterConnectionInfo), [`JupyterKernelClient`](jupyter_client.md#JupyterKernelClient), [`port`](base.md#JupyterConnectionInfo.port), [`host`](base.md#JupyterConnectionInfo.host), [`token`](base.md#JupyterConnectionInfo.token), [`use_https`](base.md#JupyterConnectionInfo.use_https)
- used by: [`execute_code`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code), [`fetch_file`](jupyter_code_executor.md#JupyterCodeExecutor.fetch_file), [`_kernel_id`](jupyter_code_executor.md#JupyterCodeExecutor._kernel_id), [`_jupyter_client`](jupyter_code_executor.md#JupyterCodeExecutor._jupyter_client), [`_jupyter_kernel_client`](jupyter_code_executor.md#JupyterCodeExecutor._jupyter_kernel_client), [`stop`](jupyter_code_executor.md#JupyterCodeExecutor.stop), [`restart`](jupyter_code_executor.md#JupyterCodeExecutor.restart), [`get_client`](apptainer_jupyter_server.md#ApptainerJupyterServer.get_client)

### `JupyterKernelClient`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py:128`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L128)
- members:
  - `execute(self, code: str, timeout_seconds: float | None = None)` — [`L236`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L236)
  - `stop(self)` — [`L186`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L186)
  - `wait_for_ready(self, timeout_seconds: float | None = None)` — [`L223`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L223)
- protocol/private: `__enter__`[`L178`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L178), `__exit__`[`L181`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L181), `__init__`[`L143`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L143), `_connected_event`[`L147`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L147), `_message_queue`[`L146`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L146), `_on_close`[`L175`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L175), `_on_error`[`L172`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L172), `_on_message`[`L169`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L169), `_on_open`[`L166`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L166), `_receive_message`[`L214`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L214), `_send_message`[`L192`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L192), `_session_id`[`L144`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L144), `_thread`[`L160`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L160), `_time_cycle`[`L163`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L163), `_ws_app`[`L151`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L151)
- uses (calls/refs, reference-scoped): [`log`](jupyter_client.md#log), [`data_items`](jupyter_client.md#JupyterKernelClient.ExecutionResult.data_items), [`is_ok`](jupyter_client.md#JupyterKernelClient.ExecutionResult.is_ok), [`ExecutionResult`](jupyter_client.md#JupyterKernelClient.ExecutionResult), [`output`](jupyter_client.md#JupyterKernelClient.ExecutionResult.output), [`timed_out`](jupyter_client.md#JupyterKernelClient.ExecutionResult.timed_out), [`data`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem.data), [`mime_type`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem.mime_type), [`DataItem`](jupyter_client.md#JupyterKernelClient.ExecutionResult.DataItem)
- used by: [`execute_code`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code), [`fetch_file`](jupyter_code_executor.md#JupyterCodeExecutor.fetch_file), [`stop`](jupyter_code_executor.md#JupyterCodeExecutor.stop), [`get_kernel_client`](jupyter_client.md#JupyterClient.get_kernel_client)

## Module values
- `log` — [`L47`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/jupyter_client.py#L47)

