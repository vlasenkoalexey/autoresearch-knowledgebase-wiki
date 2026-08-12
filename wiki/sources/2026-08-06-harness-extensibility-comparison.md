# Harness Extensibility: Claude Code vs. Antigravity vs. Codex (2026-08-06)

A design reference, written inside the
[tpu_performance_autoresearch_wiki](tpu-performance-autoresearch-wiki.md) project, for running **one
autoresearch protocol across three agent harnesses**. It introduces the six extension mechanisms from
scratch, compares Claude Code, Antigravity (Gemini), and Codex at spec level with every claim linked to
first-party docs, and closes with a **measured** worked example from the project's own repos. Its interest
to this wiki is not vendor comparison but the general question underneath it: *when an autoresearch loop is
a body of markdown protocol plus a set of delegated roles, what part of that is portable, and what has to
be rebuilt per host?* Raw clip:
[`raw/papers/2026-08-06-harness-extensibility-comparison.md`](../../raw/papers/2026-08-06-harness-extensibility-comparison.md).

## Overview

The framing device is the one that makes the document generally useful. An agent session starts empty;
everything it knows must be put in front of it, and everything put in front of it consumes the same context
window the work needs. Three of the six mechanisms — **instruction files, skills, sub-agents** — are
therefore presented not as alternatives but as **points on one spectrum: when should a piece of knowledge
be loaded?**

| Mechanism | Header (name + description) | Body |
|---|---|---|
| **Instruction file** | — | parent context, **always** |
| **Skill** | parent context, at startup, always | parent context **on invocation**, then persists for the session |
| **Sub-agent** | parent context, at startup, always | **child context only — never enters the parent** |

The remaining three differ in kind rather than timing: **tools** are what the agent can *do*, **hooks** are
what it *cannot avoid*, and **plugins** are how any of it *ships*.

## Key claims

