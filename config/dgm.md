---
slug: dgm
repo: https://github.com/jennyzzt/dgm
acquire: submodule
docs: [README.md]
synthesis_focus: the Darwin Gödel Machine's self-referential improvement loop — the growing archive of coding agents (versus a single evolving lineage), stepping-stone parent selection that favors performance and novelty/diversity over a strict fitness ratchet, and how the agent literally rewrites its own tools/prompts/workflow code and is validated by re-running it on SWE-bench/Polyglot before being admitted back into the archive
---

## Concepts
- **DGM_outer** — seeds: `choose_selfimproves`, `update_archive`, `get_full_eval_threshold`, `initialize_run`
- **self_improve_step** — seeds: `self_improve`, `diagnose_improvement`, `run_harness_swe`, `run_harness_polyglot`
