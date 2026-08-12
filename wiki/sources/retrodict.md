# Retrodict

Ryan Brown, independent — [blog post](https://blog.ryanbbrown.com/p/how-i-accidentally-got-the-top-score) +
[official scorecard](https://arcprize.org/scorecards/9c403765-db5b-40b1-beab-6fa3f40119b0). No formal paper.
Built in roughly two weeks in July 2026 on Brown's own minimal harness framework, ThinHarness. The highest
publicly reported [ARC-AGI-3](arc-agi-3.md) score at the time of this ingest, and — for this wiki's
purposes — the harness in this batch with the clearest kinship to the
[verification-independence](../concepts/verification-independence.md) discipline already established here.
Ingested 2026-08-12.

## Overview

Retrodict plays each game "like a scientist with a lab notebook": every returned frame is written to a log
file, and the agent works over that log with Python rather than looking at rendered images. Its
distinguishing move is **retrodiction** — before a hypothesis about a game mechanic earns a live action, it
must first be checked against the game's own recorded history, by writing Python that replays the
hypothesis over past frames. Being wrong there costs nothing; only a hypothesis the log can't already
falsify graduates to a real move, and every committed action carries an explicit prediction of what the
board should look like afterward, so a wrong world model costs one action, not a whole plan.

## Key claims

- **99.86% mean RHAE, all 25 public games solved, all 183 levels solved** — the ARC Prize's own
  competition-mode scorecard, at $654 in API-list-price cost and 660M tokens across 7,703 actions. Two
  games score below 100%: 98.64% on `sk48`, 97.77% on `sp80`.
- **A same-model, same-price comparison against `baseline1`** — the cleanest apples-to-apples datum in the
  set, since both publish token usage under the same model and price schedule — shows Retrodict at
  **5.5× fewer tokens** than baseline1's 98.97%-scoring run (baseline1: ~3.6B tokens; Retrodict: ~660M).
- **Only one public harness scores higher, at far greater cost**: Tycho at 100.00% for ~$2,986, against
  Retrodict's 99.86% for $654 — which the author's own published comparison frames as putting Retrodict on
  the cost-performance frontier rather than at the absolute top.
- **Structural containment, not just a prompt instruction**: the agent's Python tool runs in a venv with no
  game-engine packages available, and every run writes a `containment.json` proving those imports fail —
  and aborts if they don't. This is an enforced boundary, not a policy the model is asked to follow.
- **Context resets are designed-in, not a failure mode.** Past a 150K-input-token threshold, the
  conversation is dropped entirely and the agent resumes in a fresh session pointed only at two persistent
  workspace files (`playbook.md`, a curated per-level briefing, and `log.txt`, ground truth) — the same
  compress-and-restart pattern this wiki's [wiki-driven-autoresearch-loop](../topics/wiki-driven-autoresearch-loop.md)
  page already discusses for context-pollution mitigation, arrived at independently.
- **Escalation on stuck levels is staged, not open-ended**: after 300 actions or two self-issued resets on
  one level, the runner starts directing the agent to promote its checked rules into an explicit,
  verifiable `step(state, action)` simulator and search that instead of continuing to probe live; a second
  tier redirects toward unexplored states if the level still resists.

## Key data points

| Harness | RHAE | Cost | Coverage |
|---|--:|--:|---|
| Tycho | 100.00% | $2,986 | one full 25-game run |
| **Retrodict** | **99.86%** | **$654** | one full 25-game run, all 183 levels |
| Schema | 98.98% | ≥$6,447 | fixed conditional reruns, higher result retained |
| baseline1 | 98.97% | $2,722 | one full 25-game run |
| PRO-LONG | 97.4% best@2 | $1,750 | selective second runs |
| Prime Agent | 95.5% | ~$944 | three full runs, best shown |
| NOOA | 85.13% | $332 | one 25-game fleet, 2-hour cap |
| OPINE-World | 78.37% | $1,040 | one full 25-game run |

*Table per Retrodict's own published comparison; cost basis and run-qualification rules differ across
entries — see its [comparison methodology](https://github.com/ryanbbrown/Retrodict/blob/main/docs/arc-agi-3-harness-comparison.md)
for sourcing. Reproduced here because it directly complicates [Prime Agent](prime-agent-launch.md)'s framing
— see Connections.*

## Techniques referenced
Log-as-context (structured text log rather than image frames as the primary observation channel);
retrodiction-gated hypothesis testing; per-action forward-prediction (`expect`) with plan invalidation on
mismatch; curated playbook memory surviving context resets; sandboxed/containment-verified tool execution;
staged escalation to explicit simulator construction on stuck levels.

## Gaps & caveats
- **Self-reported, same as every other harness in this cluster** — the RHAE and cost figures come from an
  ARC-Prize-issued scorecard for this specific run, which is stronger provenance than a purely self-graded
  number, but the comparison table above blends scorecards, estimates, and API-equivalent cost conversions
  across differently-sourced entries; treat cross-row comparisons as approximate.
- **No license on the repository** (confirmed via `gh repo view`: `licenseInfo: null`) — all rights
  reserved by default. Relevant if this repo is later ingested as a code silo (submodule gitlink only, no
  vendoring, per this wiki's default).
- The retrodiction design is closely related to, but distinct from, [Schema](schema-harness.md)'s
  certified-world-model search — both build and backtest an explicit model of game mechanics against the
  interaction log before acting, which is the shared design move across the strongest ARC-AGI-3 harnesses
  in this batch, independent of which team built it.

## Connections
- [ARC-AGI-3 benchmark](arc-agi-3.md) — the benchmark and RHAE metric.
- [Schema](schema-harness.md) — the closest methodological relative: both harnesses backtest an explicit,
  falsifiable model of the environment against the full interaction log before committing an action, rather
  than acting on the latest observation alone.
- [Prime Agent launch post](prime-agent-launch.md) — the harness the source video frames as *the* result;
  Retrodict's own published table places Prime Agent's 95.5% below four other public harnesses at higher
  cost, which the video's "65 points, only the loop changed" framing does not surface.
- [`concepts/verification-independence.md`](../concepts/verification-independence.md) — retrodiction is
  this batch's sharpest instance of "check a hypothesis against ground truth before it costs anything,"
  which is structurally the same move [kgate](../sources/tpu-performance-autoresearch-wiki.md)'s parity
  gate makes for kernel candidates, one level up the stack: cheap falsification before an expensive
  commitment.

## Sources
- [How I accidentally got the top score on ARC-AGI-3](https://blog.ryanbbrown.com/p/how-i-accidentally-got-the-top-score),
  Ryan Brown
- [Official scorecard](https://arcprize.org/scorecards/9c403765-db5b-40b1-beab-6fa3f40119b0)
- Code: [ryanbbrown/Retrodict](https://github.com/ryanbbrown/Retrodict) (no license) ·
  [ryanbbrown/thinharness](https://github.com/ryanbbrown/thinharness)
