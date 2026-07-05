---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.diversity_strategy`/
symbols:
  DiversityContextStrategy: DiversityContextStrategy#
  DiversityContextStrategy.should_inject: DiversityContextStrategy#should_inject().
  InjectUntilSOTAGainedStrategy.should_inject: InjectUntilSOTAGainedStrategy#should_inject().
  InjectAtRootStrategy.should_inject: InjectAtRootStrategy#should_inject().
  InjectAtRootStrategy: InjectAtRootStrategy#
  InjectUntilSOTAGainedStrategy: InjectUntilSOTAGainedStrategy#
  AlwaysInjectStrategy: AlwaysInjectStrategy#
  AlwaysInjectStrategy.should_inject: AlwaysInjectStrategy#should_inject().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py)

## Classes
### `AlwaysInjectStrategy`  ·  implements/extends DiversityContextStrategy
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py:61`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L61)
- doc: A strategy that always injects diversity context.
- signature: `class AlwaysInjectStrategy(DiversityContextStrategy):`
- members:
  - `should_inject(self, trace: DSTrace, local_selection: tuple[int, ...])` — [`L66`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L66) — Always returns True to indicate that context should be injected.
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy)
- used by: [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy), [`should_inject`](diversity_strategy.md#DiversityContextStrategy.should_inject)

### `DiversityContextStrategy`  ·  implements/extends ABC
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py:10`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L10)
- doc: An abstract base class for strategies that determine when to inject
- signature: `class DiversityContextStrategy(ABC):`
- members:
  - `should_inject(self, trace: DSTrace, local_selection: tuple[int, ...])` — [`L17`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L17) — Decides whether to inject diversity context based on the current state of the trace
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`should_inject`](diversity_strategy.md#InjectUntilSOTAGainedStrategy.should_inject), [`should_inject`](diversity_strategy.md#InjectAtRootStrategy.should_inject), [`AlwaysInjectStrategy`](diversity_strategy.md#AlwaysInjectStrategy), [`InjectAtRootStrategy`](diversity_strategy.md#InjectAtRootStrategy), [`InjectUntilSOTAGainedStrategy`](diversity_strategy.md#InjectUntilSOTAGainedStrategy), [`should_inject`](diversity_strategy.md#AlwaysInjectStrategy.should_inject)
- used by: [`AlwaysInjectStrategy`](diversity_strategy.md#AlwaysInjectStrategy), [`InjectAtRootStrategy`](diversity_strategy.md#InjectAtRootStrategy), [`InjectUntilSOTAGainedStrategy`](diversity_strategy.md#InjectUntilSOTAGainedStrategy)

### `InjectAtRootStrategy`  ·  implements/extends DiversityContextStrategy
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py:32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L32)
- doc: A strategy that injects diversity context only when creating a new root for a sub-trace.
- signature: `class InjectAtRootStrategy(DiversityContextStrategy):`
- members:
  - `should_inject(self, trace: DSTrace, local_selection: tuple[int, ...])` — [`L37`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L37) — Injects only when `local_selection` indicates a new trace root.
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy)
- used by: [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy), [`should_inject`](diversity_strategy.md#DiversityContextStrategy.should_inject)

### `InjectUntilSOTAGainedStrategy`  ·  implements/extends DiversityContextStrategy
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py:42`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L42)
- doc: A strategy that injects diversity context until the first SOTA (State-of-the-Art)
- signature: `class InjectUntilSOTAGainedStrategy(DiversityContextStrategy):`
- members:
  - `should_inject(self, trace: DSTrace, local_selection: tuple[int, ...])` — [`L48`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/diversity_strategy.py#L48) — Injects if the sub-trace corresponding to the `local_selection` has not
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`sota_experiment`](base.md#DSTrace.sota_experiment), [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy)
- used by: [`DiversityContextStrategy`](diversity_strategy.md#DiversityContextStrategy), [`should_inject`](diversity_strategy.md#DiversityContextStrategy.should_inject)

