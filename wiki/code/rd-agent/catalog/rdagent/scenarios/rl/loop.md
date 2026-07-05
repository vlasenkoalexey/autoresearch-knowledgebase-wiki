---
title: 'Module: rdagent/scenarios/rl/loop.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.loop`/RLPostTrainingRDLoop#
symbols:
  RLPostTrainingRDLoop.feedback: feedback().
  RLPostTrainingRDLoop.direct_exp_gen: direct_exp_gen().
  RLPostTrainingRDLoop.coding: coding().
  RLPostTrainingRDLoop.record: record().
  RLPostTrainingRDLoop.dump: dump().
  RLPostTrainingRDLoop.trace: trace.
  RLPostTrainingRDLoop: ''
  RLPostTrainingRDLoop.skip_loop_error: skip_loop_error.
  RLPostTrainingRDLoop.__init__: __init__().
  RLPostTrainingRDLoop.rl_rd_setting: rl_rd_setting.
  RLPostTrainingRDLoop.skip_loop_error_stepname: skip_loop_error_stepname.
  RLPostTrainingRDLoop.withdraw_loop_error: withdraw_loop_error.
---
# Module: [`rdagent/scenarios/rl/loop.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py)

## Classes
### `RLPostTrainingRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/scenarios/rl/loop.py:13`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L13)
- doc: RL post-training loop using standard RDLoop workflow
- signature: `class RLPostTrainingRDLoop(RDLoop):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L36) — Generate rl post-training code
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L29) — Generate RL post-training experiment
  - `dump(self, path)` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L60) — Skip dump if the loop contains unpicklable objects.
  - `feedback(self, prev_out: dict[str, Any])` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L43) — Generate feedback for RL post-training experiment - always call LLM
  - `record(self, prev_out: dict[str, Any])` — [`L54`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L54) — Record the experiment and feedback into trace
  - `rl_rd_setting` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L22)
  - `skip_loop_error` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L16)
  - `skip_loop_error_stepname` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L17)
  - `trace` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L27)
  - `withdraw_loop_error` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L18)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/loop.py#L20)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`warning`](../../log/logger.md#RDAgentLog.warning), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`CoderError`](../../core/exception.md#CoderError), [`develop`](../../core/developer.md#Developer.develop), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`generate_feedback`](../../core/proposal.md#Experiment2Feedback.generate_feedback), [`__init__`](../../components/workflow/rd_loop.md#RDLoop.__init__), [`sync_dag_parent_and_hist`](../../core/proposal.md#Trace.sync_dag_parent_and_hist), [`dump`](../../utils/workflow/loop.md#LoopBase.dump), [`summarizer`](../../components/workflow/rd_loop.md#RDLoop.summarizer), [`coder`](../../components/workflow/rd_loop.md#RDLoop.coder), [`hypothesis_gen`](../../components/workflow/rd_loop.md#RDLoop.hypothesis_gen), [`RLTrace`](proposal/trace.md#RLTrace), [`EXCEPTION_KEY`](../../utils/workflow/loop.md#LoopBase.EXCEPTION_KEY), [`LOOP_IDX_KEY`](../../utils/workflow/loop.md#LoopBase.LOOP_IDX_KEY), [`RLPostTrainingScen`](scen/scenario.md#RLPostTrainingScen)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`feedback`](../../components/workflow/rd_loop.md#RDLoop.feedback), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`main`](../../app/rl/loop.md#main), [`dump`](../../utils/workflow/loop.md#LoopBase.dump), [`record`](../../components/workflow/rd_loop.md#RDLoop.record)

