---
title: The CodeAct bet — code as the universal interface
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# The CodeAct bet — code as the universal interface

## Definition
The README states the repo's design thesis directly: RLMs argue for a **CodeAct-style harness** — "all
language models should have access to a code environment" — with sub-model calls and context/prompts both
represented as *objects in code*, not as JSON tool-calling messages. The stated goal is to "move away from
the JSON tool-calling standard for both sub-agents and generic tool calls."

## In rlm (grounded)
This is not aspirational framing — it is the literal shape of [`RLM._subcall`](../catalog/rlm/core/rlm.md#RLM._subcall):
a recursive call is reached because the model's generated Python code calls a function
(`rlm_query`/`rlm_query_batched`, injected into the REPL namespace — see
[`rlm-environments-base_env`](../concepts/rlm-environments-base_env.md)'s custom-tools injection mechanism),
not because the model emitted a structured tool-call message the harness then parses and dispatches. The
long prompt itself is likewise a REPL *variable* (see [`rlm-core-rlm`](../concepts/rlm-core-rlm.md)), not a
tool-call argument.

## Why it matters / when it applies
The README frames this as a bet on future model design, not just an implementation convenience: sub-calls
"deferred... to the language model itself" are described as "incredibly flexible and lend[ing] itself well
to scale if trained correctly" — a claim the repo's own `training/` stack (see
[`training-src-rlm_train-env`](../concepts/training-src-rlm_train-env.md)) exists specifically to test, by
fine-tuning a small model to be a better RLM.

## Connections
- Code concepts: [`rlm-core-rlm`](../concepts/rlm-core-rlm.md), [`rlm-environments-base_env`](../concepts/rlm-environments-base_env.md)
- Related doc-concepts: [repl-environment-taxonomy](repl-environment-taxonomy.md)

## Source
Extracted from `README.md` (kept in place).
