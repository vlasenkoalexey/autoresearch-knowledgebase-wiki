---
title: 'Module: domains/train_opt/mechanisms/semantic_equivalence.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/semantic_equivalence.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.semantic_equivalence`/
symbols:
  SemanticEquivalence.record: SemanticEquivalence#record().
  SemanticEquivalence.canonicalize: SemanticEquivalence#canonicalize().
  SemanticEquivalence.check_duplicate: SemanticEquivalence#check_duplicate().
  SemanticEquivalence._canonical_history: SemanticEquivalence#_canonical_history.
  SemanticEquivalence._raw_proposals: SemanticEquivalence#_raw_proposals.
  SemanticEquivalence._magnitude_bin: SemanticEquivalence#_magnitude_bin().
  SemanticEquivalence.get_redundancy_summary: SemanticEquivalence#get_redundancy_summary().
  SemanticEquivalence: SemanticEquivalence#
  SemanticEquivalence.get_equivalence_text: SemanticEquivalence#get_equivalence_text().
  SemanticEquivalence._max_history: SemanticEquivalence#_max_history.
  SemanticEquivalence._MAGNITUDE_BINS: SemanticEquivalence#_MAGNITUDE_BINS.
  SemanticEquivalence._direction: SemanticEquivalence#_direction().
  logger: logger.
  SemanticEquivalence.__init__: SemanticEquivalence#__init__().
---
# Module: [`domains/train_opt/mechanisms/semantic_equivalence.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py)

## Classes
### `SemanticEquivalence`
- def: [`domains/train_opt/mechanisms/semantic_equivalence.py:22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L22)
- doc: Detects semantically equivalent proposals that differ only in wording.
- signature: `class SemanticEquivalence:`
- members:
  - `__init__(self, max_history: int = 50)` — [`L39`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L39) — Args:
  - `_direction(self, old_val: str, new_val)` — [`L68`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L68) — Determine direction of change.
  - `_magnitude_bin(self, old_val: str, new_val)` — [`L53`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L53) — Classify the relative magnitude of a parameter change.
  - `canonicalize(self, changes: dict, old_config: dict)` — [`L81`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L81) — Convert a proposal to a list of canonical (param, direction, magnitude) keys.
  - `check_duplicate(self, changes: dict, old_config: dict)` — [`L91`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L91) — Check if a proposal is semantically equivalent to a previous one.
  - `get_equivalence_text(self, changes: dict, old_config: dict)` — [`L149`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L149) — Generate a warning if the proposed change is semantically equivalent
  - `get_redundancy_summary(self)` — [`L191`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L191) — Generate a summary of which canonical regions have been over-tested.
  - `record(self, changes: dict, old_config: dict, iteration: int, hypothesis: str, val_bpb: float, best_bpb_before: float, status: str)` — [`L113`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L113) — Record a proposal and its outcome for future deduplication.
- protocol/private: `_MAGNITUDE_BINS`[`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L32), `_canonical_history`[`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L48), `_max_history`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L44), `_raw_proposals`[`L51`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L51)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`semantic_equivalence`](../runner.md#TrainRunner.semantic_equivalence)

## Module values
- `logger` — [`L19`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/semantic_equivalence.py#L19)

