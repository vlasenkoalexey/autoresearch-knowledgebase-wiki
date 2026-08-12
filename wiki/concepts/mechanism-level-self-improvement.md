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

## Grounded in code (bilevel-autoresearch silo)

With the [`bilevel-autoresearch`](../code/bilevel-autoresearch/overview.md) silo ingested, this concept is now the
only one in the wiki backed by a running mechanism-generator rather than only a paper. The machinery is concrete:
a fixed, human-authored 4-round Explore→Critique→Specify→Generate dialogue lives once in
[`core.base_mechanism_research`](../code/bilevel-autoresearch/concepts/core-base_mechanism_research.md) and is
subclassed per domain to *write new Python* — a training-search mechanism in
[`TrainMechanismResearcher`](../code/bilevel-autoresearch/concepts/domains-train_opt-mechanism_research.md) (Tabu
Search / bandit / orthogonal-exploration code patched into the runner, validated by an out-of-process import and
reverted on failure) and a new pipeline stage in
[`article_opt`](../code/bilevel-autoresearch/concepts/domains-article_opt-mechanism_research.md). The grounding
sharpens the archive-ladder position above: the generator keeps **exactly one** active mechanism (generate →
import-validate → activate-or-revert, archive size 1), which is why bilevel-autoresearch's silo pages are
*deliberately not* tagged [`evolutionary-self-improvement`](evolutionary-self-improvement.md) (no growing
population) or [`self-referential-code-rewriting`](self-referential-code-rewriting.md) (the dialogue that writes
the code is itself never rewritten). Contrast the fixed floor one level down: the inner loop it wraps is exactly
[`autoresearch`](../code/autoresearch/overview.md)'s human-authored keep-if-better ratchet, which
mechanism-level self-improvement is what would, in principle, replace.

## The rung above: when the mechanism lives in weights, not text

This concept's whole framing — artifact-level vs. mechanism-level — assumes the mechanism is **text a
frozen model reads and rewrites**: Python search code, a prompt, a skill, an evaluator. It is worth naming
what that assumption excludes. [Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md) improves the *proposal
mechanism* too, but by **post-training the model that proposes**, on execution outcomes the search itself
generated. Nothing textual changes: the harness, the operator prompts, and the selection rule are all fixed
and human-authored across the whole run. The mechanism improved by 21 percentage points anyway, because the
mechanism partly *is* the weights. See [`meta-evolution`](meta-evolution.md).

That gives this wiki two orthogonal ways to improve a search mechanism, and they are cleanly separable:

| | Bilevel Autoresearch (Level 2) | Frontis-MA1 (OpenMLE-ERL) |
|---|---|---|
| what changes | the search-mechanism **source code** | the proposal policy's **weights** |
| how | a 4-round LLM dialogue writes Python, dynamically imported | execution-grounded SFT + RL on the same operators |
| validated by | import-check, then activate-or-revert (archive size 1) | held-out benchmark, at fixed harness |
| requires | the mechanism to be legible, editable text | owning the model, and a fixed operator interface |
| measured gain | ~5× Δ`val_bpb` vs. inner loop alone | +21.22 pp Medal Average vs. base model, same harness |

> [!inferred] Neither paper knows about the other's axis, and combining them is unclaimed territory.
> Bilevel Autoresearch's Level 2 rewrites the mechanism a **frozen** model executes; Frontis-MA1 trains a
> model to execute a **fixed** mechanism better. A system doing both would generate a new search mechanism
> *and* fine-tune its proposer against that mechanism's own trace — which is roughly Frontis-MA1's stated
> limitation #4 ("evolution operates primarily over candidate solutions, while the evolutionary system
> itself remains largely fixed … a further step is to make the evolutionary system itself an object of
> evolution") answered with Bilevel Autoresearch's Level 2. Worth flagging as the concrete next experiment
> this pair of papers implies, since neither one proposes it.

## See also
- [`meta-evolution`](meta-evolution.md) — the same target reached through weights instead of text
- [`self-referential-code-rewriting`](self-referential-code-rewriting.md)
- [`evolutionary-self-improvement`](evolutionary-self-improvement.md)
- [`../sources/bilevel-autoresearch.md`](../sources/bilevel-autoresearch.md)
- [`../code/autoresearch/overview.md`](../code/autoresearch/overview.md)
- [`../code/bilevel-autoresearch/overview.md`](../code/bilevel-autoresearch/overview.md)

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **mechanism-level-self-improvement** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/core-base_mechanism_research.md) — core.base_mechanism_research — the shared Level 2 Explore→Critique→Specify→Generate protocol
- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-article_opt-cli.md) — article_opt CLI
- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-article_opt-mechanism_research.md) — article_opt mechanism research (Level 2)
- [bilevel-autoresearch](../code/bilevel-autoresearch/concepts/domains-train_opt-mechanism_research.md) — TrainMechanismResearcher — Level 2's Explore→Critique→Specify→Generate dialogue
<!-- connect:auto:end -->
