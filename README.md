# Autoresearch & Auto-Optimization Knowledge Base

A curated, cross-linked **wiki collection of papers on autoresearch and auto-optimization** — automated
scientific discovery, AI research agents, AutoML, hyperparameter and neural-architecture search, and
compiler / kernel / systems auto-tuning. Papers go in; a persistent, compounding wiki comes out.

It's built on the [Karpathy LLM-wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f):
between the raw papers and your questions sits a **persistent wiki** an agent builds and keeps current.
You curate which papers to add and ask good questions; the agent does the summarizing, cross-referencing,
and bookkeeping. See [`SCHEMA.md`](SCHEMA.md) for the full workflow.

## What's in scope

- **Autoresearch** — AI scientists / research agents, automated hypothesis generation and experimentation,
  literature synthesis, self-improving research loops, agentic discovery pipelines.
- **Auto-optimization** — AutoML, hyperparameter optimization, neural architecture search (NAS),
  learned optimizers, compiler / kernel / schedule auto-tuning, systems and performance optimization.

Each ingested paper becomes a summary page; the concepts, methods, and entities it touches become
synthesized topic pages that span the whole collection — so the wiki grows a shared vocabulary as
papers accumulate, and contradictions between papers get flagged rather than silently overwritten.

## How it's organized

```
SCHEMA.md              single source of truth — the layers, ingest/query/lint, retrieval rules.
raw/                   immutable inputs — never modified.
  papers/                ingested papers (PDFs, markdown clips, notes) — committed source of truth.
  code/<slug>/           optional: reference code repos as git submodules (for papers that ship code).
wiki/                  agent-owned markdown — the product.
  index.md               read-first catalog: papers, topics, notes (and any code repos).
  log.md                 append-only event log (## [date] <op> | <name>).
  sources/               one summary page per ingested paper.
  topics/                synthesized prose pages — methods, concepts, comparisons across papers.
  notes/                 cross-cutting answers filed back from queries (e.g. "NAS vs. learned optimizers").
  code/<slug>/           optional code wikis when a paper's implementation is ingested too.
  concepts/              optional cross-repo/cross-paper vocabulary linking to implementations.
```

`wiki/` starts with `index.md` + `log.md` stubs and fills in as you ingest papers.

## Add a paper

1. Drop the source in `raw/papers/` (PDF, markdown clip, or notes).
2. In **Claude Code, Codex, or Antigravity**, say what you want:
   > ingest raw/papers/the-ai-scientist.pdf

   The agent reads it, writes a summary at `wiki/sources/<paper>.md`, updates or creates the topic/entity
   pages it touches (`wiki/topics/…` — a single paper can touch 10–15 pages), adds cross-references,
   notes where it contradicts existing claims, updates `index.md`, and appends `log.md`.

Papers that ship code can *also* be ingested as grounded code wikis via the
[wikify-repo](https://github.com/vlasenkoalexey/wikify-repo) tooling (`ingest <repo-url>`) and connected
to the concept pages the papers already describe — but the headline here is the paper collection.

## Query it (no install)

Open [`wiki/index.md`](wiki/index.md) and follow links, or `grep -ri "<term>" wiki/`. Everything is
plain markdown — no embeddings, no database. An agent answers cheaply by reading `index.md`, grepping to
the right page, and citing back to the source paper. File good answers back as `wiki/notes/…` pages so
explorations compound alongside ingests.

## Why a wiki and not just a folder of PDFs?

The tedious part of a paper collection isn't the reading — it's the bookkeeping: keeping cross-references
current, noticing when a newer paper supersedes an older claim, representing every method, spotting
contradictions. Humans abandon reading lists because that burden outgrows the value. The agent doesn't get
bored, doesn't forget a cross-reference, and grounds every claim in a cited source — so the wiki stays
maintained because maintenance is near-zero-cost. You curate and question; the agent does everything else.
