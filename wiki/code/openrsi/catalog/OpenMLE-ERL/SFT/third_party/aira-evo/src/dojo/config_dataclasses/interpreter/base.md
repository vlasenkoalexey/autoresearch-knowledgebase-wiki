---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.interpreter.base`/InterpreterConfig#
symbols:
  InterpreterConfig: ''
  InterpreterConfig.validate: validate().
  InterpreterConfig.working_dir: working_dir.
  InterpreterConfig.timeout: timeout.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py)

## Classes
### `InterpreterConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py:15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py#L15)
- signature: `class InterpreterConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py#L28)
  - `timeout` — [`L23`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py#L23)
  - `working_dir` — [`L16`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/interpreter/base.py#L16)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`PythonInterpreterConfig`](python.md#PythonInterpreterConfig), [`validate`](python.md#PythonInterpreterConfig.validate)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`working_dir`](../../core/interpreters/python.md#PythonInterpreter.working_dir), [`timeout`](../../core/interpreters/python.md#PythonInterpreter.timeout), [`PythonInterpreterConfig`](python.md#PythonInterpreterConfig), [`interpreter`](../run.md#RunConfig.interpreter), [`interpreter`](../runner.md#RunnerConfig.interpreter), [`validate`](python.md#PythonInterpreterConfig.validate)

