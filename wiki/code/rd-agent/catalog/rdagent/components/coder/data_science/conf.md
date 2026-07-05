---
title: 'Module: rdagent/components/coder/data_science/conf.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.conf`/
symbols:
  get_ds_env: get_ds_env().
  DSCoderCoSTEERSettings: DSCoderCoSTEERSettings#
  get_clear_ws_cmd: get_clear_ws_cmd().
  DSCoderCoSTEERSettings.env_type: DSCoderCoSTEERSettings#env_type.
  DSCoderCoSTEERSettings.max_seconds_multiplier: DSCoderCoSTEERSettings#max_seconds_multiplier.
  DSCoderCoSTEERSettings.extra_evaluator: DSCoderCoSTEERSettings#extra_evaluator.
  DSCoderCoSTEERSettings.extra_eval: DSCoderCoSTEERSettings#extra_eval.
  DSCoderCoSTEERSettings.Config: DSCoderCoSTEERSettings#Config#
  DSCoderCoSTEERSettings.Config.env_prefix: DSCoderCoSTEERSettings#Config#env_prefix.
---
# Module: [`rdagent/components/coder/data_science/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py)

## Classes
### `Config`
- def: [`rdagent/components/coder/data_science/conf.py:19`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L19)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L20)

### `DSCoderCoSTEERSettings`  ·  implements/extends CoSTEERSettings
- def: [`rdagent/components/coder/data_science/conf.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L16) — documented in [rdagent-oai-llm_conf](../../../../../concepts/rdagent-oai-llm_conf.md)
- doc: Data Science CoSTEER settings
- signature: `class DSCoderCoSTEERSettings(CoSTEERSettings):`
- members:
  - `env_type` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L23)
  - `extra_eval` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L28) — ---
  - `extra_evaluator` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L25) — ---
  - `max_seconds_multiplier` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L22)
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings)
- used by: [`get_ds_env`](conf.md#get_ds_env), [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`__init__`](pipeline/__init__.md#PipelineCoSTEER.__init__), [`__init__`](ensemble/__init__.md#EnsembleCoSTEER.__init__), [`__init__`](feature/__init__.md#FeatureCoSTEER.__init__), [`__init__`](model/__init__.md#ModelCoSTEER.__init__), [`__init__`](raw_data_loader/__init__.md#DataLoaderCoSTEER.__init__), [`__init__`](workflow/__init__.md#WorkflowCoSTEER.__init__)  (1 test-only)

## Functions
- `get_clear_ws_cmd(stage: Literal["before_training", "before_inference"] = "before_training")` — [`L78`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L78) — Clean the files in workspace to a specific stage
- `get_ds_env(conf_type: Literal["kaggle", "mlebench"] = "kaggle", extra_volumes: dict = {}, running_timeout_period: int | None = DS_RD_SETTING.debug_timeout, enable_cache: bool | None = None)` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/conf.py#L41) — Retrieve the appropriate environment configuration based on the env_type setting. — documented in [rdagent-app-data_science-conf](../../../../../concepts/rdagent-app-data_science-conf.md)

