---
title: 'Module: rdagent/components/coder/model_coder/conf.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.conf`/
symbols:
  get_model_env: get_model_env().
  MODEL_COSTEER_SETTINGS: MODEL_COSTEER_SETTINGS.
  ModelCoSTEERSettings.env_type: ModelCoSTEERSettings#env_type.
  ModelCoSTEERSettings: ModelCoSTEERSettings#
  ModelCoSTEERSettings.model_config: ModelCoSTEERSettings#model_config.
---
# Module: [`rdagent/components/coder/model_coder/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py)

## Classes
### `ModelCoSTEERSettings`  ·  implements/extends CoSTEERSettings
- def: [`rdagent/components/coder/model_coder/conf.py:9`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py#L9)
- signature: `class ModelCoSTEERSettings(CoSTEERSettings):`
- members:
  - `env_type` — [`L12`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py#L12) — ---
  - `model_config` — [`L10`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py#L10)
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings)
- used by: [`execute`](model.md#ModelFBWorkspace.execute), [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`execute`](../../../scenarios/qlib/experiment/workspace.md#QlibFBWorkspace.execute), [`get_model_env`](conf.md#get_model_env), [`MODEL_COSTEER_SETTINGS`](conf.md#MODEL_COSTEER_SETTINGS)

## Functions
- `get_model_env(conf_type: Optional[str] = None, extra_volumes: dict = {}, running_timeout_period: int = 600, enable_cache: Optional[bool] = None)` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py#L16) — documented in [rdagent-utils-env](../../../../../concepts/rdagent-utils-env.md)

## Module values
- `MODEL_COSTEER_SETTINGS` — [`L38`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/conf.py#L38)

