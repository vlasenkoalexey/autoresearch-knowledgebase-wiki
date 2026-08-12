---
title: Context resets and the playbook/log split
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Context resets and the playbook/log split

## Definition
The README describes a deliberate two-file memory split: `log.txt` is raw, ground-truth history ("the log
stays ground truth"), while `playbook.md` is a curated briefing for the agent's *successor* after a context
reset, itself split into a **working model** (mechanics/controls, each point marked
checked-against-the-log vs. still-assumed) and **working memory** (the current attempt's position, plan,
and ruled-out options). When the conversation grows past a set input-token threshold, it is dropped
entirely and a fresh session resumes pointed only at these two files.

## In Retrodict (grounded)
This is the doc-level framing of exactly what [`GameRunner._restore`](../concepts/arc3-runner.md) and
[`parse_log`](../concepts/arc3-logwriter.md) implement in code: `_restore`'s own docstring — *"Rebuild env
state by replaying the logged actions; continue accounting"* — is the mechanical realization of "the log
stays ground truth," and [`_seed_level_signals`](../concepts/arc3-runner.md) is the code path that recovers
stuck-level context (the "working memory" half) from that same replay.

## Why it matters / when it applies
The design goal is that a fresh session should be able to **plan from the curated playbook instead of
re-deriving settled rules from the raw log** — the README explicitly calls out compacting into the working
model at level-completion rather than journaling indefinitely, which is what keeps a long run's context
usage bounded despite arbitrarily many resets.

## Connections
- Code concepts: [`arc3-runner`](../concepts/arc3-runner.md), [`arc3-logwriter`](../concepts/arc3-logwriter.md)
- Related doc-concepts: [retrodiction-methodology](retrodiction-methodology.md)
- Wiki: [`sources/2025-context-rot.md`](../../../sources/2025-context-rot.md) — the measured problem
  (accuracy degrading well before a window fills) this reset-and-compact design is a structural response to,
  independent of and complementary to [Recursive Language Models](../../../sources/recursive-language-models.md)'
  context-as-a-variable approach to the same problem.

## Source
Extracted from `README.md` (kept in place).
