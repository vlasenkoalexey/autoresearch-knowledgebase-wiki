---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.select.expand`/
symbols:
  LimitTimeCKPSelector.get_selection: LimitTimeCKPSelector#get_selection().
  LimitTimeCKPSelector.set_time_limit: LimitTimeCKPSelector#set_time_limit().
  SOTAJumpCKPSelector.get_selection: SOTAJumpCKPSelector#get_selection().
  BackJumpCKPSelector.get_selection: BackJumpCKPSelector#get_selection().
  BackJumpCKPSelector.MAX_TRACE_NUM: BackJumpCKPSelector#MAX_TRACE_NUM.
  SOTAJumpCKPSelector.MAX_TRACE_NUM: SOTAJumpCKPSelector#MAX_TRACE_NUM.
  BackJumpCKPSelector.SOTA_COUNT_THRESHOLD: BackJumpCKPSelector#SOTA_COUNT_THRESHOLD.
  SOTAJumpCKPSelector.SOTA_COUNT_THRESHOLD: SOTAJumpCKPSelector#SOTA_COUNT_THRESHOLD.
  LimitTimeCKPSelector.global_timer: LimitTimeCKPSelector#global_timer.
  LimitTimeCKPSelector.MAX_TRACE_NUM: LimitTimeCKPSelector#MAX_TRACE_NUM.
  SOTAJumpCKPSelector.SOTA_COUNT_WINDOW: SOTAJumpCKPSelector#SOTA_COUNT_WINDOW.
  BackJumpCKPSelector.SOTA_COUNT_WINDOW: BackJumpCKPSelector#SOTA_COUNT_WINDOW.
  LimitTimeCKPSelector.time_limit_pre_trace: LimitTimeCKPSelector#time_limit_pre_trace.
  LatestCKPSelector.__init__: LatestCKPSelector#__init__().
  LimitTimeCKPSelector.sub_trace_start_times: LimitTimeCKPSelector#sub_trace_start_times.
  LatestCKPSelector: LatestCKPSelector#
  LatestCKPSelector.get_selection: LatestCKPSelector#get_selection().
  LimitTimeCKPSelector: LimitTimeCKPSelector#
  SOTAJumpCKPSelector: SOTAJumpCKPSelector#
  BackJumpCKPSelector: BackJumpCKPSelector#
  LimitTimeCKPSelector.__init__: LimitTimeCKPSelector#__init__().
  SOTAJumpCKPSelector.__init__: SOTAJumpCKPSelector#__init__().
  BackJumpCKPSelector.__init__: BackJumpCKPSelector#__init__().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py)

## Classes
### `BackJumpCKPSelector`  ·  implements/extends CheckpointSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py:156`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L156)
- doc: back-jump policy:
- signature: `class BackJumpCKPSelector(CheckpointSelector):`
- members:
  - `get_selection(self, trace: Trace)` — [`L175`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L175) — documented in [rdagent-core-proposal](../../../../../../../concepts/rdagent-core-proposal.md)
  - `MAX_TRACE_NUM` — [`L169`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L169)
  - `SOTA_COUNT_THRESHOLD` — [`L168`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L168)
  - `SOTA_COUNT_WINDOW` — [`L167`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L167)
- protocol/private: `__init__`[`L164`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L164)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`hist`](../../../../../core/proposal.md#Trace.hist), [`Trace`](../../../../../core/proposal.md#Trace), [`NEW_ROOT`](../../../../../core/proposal.md#Trace.NEW_ROOT), [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`max_trace_num`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.max_trace_num), [`sota_count_threshold`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.sota_count_threshold), [`sota_count_window`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.sota_count_window)
- used by: [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`get_selection`](../../../../../core/proposal.md#CheckpointSelector.get_selection)

### `LatestCKPSelector`  ·  implements/extends CheckpointSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py:13`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L13)
- doc: -`(-1, )` represents starting from the latest trial in the trace
- signature: `class LatestCKPSelector(CheckpointSelector):`
- members:
  - `get_selection(self, trace: Trace)` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L23)
- protocol/private: `__init__`[`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L18)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`Trace`](../../../../../core/proposal.md#Trace), [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector)
- used by: [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`get_selection`](../../../../../core/proposal.md#CheckpointSelector.get_selection)

### `LimitTimeCKPSelector`  ·  implements/extends CheckpointSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py:28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L28)
- doc: recore the time of current sub-trace, and jump to a new sub-trace if the time is up
- signature: `class LimitTimeCKPSelector(CheckpointSelector):`
- members:
  - `get_selection(self, trace: Trace)` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L52) — Determine whether to continue with the current sub-trace or start a new one — documented in [rdagent-core-proposal](../../../../../../../concepts/rdagent-core-proposal.md)
  - `set_time_limit(self)` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L41)
  - `MAX_TRACE_NUM` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L38)
  - `global_timer` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L36) — documented in [rdagent-log-timer](../../../../../../../concepts/rdagent-log-timer.md)
  - `sub_trace_start_times` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L37)
  - `time_limit_pre_trace` — [`L39`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L39)
- protocol/private: `__init__`[`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L33)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`hist`](../../../../../core/proposal.md#Trace.hist), [`Trace`](../../../../../core/proposal.md#Trace), [`RD_Agent_TIMER_wrapper`](../../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`timer`](../../../../../log/timer.md#RDAgentTimerWrapper.timer), [`NEW_ROOT`](../../../../../core/proposal.md#Trace.NEW_ROOT), [`all_duration`](../../../../../log/timer.md#RDAgentTimer.all_duration), [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`RDAgentTimer`](../../../../../log/timer.md#RDAgentTimer), [`merge_hours`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`max_trace_num`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.max_trace_num)
- used by: [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`get_selection`](../../../../../core/proposal.md#CheckpointSelector.get_selection)

### `SOTAJumpCKPSelector`  ·  implements/extends CheckpointSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py:100`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L100)
- doc: SOTA jump policy:
- signature: `class SOTAJumpCKPSelector(CheckpointSelector):`
- members:
  - `get_selection(self, trace: Trace)` — [`L118`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L118) — documented in [rdagent-core-proposal](../../../../../../../concepts/rdagent-core-proposal.md)
  - `MAX_TRACE_NUM` — [`L112`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L112)
  - `SOTA_COUNT_THRESHOLD` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L111)
  - `SOTA_COUNT_WINDOW` — [`L110`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L110)
- protocol/private: `__init__`[`L107`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/expand.py#L107)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`hist`](../../../../../core/proposal.md#Trace.hist), [`Trace`](../../../../../core/proposal.md#Trace), [`NEW_ROOT`](../../../../../core/proposal.md#Trace.NEW_ROOT), [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`max_trace_num`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.max_trace_num), [`sota_count_threshold`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.sota_count_threshold), [`sota_count_window`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.sota_count_window)
- used by: [`CheckpointSelector`](../../../../../core/proposal.md#CheckpointSelector), [`get_selection`](../../../../../core/proposal.md#CheckpointSelector.get_selection)

