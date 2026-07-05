---
title: 'Module: rdagent/scenarios/rl/autorl_bench/core/metrics.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/core/metrics.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.core.metrics`/
symbols:
  run_workspace_metrics: run_workspace_metrics().
  compute_metrics: compute_metrics().
  _parse_iso_time: _parse_iso_time().
  _safe_div: _safe_div().
  write_metrics_json: write_metrics_json().
  plot_score_trajectory: plot_score_trajectory().
---
# Module: [`rdagent/scenarios/rl/autorl_bench/core/metrics.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py)

## Functions
- `_parse_iso_time(value: str)` — [`L15`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L15)
- `_safe_div(numerator: float, denominator: float)` — [`L22`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L22)
- `compute_metrics(workspace: Path, baseline: Optional[float], base_model_path: Optional[str])` — [`L28`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L28)
- `plot_score_trajectory(workspace: Path, metrics: dict[str, Any])` — [`L118`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L118)
- `run_workspace_metrics(workspace: Path, baseline: Optional[float], base_model_path: Optional[str], *, plot: bool = True)` — [`L145`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L145)
- `write_metrics_json(workspace: Path, metrics: dict[str, Any])` — [`L110`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/metrics.py#L110)

