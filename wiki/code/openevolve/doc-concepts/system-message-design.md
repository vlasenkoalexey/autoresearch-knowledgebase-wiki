---
title: System message design — the primary lever for steering evolution
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# System message design — the primary lever for steering evolution

## Definition

The README devotes one of its largest sections ("Crafting Effective System Messages") to the claim that
the configured system message is "arguably the most important component for evolution success" — more
consequential to a run's outcome than any numeric hyperparameter. It documents a four-phase iterative
process for writing one (initial draft → refinement from observed failures → specialization with
examples → optimization, even proposing using OpenEvolve to evolve its own system message), and gives
worked examples ranging from a one-line role description up to a detailed hardware-optimization brief
with explicit `MUST NOT CHANGE` / `ALLOWED` constraint lists.

## In openevolve (grounded)

The system message a user writes in `prompt.system_message` is not always used verbatim as literal text.
[`PromptConfig.system_message`](../catalog/openevolve/config.md#PromptConfig) defaults to the *string*
`"system_message"` — not a sentence, but the **name of a template key** — and
[`PromptSampler.build_prompt`](../catalog/openevolve/prompt/sampler.md#PromptSampler.build_prompt)
resolves it with a dual-mode check: if `self.config.system_message` matches a key already registered in
[`TemplateManager.templates`](../catalog/openevolve/prompt/templates.md#TemplateManager.templates), it
is looked up and expanded via
[`get_template`](../catalog/openevolve/prompt/templates.md#TemplateManager.get_template); otherwise the
config value is treated as literal text and used as-is. This is exactly why the README's inline YAML
examples (`system_message: |` followed by several sentences of prose) work unmodified — a user's literal
prose simply fails the "is this a known template key" check and passes through untouched — while a
deployment that never sets `system_message` at all falls back to the shipped default template.

When `system_message_changes_description` is also configured (relevant when
[`programs_as_changes_description`](../catalog/openevolve/config.md#PromptConfig) is enabled, see
[`openevolve-prompt-sampler.md`](../concepts/openevolve-prompt-sampler.md)), `build_prompt` wraps the
resolved system message a second time through the
`system_message_with_changes_description` template, splicing in a second sub-message that instructs the
model to keep the program's natural-language change description in sync with its code — one more layer
between what a user configures and what the LLM ultimately reads.

## Why it matters / when it applies

The README's constraint-list pattern (`MUST NOT CHANGE: kernel function signature ... ALLOWED: memory
access patterns ...`) is prose-level reinforcement of the same "what can this mutation touch" boundary
that [EVOLVE-BLOCK markers](evolve-block-markers.md) enforce structurally. The two are complementary,
not redundant: the marker is a hard, parsed boundary (code outside it is never shown to the diff
mechanism as evolvable), while the system message is a soft, LLM-obeyed boundary over what happens
*inside* the marked region (e.g. "don't change this function's signature" even though the whole function
body is technically inside an EVOLVE-BLOCK). The README's advice to iterate the system message based on
observed failures maps directly onto the [artifacts feedback loop](artifacts-feedback-loop.md): a system
message refined in response to "where the system gets stuck" is, in practice, a response to exactly the
stderr/error artifacts that mechanism surfaces back into later prompts.

## Connections

- Code concepts: [Prompt sampler — assembling what the LLM mutation operator sees](../concepts/openevolve-prompt-sampler.md)
  — the caller that resolves `system_message` at prompt-build time;
  [Prompt templates and fragments](../concepts/openevolve-prompt-templates.md) — the registry
  `system_message` may resolve against; [Config](../concepts/openevolve-config.md) — where
  `PromptConfig.system_message` lives.
- Module catalogs: [openevolve/prompt/sampler.py](../catalog/openevolve/prompt/sampler.md),
  [openevolve/prompt/templates.py](../catalog/openevolve/prompt/templates.md),
  [openevolve/config.py](../catalog/openevolve/config.md).
- Related doc-concepts: [EVOLVE-BLOCK markers](evolve-block-markers.md) — the structural counterpart to
  this prose-level boundary; [Artifacts feedback loop](artifacts-feedback-loop.md) — the mechanism the
  README's iterative system-message-refinement process is actually responding to.

## Source

Extracted from `README.md` (kept in place), "Crafting Effective System Messages" section.
