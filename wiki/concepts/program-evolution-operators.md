# Program-evolution operators (Draft / Improve / Debug / Crossover)

**Program-evolution operators** are the small, named vocabulary of transformations an LLM-driven search
applies to executable candidate programs. Rather than one undifferentiated "propose a better program" call,
the harness picks an *operator* and constructs a context appropriate to it. The recurring four-operator
vocabulary across this wiki's systems:

| Operator | Arity | Input context | Failure mode it addresses |
|---|---|---|---|
| **Draft** | 0 parents | task spec + data description | cold start; population diversity |
| **Improve** | 1 parent | one scored program + its execution feedback | incremental refinement of a working solution |
| **Debug** | 1 parent | one *failed* program + its error | a candidate that never produced a score |
| **Crossover** | 2 parents | two scored programs | two branches with *complementary* strengths that neither can reach alone |

The vocabulary originates in **AIDE**-style code-space exploration (Jiang et al. 2025) and **AIRA**-style
executable MLE search (Toledo et al. 2025; Hambardzumyan et al. 2026), and is adopted wholesale by
[Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md) (§4.1).

## Why the split matters

An operator is not just a prompt label — it determines **what evidence the model is shown**, and that turns
out to dominate search cost. [OpenMLE-Evo](../sources/frontis-ma1.md) builds a different bounded context per
operator (§5.4):

- `Improve` — the parent's deterministic record (score, delta-vs-parent, method family, runtime, rank,
  incumbent status, novelty) + a **vertical** trace of recent ancestors + a **horizontal** set of direct
  siblings, ranked by the same score/gain/novelty utility used for parent selection, so the operator can
  contrast its trajectory against nearby alternatives rather than unrelated programs.
- `Crossover` — the same construction for *both* parents, plus a **method-family complementarity** cue.
- `Debug` — prior attempts sharing the **same error signature**, falling back to recent attempts when no
  exact match exists.

Measured effect versus original AIRA-Evo, which supplies all operators broadly similar free-form histories
(§6.5, Figure 16, 66 matched task–runs, same checkpoint and seed): `Improve` prompts shrink 102.8K → 35.7K
mean characters (−65.3%) and 389.0K → 54.3K at p99 (**−86.1%**); `Crossover` 140.4K → 55.3K mean and
419.2K → 78.4K at p99. Total model tokens fall 41.7% while evaluated nodes fall only 12.4% — the saving is
in making each expansion cheaper, not in searching less — and new-best validation updates per million
tokens rise **1.77 → 3.27 (+84.3%)**.

## Crossover is the operator most systems don't have

`Draft`/`Improve`/`Debug` are recognizable in nearly every agentic search: propose, refine, repair.
**`Crossover` is the differentiator** — it requires a *population* with more than one live branch, which a
single-lineage hill-climber structurally cannot supply. Frontis-MA1's evidence that it carries the
long-horizon gain:

- On `leaf-classification`, `Debug` establishes viable image and tabular branches, then `Crossover` fuses
  them and a late `Improve` upgrades the fused representation; the two account for **85.0% of total
  validation gain** (held-out Human Rank 0.9455, Bronze). On `mlsp-2013-birds`, **91.9%**.
- The `nomad2018` case study (§6.5, Figure 17) is the cleanest contrast: original AIRA-Evo follows one
  lineage through **seven successive `Debug` attempts**, each inheriting an expanding history, ending at
  val RMSE 0.06633. OpenMLE-Evo instead forms a targeted `Crossover` from a physics-features parent and a
  robust-parser parent while excluding two known sibling failures as negative evidence → val 0.06087 /
  held-out 0.05410 (−8.2% / −11.3%). The paper's framing: memory converts "distinct branch strengths and
  known failures into a bounded recombination request instead of repeatedly repairing one lineage."

> [!inferred] This is a sharper version of the stepping-stone argument on
> [`evolutionary-self-improvement`](evolutionary-self-improvement.md). An archive lets a temporarily-worse
> variant be *resampled*; `Crossover` lets two surviving variants be *combined*. The first needs a
> population that doesn't collapse; the second additionally needs an operator that can read two parents at
> once. This wiki's silos mostly have the first without the second — `autoresearch`, pi-autoresearch-vkf
> and Bilevel Autoresearch have no recombination step at all, DGM's archive is sampled one parent at a
> time, and ai-scientist-v2's tree expands single nodes (its aggregation nodes combine *replication
> outputs*, not two independent solution branches).

## Operators as training targets, not just prompt roles

