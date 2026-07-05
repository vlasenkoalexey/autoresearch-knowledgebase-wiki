# Making Andrej Karpathy's autoresearch production-ready (blog, 2026-06-05)

The author's diagnosis of *why* the autoresearch loop from the
[first post](2026-05-01-tpu-model-performance-auto-optimization.md) needed babysitting, and the three
external guardrails added to fix it — none of which change the loop's logic, all of which fight context
degradation in a long-running agentic session.

## Overview
The central diagnosis: every failure mode (complaining, asking permission, stopping early, narrowing to
one direction) traces back to **context pollution** — the loop instructions sit at the top of the context
at session start, but sink further down every turn, and a sufficiently long session eventually gives them
less effective weight than everything accumulated on top
([raw](../../raw/papers/2026-06-05-making-karpathy-autoresearch-production-ready.md)). The post frames this
using Karpathy's own Software 1.0/2.0/3.0 distinction: this loop is Software 3.0 (a prompt/collection of
prompts run in an agentic harness) — deterministic code could force the loop mechanically, but the author
argues non-determinism here is a feature, and the fix should be an external guardrail, not a rewrite into
traditional control flow.

## Key claims

1. **Instruction re-injection (`/loop`) fixes drift, not compliance.** A scheduler periodically re-pushes
   the autoresearch instructions back to the top of context — the same effect as manually telling the
   model to re-read them. This must be an *external* mechanism (a harness-level scheduler), because an
   in-context instruction to "re-read yourself periodically" is exactly the kind of instruction that
   degrades under the same pollution it's meant to fix.
2. **A Stop hook enforces "never stop" as a mechanical gate, not a policy.** Even with instructions and
   `/loop` re-injection, the agent still tried to hand control back early. Claude Code's Stop hook fires
   when the agent attempts to end its turn; the author's hook is session-filtered (hooks are global, so the
   hook's own logic must check it's the right session before acting) and can inject arbitrary follow-up
   instructions — not just "keep going," but a specific corrective action.
3. **Retrospectives break narrow exploration, and are dispatched via the same Stop-hook mechanism.**
   "Exhausted all ideas" is sometimes locally true (a flag sweep really can run out of values) but globally
   false (other topics were never explored). The fix is the same engineering habit as "step back and review
   your data" — a `/create-retrospective` skill that reviews every experiment run so far, is bundled into
   the Stop hook, and can also be invoked manually at any time.
4. **Parallelizing the loop across models required per-experiment repo forks, not shared branches.**
   Autoresearch's single-branch-per-experiment model clobbers itself across concurrent loops. The author
   tried three designs — (a) one clever orchestrator + dumb workers (failed: context pollution on the
   orchestrator), (b) one dumb orchestrator + clever workers (worked, but needed a dashboard to track every
   worker), (c) fork/copy the whole repo per experiment and run an independent session per model (what
   shipped) — landing on copy-the-repo as simplest despite the disk-space cost, because "disk is cheap."
5. **Each fix is a guardrail *around* the same loop, not a redesign of it.** `/loop` keeps instructions on
   top; the Stop hook catches early exits; the retrospective widens exploration. None of the three change
   what the loop is deciding — they change whether the loop keeps deciding at all.

## Gaps & caveats
- The author states explicitly these tweaks did **not** fix Codex or Gemini CLI's reliability — that gap is
  closed in the next post, [Making TPU auto-optimization work with other agents](2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md).
- Explicitly framed as "not a critique of autoresearch" — the original repo is deliberately minimal and
  wasn't meant to carry this operational weight; these are the author's own production add-ons for a
  specific larger use case.
- No quantified before/after (e.g., hours of unattended runtime before vs. after) — the claim "was able to
  leave it running for many hours without supervision" is qualitative.

## Connections
- [karpathy/autoresearch — the autonomous experiment loop](../code/autoresearch/doc-concepts/autonomous-experiment-loop.md) —
  the original "NEVER STOP" policy this post turns into an enforced mechanism.
- [tpu_performance_autoresearch_wiki — methodology summary](tpu-performance-autoresearch-wiki.md) — `#`
  Retrospectives — a coverage-gap audit, `#` Bootstrap, launch, and shutdown skills sections describe the
  `create-retrospective` / `start-experiment` / `stop-experiment` skills this post motivates.
- [Wiki-driven autoresearch loop](../topics/wiki-driven-autoresearch-loop.md) — synthesis topic page,
  extended with the context-pollution diagnosis from this post.

## Sources
- [`raw/papers/2026-06-05-making-karpathy-autoresearch-production-ready.md`](../../raw/papers/2026-06-05-making-karpathy-autoresearch-production-ready.md)
- Original: https://vlasenkoalexey.github.io (post dated 2026-06-05)
