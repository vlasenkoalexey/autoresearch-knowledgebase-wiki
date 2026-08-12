---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.tasks.mlebench.task`/
symbols:
  MLEBenchTask.step_task: MLEBenchTask#step_task().
  MLEBenchTask.evaluate_fitness: MLEBenchTask#evaluate_fitness().
  MLEBenchTask._submission_file_path: MLEBenchTask#_submission_file_path.
  MLEBenchTask.prepare: MLEBenchTask#prepare().
  MLEBenchTask.instructions: MLEBenchTask#instructions.
  MLEBenchTask.competition: MLEBenchTask#competition.
  MLEBenchTask.task_description: MLEBenchTask#task_description.
  MLEBenchTask.__init__: MLEBenchTask#__init__().
  MLEBenchTask: MLEBenchTask#
  MLEBenchTask.instructions_path: MLEBenchTask#instructions_path.
  MLEBenchTask.public_dir: MLEBenchTask#public_dir.
  MLEBenchTask.private_dir: MLEBenchTask#private_dir.
  parse_report: parse_report().
  MLEBenchTask._solution_script: MLEBenchTask#_solution_script.
  MLEBenchTask.task_src_path: MLEBenchTask#task_src_path.
  MLEBenchTask.close: MLEBenchTask#close().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py)

## Classes
### `MLEBenchTask`  ·  implements/extends Task
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py:41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L41)
- doc: Represents an MLE Bench task.
- signature: `class MLEBenchTask(Task):`
- members:
  - `__init__(self, cfg: MLEBenchTaskConfig)` — [`L57`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L57) — Initialize the MLEBenchTask.
  - `close(self, state)` — [`L205`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L205)
  - `evaluate_fitness(self, solution: Optional[Any] = None, state: Optional[Dict[str, Any]] = None, interpreter: Optional[Interpreter] = None, aux_info: Optional[Dict[str, Any]] = None)` — [`L177`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L177)
  - `prepare(self, **task_args)` — [`L84`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L84)
  - `step_task(self, state: Dict[str, Any], action: Any)` — [`L99`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L99) — Execute a single step of the task.
  - `competition` — [`L78`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L78)
  - `instructions` — [`L69`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L69)
  - `instructions_path` — [`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L68)
  - `private_dir` — [`L82`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L82)
  - `public_dir` — [`L81`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L81)
  - `task_description` — [`L74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L74)
  - `task_src_path` — [`L67`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L67)
- protocol/private: `_solution_script`[`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L54), `_submission_file_path`[`L55`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L55)
- uses (calls/refs, reference-scoped): [`get_empty`](../../core/interpreters/base.md#ExecutionResult.get_empty), [`ExecutionResult`](../../core/interpreters/base.md#ExecutionResult), [`EXECUTION_OUTPUT`](../../core/tasks/constants.md#EXECUTION_OUTPUT), [`cfg`](../../core/tasks/base.md#Task.cfg), [`VALIDATION_FITNESS`](../../core/tasks/constants.md#VALIDATION_FITNESS), [`AUX_EVAL_INFO`](../../core/tasks/constants.md#AUX_EVAL_INFO), [`VALID_SOLUTION`](../../core/tasks/constants.md#VALID_SOLUTION), [`logger`](../../core/tasks/base.md#Task.logger), [`TASK_DESCRIPTION`](../../core/tasks/constants.md#TASK_DESCRIPTION), [`VALID_SOLUTION_FEEDBACK`](../../core/tasks/constants.md#VALID_SOLUTION_FEEDBACK), [`exec_time`](../../core/interpreters/base.md#ExecutionResult.exec_time), [`exit_code`](../../core/interpreters/base.md#ExecutionResult.exit_code), [`extract_code`](../../utils/code_parsing.md#extract_code), [`name`](../../config_dataclasses/task/base.md#TaskConfig.name), [`term_out`](../../core/interpreters/base.md#ExecutionResult.term_out), [`Interpreter`](../../core/interpreters/base.md#Interpreter), [`MLEBenchTaskConfig`](../../config_dataclasses/task/mlebench.md#MLEBenchTaskConfig), [`run`](../../core/interpreters/base.md#Interpreter.run), [`Task`](../../core/tasks/base.md#Task), [`evaluate_submission`](evaluate.md#evaluate_submission), [`__init__`](../../core/tasks/base.md#Task.__init__), [`TEST_FITNESS`](../../core/tasks/constants.md#TEST_FITNESS), [`timed_out`](../../core/interpreters/base.md#ExecutionResult.timed_out), [`parse_report`](task.md#parse_report), [`is_lower_better`](evaluate.md#is_lower_better)
- used by: [`_materialize`](../../config_dataclasses/task/__init__.md#_LazyTaskMap._materialize), [`Task`](../../core/tasks/base.md#Task), [`close`](../../core/tasks/base.md#Task.close), [`evaluate_fitness`](../../core/tasks/base.md#Task.evaluate_fitness), [`prepare`](../../core/tasks/base.md#Task.prepare), [`step_task`](../../core/tasks/base.md#Task.step_task)

## Functions
- `parse_report(report: Dict[str, Any])` — [`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/tasks/mlebench/task.py#L31)

