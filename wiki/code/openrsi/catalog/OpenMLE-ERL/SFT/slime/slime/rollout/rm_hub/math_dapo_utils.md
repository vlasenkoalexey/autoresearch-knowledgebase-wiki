---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.rm_hub.math_dapo_utils`/
symbols:
  is_correct_minerva: is_correct_minerva().
  normalize_final_answer: normalize_final_answer().
  is_correct_strict_box: is_correct_strict_box().
  verify: verify().
  timeout.__enter__: timeout#__enter__().
  compute_score: compute_score().
  timeout.handle_timeout: timeout#handle_timeout().
  last_boxed_only_string: last_boxed_only_string().
  remove_boxed: remove_boxed().
  timeout.seconds: timeout#seconds.
  timeout.error_message: timeout#error_message.
  SUBSTITUTIONS: SUBSTITUTIONS.
  REMOVED_EXPRESSIONS: REMOVED_EXPRESSIONS.
  timeout: timeout#
  timeout.__init__: timeout#__init__().
  timeout.__exit__: timeout#__exit__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py)

## Classes
### `timeout`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py:65`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L65)
- signature: `class timeout:`
- members:
  - `handle_timeout(self, signum, frame)` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L71)
  - `error_message` — [`L69`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L69)
  - `seconds` — [`L68`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L68)
- protocol/private: `__enter__`[`L74`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L74), `__exit__`[`L78`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L78), `__init__`[`L67`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L67)

## Functions
- `compute_score(solution_str: str, ground_truth: str, strict_box_verify: bool = False, pause_tokens_index: list[int] | None = None)` — [`L262`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L262) — Compute the reward score for a solution.
- `is_correct_minerva(solution_str: str, gt: str, gt_need_extract: bool = False, answer_pattern: str = r"(?i)Answer\s*:\s*([^\n]+)")` — [`L185`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L185) — Check if the solution is correct according to Minerva criteria.
- `is_correct_strict_box(pred: str, gt: str, pause_tokens_index: list[int] | None = None)` — [`L215`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L215) — Check if the prediction is correct using strict boxed answer criteria.
- `last_boxed_only_string(string: str)` — [`L20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L20) — Extract the last LaTeX boxed expression from a string.
- `normalize_final_answer(final_answer: str)` — [`L143`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L143) — Normalize a final answer to a quantitative reasoning question.
- `remove_boxed(s: str)` — [`L50`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L50) — Remove the LaTeX boxed command from a string.
- `verify(solution_str: str, answer: str, strict_box_verify: bool = False, pause_tokens_index: list[int] | None = None)` — [`L240`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L240) — Verify if the solution is correct.

## Module values
- `REMOVED_EXPRESSIONS` — [`L96`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L96)
- `SUBSTITUTIONS` — [`L83`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_dapo_utils.py#L83)

