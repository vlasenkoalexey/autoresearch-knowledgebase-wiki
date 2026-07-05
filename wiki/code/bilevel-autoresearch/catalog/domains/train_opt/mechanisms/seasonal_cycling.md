---
title: 'Module: domains/train_opt/mechanisms/seasonal_cycling.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/seasonal_cycling.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.seasonal_cycling`/
symbols:
  SeasonalCycling.get_season_text: SeasonalCycling#get_season_text().
  SeasonalCycling.advance: SeasonalCycling#advance().
  SeasonalCycling.current_season: SeasonalCycling#current_season().
  SeasonalCycling.record_harvest: SeasonalCycling#record_harvest().
  SEASON_ORDER: SEASON_ORDER.
  SEASONS: SEASONS.
  SeasonalCycling.season_info: SeasonalCycling#season_info().
  SeasonalCycling._season_harvests: SeasonalCycling#_season_harvests.
  SeasonalCycling._season_attempts: SeasonalCycling#_season_attempts.
  SeasonalCycling._iteration_in_season: SeasonalCycling#_iteration_in_season.
  SeasonalCycling: SeasonalCycling#
  SeasonalCycling._current_season_idx: SeasonalCycling#_current_season_idx.
  SeasonalCycling._season_length: SeasonalCycling#_season_length.
  logger: logger.
  SeasonalCycling.__init__: SeasonalCycling#__init__().
---
# Module: [`domains/train_opt/mechanisms/seasonal_cycling.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py)

## Classes
### `SeasonalCycling`
- def: [`domains/train_opt/mechanisms/seasonal_cycling.py:61`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L61)
- doc: Enforces crop rotation through parameter families across iterations.
- signature: `class SeasonalCycling:`
- members:
  - `advance(self)` — [`L90`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L90) — Advance one iteration within the current season, rotating if needed. — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
  - `current_season(self)` — [`L83`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L83) — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
  - `get_season_text(self, active_params: list[str])` — [`L121`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L121) — Generate seasonal guidance for the proposal prompt. — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
  - `record_harvest(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L105`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L105) — Record whether this iteration produced a harvest (improvement). — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
  - `season_info(self)` — [`L87`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L87) — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
- protocol/private: `__init__`[`L72`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L72), `_current_season_idx`[`L74`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L74), `_iteration_in_season`[`L75`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L75), `_season_attempts`[`L80`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L80), `_season_harvests`[`L78`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L78), `_season_length`[`L73`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L73)
- uses (calls/refs, reference-scoped): [`SEASON_ORDER`](seasonal_cycling.md#SEASON_ORDER), [`SEASONS`](seasonal_cycling.md#SEASONS), [`logger`](seasonal_cycling.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`seasonal_cycling`](../runner.md#TrainRunner.seasonal_cycling)

## Module values
- `SEASONS` — [`L35`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L35) — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
- `SEASON_ORDER` — [`L58`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L58) — documented in [domains-train_opt-mechanisms-seasonal_cycling](../../../../concepts/domains-train_opt-mechanisms-seasonal_cycling.md)
- `logger` — [`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/seasonal_cycling.py#L31)

