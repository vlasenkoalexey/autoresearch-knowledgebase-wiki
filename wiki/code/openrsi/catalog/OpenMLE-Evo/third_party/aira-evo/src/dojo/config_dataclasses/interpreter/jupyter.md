---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.interpreter.jupyter`/JupyterInterpreterConfig#
symbols:
  JupyterInterpreterConfig: ''
  JupyterInterpreterConfig.superimage_directory: superimage_directory.
  JupyterInterpreterConfig.superimage_version: superimage_version.
  JupyterInterpreterConfig.validate: validate().
  JupyterInterpreterConfig.strip_ansi: strip_ansi.
  JupyterInterpreterConfig.read_only_overlays: read_only_overlays.
  JupyterInterpreterConfig.read_only_binds: read_only_binds.
  JupyterInterpreterConfig.env: env.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py)

## Classes
### `JupyterInterpreterConfig`  ·  implements/extends InterpreterConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py:16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L16)
- signature: `class JupyterInterpreterConfig(InterpreterConfig):`
- members:
  - `validate(self)` — [`L48`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L48)
  - `env` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L41)
  - `read_only_binds` — [`L35`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L35)
  - `read_only_overlays` — [`L31`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L31)
  - `strip_ansi` — [`L27`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L27)
  - `superimage_directory` — [`L17`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L17)
  - `superimage_version` — [`L23`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/jupyter.py#L23)
- uses (calls/refs, reference-scoped): [`InterpreterConfig`](base.md#InterpreterConfig), [`validate`](base.md#InterpreterConfig.validate), [`get_superimage_dir`](../../utils/environment.md#get_superimage_dir)
- used by: [`execute_code`](../../grade_code.md#execute_code), [`InterpreterConfig`](base.md#InterpreterConfig), [`validate`](base.md#InterpreterConfig.validate), [`env`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.env), [`read_only_binds`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.read_only_binds), [`read_only_overlays`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.read_only_overlays), [`strip_ansi`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.strip_ansi), [`superimage_directory`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.superimage_directory), [`superimage_version`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.superimage_version), [`__init__`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreter.__init__), [`__init__`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.__init__), [`env`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.env), [`read_only_binds`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.read_only_binds), [`read_only_overlays`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.read_only_overlays), [`strip_ansi`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.strip_ansi), [`suerimage_directory`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.suerimage_directory), [`superimage_version`](../../core/interpreters/jupyter/jupyter_interpreter.md#JupyterInterpreterFactory.superimage_version)

