---
title: 'Module: rdagent/utils/workflow/tracking.py'
type: catalog
provenance: extracted
module: rdagent/utils/workflow/tracking.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.workflow.tracking`/
symbols:
  WorkflowTracker.log_workflow_state: WorkflowTracker#log_workflow_state().
  mlflow: mlflow.
  WorkflowTracker.loop_base: WorkflowTracker#loop_base.
  WorkflowTracker.is_enabled: WorkflowTracker#is_enabled().
  WorkflowTracker: WorkflowTracker#
  WorkflowTracker.__init__: WorkflowTracker#__init__().
  WorkflowTracker._datetime_to_float: WorkflowTracker#_datetime_to_float().
---
# Module: [`rdagent/utils/workflow/tracking.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py)

## Classes
### `WorkflowTracker`
- def: [`rdagent/utils/workflow/tracking.py:34`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L34)
- doc: A workflow-specific tracking system that logs metrics related to workflow execution.
- signature: `class WorkflowTracker:`
- members:
  - `__init__(self, loop_base: LoopBase)` — [`L42`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L42) — Initialize a WorkflowTracker with a LoopBase instance.
  - `_datetime_to_float(dt: datetime.datetime)` — [`L57`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L57) — Convert datetime to a structured float representation.
  - `is_enabled()` — [`L52`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L52) — Check if tracking is enabled.
  - `log_workflow_state(self)` — [`L61`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L61) — Log all workflow state metrics from the associated LoopBase instance. — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `loop_base` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L49)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`warning`](../../log/logger.md#RDAgentLog.warning), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`RD_Agent_TIMER_wrapper`](../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`remain_time`](../../log/timer.md#RDAgentTimer.remain_time), [`timer`](loop.md#LoopBase.timer), [`LoopBase`](loop.md#LoopBase), [`mlflow`](tracking.md#mlflow), [`started`](../../log/timer.md#RDAgentTimer.started), [`all_duration`](../../log/timer.md#RDAgentTimer.all_duration), [`loop_idx`](loop.md#LoopBase.loop_idx), [`step_idx`](loop.md#LoopBase.step_idx), [`enable_mlflow`](../../core/conf.md#RDAgentSettings.enable_mlflow), [`api_fail_count`](../../log/timer.md#RDAgentTimerWrapper.api_fail_count), [`latest_api_fail_time`](../../log/timer.md#RDAgentTimerWrapper.latest_api_fail_time)
- used by: [`_run_step`](loop.md#LoopBase._run_step), [`tracker`](loop.md#LoopBase.tracker)

## Module values
- `mlflow` — [`L23`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/tracking.py#L23)

