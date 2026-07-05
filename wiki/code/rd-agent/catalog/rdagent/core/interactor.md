---
title: 'Module: rdagent/core/interactor.py'
type: catalog
provenance: extracted
module: rdagent/core/interactor.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.interactor`/Interactor#
symbols:
  Interactor: ''
  Interactor.interact: interact().
  Interactor.__init__: __init__().
  Interactor.scen: scen.
---
# Module: [`rdagent/core/interactor.py`](../../../../../../raw/code/rd-agent/rdagent/core/interactor.py)

## Classes
### `Interactor`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/interactor.py:13`](../../../../../../raw/code/rd-agent/rdagent/core/interactor.py#L13)
- signature: `class Interactor(ABC, Generic[ASpecificExp]):`
- members:
  - `interact(self, exp: ASpecificExp, trace: Trace | None = None)` — [`L18`](../../../../../../raw/code/rd-agent/rdagent/core/interactor.py#L18) — Interact with the experiment to get feedback or confirmation.
  - `scen` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/core/interactor.py#L15)
- protocol/private: `__init__`[`L14`](../../../../../../raw/code/rd-agent/rdagent/core/interactor.py#L14)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`interact`](../scenarios/data_science/interactor/__init__.md#DSInteractor.interact), [`ASpecificExp`](experiment.md#ASpecificExp), [`DSInteractor`](../scenarios/data_science/interactor/__init__.md#DSInteractor), [`SkipInteractor`](../components/interactor/__init__.md#SkipInteractor), [`interact`](../components/interactor/__init__.md#SkipInteractor.interact)
- used by: [`interact`](../scenarios/data_science/interactor/__init__.md#DSInteractor.interact), [`DSInteractor`](../scenarios/data_science/interactor/__init__.md#DSInteractor), [`SkipInteractor`](../components/interactor/__init__.md#SkipInteractor)

