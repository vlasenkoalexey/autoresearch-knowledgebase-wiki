# Wiki log

Append-only, chronological. One entry per operation, prefixed so it stays greppable with plain Unix
tools (`grep '^## \[' wiki/log.md | tail -5`). Prefixes: `ingest-code | <slug>` (code repo via the
skill), `ingest | <source>` (article/doc/note), `connect | <scope>` (cross-repo), `lint | <scope>`,
`note | <title>`. Newest at the bottom.

## [2026-07-04] ingest-code | autoresearch
Ingested [karpathy/autoresearch](https://github.com/karpathy/autoresearch) @ `228791f` as a submodule under
`raw/code/autoresearch`. 177 symbols, 2 modules. Wrote concept pages
[train](code/autoresearch/concepts/train.md) and [prepare](code/autoresearch/concepts/prepare.md), an
[overview](code/autoresearch/overview.md), and 4 doc-concepts from `program.md`/`README.md` (autonomous
experiment loop, experiment logging, fixed time budget, single-file agent edits). Finalize green, 100%
symbol coverage (7/7 classes). Adversarial verify caught and fixed one error (Muon momentum is
step-indexed, not `progress`-indexed). Registered in [`index.md`](index.md).
