---
title: Tool reference — the 19-tool spine, mapped to its mechanism pages
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Tool reference — the 19-tool spine, mapped to its mechanism pages

## Definition
The README's "Tools" reference table lists every tool the host agent can call, one row per tool with a
one-line description: `init_research`, `remember_claim`, `verify_claim`, `recall_memory`, `score_ideas`,
`plan_next_step`, `set_research_mode`, `find_contradictions`, `find_transfers`, `find_compositions`,
`draft_research_plan`, `vkf_run_experiment`, `vkf_log_experiment`, `promote_to_global`, `research_graph`,
`export_dashboard`, `research_update`, `research_status`. This doc-concept is the routing index from that
table to the concept page that actually grounds each tool's mechanism — the table names *what* a tool does;
the linked concept page explains *how*.

## In pi-autoresearch-vkf (grounded)
Every one of these is a `pi.registerTool` call inside the single
[`autoresearchExtension`](../catalog/extensions/pi-autoresearch-vkf/index.ts.md#autoresearchExtension) function
in `index.ts` — grounded in depth on [the tool spine concept page](../concepts/extensions-pi-autoresearch-vkf-index.ts.md).
By subsystem:
- **Session lifecycle** — `init_research` reads/writes [`ResearchConfig`](../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  via `makeConfig`, and scaffolds the workspace via [`ensureSessionDirs`](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md).
  `set_research_mode` mutates the same config's `exploreFraction`/`altitudePreference`.
- **Memory (VKF cards)** — `remember_claim` and `verify_claim` are the write/transition path over
  [the card trust lifecycle](../concepts/extensions-pi-autoresearch-vkf-cards.ts.md) (`buildClaimCard`,
  `buildPaperCard`); `recall_memory` is the read path (`listCards`/`findCard`); `promote_to_global` copies a
  trusted card from project [`memoryPaths`](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md) to the
  global root.
- **Hypothesis generation** — `find_contradictions`, `find_transfers`, and `find_compositions` map directly
  onto [`findContradictions`/`findTransfers`/`findCompositions`](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md);
  `draft_research_plan` is the ideation-mode deliverable, gated by `sessionMode(config) === "ideate"` in
  [session config](../concepts/extensions-pi-autoresearch-vkf-config.ts.md).
- **Ranking and search** — `score_ideas` calls [`rankIdeas`](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md);
  `plan_next_step` is [`selectExpansion`](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md) —
  best-first expansion that decides both which experiment node to branch from and which idea to apply.
- **Running and logging experiments** — `vkf_run_experiment` executes the measure command and checks the
  [STOP file](../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md); `vkf_log_experiment` judges the
  result against [the parent node's value](../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  (`nodeBaseline`) and writes a [VKF experiment card](../concepts/extensions-pi-autoresearch-vkf-cards.ts.md).
- **Visibility** — `research_graph` shells to the optional [`vkf` CLI bridge](../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md);
  `export_dashboard` writes the browser dashboard via
  [`progress_data.ts`](../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md) and
  [`progress_html.ts`](../catalog/extensions/pi-autoresearch-vkf/progress_html.ts.md#renderDashboardHtml) (see
  [Browser dashboard export](browser-dashboard-export.md)); `research_status` and `research_update` drive the
  [terminal dashboard](../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md).

## Why it matters / when it applies
The table is the user-facing contract; the concept pages are where the actual decision logic (why a card gets
promoted, why one experiment node is chosen over another, why a hypothesis counts as a contradiction vs. a
transfer) lives. Reading the table alone tells you *that* `plan_next_step` picks the next experiment — reading
[the search tree concept page](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md) tells you it always
expands from the single current best node rather than a multi-node frontier, a distinction the README doesn't
state but matters for anyone comparing this loop to AIDE/The AI Scientist v2-style tree search.

## Connections
- Code concepts: [The tool spine](../concepts/extensions-pi-autoresearch-vkf-index.ts.md),
  [VKF cards](../concepts/extensions-pi-autoresearch-vkf-cards.ts.md),
  [Session config](../concepts/extensions-pi-autoresearch-vkf-config.ts.md),
  [Hypothesis synthesis](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md),
  [Idea scoring](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md),
  [The search tree](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md),
  [Experiment log & parent-relative baselines](../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md),
  [The vkf CLI bridge](../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md),
  [Dashboard payload assembly](../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md),
  [Terminal dashboard](../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md),
  [Workspace layout](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md),
  [Autonomy watchdog](../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- Module catalogs: [index.ts](../catalog/extensions/pi-autoresearch-vkf/index.ts.md)
- Related doc-concepts: [Skills architecture](skills-architecture.md), [Browser dashboard export](browser-dashboard-export.md)

## Source
Extracted from `README.md` ("Reference" → "Tools" table), kept in place.
