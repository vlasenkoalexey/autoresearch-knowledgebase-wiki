---
title: 'Module: rdagent/components/coder/finetune/unified_validator.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/finetune/unified_validator.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.finetune.unified_validator`/
symbols:
  LLMConfigValidator._run_micro_batch_test: LLMConfigValidator#_run_micro_batch_test().
  LLMConfigValidator.validate_and_test: LLMConfigValidator#validate_and_test().
  LLMConfigValidator._get_supported_parameters: LLMConfigValidator#_get_supported_parameters().
  LLMConfigValidator._filter_parameters: LLMConfigValidator#_filter_parameters().
  LLMConfigValidator._inject_required_parameters: LLMConfigValidator#_inject_required_parameters().
  ValidationResult.success: ValidationResult#success.
  SYSTEM_MANAGED_PARAMS: SYSTEM_MANAGED_PARAMS.
  ValidationResult.execution_output: ValidationResult#execution_output.
  LLMConfigValidator: LLMConfigValidator#
  ValidationResult: ValidationResult#
  ValidationResult.filtered_config: ValidationResult#filtered_config.
  LLMConfigValidator._supported_params_cache: LLMConfigValidator#_supported_params_cache.
  ValidationResult.raw_stdout: ValidationResult#raw_stdout.
  ValidationResult.errors: ValidationResult#errors.
  LLMConfigValidator._parse_execution_log: LLMConfigValidator#_parse_execution_log().
  ValidationResult.execution_time: ValidationResult#execution_time.
  DIRNAME: DIRNAME.
  LLMConfigValidator.__init__: LLMConfigValidator#__init__().
---
# Module: [`rdagent/components/coder/finetune/unified_validator.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py)

## Classes
### `LLMConfigValidator`
- def: [`rdagent/components/coder/finetune/unified_validator.py:54`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L54)
- doc: LLM configuration validator with two-step validation:
- signature: `class LLMConfigValidator:`
- members:
  - `_filter_parameters(self, config_yaml: str)` — [`L89`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L89) — Filter configuration parameters to only include supported ones.
  - `_get_supported_parameters(self)` — [`L128`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L128) — Get supported parameters from LlamaFactory Manager
  - `_inject_required_parameters(self, config_yaml: str)` — [`L114`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L114) — Inject required parameters for multi-task environments.
  - `_parse_execution_log(self, stdout: str, exit_code: int, failed_stage: str = None)` — [`L158`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L158) — Parse execution log and extract key information for LLM evaluation.
  - `_run_micro_batch_test(self, config_yaml: str, workspace: FBWorkspace, env)` — [`L256`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L256) — Run micro-batch training test for runtime validation
  - `validate_and_test(self, config_yaml: str, workspace: FBWorkspace, env)` — [`L66`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L66) — Three-step validation: parameter filtering + injection + micro-batch testing
- protocol/private: `__init__`[`L63`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L63), `_supported_params_cache`[`L64`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L64)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`exit_code`](../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../utils/env.md#EnvResult.stdout), [`run`](../../../core/experiment.md#FBWorkspace.run), [`get_workspace_prefix`](conf.md#get_workspace_prefix), [`LLaMAFactory_manager`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactory_manager), [`remove_files`](../../../core/experiment.md#FBWorkspace.remove_files), [`get_parameters`](../../../scenarios/finetune/scen/llama_factory_manager.md#LLaMAFactoryManager.get_parameters), [`FT_TEST_PARAMS_FILE_NAME`](conf.md#FT_TEST_PARAMS_FILE_NAME), [`success`](unified_validator.md#ValidationResult.success), [`FT_DEBUG_YAML_FILE_NAME`](conf.md#FT_DEBUG_YAML_FILE_NAME), [`SYSTEM_MANAGED_PARAMS`](unified_validator.md#SYSTEM_MANAGED_PARAMS), [`execution_output`](unified_validator.md#ValidationResult.execution_output), [`ValidationResult`](unified_validator.md#ValidationResult), [`filtered_config`](unified_validator.md#ValidationResult.filtered_config), [`errors`](unified_validator.md#ValidationResult.errors), [`raw_stdout`](unified_validator.md#ValidationResult.raw_stdout), [`execution_time`](unified_validator.md#ValidationResult.execution_time)
- used by: [`evaluate`](eval.md#FTCoderEvaluator.evaluate), [`_generate_llm_feedback`](../../../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback)

### `ValidationResult`
- def: [`rdagent/components/coder/finetune/unified_validator.py:43`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L43)
- doc: Configuration validation result
- signature: `class ValidationResult:`
- members:
  - `errors` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L50)
  - `execution_output` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L48)
  - `execution_time` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L51)
  - `filtered_config` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L47)
  - `raw_stdout` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L49)
  - `success` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L46)
- used by: [`evaluate`](eval.md#FTCoderEvaluator.evaluate), [`_run_micro_batch_test`](unified_validator.md#LLMConfigValidator._run_micro_batch_test), [`validate_and_test`](unified_validator.md#LLMConfigValidator.validate_and_test)

## Module values
- `DIRNAME` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L28)
- `SYSTEM_MANAGED_PARAMS` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/unified_validator.py#L33)

