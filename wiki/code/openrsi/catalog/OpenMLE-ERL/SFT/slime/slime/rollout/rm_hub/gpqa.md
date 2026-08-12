---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.rm_hub.gpqa`/
symbols:
  compute_gpqa_reward: compute_gpqa_reward().
  _normalize_text: _normalize_text().
  _extract_letter_from_response: _extract_letter_from_response().
  _strip_chain_of_thought: _strip_chain_of_thought().
  DEFAULT_VALID_LETTERS: DEFAULT_VALID_LETTERS.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py)

## Functions
- `_extract_letter_from_response(response: str, valid_letters: Iterable[str])` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py#L22) — Best-effort extraction of the selected option letter from the model response.
- `_normalize_text(text: str)` — [`L18`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py#L18)
- `_strip_chain_of_thought(text: str)` — [`L8`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py#L8)
- `compute_gpqa_reward(response: str, label, metadata: dict | None = None)` — [`L54`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py#L54) — Rule-based scorer for GPQA-style multiple-choice evaluation.

## Module values
- `DEFAULT_VALID_LETTERS` — [`L5`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/gpqa.py#L5)

