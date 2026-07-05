---
title: 'Module: openevolve/utils/metrics_utils.py'
type: catalog
provenance: extracted
module: openevolve/utils/metrics_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.utils.metrics_utils`/
symbols:
  get_fitness_score: get_fitness_score().
  safe_numeric_average: safe_numeric_average().
  format_feature_coordinates: format_feature_coordinates().
  safe_numeric_sum: safe_numeric_sum().
---
# Module: [`openevolve/utils/metrics_utils.py`](../../../../../../raw/code/openevolve/openevolve/utils/metrics_utils.py)

## Functions
- `format_feature_coordinates(metrics: Dict[str, Any], feature_dimensions: List[str])` — [`L117`](../../../../../../raw/code/openevolve/openevolve/utils/metrics_utils.py#L117) — Format feature coordinates for display in prompts — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
- `get_fitness_score(metrics: Dict[str, Any], feature_dimensions: Optional[List[str]] = None)` — [`L69`](../../../../../../raw/code/openevolve/openevolve/utils/metrics_utils.py#L69) — Calculate fitness score, excluding MAP-Elites feature dimensions — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
- `safe_numeric_average(metrics: Dict[str, Any])` — [`L8`](../../../../../../raw/code/openevolve/openevolve/utils/metrics_utils.py#L8) — Calculate the average of numeric values in a metrics dictionary,
- `safe_numeric_sum(metrics: Dict[str, Any])` — [`L40`](../../../../../../raw/code/openevolve/openevolve/utils/metrics_utils.py#L40) — Calculate the sum of numeric values in a metrics dictionary,

