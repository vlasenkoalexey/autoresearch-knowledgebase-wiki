---
title: 'Module: rdagent/scenarios/finetune/scen/llama_factory_manager.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/scen/llama_factory_manager.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.scen.llama_factory_manager`/
symbols:
  LLaMAFactoryManager.extract_info_from_docker: LLaMAFactoryManager#extract_info_from_docker().
  LLaMAFactoryManager.cache_dir: LLaMAFactoryManager#cache_dir.
  LLaMAFactory_manager: LLaMAFactory_manager.
  LLaMAFactoryManager.get_info: LLaMAFactoryManager#get_info().
  LLaMAFactoryManager.format_shared_params: LLaMAFactoryManager#format_shared_params().
  LLaMAFactoryManager.format_method_specific_params: LLaMAFactoryManager#format_method_specific_params().
  LLaMAFactoryManager._format_params_dict: LLaMAFactoryManager#_format_params_dict().
  LLaMAFactoryManager._info_cache: LLaMAFactoryManager#_info_cache.
  LLaMAFactoryManager.methods: LLaMAFactoryManager#methods().
  LLaMAFactoryManager.get_parameters: LLaMAFactoryManager#get_parameters().
  EXCLUDED_PARAM_REGEX: EXCLUDED_PARAM_REGEX.
  LLaMAFactoryManager._load_extracted_data: LLaMAFactoryManager#_load_extracted_data().
  LLaMAFactoryManager.models: LLaMAFactoryManager#models().
  LLaMAFactoryManager.peft_methods: LLaMAFactoryManager#peft_methods().
  EXTRACT_PARAMETERS_SCRIPT_NAME: EXTRACT_PARAMETERS_SCRIPT_NAME.
  LLaMAFactoryManager.hf_models: LLaMAFactoryManager#hf_models().
  LLaMAFactoryManager.training_stages: LLaMAFactoryManager#training_stages().
  LLaMAFactoryManager.templates: LLaMAFactoryManager#templates().
  LLaMAFactoryManager.is_peft_method: LLaMAFactoryManager#is_peft_method().
  DEFAULT_HELP_TRUNCATE_LEN: DEFAULT_HELP_TRUNCATE_LEN.
  EXCLUDED_PARAM_PATTERNS: EXCLUDED_PARAM_PATTERNS.
  LLaMAFactoryManager: LLaMAFactoryManager#
  LLaMAFactoryManager._format_param_line: LLaMAFactoryManager#_format_param_line().
  LLaMAFactoryManager.__init__: LLaMAFactoryManager#__init__().
---
# Module: [`rdagent/scenarios/finetune/scen/llama_factory_manager.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py)

## Classes
### `LLaMAFactoryManager`
- def: [`rdagent/scenarios/finetune/scen/llama_factory_manager.py:99`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L99)
- doc: Manager for LLaMA Factory parameter extraction and caching.
- signature: `class LLaMAFactoryManager:`
- members:
  - `__init__(self)` — [`L102`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L102) — Initialize the manager instance.
  - `_format_param_line(self, param_name: str, param_info: dict, max_help_len: int | None)` — [`L221`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L221) — Format a single parameter line.
  - `_format_params_dict(self, params_dict: dict, max_help_len: int | None)` — [`L238`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L238) — Format a dictionary of parameters.
  - `_load_extracted_data(self)` — [`L154`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L154) — Load extracted information from flat file structure.
  - `extract_info_from_docker(self)` — [`L107`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L107) — Extract LLaMA Factory information from Docker/Conda environment. — documented in [rdagent-utils-env](../../../../../concepts/rdagent-utils-env.md)
  - `format_method_specific_params(self, method: str, max_help_len: int | None = DEFAULT_HELP_TRUNCATE_LEN)` — [`L263`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L263) — Format only method-specific finetuning parameters.
  - `format_shared_params(self, max_help_len: int | None = DEFAULT_HELP_TRUNCATE_LEN)` — [`L246`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L246) — Format shared parameters (model, data, training) that apply to all methods.
  - `get_info(self)` — [`L172`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L172) — Get complete LLaMA Factory information, extracting on first call.
  - `get_parameters(self, param_type: Optional[str] = None)` — [`L214`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L214) — Get parameters by type or all parameters.
  - `hf_models(self)` — [`L189`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L189) — Available HuggingFace models.
  - `is_peft_method(self, method: str)` — [`L210`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L210) — Check if the given method is a PEFT method.
  - `methods(self)` — [`L179`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L179) — Available fine-tuning methods.
  - `models(self)` — [`L184`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L184) — Available base models.
  - `peft_methods(self)` — [`L195`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L195) — Available PEFT methods, dynamically filtered from available methods.
  - `templates(self)` — [`L206`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L206) — Available chat templates.
  - `training_stages(self)` — [`L201`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L201) — Training stage mapping.
  - `cache_dir` — [`L104`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L104)
- protocol/private: `_info_cache`[`L105`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L105)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`conf`](../../../utils/env.md#Env.conf), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`get_ft_env`](../../../components/coder/finetune/conf.md#get_ft_env), [`exit_code`](../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../utils/env.md#EnvResult.stdout), [`run`](../../../core/experiment.md#FBWorkspace.run), [`file_path`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.file_path), [`is_docker_env`](../../../components/coder/finetune/conf.md#is_docker_env), [`EXCLUDED_PARAM_REGEX`](llama_factory_manager.md#EXCLUDED_PARAM_REGEX), [`EXTRACT_PARAMETERS_SCRIPT_NAME`](llama_factory_manager.md#EXTRACT_PARAMETERS_SCRIPT_NAME), [`DEFAULT_HELP_TRUNCATE_LEN`](llama_factory_manager.md#DEFAULT_HELP_TRUNCATE_LEN)
- used by: [`_gen_hypothesis`](../proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`_generate_llamafactory_config_with_llm`](../../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`LLaMAFactory_manager`](llama_factory_manager.md#LLaMAFactory_manager), [`_get_supported_parameters`](../../../components/coder/finetune/unified_validator.md#LLMConfigValidator._get_supported_parameters), [`_initialize_llama_factory`](scenario.md#LLMFinetuneScen._initialize_llama_factory)

## Module values
- `DEFAULT_HELP_TRUNCATE_LEN` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L23)
- `EXCLUDED_PARAM_PATTERNS` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L26)
- `EXCLUDED_PARAM_REGEX` — [`L96`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L96)
- `EXTRACT_PARAMETERS_SCRIPT_NAME` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L22)
- `LLaMAFactory_manager` — [`L287`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/llama_factory_manager.py#L287)

