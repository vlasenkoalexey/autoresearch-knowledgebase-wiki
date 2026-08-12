---
title: 'Module: tests/test_logwriter.py'
type: catalog
provenance: extracted
module: tests/test_logwriter.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_logwriter`/
symbols:
  test_log_round_trips_scripted_random_play_on_ls20: test_log_round_trips_scripted_random_play_on_ls20().
  test_parse_log_skips_diff_lines_from_shared_golden_fixture: test_parse_log_skips_diff_lines_from_shared_golden_fixture().
  record_from_frame: record_from_frame().
  FIXTURE_LOG: FIXTURE_LOG.
  test_multi_frame_animation_step_round_trips: test_multi_frame_animation_step_round_trips().
  test_plan_blocks_are_skipped_by_the_parser: test_plan_blocks_are_skipped_by_the_parser().
  test_diff_boards_uses_column_row_ordering: test_diff_boards_uses_column_row_ordering().
  test_append_step_writes_listed_none_and_summarized_diffs: test_append_step_writes_listed_none_and_summarized_diffs().
  test_format_diff_threshold: test_format_diff_threshold().
---
# Module: [`tests/test_logwriter.py`](../../../../../raw/code/Retrodict/tests/test_logwriter.py)

## Functions
- `record_from_frame(step: int, action: str, frame, x: int | None = None, y: int | None = None)` — [`L13`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L13) — Build the expected StepRecord from what the environment returned.
- `test_append_step_writes_listed_none_and_summarized_diffs(tmp_path: Path)` — [`L115`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L115)
- `test_diff_boards_uses_column_row_ordering()` — [`L108`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L108)
- `test_format_diff_threshold()` — [`L138`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L138)
- `test_log_round_trips_scripted_random_play_on_ls20(tmp_path: Path, ls20_env)` — [`L28`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L28) — A scripted random agent's log parses back to the exact env observations.
- `test_multi_frame_animation_step_round_trips(tmp_path: Path)` — [`L61`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L61) — A step with intermediate animation frames is labeled and parses back exactly.
- `test_parse_log_skips_diff_lines_from_shared_golden_fixture()` — [`L146`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L146)
- `test_plan_blocks_are_skipped_by_the_parser(tmp_path: Path)` — [`L90`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L90)

## Module values
- `FIXTURE_LOG` — [`L10`](../../../../../raw/code/Retrodict/tests/test_logwriter.py#L10)

