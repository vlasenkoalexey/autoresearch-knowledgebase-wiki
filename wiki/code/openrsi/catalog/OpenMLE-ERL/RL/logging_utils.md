---
title: 'Module: OpenMLE-ERL/RL/logging_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/logging_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.logging_utils`/
symbols:
  TrainingLogger.log_sample: TrainingLogger#log_sample().
  TrainingLogger.init_csv: TrainingLogger#init_csv().
  _global_logger: _global_logger.
  get_logger: get_logger().
  init_logger: init_logger().
  TrainingLogger.group_logging_buffer: TrainingLogger#group_logging_buffer.
  TrainingLogger.run_dir: TrainingLogger#run_dir.
  TrainingLogger.csv_log_file: TrainingLogger#csv_log_file.
  TrainingLogger.log_group_data: TrainingLogger#log_group_data().
  TrainingLogger.n_samples_per_prompt: TrainingLogger#n_samples_per_prompt.
  TrainingLogger: TrainingLogger#
  TrainingLogger.get_run_dir: TrainingLogger#get_run_dir().
  TrainingLogger.csv_initialized: TrainingLogger#csv_initialized.
  EVAL_GROUP_SIZE: EVAL_GROUP_SIZE.
  TrainingLogger.group_logging_lock: TrainingLogger#group_logging_lock.
  TrainingLogger.__init__: TrainingLogger#__init__().
---
# Module: [`OpenMLE-ERL/RL/logging_utils.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py)

## Classes
### `TrainingLogger`
- def: [`OpenMLE-ERL/RL/logging_utils.py:16`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L16)
- doc: Manages logging of training data to CSV files.
- signature: `class TrainingLogger:`
- members:
  - `__init__(self, log_file_name: str = None, n_samples_per_prompt: int = 8)` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L19) — Initialize training logger.
  - `get_run_dir(self)` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L88) — Get the run directory path.
  - `init_csv(self)` — [`L44`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L44) — Initialize CSV log file with headers.
  - `log_group_data(self, group_key: str, group_data: List[Dict], group_id: int, group_size: int)` — [`L92`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L92) — Write a complete group's data to CSV.
  - `log_sample(self, sample, score: Optional[float], reward: float, static_base_reward: Optional[float], base_reward: float, result_info: Any, code: str, raw_text: str = "", parent_id: Optional[int] = None, parent_code: str = "", parent_score: Optional[float] = None, parent_reward: Optional[float] = None, mode: str = "draft", hack: int = 0, code_category: str = "valid", static_raw_reward: Optional[float] = None, static_mercy_raw_reward: Optional[float] = None, dynamic_raw_reward: Optional[float] = None, exploit_coefficient: Optional[float] = None, explore_coefficient: Optional[float] = None, cooling_coefficient: Optional[float] = None)` — [`L239`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L239) — Collect sample information and write to CSV when a group is complete. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
  - `csv_initialized` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L38)
  - `csv_log_file` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L37)
  - `group_logging_buffer` — [`L41`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L41)
  - `group_logging_lock` — [`L42`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L42)
  - `n_samples_per_prompt` — [`L27`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L27)
  - `run_dir` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L31)
- uses (calls/refs, reference-scoped): [`EVAL_GROUP_SIZE`](logging_utils.md#EVAL_GROUP_SIZE)
- used by: [`reward_func`](generate_mle.md#reward_func), [`get_logger`](logging_utils.md#get_logger), [`init_logger`](logging_utils.md#init_logger)

## Functions
- `get_logger()` — [`L359`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L359) — Get or create the global logger instance.
- `init_logger(log_file_name: str = None, n_samples_per_prompt: int = 8)` — [`L368`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L368) — Initialize the global logger.

## Module values
- `EVAL_GROUP_SIZE` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L13)
- `_global_logger` — [`L356`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/logging_utils.py#L356)

