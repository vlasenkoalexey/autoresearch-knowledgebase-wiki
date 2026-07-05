---
title: 'Module: domains/train_opt/mechanisms/soil_health.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/soil_health.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.soil_health`/
symbols:
  SoilHealthMonitor.record: SoilHealthMonitor#record().
  SoilHealthMonitor.compute_health: SoilHealthMonitor#compute_health().
  SoilHealthMonitor.get_health_text: SoilHealthMonitor#get_health_text().
  SoilHealthMonitor._recent: SoilHealthMonitor#_recent.
  SoilHealthMonitor: SoilHealthMonitor#
  SoilHealthMonitor._lookback: SoilHealthMonitor#_lookback.
  SoilHealthMonitor._total_iterations: SoilHealthMonitor#_total_iterations.
  SoilHealthMonitor._all_time_param_counts: SoilHealthMonitor#_all_time_param_counts.
  logger: logger.
  SoilHealthMonitor.__init__: SoilHealthMonitor#__init__().
---
# Module: [`domains/train_opt/mechanisms/soil_health.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py)

## Classes
### `SoilHealthMonitor`
- def: [`domains/train_opt/mechanisms/soil_health.py:31`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L31)
- doc: Tracks the holistic health of the hyperparameter search process.
- signature: `class SoilHealthMonitor:`
- members:
  - `compute_health(self, active_params: list[str])` — [`L74`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L74) — Compute the three soil health indicators.
  - `get_health_text(self, active_params: list[str])` — [`L161`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L161) — Generate a soil health dashboard for the proposal prompt.
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str, iteration: int)` — [`L57`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L57) — Record an iteration outcome for health tracking.
- protocol/private: `__init__`[`L49`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L49), `_all_time_param_counts`[`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L54), `_lookback`[`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L50), `_recent`[`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L52), `_total_iterations`[`L55`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L55)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`soil_health`](../runner.md#TrainRunner.soil_health)

## Module values
- `logger` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/soil_health.py#L28)

