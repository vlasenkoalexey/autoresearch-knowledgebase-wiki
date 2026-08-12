---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/generation_loop.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/generation_loop.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.generation_loop`/GenerationLoopCon
symbols:
  GenerationLoopController.advance_after_completion: troller#advance_after_completion().
  GenerationLoopConfig.max_generated: fig#max_generated.
  GenerationLoopConfig.__post_init__: fig#__post_init__().
  GenerationLoopController.initialize_state: troller#initialize_state().
  GenerationLoopController._config: troller#_config.
  GenerationLoopController.batch_size: troller#batch_size().
  GenerationLoopController.accepted_target: troller#accepted_target().
  GenerationLoopController._max_target_reached: troller#_max_target_reached().
  GenerationLoopConfig: fig#
  GenerationLoopController._target_met: troller#_target_met().
  GenerationLoopConfig.batch_size: fig#batch_size.
  GenerationLoopConfig.accepted_target: fig#accepted_target.
  GenerationLoopController: troller#
  GenerationLoopController.__init__: troller#__init__().
  GenerationLoopController.generation_needed: troller#generation_needed().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/generation_loop.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py)

## Classes
### `GenerationLoopConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/services/generation_loop.py:10`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L10)
- doc: Rules for when to keep generating samples for one task.
- signature: `class GenerationLoopConfig:`
- members:
  - `accepted_target` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L14)
  - `batch_size` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L13)
  - `max_generated` — [`L15`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L15)
- protocol/private: `__post_init__`[`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L17)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`advance_after_completion`](generation_loop.md#GenerationLoopController.advance_after_completion), [`initialize_state`](generation_loop.md#GenerationLoopController.initialize_state), [`batch_size`](generation_loop.md#GenerationLoopController.batch_size), [`_max_target_reached`](generation_loop.md#GenerationLoopController._max_target_reached), [`accepted_target`](generation_loop.md#GenerationLoopController.accepted_target), [`__init__`](generation_loop.md#GenerationLoopController.__init__)

### `GenerationLoopController`
- def: [`OpenMLE-ERL/SFT/tts_search/services/generation_loop.py:26`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L26)
- doc: Controls per-task generation targets independently of gen/eval services.
- signature: `class GenerationLoopController:`
- members:
  - `accepted_target(self)` — [`L37`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L37)
  - `advance_after_completion(self, state: Any)` — [`L60`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L60) — Advance target after completed evals and return additional needed gens. — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
  - `batch_size(self)` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L33)
  - `generation_needed(self, state: Any)` — [`L48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L48) — Return how many new generations should be queued for this state.
  - `initialize_state(self, state: Any)` — [`L40`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L40) — Ensure a fresh state starts with one batch target.
- protocol/private: `__init__`[`L29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L29), `_config`[`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L30), `_max_target_reached`[`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L84), `_target_met`[`L78`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generation_loop.py#L78)
- uses (calls/refs, reference-scoped): [`max_generated`](generation_loop.md#GenerationLoopConfig.max_generated), [`GenerationLoopConfig`](generation_loop.md#GenerationLoopConfig), [`accepted_target`](generation_loop.md#GenerationLoopConfig.accepted_target), [`batch_size`](generation_loop.md#GenerationLoopConfig.batch_size)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_on_eval_result`](scheduler.md#Scheduler._on_eval_result), [`_on_gen_result`](scheduler.md#Scheduler._on_gen_result), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB)