**Skills are the one ratified cross-vendor format; everything else diverges.** All three implement the
[Agent Skills](https://agentskills.io/) standard — a directory with `SKILL.md`, YAML frontmatter carrying
`name`/`description`, Markdown body, three-stage progressive disclosure. The cost model is stated sharply:
a skill's cost is *"zero, then permanent"* — the body enters the conversation once and stays for the
session — which is an argument for tight bodies, not just tight headers.

**Portability ends at the frontmatter.** Claude Code accepts ~22 frontmatter fields against the spec's six.
Lost on port: invocation control, arguments/parameterization, `context: fork|agent|background`, per-skill
model and effort routing, per-skill tool grants, skill-scoped hooks, dynamic `` !`cmd` `` context injection,
and path substitution. The trap named is **silent divergence** — Antigravity and Codex *ignore* unknown
frontmatter keys rather than erroring, so a skill using Claude Code fields "appears to work everywhere
while behaving differently on each." The recommended validation is to package against the six-field spec,
which fails loudly.

**Sub-agents share only the concept.** This is called out as the dimension of maximum disagreement: file
format (Markdown+YAML vs **TOML**), path, invocation trigger, tool inheritance, model selector, sandbox
control, nesting limit (Claude Code 3, Antigravity 10, **Codex 1**), concurrency limit (20 live/200 per
session vs undocumented vs 6), and whether a plugin can bundle one at all (Codex: no) are each decided
differently. Only four properties agree: fresh context window, skill preloading, MCP scoping, and roughly
the required fields.

**Which disagreements matter is the load-bearing distinction.** Format divergence is *cheap* (an encoding
difference over identical semantics). **Invocation divergence is not**: auto-delegation is the default on
Claude Code, requires an explicit `invoke_subagent` call on Antigravity, and is paywalled to ChatGPT Ultra
on Codex — so *"any orchestration depending on the model choosing to delegate is not portable."* And
**tool-surface divergence is invisible**: Claude Code documents filters narrowing a sub-agent's inherited
tools; neither competitor documents an equivalent, so the effective tool surface elsewhere cannot be
predicted from the definition file.

**Codex sub-agents are a parallelism mechanism, not an isolation mechanism.** *"Subagents use the tools
available to the parent chat"* — no per-agent tool restriction, so least-privilege delegation is
unavailable; depth-1 nesting by default; six concurrent threads; not bundleable in plugins; and in
non-interactive runs an action needing approval fails and surfaces to the parent, so unattended delegation
"dies on the first prompt."

**Hooks are the only mechanism that enforces anything.** Instruction files, skills, and sub-agents are
*guidance* — the model reads them and usually complies. A hook *"executes regardless of what the model
decides."* Claude Code documents 31 events and five handler types; Codex 11 events and reimplements the
Claude Code contract field-for-field (same stdin envelope, same exit-code semantics, same output fields),
so a `command` handler typically runs unmodified under both. Antigravity is a *different design*, not a
subset: 5 events, `PreInvocation`/`PostInvocation` firing around each **model call** rather than each tool
call, no documented exit-code protocol, and a 30 s default timeout (20× tighter than the other two).
**Three-way overlap is exactly `PreToolUse`, `PostToolUse`, `Stop`.**

**Plugins: skip the mechanism if you need all three.** The bundles are structurally non-equivalent (a
plugin shipping a specialist sub-agent cannot exist on Codex; a plugin shipping rules works only on
Antigravity; Antigravity has no marketplace to publish to). The recommendation is explicit: *"if you need
all three harnesses, distribute the repository, not a plugin."*

## The compatibility-layer rules (the transferable part)

Each section closes with a rule, and the rules differ by mechanism rather than being one uniform strategy —
which is the document's actual thesis:

| Mechanism | Rule | Mechanism used |
|---|---|---|
| Instruction files | "The protocol exists once. **Never triplicate it**" | symlink · symlink + delta · canonical file + pointers |
| Skills | "**One skill tree, no adapters**" | one directory, exposed at both roots by symlink |
| Sub-agents | "**One canonical body, one pointer adapter per harness**" | ~1 KB adapter: native fields + pointer + tool-name map |
| MCP | "**Generate all three declarations from one source**" | emitter — cannot be a symlink or pointer |
| Hooks | "Portable only inside the intersection. Outside it, **don't port — re-express**" | standalone executable over the shared JSON envelope |
| Plugins | "Distribute the **repository**, not a plugin" | git template |

Three cross-cutting rules generalize past this vendor set:

- **Dispatch by name, never by inference** — anything relying on the model *choosing* to delegate silently
  degrades to inline execution where auto-delegation isn't available.
- **Declare the fallback for missing adapters** — coverage will be partial; say in the instruction file
  what to do when a role has no adapter on this host.
- **Degrade, never emulate** — *"If delegation is unavailable, the caller must record the result as missing
  rather than producing it inline. An agent that writes its own verifier's output has defeated the
  isolation the sub-agent existed to provide."* This is the same invariant the kernel lane enforces
  socially (author ≠ verifier); here it is stated as a portability rule. See
  [`concepts/verification-independence.md`](../concepts/verification-independence.md).

## Key data points

Measured from the project's own repos rather than quoted from docs:

| Agent | canonical body | Antigravity adapter | Codex adapter | Adapter overhead |
|---|--:|--:|--:|--:|
| `profile-analyzer` | 23,868 B | 734 B | 1,103 B | 7.7% |
| `kernel-verifier` | 21,353 B | 812 B | 1,674 B | 11.6% |
| `process-auditor` | 12,719 B | 850 B | 2,285 B | 24.6% |

Three ~1 KB pointers replace three ~20 KB copies, and *"drift is structurally impossible because one body
exists."* Skills need no adapter at all — one symlink publishes fifteen skills to all three harnesses with
zero glue files, which the document presents as the Tier-1/Tier-2 boundary made concrete. The protocol
itself, triplicated, would be ~1,800 lines across three files; as a canonical `SCHEMA.md` plus three
pointers it is ~600 lines plus three small entry files.

The **portability tiers**: *Tier 1* (moves unmodified) is skill bodies, skill `name`/`description`, bundled
skill files, the `.agents/skills/` root. *Tier 2* (needs a generator or pointer) is sub-agent definitions,
hooks inside the shared event set, MCP declarations, plugin bundles. *Tier 3* (no target — re-express or
drop) includes worktree isolation, per-agent memory, per-skill model/effort, frontmatter hooks, 20 of
Claude Code's 31 hook events, Antigravity's per-invocation hooks, and Codex's `ultra` reasoning effort.

## Gaps & caveats

- **It is a spec-level comparison, not a benchmark.** It compares what the docs promise; the only
  behavioural measurements are the file sizes in §9. Where a vendor documents nothing (Antigravity's
  concurrency limits, effective sub-agent tool surface), the document says so rather than inferring.
- **The vendor surfaces move fast.** Compiled 2026-08-06 against then-current docs; the document itself
  records that Codex doc URLs 308-redirect to a new host as of that date, and flags four claims as **not
  first-party** (an Antigravity version number sourced from a forum, a plugin subdirectory documented in
  the CLI docs but absent from the IDE page, Codex plugin-directory size and publishing status).
- **The reference implementation is the author's own repo**, so §9 is a self-consistent example rather than
  an independent test — and the document is candid where its own repo *violates* its rules: the MCP section
  notes the project declares one server twice by hand, that the two declarations have already drifted
  between the public and private forks, and that the Antigravity schema has no field able to express the
  difference. *"This is the dimension where the repo does not implement the rule, and the failure mode is
  exactly the predicted one."*
- Its recommendation for its own layout is qualified rather than universal: the repo uses the
  canonical-file-plus-pointers shape because it predates Antigravity's `AGENTS.md` support and carries
  substantial per-harness deltas, *"but a project starting today with a short, uniform protocol should
  reach for"* the plain symlink.

## Connections

- [tpu_performance_autoresearch_wiki — methodology summary](tpu-performance-autoresearch-wiki.md) — the
  project this was written for; §6.4 documents the retirement of that project's `Stop` hook in favour of a
  harness-native scheduled watcher, which is the "re-express, don't port" rule applied to its own
  supervision mechanism.
- [Making TPU auto-optimization work with other agents (2026-06-26)](2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)
  — the earlier post that established the skills-vs-sub-agents split for this project. This document is the
  cross-harness generalization of that decision rule; the two agree on the criterion (*isolate when the
  work produces output the caller never needs*) and this one adds the portability consequences.
- [Wiki-driven autoresearch loop](../topics/wiki-driven-autoresearch-loop.md) — where the
  skills-vs-sub-agents decision rule is synthesized as a general property of agentic loops.
- [`concepts/verification-independence.md`](../concepts/verification-independence.md) — "degrade, never
  emulate."

## Sources
- [`raw/papers/2026-08-06-harness-extensibility-comparison.md`](../../raw/papers/2026-08-06-harness-extensibility-comparison.md)
  — the full document (compiled 2026-08-06; ~30 first-party doc links plus its own measured §9)
