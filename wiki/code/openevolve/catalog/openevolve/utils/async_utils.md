---
title: 'Module: openevolve/utils/async_utils.py'
type: catalog
provenance: extracted
module: openevolve/utils/async_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.utils.async_utils`/
symbols:
  TaskPool.tasks: TaskPool#tasks.
  TaskPool.semaphore: TaskPool#semaphore().
  TaskPool.create_task: TaskPool#create_task().
  run_in_executor: run_in_executor().
  logger: logger.
  gather_with_concurrency: gather_with_concurrency().
  retry_async: retry_async().
  TaskPool.run: TaskPool#run().
  TaskPool: TaskPool#
  TaskPool._semaphore: TaskPool#_semaphore.
  run_with_timeout: run_with_timeout().
  run_sync_with_timeout: run_sync_with_timeout().
  TaskPool.wait_all: TaskPool#wait_all().
  TaskPool.cancel_all: TaskPool#cancel_all().
  run_in_executor.wrapper: run_in_executor().wrapper().
  gather_with_concurrency.sem_task: gather_with_concurrency().sem_task().
  TaskPool.max_concurrency: TaskPool#max_concurrency.
  T: T.
  TaskPool.__init__: TaskPool#__init__().
---
# Module: [`openevolve/utils/async_utils.py`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py)

## Classes
### `TaskPool`
- def: [`openevolve/utils/async_utils.py:167`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L167)
- doc: A simple task pool for managing and limiting concurrent tasks
- signature: `class TaskPool:`
- members:
  - `cancel_all(self)` — [`L221`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L221) — Cancel all tasks in the pool
  - `create_task(self, coro: Callable, *args: Any, **kwargs: Any)` — [`L199`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L199) — Create and track a task in the pool
  - `run(self, coro: Callable, *args: Any, **kwargs: Any)` — [`L184`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L184) — Run a coroutine in the pool
  - `semaphore(self)` — [`L178`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L178) — Lazy-initialize the semaphore when first needed
  - `wait_all(self)` — [`L216`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L216) — Wait for all tasks in the pool to complete
  - `max_concurrency` — [`L173`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L173)
  - `tasks` — [`L175`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L175)
- protocol/private: `__init__`[`L172`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L172), `_semaphore`[`L174`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L174)
- used by: [`task_pool`](../evaluator.md#Evaluator.task_pool), [`evaluate_multiple`](../evaluator.md#Evaluator.evaluate_multiple)

## Functions
- `gather_with_concurrency(n: int, *tasks: asyncio.Future, return_exceptions: bool = False)` — [`L89`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L89) — Run tasks with a concurrency limit
- `retry_async(coro: Callable, *args: Any, retries: int = 3, delay: float = 1, backoff: float = 2, exceptions: Union[Exception, tuple] = Exception, **kwargs: Any)` — [`L114`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L114) — Retry an async function with exponential backoff
- `run_in_executor(f: Callable)` — [`L16`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L16) — Decorator to run a synchronous function in an executor
- `run_sync_with_timeout(func: Callable, timeout: float, *args: Any, timeout_error_value: Any = None, **kwargs: Any)` — [`L61`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L61) — Run a synchronous function in an executor with a timeout
- `run_with_timeout(coro: Callable, timeout: float, *args: Any, timeout_error_value: Any = None, **kwargs: Any)` — [`L35`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L35) — Run a coroutine with a timeout, returning a default value on timeout
- `sem_task(task: asyncio.Future)` — [`L105`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L105)
- `wrapper(*args: Any, **kwargs: Any)` — [`L28`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L28)

## Module values
- `T` — [`L13`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L13)
- `logger` — [`L11`](../../../../../../raw/code/openevolve/openevolve/utils/async_utils.py#L11)

