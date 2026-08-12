---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.interpreters.jupyter.apptainer_jupyter_server`/
symbols:
  ApptainerJupyterServer.connection_info: ApptainerJupyterServer#connection_info().
  ApptainerJupyterServer._subprocess: ApptainerJupyterServer#_subprocess.
  log: log.
  ApptainerJupyterServer.superimage_version: ApptainerJupyterServer#superimage_version.
  ApptainerJupyterServer.stop: ApptainerJupyterServer#stop().
  ApptainerJupyterServer.port: ApptainerJupyterServer#port.
  ApptainerJupyterServer.read_only_overlays: ApptainerJupyterServer#read_only_overlays.
  ApptainerJupyterServer.read_only_binds: ApptainerJupyterServer#read_only_binds.
  ApptainerJupyterServer.get_client: ApptainerJupyterServer#get_client().
  ApptainerJupyterServer: ApptainerJupyterServer#
  ApptainerJupyterServer.__exit__: ApptainerJupyterServer#__exit__().
  ApptainerJupyterServer.__del__: ApptainerJupyterServer#__del__().
  ApptainerJupyterServer.env: ApptainerJupyterServer#env.
  ApptainerJupyterServer.token: ApptainerJupyterServer#token.
  ApptainerJupyterServer.ip: ApptainerJupyterServer#ip.
  ApptainerJupyterServer.__init__: ApptainerJupyterServer#__init__().
  ApptainerJupyterServer.bind_inputs_dir: ApptainerJupyterServer#bind_inputs_dir.
  ApptainerJupyterServer.path_to_superimage: ApptainerJupyterServer#path_to_superimage.
  ApptainerJupyterServer.__enter__: ApptainerJupyterServer#__enter__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py)

## Classes
### `ApptainerJupyterServer`  ·  implements/extends JupyterConnectable
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py:34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L34)
- signature: `class ApptainerJupyterServer(JupyterConnectable):`
- members:
  - `connection_info(self)` — [`L163`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L163)
  - `get_client(self)` — [`L171`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L171)
  - `stop(self)` — [`L141`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L141)
  - `bind_inputs_dir` — [`L59`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L59)
  - `env` — [`L51`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L51)
  - `ip` — [`L131`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L131)
  - `path_to_superimage` — [`L60`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L60)
  - `port` — [`L132`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L132)
  - `read_only_binds` — [`L48`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L48)
  - `read_only_overlays` — [`L45`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L45)
  - `superimage_version` — [`L61`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L61)
  - `token` — [`L58`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L58)
- protocol/private: `__del__`[`L182`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L182), `__enter__`[`L174`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L174), `__exit__`[`L177`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L177), `__init__`[`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L35), `_subprocess`[`L102`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L102)
- uses (calls/refs, reference-scoped): [`log`](apptainer_jupyter_server.md#log), [`JupyterConnectionInfo`](base.md#JupyterConnectionInfo), [`JupyterConnectable`](base.md#JupyterConnectable), [`JupyterClient`](jupyter_client.md#JupyterClient), [`port`](base.md#JupyterConnectionInfo.port), [`host`](base.md#JupyterConnectionInfo.host), [`token`](base.md#JupyterConnectionInfo.token), [`use_https`](base.md#JupyterConnectionInfo.use_https)
- used by: [`jupyter_server`](jupyter_interpreter.md#JupyterInterpreter.jupyter_server), [`close`](jupyter_interpreter.md#JupyterInterpreter.close), [`JupyterConnectable`](base.md#JupyterConnectable), [`connection_info`](base.md#JupyterConnectable.connection_info)

## Module values
- `log` — [`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/interpreters/jupyter/apptainer_jupyter_server.py#L31)

