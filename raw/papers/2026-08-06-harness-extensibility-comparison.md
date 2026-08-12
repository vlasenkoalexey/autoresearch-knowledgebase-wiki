---
title: "Harness Extensibility: Claude Code vs. Antigravity vs. Codex"
type: analysis
tags: [claude-code, antigravity, codex, skills, subagents, hooks, mcp, plugins, translation-layer, agent-skills]
created: 2026-08-06
updated: 2026-08-06
---

# Harness Extensibility: Claude Code vs. Antigravity vs. Codex

Design reference for a cross-harness translation layer. §1 introduces the extension mechanisms from scratch; §2–§7 compare the three harnesses at spec level; §8–§9 cover what actually ports.

**Compiled 2026-08-06.** Every claim links to its source. §9 is measured from this repo and its public template, not quoted from docs.

**Contents** — [§1 Concepts](#1-concepts) · [§2 Instruction files](#2-instruction-files) · [§3 Skills](#3-skills) · [§4 Sub-agents](#4-sub-agents) · [§5 MCP](#5-mcp) · [§6 Hooks](#6-hooks) · [§7 Plugins](#7-plugins) · [§8 Portability](#8-portability) · [§9 Worked example](#9-worked-example) · [§10 References](#10-references)

---

## 1. Concepts

An agent session starts empty. Everything the agent knows about your project — the build command, the deploy checklist, the reason a directory is off-limits — has to be put in front of it, and everything put in front of it consumes the same context window it needs for the actual work.

The first three mechanisms below — instruction files, skills, sub-agents — are three answers to one question: **when should a piece of knowledge be loaded?** They are not alternatives to each other so much as points on a spectrum, from "always in context" through "loaded on demand" to "never in context, executed elsewhere." §1.4 gives the decision rule.

The remaining three differ in kind rather than in timing: **tools** are what the agent can *do*, **hooks** are what it *cannot avoid*, and **plugins** are how any of it *ships*.

### 1.1 Instruction files

An **instruction file** is a Markdown file at a known path that the harness loads at the start of every session. `CLAUDE.md`, `AGENTS.md`, and `GEMINI.md` are the same idea under three vendor filenames. The content is standing facts: *run `make lint` before committing*, *API handlers live in `src/api/handlers/`*, *never edit files under `vendor/`*.

The defining property is that it is **always loaded**. That makes it right for things true on every turn and wrong for anything long or situational, since it is charged to the context window whether or not this session touches the topic. Claude Code advises keeping one under 200 lines for exactly that reason ([Memory](https://code.claude.com/docs/en/memory)).

Instruction files are guidance, not enforcement. The harness says so plainly: they are *"context, not enforced configuration. To block an action regardless of what Claude decides, use a PreToolUse hook instead"* ([Memory](https://code.claude.com/docs/en/memory)).

### 1.2 Skills

A **skill** is an instruction file with a loading condition. Physically it is a directory containing a `SKILL.md`, and that file has two parts that are loaded at different times:

- The **header** is YAML frontmatter between `---` markers, carrying a `name` and a `description` of when the skill applies. It is one or two lines.
- The **body** is everything after the frontmatter: the actual procedure, in Markdown.

**The header is loaded at session start, for every skill you have. The body is not loaded until the skill is invoked.** That split is the mechanism — called **progressive disclosure** — and it is the whole point of the format. Fifty skills cost fifty descriptions at startup, not fifty procedures. The body arrives only when a task matches, either because the model matched the description or because you typed `/skill-name`, which makes a skill double as a slash command.

Once the body does load, it stays. Claude Code documents it explicitly: the rendered content *"enters the conversation as a single message and stays there for the rest of the session"*, and the file is not re-read on later turns ([Skills](https://code.claude.com/docs/en/skills)). So a skill's cost is zero, then permanent — which is an argument for keeping bodies tight, not just headers.

Optional files can sit alongside `SKILL.md` (`scripts/`, reference docs, templates). These are a third tier: not loaded at startup, and not loaded on invocation either — only if the body tells the agent to read them.

Concretely: a `release` skill whose header description reads *"Use when the user asks to cut a release or publish a version"* and whose body is the twelve-step release checklist. The description is in context all session; the checklist costs nothing until someone releases.

Claude Code states the tradeoff against instruction files directly: *"a skill's body loads only when it's used, so long reference material costs almost nothing until you need it"* ([Skills](https://code.claude.com/docs/en/skills)).

Skills are the one mechanism with a ratified cross-vendor format — [Agent Skills](https://agentskills.io/), originated by Anthropic, released openly, implemented by ~40 clients.

### 1.3 Sub-agents

A **sub-agent** is a second agent session spawned by the first. It gets a fresh context window, its own system prompt, usually a restricted tool set, and no view of the parent conversation. It does the work and returns a summary; the intermediate steps never enter the caller's context.

Its definition file has the same two parts as a skill, but they load into *different context windows*:

- The **header** carries a `name` and a `description` of when to delegate, plus optional overrides for tools, model, and sandbox. It is loaded into the **parent's** context at session start, exactly like a skill header — that is how the parent knows the sub-agent exists and when to reach for it.
- The **body** becomes the **child's system prompt**. It is never loaded into the parent at all.

That is the sharpest way to state the difference from a skill: both cost the parent a description forever, but a skill's body eventually lands in your context, and a sub-agent's body lands in a context you never see.

| | Header (`name` + `description`) | Body |
|---|---|---|
| **Skill** | Parent context, at startup, always | Parent context, on invocation, then persists for the session |
| **Sub-agent** | Parent context, at startup, always | Child context only — never enters the parent |

Concretely: a `test-runner` sub-agent whose header says *"Use to run the test suite and report failures"* and whose body is the instructions for doing that. It runs the suite, reads four thousand lines of failure output, and returns the six tests that actually broke. Neither the body nor the four thousand lines ever touch the main session.

All three harnesses describe the purpose identically. [Claude Code](https://code.claude.com/docs/en/sub-agents): *"Each subagent runs in its own context window."* [Antigravity](https://antigravity.google/docs/subagents): it *"does not inherit the parent's existing conversation history (context window), starting with a clean slate."* [Codex](https://learn.chatgpt.com/docs/agent-configuration/subagents) frames it as defense against *"context pollution"* and *"context rot."*

### 1.4 Choosing between the three

The three mechanisms above carry the same kind of payload — Markdown instructions — and differ only in when and where it lands. Two questions separate them.

| Question | Answer |
|---|---|
| Is it a **fact** the agent should hold on every turn? | Instruction file |
| Is it a **procedure** needed only sometimes? | Skill |
| Will doing it produce **output the caller doesn't need to see**? | Sub-agent |

**Instruction file → skill.** Move an entry out of the instruction file when it stops being a fact and becomes a procedure. Claude Code's rule: *"Keep it to facts Claude should hold in every session… If an entry is a multi-step procedure or only matters for one part of the codebase, move it to a skill"* ([Memory](https://code.claude.com/docs/en/memory)). From the other direction: *"Create a skill when you keep pasting the same instructions, checklist, or multi-step procedure into chat, or when a section of CLAUDE.md has grown into a procedure rather than a fact"* ([Skills](https://code.claude.com/docs/en/skills)).

**Skill → sub-agent.** This is an isolation decision, not a reuse decision. Both are reusable; the difference is that a skill executes *in* your conversation and a sub-agent executes *beside* it. Delegate when the work generates volume you will never reference again — test output, log files, search results — or when you want to hard-limit which tools the worker can touch. Keep it inline when the work needs back-and-forth, when later phases depend on context the sub-agent won't have, or when the task is small enough that a cold start costs more than it saves ([Subagents](https://code.claude.com/docs/en/sub-agents)).

The costs are real and asymmetric. A sub-agent starts cold and must rediscover context the parent already has, adding latency. It runs its own model and tool calls, so it costs strictly more tokens than doing the work inline — Codex says so outright: *"Subagent workflows consume more tokens than comparable single-agent runs"* ([Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents)). And the savings evaporate if children return detailed results instead of summaries; Claude Code warns that many sub-agents each returning full findings *"can consume significant context."*

A useful default: reach for a skill first. Escalate to a sub-agent when you can name the specific output you don't want in your context.

### 1.5 Tools and MCP

A **tool** is a function the agent can call: read a file, run a shell command, query an API. Built-in tools ship with the harness. External ones arrive over the **Model Context Protocol (MCP)** — an open standard for exposing a service's capabilities to any agent that speaks it, originated by Anthropic and now governed by the Linux Foundation's [Agentic AI Foundation](https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation) alongside `AGENTS.md` and Goose.

An MCP server is a process, local or remote, that advertises a set of tools. Connecting one adds those tools to the agent's repertoire for the session. Every tool's schema sits in context permanently, so connecting many servers is not free.

Tools sit underneath everything above: an instruction file, a skill, and a sub-agent all end in a tool call. They are also the layer where the three harnesses converged furthest — an MCP server written once runs against all three, though its *configuration* is declared three incompatible ways (§5).

### 1.6 Hooks

A **hook** is a shell command the harness runs at a fixed lifecycle point — before a tool call, after one, when the turn ends. The harness pipes it a JSON description of what is happening on stdin; the command's exit code and stdout can allow, block, or modify the action.

Hooks are categorically different from instruction files, skills, and sub-agents. Those are *guidance*: the model reads them and usually complies. A hook **executes regardless of what the model decides**, which makes it the only mechanism that can enforce anything. If a rule must hold — no writes outside `src/`, always run the formatter after an edit — it belongs in a hook, not an instruction file.

### 1.7 Plugins and marketplaces

A **plugin** is a versioned bundle of the above — some skills, some sub-agents, hooks, MCP server declarations — installed as a unit with a manifest describing it. A **marketplace** is a catalog you install plugins from, which is how a plugin reaches someone who didn't write it.

Plugins add no new capability; they are the packaging and distribution story for capabilities that already exist.

---

## 2. Instruction files

| | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Workspace file** | `CLAUDE.md`, `./.claude/CLAUDE.md` | `GEMINI.md` **and** `AGENTS.md` | `AGENTS.md` |
| **Global file** | `~/.claude/CLAUDE.md` | `~/.gemini/GEMINI.md` | `~/.codex/AGENTS.md` |
| **Modular rules dir** | `.claude/rules/*.md`, glob-scoped via `paths:` frontmatter | `.agents/rules/` (legacy `.agent/rules/`) | — |
| **Per-file size cap** | none (advises <200 lines) | **12,000 characters** | none documented |
| **Include syntax** | `@path/to/file`, max 4 hops | `@filename`, relative to the rules file | none |
| **Org layer** | `/etc/claude-code/CLAUDE.md`, `claudeMd` in managed settings | — | — |

Sources: [CC Memory](https://code.claude.com/docs/en/memory) · [AG Rules & Workflows](https://antigravity.google/docs/rules-workflows) · [AG CLI best practices](https://antigravity.google/docs/cli/best-practices) · [Codex Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents)

**`AGENTS.md` is read by two of three; Claude Code is the holdout.** Antigravity parses it alongside `GEMINI.md` — *"The agent continues to parse and enforce rule constraints defined inside your active directory's `GEMINI.md` and `AGENTS.md` files"* ([CLI migration](https://antigravity.google/docs/cli/gcli-migration)); IDE support landed in [v1.20.3, 2026-03-05](https://discuss.ai.google.dev/t/antigravity-update-1-20-3-2026-3-5/129320), and precedence between the two is undocumented. Claude Code is explicit that it doesn't participate: *"Claude Code reads `CLAUDE.md`, not `AGENTS.md`"* ([Memory](https://code.claude.com/docs/en/memory)).

**Bridging the holdout.** Anthropic documents the fix rather than adopting the format: *"create a `CLAUDE.md` that imports it so both tools read the same instructions without duplicating them"* — via `@AGENTS.md` or `ln -s AGENTS.md CLAUDE.md` ([Memory](https://code.claude.com/docs/en/memory)).

### 2.1 Compatibility layer

**Rule: the protocol exists once. Never triplicate it** — three hand-maintained copies are edited independently and diverge within a week. Three shapes achieve that, in increasing order of cost. Pick by how much harness-specific content you actually need.

**Shape A — symlink.** Since Antigravity reads `AGENTS.md` natively (§2), one file can serve all three: put the protocol in `AGENTS.md`, read directly by Codex and Antigravity, and link Claude Code to it.

```bash
ln -s AGENTS.md CLAUDE.md
```

Anthropic documents this exact form, with its condition: *"A symlink also works if you don't need to add Claude-specific content"* ([Memory](https://code.claude.com/docs/en/memory)). Zero indirection, zero extra tool calls, one file to edit. Three caveats: it is Windows-hostile — *"creating a symlink requires Administrator privileges or Developer Mode, so use the `@AGENTS.md` import instead"* — you cannot add per-harness content by construction, and the whole protocol now sits in a file Antigravity treats as a rules file, so a long one may hit the 12,000-character cap that a pointer file would have avoided.

**Shape B — symlink plus a delta file.** Same as A, but add `GEMINI.md` carrying only Antigravity-specific content. Antigravity reads both files, so `GEMINI.md` must *not* re-import `AGENTS.md` or the protocol loads twice. Claude Code deltas have nowhere to go in `CLAUDE.md` — it is a symlink — so put them in `.claude/rules/*.md`, which also lets you glob-scope them. This buys per-harness content for one extra file and keeps the symlink's directness.

**Shape C — canonical file plus pointers.** Put the protocol in a vendor-neutral file no harness looks for (`SCHEMA.md`, `PROTOCOL.md`) and make each root file a pointer. Claude Code and Antigravity resolve `@filename` includes; Codex has none, so its pointer is a prose instruction costing one tool call. Each root file then carries the harness's own deltas — primitive mappings, gotchas, fallbacks — and nothing that belongs to the protocol.

Choose C when the harnesses need substantially different instructions, or when the protocol is long enough that keeping the root files small matters. Its one structural advantage over A and B: the cap applies to the pointer, not the imported target.

Whichever shape, the canonical file must not assume a vendor's paths. A protocol that says "read `.claude/agents/x.md`" is not neutral, and every non-Claude harness needs a translation note to compensate.

**Live example (Shape C)** — [`SCHEMA.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/SCHEMA.md), ~600 lines, reached from [`CLAUDE.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/CLAUDE.md) (a single line, `@SCHEMA.md`), [`GEMINI.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/GEMINI.md) (the same import plus a Claude→Antigravity primitive map), and [`AGENTS.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/AGENTS.md) (prose pointer plus Codex translation notes). The repo predates Antigravity's `AGENTS.md` support and carries three substantial per-harness deltas, so C is the right shape for it — but a project starting today with a short, uniform protocol should reach for A. Measured in §9.1.

---

## 3. Skills

All three implement [Agent Skills](https://agentskills.io/): a directory containing `SKILL.md`, YAML frontmatter carrying `name` and `description` at minimum, Markdown body carrying the procedure, three-stage progressive disclosure described near-verbatim in each vendor's docs. Claude Code declares the dependency: *"Claude Code skills follow the Agent Skills open standard, which works across multiple AI tools"* ([Skills](https://code.claude.com/docs/en/skills)).

| | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Required frontmatter** | none (`description` recommended) | `description` (`name` defaults to folder) | `name`, `description` |
| **Frontmatter surface** | ~22 fields | 2 | 2 + `agents/openai.yaml` sidecar |
| **Workspace path** | `.claude/skills/<name>/SKILL.md` | `.agents/skills/<name>/` | `$CWD/.agents/skills`, `$REPO_ROOT/.agents/skills` |
| **User path** | `~/.claude/skills/<name>/` | `~/.gemini/config/skills/` (IDE) / `~/.gemini/antigravity-cli/skills/` (CLI) | `$HOME/.agents/skills` |
| **Admin path** | managed settings | — | `/etc/codex/skills`, bundled |
| **Bundled files** | any (`scripts/`, refs) | `scripts/`, `examples/`, `resources/` | `scripts/`, `references/`, `assets/` |
| **Manual invocation** | `/skill-name` | `/skill-name` | `$` (CLI), `/skills`, `@` (ChatGPT) |
| **Suppress model invocation** | `disable-model-invocation: true` | not documented | `policy.allow_implicit_invocation: false` |
| **Listing budget** | `description` + `when_to_use` truncated at 1,536 chars | not documented | list ≤ 2% of context or 8,000 chars |

Sources: [CC Skills](https://code.claude.com/docs/en/skills) · [AG Skills](https://antigravity.google/docs/skills) · [AG CLI Plugins & Skills](https://antigravity.google/docs/cli/plugins) · [Codex Build skills](https://learn.chatgpt.com/docs/build-skills)

### 3.1 Path mapping

Workspace roots differ by one directory: `.claude/skills/` for Claude Code, `.agents/skills/` for Antigravity and Codex. `.agents/skills/` is the neutral path — Antigravity migrated onto it from `.gemini/skills/` and requires the move explicitly (*"you must manually rename or relocate the folder to `.agents/skills/`"*, [CLI migration](https://antigravity.google/docs/cli/gcli-migration)); Codex scans it at CWD, repo root, and `$HOME` ([Build skills](https://learn.chatgpt.com/docs/build-skills)).

A symlink between the two roots yields one tree, in either direction; Claude Code resolves symlinked skill entries natively ([Skills](https://code.claude.com/docs/en/skills)). This is established practice — `.agents/skills/` with symlink bridging is the emerging cross-agent convention ([mcp.directory](https://mcp.directory/blog/cross-agent-skills-cursor-codex-cline-antigravity-gemini-mastra-portability)).

`.agents/` as a whole is *not* shared, though. `skills/` is the only subdirectory all parties agree on: `.agents/agents/` and `.agents/rules/` are Antigravity-only, and `.agents/plugins/` means installed plugin directories to Antigravity ([Plugins](https://antigravity.google/docs/plugins)) but a marketplace manifest to Codex ([Build plugins](https://learn.chatgpt.com/docs/build-plugins)).

### 3.2 Frontmatter is where portability ends

Claude Code accepts ~22 fields; the spec accepts six. Its docs draw the line and enforce it with a hard error:

> Outside Claude Code, you can use only the fields in the Agent Skills spec: `name`, `description`, `license`, `compatibility`, `metadata`, `allowed-tools`. — [Skills](https://code.claude.com/docs/en/skills)

| Group | Claude Code-only | Lost on port |
|---|---|---|
| Invocation control | `disable-model-invocation`, `user-invocable`, `when_to_use`, `paths` | Who triggers, and when it's offered |
| Arguments | `argument-hint`, `arguments`; `$ARGUMENTS`, `$N`, `$name` | Parameterized skills |
| Execution context | `context: fork`, `agent`, `background` | Running a skill as a sub-agent |
| Model | `model`, `effort` | Per-skill routing |
| Permissions | `allowed-tools`, `disallowed-tools` | Per-turn tool grants and denials |
| Lifecycle | `hooks` | Skill-scoped hooks |

Two body-level features are also Claude Code-only ([Skills](https://code.claude.com/docs/en/skills)): **dynamic context injection**, where `` !`cmd` `` executes before the model sees the file and is replaced by its output — *"preprocessing, not something Claude executes"* — the only mechanism in any of the three that produces a runtime-generated instruction; and **path substitution** (`${CLAUDE_SKILL_DIR}`, `${CLAUDE_PROJECT_DIR}`), which expands in both the body and `allowed-tools`, letting a skill run its own bundled script without a permission prompt.

**Codex's sidecar is the portable design.** Frontmatter stays at two fields; presentation and policy move to `agents/openai.yaml` — `interface.*`, `policy.allow_implicit_invocation`, `dependencies.tools` ([Build skills](https://learn.chatgpt.com/docs/build-skills)).

### 3.3 Compatibility layer

**Rule: one skill tree, no adapters.** This is the only dimension that needs no per-harness file, and the layer's job is to keep it that way.

1. Maintain one directory of skills and expose it at both roots with a symlink. Direction is free; pick the canonical root by which harness you author in.
2. Hold frontmatter at `name` and `description`. Everything a harness might not understand goes in the body, which is fully portable, or in a vendor-namespaced sidecar next to `SKILL.md`.
3. Write the body against capabilities, not tool names. A body that says "run the tests" ports; one that says "use the Bash tool" needs a mapping note for Antigravity (`run_command`) and Codex.
4. Encode invocation intent in the `description` prose, not only in frontmatter. `disable-model-invocation` is Claude Code-only and `policy.allow_implicit_invocation` is Codex-only; Antigravity has neither, so a skill that must not fire on its own has to say so in words.

The trap is silent divergence: Antigravity and Codex ignore unknown frontmatter keys rather than erroring, so a skill using Claude Code fields appears to work everywhere while behaving differently on each. Validate by packaging against the six-field spec, which fails loudly (§3.2).

**Live example** — [`.agents/skills`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/tree/main/.agents) is a symlink to [`.claude/skills/`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/tree/main/.claude/skills), publishing thirteen skills to all three harnesses with zero glue. A representative body: [`lint/SKILL.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.claude/skills/lint/SKILL.md).

---

## 4. Sub-agents

**This is the dimension where the three harnesses disagree most.** Skills share a ratified format; MCP shares a protocol; hooks at least share three event names. Sub-agents share only the concept. Every mechanical property — file format, invocation trigger, tool inheritance, nesting depth, whether a plugin can even ship one — is decided differently by each harness.

| Axis | Claude Code | Antigravity | Codex | Agree? |
|---|---|---|---|:--:|
| **File format** | MD + YAML frontmatter, body = prompt | MD + YAML frontmatter, body = prompt | **TOML**, prompt in `developer_instructions` | ✗ |
| **Project path** | `.claude/agents/` | `.agents/agents/<name>/agent.md` | `.codex/agents/` | ✗ |
| **User path** | `~/.claude/agents/` | `~/.gemini/config/agents/` | `~/.codex/agents/` | ✗ |
| **Invocation** | auto-delegation by `description`; `@`-mention; `--agent` for whole session | explicit `invoke_subagent` tool call | manual prompt; auto-delegation **ChatGPT Ultra only** | ✗ |
| **Tool inheritance** | `tools` allowlist + `disallowedTools` denylist | `tools[]` allowlist, default `[]` | inherits parent chat's tools | ✗ |
| **Model selector** | `sonnet`/`opus`/`haiku`/`fable`/ID/`inherit` | `inherit`/`flash`/`pro` | `gpt-5.6-luna`/`-terra`/`gpt-5.6` | ✗ |
| **Effort control** | `effort`: low→max | — | `model_reasoning_effort`: low→`ultra` | ✗ |
| **Sandbox control** | `permissionMode`, 7 modes | `commandExecutionPolicy`: off/auto/eager/sandbox | `sandbox_mode`: read-only/workspace-write | ✗ |
| **Nesting limit** | 3, configurable | 10 | **1** — `agents.max_depth`; children cannot spawn | ✗ |
| **Concurrency limit** | 20 live / 200 per session | not documented | 6 — `agents.max_threads` | ✗ |
| **Plugin-bundleable** | ✅ | ✅ | ❌ | ✗ |
| **Required fields** | `name`, `description` | `name`, `description` | `name`, `description`, `developer_instructions` | ~ |
| **Fresh context window** | ✅ | ✅ | ✅ | ✅ |
| **Skill preloading** | `skills` | `skills`/`plugins` | `skills.config` | ✅ |
| **MCP scoping** | `mcpServers` | `mcpServers[]` | `mcp_servers` | ✅ |

Sources: [CC Subagents](https://code.claude.com/docs/en/sub-agents) · [AG Subagents](https://antigravity.google/docs/subagents) · [AG `/agents`](https://antigravity.google/docs/cli/commands/agents) · [Codex Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents)

### 4.1 Which disagreements matter

**Format divergence is cheap.** TOML vs. MD+YAML is an encoding difference with identical semantics — name, description, system prompt, optional overrides. Generate three files from one source, or keep one canonical body and make each per-harness file a pointer to it. §9.2 measures the pointer approach at 3–10% overhead with drift structurally eliminated.

**Invocation divergence is not.** Claude Code delegates automatically from `description` and backgrounds sub-agents by default. Antigravity requires an explicit `invoke_subagent` call. Codex requires the user to ask — *"Direct instructions like 'spawn two agents'"* — with proactive delegation gated to ChatGPT Ultra. **Any orchestration depending on the model choosing to delegate is not portable**; portable orchestration names the agent explicitly, from the prompt or an instruction file.

**Tool-surface divergence is invisible.** Claude Code documents two filters that narrow a sub-agent's inherited tools, one unconditional and one applying to background sub-agents ([Subagents](https://code.claude.com/docs/en/sub-agents)). Neither competitor documents an equivalent, so the effective tool surface on Antigravity and Codex cannot be predicted from the definition file.

### 4.2 Capabilities with no counterpart

Claude Code-only ([Subagents](https://code.claude.com/docs/en/sub-agents)): `isolation: worktree`, a temporary git worktree per sub-agent, enforced against Bash commands redirecting git into the main checkout; `memory: user|project|local`, a directory persisting across conversations; `hooks` in frontmatter, torn down on completion; and **output scanning**, which escapes text in a sub-agent's report imitating `<system-reminder>` tags or `Human:`/`Assistant:` lines — a prompt-injection mitigation at the delegation boundary that neither competitor documents.

Antigravity-only: `mainAgent` and `subagent` booleans controlling whether a definition may serve as primary agent, callee, or both. Codex-only: `model_reasoning_effort: ultra`.

Antigravity also documents a live defect — *"Known issue: Misspelled tool names may cause hangs; schema validation pending"* ([Subagents](https://antigravity.google/docs/subagents)) — where Claude Code instead refuses to launch and names the bad entries.

**Codex is the most constrained of the three**, and the constraints compound. Collected from [Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents):

- **No per-agent tool restriction.** *"Subagents use the tools available to the parent chat."* A custom agent may override `sandbox_mode`, but not the tool list — so a read-only reviewer can be sandboxed, never tool-restricted. Claude Code has `tools`/`disallowedTools` and Antigravity has `tools[]`; Codex has no equivalent, which makes least-privilege delegation unavailable.
- **Nesting is off by default.** `agents.max_depth` defaults to `1`: the primary spawns, spawned agents cannot. Raising it is discouraged — broad delegation instructions turn into repeated fan-out, multiplying tokens, latency, and local resource use. Compare Claude Code's default 3 and Antigravity's 10.
- **Six concurrent threads** by default (`agents.max_threads`), against Claude Code's 20 live / 200 per session.
- **Auto-delegation is paywalled.** Proactive delegation without an explicit request is ChatGPT Ultra only; everywhere else the user or an `AGENTS.md`/skill instruction must ask. ChatGPT Work additionally *"exposes subagent workflows and activity to eligible accounts."*
- **Not bundleable in plugins** (§7.1) — a plugin can ship a skill that instructs delegation, never the agent it delegates to.
- **Strictly more expensive**, stated twice in the docs: *"subagent workflows consume more tokens than comparable single-agent runs because each subagent does its own model and tool work."*
- **Approval UX leaks across threads** — *"approval requests can surface from inactive agent threads even while you are looking at the main thread"* — and in non-interactive runs (`codex exec`, batch) an action needing approval fails and surfaces the error to the parent, so unattended delegation dies on the first prompt.

Net: Codex sub-agents are a parallelism mechanism, not an isolation or least-privilege mechanism. Depth 1, no tool restriction, and no plugin distribution mean the pattern they support well is one primary fanning out to a flat set of workers that inherit its capabilities.

### 4.3 Compatibility layer

This is the dimension that needs the most layer and gets the best return on it. **Rule: one canonical body, one pointer adapter per harness.**

The alternative — generating three full definitions from a source of truth — also works, but requires a build step and re-runs on every edit. Pointers need neither: the adapter is written once and never changes when the body does.

An adapter does exactly three jobs, and should do nothing else:

1. **Declare the harness's native fields.** YAML frontmatter for Claude Code and Antigravity, TOML keys for Codex. This is where per-harness tool allowlists, model tiers, and sandbox modes live, because they have no common vocabulary.
2. **Point at the canonical body** — *"Read `<path>` in full and follow it as the canonical workflow."*
3. **Supply a tool-name mapping** — `Bash` → `run_command`, `Read` → `view_file`, and so on, so the canonical body can be written in one dialect.

Three further rules follow from §4.1:

- **Dispatch by name, never by inference.** Auto-delegation is default on Claude Code, tool-gated on Antigravity, and Ultra-only on Codex, so any workflow relying on the model choosing to delegate silently degrades to inline execution on Codex.
- **Declare the fallback for missing adapters.** Coverage will be partial; say in the instruction file what to do when an agent has no adapter on this harness.
- **Degrade, never emulate.** If delegation is unavailable, the caller must record the result as missing rather than producing it inline. An agent that writes its own verifier's output has defeated the isolation the sub-agent existed to provide.

**Live example** — canonical body [`.claude/agents/profile-analyzer.md`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.claude/agents/profile-analyzer.md) (~24 KB) with its Codex adapter [`.codex/agents/profile-analyzer.toml`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.codex/agents/profile-analyzer.toml) (~1 KB); same pattern for [`gke-cluster-runner`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.codex/agents/gke-cluster-runner.toml). Note the public template ships **no Antigravity adapters at all** — three of its five agents have no adapter on any harness but Claude Code, which is exactly the partial-coverage case the fallback rule exists for. Overheads measured in §9.2.

---

## 5. MCP

MCP is the layer everyone calls standard. The **protocol** is shared; the **configuration schema** is not — the three disagree on file name, file format, and field names, including the name of the remote-URL field.

| | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Workspace config** | `.mcp.json` | `.agents/mcp_config.json` | `.codex/config.toml` (trusted projects only) |
| **User config** | `~/.claude.json` | `~/.gemini/config/mcp_config.json` | `~/.codex/config.toml` |
| **Format** | JSON, root key `mcpServers` | JSON, root key `mcpServers` | TOML, `[mcp_servers.<name>]` |
| **Scopes** | `local` (default), `project`, `user` | workspace, global | workspace, user |
| **stdio fields** | `command`, `args`, `env` | `command`, `args`, `env`, `cwd` | `command`, `args`, `env`, `env_vars`, `cwd` |
| **Remote URL field** | `url` (+ required `type`) | **`serverUrl`** | `url` |
| **Transports** | `stdio`, `http`, `sse`, `ws` | stdio, Streamable HTTP, SSE | stdio, Streamable HTTP |
| **Auth** | `headers`, `headersHelper`, OAuth via `/mcp` | `authProviderType`, `oauth.{clientId, clientSecret}` | `auth` (`oauth`\|`chatgpt`), `bearer_token_env_var`, `http_headers` |
| **Disable without deleting** | `disabledMcpServers` setting | `disabled: true` | `enabled = false` |
| **Per-server tool filter** | permission rules | `disabledTools[]` | `enabled_tools`, `disabled_tools` |
| **Timeouts** | `timeout` ms per server | not documented | `startup_timeout_sec` (10), `tool_timeout_sec` (60) |
| **CLI** | `claude mcp add/add-json/list/get` | `/mcp` overlay | `codex mcp add/list/login` |
| **Approval default** | project `.mcp.json` needs approval + workspace trust | Ask mode; `mcp(server/tool)` patterns | `default_tools_approval_mode`: `auto`\|`prompt`\|`writes`\|`approve` |

Sources: [CC MCP](https://code.claude.com/docs/en/mcp) · [AG MCP](https://antigravity.google/docs/mcp) · [Codex MCP](https://learn.chatgpt.com/docs/extend/mcp?surface=cli)

**The `url` / `serverUrl` split.** Claude Code and Codex name the remote endpoint `url`. Antigravity names it `serverUrl` and rejects the other spelling: *"Legacy fields like `url` or `httpUrl` are not supported"* ([AG MCP](https://antigravity.google/docs/mcp)). Claude Code additionally errors when `url` appears without `type` ([CC MCP](https://code.claude.com/docs/en/mcp)).

The same server therefore needs three declarations sharing no field vocabulary beyond `command`/`args`/`env` — a generator problem, not a copy problem. The schemas also differ in expressive power: Codex can express per-server timeouts, the Antigravity schema has no timeout fields at all.

Claude Code namespaces MCP tools as `mcp__<server>__<tool>`, the form hook matchers and permission rules target; Antigravity expresses the same targeting as `mcp(server/tool)` permission patterns; Codex uses per-server `enabled_tools`/`disabled_tools`. Sub-agent-scoped MCP exists in all three (§4) and is the recommended way to keep a server's tool schemas out of the parent context.

### 5.1 Compatibility layer

**Rule: generate all three declarations from one source. This one cannot be a symlink or a pointer.** The files are different formats (JSON, JSON, TOML) at different paths with different field names, and no harness reads another's.

A minimal source record carries what all three can express — server name, transport, `command`/`args`/`env` for stdio, endpoint URL for remote — and the emitter renames per target: `url` for Claude Code and Codex, `serverUrl` for Antigravity, plus Claude Code's mandatory `type`.

Three things do not round-trip, and the layer should fail loudly rather than silently drop them:

- **Disable state.** Codex has `enabled = false`, Antigravity has `disabled: true`, Claude Code uses a separate `disabledMcpServers` setting. A server disabled in one declaration stays live in the others unless the emitter handles all three.
- **Timeouts.** Codex has `startup_timeout_sec` and `tool_timeout_sec`; Claude Code has a per-server `timeout` in milliseconds; Antigravity documents none. Timeout tuning is not portable.
- **Auth.** Three unrelated schemes — `headersHelper`, `authProviderType`/`oauth`, `bearer_token_env_var`/`env_http_headers`. Credentials belong in the environment, referenced per-harness, not in the shared source.

**Live example, and a counter-example.** The template declares one server twice by hand — [`.agents/mcp_config.json`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.agents/mcp_config.json) using `serverUrl`, and [`.codex/config.toml`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.codex/config.toml) using `url` — with no Claude Code declaration at all. The two have already drifted between the public and private forks — `enabled` is `true` in one and `false` in the other, and the Antigravity declaration has no field able to express the difference. This is the dimension where the repo does *not* implement the rule, and the failure mode is exactly the predicted one.

---

## 6. Hooks

| | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Event count** | 31 | 5 | 11 |
| **Handler types** | `command`, `http`, `mcp_tool`, `prompt`, `agent` | `command` | `command` (`prompt`/`agent` *"parsed but skipped"*) |
| **Config location** | `settings.json` × 4 scopes; plugin `hooks/hooks.json`; **skill & agent frontmatter** | `hooks.json` in `.agents/` or `~/.gemini/config/` | `~/.codex/hooks.json` or `config.toml`; repo `.codex/`; plugin |
| **Config format** | JSON | JSON | JSON or TOML `[[hooks.EventName]]` |
| **Matchers** | exact / list / unanchored regex, per-event target | regex on tool name, PreToolUse+PostToolUse only | regex on `tool_name`/`source`/`trigger` |
| **Exit codes** | 0 ok · 1 non-blocking · **2 blocking**, stderr → model | not documented; JSON `decision` instead | 0 ok · 2 failure, stderr as reason |
| **Default timeout** | 600 s | **30 s** | 600 s; `SessionEnd` 1 s |
| **Mutate tool input / output** | `updatedInput` / `updatedToolOutput` | not documented | `updatedInput` / `decision: "block"` |
| **Org lockdown** | `allowManagedHooksOnly`, `disableAllHooks` | not documented | `allow_managed_hooks_only` |

Sources: [CC Hooks](https://code.claude.com/docs/en/hooks) · [AG Hooks](https://antigravity.google/docs/hooks) · [Codex Hooks](https://learn.chatgpt.com/docs/hooks)

### 6.1 Event coverage

| Event | CC | AG | Codex |
|---|:--:|:--:|:--:|
| `PreToolUse`, `PostToolUse`, `Stop` | ✅ | ✅ | ✅ |
| `SessionStart`, `SessionEnd`, `UserPromptSubmit` | ✅ | — | ✅ |
| `PermissionRequest`, `PreCompact`, `PostCompact` | ✅ | — | ✅ |
| `SubagentStart`, `SubagentStop` | ✅ | — | ✅ |
| `PreInvocation`, `PostInvocation` | — | ✅ | — |
| 20 further events (compaction, task, file-watch, worktree, elicitation, …) | ✅ | — | — |

Three-way overlap is exactly `PreToolUse`, `PostToolUse`, `Stop`. Claude Code ↔ Codex overlap is eleven.

### 6.2 Codex reimplements the Claude Code contract

Field for field ([Codex Hooks](https://learn.chatgpt.com/docs/hooks) vs [CC Hooks](https://code.claude.com/docs/en/hooks)): same event names; same stdin envelope (`session_id`, `transcript_path`, `cwd`, `hook_event_name`, `permission_mode`); same exit-code semantics; same output fields (`continue`, `stopReason`, `systemMessage`, `decision`, `hookSpecificOutput.additionalContext`); same `PreToolUse` control shape (`permissionDecision: "deny"` + reason, or `"allow"` + `updatedInput`); same regex matchers.

A `command` handler written against the Claude Code contract typically runs unmodified under Codex; only the registration file differs. Codex constraints: only `command` handlers execute, and `PreToolUse`/`PostToolUse` *"don't observe hosted tools (e.g., WebSearch)."*

### 6.3 Antigravity is a different design

Not a subset ([AG Hooks](https://antigravity.google/docs/hooks)). `PreInvocation`/`PostInvocation` fire around each **model call** rather than each tool call, with `injectSteps` and `terminationBehavior` (`"force_continue"` | `"terminate"`) — no analogue in either competitor. `PreToolUse` returns five decisions (`allow`, `deny`, `ask`, `force_ask`, `deny_unless_prior_grant`) against Claude Code's four and Codex's three. Absent: session and compaction events, sub-agent events, non-`command` handlers, a documented exit-code protocol, org lockdown. The 30 s default timeout is 20× tighter than the other two.

Claude Code alone treats hooks as components: five handler types rather than one, and hooks declarable in skill and agent frontmatter so they ship and tear down with the component whose lifetime they govern ([CC Hooks](https://code.claude.com/docs/en/hooks)).

### 6.4 Compatibility layer

**Rule: portable hooks are possible only inside the intersection. Outside it, don't port — re-express.**

For a hook on `PreToolUse`, `PostToolUse`, or `Stop`:

1. Write the handler as a standalone executable that reads the JSON envelope on stdin and writes control JSON on stdout. Use only the shared fields — `session_id`, `cwd`, `hook_event_name`, `tool_name`, `tool_input` — and ignore harness extras.
2. Signal decisions through JSON, not exit codes. Claude Code and Codex both define exit 2 as blocking; Antigravity documents no exit-code protocol at all and expects a `decision` field.
3. Register it per harness. This is the only file that varies: `settings.json` for Claude Code, `.agents/hooks.json` for Antigravity, `.codex/hooks.json` or `config.toml` for Codex.
4. Budget to 30 seconds — Antigravity's default, 20× tighter than the other two. A handler that shells out to a linter or test run will not fit.

Everything outside those three events is a different decision. Rather than emulating a missing event, re-express the *service* the hook provided using whatever each harness has natively — a scheduler, a background task, a sub-agent. That trade is worth taking earlier than it looks: a session-lifecycle or sub-agent-lifecycle hook covers two of three harnesses at best, and the Claude Code-only two-thirds of the event surface covers one.

**Live example, and its retirement.** [`.codex/hooks.json`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.codex/hooks.json) registers a single `Stop` hook — `type: "command"`, `timeout: 30` — running [`.codex/hooks/stop_hook.sh`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki/blob/main/.codex/hooks/stop_hook.sh). It sits squarely inside the intersection: shared event, shared handler type, weakest-link timeout. The private fork nonetheless deleted it and re-expressed the same service on each harness's native scheduler, on the grounds that *"The Stop hook was Claude-only and opt-in; the watcher is harness-native, unconditional, and additionally revives dead-idle sessions, which the hook never could."* Even a hook inside the intersection covered one harness in practice.

---

## 7. Plugins

| | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Manifest** | `.claude-plugin/plugin.json` — **optional** | `plugin.json` at root | `.codex-plugin/plugin.json` — **required** |
| **Required fields** | `name`, if a manifest exists | none (`name` defaults to dir) | `name`, `version`, `description` |
| **Skills** | ✅ | ✅ | ✅ |
| **Sub-agents** | ✅ | ✅ | ❌ |
| **Hooks** | ✅ | ✅ | ✅ |
| **MCP** | ✅ | ✅ | ✅ |
| **Rules** | — | ✅ | — |
| **Connectors** | — | — | ✅ `.app.json` |
| **LSP / monitors / `bin/` / settings** | ✅ all four | — | — |
| **Marketplace** | ✅ two public catalogs | ❌ none documented | ✅ universal directory shared with ChatGPT |
| **Namespacing** | `/plugin-name:skill-name` | namespaced bundles | not documented |
| **Local dev** | `--plugin-dir`, `/reload-plugins`, `claude plugin validate` | `agy plugin install <path>` | local marketplace |

Sources: [CC Plugins](https://code.claude.com/docs/en/plugins) · [CC Plugins reference](https://code.claude.com/docs/en/plugins-reference) · [AG Plugins](https://antigravity.google/docs/plugins) · [AG CLI Plugins](https://antigravity.google/docs/cli/plugins) · [Codex Build plugins](https://learn.chatgpt.com/docs/build-plugins)

**Claude Code** — widest bundle, optional manifest. Unrecognized manifest fields are ignored deliberately, so *"one manifest that doubles as a VS Code or Cursor extension manifest, an npm `package.json`, or an MCPB/DXT bundle manifest"* is supported ([Plugins reference](https://code.claude.com/docs/en/plugins-reference)). Plugin sub-agents are stripped of `hooks`, `mcpServers`, and `permissionMode` — *"For security reasons"* — so an installed plugin cannot silently attach hooks via an agent definition.

**Codex** — strongest distribution: storefront metadata, marketplace `policy` fields (`installation`, `authentication`), three source types (`local`, `git-subdir`, `npm`), a directory shared with ChatGPT. It reads Claude Code's marketplace path as legacy — *"Legacy: `$REPO_ROOT/.claude-plugin/marketplace.json`"* ([Build plugins](https://learn.chatgpt.com/docs/build-plugins)).

**Antigravity** — thinnest bundle; `plugin.json` is a marker file whose only field is optional. Managed with `agy plugin install|disable|enable|uninstall` ([CLI Plugins](https://antigravity.google/docs/cli/plugins)). The only harness whose plugins ship **rules**.

### 7.1 Two claims worth checking

Both were verified against first-party docs, because both are load-bearing for §8.

**Codex plugins cannot bundle sub-agents — confirmed.** The [plugin build spec](https://learn.chatgpt.com/docs/build-plugins) enumerates the directory layout as `.codex-plugin/plugin.json`, `skills/`, `.mcp.json`, `.app.json`, `hooks/`, `assets/`, and the manifest's component pointers as `skills`, `mcpServers`, `apps`, `hooks`. There is no `agents/` directory, no `agents` manifest key, and no reference to custom-agent `.toml` files anywhere in the layout — while Codex sub-agents themselves live in `~/.codex/agents/` or `.codex/agents/` ([Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents)), paths a plugin does not write to. **Consequence: a Codex plugin can ship a skill that instructs delegation, but never the specialist agent it delegates to.** Note the page's own summary sentence is narrower still — *"A plugin is an installable package that can include skills, an MCP server, or both"* — omitting hooks, which the [hooks reference](https://learn.chatgpt.com/docs/hooks) independently confirms are plugin-bundleable via `hooks/hooks.json` and gated behind a trust prompt.

**Antigravity has no marketplace — confirmed.** [Plugins](https://antigravity.google/docs/plugins) documents exactly two install paths: browsing Google's bundled plugins from the Customizations page, and manual folder placement in `.agents/plugins/`, `_agents/plugins/`, or `~/.gemini/config/plugins/`, after which *"Antigravity automatically scans these directories to discover and load your customizations."* There is no registry file, no catalog, and no `agy plugin marketplace` subcommand — the [CLI](https://antigravity.google/docs/cli/plugins) exposes only `list`, `install <path>`, `disable`, `enable`, `uninstall`, all local-path operations. Third parties have filled the gap ([`agy-plugins-cli`](https://github.com/ZaunEkko/agy-plugins-cli) adds GitHub-backed marketplaces and batch install), which is evidence of demand, not of vendor support.

### 7.2 Compatibility layer

**Rule: if you need all three harnesses, distribute the repository, not a plugin.** This is the one dimension where the honest answer is to skip the mechanism.

The bundles are not equivalent, and the gaps are structural rather than cosmetic. A plugin that ships a specialist sub-agent works on Claude Code and Antigravity and cannot exist on Codex (§7.1). A plugin that ships rules works only on Antigravity. And even a bundle restricted to the common four components has nowhere to go on Antigravity, which has no registry to publish to.

If you do bundle:

1. **One physical directory, three manifests.** Claude Code ignores unrecognized top-level manifest keys deliberately, so `.claude-plugin/plugin.json` can carry the other vendors' fields; Codex requires its own `.codex-plugin/plugin.json`, and Antigravity a root `plugin.json`.
2. **Restrict the bundle to skills, hooks, and MCP** — the three components all three harnesses accept. Ship sub-agents through the repo layout instead, where all three can reach them.
3. **Expect namespacing to differ.** Claude Code prefixes plugin skills as `/plugin-name:skill-name`; the others don't document a scheme, so a bare skill name that is unique in one install may collide in another.

Distributing as a git template sidesteps all of it: the layout in §9 is reachable by every harness on clone, needs no install step, no manifest, and no registry — at the cost of updates being a `git pull` rather than a version bump.

**Live example** — the template ships **no plugin manifest of any kind**. [`tpu_performance_autoresearch_wiki`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki) is consumed by forking it, and every harness picks up the skills, agents, hooks, and MCP config from their native paths directly. That is the recommendation implemented.

---

## 8. Portability

### 8.1 Tiers

**Tier 1 — moves unmodified.** Skill body; skill `name` + `description`; bundled skill files; the `.agents/skills/` workspace root (Antigravity + Codex directly, Claude Code via symlink).

**Tier 2 — needs a generator or a pointer.**

| Construct | Work required |
|---|---|
| Sub-agent definition | Four semantic fields, three encodings, three paths → three emitters, or three pointers to one body (§9.2) |
| Hooks on the shared 3 events | CC ↔ Codex: registration file only. → AG: rewrite `decision` values, drop exit-code-2, fit 30 s |
| Hooks on the shared 11 | CC ↔ Codex only: registration file only |
| MCP server declaration | Three schemas, three formats, `url` vs `serverUrl` (§5) |
| Plugin bundle | Same four core components, three manifests; CC's ignore-unknown-fields rule lets one file carry all three vendors' keys |

**Tier 3 — no target; re-express in the body or drop.**

| Harness | Construct | Substitute |
|---|---|---|
| Claude Code | `context: fork` + `agent` | Separate sub-agent definition + a skill instructing invocation |
| Claude Code | `` !`cmd` `` injection | Pre-render in a build step, or make it step 1 of the body |
| Claude Code | `allowed-tools` / `disallowed-tools` | Prose constraint + a `PreToolUse` hook |
| Claude Code | `memory`, `isolation: worktree`, `paths`, `effort`, per-skill `model`, frontmatter `hooks` | None |
| Claude Code | 20 of 31 hook events; `http`/`mcp_tool`/`prompt`/`agent` handlers; LSP; monitors; `bin/` | None |
| Antigravity | `PreInvocation`/`PostInvocation`, `injectSteps`, `terminationBehavior` | None |
| Antigravity | `commandExecutionPolicy`, `mainAgent`/`subagent` | Approximate with `permissionMode` / `sandbox_mode` |
| Codex | `model_reasoning_effort: ultra`, `openai.yaml` interface block, `.app.json` connectors | None |

### 8.2 Rules

1. Hold skill frontmatter at the spec's six fields; put everything else in the body. Bodies are fully portable, frontmatter is not.
2. Use Codex's sidecar shape — spec-pure `SKILL.md`, one vendor-namespaced sidecar per target.
3. Map `.agents/skills/` and `.claude/skills/` to one tree with a symlink.
4. Generate sub-agent definitions; do not hand-maintain three.
5. Write hook handlers as standalone executables over the shared JSON envelope. Three events for three-way portability, eleven for CC + Codex. Only the registration file varies.
6. Delegate to sub-agents explicitly. Auto-delegation is default on CC, tool-gated on AG, Ultra-only on Codex.
7. Budget to the weakest link: 30 s hook timeout, 8,000-char skill-listing budget.
8. Declare MCP servers from one source. No two schemas agree, including on `url`.

### 8.3 Scorecard

| Dimension | Claude Code | Antigravity | Codex |
|---|---|---|---|
| **Skills** | ★★★★★ standard + ~22 fields, invocation control, dynamic injection, forking | ★★★☆☆ clean standard implementation only | ★★★★☆ standard + factored sidecar |
| **Sub-agents** | ★★★★★ deepest fields, memory, worktree isolation, documented limits, output scanning | ★★★☆☆ solid fields, 10-level nesting; hang bug, no isolation or memory | ★★★☆☆ clean model/sandbox story; TOML outlier, not bundleable |
| **Hooks** | ★★★★★ 31 events, 5 handler types, component-scoped | ★★☆☆☆ 5 events, command-only; unique per-invocation control | ★★★★☆ 11 events, reimplements the CC contract |
| **MCP** | ★★★★☆ 4 transports, scoped, namespaced tools | ★★★☆☆ full auth story; no timeouts, non-standard `serverUrl` | ★★★★☆ richest per-server controls |
| **Plugins** | ★★★★★ widest components, two marketplaces, dev tooling | ★★☆☆☆ simplest bundle, ships rules, no distribution | ★★★★☆ commercial directory; no sub-agents |

Claude Code set the vocabulary: Codex reimplemented its hook contract and reads its marketplace path as legacy; both others adopted its skill format via the open standard. Codex is closest to parity and the cheapest translation target. Antigravity is thinnest on hooks and distribution and owns two originals — bundled rules and per-model-invocation hooks. A three-way layer is viable if designed around the intersection.

---

## 9. Worked example

Measured from two repos running one autoresearch workflow under all three harnesses: public template [`tpu_performance_autoresearch_wiki`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki) and private fork [`…_private`](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki_private).

```
├── SCHEMA.md          ← canonical protocol, ~600 lines
├── CLAUDE.md  GEMINI.md  AGENTS.md    ← three entry points
├── .claude/
│   ├── skills/        ← canonical skill bodies (13 public / 15 private)
│   ├── agents/        ← canonical agent bodies (5)
│   └── scripts/       ← shared executables, referenced by path from all three
├── .agents/
│   ├── skills -> ../.claude/skills    ← symlink
│   ├── agents/<name>/agent.md         ← Antigravity adapters (private only)
│   └── mcp_config.json
└── .codex/
    ├── agents/<name>.toml   config.toml
    └── hooks.json + hooks/  ← public only; retired in the private fork (§6.4)
```

### 9.1 One protocol, three entry points

| File | Read by | Mechanism | Content |
|---|---|---|---|
| `CLAUDE.md` | Claude Code | `@SCHEMA.md` import | one line |
| `GEMINI.md` | Antigravity | `@SCHEMA.md` import + emulation layer | import, then Claude→Antigravity primitive mapping |
| `AGENTS.md` | Codex, Antigravity | prose pointer | *"The canonical cross-agent protocol is `SCHEMA.md`; read it…"* + translation notes |

Triplicated, `SCHEMA.md` would be ~1,800 lines across three files. Root-file size is inversely proportional to native support for the canonical layout: `CLAUDE.md` is one line because the repo is authored in Claude Code's dialect; `GEMINI.md` is largest because Antigravity has neither auto-discovered agents at the canonical path nor identically-wired slash-command skills, so it enumerates all fifteen skills by path and maps each Claude primitive to an Antigravity native (`Task` → `invoke_subagent`, `ScheduleWakeup` → `schedule`).

`AGENTS.md` states the rule governing the whole layer:

> When a shared skill mentions Claude `/loop`, `ScheduleWakeup`, `Task`, `TaskStop`, or background subagent notifications, translate that step to the available Codex subagent, hook, or automation mechanism. **Do not pretend the Claude primitive exists.**

### 9.2 Pointer adapters, not copies

One canonical body per agent; each harness gets a pointer. Measured (private repo):

| Agent | `.claude/agents/*.md` | `.agents/agents/*/agent.md` | `.codex/agents/*.toml` | Overhead |
|---|--:|--:|--:|--:|
| `profile-analyzer` | 23,868 B | 734 B | 1,103 B | 7.7% |
| `kernel-verifier` | 21,353 B | 812 B | 1,674 B | 11.6% |
| `process-auditor` | 12,719 B | 850 B | 2,285 B | 24.6% |

The full Antigravity adapter, 734 bytes:

```yaml
---
name: profile-analyzer
description: Analyzes a completed experiment's xprof trace + HLO dump via the
  xprof-cli CLI (XPROF_MODE=local, serverless) and returns structured Profile /
  HLO Dump sections including the Phase 3 hypothesis-firing audit. Never assigns
  verdicts.
tools: [run_command, view_file, grep_search, find_by_name, list_dir]
---
Read `.claude/agents/profile-analyzer.md` in full and follow it as the canonical
workflow. Tool mapping: Bash means run_command (all xprof reads go through the
xprof-cli CLI with XPROF_MODE=local); Read means view_file. Run everything
synchronously in the foreground. Your final message IS the analysis.
```

Codex's is the same construction in TOML, pointer inside `developer_instructions`. Each adapter declares native fields, points at the canonical body, and supplies a tool-name mapping. Three ~1 KB pointers replace three 20 KB copies; drift is structurally impossible because one body exists.

Skills need no adapter at all: `.agents/skills -> ../.claude/skills` reaches all three harnesses with zero glue files. The contrast is the Tier-1/Tier-2 boundary made concrete — sub-agents need an adapter each because encodings differ, skills need none because the standard makes `SKILL.md` directly executable everywhere.

## 10. References

Codex doc URLs `308`-redirect from `developers.openai.com/codex/*` to `learn.chatgpt.com/docs/*` (verified 2026-08-06).

| Topic | URL |
|---|---|
| Agent Skills open standard | https://agentskills.io/ |
| Agentic AI Foundation (Linux Foundation) | https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation |
| CC — Skills | https://code.claude.com/docs/en/skills |
| CC — Sub-agents | https://code.claude.com/docs/en/sub-agents |
| CC — Hooks | https://code.claude.com/docs/en/hooks |
| CC — MCP | https://code.claude.com/docs/en/mcp |
| CC — Memory / instruction files | https://code.claude.com/docs/en/memory |
| CC — Plugins | https://code.claude.com/docs/en/plugins |
| CC — Plugins reference | https://code.claude.com/docs/en/plugins-reference |
| AG — Skills | https://antigravity.google/docs/skills |
| AG — Sub-agents | https://antigravity.google/docs/subagents |
| AG — Hooks | https://antigravity.google/docs/hooks |
| AG — MCP | https://antigravity.google/docs/mcp |
| AG — Rules & Workflows | https://antigravity.google/docs/rules-workflows |
| AG — Plugins (IDE) | https://antigravity.google/docs/plugins |
| AG — CLI Plugins & Skills | https://antigravity.google/docs/cli/plugins |
| AG — CLI `/agents` | https://antigravity.google/docs/cli/commands/agents |
| AG — CLI best practices | https://antigravity.google/docs/cli/best-practices |
| AG — Gemini CLI migration | https://antigravity.google/docs/cli/gcli-migration |
| Codex — Skills | https://learn.chatgpt.com/docs/build-skills |
| Codex — Sub-agents | https://learn.chatgpt.com/docs/agent-configuration/subagents |
| Codex — Hooks | https://learn.chatgpt.com/docs/hooks |
| Codex — MCP | https://learn.chatgpt.com/docs/extend/mcp?surface=cli |
| Codex — Build plugins | https://learn.chatgpt.com/docs/build-plugins |

**§9 sources (measured):** `.claude/agents/*.md`, `.agents/agents/<name>/agent.md`, `.codex/agents/<name>.toml`, `.agents/skills` symlink, `CLAUDE.md`/`GEMINI.md`/`AGENTS.md`, `.codex/hooks.json` (public only), `SCHEMA.md` § "Launch-armed process watcher".

**Not first-party:** Antigravity IDE `AGENTS.md` support version ([v1.20.3](https://discuss.ai.google.dev/t/antigravity-update-1-20-3-2026-3-5/129320) — forum, not changelog); Antigravity plugin `agents/` subdirectory (in [CLI docs](https://antigravity.google/docs/cli/plugins) only, absent from the [IDE Plugins page](https://antigravity.google/docs/plugins)); Codex plugin-directory size and publishing status.
