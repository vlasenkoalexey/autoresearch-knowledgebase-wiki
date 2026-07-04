# autoresearch-knowledgebase-wiki — project memory

## What this is
A **wiki collection of papers on autoresearch and auto-optimization**, built as a working instantiation of
the [Karpathy LLM-wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f). The
headline source type is **papers** — read the source, write a summary page, update the topic and entity
pages it touches, cross-link, log. Topics in scope:
- **Autoresearch** — AI scientists / research agents, automated hypothesis generation and experimentation,
  literature synthesis, self-improving research loops, agentic discovery pipelines.
- **Auto-optimization** — AutoML, hyperparameter optimization, neural-architecture search (NAS), learned
  optimizers, compiler / kernel / schedule auto-tuning, systems and performance optimization.

A second, **optional** source type rides along in the same wiki: **code repos** — when a paper ships an
implementation worth grounding, it can be ingested by the **`wikify-ingest-repo`** skill (which ships with
[wikify-repo](https://github.com/vlasenkoalexey/wikify-repo)) into a grounded, lint-clean code wiki and
connected to the concept pages the papers already describe.

Both paths feed **one wiki**, one `index.md`, one `log.md`. Papers are the core; code is a powerful
*automated* source type alongside them. Everything below tells the agent how to maintain both.

## The core idea
The usual way an agent uses documents is RAG-shaped: retrieve chunks at query time and reconstruct the
answer from scratch, *every time*. Nothing accumulates. This repo is different: between the raw papers
and your questions sits a **persistent, compounding wiki** the agent builds and keeps current. The
cross-references are already there, the synthesis already reflects everything ingested, and — for any
ingested code — the grounding and the dynamic-dispatch seams a call-graph walk misses are already
resolved. Compiled once, kept current, not re-derived per query.

You never hand-write the wiki. **Your job:** curate which papers to add and ask good questions.
**The agent/tooling's job:** the summarizing, cross-referencing, grounding, and bookkeeping.

## Architecture — three layers, two source types
1. **Raw sources — immutable.** Read, never edited.
   - **Papers / docs / notes** → `raw/papers/`. **Committed** — these *are* your curated source of truth
     (PDFs, markdown clips, transcripts) and must persist.
   - **Code repos (optional)** → `raw/code/<slug>/` as a **git submodule** — defaults to
     **`acquire: submodule`** in each `config/<slug>.md`. The committed gitlink + `.gitmodules` *is* the
     pin (reproducible via `git submodule update --init`); the contents aren't vendored as blobs. (The
     tool also supports `acquire: clone` — gitignored clone, pin in state — for huge upstreams.)
2. **The wiki — generated, the agent owns it.** Markdown only.
   - **Papers** → `wiki/sources/<paper>.md` (one summary per ingested paper) and
     `wiki/topics/<topic>.md` (synthesized method/concept/entity pages that span papers).
   - **Cross-cutting answers** → `wiki/notes/<note>.md` (filed back from queries).
   - **Code (optional)** → `wiki/code/<slug>/` (written by the skill): `overview.md`, `concepts/`,
     `catalog/`, `doc-concepts/`; and `wiki/concepts/<key>.md` for cross-paper/cross-repo vocabulary.
   - **Shared** → `wiki/index.md`, `wiki/log.md`.
3. **The schema — this file.** `CLAUDE.md` / `AGENTS.md` / `GEMINI.md` are thin pointers so Claude Code,
   Codex, and Antigravity read this one brain. Co-evolve it as conventions settle.

## Operations

### Ingest — two paths into one wiki
- **Paper / doc / note (the core path).** Drop the source in `raw/papers/`, then: read it, discuss
  takeaways, write a summary page at `wiki/sources/<paper>.md`, **update or create the topic/entity/method
  pages it touches** (`wiki/topics/…` — a single paper can touch 10–15 pages), add cross-references, note
  where it contradicts or supersedes existing claims, update `wiki/index.md`, append `wiki/log.md`.
  Freeform prose with citations back to the source file.
- **Code repo (optional).** When a paper's implementation is worth grounding, say
  **`ingest <repo-url-or-local-path>`** → runs the **`wikify-ingest-repo`** skill, which bootstraps
  `config/<slug>.md` with `acquire: submodule` so the repo lands as a submodule under `raw/code/<slug>`,
  then `prepare` (pin + SCIP-index + symbol graph + packets) → synthesize one grounded concept page per
  packet → `overview.md` → ingest the repo's own docs into `doc-concepts/` → `finalize` (citation lint +
  coverage catalogs + assemble) → the **register step** links the repo's `overview.md` into
  `wiki/index.md` and appends `wiki/log.md`. **Idempotent reconcile** — re-running converges;
  `ingest --ref <commit>` rebuilds only the symbols that moved. From the **second** code repo on, the
  ingest ends by **connecting** the new silo to the others (below).

