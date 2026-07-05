---
title: 'Module: domains/train_opt/mechanisms/step_calibrator.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/step_calibrator.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.step_calibrator`/
symbols:
  StepSizeCalibrator.record: StepSizeCalibrator#record().
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  StepSizeCalibrator.get_step_size_text: StepSizeCalibrator#get_step_size_text().
  StepSizeCalibrator: StepSizeCalibrator#
  StepSizeCalibrator._compute_relative_change: StepSizeCalibrator#_compute_relative_change().
  logger: logger.
  StepSizeCalibrator.__init__: StepSizeCalibrator#__init__().
---
# Module: [`domains/train_opt/mechanisms/step_calibrator.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py)

## Classes
### `StepSizeCalibrator`
- def: [`domains/train_opt/mechanisms/step_calibrator.py:11`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L11)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L41`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L41) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L52) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L22) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L18`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L18), `_history`[`L20`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L20)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`step_calibrator`](../runner.md#TrainRunner.step_calibrator)

## Module values
- `logger` — [`L8`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/step_calibrator.py#L8)

