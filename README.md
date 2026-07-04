# 🧠 wikify repo demo

> **You're on `main` — the empty template.** The actual populated demo (two ingested codebases as
> grounded, cross-linked wikis + the live graph) lives on the **[`demo` branch](https://github.com/vlasenkoalexey/wikify-repo-demo/tree/demo)**.
> `main` deliberately omits that ingested content so **“Use this template” works** — GitHub can't generate
> a template from a repo with git submodules, and the demo pins its sources as submodules. When you use
> the template, leave **“Include all branches” off** (the `demo` branch carries the submodules).

**The companion demo for [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo).** wikify-repo
is the tool — a CLI + agent skill that ingests a code repo into a grounded markdown wiki. This repo
is what that tool *produces*: a live, browseable example so you can see the output before installing
anything.

It's a [Karpathy LLM-wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) that
handles **two source types** in one knowledge base: **code repos** — ingested by the
**`wikify-ingest-repo`** skill (which ships with
[wikify-repo](https://github.com/vlasenkoalexey/wikify-repo), not defined here) into a grounded,
lint-clean **markdown** wiki an agent answers internals questions from — and **articles / docs / notes**,
ingested the classic Karpathy way (read → summarize → cross-link). Code is the headline; prose rides
along in the same `index.md` / `log.md`. See [`SCHEMA.md`](SCHEMA.md) for the full workflow.

This repo is both:
- a **showcase** — browse a real, populated wiki on the **[`demo` branch](https://github.com/vlasenkoalexey/wikify-repo-demo/tree/demo)**; and
- a **template** — you're on it: click **“Use this template”** to start your own code-wiki with the
  skills and agent conventions already wired up.

## The whole wiki at a glance

[![Force-directed graph of the wiki: two ingested codebases (mini_pytorch_xla and wikify-repo) plus the prose pages, colored by page type](https://raw.githubusercontent.com/vlasenkoalexey/wikify-repo-demo/demo/tools/graph/graph.png)](https://vlasenkoalexey.github.io/wikify-repo-demo/tools/graph/)
(click image for interactive view)

A snapshot of the live viewer (92 pages · 384 links) — the populated wiki on the [`demo` branch](https://github.com/vlasenkoalexey/wikify-repo-demo/tree/demo).
Every node is a wiki page; every edge a markdown link between pages. The two dense clusters are the two
ingested codebases — [`mini_pytorch_xla`](https://github.com/vlasenkoalexey/wikify-repo-demo/blob/demo/wiki/code/mini_pytorch_xla/overview.md)
and [`wikify-repo`](https://github.com/vlasenkoalexey/wikify-repo-demo/blob/demo/wiki/code/wikify-repo/overview.md) — joined
through the shared root `index.md` and the prose pages. **Code** pages are colored by page type
(`code:concepts`, `code:catalog`, `code:doc-concepts`, `code:overview`); **prose** by folder
(`topics`, `sources`).

## Repo layout (what a populated wiki looks like)

```
SCHEMA.md              single source of truth — the three layers, ingest/query/lint, retrieval rules.
raw/                   immutable inputs — never modified.
  code/<slug>/           ingested repos as git SUBMODULES, pinned by gitlink (this demo defaults to acquire: submodule).
  sources/               ingested articles / docs / notes — committed source of truth.
wiki/                  LLM-owned markdown — the product.
  index.md               read-first catalog: code repos, cross-repo concepts, topics, sources, notes.
  log.md                 append-only event log (## [date] <op> | <name>).
  code/                  code wikis (one dir per repo) + an auto code catalog (index.md).
    <slug>/                one CODE wiki per repo:
      overview.md            high-level map — main concepts + system diagrams.
      concepts/              grounded mechanism pages (prose + Mermaid + citations).
      catalog/               per-module symbol catalogs — signatures, docstrings, source links, uses-by.
      doc-concepts/          pages derived from the repo's own docs.
  concepts/              cross-repo vocabulary — each concept links down to every repo's implementation (via wikify-connect-repo).
  sources/               one summary page per ingested article.
  topics/                synthesized prose pages — entities, concepts, comparisons.
  notes/                 cross-cutting answers filed back from queries.
```

On **this template branch** `wiki/` starts empty (just `index.md` + `log.md` stubs) and `raw/` doesn't
exist yet — both fill in on your first ingest. To browse a *populated* one, switch to the
[`demo` branch](https://github.com/vlasenkoalexey/wikify-repo-demo/tree/demo), whose code sources are
**git submodules** (pinned by gitlink):
```bash
git clone --recurse-submodules -b demo https://github.com/vlasenkoalexey/wikify-repo-demo
# already cloned?  git checkout demo && git submodule update --init
```

## Browse it (no install)

On the [`demo` branch](https://github.com/vlasenkoalexey/wikify-repo-demo/tree/demo), open
[`wiki/index.md`](https://github.com/vlasenkoalexey/wikify-repo-demo/blob/demo/wiki/index.md) and follow
links, or `grep -ri "<term>" wiki/`. Everything is plain markdown — no embeddings, no database. An agent
answers cheaply by reading `index.md`, grepping to the right page, and citing the catalog anchor.

## Make your own

1. **Use this template** (button above) — or `git clone` this branch. Leave **“Include all branches” off**
   (the `demo` branch's submodules would break generation).
2. Install the tooling once — see [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo)
   (`pip install -e .` → `setup-vendor.sh` → `install-skill.sh /path/to/this-repo`).
3. In **Claude Code, Codex, or Antigravity**, just say:
   > ingest https://github.com/owner/your-repo

   The skill pins + indexes the repo, writes the grounded pages, lints them, assembles `wiki/<slug>/`,
   and updates `index.md` + `log.md`. Re-running is idempotent; `ingest --ref <commit>` updates to a
   newer commit and rebuilds only what changed. From the **second** repo on, it can **connect** shared
   concepts across repos into the cross-repo `wiki/concepts/` pages (the `wikify-connect-repo` skill).

## Why a wiki and not just grep over the source?

The wiki sits *between* raw repos and your questions: the cross-references are already there, the
dynamic-dispatch seams a call-graph walk misses are covered by deterministic catalogs, and every
mechanism page is grounded in real SCIP symbols. The tedious part — the bookkeeping — is done once
and kept current, so answers are fast, grounded, and consistent. Conceptually, the generated wiki is
an annotated map of your codebase that an LLM agent can navigate efficiently.

> Note on citation anchors: a citation like `catalog/<module>.md#Buffer.shape` resolves against the
> catalog's frontmatter `symbols:` map (that's what the linter gates), not against a rendered
> heading — so clicking one on github.com opens the right catalog *file* but won't auto-scroll.
> Grep the anchor name inside the file, or read the wiki locally.
