---
title: "T(...).r(...) — the prompt-templating layer every reasoning-pipeline stage renders through"
type: concept
provenance: mixed
concept: rdagent-utils-agent-tpl
updated: 2026-07-04
status: fresh
---
# T(...).r(...) — the prompt-templating layer every reasoning-pipeline stage renders through

## Overview
`T` (a shortcut for the `RDAT` class) is how every Research/Development component in this codebase turns
"I need a prompt" into actual message text: `T(".prompts:hypothesis_gen.system").r(pipeline=..., ...)`
loads a YAML-addressed template and renders it through Jinja2 with strict, fail-loud variable checking.
This is the layer directly underneath the six-component Research→Development split this repo implements —
`hypothesis_gen`, `task_gen`, every coder's `evaluate`, `generate_feedback` — none of them build prompt
strings by hand; they all render through this one mechanism before handing the result to
[`APIBackend().build_messages_and_create_chat_completion`](rdagent-oai-backend-base.md). The one idea
worth remembering: template resolution and Jinja's `{% include %}` mechanism share the *same* URI-lookup
function, so prompt fragments compose recursively without any separate include-path configuration.

## Diagram
```mermaid
flowchart TD
    call["T(uri).r(**context)<br/>(hypothesis_gen, task_gen, evaluate, ...)"]
    call --> init["RDAT.__init__(uri)"]
    init --> lc1["load_content(uri, caller_dir)"]
    lc1 --> pri{"file lookup priority:<br/>app_tpl override →<br/>caller-relative →<br/>project-relative"}
    pri --> tmpl["self.template (raw yaml/text)"]
    tmpl --> render["r(**context):<br/>Jinja2 Environment(StrictUndefined,<br/>FunctionLoader(load_content))"]
    render -->|"{% include \"a.b:c\" %}"| lc2["load_content (recursive)"]
    lc2 --> render
    render --> collapse["collapse 3+ blank lines"]
    collapse --> log["log_object(uri, template,<br/>context, rendered), tag=debug_tpl"]
    log --> out["rendered prompt string"]
```

