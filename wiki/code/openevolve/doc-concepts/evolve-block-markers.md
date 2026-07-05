---
title: EVOLVE-BLOCK markers — declaring what an LLM is allowed to mutate
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# EVOLVE-BLOCK markers — declaring what an LLM is allowed to mutate

## Definition

`# EVOLVE-BLOCK-START` / `# EVOLVE-BLOCK-END` are plain-text comment markers a user wraps around the
part(s) of an initial program that are open to mutation. Everything outside the markers — imports,
harness code, a `main()` that invokes the evolving function — is a fixed skeleton the LLM is not asked
to touch. The README frames this as the load-bearing contract between a user and OpenEvolve: it is how
a user tells the evolutionary loop "optimize *this*, leave the rest alone" without needing a separate
config schema for scope.

## In openevolve (grounded)

The markers are parsed by
[`parse_evolve_blocks`](../catalog/openevolve/utils/code_utils.md#parse_evolve_blocks) in
`openevolve/utils/code_utils.py` — the same module that implements the SEARCH/REPLACE diff mechanism
documented on [`openevolve-utils-code_utils.md`](../concepts/openevolve-utils-code_utils.md). It walks
the source line-by-line, and while a `# EVOLVE-BLOCK-START` line is "open," it accumulates lines until
the matching `# EVOLVE-BLOCK-END`, returning `(start_line, end_line, block_content)` tuples — the same
plain-text-scanning philosophy the diff-application code uses elsewhere in that module (no AST, no
parser, just string matching).

The library entry point (`openevolve/api.py`, see
[`openevolve-api.md`](../concepts/openevolve-api.md)) leans on the markers being *optional* input rather
than a hard requirement: [`run_evolution`](../catalog/openevolve/api.md#run_evolution) auto-wraps a bare
code string in `EVOLVE-BLOCK-START`/`END` if it doesn't already contain the marker (checked with
`"EVOLVE-BLOCK-START" not in code`), so a caller who supplies a whole small program without markers gets
the entire thing treated as evolvable by default. The two convenience wrappers go further:
[`evolve_function`](../catalog/openevolve/api.md#evolve_function) and
[`evolve_algorithm`](../catalog/openevolve/api.md#evolve_algorithm) each serialize a user's in-memory
Python function/class to source text via `inspect.getsource`, then programmatically **insert** the
markers around just the function body or class body if the source doesn't already have them — so a
caller who hands over a bare Python callable never has to think about the marker syntax at all; the
scoping decision ("evolve the whole function, not the surrounding module") is made for them.

## Why it matters / when it applies

The markers exist because OpenEvolve's mutation operator (an LLM proposing SEARCH/REPLACE diffs, see
[`openevolve-llm-ensemble.md`](../concepts/openevolve-llm-ensemble.md)) has no other signal for scope —
there is no separate "allowed paths" config, no AST-level annotation, no decorator. A user who wants to
protect a function signature, an external API contract, or safety-critical logic from mutation keeps it
outside the markers; the README's "Crafting Effective System Messages" guidance (see
[`system-message-design.md`](system-message-design.md)) reinforces this at the prompt level too ("MUST
NOT CHANGE: kernel function signature...") — the marker is the structural guarantee, and the system
message is the natural-language reinforcement of the same boundary.

## Connections

- Code concepts: [SEARCH/REPLACE diffs — turning an LLM's text output into a child program](../concepts/openevolve-utils-code_utils.md)
  — the sibling mechanism in the same module that mutates what the markers scope.
  [The library entry point](../concepts/openevolve-api.md) — where markers are auto-inserted for callers
  who don't supply them.
- Module catalogs: [openevolve/utils/code_utils.py](../catalog/openevolve/utils/code_utils.md),
  [openevolve/api.py](../catalog/openevolve/api.md).
- Related doc-concepts: [System message design](system-message-design.md) — the natural-language
  reinforcement of the same "what's allowed to change" boundary.

## Source

Extracted from `README.md` (kept in place), specifically the Quick Start code sample and the
"Code Evolution Markers" section of the repo's own `CLAUDE.md`.
