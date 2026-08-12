---
title: 'Module: training/src/rlm_train/rubric.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/rubric.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.rubric`/RLMTrainRubric#
symbols:
  RLMTrainRubric._user_correctness: _user_correctness.
  RLMTrainRubric._make_main_correctness: _make_main_correctness().
  RLMTrainRubric._passes_gates: _passes_gates().
  RLMTrainRubric.main: main().
  RLMTrainRubric.gated_reward: gated_reward().
  RLMTrainRubric._make_gated_metric: _make_gated_metric().
  RLMTrainRubric.rlm_below_min_iterations: rlm_below_min_iterations().
  RLMTrainRubric.rlm_below_min_subcall: rlm_below_min_subcall().
  RLMTrainRubric.rlm_below_min_reward: rlm_below_min_reward().
  RLMTrainRubric: ''
  RLMTrainRubric._min_subcall: _min_subcall.
  RLMTrainRubric._min_reward: _min_reward.
  RLMTrainRubric._min_iterations: _min_iterations.
  RLMTrainRubric._call_correctness: _call_correctness().
  RLMTrainRubric._gate_reward: _gate_reward.
  RLMTrainRubric.rlm_iterations: rlm_iterations().
  RLMTrainRubric.rlm_repl_calls: rlm_repl_calls().
  RLMTrainRubric.rlm_sub_llm_calls: rlm_sub_llm_calls().
  RLMTrainRubric.rlm_has_final_answer: rlm_has_final_answer().
  RLMTrainRubric.__init__: __init__().
---
# Module: [`training/src/rlm_train/rubric.py`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py)

## Classes
### `RLMTrainRubric`
- def: [`training/src/rlm_train/rubric.py:13`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L13)
- signature: `class RLMTrainRubric(vf.Rubric):`
- members:
  - `gated_reward(**kwargs: Any)` — [`L80`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L80)
  - `main(**kwargs: Any)` — [`L63`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L63)
  - `rlm_below_min_iterations(self, state: State)` — [`L104`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L104)
  - `rlm_below_min_reward(self, state: State)` — [`L114`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L114)
  - `rlm_below_min_subcall(self, state: State)` — [`L108`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L108)
  - `rlm_has_final_answer(self, state: State)` — [`L101`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L101)
  - `rlm_iterations(self, state: State)` — [`L92`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L92)
  - `rlm_repl_calls(self, state: State)` — [`L95`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L95)
  - `rlm_sub_llm_calls(self, state: State)` — [`L98`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L98)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L14), `_call_correctness`[`L51`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L51), `_gate_reward`[`L28`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L28), `_make_gated_metric`[`L77`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L77), `_make_main_correctness`[`L59`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L59), `_min_iterations`[`L25`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L25), `_min_reward`[`L27`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L27), `_min_subcall`[`L26`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L26), `_passes_gates`[`L42`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L42), `_user_correctness`[`L29`](../../../../../../../raw/code/rlm/training/src/rlm_train/rubric.py#L29)
- used by: [`__init__`](env.md#RLMTrainEnv.__init__)

