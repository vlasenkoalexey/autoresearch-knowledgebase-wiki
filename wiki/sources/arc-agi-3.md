# ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence

The ARC Prize Foundation's third-generation benchmark ([arXiv:2603.24621](https://arxiv.org/abs/2603.24621),
v1 2026-03-24, v2 2026-04-17; submitted by François Chollet), and the scoring metric — **RHAE**, relative
human action efficiency — every result in this wiki's Prime Agent / Retrodict / Schema cluster is quoted
in. Ingested 2026-08-12 as the metric-defining source behind
[Prime Agent](prime-agent-launch.md), [Retrodict](retrodict.md), and [Schema](schema-harness.md).

## Overview

Where ARC-AGI-1/2 are static grid puzzles, ARC-AGI-3 drops an agent into one of a set of **interactive**,
turn-based game environments it has never seen, gives it no rules, and requires it to explore, form a
working model of what its actions do, and win — evaluated on **skill-acquisition efficiency**, not just
success. The design goal stated by the benchmark is to resist the two easiest ways to inflate a score on a
static benchmark: memorization (every environment is novel) and brute force (efficiency, not just a win, is
scored).

## Key claims

- **RHAE is a squared ratio, not a linear one.** Per level: `min(1.0, human_baseline_actions /
  agent_actions)²`. Taking twice as many actions as the human baseline scores a quarter, not a half; ten
  times the actions scores near zero. The squaring is deliberate — it is what makes the metric resistant to
  an agent that eventually stumbles into a win by exhaustive search rather than understanding the
  environment.
- **The human baseline is the second-best of 10 first-exposure testers**, not the best — filtering lucky
  outliers while staying anchored to genuine human play on a level nobody has seen before.
- **The headline score is an unweighted mean of per-level RHAE across the public game set.** As of the
  paper's own July 2026 administered run, Claude Opus 5 held the frontier at 30.2%, independently measured
  by ARC Prize — 19 of 25 public environments unsolved by any system at that point.
- **Language and outside knowledge are deliberately excluded from the task itself** — environments are
  built from Core Knowledge priors (the same non-linguistic primitives ARC-AGI-1/2 draw on: objects,
  counting, basic physics), so an agent can't shortcut by pattern-matching on English task descriptions.
- **The gap between human and AI performance the paper reports is stark**: as of its snapshot, humans solve
  essentially 100% of the environments; frontier systems scored below 1% before the wave of harness work
  this wiki tracks (Schema, Retrodict, Prime Agent) pushed self-reported numbers to 95–99%+ months later.

## Key data points

| Signal | Value |
|---|---|
| Metric | RHAE = mean over levels of `min(1.0, human_actions/agent_actions)²` |
| Human baseline definition | 2nd-best of 10 first-exposure human testers per environment |
| Public game count | 25 |
| Human success rate (paper's own framing) | ~100% |
| Frontier AI score at paper's March 2026 snapshot | <1% |
| Administered frontier score, Jul 2026 (Claude Opus 5, ARC Prize's own run) | 30.2% |

## Techniques referenced
Core Knowledge priors as the environment-design substrate; efficiency-normalized (not success-only)
scoring; held-out vs. public environment splits; first-exposure human baselining.

## Gaps & caveats
- This ingest is scoped to the **benchmark and metric**, not the leaderboard — scores this wiki cites
  elsewhere (Prime Agent 95.5%, Schema ~99%, Retrodict 99.86%) come from those systems' own pages/scorecards,
  not from this paper, and several are **self-reported rather than administered by ARC Prize** — flagged
  explicitly on each of those source pages.
- The paper does not itself adjudicate the live methodological dispute this wiki also records (see
  [Retrodict](retrodict.md) and [`concepts/verification-independence.md`](../concepts/verification-independence.md)):
  whether a harness that rewrites itself between few-shot attempts, or precomputes a simulator from the
  interaction log, is still measuring the thing RHAE was designed to measure. That dispute belongs to the
  harnesses cited above, not to this benchmark paper.
- Full technical detail (exact per-game design, held-out set composition) sits behind the paper and the
  ARC Prize technical report; this summary covers only the mechanism the rest of this wiki's citations
  depend on.

## Connections
- [Prime Agent launch post](prime-agent-launch.md) — reports 95.5% RHAE (self-administered) against the
  paper's own 30.2% administered baseline on the same model and game set.
- [Schema harness](schema-harness.md), [Retrodict](retrodict.md) — the two harnesses that crossed the
  human-expert line before Prime Agent's launch post, both self-reported.
- [`concepts/verification-independence.md`](../concepts/verification-independence.md) — the
  self-reported-vs-administered distinction this benchmark makes newly load-bearing: RHAE's efficiency
  design defends against brute force, but not against who runs the scoring.

## Sources
- [ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence](https://arxiv.org/abs/2603.24621),
  ARC Prize Foundation (Chollet), arXiv:2603.24621, v2 2026-04-17
- [arcprize.org/arc-agi/3](https://arcprize.org/arc-agi/3) · [arcprize.org/leaderboard](https://arcprize.org/leaderboard)
