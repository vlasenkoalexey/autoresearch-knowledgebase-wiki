# wikify-repo-demo — project memory

## What this is
A working instantiation of the
[Karpathy LLM-wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) that
handles **two kinds of source** in one knowledge base:
- **Code repos** — ingested by the **`wikify-ingest-repo`** skill (which ships with
  [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo), installed into `.agents/skills/` here)
  into a grounded, lint-clean wiki. This is the headline — the repo is the **companion demo for
  wikify-repo**, showing what that tool produces.
- **Articles / docs / notes** — ingested the classic Karpathy way: read the source, write a summary
  page, update the topic and entity pages it touches, cross-link, log.

Both paths feed **one wiki**, one `index.md`, one `log.md`. Code is a powerful *automated* source type
alongside prose; everything below tells the agent how to maintain both.

## The core idea
The usual way an agent uses documents is RAG-shaped: retrieve chunks at query time and reconstruct the
answer from scratch, *every time*. Nothing accumulates. This repo is different: between the raw sources
and your questions sits a **persistent, compounding wiki** the agent builds and keeps current. The
cross-references are already there, the synthesis already reflects everything ingested, and — for code —
the grounding and the dynamic-dispatch seams a call-graph walk misses are already resolved. Compiled
once, kept current, not re-derived per query.

You never hand-write the wiki. **Your job:** curate which sources to add and ask good questions.
**The agent/tooling's job:** the summarizing, cross-referencing, grounding, and bookkeeping.

## Architecture — three layers, two source types
1. **Raw sources — immutable.** Read, never edited.
   - **Code repos** → `raw/code/<slug>/` as a **git submodule** — this demo defaults to
     **`acquire: submodule`** in each `config/<slug>.md`. The committed gitlink + `.gitmodules` *is* the
     pin (reproducible via `git submodule update --init`); the contents aren't vendored as blobs. (The
     tool also supports `acquire: clone` — gitignored clone, pin in state — for huge upstreams.)
   - **Articles / docs / notes** → `raw/sources/`. **Committed** — these *are* your curated source of
     truth (markdown clips, PDFs, transcripts) and must persist.
2. **The wiki — generated, the agent owns it.** Markdown only.
   - **Code** → `wiki/code/<slug>/` (written by the skill): `overview.md`, `concepts/`, `catalog/`,
     `doc-concepts/`.
   - **Prose** → `wiki/sources/<source>.md` (one summary per ingested article) and
     `wiki/topics/<topic>.md` (synthesized entity/concept/topic pages that span sources).
   - **Cross-cutting answers** → `wiki/notes/<note>.md` (filed back from queries; may mix code + prose).
   - **Shared** → `wiki/index.md`, `wiki/log.md`.
3. **The schema — this file.** `CLAUDE.md` / `AGENTS.md` / `GEMINI.md` are thin pointers so Claude Code,
   Codex, and Antigravity read this one brain. Co-evolve it as conventions settle.

## Operations

### Ingest — two paths into one wiki
- **Code repo.** Just say **`ingest <repo-url-or-local-path>`** → runs
  **`.agents/skills/wikify-ingest-repo/SKILL.md`**, which here bootstraps `config/<slug>.md` with
  `acquire: submodule` so the repo lands as a submodule under `raw/code/<slug>`, then
  `prepare` (pin + SCIP-index + symbol graph + packets)
  → synthesize one grounded concept page per packet → `overview.md` → ingest the repo's own docs into
  `doc-concepts/` → `finalize` (citation lint + coverage catalogs + assemble) → the skill's **register
  step** links the repo's `overview.md` into `wiki/index.md` and appends `wiki/log.md` (the format is
  the "Indexing and logging" section below). **Idempotent reconcile** — re-running converges;
  `ingest --ref <commit>` rebuilds only the symbols that moved. From the **second** code repo on, the
  ingest ends by **connecting** the new silo to the others (below).
- **Article / doc / note.** Drop the source in `raw/sources/`, then: read it, discuss takeaways, write a
  summary page at `wiki/sources/<source>.md`, **update or create the topic/entity pages it touches**
  (`wiki/topics/…` — a single source can touch 10–15 pages), add cross-references, note where it
  contradicts existing claims, update `wiki/index.md`, append `wiki/log.md`. Freeform prose with
  citations back to the source file.

### Connect — cross-link the same concept across repos (inline, no new page type)
One silo answers "how does *this repo* do X"; the cross-repo view answers "**who implements X**".
The **`wikify-connect-repo`** skill (invoked at the tail of an ingest, or on request) builds it
**inline, as a normal wiki** — through the concept pages you already curate (`wiki/concepts/*.md`).
`wikify connect` proposes which concepts have implementations across the silos; you pick **which to
connect** (selective — connecting everything drowns the pages); `wikify connect --apply <keys>` then
writes, in regenerable `connect:auto` blocks, a `## In this wiki's repos` list on the concept page
linking **down** to each repo's implementation, and a one-line **up-link** on each silo page. No
side-table, no `_connect/` directory. Optionally add hub prose (a *how they differ* synthesis) in the
concept page *above* the auto block. Connection state is the pages themselves; `--refresh` regenerates
after a new ingest. It never rewrites the linted silo prose.

