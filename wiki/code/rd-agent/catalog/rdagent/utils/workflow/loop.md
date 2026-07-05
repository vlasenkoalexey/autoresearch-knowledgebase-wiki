---
title: 'Module: rdagent/utils/workflow/loop.py'
type: catalog
provenance: extracted
module: rdagent/utils/workflow/loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.workflow.loop`/
symbols:
  LoopBase._run_step: LoopBase#_run_step().
  LoopBase.run: LoopBase#run().
  LoopBase.load: LoopBase#load().
  LoopBase._check_exit_conditions_on_step: LoopBase#_check_exit_conditions_on_step().
  LoopBase.kickoff_loop: LoopBase#kickoff_loop().
  LoopBase.timer: LoopBase#timer.
  LoopBase: LoopBase#
  LoopBase.execute_loop: LoopBase#execute_loop().
  LoopBase.dump: LoopBase#dump().
  LoopBase.steps: LoopBase#steps.
  LoopBase.loop_idx: LoopBase#loop_idx.
  LoopBase.withdraw_loop: LoopBase#withdraw_loop().
  LoopBase.loop_prev_out: LoopBase#loop_prev_out.
  LoopBase.session_folder: LoopBase#session_folder.
  LoopBase.get_unfinished_loop_cnt: LoopBase#get_unfinished_loop_cnt().
  LoopBase.loop_trace: LoopBase#loop_trace.
  LoopBase.step_idx: LoopBase#step_idx.
  LoopBase.get_semaphore: LoopBase#get_semaphore().
  LoopBase.loop_n: LoopBase#loop_n.
  LoopMeta: LoopMeta#
  LoopMeta._get_steps: LoopMeta#_get_steps().
  LoopBase.pbar: LoopBase#pbar().
  LoopBase.EXCEPTION_KEY: LoopBase#EXCEPTION_KEY.
  LoopBase.queue: LoopBase#queue.
  LoopMeta.__new__: LoopMeta#__new__().
  LoopBase.LOOP_IDX_KEY: LoopBase#LOOP_IDX_KEY.
  LoopBase.__setstate__: LoopBase#__setstate__().
  LoopBase._pbar: LoopBase#_pbar.
  LoopBase.LoopTerminationError: LoopBase#LoopTerminationError#
  LoopBase.__init__: LoopBase#__init__().
  LoopBase.step_n: LoopBase#step_n.
  LoopBase.semaphores: LoopBase#semaphores.
  LoopBase.tracker: LoopBase#tracker.
  LoopBase.close_pbar: LoopBase#close_pbar().
  LoopBase.truncate_session_folder: LoopBase#truncate_session_folder().
  LoopTrace: LoopTrace#
  LoopTrace.step_idx: LoopTrace#step_idx.
  LoopBase.skip_loop_error_stepname: LoopBase#skip_loop_error_stepname.
  LoopBase.SENTINEL: LoopBase#SENTINEL.
  LoopBase.LoopResumeError: LoopBase#LoopResumeError#
  LoopTrace.end: LoopTrace#end.
  LoopBase.skip_loop_error: LoopBase#skip_loop_error.
  LoopBase.withdraw_loop_error: LoopBase#withdraw_loop_error.
  kill_subprocesses: kill_subprocesses().
  LoopTrace.start: LoopTrace#start.
  LoopBase.__getstate__: LoopBase#__getstate__().
---
# Module: [`rdagent/utils/workflow/loop.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py)

