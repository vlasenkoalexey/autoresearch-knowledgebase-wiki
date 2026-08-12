---
title: 'Module: src/arc3/logwriter.py'
type: catalog
provenance: extracted
module: src/arc3/logwriter.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.logwriter`/
symbols:
  _finish: _finish().
  LogWriter.append_step: LogWriter#append_step().
  parse_log: parse_log().
  StepRecord: StepRecord#
  StepRecord.action: StepRecord#action.
  StepRecord.levels_completed: StepRecord#levels_completed.
  action_name: action_name().
  StepRecord.step: StepRecord#step.
  StepRecord.frames: StepRecord#frames.
  StepRecord.state: StepRecord#state.
  StepRecord.x: StepRecord#x.
  StepRecord.y: StepRecord#y.
  LogWriter._append: LogWriter#_append().
  diff_boards: diff_boards().
  BoardDiff: BoardDiff.
  LogWriter.append_plan: LogWriter#append_plan().
  _NAME_TO_ID: _NAME_TO_ID.
  format_diff: format_diff().
  StepRecord.win_levels: StepRecord#win_levels.
  StepRecord.available_actions: StepRecord#available_actions.
  LogWriter.path: LogWriter#path.
  _StepBuilder: _StepBuilder#
  LogWriter.__init__: LogWriter#__init__().
  ACTION_NAMES: ACTION_NAMES.
  LogWriter: LogWriter#
  _StepBuilder.step: _StepBuilder#step.
  _StepBuilder.action: _StepBuilder#action.
  _StepBuilder.x: _StepBuilder#x.
  _StepBuilder.y: _StepBuilder#y.
  _StepBuilder.frames: _StepBuilder#frames.
  _StepBuilder.levels_completed: _StepBuilder#levels_completed.
  _StepBuilder.win_levels: _StepBuilder#win_levels.
  _StepBuilder.state: _StepBuilder#state.
  _StepBuilder.available_actions: _StepBuilder#available_actions.
---
# Module: [`src/arc3/logwriter.py`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py)

## Classes
### `LogWriter`
- def: [`src/arc3/logwriter.py:51`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L51)
- doc: Append-only writer for the per-run game log.
- signature: `class LogWriter:`
- members:
  - `append_plan(self, invocation: int, plan_text: str)` — [`L78`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L78) — Append the agent's stated plan after an invocation.
  - `append_step(self, record: StepRecord, *, diff: BoardDiff | None = None)` — [`L59`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L59) — Append one step section. — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `path` — [`L55`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L55)
- protocol/private: `__init__`[`L54`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L54), `_append`[`L83`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L83)
- uses (calls/refs, reference-scoped): [`StepRecord`](logwriter.md#StepRecord), [`action`](logwriter.md#StepRecord.action), [`levels_completed`](logwriter.md#StepRecord.levels_completed), [`action_name`](logwriter.md#action_name), [`frames`](logwriter.md#StepRecord.frames), [`state`](logwriter.md#StepRecord.state), [`step`](logwriter.md#StepRecord.step), [`x`](logwriter.md#StepRecord.x), [`y`](logwriter.md#StepRecord.y), [`BoardDiff`](logwriter.md#BoardDiff), [`format_diff`](logwriter.md#format_diff), [`available_actions`](logwriter.md#StepRecord.available_actions), [`win_levels`](logwriter.md#StepRecord.win_levels)
- used by: [`_accept`](runner.md#GameRunner._accept), [`_log_frame`](runner.md#GameRunner._log_frame), [`log`](runner.md#GameRunner.log)

### `StepRecord`
- def: [`src/arc3/logwriter.py:37`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L37) — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
- doc: One environment step as written to and parsed from the log.
- signature: `class StepRecord:`
- members:
  - `action` — [`L41`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L41)
  - `available_actions` — [`L46`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L46)
  - `frames` — [`L42`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L42) — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `levels_completed` — [`L43`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L43) — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `state` — [`L45`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L45) — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `step` — [`L40`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L40)
  - `win_levels` — [`L44`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L44)
  - `x` — [`L47`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L47)
  - `y` — [`L48`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L48)
- used by: [`_restore`](runner.md#GameRunner._restore), [`_finish`](logwriter.md#_finish), [`_log_frame`](runner.md#GameRunner._log_frame), [`append_step`](logwriter.md#LogWriter.append_step), [`parse_log`](logwriter.md#parse_log), [`_seed_level_signals`](runner.md#GameRunner._seed_level_signals)

### `_StepBuilder`
- def: [`src/arc3/logwriter.py:89`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L89)
- signature: `class _StepBuilder:`
- members:
  - `action` — [`L91`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L91)
  - `available_actions` — [`L98`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L98)
  - `frames` — [`L94`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L94)
  - `levels_completed` — [`L95`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L95)
  - `state` — [`L97`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L97)
  - `step` — [`L90`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L90)
  - `win_levels` — [`L96`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L96)
  - `x` — [`L92`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L92)
  - `y` — [`L93`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L93)
- used by: [`_finish`](logwriter.md#_finish), [`parse_log`](logwriter.md#parse_log)

## Functions
- `_finish(builder: _StepBuilder)` — [`L158`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L158) — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
- `action_name(action_id: int)` — [`L31`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L31) — Map an environment action id to its log name.
- `diff_boards(before: list[list[int]], after: list[list[int]])` — [`L172`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L172) — Return changed cells as (x, y, old, new), with x=column and y=row.
- `format_diff(diff: BoardDiff)` — [`L184`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L184) — Render the derived settled-board diff line for log.txt. — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
- `parse_log(text: str)` — [`L104`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L104) — Parse step sections back out of a log; derived [DIFF] and [PLAN] blocks are skipped. — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)

## Module values
- `ACTION_NAMES` — [`L27`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L27)
- `BoardDiff` — [`L28`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L28)
- `_NAME_TO_ID` — [`L101`](../../../../../../raw/code/Retrodict/src/arc3/logwriter.py#L101)