## Design rationale (why it's built this way)
- **Dotted-path + nested-key addressing, not one file per prompt.** A [`uri`](../catalog/rdagent/utils/agent/tpl.md#RDAT.uri)
  like `"scenarios.data_science.proposal.exp_gen.prompts_v2:hypothesis_gen.system"` lets one YAML file
  bundle every prompt variant a component needs — system prompt, user prompt, several output-format
  snippets — under nested keys in one place, rather than scattering many single-prompt files across the
  tree.
- **Caller-relative resolution removes a whole class of path bugs.** [`load_content`](../catalog/rdagent/utils/agent/tpl.md#load_content)
  inspects the call stack to find the calling module's own directory, so `T(".prompts:x")` written
  identically inside *any* component module always resolves to the `prompts.yaml` sitting next to that
  specific file — no component needs to spell out or maintain its own dotted package path.
- **An explicit override seam for embedding applications.** `load_content` checks `RD_AGENT_SETTINGS.app_tpl`
  first, ahead of both the caller-relative and project-relative candidates — an application built on top of
  RD-Agent can shadow any default prompt by placing a same-named file under its own `app_tpl` directory,
  without forking the library.
- **`StrictUndefined` turns a silent bug into a loud one.** [`r`](../catalog/rdagent/utils/agent/tpl.md#RDAT.r)'s
  Jinja `Environment` is built with `undefined=StrictUndefined`, so a template referencing a context
  variable the caller forgot to pass raises immediately at render time rather than silently substituting an
  empty string into a prompt that then gets sent to a real, billed LLM call — a subtle prompt-assembly bug
  becomes an immediate crash instead of a confusing wrong answer three layers downstream.
- **The same URI resolver backs both top-level load and recursive include.** `r`'s `Environment` is
  constructed with `loader=FunctionLoader(load_content)` — the *identical* function `RDAT.__init__` uses to
  load the outer template is reused by Jinja to resolve `{% include "scenarios.data_science.share:component_spec.DataLoadSpec" %}`
  directives inside it. A shared prompt fragment (say, one component's output-format spec) is written once
  and pulled into every template that needs it, using the same dotted-path syntax a caller would use to
  load it directly.
- **Collapsing repeated blank lines keeps conditionally-assembled prompts compact.** Templates like
  [`hypothesis_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen)'s
  system prompt conditionally include large optional blocks (`pipeline=`, `enable_idea_pool=`,
  `inject_diverse=`, `sibling_hypotheses=`, …); when a branch is omitted, `r` collapses the resulting
  runs of 3+ newlines down to a single blank line so the final prompt doesn't accumulate visible gaps or
  waste tokens on whitespace.

## Entry points
- [`T`](../catalog/rdagent/utils/agent/tpl.md#T) — the module-level shortcut essentially every
  prompt-producing call site in the FC pipeline uses first; reached at the top of
  [`hypothesis_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen),
  [`task_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen),
  and the coder [`evaluate`](../catalog/rdagent/scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate)
  / [`evaluate`](../catalog/rdagent/components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate)
  methods alike.
- [`r`](../catalog/rdagent/utils/agent/tpl.md#RDAT.r) — reached once `T(...)` has loaded a template, to
  render it against a context dict into the literal string handed to the LLM backend.
- [`load_content`](../catalog/rdagent/utils/agent/tpl.md#load_content) — reached both directly (loading the
  top-level template) and recursively (resolving nested `{% include %}` directives during rendering) —
  the one function that implements the whole URI-resolution scheme.

## Mechanism (step-by-step)
1. **URI parsing and file-priority resolution.** `RDAT.__init__` hands its `uri` to
   [`load_content`](../catalog/rdagent/utils/agent/tpl.md#load_content), which splits it into a path part
   and an optional yaml-key trace, then tries candidate file paths in a fixed priority order — an
   `app_tpl`-shadowed path first (if configured), then the caller-relative or project-relative default —
   returning the first that exists and (for yaml) has the requested nested key.
2. **Rendering with fail-loud semantics.** [`r`](../catalog/rdagent/utils/agent/tpl.md#RDAT.r) builds a
   Jinja2 `Environment(undefined=StrictUndefined, loader=FunctionLoader(load_content))` from the cached
   `self.template` string and renders it against the caller's keyword context — any referenced-but-missing
   variable raises rather than rendering blank.
3. **Recursive composition through the same loader.** Because that `Environment`'s loader is
   `load_content` itself, a `{% include "a.b:c" %}` directive inside any template re-enters
   [`load_content`](../catalog/rdagent/utils/agent/tpl.md#load_content) with the included URI — the same
   override-priority and yaml-key-trace logic applies recursively, so shared prompt fragments compose
   without a separate include-path mechanism.
4. **Every render is logged for later replay.** After collapsing blank-line runs, `r` calls
   [`log_object`](../catalog/rdagent/log/logger.md#RDAgentLog.log_object) via
   [`rdagent_logger`](../catalog/rdagent/log/__init__.md#rdagent_logger.rdagent_logger) with `tag="debug_tpl"`,
   capturing the uri, the raw template, the context dict, and the final rendered string as one object —
   this is the audit trail a trace UI would replay to show exactly what prompt bytes a given LLM call sent.
5. **Every reasoning-pipeline stage renders both halves of its prompt this way before calling the LLM.**
   [`gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen)
   renders scenario/SOTA/feedback descriptions via `T(...).r(...)`, then calls
   [`hypothesis_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen),
   [`hypothesis_select_with_llm`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm),
   [`hypothesis_rewrite`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite),
   and [`task_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen)
   in sequence — each of which independently renders its own system/user prompt through `T(...).r(...)`
   before reaching the LLM backend described on the [rdagent-oai-backend-base](rdagent-oai-backend-base.md)
   page. The templating layer and the LLM call layer are the two halves of "how an FC-component actually
   talks to an LLM."

## Key data structures
- **`self.template`** — the raw loaded string (a yaml value or a whole text file), cached on the `RDAT`/`T`
  instance after `__init__` so `.r()` can be called repeatedly against the same loaded template with
  different context dicts without re-touching disk.
- **The `debug_tpl` log object** — a four-field record (`uri`, `template`, `context`, `rendered`) captured
  on every render call via [`log_object`](../catalog/rdagent/log/logger.md#RDAgentLog.log_object); this is
  the structure a log-viewer or trace-replay tool would key off of to reconstruct exactly what prompt was
  sent for any given call.

## Dynamics (design intent)
Rendering is synchronous and stateless per call: nothing is cached across `.r()` invocations beyond the
already-loaded `self.template`, so a component that renders the same template every experiment-loop
iteration (e.g. a recurring system prompt with a changing `scenario_desc`) pays a fresh Jinja render each
time — cheap relative to the LLM call it feeds, but not memoized. File-lookup order is strict-first-match,
not merge: if both an `app_tpl` override and the default template exist for the same path, the override
fully replaces the default rather than the two being combined.

## Edge cases
- A missing template surfaces as `FileNotFoundError` only after **every** candidate path in the priority
  list has been tried and failed — a typo'd URI can silently probe 2–4 different file locations before the
  final error names all of them together.
- A file that exists but is missing the requested nested yaml key is treated identically to a missing file
  (both caught and skipped internally before trying the next candidate) — from the outside, "wrong file"
  and "right file, wrong key" produce the same final exception, which can make debugging a broken template
  reference slower than it needs to be.
- `StrictUndefined` only protects the *rendering* step — a context value that is present but the wrong
  shape (e.g. a string where the template expects an iterable) still fails inside Jinja's own evaluation,
  not at this layer's boundary.

## Open questions
- Whether templates are ever cached/compiled across separate process runs, versus reloaded and reparsed
  from disk on every `RDAT.__init__` call, isn't addressed by this packet.
- The full catalog of shared prompt fragments pulled in via recursive `{% include %}` calls isn't
  enumerable from this packet alone — it would need a walk of the actual `prompts*.yaml` files across the
  repo, which are outside this subgraph.

## See also
- [rdagent-oai-backend-base — what happens to the string this layer produces](rdagent-oai-backend-base.md)
- [rdagent-oai-llm_conf — the `app_tpl` override field and other settings this layer reads](rdagent-oai-llm_conf.md)
