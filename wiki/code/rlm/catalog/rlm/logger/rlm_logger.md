---
title: 'Module: rlm/logger/rlm_logger.py'
type: catalog
provenance: extracted
module: rlm/logger/rlm_logger.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.logger.rlm_logger`/RLMLogger#
symbols:
  RLMLogger: ''
  RLMLogger.log: log().
  RLMLogger.log_metadata: log_metadata().
  RLMLogger.log_file_path: log_file_path.
  RLMLogger.get_trajectory: get_trajectory().
  RLMLogger.clear_iterations: clear_iterations().
  RLMLogger._run_metadata: _run_metadata.
  RLMLogger._iteration_count: _iteration_count.
  RLMLogger._save_to_disk: _save_to_disk.
  RLMLogger._iterations: _iterations.
  RLMLogger.iteration_count: iteration_count().
  RLMLogger._metadata_logged: _metadata_logged.
  RLMLogger.__init__: __init__().
  RLMLogger.log_dir: log_dir.
---
# Module: [`rlm/logger/rlm_logger.py`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py)

## Classes
### `RLMLogger`
- def: [`rlm/logger/rlm_logger.py:16`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L16) — documented in [rlm-logger-rlm_logger](../../../concepts/rlm-logger-rlm_logger.md)
- doc: Captures trajectory (run metadata + iterations) for each completion.
- signature: `class RLMLogger:`
- members:
  - `clear_iterations(self)` — [`L75`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L75) — Reset iterations for the next completion (trajectory is per completion).
  - `get_trajectory(self)` — [`L80`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L80) — Return captured run_metadata + iterations for the current completion, or None if no metadata yet.
  - `iteration_count(self)` — [`L90`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L90)
  - `log(self, iteration: RLMIteration)` — [`L59`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L59) — Capture one iteration (and optionally append to file). — documented in [rlm-logger-rlm_logger](../../../concepts/rlm-logger-rlm_logger.md)
  - `log_metadata(self, metadata: RLMMetadata)` — [`L41`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L41) — Capture run metadata (and optionally write to file). — documented in [rlm-logger-rlm_logger](../../../concepts/rlm-logger-rlm_logger.md)
  - `log_dir` — [`L28`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L28)
  - `log_file_path` — [`L29`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L29) — documented in [rlm-logger-rlm_logger](../../../concepts/rlm-logger-rlm_logger.md)
- protocol/private: `__init__`[`L26`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L26), `_iteration_count`[`L38`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L38), `_iterations`[`L37`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L37), `_metadata_logged`[`L39`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L39), `_run_metadata`[`L36`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L36), `_save_to_disk`[`L27`](../../../../../../raw/code/rlm/rlm/logger/rlm_logger.py#L27)
- uses (calls/refs, reference-scoped): [`RLMIteration`](../core/types.md#RLMIteration), [`to_dict`](../core/types.md#RLMMetadata.to_dict), [`to_dict`](../core/types.md#RLMIteration.to_dict), [`RLMMetadata`](../core/types.md#RLMMetadata)
- used by: [`completion`](../core/rlm.md#RLM.completion), [`_subcall`](../core/rlm.md#RLM._subcall), [`_persistent_env`](../core/rlm.md#RLM._persistent_env), [`_default_answer`](../core/rlm.md#RLM._default_answer), [`__init__`](../core/rlm.md#RLM.__init__)  (14 test-only)