Frontis-MA1's contribution is making these four the **shared interface between post-training and
inference** — SFT and RL train exactly the transformations the search later composes. The design rationale
(§4.1): training whole controller trajectories yields sparse, controller-specific supervision, whereas a
compact set of reusable local transformations can be composed by *different* search procedures under one
sandbox protocol. Local skill in the weights, global composition in the harness. See
[`meta-evolution`](meta-evolution.md).

The SFT corpus is collected along the operator split (§4.2): a *parallel path* of independently sampled,
threshold-filtered `Draft` solutions (**17,245** full-response examples) and an *evolutionary path* of
`Improve`/`Debug`/`Crossover` steps over already-executed programs (**9,014** trajectory-step examples),
**26,259** total. A neat detail: when a valid endpoint only emerges after a run of repeated `Debug` steps,
collection traces back to the preceding non-debug operator and keeps only the useful steps of that repair
trace — rather than supervising on the whole flailing sequence.

The paper's own motivation for training the non-`Draft` operators at all: "Evolutionary search depends on
learning revisions, not only fresh drafts" (§4 takeaway, p.10). A controller invokes these hundreds or
thousands of times, so one-shot solution generation is the wrong capability to optimize.

> [!inferred] **Code-grounding [openrsi](../code/openrsi/overview.md) qualifies the paragraph above.** Every
> claim in this section is accurate as a description of the paper — but reading the actual wired code paths
> shows the four-operator vocabulary is not realized uniformly. The primary SFT collection scheduler's
> [`GreedySearch`](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md) and the RL
> rollout's [`AIRAGreedySearch`](../code/openrsi/concepts/OpenMLE-ERL-RL-generate_mle.md) both only ever emit
> `draft`/`improve` as `generation_mode` — "Debug" there is a parent-selection heuristic *inside* Improve
> (pick a currently-failing program as the parent), not a distinct prompt template, and "Crossover" never
> appears in either path at all. The one place `generation_mode` genuinely reads `"debug"`/`"crossover"` is
> the **vendored, third-party** AIRA-Dojo `Evolutionary` solver wrapped by `single_task_runner.py` — reading
> its own real `_draft`/`_improve`/`_debug`/`_crossover` methods, not Frontis's own harness. Three independent
> readings (the scheduler, its tree-search event log, and its program database) converged on this
> independently; see the [openrsi overview](../code/openrsi/overview.md)'s comparison table for the
> per-mechanism detail. The released **26,259-example SFT corpus** and the paper's headline results may still
> be exactly as reported — nothing here contradicts the paper's *numbers* — but a reader reproducing "the
> operator-conditioned policy" from this specific released harness should know Crossover's code path is
> vendored infrastructure, not something Frontis wrote or that this repo's primary scheduler drives.

## How this wiki's other systems realize the same idea

- **[openevolve](../code/openevolve/overview.md) / AlphaEvolve** — collapses the vocabulary to a *single*
  mutation operator: an LLM emits a
  [SEARCH/REPLACE diff](../code/openevolve/concepts/openevolve-utils-code_utils.md) against one parent,
  with "inspiration" programs supplied as context by the
  [PromptSampler](../code/openevolve/concepts/openevolve-prompt-sampler.md). There is no distinct
  Debug-vs-Improve dispatch and no two-parent recombination call — diversity comes from the MAP-Elites ×
  island [database](../code/openevolve/concepts/openevolve-database.md) instead of from an operator.
- **[ai-scientist-v2](../code/ai-scientist-v2/overview.md)** — comes closest structurally: its
  [ParallelAgent](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) has an
  explicit *debug branch* (fixed debug probability, max debug depth) separate from best-first expansion of
  non-buggy nodes, i.e. `Debug` vs. `Improve` as distinct moves — but the decision is a probability, not a
  trained, context-shaped operator, and there is no `Crossover`.