### Query — let the wiki's structure route you
Read **`index.md` first** to see what exists, then go by what you're asking:

**Code questions** route by page type — don't fall back to grepping raw source:
- *"Which repos implement `<concept>` (a kernel, a technique)?"* → the concept page
  `wiki/concepts/<concept>.md` — its `## In this wiki's repos` block links to each repo's
  implementation (and every implementation links back up).
- *"Where do I start / what are the systems?"* → `wiki/code/<slug>/overview.md` (concepts + diagrams + a map of
  which concept answers which question).
- *"How does `<mechanism>` work, and why?"* → `wiki/code/<slug>/concepts/<concept>.md` (prose + Mermaid
  diagram + woven citations). Per-repo concept pages live under the silo; only the cross-repo
  vocabulary lives at top-level `wiki/concepts/`.
- *"What is `<symbol>` — signature, definition, who calls it?"* → `wiki/code/<slug>/catalog/<module>.md`
  (the symbol's single home: signature, extracted docstring, a relative link to its exact source line,
  importance-ranked **uses-by**).
- *Need line-level certainty?* **Drop to the pinned source** — every catalog entry links to
  `raw/code/<slug>/…` at the pinned commit. The wiki gets you to the right ten lines; the source confirms
  the exact branch/signature/edge case.

**Prose questions** → read the relevant `wiki/topics/<topic>.md` (and the `wiki/sources/…` summaries it
cites); synthesize with citations back to the source pages / raw files.

In both cases: read only the relevant section (don't bulk-read), cite precisely (a catalog anchor
`catalog/<module>.md#<QualifiedName>` for code, a source/topic page for prose), and **file good answers
back** — a reconstructed cross-cutting trace, a cross-repo or cross-source comparison, an invariant you
verified — as a `wiki/notes/…` (or `concepts/…`/`topics/…`) page, linked from `index.md` and logged, so
explorations compound like ingests.

### Lint — health-check both
- **Code** (deterministic gates): `wikify finalize <slug>` (every citation resolves, every mechanism claim
  is cited), `wikify verify <slug>` (adversarial), and **coverage** (set-difference over the symbol table
  → a catalog page per module, so no subsystem is silently dropped). Stale at a new commit → `ingest
  --ref`.
- **Prose** (judgment pass): contradictions between pages, stale claims a newer source superseded, orphan
  pages with no inbound links, concepts mentioned but lacking their own page, gaps worth a web search.
- **Shared**: orphan detection, missing cross-references, staleness across the whole `wiki/`.

## Indexing and logging
- **`wiki/index.md` is read first.** A content catalog with three sections — **Code repos** (link →
  `overview.md`, pinned commit, what it answers), **Topics** (synthesized prose pages), **Sources**
  (ingested articles) — each line a link + one-line summary. Updated on every ingest. At this scale the
  index + `grep` replaces embedding-based RAG.
- **`wiki/log.md` is append-only**, prefixed so it stays greppable
  (`grep '^## \[' wiki/log.md | tail -5`):
  `## [YYYY-MM-DD] ingest-code | <slug>` · `## [YYYY-MM-DD] ingest | <source>` ·
  `## [YYYY-MM-DD] lint | <scope>` · `## [YYYY-MM-DD] note | <title>`.

## Grounding — what makes the wiki trustworthy
- **Code** (strict): synthesis cites **only** symbols in the packet subgraph; uncited claims go in
  `> [!inferred]` blocks; the citation linter is a build gate, not a prompt. Prefer the author's extracted
  docstrings over re-deriving behavior.
- **Prose**: cite the raw source for every claim; flag contradictions instead of silently overwriting; put
  synthesis that goes beyond the sources in `> [!inferred]`.
- **Shared**: **markdown is the only product** — SCIP indexes and build artifacts live in gitignored
  `.cache/`, never in `raw/`.

## Why this works
The tedious part of a knowledge base isn't the reading — it's the bookkeeping: keeping cross-references
current, re-grounding claims when a source (or a commit) moves, representing everything, noticing
contradictions. Humans abandon wikis because that burden outgrows the value. The tooling doesn't get
bored, doesn't forget a cross-reference, rebuilds only the delta, and (for code) grounds every claim in a
real symbol — so the wiki stays maintained because maintenance is near-zero-cost. You curate and question;
the agent does everything else.
