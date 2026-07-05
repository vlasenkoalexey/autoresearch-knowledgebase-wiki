---
title: 'Module: ai_scientist/perform_llm_review.py'
type: catalog
provenance: extracted
module: ai_scientist/perform_llm_review.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.perform_llm_review`/
symbols:
  perform_review: perform_review().
  get_review_fewshot_examples: get_review_fewshot_examples().
  get_meta_review: get_meta_review().
  load_paper: load_paper().
  dir_path: dir_path.
  neurips_form: neurips_form.
  reviewer_system_prompt_neg: reviewer_system_prompt_neg.
  fewshot_papers: fewshot_papers.
  fewshot_reviews: fewshot_reviews.
  reviewer_system_prompt_pos: reviewer_system_prompt_pos.
  reviewer_system_prompt_base: reviewer_system_prompt_base.
  template_instructions: template_instructions.
  reviewer_reflection_prompt: reviewer_reflection_prompt.
  load_review: load_review().
  meta_reviewer_system_prompt: meta_reviewer_system_prompt.
---
# Module: [`ai_scientist/perform_llm_review.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py)

## Functions
- `get_meta_review(model, client, temperature, reviews)` — [`L349`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L349) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `get_review_fewshot_examples(num_fs_examples=1)` — [`L312`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L312) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `load_paper(pdf_path, num_pages=None, min_size=100)` — [`L257`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L257) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `load_review(json_path)` — [`L291`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L291)
- `perform_review(text, model, client, num_reflections=1, num_fs_examples=1, num_reviews_ensemble=1, temperature=0.75, msg_history=None, return_msg_history=False, reviewer_system_prompt=reviewer_system_prompt_neg, review_instruction_form=neurips_form)` — [`L125`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L125) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)

## Module values
- `dir_path` — [`L297`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L297)
- `fewshot_papers` — [`L299`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L299)
- `fewshot_reviews` — [`L305`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L305)
- `meta_reviewer_system_prompt` — [`L343`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L343)
- `neurips_form` — [`L64`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L64) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `reviewer_reflection_prompt` — [`L236`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L236)
- `reviewer_system_prompt_base` — [`L13`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L13)
- `reviewer_system_prompt_neg` — [`L17`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L17) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `reviewer_system_prompt_pos` — [`L21`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L21)
- `template_instructions` — [`L26`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_llm_review.py#L26)

