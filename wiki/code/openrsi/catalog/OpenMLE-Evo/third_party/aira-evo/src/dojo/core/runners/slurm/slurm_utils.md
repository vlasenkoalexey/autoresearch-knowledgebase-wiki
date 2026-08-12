---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.runners.slurm.slurm_utils`/
symbols:
  JobObserver._observe_job: JobObserver#_observe_job().
  JobObserver._map_slurm_state_to_job_status: JobObserver#_map_slurm_state_to_job_status().
  main: main().
  submit_job: submit_job().
  JobObserver.observe: JobObserver#observe().
  JobStatus: JobStatus#
  JobResult.status: JobResult#status.
  JobResult: JobResult#
  JobObserver._observing_tasks: JobObserver#_observing_tasks.
  JobObserver.wait: JobObserver#wait().
  JobStatus.FAILED: JobStatus#FAILED.
  JobObserver: JobObserver#
  get_logs: get_logs().
  log: log.
  JobStatus.COMPLETED: JobStatus#COMPLETED.
  JobStatus.CANCELLED: JobStatus#CANCELLED.
  JobStatus.UNKNOWN: JobStatus#UNKNOWN.
  JobResult.job_id: JobResult#job_id.
  JobResult.metadata: JobResult#metadata.
  JobResult.log_out: JobResult#log_out.
  JobResult.log_err: JobResult#log_err.
  JobObserver.shared: JobObserver#shared.
  submit_job.job_function: submit_job().job_function().
  main._wrapper: main()._wrapper().
  JobObserver.__init__: JobObserver#__init__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py)

## Classes
### `JobObserver`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py:39`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L39)
- doc: Manages a pool of asyncio tasks for observing submitit job status.
- signature: `class JobObserver:`
- members:
  - `_map_slurm_state_to_job_status(self, slurm_state: str, job: submitit.Job)` — [`L113`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L113) — Convert a Slurm or Submitit job state to simpler JobStatus states
  - `_observe_job(self, job: submitit.Job, poll_interval=30, focus_rank: Optional[int] = None, callback: Optional[Callable[[JobResult], None]] = None, metadata: Optional[dict[str, str | int | float, bool]] = None)` — [`L78`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L78) — Loop that periodically checks the job until it's done,
  - `observe(self, job: submitit.Job, metadata: Optional[dict[str, str | int | float, bool]] = None, callback: Optional[Callable[[JobResult], None]] = None, focus_rank: Optional[int] = None, poll_interval: int = 10)` — [`L48`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L48) — Observe the status of a submitit job, and execute a callback when finished.
  - `wait(self)` — [`L73`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L73) — Returns only when all observed jobs and their callbacks are complete.
  - `shared` — [`L42`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L42)
- protocol/private: `__init__`[`L44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L44), `_observing_tasks`[`L46`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L46)
- uses (calls/refs, reference-scoped): [`JobStatus`](slurm_utils.md#JobStatus), [`status`](slurm_utils.md#JobResult.status), [`JobResult`](slurm_utils.md#JobResult), [`FAILED`](slurm_utils.md#JobStatus.FAILED), [`get_logs`](slurm_utils.md#get_logs), [`CANCELLED`](slurm_utils.md#JobStatus.CANCELLED), [`COMPLETED`](slurm_utils.md#JobStatus.COMPLETED), [`UNKNOWN`](slurm_utils.md#JobStatus.UNKNOWN), [`job_id`](slurm_utils.md#JobResult.job_id), [`log_err`](slurm_utils.md#JobResult.log_err), [`log_out`](slurm_utils.md#JobResult.log_out), [`metadata`](slurm_utils.md#JobResult.metadata)

### `JobResult`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py:29`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L29)
- doc: Aggregate information about the finished job.
- signature: `class JobResult:`
- members:
  - `job_id` — [`L32`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L32)
  - `log_err` — [`L36`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L36)
  - `log_out` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L35)
  - `metadata` — [`L33`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L33)
  - `status` — [`L34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L34)
- uses (calls/refs, reference-scoped): [`JobStatus`](slurm_utils.md#JobStatus)
- used by: [`_observe_job`](slurm_utils.md#JobObserver._observe_job), [`observe`](slurm_utils.md#JobObserver.observe)

### `JobStatus`  ·  implements/extends Enum
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py:21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L21)
- signature: `class JobStatus(Enum):`
- members:
  - `CANCELLED` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L24)
  - `COMPLETED` — [`L22`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L22)
  - `FAILED` — [`L23`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L23)
  - `UNKNOWN` — [`L25`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L25)
- used by: [`_map_slurm_state_to_job_status`](slurm_utils.md#JobObserver._map_slurm_state_to_job_status), [`status`](slurm_utils.md#JobResult.status)

## Functions
- `_wrapper(job, data_dict)` — [`L270`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L270)
- `get_logs(job: submitit.Job, focus_rank: Optional[int] = None)` — [`L135`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L135) — Gathers job stdout/stderr logs as lists of strings.
- `job_function()` — [`L198`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L198)
- `main()` — [`L213`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L213)
- `submit_job(command: str, slurm_job_name: str, working_dir: str = ".", log_dir="slurm_logs", env_vars: Optional[dict[str, str]] = None, **slurm_kwargs)` — [`L163`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L163) — Launches a SLURM job using submitit with the specified arguments.

## Module values
- `log` — [`L18`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/runners/slurm/slurm_utils.py#L18)

