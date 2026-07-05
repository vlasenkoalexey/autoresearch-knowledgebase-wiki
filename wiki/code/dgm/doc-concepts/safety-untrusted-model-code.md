---
title: Safety — executing untrusted model-generated code
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Safety — executing untrusted model-generated code

## Definition
The README carries an explicit `[!WARNING]`: "This repository involves executing untrusted, model-generated
code. We strongly advise users to be aware of the associated safety risks... it may still behave
destructively due to limitations in model capability or alignment." This is intrinsic to what DGM *is* — a
system that writes new code (edits to its own agent) and then runs that code — so every self-improvement
attempt and every benchmark evaluation is, by construction, executing code no human reviewed.

## In dgm (grounded)
The concrete mitigation in the codebase is **containerization**: model-generated edits never run in the host
process. In [self_improve_step](../concepts/self_improve_step.md),
[`build_dgm_container`](../catalog/utils/docker_utils.md#build_dgm_container) creates a fresh Docker container
per attempt, the parent's code and patches are copied in with
[`copy_to_container`](../catalog/utils/docker_utils.md#copy_to_container), the self-editing coding agent runs
*inside* that container (under a 30-minute `timeout`), and results are copied back out with
[`copy_from_container`](../catalog/utils/docker_utils.md#copy_from_container) before
[`cleanup_container`](../catalog/utils/docker_utils.md#cleanup_container) tears it down. Benchmark evaluation
is likewise sandboxed: the Polyglot harness builds and runs each task in its own image
(→ [polyglot-docker_build](../concepts/polyglot-docker_build.md)). So a destructive or broken self-edit is
contained to a disposable container and can neither corrupt the host DGM process nor a concurrently running
sibling attempt.

## Why it matters / when it applies
The containment boundary is also what makes the archive's "keep every viable variant" policy safe to run at
scale: `DGM_outer.py` fans out several self-improvement attempts concurrently (→ [DGM_outer](../concepts/DGM_outer.md)),
each mutating agent code, and the only reason those parallel mutations don't interfere is that each lives in
its own container. The README's warning is the human-facing counterpart to that engineering boundary: the
sandbox reduces but does not eliminate risk, so the maintainers ask users to run it knowingly.

## Connections
- Code concepts: [self_improve_step](../concepts/self_improve_step.md) — where the untrusted self-edit is
  built, run, and torn down in a container; [polyglot-docker_build](../concepts/polyglot-docker_build.md) —
  the sandboxed evaluation images.
- Module catalogs: [utils/docker_utils](../catalog/utils/docker_utils.md).
- Related doc-concepts: [running-the-dgm](running-the-dgm.md).

## Source
Extracted from `README.md` (kept in place).
