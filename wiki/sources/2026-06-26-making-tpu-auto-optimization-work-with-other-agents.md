# Making TPU Model Performance Auto-optimization work with other Agents (blog, 2026-06-26)

The author's account of *why* Codex and Gemini CLI couldn't reliably run the autoresearch loop even after
the `/loop` + Stop-hook + retrospective guardrails from the
[prior post](2026-06-05-making-karpathy-autoresearch-production-ready.md), and the fix: decomposing one
monolithic loop prompt into a small number of purpose-built **skills** and **sub-agents**.

## Overview
The diagnosis is a second, different-shaped instance of context pollution: the *previous* fixes solved
"the top-level instructions sink over a long session," but the loop body itself was still one giant prompt
per iteration — "read these ten wiki pages, look at three prior experiments, pick a hypothesis, write a
falsification criterion, edit the model, build, submit, poll, analyze the profile, write the verdict," all
competing for the same context window in the same turn. A strong model (Opus 4.7) had enough headroom to
track all of it; weaker models cut corners — skipped the profile, blind-flag-swept instead of testing a
real hypothesis, handed back control mid-experiment
([raw](../../raw/papers/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)). The fix
generalizes the Software 3.0 framing from the prior post: reliability — not just capability — requires
splitting one big prompt into small, single-purpose components.

## Key claims

1. **Skills vs. sub-agents is a context-sharing vs. context-isolation choice, not a naming detail.** A
   **skill** is a slash-command prompt loaded into the master's own context — cheap, stateful, good for
   decisions the master needs to remember. A **sub-agent** is a separate conversation with its own context
   window; only a summary returns to the master — expensive per call, but keeps the master's context clean.
   The author's rule of thumb: *if the work needs the master to remember it, use a skill; if the work would
   burn tens of thousands of tokens of intermediate output the master doesn't need, use a sub-agent.* This
   maps across harnesses with the same shape under different names (Claude Code, Antigravity, Codex all
   expose both).
