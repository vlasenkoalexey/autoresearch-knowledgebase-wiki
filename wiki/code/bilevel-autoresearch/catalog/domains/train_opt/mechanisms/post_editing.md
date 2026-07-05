---
title: 'Module: domains/train_opt/mechanisms/post_editing.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/post_editing.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.post_editing`/
symbols:
  PostEditing.post_edit: PostEditing#post_edit().
  PostEditing._record_trigger: PostEditing#_record_trigger().
  PostEditing._safe_eval: PostEditing#_safe_eval().
  PostEditing._rule_triggers: PostEditing#_rule_triggers.
  PostEditing.get_post_edit_text: PostEditing#get_post_edit_text().
  PostEditing: PostEditing#
  PostEditing._corrections: PostEditing#_corrections.
  PostEditing._is_power_of_2: PostEditing#_is_power_of_2().
  PostEditing._nearest_power_of_2: PostEditing#_nearest_power_of_2().
  logger: logger.
  PostEditing.__init__: PostEditing#__init__().
---
# Module: [`domains/train_opt/mechanisms/post_editing.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py)

## Classes
### `PostEditing`
- def: [`domains/train_opt/mechanisms/post_editing.py:27`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L27)
- doc: Applies rule-based post-editing to refine LLM proposals before GPU runs.
- signature: `class PostEditing:`
- members:
  - `_is_power_of_2(self, n: float)` — [`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L52) — Check if a number is a power of 2.
  - `_nearest_power_of_2(self, n: float)` — [`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L59) — Return the nearest power of 2.
  - `_record_trigger(self, rule_name: str)` — [`L70`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L70) — Record that a rule was triggered.
  - `_safe_eval(self, val)` — [`L41`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L41) — Safely evaluate a parameter value to a float.
  - `get_post_edit_text(self)` — [`L227`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L227) — Generate a summary of common post-editing corrections for the prompt.
  - `post_edit(self, changes: dict, current_config: dict)` — [`L74`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L74) — Apply post-editing rules to a proposed set of changes.
- protocol/private: `__init__`[`L35`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L35), `_corrections`[`L39`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L39), `_rule_triggers`[`L37`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L37)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`post_editing`](../runner.md#TrainRunner.post_editing)

## Module values
- `logger` — [`L24`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/post_editing.py#L24)

