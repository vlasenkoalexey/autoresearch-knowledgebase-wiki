---
title: 'Module: launch_scientist_bfts.py'
type: catalog
provenance: extracted
module: launch_scientist_bfts.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 launch_scientist_bfts/
symbols:
  idea_dir: idea_dir.
  args: args.
  code_path: code_path.
  review_img_cap_ref: review_img_cap_ref.
  attempt: attempt.
  added_code: added_code.
  idea_config_path: idea_config_path.
  idea_path_json: idea_path_json.
  experiment_results_dir: experiment_results_dir.
  dataset_ref_path: dataset_ref_path.
  ideas: ideas.
  pdf_path: pdf_path.
  review_text: review_text.
  f: f.
  save_token_tracker: save_token_tracker().
  dataset_ref_code: dataset_ref_code.
  citations_text: citations_text.
  available_gpus: available_gpus.
  code: code.
  cmdline: cmdline.
  client_model: client_model.
  idea: idea.
  paper_content: paper_content.
  child: child.
  process: process.
  proc: proc.
  children: children.
  writeup_success: writeup_success.
  idea_path_md: idea_path_md.
  alive: alive.
  client: client.
  parse_arguments: parse_arguments().
  get_available_gpus: get_available_gpus().
  find_pdf_path_for_review: find_pdf_path_for_review().
  date: date.
  config_path: config_path.
  current_process: current_process.
  keywords: keywords.
  print_time: print_time().
  redirect_stdout_stderr_to_file: redirect_stdout_stderr_to_file().
  gone: gone.
---
# Module: [`launch_scientist_bfts.py`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py)

## Functions
- `find_pdf_path_for_review(idea_dir)` — [`L140`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L140) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `get_available_gpus(gpu_ids=None)` — [`L134`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L134)
- `parse_arguments()` — [`L42`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L42) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `print_time()` — [`L31`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L31)
- `redirect_stdout_stderr_to_file(log_file_path)` — [`L168`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L168)
- `save_token_tracker(idea_dir)` — [`L35`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L35) — documented in [ai_scientist-utils-token_tracker](../concepts/ai_scientist-utils-token_tracker.md)

## Module values
- `added_code` — [`L230`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L230) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `alive` — [`L338`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L338)
- `args` — [`L183`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L183) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `attempt` — [`L278`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L278) — documented in [ai_scientist-perform_icbinb_writeup](../concepts/ai_scientist-perform_icbinb_writeup.md)
- `available_gpus` — [`L188`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L188) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `child` — [`L331`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L331)
- `children` — [`L328`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L328)
- `citations_text` — [`L273`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L273) — documented in [ai_scientist-perform_icbinb_writeup](../concepts/ai_scientist-perform_icbinb_writeup.md)
- `client` — [`L310`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L310) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `client_model` — [`L310`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L310) — documented in [ai_scientist-llm](../concepts/ai_scientist-llm.md)
- `cmdline` — [`L352`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L352)
- `code` — [`L206`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L206) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `code_path` — [`L208`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L208) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `config_path` — [`L249`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L249)
- `current_process` — [`L327`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L327)
- `dataset_ref_code` — [`L219`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L219) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `dataset_ref_path` — [`L221`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L221)
- `date` — [`L197`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L197)
- `experiment_results_dir` — [`L257`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L257) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `f` — [`L191`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L191)
- `gone` — [`L338`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L338)
- `idea` — [`L195`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L195) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `idea_config_path` — [`L250`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L250) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `idea_dir` — [`L198`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L198) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `idea_path_json` — [`L245`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L245) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `idea_path_md` — [`L203`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L203)
- `ideas` — [`L192`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L192) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `keywords` — [`L348`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L348)
- `paper_content` — [`L309`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L309) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `pdf_path` — [`L306`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L306) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `proc` — [`L349`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L349)
- `process` — [`L341`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L341)
- `review_img_cap_ref` — [`L312`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L312) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `review_text` — [`L311`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L311) — documented in [launch_scientist_bfts](../concepts/launch_scientist_bfts.md)
- `writeup_success` — [`L272`](../../../../raw/code/ai-scientist-v2/launch_scientist_bfts.py#L272)