### Connect — cross-link the same concept across papers/repos (inline, no new page type)
One paper or silo answers "how does *this one* do X"; the cross-cutting view answers "**who does X**".
The **`wikify-connect-repo`** skill (invoked at the tail of a code ingest, or on request) builds it
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

**Paper / topic questions (the core path)** → read the relevant `wiki/topics/<topic>.md` (and the
`wiki/sources/…` summaries it cites); synthesize with citations back to the source pages / raw papers.
Comparisons ("NAS vs. learned optimizers", "which AI-scientist systems close the experiment loop") route
through the topic pages, which already span multiple papers.

**Code questions (when a repo has been ingested)** route by page type — don't fall back to grepping raw
source:
- *"Which repos implement `<concept>` (a technique, a kernel)?"* → the concept page
  `wiki/concepts/<concept>.md` — its `## In this wiki's repos` block links to each repo's implementation
  (and every implementation links back up).
- *"Where do I start / what are the systems?"* → `wiki/code/<slug>/overview.md`.
- *"How does `<mechanism>` work, and why?"* → `wiki/code/<slug>/concepts/<concept>.md` (prose + Mermaid
  diagram + woven citations).
- *"What is `<symbol>` — signature, definition, who calls it?"* → `wiki/code/<slug>/catalog/<module>.md`
  (signature, extracted docstring, a relative link to its exact source line, importance-ranked **uses-by**).
- *Need line-level certainty?* **Drop to the pinned source** — every catalog entry links to
  `raw/code/<slug>/…` at the pinned commit.

In both cases: read only the relevant section (don't bulk-read), cite precisely (a source/topic page for
papers, a catalog anchor `catalog/<module>.md#<QualifiedName>` for code), and **file good answers back** —
a cross-paper comparison, a reconstructed trace, an invariant you verified — as a `wiki/notes/…` (or
`topics/…`/`concepts/…`) page, linked from `index.md` and logged, so explorations compound like ingests.

### Lint — health-check both
- **Papers** (judgment pass): contradictions between pages, stale claims a newer paper superseded, orphan
  pages with no inbound links, methods mentioned but lacking their own page, gaps worth a web search.
- **Code** (deterministic gates): `wikify finalize <slug>` (every citation resolves, every mechanism claim
  is cited), `wikify verify <slug>` (adversarial), and **coverage** (set-difference over the symbol table
  → a catalog page per module). Stale at a new commit → `ingest --ref`.
- **Shared**: orphan detection, missing cross-references, staleness across the whole `wiki/`.

## Indexing and logging
- **`wiki/index.md` is read first.** A content catalog with sections — **Papers/Sources** (ingested
  papers), **Topics** (synthesized prose pages), **Notes**, and, if any exist, **Code repos** (link →
  `overview.md`, pinned commit, what it answers) and **Cross-paper concepts** — each line a link + a
  one-line summary. Updated on every ingest. At this scale the index + `grep` replaces embedding-based RAG.
- **`wiki/log.md` is append-only**, prefixed so it stays greppable
  (`grep '^## \[' wiki/log.md | tail -5`):
  `## [YYYY-MM-DD] ingest | <paper>` · `## [YYYY-MM-DD] ingest-code | <slug>` ·
  `## [YYYY-MM-DD] lint | <scope>` · `## [YYYY-MM-DD] note | <title>`.

## Grounding — what makes the wiki trustworthy
- **Papers**: cite the raw paper for every claim; flag contradictions instead of silently overwriting; put
  synthesis that goes beyond the sources in `> [!inferred]` blocks.
- **Code** (strict): synthesis cites **only** symbols in the packet subgraph; uncited claims go in
  `> [!inferred]` blocks; the citation linter is a build gate, not a prompt. Prefer the author's extracted
  docstrings over re-deriving behavior.
- **Shared**: **markdown is the only product** — SCIP indexes and build artifacts live in gitignored
  `.cache/`, never in `raw/`.

## Why this works
The tedious part of a paper collection isn't the reading — it's the bookkeeping: keeping cross-references
current, re-grounding claims when a source (or a commit) moves, representing every method, noticing when a
newer paper supersedes an older claim. Humans abandon reading lists because that burden outgrows the value.
The tooling doesn't get bored, doesn't forget a cross-reference, rebuilds only the delta, and (for code)
grounds every claim in a real symbol — so the wiki stays maintained because maintenance is near-zero-cost.
You curate and question; the agent does everything else.
