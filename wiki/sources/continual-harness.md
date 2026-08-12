# Continual Harness: Online Adaptation for Self-Improving Foundation Agents

Seth Karten, Joel Zhang, Tersoo Upaa Jr, Ruirong Feng, Wenzhe Li, Chengshuai Shi, Chi Jin, Kiran
Vodrahalli (Princeton University, ARISE Foundation, Google DeepMind) —
[arXiv:2605.09998](https://arxiv.org/abs/2605.09998). **This, not [the PokéAgent Challenge
paper](pokeagent-challenge.md), is the paper the video's narration actually describes** — its description
links the older benchmark paper by mistake; both trace to the same author and the same (renamed)
repository. Ingested 2026-08-12 as the second of Prime Agent's two core abstractions.

## Overview

The starting observation: coding agents have "harnesses" — Claude Code, Codex, and similar wrap a base
model with a system prompt, tools, and accumulated conventions — but embodied, long-horizon agents mostly
don't have an equivalent. **Gemini Plays Pokémon** (GPP) is the origin case: a human iteratively rewrote
the agent's own harness while it played, and the result was the first AI system to finish Pokémon Blue,
Yellow Legacy on hard mode, and Crystal without losing a single battle. Continual Harness automates that
human role — the loop of watching what's failing and rewriting the scaffold — out of the process.

## Key claims

- **Four editable components, one automated Refiner.** The harness state is a system prompt `p`,
  a set of sub-agents `G`, a library of skills `K`, and memory `M`. Every fixed number of steps, a Refiner
  reads the recent trajectory window, identifies failure signatures (navigation loops, repeated tool-call
  failures, stalled objectives), and runs CRUD (create/read/update/delete) edits across all four —
  rewriting the prompt against observed failures, adding/removing sub-agent entries for repeated
  multi-step patterns, codifying successful sequences into skills, and refreshing stale memory.
- **Reset-free, mid-episode adaptation is the headline mechanism.** Prompt-optimization methods generally
  require an episode boundary to update; Continual Harness edits the harness **in place, inside a single
  continuous run**, so there is no reset between "the agent playing" and "the agent revising how it
  plays."
- **Evaluated on Pokémon Red and Emerald**, starting from a deliberately minimal interface (frames, an
  ASCII text map, button inputs) rather than the hand-engineered `H_expert` scaffold. Against that minimal
  baseline, the paper reports Continual Harness substantially reduces action cost and recovers a majority
  of the gap to the hand-engineered expert harness — the paper's own numeric tables for exactly how much
  were not independently confirmed for this ingest (see caveats).
- **A training extension closes the loop for open-source weights.** An online process-reward co-learning
  pipeline relabels an open-source agent's own rollouts through the Refiner using a frontier model as
  teacher, and uses that signal to update the smaller model's weights — again without resetting the
  environment between training iterations, producing sustained in-game milestone progress on Pokémon Red.
- **One boundary is stated as immutable**: the base system prompt itself is never CRUD-edited by the
  Refiner. Everything built *on top* of it — memories, skills, sub-agent definitions — is the agent's to
  rewrite.

## Techniques referenced
CRUD-based harness self-editing; reset-free / mid-episode online adaptation; failure-signature detection
over a trajectory window; online process-reward co-learning (DAgger-style relabeling) for open-source model
training; snapshot-and-rollback for harness edits.

## Gaps & caveats
- **Numeric results were not independently confirmed for this ingest.** Public summaries describe the
  headline comparison qualitatively ("substantially reduces button-press cost," "recovers a majority of the
  gap to the hand-engineered expert harness") without the underlying table; this page reports that
  qualitative claim rather than a number I could verify directly against the paper's own tables.
- **Repository lineage is a real point of confusion worth stating plainly**: this paper's reference
  implementation lives in `sethkarten/continual-harness`, which is the **renamed** `pokeagent-speedrun`
  repo from [the PokéAgent Challenge paper](pokeagent-challenge.md) — the hand-engineered `H_expert`
  scaffold from that earlier paper survives inside it as one scaffold among several, no longer the headline
  contribution.
- The base-system-prompt-immutable boundary is a design choice stated by the authors, not something this
  ingest independently verified against the implementation (see the code-silo ingest for a grounded check).

## Connections
- [The PokéAgent Challenge](pokeagent-challenge.md) — the earlier paper and benchmark infrastructure this
  one builds on; same lead author, same (renamed) repository.
- [Prime Agent launch post](prime-agent-launch.md) — ships this mechanism as `/refine`, with the same
  immutable-base-prompt boundary and snapshot/rollback described here.
- [Recursive Language Models](recursive-language-models.md) — Prime Agent's other core abstraction; RLM
  handles *what enters context*, Continual Harness handles *how the scaffold itself changes* — orthogonal
  mechanisms combined in one product.
- [`concepts/self-referential-code-rewriting.md`](../concepts/self-referential-code-rewriting.md) — the
  vocabulary key this paper's mechanism plausibly connects to; see the code-silo connect step.

## Sources
- [Continual Harness: Online Adaptation for Self-Improving Foundation Agents](https://arxiv.org/abs/2605.09998),
  Karten et al. — arXiv:2605.09998
- [sethkarten.ai/continual-harness](https://sethkarten.ai/continual-harness/)
- Code: [sethkarten/continual-harness](https://github.com/sethkarten/continual-harness) (renamed from
  `pokeagent-speedrun`)
