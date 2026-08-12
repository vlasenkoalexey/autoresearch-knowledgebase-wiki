---
title: Retrodiction — check every hypothesis against the log before acting
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Retrodiction — check every hypothesis against the log before acting

## Definition
The README states the agent's central discipline as: "Never act blindly: every hypothesis about a game
mechanic must first be checked against the recorded history. The agent writes python that replays the
hypothesis over past frames in `log.txt`, and if any recorded frame contradicts it, it's falsified for
free. Only questions the log can't settle earn a live action." This is the source of the repo's name.

## In Retrodict (grounded)
The mechanism this describes lives at the boundary between [`arc3-logwriter`](../concepts/arc3-logwriter.md)
(the replayable log a hypothesis can be checked against) and [`arc3-plan_parser`](../concepts/arc3-plan_parser.md)
(where a per-action `expect` prediction is captured before the action runs). The runtime enforcement is in
[`arc3-runner`](../concepts/arc3-runner.md): [`GameRunner._check_expectations`](../concepts/arc3-runner.md)
compares the prediction against what actually happened after each step, and
[`GameRunner._restore`](../concepts/arc3-runner.md) rebuilds the agent's entire understanding of the game
from that same log after a context reset — so "checked against the recorded history" is not just a prompt
instruction, it is what the log format and the runner's resume path are built to do.

## Why it matters / when it applies
The README frames the payoff directly: being wrong against the log "costs nothing," while a wrong live
action can waste the fixed action budget the RHAE metric ([`arc-agi-3.md`](../../../sources/arc-agi-3.md))
scores against. The forward-simulation companion rule — every action must carry a computed `expect` before
it is played, "so a wrong world model costs one action rather than a whole plan" — is what
`_check_expectations` and the plan-drain-abort behavior in [`arc3-runner`](../concepts/arc3-runner.md)
implement.

## Connections
- Code concepts: [`arc3-runner`](../concepts/arc3-runner.md), [`arc3-logwriter`](../concepts/arc3-logwriter.md),
  [`arc3-plan_parser`](../concepts/arc3-plan_parser.md)
- Module catalogs: [`src/arc3/runner`](../catalog/src/arc3/runner.md)
- Related doc-concepts: [context-reset-and-playbook](context-reset-and-playbook.md)
- Wiki: [`concepts/verification-independence.md`](../../../concepts/verification-independence.md) — the
  cheap-falsification-before-expensive-commitment pattern this shares with kernel-lane parity gates in the
  TPU autoresearch wiki, and with Schema's own backtest-before-acting design (see
  [`sources/schema-harness.md`](../../../sources/schema-harness.md)).

## Source
Extracted from `README.md` (kept in place).
