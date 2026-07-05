---
title: Running the DGM
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Running the DGM

## Definition
The README frames the whole system's entry point in one line: `python DGM_outer.py`, "By default, outputs
will be saved in the `output_dgm/` directory." That single command launches the open-ended evolution loop —
the archive of self-improving coding agents that the paper is about — and every artifact of a run (per-node
metadata, patches, logs, the archive snapshot) lands under `output_dgm/<run_id>/`.

## In dgm (grounded)
`DGM_outer.py`'s [`main`](../catalog/DGM_outer.md#main) is what that command invokes: it parses the run
arguments (max generations, self-improve batch size, parent-selection method, archive-update method,
baselines), calls [`initialize_run`](../catalog/DGM_outer.md#initialize_run) to seed or resume the archive
from the frozen `'initial'` agent, and then drives the generation loop that alternates
[`choose_selfimproves`](../catalog/DGM_outer.md#choose_selfimproves) (pick parents) →
`self_improve` (edit + evaluate, in [self_improve_step](../concepts/self_improve_step.md)) →
[`update_archive`](../catalog/DGM_outer.md#update_archive) (admit survivors), appending each generation's
state to `dgm_metadata.jsonl`. The README's file-structure list maps one-to-one onto this silo's modules:
`coding_agent.py` (the agent being evolved → [coding_agent](../concepts/coding_agent.md)), `DGM_outer.py`
(the algorithm entry point → [DGM_outer](../concepts/DGM_outer.md)), `prompts/`
(→ [prompts-self_improvement_prompt](../concepts/prompts-self_improvement_prompt.md)), `tools/`
(→ [tools-bash](../concepts/tools-bash.md)), `swe_bench/` and `polyglot/` (the two evaluation harnesses),
and `analysis/` (offline plotting → [analysis-visualize_archive](../concepts/analysis-visualize_archive.md)).

## Why it matters / when it applies
The README's setup steps make the run's two external dependencies explicit: **Docker** (each
self-improvement attempt and each evaluation runs inside a container — see
[self_improve_step](../concepts/self_improve_step.md) and
[polyglot-docker_build](../concepts/polyglot-docker_build.md)) and **API keys** (`OPENAI_API_KEY`,
`ANTHROPIC_API_KEY`) for the LLMs the agent and the diagnosis model call. The two benchmarks it evaluates on
— SWE-bench (Python) and Polyglot (six languages) — are prepared separately (cloning SWE-bench, running
`python -m polyglot.prepare_polyglot_dataset`), which is why the archive's viability and scoring machinery
(`swe_bench/`, `polyglot/`, `utils/swe_log_parsers.py`) is a large fraction of the repo.

## Connections
- Code concepts: [DGM_outer](../concepts/DGM_outer.md) — the loop `python DGM_outer.py` runs;
  [self_improve_step](../concepts/self_improve_step.md) — one dispatched attempt.
- Module catalogs: [DGM_outer](../catalog/DGM_outer.md).
- Related doc-concepts: [safety-untrusted-model-code](safety-untrusted-model-code.md),
  [benchmark-evaluation-swe-and-polyglot](benchmark-evaluation-swe-and-polyglot.md).

## Source
Extracted from `README.md` (kept in place).
