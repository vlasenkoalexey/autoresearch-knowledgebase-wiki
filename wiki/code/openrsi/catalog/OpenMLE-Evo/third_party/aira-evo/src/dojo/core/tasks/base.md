---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.tasks.base`/Task#
symbols:
  Task.cfg: cfg.
  Task.logger: logger.
  Task: ''
  Task.__init__: __init__().
  Task.prepare: prepare().
  Task.step_task: step_task().
  Task.evaluate_fitness: evaluate_fitness().
  Task.close: close().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py)

## Classes
### `Task`  ·  implements/extends ABC
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py:19`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L19)
- doc: Abstract base class representing a Task.
- signature: `class Task(ABC):`
- members:
  - `__init__(self, cfg: TaskConfig)` — [`L32`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L32) — Initialize a Task instance.
  - `close(self, state: Dict)` — [`L97`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L97) — Perform cleanup and close any resources associated with the task.
  - `evaluate_fitness(self, solution: Optional[Dict] = None, state: Optional[Dict] = None, interpreter: Optional[Dict] = None, aux_info: Dict[str, Any] = None)` — [`L75`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L75) — Evaluates how good (or correct) the provided solution is for this task.
  - `prepare(self, **task_args: Optional[Dict])` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L44) — Prepares everything for the task execution to start (e.g., copies data to the agent's workspace).
  - `step_task(self, state: Dict, action: Any)` — [`L59`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L59) — Execute a single step of the task using the provided action.
  - `cfg` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L40)
  - `logger` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/tasks/base.py#L41)
- uses (calls/refs, reference-scoped): [`step_task`](../../tasks/mlebench/task.md#MLEBenchTask.step_task), [`evaluate_fitness`](../../tasks/mlebench/task.md#MLEBenchTask.evaluate_fitness), [`prepare`](../../tasks/mlebench/task.md#MLEBenchTask.prepare), [`get_logger`](../../utils/logger.md#get_logger), [`TaskConfig`](../../config_dataclasses/task/base.md#TaskConfig), [`MLEBenchTask`](../../tasks/mlebench/task.md#MLEBenchTask), [`close`](../../tasks/mlebench/task.md#MLEBenchTask.close)
- used by: [`step_task`](../../tasks/mlebench/task.md#MLEBenchTask.step_task), [`evaluate_fitness`](../../tasks/mlebench/task.md#MLEBenchTask.evaluate_fitness), [`prepare`](../../tasks/mlebench/task.md#MLEBenchTask.prepare), [`instructions`](../../tasks/mlebench/task.md#MLEBenchTask.instructions), [`competition`](../../tasks/mlebench/task.md#MLEBenchTask.competition), [`task_description`](../../tasks/mlebench/task.md#MLEBenchTask.task_description), [`__init__`](../../tasks/mlebench/task.md#MLEBenchTask.__init__), [`MLEBenchTask`](../../tasks/mlebench/task.md#MLEBenchTask), [`private_dir`](../../tasks/mlebench/task.md#MLEBenchTask.private_dir), [`public_dir`](../../tasks/mlebench/task.md#MLEBenchTask.public_dir)

