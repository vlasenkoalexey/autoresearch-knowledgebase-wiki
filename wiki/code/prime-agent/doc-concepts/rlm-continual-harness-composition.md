---
title: Composing RLM and Continual Harness into one agent
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Composing RLM and Continual Harness into one agent

## Definition
The README states Prime Agent "is designed around two core abstractions" — RLM, which "treats context as
variables (*prompt-as-a-variable*) and tools like recursive subagents as function calls... inside a
persistent REPL," and Continual Harness, which "stores supplemental prompts, memories, skill descriptions,
and reusable subagent specifications as durable state that Prime Agent can refine through small,
evidence-backed updates." Combined: "a persistent Python control environment with durable harness state, so
useful working context and reusable operating patterns can outlive a single chat window."

## In prime-agent (grounded)
This is a TypeScript port of both mechanisms, not a wrapper around the original Python projects. RLM's
`rlm(...)` call becomes [`AgentSession._startRlmChildRun`](../concepts/packages-coding-agent-src-core-agent-session.ts.md),
dispatched through a persistent [`KernelManager`](../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
IPython process rather than the original's REPL variable substitution — the same *prompt-as-a-variable*
design, reimplemented as a coding-agent's own kernel/tool boundary. Continual Harness's evidence-backed
`/refine` becomes [`refinement.ts`](../concepts/packages-coding-agent-src-core-refinement-refinement.ts.md)'s
`applyRefinementProposal`, with the same immutable-base-prompt boundary and optimistic-concurrency
rollback the Python original ([`immutable-base-prompt`](../../continual-harness/doc-concepts/immutable-base-prompt.md))
establishes, but implemented with TypeScript's `HarnessEntry` versioning instead of Python's
snapshot-and-restore.

## Why it matters / when it applies
This wiki now holds both lineages side by side: the research prototypes
([`rlm`](../../rlm/overview.md), [`continual-harness`](../../continual-harness/overview.md)) that
demonstrated each mechanism in isolation, and prime-agent's production TypeScript reimplementation that
composes them into a single shipped coding agent. Comparing a mechanism across the pair (e.g. how rollback
is implemented) is a "how do independent implementations solve the same problem" question, not a
"which one is correct" question — both make different but reasonable tradeoffs for their runtime.

## Connections
- Code concepts: [`packages-coding-agent-src-core-refinement-refinement.ts`](../concepts/packages-coding-agent-src-core-refinement-refinement.ts.md),
  [`packages-coding-agent-src-core-kernel-index.ts`](../concepts/packages-coding-agent-src-core-kernel-index.ts.md),
  [`packages-coding-agent-src-core-agent-session.ts`](../concepts/packages-coding-agent-src-core-agent-session.ts.md)
- Related doc-concepts: [immutable-base-prompt](../../continual-harness/doc-concepts/immutable-base-prompt.md),
  [reset-free-harness-evolution](../../continual-harness/doc-concepts/reset-free-harness-evolution.md)
- Wiki: [`sources/prime-agent-launch.md`](../../../sources/prime-agent-launch.md),
  [`sources/recursive-language-models.md`](../../../sources/recursive-language-models.md),
  [`sources/continual-harness.md`](../../../sources/continual-harness.md)

## Source
Extracted from `README.md` (kept in place).
