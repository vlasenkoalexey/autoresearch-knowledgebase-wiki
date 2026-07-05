# Mechanism-level self-improvement

**Mechanism-level self-improvement** describes a self-improving agent whose target of modification is not
a one-off artifact used in the current episode (a prompt, a config, a trained model) but the **logic that
generates, evaluates, selects, and revises future artifacts** — the proposal/acceptance/update mechanism
itself. Changing the mechanism doesn't just fix the current run; it changes what *every subsequent* run of
the loop looks like.

## Artifact-level vs. mechanism-level

An artifact-level self-improver optimizes something the loop *uses*: a prompt template, a hyperparameter
config, a skill document. The loop that decides how to propose, accept, or revise that artifact stays fixed.
A mechanism-level self-improver instead optimizes *that decision logic itself* — after a mechanism-level
edit, the next artifact isn't just different in value, it was arrived at by a different search procedure.
Python code is one convenient carrier for a mechanism (explicit, executable, easy to validate before
activation), but the same role can in principle be played by a skill, a prompt, a workflow, an evaluator, a
scientific principle, a world-model assumption, or a memory schema — anything that shapes how future
proposals are generated, evaluated, or revised.

## In this wiki's papers

- [**Bilevel Autoresearch**](../sources/bilevel-autoresearch.md) is this wiki's clearest instance. Its outer
  "Level 2" reads the inner autoresearch loop's runner code and search trace, then writes and injects new
  Python search-mechanism code (Tabu Search, multi-armed-bandit proposal, orthogonal design-of-experiments)
  at runtime — not tuning the inner loop's training config, but replacing the *procedure* that generates
  training-config candidates. The paper explicitly distinguishes this from its own "Level 1.5," which only
  adjusts parameters (freeze/unfreeze, exploration guidance) of the existing, fixed mechanism — a knob on a
  fixed procedure, not a new procedure. A four-group ablation isolates the effect: full mechanism injection
  (Level 1+1.5+2) reached a ~5x improvement over the inner loop alone, while parameter-only adjustment
  (Level 1+1.5) showed no reliable gain over no outer loop at all — evidence, in this benchmark, that the
  mechanism/parameter distinction is not just conceptual but load-bearing.

> [!inferred] This concept sits *between* two other ideas already in this wiki. It's a narrower target than
> [`self-referential-code-rewriting`](self-referential-code-rewriting.md) (Darwin Gödel Machine rewrites its
> entire agent scaffold — tools, prompts, orchestration — and is itself the thing doing the rewriting;
> Bilevel Autoresearch's outer loop only rewrites the inner loop's search mechanism, and is not itself
> rewritten by anything in the paper). And it's a level up from plain task-artifact optimization: this
> wiki's `autoresearch` ratchet ([overview](../code/autoresearch/overview.md)) is mechanism-level
> self-improvement's *fixed floor* — a mechanism (keep-if-better) that Bilevel Autoresearch's Level 2 could,
> in principle, itself be a candidate for replacing, though no paper in this wiki does that yet.

## See also
- [`self-referential-code-rewriting`](self-referential-code-rewriting.md)
- [`evolutionary-self-improvement`](evolutionary-self-improvement.md)
- [`../sources/bilevel-autoresearch.md`](../sources/bilevel-autoresearch.md)
- [`../code/autoresearch/overview.md`](../code/autoresearch/overview.md)
