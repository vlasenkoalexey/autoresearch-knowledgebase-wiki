---
title: "Hypothesis Generation"
type: concept
tags: [autoresearch, scientific-discovery, idea-generation]
created: 2026-07-04
updated: 2026-07-04
sources: 1
---

The task of proposing a **novel, testable claim or mechanism** for a research goal — as distinct from
literature synthesis or retrieval, which reconstructs what is already known. A hypothesis-generation system
is judged on whether its outputs are plausible, novel (not already published, even in a modified form),
testable within stated constraints, and safe, not on retrieval accuracy.

## As instantiated by Co-Scientist

[Co-Scientist](../sources/ai-co-scientist.md) (Google, arXiv:2502.18864) is this wiki's fullest working
instance of hypothesis generation as a *system*, not just a prompting task. It decomposes the job across
six specialized agents built on Gemini:

- **Generation** produces the initial candidates — via web-search-grounded literature exploration, simulated
  multi-turn scientific debate (self-play), iterative identification of testable sub-assumptions, and
  "research expansion" that reads the prior run's research overview to find unexplored territory.
- **Reflection** filters and grounds candidates through several review modes (initial/fast, full/web-search-
  grounded, deep verification that recursively checks sub-assumptions, observation review against existing
  experimental data, and step-wise simulation review).
- **Ranking** orchestrates an **Elo tournament** (initial rating 1200) with scientific-debate-style pairwise
  matches for top contenders, prioritizing matches between similar hypotheses (via the Proximity agent) and
  toward currently-top-ranked ones.
- **Evolution** generates new candidates derived from top performers (grounding-driven repair, combination,
  simplification, deliberate divergence) — it never edits a hypothesis in place; every evolved idea must
  re-earn its rank in the tournament.
- **Meta-review** closes the loop by synthesizing recurring failure patterns across all reviews/debates into
  feedback appended to other agents' prompts next iteration (in-context, not gradient-based), and produces a
  final research-overview synthesis of the top-ranked hypotheses.

Ablations tie concrete gains to this decomposition: Reflection's novelty judgment is unreliable without web
search (6.14/10 vs. a correct 2.38/10 novelty score on known non-novel ideas); debate-style ranking beats
plain pairwise comparison and reduces positional bias; Evolution's refinement raised GPQA precision from
70.9% to 75.4%. Across 203 research goals, both average-top-10 and best-Elo climbed with more test-time
compute, with no observed saturation — the paper's central claim that scaling test-time compute, not just
model size, drives hypothesis quality.

## The generation/validation split

Co-Scientist generates and ranks hypotheses purely over text; it does not execute the experiments that would
confirm them. All three of its biomedical validations were confirmed by human-run wet-lab assays outside the
system. See [`../topics/autoresearch.md`](../topics/autoresearch.md) for the contrast with systems (like The
AI Scientist-v2) whose target experiments are themselves executable code, letting them close the loop
in-system.

## Where else this appears

The roadmap survey [`ai-for-auto-research-roadmap.md`](../sources/ai-for-auto-research-roadmap.md)
catalogues hypothesis/idea generation as its own lifecycle stage (**S1 Idea Generation**), splitting it into
LLM-internal-knowledge methods, external-signal-driven methods (knowledge-graph reasoning, retrieval, trend
analysis), and multi-agent collaborative generation — the category Co-Scientist's Generation/Evolution
agents instantiate. That survey also documents a broader "ideation–execution gap": LLM-generated ideas score
higher on novelty than human ideas but degrade more after implementation, and a separate "Artificial
Hivemind" finding suggests LLM idea generation clusters in narrow regions of idea space (a structural
diversity-collapse risk not obviously solved by adding more agents) — a caution worth weighing against
Co-Scientist's own Elo-based framing of "quality improving with more compute."

## A structural, non-LLM instance: pi-autoresearch-vkf

Where Co-Scientist and ai-scientist-v2's ideation both generate hypotheses by having an LLM read/synthesize
literature, [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)'s
[`synthesis.ts`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md) generates
them by mining **structural tensions in its own already-verified memory** — three deterministic functions over
lexical/mechanism/context similarity: `findContradictions` (high topic overlap, diverging outcome — "these two
trusted claims disagree, why?"), `findTransfers` (high mechanism similarity, low context similarity — "this
mechanism worked *there*, does it work *here*?"), and `findCompositions` (two independently-verified,
low-overlap claims combined into one hypothesis "no single source states"). It has no debate, no ranking
tournament, no Elo — novel-hypothesis discovery is a deterministic query over VKF's trust-tagged card store
rather than an LLM-mediated generation step. The repo's own benchmark harness is built specifically to isolate
this: in its deterministic ground-truth scenarios, the global optimum is always a *synthesized* idea, and a
blind ranking loop (no synthesis) finds it 0% of the time versus 100% for the synthesis-enabled policy.

## See also

- [`../sources/ai-co-scientist.md`](../sources/ai-co-scientist.md)
- [`../sources/ai-for-auto-research-roadmap.md`](../sources/ai-for-auto-research-roadmap.md)
- [`multi-agent-debate`](multi-agent-debate.md)
- [`../topics/autoresearch.md`](../topics/autoresearch.md)

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **hypothesis-generation** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-article_opt-mechanism_research.md) — article_opt mechanism research (Level 2)
- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-train_opt-mechanism_research.md) — TrainMechanismResearcher — Level 2's Explore→Critique→Specify→Generate dialogue
- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-train_opt-runner.md) — TrainRunner — the Level 1 inner loop
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-perform_ideation_temp_free.md) — Ideation — literature-grounded idea generation
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md) — Hypothesis synthesis — contradiction mining, transfer, and composition
<!-- connect:auto:end -->
