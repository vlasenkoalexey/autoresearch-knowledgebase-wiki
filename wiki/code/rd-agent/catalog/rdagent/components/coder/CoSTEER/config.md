---
title: 'Module: rdagent/components/coder/CoSTEER/config.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/CoSTEER/config.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.CoSTEER.config`/CoSTEER
symbols:
  CoSTEERSettings: Settings#
  CoSTEER_SETTINGS: _SETTINGS.
  CoSTEERSettings.coder_use_cache: Settings#coder_use_cache.
  CoSTEERSettings.max_seconds_multiplier: Settings#max_seconds_multiplier.
  CoSTEERSettings.knowledge_base_path: Settings#knowledge_base_path.
  CoSTEERSettings.new_knowledge_base_path: Settings#new_knowledge_base_path.
  CoSTEERSettings.max_loop: Settings#max_loop.
  CoSTEERSettings.fail_task_trial_limit: Settings#fail_task_trial_limit.
  CoSTEERSettings.v2_query_component_limit: Settings#v2_query_component_limit.
  CoSTEERSettings.v2_query_error_limit: Settings#v2_query_error_limit.
  CoSTEERSettings.v2_query_former_trace_limit: Settings#v2_query_former_trace_limit.
  CoSTEERSettings.v2_add_fail_attempt_to_latest_successful_execution: Settings#v2_add_fail_attempt_to_latest_successful_execution.
  CoSTEERSettings.v2_error_summary: Settings#v2_error_summary.
  CoSTEERSettings.v2_knowledge_sampler: Settings#v2_knowledge_sampler.
  CoSTEERSettings.enable_filelock: Settings#enable_filelock.
  CoSTEERSettings.filelock_path: Settings#filelock_path.
  CoSTEERSettings.Config: Settings#Config#
  CoSTEERSettings.Config.env_prefix: Settings#Config#env_prefix.
  CoSTEERSettings.v1_query_former_trace_limit: Settings#v1_query_former_trace_limit.
  CoSTEERSettings.v1_query_similar_success_limit: Settings#v1_query_similar_success_limit.
---
# Module: [`rdagent/components/coder/CoSTEER/config.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py)

## Classes
### `CoSTEERSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/components/coder/CoSTEER/config.py:6`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L6) — documented in [rdagent-core-conf](../../../../../concepts/rdagent-core-conf.md)
- doc: CoSTEER settings, this setting is supposed not to be used directly!!!
- signature: `class CoSTEERSettings(ExtendedBaseSettings):`
- members:
  - `coder_use_cache` — [`L12`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L12) — ---
  - `enable_filelock` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L36)
  - `fail_task_trial_limit` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L18)
  - `filelock_path` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L37)
  - `knowledge_base_path` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L30) — ---
  - `max_loop` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L15) — ---
  - `max_seconds_multiplier` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L39)
  - `new_knowledge_base_path` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L33) — ---
  - `v1_query_former_trace_limit` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L20)
  - `v1_query_similar_success_limit` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L21)
  - `v2_add_fail_attempt_to_latest_successful_execution` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L26)
  - `v2_error_summary` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L27)
  - `v2_knowledge_sampler` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L28)
  - `v2_query_component_limit` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L23)
  - `v2_query_error_limit` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L24)
  - `v2_query_former_trace_limit` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L25)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings), [`DSCoderCoSTEERSettings`](../data_science/conf.md#DSCoderCoSTEERSettings), [`DSRunnerCoSTEERSettings`](../../../scenarios/data_science/dev/runner/__init__.md#DSRunnerCoSTEERSettings), [`FactorCoSTEERSettings`](../factor_coder/config.md#FactorCoSTEERSettings), [`ModelCoSTEERSettings`](../model_coder/conf.md#ModelCoSTEERSettings), [`RLCoderCoSTEERSettings`](../rl/costeer.md#RLCoderCoSTEERSettings)
- used by: [`evolve_agent`](__init__.md#CoSTEER.evolve_agent), [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings), [`implement_one_task`](../factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../model_coder/evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`query`](knowledge_management.md#CoSTEERRAGStrategyV2.query), [`error_summary`](../factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.error_summary), [`__init__`](__init__.md#CoSTEER.__init__), [`former_trace_query`](knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`DSCoderCoSTEERSettings`](../data_science/conf.md#DSCoderCoSTEERSettings), [`FTCoderCoSTEERSettings`](../finetune/conf.md#FTCoderCoSTEERSettings), [`CoSTEER_SETTINGS`](config.md#CoSTEER_SETTINGS), [`__init__`](evolving_strategy.md#MultiProcessEvolvingStrategy.__init__), [`DSRunnerCoSTEERSettings`](../../../scenarios/data_science/dev/runner/__init__.md#DSRunnerCoSTEERSettings), [`get_develop_max_seconds`](../data_science/share/ds_costeer.md#DSCoSTEER.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.get_develop_max_seconds), [`__init__`](knowledge_management.md#CoSTEERRAGStrategyV1.__init__), [`__init__`](knowledge_management.md#CoSTEERRAGStrategyV2.__init__), [`__init__`](../rl/costeer.md#RLEvolvingStrategy.__init__), [`FactorCoSTEERSettings`](../factor_coder/config.md#FactorCoSTEERSettings), [`ModelCoSTEERSettings`](../model_coder/conf.md#ModelCoSTEERSettings), [`knowledge_base_path`](__init__.md#CoSTEER.knowledge_base_path), [`new_knowledge_base_path`](__init__.md#CoSTEER.new_knowledge_base_path), [`RLCoderCoSTEERSettings`](../rl/costeer.md#RLCoderCoSTEERSettings), [`max_loop`](__init__.md#CoSTEER.max_loop)

### `Config`
- def: [`rdagent/components/coder/CoSTEER/config.py:9`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L9)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L10`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L10)

## Module values
- `CoSTEER_SETTINGS` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/config.py#L42)

