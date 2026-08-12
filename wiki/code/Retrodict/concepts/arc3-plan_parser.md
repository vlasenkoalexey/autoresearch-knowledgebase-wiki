---
title: PlannedAction / ParsedPlan — where the per-action prediction is born
type: concept
provenance: mixed
concept: arc3-plan_parser
concepts: [verification-independence]
updated: 2026-08-12
status: fresh
---
# PlannedAction / ParsedPlan — where the per-action prediction is born

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [verification-independence](../../../concepts/verification-independence.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview

`plan_parser` turns a model's free-text reply into validated, structured actions: `parse_actions` extracts
the `[ACTIONS]` block (*"Parse the final [ACTIONS] block out of an agent reply"*), and
[`_validate_item`](../catalog/src/arc3/plan_parser.md#_validate_item) turns each raw entry into a
[`PlannedAction`](../catalog/src/arc3/plan_parser.md#PlannedAction) — *"One validated action from the
agent's plan"* — which is where the `expect` field that
[`GameRunner._check_expectations`](../catalog/src/arc3/runner.md#GameRunner._check_expectations) later
verifies actually originates.

## Design rationale (why it's built this way)

**Parse errors are model-facing by design.** [`PlanParseError`](../catalog/src/arc3/plan_parser.md#PlanParseError)'s
docstring states this directly: *"The [ACTIONS] block is missing or invalid; the message is model-facing"* —
the exception's text is written to be re-shown to the model as feedback, not just logged for a human
developer, so a malformed plan becomes a correction the model can act on rather than a silent failure.

**Truncation is handled as a first-class parsing condition, not an error.** `parse_actions` accepts a
`truncated: bool` flag and [`_decode_object`](../catalog/src/arc3/plan_parser.md#_decode_object) — *"Decode
the first complete JSON object in the payload"* — is written to recover a usable plan even from a reply cut
short by a token limit, via `_with_truncation_hint`, rather than discarding a partially-generated plan
outright.

**Every plan carries `expect_levels` at the plan level, not just per-action.** `ParsedPlan.expect_levels`
sits alongside the per-action `expect` on each `PlannedAction` — the plan format supports predicting outcomes
at two granularities, a single action's expected board state and the plan's expected level-count outcome.

## Entry points
- [`parse_actions`](../catalog/src/arc3/plan_parser.md#parse_actions) — the single entry point, called from
  [`GameRunner._accept`](../catalog/src/arc3/runner.md#GameRunner._accept).

## Mechanism (step-by-step)
1. [`GameRunner._accept`](../catalog/src/arc3/runner.md#GameRunner._accept) hands the model's raw reply to
   [`parse_actions`](../catalog/src/arc3/plan_parser.md#parse_actions), which locates the `[ACTIONS]` marker
   and decodes the JSON payload via [`_decode_object`](../catalog/src/arc3/plan_parser.md#_decode_object).
2. Each item in the decoded array is validated by
   [`_validate_item`](../catalog/src/arc3/plan_parser.md#_validate_item) into a
   [`PlannedAction`](../catalog/src/arc3/plan_parser.md#PlannedAction) — carrying
   [`name`](../catalog/src/arc3/plan_parser.md#PlannedAction.name),
   [`x`](../catalog/src/arc3/plan_parser.md#PlannedAction.x)/[`y`](../catalog/src/arc3/plan_parser.md#PlannedAction.y),
   and [`expect`](../catalog/src/arc3/plan_parser.md#PlannedAction.expect) — against the environment's
   `available` action set, raising [`PlanParseError`](../catalog/src/arc3/plan_parser.md#PlanParseError) on
   an invalid entry.
3. The validated actions assemble into a [`ParsedPlan`](../catalog/src/arc3/plan_parser.md#ParsedPlan)
   (`actions`, `expect_levels`), which [`GameRunner._drain`](../catalog/src/arc3/runner.md#GameRunner._drain)
   then executes one [`PlannedAction`](../catalog/src/arc3/plan_parser.md#PlannedAction) at a time, checking
   each one's `expect` against reality via
   [`_check_expectations`](../catalog/src/arc3/runner.md#GameRunner._check_expectations).

## Key data structures
- [`PlannedAction`](../catalog/src/arc3/plan_parser.md#PlannedAction) — `name`, `x`, `y`, `expect`: the
  atomic unit `_check_expectations` verifies.
- [`ParsedPlan`](../catalog/src/arc3/plan_parser.md#ParsedPlan) — `actions`, `expect_levels`: a whole
  validated plan, ready to drain.

## See also
- [`arc3-runner`](arc3-runner.md) — the consumer: `_accept` produces a `ParsedPlan`, `_drain`/`_step`/
  `_check_expectations` execute and verify it action by action.
