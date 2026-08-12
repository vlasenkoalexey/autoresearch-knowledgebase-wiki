---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.solver.evo`/EvolutionarySolverConfig#
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
  EvolutionarySolverConfig.data_preview: data_preview.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py)

## Classes
### `EvolutionarySolverConfig`  ·  implements/extends SolverConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py:15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L15)
- signature: `class EvolutionarySolverConfig(SolverConfig):`
- members:
  - `validate(self)` — [`L62`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L62)
  - `crossover_prob` — [`L21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L21)
  - `data_preview` — [`L57`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L57)
  - `few_shot` — [`L40`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L40)
  - `final_temp` — [`L29`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L29)
  - `individuals_per_generation` — [`L47`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L47)
  - `initial_temp` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L28)
  - `max_debug_depth` — [`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L54)
  - `max_debug_time` — [`L51`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L51)
  - `max_island_size` — [`L18`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L18)
  - `migration_prob` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L24)
  - `num_generations` — [`L46`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L46)
  - `num_generations_till_crossover` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L35)
  - `num_generations_till_migration` — [`L32`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L32)
  - `num_islands` — [`L17`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/solver/evo.py#L17)
- uses (calls/refs, reference-scoped): [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate)
- used by: [`SolverConfig`](base.md#SolverConfig), [`validate`](base.md#SolverConfig.validate), [`__init__`](../../solvers/evo/evo.md#Evolutionary.__init__)

