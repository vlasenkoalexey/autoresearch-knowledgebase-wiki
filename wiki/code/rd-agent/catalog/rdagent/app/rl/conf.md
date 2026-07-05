---
title: 'Module: rdagent/app/rl/conf.py'
type: catalog
provenance: extracted
module: rdagent/app/rl/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.rl.conf`/RL
symbols:
  RL_RD_SETTING: _RD_SETTING.
  RLPostTrainingPropSetting.base_model: PostTrainingPropSetting#base_model.
  RLPostTrainingPropSetting.benchmark: PostTrainingPropSetting#benchmark.
  RLPostTrainingPropSetting: PostTrainingPropSetting#
  RLPostTrainingPropSetting.file_path: PostTrainingPropSetting#file_path.
  RLPostTrainingPropSetting.model_config: PostTrainingPropSetting#model_config.
  RLPostTrainingPropSetting.scen: PostTrainingPropSetting#scen.
  RLPostTrainingPropSetting.hypothesis_gen: PostTrainingPropSetting#hypothesis_gen.
  RLPostTrainingPropSetting.coder: PostTrainingPropSetting#coder.
  RLPostTrainingPropSetting.runner: PostTrainingPropSetting#runner.
  RLPostTrainingPropSetting.summarizer: PostTrainingPropSetting#summarizer.
  RLPostTrainingPropSetting.benchmark_timeout: PostTrainingPropSetting#benchmark_timeout.
---
# Module: [`rdagent/app/rl/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py)

## Classes
### `RLPostTrainingPropSetting`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/app/rl/conf.py:8`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L8)
- doc: RL Post-training dedicated property settings.
- signature: `class RLPostTrainingPropSetting(ExtendedBaseSettings):`
- members:
  - `base_model` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L29) — ---
  - `benchmark` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L32) — ---
  - `benchmark_timeout` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L36) — ---
  - `coder` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L19)
  - `file_path` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L24) — ---
  - `hypothesis_gen` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L18)
  - `model_config` — [`L14`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L14)
  - `runner` — [`L20`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L20)
  - `scen` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L17)
  - `summarizer` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L21)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings)
- used by: [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`_generate_code`](../../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`RL_RD_SETTING`](conf.md#RL_RD_SETTING), [`main`](loop.md#main), [`_gen_hypothesis_with_llm`](../../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen._gen_hypothesis_with_llm), [`benchmark`](../../scenarios/rl/scen/scenario.md#RLPostTrainingScen.benchmark), [`base_model`](../../scenarios/rl/scen/scenario.md#RLPostTrainingScen.base_model), [`RL_DATA_DIR`](../../scenarios/rl/env/conf.md#RL_DATA_DIR), [`RL_MODELS_DIR`](../../scenarios/rl/env/conf.md#RL_MODELS_DIR)

## Module values
- `RL_RD_SETTING` — [`L41`](../../../../../../../raw/code/rd-agent/rdagent/app/rl/conf.py#L41)

