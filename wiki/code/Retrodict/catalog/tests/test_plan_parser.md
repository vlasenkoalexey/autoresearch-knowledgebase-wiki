---
title: 'Module: tests/test_plan_parser.py'
type: catalog
provenance: extracted
module: tests/test_plan_parser.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_plan_parser`/
symbols:
  AVAILABLE: AVAILABLE.
  wrap: wrap().
  test_valid_plan_parses: test_valid_plan_parses().
  test_json_code_fence_is_tolerated: test_json_code_fence_is_tolerated().
  test_malformed_json_is_an_error: test_malformed_json_is_an_error().
  test_trailing_bracket_after_object_is_tolerated: test_trailing_bracket_after_object_is_tolerated().
  test_trailing_prose_after_object_is_tolerated: test_trailing_prose_after_object_is_tolerated().
  test_truncated_output_mentions_the_cutoff: test_truncated_output_mentions_the_cutoff().
  test_unavailable_action_is_an_error: test_unavailable_action_is_an_error().
  test_empty_plan_is_an_error: test_empty_plan_is_an_error().
  test_action6_missing_coordinates_is_an_error: test_action6_missing_coordinates_is_an_error().
  test_action6_out_of_bounds_is_an_error: test_action6_out_of_bounds_is_an_error().
  test_action6_non_integer_coordinates_are_an_error: test_action6_non_integer_coordinates_are_an_error().
  test_duplicate_actions_blocks_use_the_last_one: test_duplicate_actions_blocks_use_the_last_one().
  test_expectations_parse_to_tuples: test_expectations_parse_to_tuples().
  test_expect_must_be_cells_of_three_ints: test_expect_must_be_cells_of_three_ints().
  test_expect_ranges_are_enforced: test_expect_ranges_are_enforced().
  test_expect_levels_must_be_a_non_negative_integer: test_expect_levels_must_be_a_non_negative_integer().
  test_plan_longer_than_remaining_budget_is_clamped: test_plan_longer_than_remaining_budget_is_clamped().
  test_missing_block_is_an_error: test_missing_block_is_an_error().
---
# Module: [`tests/test_plan_parser.py`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py)

## Functions
- `test_action6_missing_coordinates_is_an_error()` — [`L72`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L72)
- `test_action6_non_integer_coordinates_are_an_error()` — [`L82`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L82)
- `test_action6_out_of_bounds_is_an_error()` — [`L77`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L77)
- `test_duplicate_actions_blocks_use_the_last_one()` — [`L89`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L89)
- `test_empty_plan_is_an_error()` — [`L67`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L67)
- `test_expect_levels_must_be_a_non_negative_integer()` — [`L120`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L120)
- `test_expect_must_be_cells_of_three_ints()` — [`L104`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L104)
- `test_expect_ranges_are_enforced()` — [`L113`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L113)
- `test_expectations_parse_to_tuples()` — [`L95`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L95)
- `test_json_code_fence_is_tolerated()` — [`L26`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L26)
- `test_malformed_json_is_an_error()` — [`L36`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L36)
- `test_missing_block_is_an_error()` — [`L31`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L31)
- `test_plan_longer_than_remaining_budget_is_clamped()` — [`L127`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L127)
- `test_trailing_bracket_after_object_is_tolerated()` — [`L41`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L41)
- `test_trailing_prose_after_object_is_tolerated()` — [`L52`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L52)
- `test_truncated_output_mentions_the_cutoff()` — [`L57`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L57)
- `test_unavailable_action_is_an_error()` — [`L62`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L62)
- `test_valid_plan_parses()` — [`L16`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L16)
- `wrap(json_text: str, prefix: str = "Analysis of the board.\n\n")` — [`L12`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L12)

## Module values
- `AVAILABLE` — [`L9`](../../../../../raw/code/Retrodict/tests/test_plan_parser.py#L9)

