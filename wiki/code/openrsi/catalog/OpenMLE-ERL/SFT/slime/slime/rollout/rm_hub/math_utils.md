---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.rm_hub.math_utils`/
symbols:
  _normalize: _normalize().
  grade_answer_sympy: grade_answer_sympy().
  _strip_string: _strip_string().
  extract_answer: extract_answer().
  grade_answer_verl: grade_answer_verl().
  should_allow_eval: should_allow_eval().
  split_tuple: split_tuple().
  are_equal_under_sympy: are_equal_under_sympy().
  extract_boxed_answer: extract_boxed_answer().
  _str_is_int: _str_is_int().
  grade_answer_mathd: grade_answer_mathd().
  mathd_normalize_answer: mathd_normalize_answer().
  TUPLE_CHARS: TUPLE_CHARS.
  _is_frac: _is_frac().
  _strip_properly_formatted_commas: _strip_properly_formatted_commas().
  _strip_string._fix_fracs: _strip_string()._fix_fracs().
  _strip_string._fix_a_slash_b: _strip_string()._fix_a_slash_b().
  _strip_string._remove_right_units: _strip_string()._remove_right_units().
  _strip_string._fix_sqrt: _strip_string()._fix_sqrt().
  BAD_SUBSTRINGS: BAD_SUBSTRINGS.
  BAD_REGEXES: BAD_REGEXES.
  _sympy_parse: _sympy_parse().
  _parse_latex: _parse_latex().
  _is_float: _is_float().
  _is_int: _is_int().
  _str_to_int: _str_to_int().
  _inject_implicit_mixed_number: _inject_implicit_mixed_number().
  count_unknown_letters_in_expr: count_unknown_letters_in_expr().
  last_boxed_only_string: last_boxed_only_string().
  remove_boxed: remove_boxed().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py)

## Functions
- `_fix_a_slash_b(string)` — [`L61`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L61)
- `_fix_fracs(string)` — [`L30`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L30)
- `_fix_sqrt(string)` — [`L84`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L84)
- `_inject_implicit_mixed_number(step: str)` — [`L234`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L234) — Automatically make a mixed number evalable
- `_is_float(num: str)` — [`L200`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L200)
- `_is_frac(expr: str)` — [`L215`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L215)
- `_is_int(x: float)` — [`L208`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L208)
- `_normalize(expr: str)` — [`L255`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L255) — Normalize answer expressions.
- `_parse_latex(expr: str)` — [`L182`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L182) — Attempts to parse latex to an expression sympy can read.
- `_remove_right_units(string)` — [`L75`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L75)
- `_str_is_int(x: str)` — [`L219`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L219)
- `_str_to_int(x: str)` — [`L228`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L228)
- `_strip_properly_formatted_commas(expr: str)` — [`L244`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L244)
- `_strip_string(string)` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L29)
- `_sympy_parse(expr: str)` — [`L168`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L168) — Parses an expression with sympy.
- `are_equal_under_sympy(ground_truth_normalized: str, given_normalized: str)` — [`L351`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L351)
- `count_unknown_letters_in_expr(expr: str)` — [`L328`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L328)
- `extract_answer(passage: str)` — [`L478`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L478)
- `extract_boxed_answer(solution: str)` — [`L422`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L422) — Extract the answer from inside a LaTeX \boxed{} command
- `grade_answer_mathd(given_answer: str, ground_truth: str)` — [`L468`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L468)
- `grade_answer_sympy(given_answer: str, ground_truth: str)` — [`L429`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L429)
- `grade_answer_verl(solution_str, ground_truth)` — [`L484`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L484)
- `last_boxed_only_string(string)` — [`L384`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L384)
- `mathd_normalize_answer(answer: str | None)` — [`L15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L15)
- `remove_boxed(s)` — [`L412`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L412)
- `should_allow_eval(expr: str)` — [`L335`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L335)
- `split_tuple(expr: str)` — [`L365`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L365) — Split the elements in a tuple/interval, while handling well-formatted commas in large numbers

## Module values
- `BAD_REGEXES` — [`L164`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L164)
- `BAD_SUBSTRINGS` — [`L163`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L163)
- `TUPLE_CHARS` — [`L165`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/math_utils.py#L165)

