---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.trace_scheduler`/
symbols:
  MCTSScheduler.select: MCTSScheduler#select().
  MCTSScheduler.observe_feedback: MCTSScheduler#observe_feedback().
  ProbabilisticScheduler.select: ProbabilisticScheduler#select().
  BaseScheduler.next: BaseScheduler#next().
  ProbabilisticScheduler: ProbabilisticScheduler#
  RoundRobinScheduler.select: RoundRobinScheduler#select().
  MCTSScheduler.reset: MCTSScheduler#reset().
  SOTABasedScheduler.calculate_potential: SOTABasedScheduler#calculate_potential().
  MCTSScheduler.process_uncommitted_nodes: MCTSScheduler#process_uncommitted_nodes().
  ProbabilisticScheduler.calculate_potential: ProbabilisticScheduler#calculate_potential().
  MCTSScheduler._get_u: MCTSScheduler#_get_u().
  BaseScheduler.uncommited_rec_status: BaseScheduler#uncommited_rec_status.
  BaseScheduler: BaseScheduler#
  BaseScheduler.select: BaseScheduler#select().
  BaseScheduler.reset: BaseScheduler#reset().
  TraceLengthScheduler.__init__: TraceLengthScheduler#__init__().
  TraceLengthScheduler.calculate_potential: TraceLengthScheduler#calculate_potential().
  SOTABasedScheduler.__init__: SOTABasedScheduler#__init__().
  TraceScheduler.next: TraceScheduler#next().
  BaseScheduler.process_uncommitted_nodes: BaseScheduler#process_uncommitted_nodes().
  MCTSScheduler._get_q: MCTSScheduler#_get_q().
  TraceScheduler: TraceScheduler#
  RoundRobinScheduler.__init__: RoundRobinScheduler#__init__().
  MCTSScheduler.node_visit_count: MCTSScheduler#node_visit_count.
  ProbabilisticScheduler._softmax_probabilities: ProbabilisticScheduler#_softmax_probabilities().
  MCTSScheduler: MCTSScheduler#
  MCTSScheduler.node_value_sum: MCTSScheduler#node_value_sum.
  TraceScheduler.reset: TraceScheduler#reset().
  RoundRobinScheduler: RoundRobinScheduler#
  ProbabilisticScheduler.temperature: ProbabilisticScheduler#temperature.
  SOTABasedScheduler: SOTABasedScheduler#
  MCTSScheduler.c_puct: MCTSScheduler#c_puct.
  BaseScheduler.rec_commit_idx: BaseScheduler#rec_commit_idx.
  ProbabilisticScheduler.__init__: ProbabilisticScheduler#__init__().
  MCTSScheduler.node_prior: MCTSScheduler#node_prior.
  MCTSScheduler.global_visit_count: MCTSScheduler#global_visit_count.
  MCTSScheduler.last_observed_commit_idx: MCTSScheduler#last_observed_commit_idx.
  RoundRobinScheduler._last_selected_leaf_id: RoundRobinScheduler#_last_selected_leaf_id.
  TraceLengthScheduler: TraceLengthScheduler#
  RandomScheduler: RandomScheduler#
  RandomScheduler.calculate_potential: RandomScheduler#calculate_potential().
  MCTSScheduler.__init__: MCTSScheduler#__init__().
  BaseScheduler.__init__: BaseScheduler#__init__().
  ProbabilisticScheduler.max_trace_num: ProbabilisticScheduler#max_trace_num.
  RoundRobinScheduler.max_trace_num: RoundRobinScheduler#max_trace_num.
  TraceLengthScheduler.inverse: TraceLengthScheduler#inverse.
  SOTABasedScheduler.inverse: SOTABasedScheduler#inverse.
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py)

## Classes
### `BaseScheduler`  ·  implements/extends TraceScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:50`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L50)
- signature: `class BaseScheduler(TraceScheduler):`
- members:
  - `next(self, trace: DSTrace)` — [`L55`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L55) — Atomically selects the next leaf node from the trace in order. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `process_uncommitted_nodes(self, trace: DSTrace)` — [`L85`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L85) — A slot for implementing custom logic to process uncommitted nodes.
  - `reset(self)` — [`L97`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L97)
  - `select(self, trace: DSTrace)` — [`L93`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L93) — Selects the parent nodes for the new experiment, or None if no selection can be made.
  - `rec_commit_idx` — [`L52`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L52)
  - `uncommited_rec_status` — [`L53`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L53)