## Classes
### `LoopBase`
- def: [`rdagent/utils/workflow/loop.py:85`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L85) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
- doc: Assumption:
- signature: `class LoopBase:`
- members:
  - `_check_exit_conditions_on_step(self, loop_id: Optional[int] = None, step_id: Optional[int] = None)` — [`L172`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L172) — Check if the loop should continue or terminate. — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `_run_step(self, li: int, force_subproc: bool = False)` — [`L194`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L194) — Execute a single step (next unrun step) in the workflow (async version with force_subproc option). — documented in [rdagent-log-logger](../../../../concepts/rdagent-log-logger.md)
  - `close_pbar(self)` — [`L167`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L167)
  - `dump(self, path: str | Path)` — [`L426`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L426) — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `execute_loop(self)` — [`L336`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L336) — documented in [rdagent-core-conf](../../../../concepts/rdagent-core-conf.md)
  - `get_semaphore(self, step_name: str)` — [`L144`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L144) — documented in [rdagent-core-conf](../../../../concepts/rdagent-core-conf.md)
  - `get_unfinished_loop_cnt(self, next_loop: int)` — [`L137`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L137)
  - `kickoff_loop(self)` — [`L313`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L313) — documented in [rdagent-core-conf](../../../../concepts/rdagent-core-conf.md)
  - `load(cls, path: str | Path, checkout: bool | Path | str = False, replace_timer: bool = True)` — [`L454`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L454) — Load a session from a given path. — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `pbar(self)` — [`L161`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L161) — Progress bar property that initializes itself if it doesn't exist.
  - `run(self, step_n: int | None = None, loop_n: int | None = None, all_duration: str | None = None)` — [`L353`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L353) — Run the workflow loop. — documented in [rdagent-core-conf](../../../../concepts/rdagent-core-conf.md)
  - `truncate_session_folder(self, li: int, si: int)` — [`L434`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L434) — Clear the session folder by removing all session objects after the given loop index (li) and step index (si).
  - `withdraw_loop(self, loop_idx: int)` — [`L406`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L406) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `EXCEPTION_KEY` — [`L104`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L104)
  - `LOOP_IDX_KEY` — [`L105`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L105)
  - `SENTINEL` — [`L106`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L106)
  - `loop_idx` — [`L118`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L118) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `loop_n` — [`L132`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L132)
  - `loop_prev_out` — [`L125`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L125) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `loop_trace` — [`L96`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L96) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `queue` — [`L120`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L120)
  - `semaphores` — [`L135`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L135)
  - `session_folder` — [`L127`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L127) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `skip_loop_error` — [`L98`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L98)
  - `skip_loop_error_stepname` — [`L99`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L99)
  - `step_idx` — [`L119`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L119) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `step_n` — [`L133`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L133)
  - `steps` — [`L95`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L95) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `timer` — [`L128`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L128) — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `tracker` — [`L129`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L129)
  - `withdraw_loop_error` — [`L100`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L100)
