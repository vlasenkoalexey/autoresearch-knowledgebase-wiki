---
title: 'Module: rdagent/app/qlib_rd_loop/model.py'
type: catalog
provenance: extracted
module: rdagent/app/qlib_rd_loop/model.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.qlib_rd_loop.model`/
symbols:
  main: main().
  ModelRDLoop: ModelRDLoop#
  ModelRDLoop.skip_loop_error: ModelRDLoop#skip_loop_error.
---
# Module: [`rdagent/app/qlib_rd_loop/model.py`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/model.py)

## Classes
### `ModelRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/app/qlib_rd_loop/model.py:14`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/model.py#L14)
- signature: `class ModelRDLoop(RDLoop):`
- members:
  - `skip_loop_error` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/model.py#L15)
- uses (calls/refs, reference-scoped): [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`ModelEmptyError`](../../core/exception.md#ModelEmptyError)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`main`](model.md#main)

## Functions
- `main(path=None, step_n: int | None = None, loop_n: int | None = None, all_duration: str | None = None, checkout: bool = True, base_features_path: str | None = None, **kwargs)` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/model.py#L18) — Auto R&D Evolving loop for fintech models — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)

