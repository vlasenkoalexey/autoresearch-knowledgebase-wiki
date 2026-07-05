---
title: 'Module: rdagent/components/interactor/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/interactor/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.interactor`/SkipInteractor#
symbols:
  SkipInteractor: ''
  SkipInteractor.interact: interact().
---
# Module: [`rdagent/components/interactor/__init__.py`](../../../../../../../raw/code/rd-agent/rdagent/components/interactor/__init__.py)

## Classes
### `SkipInteractor`  ·  implements/extends Interactor
- def: [`rdagent/components/interactor/__init__.py:6`](../../../../../../../raw/code/rd-agent/rdagent/components/interactor/__init__.py#L6)
- signature: `class SkipInteractor(Interactor[ASpecificExp]):`
- members:
  - `interact(self, exp: ASpecificExp, trace: Trace)` — [`L8`](../../../../../../../raw/code/rd-agent/rdagent/components/interactor/__init__.py#L8) — Interact with the user to get feedback or confirmation.
- uses (calls/refs, reference-scoped): [`Trace`](../../core/proposal.md#Trace), [`ASpecificExp`](../../core/experiment.md#ASpecificExp), [`Interactor`](../../core/interactor.md#Interactor)
- used by: [`Interactor`](../../core/interactor.md#Interactor), [`interact`](../../core/interactor.md#Interactor.interact)

