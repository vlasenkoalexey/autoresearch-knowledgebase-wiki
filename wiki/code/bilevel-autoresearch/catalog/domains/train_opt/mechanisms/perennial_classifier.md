---
title: 'Module: domains/train_opt/mechanisms/perennial_classifier.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/perennial_classifier.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.perennial_classifier`/
symbols:
  PerennialClassifier.classify: PerennialClassifier#classify().
  PerennialClassifier.get_perennial_text: PerennialClassifier#get_perennial_text().
  PerennialClassifier.record: PerennialClassifier#record().
  PerennialClassifier: PerennialClassifier#
  PerennialClassifier._history: PerennialClassifier#_history.
  PerennialClassifier._min_trials: PerennialClassifier#_min_trials.
  PerennialClassifier._convergence_threshold: PerennialClassifier#_convergence_threshold.
  logger: logger.
  PerennialClassifier.__init__: PerennialClassifier#__init__().
---
# Module: [`domains/train_opt/mechanisms/perennial_classifier.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py)

## Classes
### `PerennialClassifier`
- def: [`domains/train_opt/mechanisms/perennial_classifier.py:32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L32)
- doc: Classifies parameters as perennial (settled) vs annual (volatile).
- signature: `class PerennialClassifier:`
- members:
  - `classify(self, active_params: list[str])` — [`L72`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L72) — Classify each active parameter as perennial or annual.
  - `get_perennial_text(self, active_params: list[str])` — [`L117`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L117) — Generate perennial/annual classification for the proposal prompt.
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str, iteration: int)` — [`L57`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L57) — Record a parameter change and its outcome.
- protocol/private: `__init__`[`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L48), `_convergence_threshold`[`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L52), `_history`[`L55`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L55), `_min_trials`[`L49`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L49)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`perennial_classifier`](../runner.md#TrainRunner.perennial_classifier)

## Module values
- `logger` — [`L29`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/perennial_classifier.py#L29)

