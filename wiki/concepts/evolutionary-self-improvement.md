# Evolutionary self-improvement

**Evolutionary self-improvement** is a search strategy for self-modifying agents that replaces a single
hill-climbing lineage (always mutate the current best) with a **growing archive** of every accepted variant,
sampled for future mutation roughly in proportion to performance but *not* exclusively from the best node —
so weaker, even currently underperforming, variants remain eligible to be resampled and built upon later.

## Why archives beat hill-climbing

A pure hill-climber only ever branches from its single best-known point. If the best current line requires
passing through an intermediate state that scores *worse* than its parent before it can reach a much better
descendant, hill-climbing will never find that path — it prunes anything that doesn't immediately improve.
An archive-based search keeps every variant that still meets a minimal viability bar (e.g., "still compiles
and can still edit code") and gives all of them a non-zero chance of being selected again, so a temporarily
weak node can still serve as a **stepping stone** to a later breakthrough.

## In this wiki's papers

- [**Darwin Gödel Machine**](../sources/darwin-godel-machine.md) is the clearest instance in this wiki: it
  maintains an archive of every self-modified coding agent it has produced, with parent-selection roughly
  proportional to a sigmoid of performance times an inverse-novelty (`1/(1+children)`) bonus, sampled
  categorically so every archive member keeps non-zero selection probability. The paper demonstrates two
  concrete lineages (SWE-bench iterations 4 and 56) where the eventual best agent passed through nodes that
  temporarily scored *below* their parent — paths a hill-climber would have discarded. An ablation that
  removes only this property (`DGM Greedy`: always branch from the single best-scoring node, per Robeyns et
  al. 2025) underperforms the full archive-based version on both benchmarks (39.7%/30.0% vs. 50.0%/38.0%),
  isolating archive-based exploration as a distinct, load-bearing ingredient rather than an artifact of
  simply having *an* archive at all.

> [!inferred] This is the same "keep multiple good-enough branches alive, not just the current best" idea
> that shows up more narrowly in this wiki's `autoresearch` harness only as a *single-branch* ratchet
> (keep the new version only if it beats the current one, discard otherwise, no archive of alternates) —
> see [`../code/autoresearch/overview.md`](../code/autoresearch/overview.md). `autoresearch` is the special
> case of this concept with archive size 1.

> [!inferred] [**Bilevel Autoresearch**](../sources/bilevel-autoresearch.md)'s outer "Level 2" is the same
> "archive size 1" special case already noted above for `autoresearch`'s ratchet — but one level up the
> stack. At any time there is exactly one active search-mechanism module; a newly generated one is
> import-validated and then either replaces it outright or is discarded (revert-on-failure), with no growing
> population of surviving alternative mechanisms and no stepping-stone resampling of a temporarily-worse
> mechanism. So this wiki now has the same hill-climbing-vs-archive distinction recurring at two different
> altitudes: `autoresearch` hill-climbs over *task configs*, Bilevel Autoresearch's Level 2 hill-climbs over
> *search mechanisms*, and only DGM runs a genuine archive — and only over the whole agent scaffold, not a
> narrower mechanism slice.

## How the implementations differ

Among this wiki's ingested code silos, **only DGM implements this concept as a genuine archive** — and the
grounded code makes the contrast with the other silos' search shapes precise:

- **dgm** ([`DGM_outer`](../code/dgm/concepts/DGM_outer.md)) keeps a *growing* `archive` list of every viable
  agent variant and samples the next parent *categorically* (default `score_child_prop`: a sigmoid of score
  times an inverse-child-count novelty term, via `random.choices`, never `argmax`), so a temporarily-worse
  variant retains non-zero selection probability and can serve as a stepping stone. Admission is `keep_all`
  gated only by a "still compiles" viability check — not a fitness ratchet. This is the one true archive here.
- **ai-scientist-v2**'s agentic tree search
  ([`ParallelAgent`](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md)) keeps a
  multi-node frontier and expands the best-scoring leaf — a *tree*, not a flat archive, and driven by an
  LLM/VLM verdict rather than a benchmark re-score. It explores multiple branches, but selection is best-first
  within one experiment tree, not stepping-stone resampling of a persistent population of whole agents.
- **pi-autoresearch-vkf**'s search tree
  ([`tree.ts`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md)) is verified
  (its own source shows `selectExpansion` never calls `frontier`) to *hill-climb from a single best node* —
  an archive of size 1 with parent-relative scoring, closer to a ratchet than to DGM's population.
- **autoresearch** ([`overview`](../code/autoresearch/overview.md)) is the pure single-branch ratchet: keep
  the new version only if it beats the current one, discard otherwise — archive size 1, no stepping stones.

So the four silos form a ladder from ratchet (autoresearch) → single-node hill-climb (pi-autoresearch-vkf) →
best-first tree (ai-scientist-v2) → genuine growing archive (dgm), and only the last keeps every viable
variant selectable.

## See also
- [`self-referential-code-rewriting`](self-referential-code-rewriting.md)
- [`mechanism-level-self-improvement`](mechanism-level-self-improvement.md) — Bilevel Autoresearch's Level 2 as the "archive size 1" mechanism-level case contrasted above
- [`../sources/darwin-godel-machine.md`](../sources/darwin-godel-machine.md)
- [`../topics/autoresearch.md`](../topics/autoresearch.md)
- [`../code/bilevel-autoresearch/overview.md`](../code/bilevel-autoresearch/overview.md) — the contrastive silo: one active mechanism, generate-then-activate-or-revert, no growing archive

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **evolutionary-self-improvement** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [dgm](../code/dgm/concepts/DGM_outer.md) — The DGM outer loop — archive and stepping-stone parent selection
<!-- connect:auto:end -->
