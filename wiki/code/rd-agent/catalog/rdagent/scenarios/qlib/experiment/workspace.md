---
title: 'Module: rdagent/scenarios/qlib/experiment/workspace.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/experiment/workspace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.experiment.workspace`/QlibFBWorkspace#
symbols:
  QlibFBWorkspace.execute: execute().
  QlibFBWorkspace: ''
  QlibFBWorkspace.__init__: __init__().
---
# Module: [`rdagent/scenarios/qlib/experiment/workspace.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/workspace.py)

## Classes
### `QlibFBWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/scenarios/qlib/experiment/workspace.py:13`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/workspace.py#L13)
- signature: `class QlibFBWorkspace(FBWorkspace):`
- members:
  - `execute(self, qlib_config_name: str = "conf.yaml", run_env: dict = {}, *args, **kwargs)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/workspace.py#L18)
- protocol/private: `__init__`[`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/workspace.py#L14)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`error`](../../../log/logger.md#RDAgentLog.error), [`check_output`](../../../utils/env.md#Env.check_output), [`prepare`](../../../utils/env.md#QTDockerEnv.prepare), [`QTDockerEnv`](../../../utils/env.md#QTDockerEnv), [`QlibCondaEnv`](../../../utils/env.md#QlibCondaEnv), [`QlibCondaConf`](../../../utils/env.md#QlibCondaConf), [`MODEL_COSTEER_SETTINGS`](../../../components/coder/model_coder/conf.md#MODEL_COSTEER_SETTINGS), [`env_type`](../../../components/coder/model_coder/conf.md#ModelCoSTEERSettings.env_type), [`__init__`](../../../core/experiment.md#FBWorkspace.__init__), [`inject_code_from_folder`](../../../core/experiment.md#FBWorkspace.inject_code_from_folder)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`develop`](../developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../developer/model_runner.md#QlibModelRunner.develop), [`QlibFactorExperiment`](factor_experiment.md#QlibFactorExperiment), [`execute`](../../../core/experiment.md#FBWorkspace.execute), [`QlibModelExperiment`](model_experiment.md#QlibModelExperiment), [`QlibFactorExperiment`](quant_experiment.md#QlibFactorExperiment), [`QlibModelExperiment`](quant_experiment.md#QlibModelExperiment), [`__init__`](factor_experiment.md#QlibFactorExperiment.__init__), [`__init__`](model_experiment.md#QlibModelExperiment.__init__), [`__init__`](quant_experiment.md#QlibFactorExperiment.__init__), [`__init__`](quant_experiment.md#QlibModelExperiment.__init__)

