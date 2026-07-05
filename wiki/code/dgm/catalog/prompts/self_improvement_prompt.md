---
title: 'Module: prompts/self_improvement_prompt.py'
type: catalog
provenance: extracted
module: prompts/self_improvement_prompt.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `prompts.self_improvement_prompt`/
symbols:
  get_diagnose_prompt_swe: get_diagnose_prompt_swe().
  get_diagnose_prompt_polyglot: get_diagnose_prompt_polyglot().
  find_selfimprove_eval_logs: find_selfimprove_eval_logs().
  get_problem_description_prompt: get_problem_description_prompt().
  get_current_code: get_current_code().
  process_selfimprove_eval_logs: process_selfimprove_eval_logs().
  coding_agent_summary_polyglot: coding_agent_summary_polyglot.
  diagnose_system_message: diagnose_system_message.
  read_mdlog_file: read_mdlog_file().
  coding_agent_summary: coding_agent_summary.
  diagnose_prompt: diagnose_prompt.
  problem_description_prompt: problem_description_prompt.
  swe_issue_prompt: swe_issue_prompt.
  polyglot_issue_prompt: polyglot_issue_prompt.
  diagnose_prompt_emptypatches: diagnose_prompt_emptypatches.
  diagnose_prompt_stochasticity: diagnose_prompt_stochasticity.
  diagnose_prompt_contextlength: diagnose_prompt_contextlength.
  diagnose_prompt_emptypatches_polyglot: diagnose_prompt_emptypatches_polyglot.
  diagnose_prompt_stochasticity_polyglot: diagnose_prompt_stochasticity_polyglot.
  get_eval_log_text: get_eval_log_text().
---
# Module: [`prompts/self_improvement_prompt.py`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py)

## Functions
- `find_selfimprove_eval_logs(entry, out_dir, commit_id='initial', filter=True)` — [`L200`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L200) — documented in [DGM_outer](../../concepts/DGM_outer.md)
- `get_current_code(current_dir, code_files, patch_files=None, exclude_files=None, is_polyglot=False)` — [`L409`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L409) — Retrieves the contents of specified Python files/directories, optionally — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `get_diagnose_prompt_polyglot(entry_id, commit, root_dir, out_dir, dataset, patch_files=[])` — [`L338`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L338) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `get_diagnose_prompt_swe(entry_id, commit, root_dir, out_dir, dataset, patch_files=[])` — [`L305`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L305) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `get_eval_log_text(eval_json, test_status=None)` — [`L371`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L371) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `get_problem_description_prompt(response_json, is_polyglot=False)` — [`L177`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L177) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `process_selfimprove_eval_logs(md_logs, eval_logs, predicted_patches, eval_results)` — [`L241`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L241) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `read_mdlog_file(filepath, filter=True)` — [`L183`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L183) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)

## Module values
- `coding_agent_summary` — [`L6`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L6) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `coding_agent_summary_polyglot` — [`L29`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L29)
- `diagnose_prompt` — [`L77`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L77) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `diagnose_prompt_contextlength` — [`L154`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L154)
- `diagnose_prompt_emptypatches` — [`L122`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L122)
- `diagnose_prompt_emptypatches_polyglot` — [`L254`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L254)
- `diagnose_prompt_stochasticity` — [`L138`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L138)
- `diagnose_prompt_stochasticity_polyglot` — [`L277`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L277)
- `diagnose_system_message` — [`L64`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L64) — documented in [prompts-self_improvement_prompt](../../concepts/prompts-self_improvement_prompt.md)
- `polyglot_issue_prompt` — [`L75`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L75)
- `problem_description_prompt` — [`L174`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L174)
- `swe_issue_prompt` — [`L74`](../../../../../raw/code/dgm/prompts/self_improvement_prompt.py#L74)

