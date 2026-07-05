---
title: 'Module: rdagent/utils/workflow/misc.py'
type: catalog
provenance: extracted
module: rdagent/utils/workflow/misc.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.workflow.misc`/
symbols:
  wait_retry: wait_retry().
  wait_retry.decorator: wait_retry().decorator().
  ASpecificRet: ASpecificRet.
  wait_retry.decorator.wrapper: wait_retry().decorator().wrapper().
---
# Module: [`rdagent/utils/workflow/misc.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/misc.py)

## Functions
- `decorator(f: Callable[..., ASpecificRet])` — [`L35`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/misc.py#L35)
- `wait_retry(retry_n: int = 3, sleep_time: int = 1, transform_args_fn: Callable[[tuple, dict], tuple[tuple, dict]] | None = None)` — [`L8`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/misc.py#L8) — Decorator to wait and retry the function for retry_n times.
- `wrapper(*args: Any, **kwargs: Any)` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/misc.py#L36)

## Module values
- `ASpecificRet` — [`L5`](../../../../../../../raw/code/rd-agent/rdagent/utils/workflow/misc.py#L5)

