---
title: 'Module: ai_scientist/perform_vlm_review.py'
type: catalog
provenance: extracted
module: ai_scientist/perform_vlm_review.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.perform_vlm_review`/
symbols:
  generate_vlm_img_review: generate_vlm_img_review().
  perform_imgs_cap_ref_review: perform_imgs_cap_ref_review().
  perform_imgs_cap_ref_review_selection: perform_imgs_cap_ref_review_selection().
  generate_vlm_img_cap_ref_review: generate_vlm_img_cap_ref_review().
  generate_vlm_img_selection_review: generate_vlm_img_selection_review().
  detect_duplicate_figures: detect_duplicate_figures().
  extract_figure_screenshots: extract_figure_screenshots().
  reviewer_system_prompt_base: reviewer_system_prompt_base.
  extract_abstract: extract_abstract().
  encode_image_to_base64: encode_image_to_base64().
  img_cap_ref_review_prompt: img_cap_ref_review_prompt.
  img_cap_selection_prompt: img_cap_selection_prompt.
  img_review_prompt: img_review_prompt.
  extract_figure_screenshots.is_subfigure_caption: extract_figure_screenshots().is_subfigure_caption().
---
# Module: [`ai_scientist/perform_vlm_review.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py)

## Functions
- `detect_duplicate_figures(client, client_model, pdf_path)` — [`L389`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L389) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `encode_image_to_base64(image_data)` — [`L15`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L15) — Encode image data to base64 string.
- `extract_abstract(text)` — [`L311`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L311) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `extract_figure_screenshots(pdf_path, img_folder_path, num_pages=None, min_text_length=50, min_vertical_gap=30)` — [`L154`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L154) — Extract screenshots for figure captions ("Figure X." or "Figure X:") — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `generate_vlm_img_cap_ref_review(img, abstract, model, client)` — [`L350`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L350) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `generate_vlm_img_review(img, model, client)` — [`L363`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L363) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `generate_vlm_img_selection_review(img, abstract, model, client, reflection_page_info)` — [`L448`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L448)
- `is_subfigure_caption(txt)` — [`L204`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L204) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `perform_imgs_cap_ref_review(client, client_model, pdf_path)` — [`L372`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L372) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `perform_imgs_cap_ref_review_selection(client, client_model, pdf_path, reflection_page_info)` — [`L464`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L464) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)

## Module values
- `img_cap_ref_review_prompt` — [`L33`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L33) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `img_cap_selection_prompt` — [`L74`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L74)
- `img_review_prompt` — [`L126`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L126)
- `reviewer_system_prompt_base` — [`L28`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_vlm_review.py#L28)

