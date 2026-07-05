---
title: 'Module: rdagent/components/coder/factor_coder/config.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/config.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder.config`/
symbols:
  FACTOR_COSTEER_SETTINGS: FACTOR_COSTEER_SETTINGS.
  get_factor_env: get_factor_env().
  FactorCoSTEERSettings.data_folder_debug: FactorCoSTEERSettings#data_folder_debug.
  FactorCoSTEERSettings.data_folder: FactorCoSTEERSettings#data_folder.
  FactorCoSTEERSettings: FactorCoSTEERSettings#
  FactorCoSTEERSettings.file_based_execution_timeout: FactorCoSTEERSettings#file_based_execution_timeout.
  FactorCoSTEERSettings.simple_background: FactorCoSTEERSettings#simple_background.
  FactorCoSTEERSettings.python_bin: FactorCoSTEERSettings#python_bin.
  FactorCoSTEERSettings.model_config: FactorCoSTEERSettings#model_config.
  FactorCoSTEERSettings.select_method: FactorCoSTEERSettings#select_method.
---
# Module: [`rdagent/components/coder/factor_coder/config.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py)

## Classes
### `FactorCoSTEERSettings`  ·  implements/extends CoSTEERSettings
- def: [`rdagent/components/coder/factor_coder/config.py:10`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L10)
- signature: `class FactorCoSTEERSettings(CoSTEERSettings):`
- members:
  - `data_folder` — [`L13`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L13) — ---
  - `data_folder_debug` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L16) — ---
  - `file_based_execution_timeout` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L22) — ---
  - `model_config` — [`L11`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L11)
  - `python_bin` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L28) — ---
  - `select_method` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L25) — ---
  - `simple_background` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L19) — ---
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings)
- used by: [`execute`](factor.md#FactorFBWorkspace.execute), [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`evaluate`](eva_utils.md#FactorCodeEvaluator.evaluate), [`FACTOR_COSTEER_SETTINGS`](config.md#FACTOR_COSTEER_SETTINGS), [`get_factor_env`](config.md#get_factor_env), [`get_data_folder_intro`](../../../scenarios/qlib/experiment/utils.md#get_data_folder_intro), [`generate_data_folder_from_qlib`](../../../scenarios/qlib/experiment/utils.md#generate_data_folder_from_qlib)

## Functions
- `get_factor_env(conf_type: Optional[str] = None, extra_volumes: dict = {}, running_timeout_period: int = 600, enable_cache: Optional[bool] = None)` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L32) — documented in [rdagent-utils-env](../../../../../concepts/rdagent-utils-env.md)

## Module values
- `FACTOR_COSTEER_SETTINGS` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/config.py#L49) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)

