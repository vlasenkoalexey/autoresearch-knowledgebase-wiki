---
slug: bilevel-autoresearch
repo: https://github.com/EdwardOptimization/Bilevel-Autoresearch
acquire: submodule
docs: [README.md]
synthesis_focus: the outer bilevel autoresearch loop — how Level 1.5 reads the inner loop's proposal/outcome trace and adjusts freeze/unfreeze parameters, and how Level 2's 4-round Explore→Critique→Specify→Generate dialogue reads the inner loop's runner code + trace, writes new Python search-mechanism code (Tabu Search, multi-armed-bandit proposal, orthogonal design-of-experiments), and validates it by dynamic import before activation, reverting to the prior mechanism on failure
---

## Concepts
