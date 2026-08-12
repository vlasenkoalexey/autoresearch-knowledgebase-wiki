---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.solver.evo`/EvolutionarySolverConfig#
symbols:
  EvolutionarySolverConfig: ''
  EvolutionarySolverConfig.validate: validate().
  EvolutionarySolverConfig.num_islands: num_islands.
  EvolutionarySolverConfig.max_island_size: max_island_size.
  EvolutionarySolverConfig.crossover_prob: crossover_prob.
  EvolutionarySolverConfig.migration_prob: migration_prob.
  EvolutionarySolverConfig.initial_temp: initial_temp.
  EvolutionarySolverConfig.final_temp: final_temp.
  EvolutionarySolverConfig.num_generations_till_migration: num_generations_till_migration.
  EvolutionarySolverConfig.num_generations_till_crossover: num_generations_till_crossover.
  EvolutionarySolverConfig.few_shot: few_shot.
  EvolutionarySolverConfig.num_generations: num_generations.
  EvolutionarySolverConfig.individuals_per_generation: individuals_per_generation.
  EvolutionarySolverConfig.max_debug_time: max_debug_time.
  EvolutionarySolverConfig.max_debug_depth: max_debug_depth.
  EvolutionarySolverConfig.fresh_draft_prob: fresh_draft_prob.
  EvolutionarySolverConfig.max_wall_time_secs: max_wall_time_secs.
  EvolutionarySolverConfig.data_preview: data_preview.
  EvolutionarySolverConfig.experience: experience.
  EvolutionarySolverConfig.execution_mode: execution_mode.
  EvolutionarySolverConfig.async_workers: async_workers.
  EvolutionarySolverConfig.async_sandbox_urls: async_sandbox_urls.
  EvolutionarySolverConfig.async_sandbox_assignment: async_sandbox_assignment.
  EvolutionarySolverConfig.async_checkpoint_every_commits: async_checkpoint_every_commits.
  EvolutionarySolverConfig.async_worker_max_retries: async_worker_max_retries.
  EvolutionarySolverConfig.async_worker_retry_backoff_secs: async_worker_retry_backoff_secs.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py)

## Classes
### `EvolutionarySolverConfig`  ·  implements/extends SolverConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py:18`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L18)
- signature: `class EvolutionarySolverConfig(SolverConfig):`
- members:
  - `validate(self)` — [`L113`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L113)
  - `async_checkpoint_every_commits` — [`L96`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L96)
  - `async_sandbox_assignment` — [`L92`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L92)
  - `async_sandbox_urls` — [`L88`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L88)
  - `async_worker_max_retries` — [`L100`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L100)
  - `async_worker_retry_backoff_secs` — [`L106`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L106)
  - `async_workers` — [`L84`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L84)
  - `crossover_prob` — [`L24`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L24)
  - `data_preview` — [`L72`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L72)
  - `execution_mode` — [`L80`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L80)
  - `experience` — [`L76`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L76)
  - `few_shot` — [`L43`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L43)
  - `final_temp` — [`L32`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L32)
  - `fresh_draft_prob` — [`L58`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L58)
  - `individuals_per_generation` — [`L50`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L50)
  - `initial_temp` — [`L31`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L31)
  - `max_debug_depth` — [`L57`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L57)
  - `max_debug_time` — [`L54`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L54)
  - `max_island_size` — [`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L21)
  - `max_wall_time_secs` — [`L64`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L64)
  - `migration_prob` — [`L27`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L27)
  - `num_generations` — [`L49`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L49)
  - `num_generations_till_crossover` — [`L38`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L38)
  - `num_generations_till_migration` — [`L35`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L35)
  - `num_islands` — [`L20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L20)
- uses (calls/refs, reference-scoped): [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate)
- used by: [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate), [`__init__`](../../solvers/evo/evo.md#Evolutionary.__init__)

