---
title: 'Module: domains/train_opt/mechanisms/register_adaptation.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/register_adaptation.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.register_adaptation`/
symbols:
  RegisterAdaptation._maybe_switch: RegisterAdaptation#_maybe_switch().
  RegisterAdaptation.record: RegisterAdaptation#record().
  RegisterAdaptation.get_register_text: RegisterAdaptation#get_register_text().
  _REGISTERS: _REGISTERS.
  RegisterAdaptation._current_register: RegisterAdaptation#_current_register.
  RegisterAdaptation.get_register_prefix: RegisterAdaptation#get_register_prefix().
  RegisterAdaptation._switch_window: RegisterAdaptation#_switch_window.
  RegisterAdaptation._outcomes: RegisterAdaptation#_outcomes.
  RegisterAdaptation._stagnation_count: RegisterAdaptation#_stagnation_count.
  RegisterAdaptation: RegisterAdaptation#
  RegisterAdaptation._switch_log: RegisterAdaptation#_switch_log.
  RegisterAdaptation._iters_in_register: RegisterAdaptation#_iters_in_register.
  RegisterAdaptation.get_current_register: RegisterAdaptation#get_current_register().
  REGISTER_FORMAL: REGISTER_FORMAL.
  logger: logger.
  REGISTER_INFORMAL: REGISTER_INFORMAL.
  REGISTER_TERSE: REGISTER_TERSE.
  RegisterAdaptation._min_samples: RegisterAdaptation#_min_samples.
  RegisterAdaptation.__init__: RegisterAdaptation#__init__().
---
# Module: [`domains/train_opt/mechanisms/register_adaptation.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py)

## Classes
### `RegisterAdaptation`
- def: [`domains/train_opt/mechanisms/register_adaptation.py:51`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L51)
- doc: Adaptively selects prompt register based on search phase and outcomes.
- signature: `class RegisterAdaptation:`
- members:
  - `__init__(self, switch_window: int = 4, min_samples_per_register: int = 2)` — [`L60`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L60) — Args:
  - `_maybe_switch(self, iteration: int)` — [`L122`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L122) — Evaluate whether to switch to a different register. — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
  - `get_current_register(self)` — [`L84`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L84) — Return the name of the currently active register.
  - `get_register_prefix(self)` — [`L88`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L88) — Return the prompt prefix text for the current register. — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
  - `get_register_text(self)` — [`L179`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L179) — Generate register context for the proposal prompt. — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
  - `record(self, val_bpb: float, best_bpb_before: float, status: str, iteration: int)` — [`L92`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L92) — Record the outcome of a proposal made under the current register. — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
- protocol/private: `_current_register`[`L73`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L73), `_iters_in_register`[`L79`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L79), `_min_samples`[`L67`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L67), `_outcomes`[`L70`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L70), `_stagnation_count`[`L82`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L82), `_switch_log`[`L76`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L76), `_switch_window`[`L66`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L66)
- uses (calls/refs, reference-scoped): [`_REGISTERS`](register_adaptation.md#_REGISTERS), [`REGISTER_FORMAL`](register_adaptation.md#REGISTER_FORMAL), [`logger`](register_adaptation.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`register_adaptation`](../runner.md#TrainRunner.register_adaptation)

## Module values
- `REGISTER_FORMAL` — [`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L22) — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
- `REGISTER_INFORMAL` — [`L30`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L30) — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
- `REGISTER_TERSE` — [`L37`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L37) — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
- `_REGISTERS` — [`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L44) — documented in [domains-train_opt-mechanisms-register_adaptation](../../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
- `logger` — [`L18`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/register_adaptation.py#L18)