- protocol/private: `__init__`[`L51`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L51)
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`hist`](base.md#DSTrace.hist), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`select`](trace_scheduler.md#ProbabilisticScheduler.select), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`dag_parent`](../../../../core/proposal.md#Trace.dag_parent), [`reset`](trace_scheduler.md#MCTSScheduler.reset), [`select`](trace_scheduler.md#RoundRobinScheduler.select), [`process_uncommitted_nodes`](trace_scheduler.md#MCTSScheduler.process_uncommitted_nodes), [`TraceScheduler`](trace_scheduler.md#TraceScheduler), [`RoundRobinScheduler`](trace_scheduler.md#RoundRobinScheduler)
- used by: [`select`](trace_scheduler.md#MCTSScheduler.select), [`select`](trace_scheduler.md#ProbabilisticScheduler.select), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`reset`](trace_scheduler.md#MCTSScheduler.reset), [`select`](trace_scheduler.md#RoundRobinScheduler.select), [`next`](trace_scheduler.md#TraceScheduler.next), [`TraceScheduler`](trace_scheduler.md#TraceScheduler), [`RoundRobinScheduler`](trace_scheduler.md#RoundRobinScheduler), [`reset`](trace_scheduler.md#TraceScheduler.reset), [`temperature`](trace_scheduler.md#ProbabilisticScheduler.temperature), [`_last_selected_leaf_id`](trace_scheduler.md#RoundRobinScheduler._last_selected_leaf_id)

### `MCTSScheduler`  ·  implements/extends ProbabilisticScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:316`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L316)
- doc: A simplified MCTS-based scheduler using a PUCT-like scoring rule.
- signature: `class MCTSScheduler(ProbabilisticScheduler):`
- members:
  - `observe_feedback(self, trace: DSTrace, new_idx: int)` — [`L396`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L396) — Update statistics after an experiment is committed to the trace. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `process_uncommitted_nodes(self, trace: DSTrace)` — [`L431`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L431) — Batch observe all newly committed experiments since last observation.
  - `reset(self)` — [`L420`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L420) — Clear all maintained statistics. Should be called when the underlying trace is reset.
  - `select(self, trace: DSTrace)` — [`L358`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L358) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `c_puct` — [`L334`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L334)
  - `global_visit_count` — [`L340`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L340)
  - `last_observed_commit_idx` — [`L342`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L342)
  - `node_prior` — [`L338`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L338)
  - `node_value_sum` — [`L337`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L337)
  - `node_visit_count` — [`L336`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L336)
- protocol/private: `__init__`[`L331`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L331), `_get_q`[`L344`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L344), `_get_u`[`L352`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L352)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`DSTrace`](base.md#DSTrace), [`result`](../../../../core/experiment.md#Experiment.result), [`scen`](../../../../core/proposal.md#Trace.scen), [`hist`](base.md#DSTrace.hist), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`dag_parent`](../../../../core/proposal.md#Trace.dag_parent), [`get_metric_direction`](../../../kaggle/kaggle_crawler.md#get_metric_direction), [`competition`](../../scen/__init__.md#DataScienceScen.competition), [`get_parents`](../../../../core/proposal.md#Trace.get_parents), [`calculate_potential`](trace_scheduler.md#ProbabilisticScheduler.calculate_potential), [`uncommited_rec_status`](trace_scheduler.md#BaseScheduler.uncommited_rec_status), [`sub_trace_count`](base.md#DSTrace.sub_trace_count), [`reset`](trace_scheduler.md#BaseScheduler.reset), [`_softmax_probabilities`](trace_scheduler.md#ProbabilisticScheduler._softmax_probabilities), [`__init__`](trace_scheduler.md#ProbabilisticScheduler.__init__), [`max_trace_num`](trace_scheduler.md#ProbabilisticScheduler.max_trace_num), [`enable_score_reward`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_score_reward)
- used by: [`select`](trace_scheduler.md#ProbabilisticScheduler.select), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`reset`](trace_scheduler.md#BaseScheduler.reset), [`process_uncommitted_nodes`](trace_scheduler.md#BaseScheduler.process_uncommitted_nodes)

### `ProbabilisticScheduler`  ·  implements/extends BaseScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:139`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L139)
- doc: A concurrency-safe scheduling strategy that samples the next trace to expand
- signature: `class ProbabilisticScheduler(BaseScheduler):`
- members:
  - `__init__(self, max_trace_num: int, temperature: float = 1, *args, **kwargs)` — [`L145`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L145) — Args:
  - `_softmax_probabilities(self, potentials: list[float])` — [`L174`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L174) — Convert potential scores to probabilities using softmax.
  - `calculate_potential(self, trace: DSTrace, leaf_id: int)` — [`L160`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L160) — Calculate potential score for a given leaf node.
  - `select(self, trace: DSTrace)` — [`L201`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L201) — Selects the next leaf node based on probabilistic sampling. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `max_trace_num` — [`L156`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L156)
  - `temperature` — [`L157`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L157)
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`select`](trace_scheduler.md#MCTSScheduler.select), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`get_leaves`](base.md#DSTrace.get_leaves), [`calculate_potential`](trace_scheduler.md#SOTABasedScheduler.calculate_potential), [`uncommited_rec_status`](trace_scheduler.md#BaseScheduler.uncommited_rec_status), [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`sub_trace_count`](base.md#DSTrace.sub_trace_count), [`calculate_potential`](trace_scheduler.md#TraceLengthScheduler.calculate_potential), [`MCTSScheduler`](trace_scheduler.md#MCTSScheduler), [`SOTABasedScheduler`](trace_scheduler.md#SOTABasedScheduler), [`RandomScheduler`](trace_scheduler.md#RandomScheduler), [`TraceLengthScheduler`](trace_scheduler.md#TraceLengthScheduler), [`calculate_potential`](trace_scheduler.md#RandomScheduler.calculate_potential), [`__init__`](trace_scheduler.md#BaseScheduler.__init__)
- used by: [`select`](trace_scheduler.md#MCTSScheduler.select), [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`select`](trace_scheduler.md#BaseScheduler.select), [`__init__`](trace_scheduler.md#SOTABasedScheduler.__init__), [`__init__`](trace_scheduler.md#TraceLengthScheduler.__init__), [`MCTSScheduler`](trace_scheduler.md#MCTSScheduler), [`SOTABasedScheduler`](trace_scheduler.md#SOTABasedScheduler), [`RandomScheduler`](trace_scheduler.md#RandomScheduler), [`TraceLengthScheduler`](trace_scheduler.md#TraceLengthScheduler), [`__init__`](trace_scheduler.md#MCTSScheduler.__init__)

### `RandomScheduler`  ·  implements/extends ProbabilisticScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:304`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L304)
- doc: A scheduler that selects traces randomly with uniform distribution.
- signature: `class RandomScheduler(ProbabilisticScheduler):`
- members:
  - `calculate_potential(self, trace: DSTrace, leaf_id: int)` — [`L309`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L309) — Return random potential for uniform random selection.
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler)
- used by: [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`calculate_potential`](trace_scheduler.md#ProbabilisticScheduler.calculate_potential)

### `RoundRobinScheduler`  ·  implements/extends BaseScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:102`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L102)
- doc: A concurrency-safe scheduling strategy that cycles through active traces
- signature: `class RoundRobinScheduler(BaseScheduler):`
- members:
  - `select(self, trace: DSTrace)` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L116) — Atomically selects the next leaf node from the trace in order.
  - `max_trace_num` — [`L112`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L112)
- protocol/private: `__init__`[`L110`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L110), `_last_selected_leaf_id`[`L113`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L113)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DSTrace`](base.md#DSTrace), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`get_leaves`](base.md#DSTrace.get_leaves), [`uncommited_rec_status`](trace_scheduler.md#BaseScheduler.uncommited_rec_status), [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`sub_trace_count`](base.md#DSTrace.sub_trace_count), [`__init__`](trace_scheduler.md#BaseScheduler.__init__)
- used by: [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`select`](trace_scheduler.md#BaseScheduler.select)

### `SOTABasedScheduler`  ·  implements/extends ProbabilisticScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:267`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L267)
- doc: A scheduler that prefers traces with more SOTA (State of the Art) results.
- signature: `class SOTABasedScheduler(ProbabilisticScheduler):`
- members:
  - `__init__(self, max_trace_num: int, temperature: float = 1, inverse: bool = False, *args, **kwargs)` — [`L272`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L272) — Args:
  - `calculate_potential(self, trace: DSTrace, leaf_id: int)` — [`L283`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L283) — Calculate potential based on the number of SOTA results in the trace.
  - `inverse` — [`L281`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L281)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DSTrace`](base.md#DSTrace), [`hist`](base.md#DSTrace.hist), [`decision`](../../../../core/proposal.md#ExperimentFeedback.decision), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`get_parents`](../../../../core/proposal.md#Trace.get_parents), [`__init__`](trace_scheduler.md#ProbabilisticScheduler.__init__)
- used by: [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`calculate_potential`](trace_scheduler.md#ProbabilisticScheduler.calculate_potential)

### `TraceLengthScheduler`  ·  implements/extends ProbabilisticScheduler
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:232`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L232)
- doc: A scheduler that prefers longer traces (more experiments)
- signature: `class TraceLengthScheduler(ProbabilisticScheduler):`
- members:
  - `__init__(self, max_trace_num: int, temperature: float = 1, inverse: bool = False, *args, **kwargs)` — [`L240`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L240) — Args:
  - `calculate_potential(self, trace: DSTrace, leaf_id: int)` — [`L253`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L253) — Calculate potential based on the length of the trace leading to the leaf.
  - `inverse` — [`L251`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L251)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DSTrace`](base.md#DSTrace), [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`get_parents`](../../../../core/proposal.md#Trace.get_parents), [`__init__`](trace_scheduler.md#ProbabilisticScheduler.__init__)
- used by: [`ProbabilisticScheduler`](trace_scheduler.md#ProbabilisticScheduler), [`calculate_potential`](trace_scheduler.md#ProbabilisticScheduler.calculate_potential)

### `TraceScheduler`  ·  implements/extends ABC
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py:18`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L18)
- doc: An abstract base class for trace scheduling strategies.
- signature: `class TraceScheduler(ABC):`
- members:
  - `next(self, trace: DSTrace)` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L25) — Selects the next trace to expand.
  - `reset(self)` — [`L43`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/trace_scheduler.py#L43) — Reset the scheduler to the initial state.
- uses (calls/refs, reference-scoped): [`DSTrace`](base.md#DSTrace), [`next`](trace_scheduler.md#BaseScheduler.next), [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`reset`](trace_scheduler.md#BaseScheduler.reset)
- used by: [`async_gen`](router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`trace_scheduler`](router/__init__.md#ParallelMultiTraceExpGen.trace_scheduler), [`BaseScheduler`](trace_scheduler.md#BaseScheduler), [`reset`](router/__init__.md#ParallelMultiTraceExpGen.reset)