- **[dgm](../code/dgm/overview.md)** — one operator only (diagnose-then-edit the agent's own code), applied
  to a single sampled archive parent.
- **[rd-agent](../code/rd-agent/overview.md)** — splits the work along a different seam entirely (Research
  proposes, Development implements); its Co-STEER
  [evolving framework](../code/rd-agent/concepts/rdagent-core-evolving_framework.md) is a
  propose/evaluate/refine loop closer to `Improve`+`Debug` fused, with no recombination.

> [!inferred] Read across the silos, the operator vocabulary and the population shape are two independent
> design axes that this wiki had been conflating. openevolve has a rich population and one operator;
> ai-scientist-v2 has a tree and two-ish operators; OpenMLE-Evo has both a population *and* four trained
> operators, and its evidence (85–92% of gain from late `Improve`/`Crossover`) argues the second axis is
> where the long-horizon returns are.

## The live disagreement: specialized operators vs. one universal operator

[KernelEvolve](../sources/kernelevolve.md) (Meta, ISCA 2026) argues the opposite of this page's premise. It
replaces `Draft`/`Debug`/`Improve` with a **single universal operator** whose behavior comes entirely from
retrieval-augmented, runtime-synthesized context, on the grounds that a specialized operator "imposes
cognitive constraints on the model's reasoning" — a `Debug` prompt is error-focused whether the fault is
algorithmic or a memory-access pattern — and that operator boundaries prevent one step from simultaneously
fixing a numerical error *and* restructuring memory access. See
[`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md).

**Both papers cite the same premise** (Toledo et al., 2025: performance bottlenecks in LLM code generation
stem from *operator design* rather than search algorithms) and agree on the diagnosis. They split on the
cure — but less than it first appears, because KernelEvolve's actual target is the **static prompt
template**, not the operator vocabulary. OpenMLE-Evo's operators are not static-template either: §5.4 builds
a *different* bounded context per operator from live search state (ancestors + siblings for `Improve`, both
parents plus a complementarity cue for `Crossover`, same-error-signature retrieval for `Debug`), and §5.3
defers LLM memory synthesis until *after* an operator has selected its nodes. Both systems concluded that
what the model is shown must be computed at runtime; they differ on whether the *name* of the move is a
useful index into that computation.

Where the evidence now stands, with neither paper running the other's experiment:

- **For specialized operators.** OpenMLE-Evo's `nomad2018` case study is the closest thing to a direct test:
  a single-lineage search that repeatedly applies repair (seven successive `Debug` steps on one branch)
  loses to one targeted `Crossover` drawing on two complementary parents (−8.2% val, −11.3% held-out RMSE).
  And late `Improve`/`Crossover` carry 85.0–91.9% of total validation gain in the two trajectory studies.
  Distinguishing "repair this" from "recombine these two" changed what the search *did*, not just how it
  was prompted.
- **For the universal operator.** KernelEvolve's own evidence is deployment-scale rather than ablational —
  480/480 correct across 160 operators × 3 platforms, 100% KernelBench — and it never ablates the universal
  operator against a specialized menu.

> [!inferred] **The uncomfortable asymmetry neither paper states: a universal operator has nothing to
> post-train against.** Frontis-MA1's whole meta-evolution loop depends on operators being a *fixed, named,
> low-cardinality vocabulary* — that is what lets a verified evolutionary transition become a labeled SFT
> example and an RL rollout for the same move the harness will later invoke
> ([`meta-evolution`](meta-evolution.md)). Dissolve the vocabulary into one context-conditioned operator and
> you keep the flexibility but lose the crisp training interface; you would be training "respond well to
> arbitrary retrieved context," which is just general capability. So the choice may not be
> specialized-vs-universal on the merits of any one search run, but **frozen-model vs. trainable-model
> architecture**: if the backbone is fixed (KernelEvolve wraps frontier models it doesn't own), spend the
> complexity budget on retrieval; if you intend to train the backbone, you need the interface. That
> reframing is this wiki's, not either paper's.

## See also
- [`meta-evolution`](meta-evolution.md) — what makes these operators training targets rather than prompt roles
- [`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md) — the opposing design
- [`evolutionary-algorithm-discovery`](evolutionary-algorithm-discovery.md) — the single-mutation-operator lineage
- [`agentic-tree-search`](agentic-tree-search.md) — the AIDE ancestry these operators come from
- [`../sources/frontis-ma1.md`](../sources/frontis-ma1.md)

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **program-evolution-operators** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-airaevo_experience.md) — airaevo_experience.py — the original-AIRA-Evo selection/memory adapter for RL rollouts
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-generate_mle.md) — The RL rollout — operator-conditioned generation and reward computation
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-program_database.md) — Program database — three-term fitness and operator-conditioned parent sampling
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-program_database.md) — Program database — reward-as-fitness store behind SFT's greedy draft/improve search
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md) — GeneratorService — the operator-agnostic LLM caller behind tts_search's SFT trajectory collection
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md) — Scheduler — the tts_search orchestrator behind the SFT evolutionary path
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md) — Tree-search state — the append-only event log and resumable snapshot behind SFT collection
- [openrsi](../code/openrsi/concepts/OpenMLE-Evo-tts_search-program_database.md) — Program database — the storage substrate, not the selection policy
<!-- connect:auto:end -->
