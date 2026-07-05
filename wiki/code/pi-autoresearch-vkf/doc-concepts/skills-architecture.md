---
title: Skills architecture — machinery vs. domain knowledge
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Skills architecture — machinery vs. domain knowledge

## Definition
`pi-autoresearch-vkf` ships two kinds of files: TypeScript tools (deterministic, unit-testable) and
markdown **skills** (prose that tells the host agent *how* to think). The README's Skills table names
ten: the orchestrator `autoresearch-vkf` plus nine sub-skills it delegates to —
`autoresearch-vkf-knowledge-gather` (find candidate techniques via WebSearch/WebFetch),
`autoresearch-vkf-claim-extract` (distill sources into claim cards), `autoresearch-vkf-claim-verify`
(check citations & codebase fit), `autoresearch-vkf-contradiction-miner` and
`autoresearch-vkf-cross-domain-transfer` (turn tensions/analogies into hypotheses),
`autoresearch-vkf-idea-tournament` (multi-perspective debate to pick 2–3 ideas worth testing),
`autoresearch-vkf-hypothesis-loop` (pick the next idea and run the smallest falsifying experiment),
`autoresearch-vkf-research-plan` (ideation mode), and `autoresearch-vkf-research-report` (the auditable
lineage report). `CLAUDE.md` states the split as the repo's central architectural rule: "the extension is
the machinery; the skills are the domain knowledge."

## In pi-autoresearch-vkf (grounded)
Skills are pure markdown — they carry no SCIP symbols of their own — but every skill's job is to call the
deterministic tools registered by [`autoresearchExtension`](../catalog/extensions/pi-autoresearch-vkf/index.ts.md#autoresearchExtension)
in `index.ts`, so each skill maps onto a slice of that tool spine and the concept page grounding it:
`autoresearch-vkf-claim-extract`/`autoresearch-vkf-claim-verify` drive `remember_claim`/`verify_claim`,
grounded in the [VKF card lifecycle](../concepts/extensions-pi-autoresearch-vkf-cards.ts.md);
`autoresearch-vkf-contradiction-miner` and `autoresearch-vkf-cross-domain-transfer` drive
`find_contradictions`/`find_transfers`, grounded in
[hypothesis synthesis](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md);
`autoresearch-vkf-idea-tournament` and `autoresearch-vkf-hypothesis-loop` drive `score_ideas`/`plan_next_step`,
grounded in [idea scoring](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md) and
[the search tree](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md); `autoresearch-vkf-research-plan`
drives `draft_research_plan`, gated by the `ideate` branch of
[session config](../concepts/extensions-pi-autoresearch-vkf-config.ts.md). Because the loop runs
`autonomy: "continuous"` by default, every skill's prose is reinforced turn-to-turn by the
[autonomy watchdog](../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)'s `continuationNote`, which is
why `index.ts`'s own header comment calls tool output — not skill prose — the thing that "actually keeps the
loop running unattended."

## Why it matters / when it applies
The split exists so the *how to think* layer (which papers to trust, when a tension is worth mining, how to
phrase a falsifiable experiment) can be edited as prose without touching typechecked code, while the *how to
persist state safely* layer (memory lifecycle, transaction audit trail, tree bookkeeping) stays deterministic
and tested. It also explains a load-bearing design choice noted on the
[tool spine's concept page](../concepts/extensions-pi-autoresearch-vkf-index.ts.md): skill text fades from a
long agent's context faster than recurring tool output does, so anything that must survive an entire
unattended run (the continuation contract, the audit trail) is pushed into the tools, not left to skill prose
alone.

## Connections
- Code concepts: [The tool spine](../concepts/extensions-pi-autoresearch-vkf-index.ts.md),
  [VKF cards](../concepts/extensions-pi-autoresearch-vkf-cards.ts.md),
  [Hypothesis synthesis](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md),
  [Idea scoring](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md),
  [The search tree](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md),
  [Session config](../concepts/extensions-pi-autoresearch-vkf-config.ts.md),
  [Autonomy watchdog](../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- Module catalogs: [index.ts](../catalog/extensions/pi-autoresearch-vkf/index.ts.md)
- Related doc-concepts: [Tool reference](tool-reference.md)

## Source
Extracted from `README.md` (Skills reference table) and `CLAUDE.md` ("Architecture" / "Skills" sections),
both kept in place.
