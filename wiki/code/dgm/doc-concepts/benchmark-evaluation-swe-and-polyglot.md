---
title: Benchmark evaluation — SWE-bench and Polyglot
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Benchmark evaluation — SWE-bench and Polyglot

## Definition
The README's setup instructions reveal that DGM validates every self-edit against **two** coding benchmarks,
prepared separately: **SWE-bench** (Python GitHub issues — "Clone SWE-bench... `pip install -e .`") and
**Polyglot** (a multi-language benchmark spanning C++, Go, Java, JavaScript, Python, and Rust — "Prepare
Polyglot... `python -m polyglot.prepare_polyglot_dataset`"). A run targets one or the other; the empirical
score on the chosen benchmark is the sole criterion by which a self-edit is kept or discarded, standing in
for the theoretical Gödel machine's impossible correctness proof.

## In dgm (grounded)
The two benchmarks are why several modules come in paired SWE / Polyglot variants.
[self_improve_step](../concepts/self_improve_step.md) branches on a `polyglot` flag to call either
`run_harness_swe` or `run_harness_polyglot`; the diagnosis-prompt builder has parallel
[`get_diagnose_prompt_swe`](../catalog/prompts/self_improvement_prompt.md#get_diagnose_prompt_swe) and
[`get_diagnose_prompt_polyglot`](../catalog/prompts/self_improvement_prompt.md#get_diagnose_prompt_polyglot)
paths (→ [prompts-self_improvement_prompt](../concepts/prompts-self_improvement_prompt.md)); and the agent
itself ships as both `coding_agent.py` and `coding_agent_polyglot.py`, one swapped in for the other inside
the container depending on mode. Turning a raw benchmark run into a *score* is where the two benchmarks
diverge most: SWE-bench target repos each print test results in their own format, normalized by the
per-framework parsers in [utils-swe_log_parsers](../concepts/utils-swe_log_parsers.md) and dispatched via
[`MAP_REPO_TO_PARSER`](../catalog/utils/swe_log_parsers.md#MAP_REPO_TO_PARSER); Polyglot instead builds and
runs each task in a dedicated Docker image produced by
[polyglot-docker_build](../concepts/polyglot-docker_build.md).

## Why it matters / when it applies
Because scoring is the accept/reject gate for the entire evolutionary loop, this evaluation infrastructure —
though none of it is a "research idea" — is load-bearing: a mis-parsed test log or a mis-built image would
silently corrupt the archive's fitness signal, and thus which agents get selected as future parents in
[DGM_outer](../concepts/DGM_outer.md). Running on two structurally different benchmarks (single-language
issue-fixing vs. six-language task-solving) is also what lets the paper argue the discovered
self-improvements generalize rather than overfit one benchmark's quirks.

## Connections
- Code concepts: [utils-swe_log_parsers](../concepts/utils-swe_log_parsers.md) — SWE-bench log→score;
  [polyglot-docker_build](../concepts/polyglot-docker_build.md) — Polyglot's sandboxed eval images;
  [self_improve_step](../concepts/self_improve_step.md) — the harness dispatch;
  [prompts-self_improvement_prompt](../concepts/prompts-self_improvement_prompt.md) — the paired diagnosis paths.
- Module catalogs: [utils/swe_log_parsers](../catalog/utils/swe_log_parsers.md),
  [polyglot/docker_build](../catalog/polyglot/docker_build.md).
- Related doc-concepts: [running-the-dgm](running-the-dgm.md),
  [safety-untrusted-model-code](safety-untrusted-model-code.md).

## Source
Extracted from `README.md` (kept in place).
