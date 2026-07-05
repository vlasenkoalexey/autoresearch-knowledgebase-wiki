---
title: 'Module: rdagent/scenarios/rl/autorl_bench/conf.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.conf`/
symbols:
  get_workspace_dir: get_workspace_dir().
  get_models_dir: get_models_dir().
  get_data_dir: get_data_dir().
  get_baseline_cache_dir: get_baseline_cache_dir().
  AUTORL_BENCH_SETTING: AUTORL_BENCH_SETTING.
  get_instructions_file: get_instructions_file().
  get_autorl_bench_dir: get_autorl_bench_dir().
  AutoRLBenchSettings: AutoRLBenchSettings#
  AutoRLBenchSettings.file_path: AutoRLBenchSettings#file_path.
  AutoRLBenchSettings.model_config: AutoRLBenchSettings#model_config.
  AutoRLBenchSettings.rdagent_root: AutoRLBenchSettings#rdagent_root.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py)

## Classes
### `AutoRLBenchSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/scenarios/rl/autorl_bench/conf.py:14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L14)
- doc: AutoRL-Bench 配置
- signature: `class AutoRLBenchSettings(ExtendedBaseSettings):`
- members:
  - `file_path` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L23)
  - `model_config` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L21)
  - `rdagent_root` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L24)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings)
- used by: [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings), [`get_baseline_cache_dir`](conf.md#get_baseline_cache_dir), [`get_data_dir`](conf.md#get_data_dir), [`get_models_dir`](conf.md#get_models_dir), [`AUTORL_BENCH_SETTING`](conf.md#AUTORL_BENCH_SETTING)

## Functions
- `get_autorl_bench_dir()` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L30)
- `get_baseline_cache_dir()` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L50)
- `get_data_dir()` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L46)
- `get_instructions_file()` — [`L38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L38)
- `get_models_dir()` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L42)
- `get_workspace_dir()` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L34)

## Module values
- `AUTORL_BENCH_SETTING` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/conf.py#L27)

