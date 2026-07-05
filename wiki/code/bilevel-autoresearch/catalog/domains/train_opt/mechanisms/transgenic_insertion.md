---
title: 'Module: domains/train_opt/mechanisms/transgenic_insertion.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/transgenic_insertion.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.transgenic_insertion`/
symbols:
  TransgenicInsertion.generate_transgenic_candidate: TransgenicInsertion#generate_transgenic_candidate().
  TransgenicInsertion.get_operon_text: TransgenicInsertion#get_operon_text().
  TransgenicInsertion._operon_attempts: TransgenicInsertion#_operon_attempts.
  OPERONS: OPERONS.
  TransgenicInsertion: TransgenicInsertion#
  TransgenicInsertion._insertion_history: TransgenicInsertion#_insertion_history.
  logger: logger.
  TransgenicInsertion.__init__: TransgenicInsertion#__init__().
---
# Module: [`domains/train_opt/mechanisms/transgenic_insertion.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py)

## Classes
### `TransgenicInsertion`
- def: [`domains/train_opt/mechanisms/transgenic_insertion.py:46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L46)
- doc: Transplants exact parameter blocks from elite configs into the current config.
- signature: `class TransgenicInsertion:`
- members:
  - `generate_transgenic_candidate(self, current_config: dict, elite_configs: list[tuple[float, dict]], active_params: list[str])` — [`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L59) — Generate a transgenic insertion candidate.
  - `get_operon_text(self)` — [`L130`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L130) — Generate operon information for the proposal prompt.
- protocol/private: `__init__`[`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L54), `_insertion_history`[`L55`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L55), `_operon_attempts`[`L57`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L57)
- uses (calls/refs, reference-scoped): [`OPERONS`](transgenic_insertion.md#OPERONS)
- used by: [`_propose`](../runner.md#TrainRunner._propose), [`transgenic`](../runner.md#TrainRunner.transgenic)

## Module values
- `OPERONS` — [`L26`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L26)
- `logger` — [`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/transgenic_insertion.py#L22)

