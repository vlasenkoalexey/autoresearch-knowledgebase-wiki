---
title: 'Module: rdagent/app/qlib_rd_loop/factor.py'
type: catalog
provenance: extracted
module: rdagent/app/qlib_rd_loop/factor.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.qlib_rd_loop.factor`/
symbols:
  main: main().
  FactorRDLoop.running: FactorRDLoop#running().
  FactorRDLoop: FactorRDLoop#
  FactorRDLoop.skip_loop_error: FactorRDLoop#skip_loop_error.
  FactorRDLoop.skip_loop_error_stepname: FactorRDLoop#skip_loop_error_stepname.
---
# Module: [`rdagent/app/qlib_rd_loop/factor.py`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py)

## Classes
### `FactorRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/app/qlib_rd_loop/factor.py:17`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py#L17)
- signature: `class FactorRDLoop(RDLoop):`
- members:
  - `running(self, prev_out: dict[str, Any])` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py#L21)
  - `skip_loop_error` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py#L18)
  - `skip_loop_error_stepname` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py#L19)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`CoderError`](../../core/exception.md#CoderError), [`error`](../../log/logger.md#RDAgentLog.error), [`develop`](../../core/developer.md#Developer.develop), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`FactorEmptyError`](../../core/exception.md#FactorEmptyError), [`runner`](../../components/workflow/rd_loop.md#RDLoop.runner), [`FactorReportLoop`](factor_from_report.md#FactorReportLoop)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`main`](factor.md#main), [`running`](../../components/workflow/rd_loop.md#RDLoop.running), [`FactorReportLoop`](factor_from_report.md#FactorReportLoop)

## Functions
- `main(path: Optional[str] = None, step_n: Optional[int] = None, loop_n: Optional[int] = None, all_duration: str | None = None, checkout: bool = True, checkout_path: Optional[str] = None, base_features_path: Optional[str] = None, **kwargs)` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor.py#L30) — Auto R&D Evolving loop for fintech factors. — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)