- protocol/private: `__getstate__`[`L529`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L529), `__init__`[`L116`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L116), `__setstate__`[`L539`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L539), `_pbar`[`L108`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L108)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`warning`](../../log/logger.md#RDAgentLog.warning), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`error`](../../log/logger.md#RDAgentLog.error), [`RD_Agent_TIMER_wrapper`](../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`log_workflow_state`](tracking.md#WorkflowTracker.log_workflow_state), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`load`](../../scenarios/data_science/loop.md#DataScienceRDLoop.load), [`remain_time`](../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../log/timer.md#RDAgentTimerWrapper.timer), [`started`](../../log/timer.md#RDAgentTimer.started), [`restart_by_remain_time`](../../log/timer.md#RDAgentTimer.restart_by_remain_time), [`LOG_SETTINGS`](../../log/conf.md#LOG_SETTINGS), [`reset`](../../log/timer.md#RDAgentTimer.reset), [`RDAgentTimer`](../../log/timer.md#RDAgentTimer), [`update_remain_time`](../../log/timer.md#RDAgentTimer.update_remain_time), [`replace_timer`](../../log/timer.md#RDAgentTimerWrapper.replace_timer), [`get_max_parallel`](../../core/conf.md#RDAgentSettings.get_max_parallel), [`set_storages_path`](../../log/logger.md#RDAgentLog.set_storages_path), [`tag`](../../log/logger.md#RDAgentLog.tag), [`is_timeout`](../../log/timer.md#RDAgentTimer.is_timeout), [`truncate_storages`](../../log/logger.md#RDAgentLog.truncate_storages), [`dump`](../../scenarios/data_science/loop.md#DataScienceRDLoop.dump), [`dump`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.dump), [`is_force_subproc`](../../core/conf.md#RDAgentSettings.is_force_subproc), [`_check_exit_conditions_on_step`](../../scenarios/data_science/loop.md#DataScienceRDLoop._check_exit_conditions_on_step), [`LoopTerminationError`](loop.md#LoopBase.LoopTerminationError), [`step_semaphore`](../../core/conf.md#RDAgentSettings.step_semaphore), [`trace_path`](../../log/conf.md#LogSettings.trace_path), [`LoopTrace`](loop.md#LoopTrace), [`WorkflowTracker`](tracking.md#WorkflowTracker), [`step_idx`](loop.md#LoopTrace.step_idx), [`LoopResumeError`](loop.md#LoopBase.LoopResumeError), [`end`](loop.md#LoopTrace.end), [`kill_subprocesses`](loop.md#kill_subprocesses)
- used by: [`record`](../../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`async_gen`](../../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`direct_exp_gen`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`trace`](../../scenarios/data_science/loop.md#DataScienceRDLoop.trace), [`log_workflow_state`](tracking.md#WorkflowTracker.log_workflow_state), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`main`](../../app/finetune/llm/loop.md#main), [`direct_exp_gen`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.direct_exp_gen), [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`feedback`](../../components/workflow/rd_loop.md#RDLoop.feedback), [`main`](../../app/data_science/loop.md#main), [`load`](../../scenarios/data_science/loop.md#DataScienceRDLoop.load), [`main`](../../app/kaggle/loop.md#main), [`async_gen`](../../core/proposal.md#ExpGen.async_gen), [`feedback`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.feedback), [`main`](../../app/qlib_rd_loop/factor.md#main), [`main`](../../app/qlib_rd_loop/model.md#main), [`main`](../../app/qlib_rd_loop/quant.md#main), [`main`](../../app/rl/loop.md#main), [`judge_pdf_data_items`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.judge_pdf_data_items), [`feedback`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.feedback), [`feedback`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.feedback), [`record`](../../components/workflow/rd_loop.md#RDLoop.record), [`_get_loop_and_fn_after_hours`](../../log/mle_summary.md#_get_loop_and_fn_after_hours), [`last_step`](../../log/utils/folder.md#last_step), [`main`](../../app/finetune/data_science/loop.md#main), [`get_first_session_file_after_duration`](../../log/utils/folder.md#get_first_session_file_after_duration), [`main`](../../app/qlib_rd_loop/factor_from_report.md#main), [`trace`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.trace), [`trace`](../../components/workflow/rd_loop.md#RDLoop.trace), [`dump`](../../scenarios/data_science/loop.md#DataScienceRDLoop.dump), [`dump`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.dump), [`record`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.record), [`record`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.record), [`trace`](../../app/kaggle/loop.md#KaggleRDLoop.trace), [`loop_trace`](../../log/utils/folder.md#loop_trace), [`session_obj`](../../log/utils/folder.md#session_obj), [`_check_exit_conditions_on_step`](../../scenarios/data_science/loop.md#DataScienceRDLoop._check_exit_conditions_on_step), [`__init__`](tracking.md#WorkflowTracker.__init__)

### `LoopMeta`  ·  implements/extends type
- def: [`rdagent/utils/workflow/loop.py:33`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L33)
- signature: `class LoopMeta(type):`
- members:
  - `__new__(mcs, clsname: str, bases: tuple[type, ...], attrs: dict[str, Any])` — [`L53`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L53) — Create a new class with combined steps from base classes and current class.
  - `_get_steps(bases: tuple[type, ...])` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L36) — Recursively get all the `steps` from the base classes and combine them into a single list.
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`FactorReportLoop`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop)

### `LoopResumeError`  ·  implements/extends Exception
- def: [`rdagent/utils/workflow/loop.py:113`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L113)
- doc: Exception raised when loop conditions indicate the loop should stop all coroutines and resume
- signature: `class LoopResumeError(Exception):`
- used by: [`_run_step`](loop.md#LoopBase._run_step), [`run`](loop.md#LoopBase.run)

### `LoopTerminationError`  ·  implements/extends Exception
- def: [`rdagent/utils/workflow/loop.py:110`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L110)
- doc: Exception raised when loop conditions indicate the loop should terminate
- signature: `class LoopTerminationError(Exception):`
- used by: [`direct_exp_gen`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`run`](loop.md#LoopBase.run), [`_check_exit_conditions_on_step`](loop.md#LoopBase._check_exit_conditions_on_step)

### `LoopTrace`
- def: [`rdagent/utils/workflow/loop.py:78`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L78)
- signature: `class LoopTrace:`
- members:
  - `end` — [`L80`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L80)
  - `start` — [`L79`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L79)
  - `step_idx` — [`L81`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L81)
- used by: [`_run_step`](loop.md#LoopBase._run_step), [`load`](loop.md#LoopBase.load), [`_get_loop_and_fn_after_hours`](../../log/mle_summary.md#_get_loop_and_fn_after_hours), [`last_step`](../../log/utils/folder.md#last_step), [`loop_prev_out`](loop.md#LoopBase.loop_prev_out), [`loop_trace`](loop.md#LoopBase.loop_trace)

## Functions
- `kill_subprocesses()` — [`L545`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/loop.py#L545) — Due to the coroutine-based nature of the workflow, the event loop of the main process can't

