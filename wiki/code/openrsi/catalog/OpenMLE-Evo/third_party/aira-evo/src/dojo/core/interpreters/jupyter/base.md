---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.jupyter.base`/
symbols:
  JupyterConnectionInfo: JupyterConnectionInfo#
  CodeExecutor.execute_code_blocks: CodeExecutor#execute_code_blocks().
  JupyterConnectable: JupyterConnectable#
  CodeResult: CodeResult#
  JupyterConnectable.connection_info: JupyterConnectable#connection_info().
  CodeExecutor: CodeExecutor#
  CodeExecutor.code_extractor: CodeExecutor#code_extractor().
  JupyterConnectionInfo.port: JupyterConnectionInfo#port.
  CodeBlock: CodeBlock#
  IPythonCodeResult: IPythonCodeResult#
  CodeExtractor: CodeExtractor#
  JupyterConnectionInfo.host: JupyterConnectionInfo#host.
  JupyterConnectionInfo.token: JupyterConnectionInfo#token.
  CodeExtractor.extract_code_blocks: CodeExtractor#extract_code_blocks().
  CodeExecutor.restart: CodeExecutor#restart().
  CodeExecutionConfig: CodeExecutionConfig.
  JupyterConnectionInfo.use_https: JupyterConnectionInfo#use_https.
  CodeBlock.code: CodeBlock#code.
  CodeBlock.language: CodeBlock#language.
  CodeResult.exit_code: CodeResult#exit_code.
  CodeResult.output: CodeResult#output.
  IPythonCodeResult.output_files: IPythonCodeResult#output_files.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py)

## Classes
### `CodeBlock`  ·  implements/extends BaseModel
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:22`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L22)
- doc: (Experimental) A class that represents a code block.
- signature: `class CodeBlock(BaseModel):`
- members:
  - `code` — [`L25`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L25)
  - `language` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L27)
- used by: [`execute_code_blocks`](base.md#CodeExecutor.execute_code_blocks), [`execute_code_blocks`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code_blocks), [`extract_code_blocks`](base.md#CodeExtractor.extract_code_blocks)

### `CodeExecutor`  ·  implements/extends Protocol
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L54)
- doc: (Experimental) A code executor class that executes code blocks and returns the result.
- signature: `class CodeExecutor(Protocol):`
- members:
  - `code_extractor(self)` — [`L58`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L58) — (Experimental) The code extractor used by this code executor.
  - `execute_code_blocks(self, code_blocks: list[CodeBlock])` — [`L62`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L62) — (Experimental) Execute code blocks and return the result.
  - `restart(self)` — [`L75`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L75) — (Experimental) Restart the code executor.
- uses (calls/refs, reference-scoped): [`restart`](jupyter_code_executor.md#JupyterCodeExecutor.restart), [`CodeResult`](base.md#CodeResult), [`JupyterCodeExecutor`](jupyter_code_executor.md#JupyterCodeExecutor), [`execute_code_blocks`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code_blocks), [`CodeBlock`](base.md#CodeBlock), [`CodeExtractor`](base.md#CodeExtractor), [`code_extractor`](jupyter_code_executor.md#JupyterCodeExecutor.code_extractor)
- used by: [`JupyterCodeExecutor`](jupyter_code_executor.md#JupyterCodeExecutor), [`CodeExecutionConfig`](base.md#CodeExecutionConfig)

### `CodeExtractor`  ·  implements/extends Protocol
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:38`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L38)
- doc: (Experimental) A code extractor class that extracts code blocks from a message.
- signature: `class CodeExtractor(Protocol):`
- members:
  - `extract_code_blocks(self, message: str | list[Any] | None)` — [`L41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L41) — (Experimental) Extract code blocks from a message.
- uses (calls/refs, reference-scoped): [`CodeBlock`](base.md#CodeBlock)
- used by: [`code_extractor`](base.md#CodeExecutor.code_extractor), [`code_extractor`](jupyter_code_executor.md#JupyterCodeExecutor.code_extractor)

### `CodeResult`  ·  implements/extends BaseModel
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L30)
- doc: (Experimental) A class that represents the result of a code execution.
- signature: `class CodeResult(BaseModel):`
- members:
  - `exit_code` — [`L33`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L33)
  - `output` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L35)
- uses (calls/refs, reference-scoped): [`IPythonCodeResult`](base.md#IPythonCodeResult)
- used by: [`execute_code_blocks`](base.md#CodeExecutor.execute_code_blocks), [`execute_code_blocks`](jupyter_code_executor.md#JupyterCodeExecutor.execute_code_blocks), [`IPythonCodeResult`](base.md#IPythonCodeResult)

### `IPythonCodeResult`  ·  implements/extends CodeResult
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:85`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L85)
- doc: (Experimental) A code result class for IPython code executor.
- signature: `class IPythonCodeResult(CodeResult):`
- members:
  - `output_files` — [`L88`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L88)
- uses (calls/refs, reference-scoped): [`CodeResult`](base.md#CodeResult)
- used by: [`CodeResult`](base.md#CodeResult)

### `JupyterConnectable`  ·  implements/extends Protocol
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:124`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L124)
- doc: (Experimental)
- signature: `class JupyterConnectable(Protocol):`
- members:
  - `connection_info(self)` — [`L128`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L128) — Return the connection information for this connectable.
- uses (calls/refs, reference-scoped): [`connection_info`](apptainer_jupyter_server.md#ApptainerJupyterServer.connection_info), [`JupyterConnectionInfo`](base.md#JupyterConnectionInfo), [`ApptainerJupyterServer`](apptainer_jupyter_server.md#ApptainerJupyterServer)
- used by: [`_connection_info`](jupyter_code_executor.md#JupyterCodeExecutor._connection_info), [`__init__`](jupyter_code_executor.md#JupyterCodeExecutor.__init__), [`ApptainerJupyterServer`](apptainer_jupyter_server.md#ApptainerJupyterServer)

### `JupyterConnectionInfo`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py:110`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L110)
- doc: (Experimental)
- signature: `class JupyterConnectionInfo:`
- members:
  - `host` — [`L113`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L113) — ---
  - `port` — [`L117`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L117) — ---
  - `token` — [`L119`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L119) — ---
  - `use_https` — [`L115`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L115) — ---
- used by: [`connection_info`](apptainer_jupyter_server.md#ApptainerJupyterServer.connection_info), [`_get_api_base_url`](jupyter_client.md#JupyterClient._get_api_base_url), [`_get_headers`](jupyter_client.md#JupyterClient._get_headers), [`_connection_info`](jupyter_code_executor.md#JupyterCodeExecutor._connection_info), [`_get_ws_base_url`](jupyter_client.md#JupyterClient._get_ws_base_url), [`connection_info`](base.md#JupyterConnectable.connection_info), [`__init__`](jupyter_code_executor.md#JupyterCodeExecutor.__init__), [`__init__`](jupyter_client.md#JupyterClient.__init__)

## Module values
- `CodeExecutionConfig` — [`L94`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/base.py#L94)

