---
title: 'Module: rdagent/components/coder/finetune/conf.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/finetune/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.finetune.conf`/
symbols:
  get_ft_env: get_ft_env().
  get_benchmark_env: get_benchmark_env().
  FT_YAML_FILE_NAME: FT_YAML_FILE_NAME.
  clear_workspace: clear_workspace().
  get_workspace_prefix: get_workspace_prefix().
  get_data_processing_env: get_data_processing_env().
  inject_data_stats: inject_data_stats().
  FT_PATHS: FT_PATHS.
  FT_DATA_SCRIPT_NAME: FT_DATA_SCRIPT_NAME.
  FTPathConfig.datasets: FTPathConfig#datasets().
  FTCoderCoSTEERSettings: FTCoderCoSTEERSettings#
  FTPathConfig.models: FTPathConfig#models().
  _get_standard_ft_volumes: _get_standard_ft_volumes().
  is_docker_env: is_docker_env().
  FTPathConfig.is_docker: FTPathConfig#is_docker().
  FT_DATA_FILE_NAME: FT_DATA_FILE_NAME.
  FTPathConfig.workspace: FTPathConfig#workspace().
  FTCoderCoSTEERSettings.env_type: FTCoderCoSTEERSettings#env_type.
  get_data_processing_cache_key: get_data_processing_cache_key().
  FT_TEST_PARAMS_FILE_NAME: FT_TEST_PARAMS_FILE_NAME.
  FT_MODEL_PATH: FT_MODEL_PATH.
  FT_DEBUG_YAML_FILE_NAME: FT_DEBUG_YAML_FILE_NAME.
  FTPathConfig.deepspeed: FTPathConfig#deepspeed().
  FT_DATASET_PATH: FT_DATASET_PATH.
  FTPathConfig: FTPathConfig#
  FT_DATA_PROC_FILE_NAME: FT_DATA_PROC_FILE_NAME.
  FTCoderCoSTEERSettings.Config: FTCoderCoSTEERSettings#Config#
  FTCoderCoSTEERSettings.Config.env_prefix: FTCoderCoSTEERSettings#Config#env_prefix.
  FTCoderCoSTEERSettings.max_seconds_multiplier: FTCoderCoSTEERSettings#max_seconds_multiplier.
  FTCoderCoSTEERSettings.extra_eval: FTCoderCoSTEERSettings#extra_eval.
---
# Module: [`rdagent/components/coder/finetune/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py)

## Classes
### `Config`
- def: [`rdagent/components/coder/finetune/conf.py:129`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L129)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L130`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L130)

### `FTCoderCoSTEERSettings`
- def: [`rdagent/components/coder/finetune/conf.py:126`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L126)
- members:
  - `env_type` — [`L135`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L135) — ---
  - `extra_eval` — [`L138`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L138) — ---
  - `max_seconds_multiplier` — [`L132`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L132) — ---
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`FTRunnerSettings`](../../../scenarios/finetune/train/runner.md#FTRunnerSettings)
- used by: [`get_ft_env`](conf.md#get_ft_env), [`get_benchmark_env`](conf.md#get_benchmark_env), [`__init__`](__init__.md#LLMFinetuneCoSTEER.__init__), [`is_docker`](conf.md#FTPathConfig.is_docker), [`FTRunnerSettings`](../../../scenarios/finetune/train/runner.md#FTRunnerSettings)

### `FTPathConfig`
- def: [`rdagent/components/coder/finetune/conf.py:70`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L70)
- doc: Centralized path configuration for FT scenario.
- signature: `class FTPathConfig:`
- members:
  - `datasets(self)` — [`L99`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L99) — Dataset directory path for raw datasets (with trailing slash). — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `deepspeed(self)` — [`L111`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L111) — DeepSpeed config directory.
  - `is_docker(self)` — [`L85`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L85) — Check if current environment is Docker-based.
  - `models(self)` — [`L92`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L92) — Model directory path (with trailing slash). — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `workspace(self)` — [`L106`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L106) — Workspace path prefix for prompts (with trailing slash).
- uses (calls/refs, reference-scoped): [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`file_path`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.file_path), [`FTCoderCoSTEERSettings`](conf.md#FTCoderCoSTEERSettings), [`env_type`](conf.md#FTCoderCoSTEERSettings.env_type), [`FT_MODEL_PATH`](conf.md#FT_MODEL_PATH), [`FT_DATASET_PATH`](conf.md#FT_DATASET_PATH)
- used by: [`implement_data`](__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`_generate_llamafactory_config_with_llm`](__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`_get_dataset_info`](__init__.md#LLMFinetuneEvolvingStrategy._get_dataset_info), [`FT_PATHS`](conf.md#FT_PATHS)

## Functions
- `_get_standard_ft_volumes()` — [`L142`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L142) — Get standard mount volume configuration for LLM finetune environments.
- `clear_workspace(workspace: FBWorkspace, env: Env)` — [`L273`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L273) — Clean the files in LLM finetune workspace.
- `get_benchmark_env(extra_volumes: dict = {}, timeout: int | None = None)` — [`L308`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L308) — OpenCompass benchmark environment construction function. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
- `get_data_processing_cache_key(local_path: str | Path)` — [`L52`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L52) — Generate cache key based only on data processing script and dataset info.
- `get_data_processing_env(enable_cache: bool | None = None, is_debug: bool = False)` — [`L231`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L231) — Get environment for data processing scripts with LLM API access.
- `get_ft_env(extra_volumes: dict = {}, operation: str = "full_training", enable_cache: bool | None = None)` — [`L168`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L168) — LLM finetune dedicated environment construction function. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
- `get_workspace_prefix(env: Env)` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L32) — Return workspace path prefix based on env type.
- `inject_data_stats(implementation: FBWorkspace, data: list, stdout: str)` — [`L368`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L368) — Compute token statistics and inject data_stats.json.
- `is_docker_env(env: Env)` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L27) — Check if the environment is Docker-based.

## Module values
- `FT_DATASET_PATH` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L49)
- `FT_DATA_FILE_NAME` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L44)
- `FT_DATA_PROC_FILE_NAME` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L41)
- `FT_DATA_SCRIPT_NAME` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L45)
- `FT_DEBUG_YAML_FILE_NAME` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L42)
- `FT_MODEL_PATH` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L48)
- `FT_PATHS` — [`L123`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L123)
- `FT_TEST_PARAMS_FILE_NAME` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L43)
- `FT_YAML_FILE_NAME` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/conf.py#L40)

