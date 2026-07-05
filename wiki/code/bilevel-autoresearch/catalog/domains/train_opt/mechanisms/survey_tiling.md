---
title: 'Module: domains/train_opt/mechanisms/survey_tiling.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/survey_tiling.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.survey_tiling`/
symbols:
  SurveyTiling._rebuild_bins: SurveyTiling#_rebuild_bins().
  SurveyTiling.record: SurveyTiling#record().
  SurveyTiling.get_coverage_text: SurveyTiling#get_coverage_text().
  SurveyTiling.N_BINS: SurveyTiling#N_BINS.
  SurveyTiling._bin_counts: SurveyTiling#_bin_counts.
  SurveyTiling.get_least_covered_param: SurveyTiling#get_least_covered_param().
  SurveyTiling._observations: SurveyTiling#_observations.
  SurveyTiling: SurveyTiling#
  SurveyTiling._ranges: SurveyTiling#_ranges.
  SurveyTiling._try_numeric: SurveyTiling#_try_numeric().
  logger: logger.
  SurveyTiling.__init__: SurveyTiling#__init__().
---
# Module: [`domains/train_opt/mechanisms/survey_tiling.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py)

## Classes
### `SurveyTiling`
- def: [`domains/train_opt/mechanisms/survey_tiling.py:26`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L26)
- doc: Tracks parameter-space coverage using binned observation counts.
- signature: `class SurveyTiling:`
- members:
  - `_rebuild_bins(self)` — [`L76`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L76) — Rebuild the bin counts for all observed parameters.
  - `_try_numeric(self, val)` — [`L69`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L69) — Try to parse a value as a float. Returns None for non-numeric.
  - `get_coverage_text(self)` — [`L105`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L105) — Generate a survey coverage map for injection into the proposal prompt.
  - `get_least_covered_param(self, active_params: list[str])` — [`L170`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L170) — Return the active param with the lowest coverage fraction.
  - `record(self, changes: dict, old_config: dict)` — [`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L44) — Record a parameter observation (regardless of keep/discard/crash).
  - `N_BINS` — [`L34`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L34)
- protocol/private: `__init__`[`L36`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L36), `_bin_counts`[`L42`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L42), `_observations`[`L38`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L38), `_ranges`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L40)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`survey_tiling`](../runner.md#TrainRunner.survey_tiling)

## Module values
- `logger` — [`L23`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/survey_tiling.py#L23)