2. **Sub-wiki scoping — force-load only the relevant slice, never the whole wiki.** Left to its own
   judgment, an agent does "a sloppy job" of deciding what to read from a large wiki. The fix used
   throughout: extract a domain-specific slice (e.g.
   [`model-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-index.md)
   for hypothesis formulation, a separate `profile-analyzer-index.md` for profile/HLO interpretation) and
   force the relevant skill/sub-agent to load *only* that slice — never the whole wiki.
3. **`/formulate-hypothesis` force-loads three layers before proposing anything** — a domain-specific
   optimization index (topics + pointers), a generic optimization blueprint (ordered phases:
   substrate-sanity → cheap memory/precision → known-good flag bundles → kernel/structural work →
   batch/sequence amortization → cross-variant transfer → exploratory sweeps last), and per-model state
   (recent experiments, most recent retrospective, a `refuted-patterns.md`). The output is checked against
   both refuted-pattern layers before dispatch — "the largest safeguard against repeat-failure
   regressions." This is a skill, not a sub-agent, because the decision belongs to the master and the
   context cost of loading the two index files is small enough to keep.
4. **`gke-cluster-runner` is the canonical "isolate a long, noisy, parallel task" sub-agent.** Launch, poll,
   and artifact capture for a cluster workload used to run inline in the master session — kubectl/XPK
   output that contributed nothing to the next decision filled the master's context, and a 10–60 minute
   multi-host workload blocked the master from doing anything else. Moved to a background sub-agent, the
   noise stays isolated and the master gets a callback on completion. Notable finding: **no matter how many
   times you instruct an agent to keep polling, it eventually stops** — reliable polling is itself a
   context-pollution victim, not a discipline problem.
5. **`profile-analyzer` is the canonical "isolate a context-heavy interpretation step" sub-agent, run
   synchronously.** A single xprof trace is hundreds of MB; an HLO dump is thousands of files — analyzing
   them inline consumed tens of thousands of tokens per experiment, most of the master's window going to
   remembering profile data rather than deciding what to try next. Moved to a sub-agent, it returns only two
   paste-ready markdown sections (`## Profile`, `## HLO Dump`). It runs *synchronously* (not backgrounded,
   unlike `gke-cluster-runner`) because the master genuinely cannot pick the next hypothesis without this
   result — the blocking cost (30s–2min) is worth paying.
6. **The hypothesis-firing audit is a distinct, load-bearing third phase inside `profile-analyzer`.**
   It reads the experiment stub's `Predicted signal` / `Mechanism` labels and checks the HLO dump for
   structural evidence the predicted mechanism actually fired (e.g., does `tokamax_ce` actually appear as
   a `custom_call`). If not: `SILENT NO-OP DETECTED`, verdict downgraded to inconclusive. Before this
   check, silent no-ops — the compiler quietly optimizing away a change, or a flag never taking effect —
   would sometimes get filed as `supported` on a lucky noise sample; after it, they don't reach dispatch.
7. **The loop's own artifacts feed back into its own instructions (self-improvement, two mechanisms).**
   (a) *Production*: the ordered phase blueprint
   ([`model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md))
   is itself LLM-extracted from the corpus of `supported` experiments via a canned regeneration prompt, and
   is periodically regenerated as the corpus grows. (b) *Exploratory, not yet productionized*: session logs
   (which skills/sub-agents fired, where the master looped on a refuted hypothesis) are themselves
   analyzable material for improving the skill/sub-agent definitions — the author notes different LLMs
   have different quirks (Codex follows instructions most literally; Opus is most flexible; Gemini needed
   the surgical-edit discipline enforced harder) that could motivate per-harness skill variants.
8. **`/edit-model-code` productionizes Karpathy's general LLM-coding guidelines** (think before coding,
   simplicity first, surgical changes, goal-driven execution) as a skill invoked before any per-experiment
   code edit. The author reports the failure rate from "wrong or overly aggressive code change" dropped
   visibly on Gemini once this was in place (no controlled A/B was run).

## Key data points

Qwen3 8B head-to-head, same repo/skills/sub-agents/wiki/hardware/baseline, one-line kickoff prompt, left
unattended per harness:

| Harness / model | Top MFU | Delta vs MaxText 39.8% | Loop behavior |
|---|---:|---:|---|
| Codex + GPT-5.5 | 43.2% | +8.5% | Ran cleanly end-to-end; fewest silent no-ops caught by the audit; aggressive on structural code changes. |
| Claude Code + Fable 5 | 39.9% | +0.3% | Fastest per-iteration wall clock; good profile pattern recognition. |
| Claude Code + Opus 4.8 | 34.8% | −12.6% | Solid but conservative — favored flag sweeps over kernel work. |
| Antigravity + Gemini 3.1 Pro | 30.6% | −23.1% | First time this harness ran the loop end-to-end unattended; `/edit-model-code` was "clearly load-bearing." |

All four ran the loop **unattended** and filed real experiment trails — the point of the case study is
explicitly that specialization (not any one model's superiority) is what made that possible; before it,
only Claude Code + Opus 4.7 reliably got past hypothesis formulation.

## Gaps & caveats
- No controlled before/after A/B for `/edit-model-code`'s effect on Gemini's failure rate — reported as an
  observed, not measured, improvement.
- The "process optimization from session logs" self-improvement mechanism is explicitly exploratory /
  not yet productionized, unlike the blueprint-regeneration mechanism.
- Per-harness skill variants are floated as a plausible future direction, not something implemented.

## Connections
- [Making Karpathy's autoresearch production-ready](2026-06-05-making-karpathy-autoresearch-production-ready.md) —
  the guardrails (`/loop`, Stop hook, retrospective) this post's decomposition builds on.
- [tpu_performance_autoresearch_wiki — methodology summary](tpu-performance-autoresearch-wiki.md) — `#`
  The `formulate-hypothesis` skill, `#` Coding discipline for the agent's edits sections describe
  `formulate-hypothesis` / `edit-model-code` from the skill-file side; this post explains why they exist
  and adds the `gke-cluster-runner` / `profile-analyzer` sub-agents and the hypothesis-firing audit, which
  weren't in the skill files pulled earlier.
- [Wiki-driven autoresearch loop](../topics/wiki-driven-autoresearch-loop.md) — synthesis topic page,
  extended with the skill-vs-sub-agent axis and sub-wiki-scoping pattern from this post.

## Sources
- [`raw/papers/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md`](../../raw/papers/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)
- Original: https://vlasenkoalexey.github.io (post dated 2026-06-26)
