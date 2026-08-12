---
title: 'Module: tests/test_prompts.py'
type: catalog
provenance: extracted
module: tests/test_prompts.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_prompts`/test_
symbols:
  test_system_prompt_documents_diff_arclog_scratch_and_hud_guidance: system_prompt_documents_diff_arclog_scratch_and_hud_guidance().
  test_system_prompt_prescribes_explore_then_commit_cadence: system_prompt_prescribes_explore_then_commit_cadence().
  test_system_prompt_prescribes_forward_simulation_over_live_probing: system_prompt_prescribes_forward_simulation_over_live_probing().
  test_system_prompt_forbids_acting_without_a_prediction: system_prompt_forbids_acting_without_a_prediction().
  test_system_prompt_prescribes_curated_playbook_memory: system_prompt_prescribes_curated_playbook_memory().
  test_invocation_prompts_nudge_agents_to_use_arclog_and_diff: invocation_prompts_nudge_agents_to_use_arclog_and_diff().
  test_fresh_session_prompt_directs_reading_playbook_first: fresh_session_prompt_directs_reading_playbook_first().
---
# Module: [`tests/test_prompts.py`](../../../../../raw/code/Retrodict/tests/test_prompts.py)

## Functions
- `test_fresh_session_prompt_directs_reading_playbook_first()` — [`L111`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L111) — A fresh session is exactly the moment curated memory pays off: it must read playbook.md before
- `test_invocation_prompts_nudge_agents_to_use_arclog_and_diff()` — [`L104`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L104)
- `test_system_prompt_documents_diff_arclog_scratch_and_hud_guidance()` — [`L8`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L8)
- `test_system_prompt_forbids_acting_without_a_prediction()` — [`L63`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L63) — The observed weak-model failure was acting with no hypothesis at all — blind guessing and
- `test_system_prompt_prescribes_curated_playbook_memory()` — [`L73`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L73) — The dominant cost sink on hard levels is a fresh session (triggered by the context drop)
- `test_system_prompt_prescribes_explore_then_commit_cadence()` — [`L33`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L33) — Weak models thrash by advancing a known mechanic one action per reply; the prompt must
- `test_system_prompt_prescribes_forward_simulation_over_live_probing()` — [`L51`](../../../../../raw/code/Retrodict/tests/test_prompts.py#L51) — The behavior that separates strong from weak runs is resolving an action's outcome by

