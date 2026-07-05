---
title: Two-stage operator workflow (ideate → run)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Two-stage operator workflow (ideate → run)

## Definition
The README frames operating AI Scientist-v2 as two sequential commands, not one monolithic run.
**Stage 1 — ideation**: you write a Markdown topic description (with `Title`, `Keywords`, `TL;DR`,
`Abstract` sections) and run `perform_ideation_temp_free.py`, which has an LLM brainstorm and refine
research ideas (checking novelty via Semantic Scholar) and emits a JSON idea file named after the input.
**Stage 2 — experiments + writeup**: you feed that JSON to `launch_scientist_bfts.py`, which runs the
agentic best-first tree search, analyzes results, and drafts a paper. The JSON idea file is the hand-off
artifact between the two stages.

## In ai-scientist-v2 (grounded)
- **Ideation entrypoint.** The README's `python ai_scientist/perform_ideation_temp_free.py --workshop-file
  … --model … --max-num-generations … --num-reflections …` is driven by
  [`generate_temp_free_idea`](../catalog/ai_scientist/perform_ideation_temp_free.md#generate_temp_free_idea),
  whose `max_num_generations` / `num_reflections` parameters correspond directly to the two flags. The CLI
  flags are parsed by the module's argument
  [`parser`](../catalog/ai_scientist/perform_ideation_temp_free.md#parser) into
  [`args`](../catalog/ai_scientist/perform_ideation_temp_free.md#args), the novelty check runs through the
  [`semantic_scholar_tool`](../catalog/ai_scientist/perform_ideation_temp_free.md#semantic_scholar_tool),
  and the resulting ideas are written to the JSON path
  [`idea_fname`](../catalog/ai_scientist/perform_ideation_temp_free.md#idea_fname) (owning module:
  [`ai_scientist/perform_ideation_temp_free.py`](../catalog/ai_scientist/perform_ideation_temp_free.md)).
- **Experiment entrypoint.** The README's `python launch_scientist_bfts.py --load_ideas … --load_code
  --add_dataset_ref --model_writeup … --model_citation … --model_review … --model_agg_plots …
  --num_cite_rounds …` is wired through
  [`parse_arguments`](../catalog/launch_scientist_bfts.md#parse_arguments); the `--load_ideas` JSON is the
  artifact produced by Stage 1. The finished PDF the README says to look for is located by
  [`find_pdf_path_for_review`](../catalog/launch_scientist_bfts.md#find_pdf_path_for_review), and run-wide
  cost accounting is flushed by
  [`save_token_tracker`](../catalog/launch_scientist_bfts.md#save_token_tracker) (owning module:
  [`launch_scientist_bfts.py`](../catalog/launch_scientist_bfts.md)).

## Why it matters / when it applies
Separating ideation from experimentation is what lets the operator *curate*: the README recommends
reviewing the JSON idea file (and `bfts_config.yaml`) before committing to a costly experiment run. It is
also the mechanism for retargeting to a new subject field — the FAQ's "run for different subject fields"
answer is simply "re-run Stage 1 with a new topic Markdown, then pass the new JSON to Stage 2." The two
stages have very different cost profiles (ideation is a few dollars; a full experiment run is ~$15–20 plus
~$5 writeup), so treating them as distinct steps is a budgeting decision as much as a workflow one.

## Connections
- Code concepts:
  [ai_scientist-perform_ideation_temp_free](../concepts/ai_scientist-perform_ideation_temp_free.md) —
  the ideation loop in depth;
  [launch_scientist_bfts](../concepts/launch_scientist_bfts.md) — the experiment/writeup orchestrator.
- Module catalogs:
  [ai_scientist/perform_ideation_temp_free](../catalog/ai_scientist/perform_ideation_temp_free.md),
  [launch_scientist_bfts](../catalog/launch_scientist_bfts.md).
- Related doc-concepts: [bfts-tree-search-configuration](bfts-tree-search-configuration.md),
  [multi-provider-model-selection](multi-provider-model-selection.md).

## Source
Extracted from `README.md` (kept in place).
