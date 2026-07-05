---
title: 'Module: domains/train_opt/mechanisms/back_translation.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/back_translation.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.back_translation`/
symbols:
  BackTranslation.get_calibration_text: BackTranslation#get_calibration_text().
  BackTranslation.record_prediction: BackTranslation#record_prediction().
  BackTranslation.record_outcome: BackTranslation#record_outcome().
  BackTranslation._predictions: BackTranslation#_predictions.
  BackTranslation: BackTranslation#
  BackTranslation._overall: BackTranslation#_overall.
  BackTranslation._min_samples: BackTranslation#_min_samples.
  BackTranslation._error_threshold: BackTranslation#_error_threshold.
  logger: logger.
  BackTranslation.__init__: BackTranslation#__init__().
---
# Module: [`domains/train_opt/mechanisms/back_translation.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py)

## Classes
### `BackTranslation`
- def: [`domains/train_opt/mechanisms/back_translation.py:19`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L19)
- doc: Tracks LLM prediction accuracy to expose systematic misunderstandings.
- signature: `class BackTranslation:`
- members:
  - `__init__(self, min_samples: int = 3, error_threshold: float = 0.002)` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L28) — Args:
  - `get_calibration_text(self)` — [`L98`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L98) — Generate a calibration report for the proposal prompt.
  - `record_outcome(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L69`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L69) — Record the actual outcome after training completes.
  - `record_prediction(self, changes: dict, expected_direction: str, hypothesis: str)` — [`L45`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L45) — Record the LLM's prediction before training runs.
- protocol/private: `_error_threshold`[`L35`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L35), `_min_samples`[`L34`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L34), `_overall`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L43), `_predictions`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L40)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`back_translation`](../runner.md#TrainRunner.back_translation)

## Module values
- `logger` — [`L16`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/back_translation.py#L16)

