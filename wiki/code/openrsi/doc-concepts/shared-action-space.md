---
title: One shared action space across Gym-scored training and search
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-06
status: fresh
---
# One shared action space across Gym-scored training and search

## Definition
The README frames the whole repository as one loop: "Search produces experience, experience enters training,
and trained models return to search and evaluation." Concretely, it names three independently runnable
components — OpenMLE-Gym (build/execute verifiable tasks), OpenMLE-RL (learn operators via SFT + online RL),
OpenMLE-Evo (compose the learned operators into search) — that "align post-training and inference around a
shared action space" rather than each defining its own program-candidate representation.

## In openrsi (grounded)
The shared representation is literal, not just conceptual: the same `Program` dataclass shape — code, a
sandbox-derived score/reward/fitness, parent lineage, and a `generation_mode` — recurs at all three layers
this ingest grounds, as three structurally similar but independently-evolving implementations:
[`Program`](../catalog/OpenMLE-ERL/RL/program_database.md#Program) in the RL trainer (with a paper-Eq.3
three-term fitness recomputed on every insert),
[`Program`](../catalog/OpenMLE-ERL/SFT/tts_search/program_database.md#Program) in the SFT collection harness
(a much simpler `fitness = reward` copy), and
[`Program`](../catalog/OpenMLE-Evo/tts_search/program_database.md#Program) in the inference-time search (a
storage substrate with no fitness computation of its own). Underneath all three, every program's score
ultimately comes from the same sandbox primitive,
[`TaskProcessOutcome`](../catalog/OpenMLE-Gym/openmle_gym/process_runner.md#TaskProcessOutcome), returned by
[`run_task_process`](../catalog/OpenMLE-Gym/openmle_gym/process_runner.md#run_task_process) — the one place
"execution feedback" (the README's phrase) actually gets produced, regardless of which layer requested it.

## Why it matters / when it applies
This explains a genuinely surprising structural fact a reader would otherwise have to discover by diffing
three files: `ProgramDatabase`/`Program` is not one shared library imported three times — it is copy-evolved
independently per layer, with real behavioral differences (see the RL vs. SFT program-database concept pages'
"See also" cross-comparison). The README's "shared action space" framing is true at the *design* level (one
operator vocabulary, one sandbox contract) but not at the *implementation-sharing* level — each layer owns its
own copy of the record type and can (and does) diverge in what it computes from it.

## Connections
- Code concepts: [`OpenMLE-ERL-RL-program_database`](../concepts/OpenMLE-ERL-RL-program_database.md),
  [`OpenMLE-ERL-SFT-tts_search-program_database`](../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
  (its "See also" section is the direct three-term-fitness-vs-reward-copy comparison this doc-concept
  summarizes), [`OpenMLE-Evo-tts_search-program_database`](../concepts/OpenMLE-Evo-tts_search-program_database.md),
  [`OpenMLE-Gym-openmle_gym-process_runner`](../concepts/OpenMLE-Gym-openmle_gym-process_runner.md) — the
  shared sandbox-execution primitive underneath all three.
- Module catalogs: [`OpenMLE-ERL/RL/program_database.md`](../catalog/OpenMLE-ERL/RL/program_database.md),
  [`OpenMLE-ERL/SFT/tts_search/program_database.md`](../catalog/OpenMLE-ERL/SFT/tts_search/program_database.md),
  [`OpenMLE-Evo/tts_search/program_database.md`](../catalog/OpenMLE-Evo/tts_search/program_database.md),
  [`OpenMLE-Gym/openmle_gym/process_runner.md`](../catalog/OpenMLE-Gym/openmle_gym/process_runner.md).
- Related doc-concepts: [`trainable-atomic-operators`](trainable-atomic-operators.md) — the operator-vocabulary
  side of the same "shared action space" claim; [`openmle-evo-max-profile`](openmle-evo-max-profile.md).
- Cross-repo: [`meta-evolution`](../../../concepts/meta-evolution.md) — the search-produces-experience,
  experience-enters-training loop this doc-concept's opening quote describes.

## Source
Extracted from `README.md` (sections "📖 OpenRSI" and "🧩 OpenMLE: The Executable Stack"), kept in place.
