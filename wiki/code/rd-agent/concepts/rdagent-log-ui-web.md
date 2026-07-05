---
title: "rdagent/log/ui/web.py — a type-dispatched Streamlit log viewer (superseded for DS/MLE-Bench)"
type: concept
provenance: mixed
concept: rdagent-log-ui-web
updated: 2026-07-04
status: fresh
---
# rdagent/log/ui/web.py — a type-dispatched Streamlit log viewer (superseded for DS/MLE-Bench)

## Overview
`web.py` defines a small Composite-pattern hierarchy of Streamlit "window" objects — [`StWindow`](../catalog/rdagent/log/ui/web.md#StWindow)
and roughly twenty subclasses — that turn a flat, time-ordered stream of typed log
[`Message`](../catalog/rdagent/log/base.md#Message)s into a nested, human-browsable report: one widget class
per domain object (hypotheses, feedback, factor/model tasks and workspaces, Qlib experiments), selected
purely by `isinstance(msg.content, ...)` rather than by the message's tag. But this module is built entirely
around the *earlier* Qlib factor/model scenario's object types, and is not reachable from anywhere else in
the current codebase — a repo-wide search finds zero imports of its `WebView`/`SimpleTraceWindow`/`TraceWindow`
classes outside the file itself. The flagship Data-Science/MLE-Bench scenario this wiki otherwise centers on
is instead served by a separate, actively-committed sibling module (`rdagent/log/ui/ds_trace.py`, wired into
`dsapp.py`) that sits outside this packet's Subgraph. Read this page as "how a generic message-stream
renderer works," not as "the UI you'd run today to inspect an MLE-Bench trace."

## Diagram
```mermaid
flowchart TD
    MSG["Message stream<br/>(tag, content)"] --> DISPATCH["StWindow.consume_msg()"]
    DISPATCH -->|tag ends llm_messages| LLMW["LLMWindow"]
    DISPATCH -->|content isinstance Hypothesis| HYPW["HypothesisWindow.consume_msg()"]
    DISPATCH -->|content isinstance HypothesisFeedback| HFW["HypothesisFeedbackWindow.consume_msg()"]
    DISPATCH -->|content isinstance QlibFactorExperiment /<br/>QlibModelExperiment| QEW["QlibFactorExpWindow /<br/>QlibModelExpWindow .consume_msg()"]
    DISPATCH -->|content is a list| OTW["ObjectsTabsWindow.consume_msg()"]
    OTW -->|per item, fresh Message| DISPATCH
    HIST["Trace.hist"] -->|mock_msg() per tuple| TOW["TraceObjWindow.consume_msg()"]
    TOW --> HYPW
    TOW --> QEW
    TOW --> HFW
```

## Design rationale (why it's built this way)
Dispatch is purely type-based (`isinstance(msg.content, X)`), not tag-based, and this generality is real, not
accidental: [`Hypothesis`](../catalog/rdagent/core/proposal.md#Hypothesis) and
[`HypothesisFeedback`](../catalog/rdagent/core/proposal.md#HypothesisFeedback) are defined in the fully
generic `rdagent.core.proposal` module, so `HypothesisWindow`'s
[`consume_msg`](../catalog/rdagent/log/ui/web.md#HypothesisWindow.consume_msg) would happily render a
[`DSHypothesis`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis)
too, since `DSHypothesis` is-a `Hypothesis`. But that generality stops at the experiment layer:
[`SimpleTraceWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#SimpleTraceWindow.consume_msg) and
[`TraceWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#TraceWindow.consume_msg) only special-case
[`QlibFactorExperiment`](../catalog/rdagent/scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment)
and [`QlibModelExperiment`](../catalog/rdagent/scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment).
[`DSExperiment`](../catalog/rdagent/scenarios/data_science/experiment/experiment.md#DSExperiment) — present in
this packet's Subgraph only because it reaches the generic
[`Experiment`](../catalog/rdagent/core/experiment.md#Experiment) base class via a class-hierarchy edge, not
because `web.py` actually branches on it — falls through every `isinstance` check in
`SimpleTraceWindow.consume_msg` to the generic "common logs" fallback: a bare `str()` dump, shown only if
`show_common_logs` is enabled, otherwise silently dropped. This module's richer per-object rendering (results
tables, plotly bar charts) genuinely does not extend to the experiments the Data-Science/MLE-Bench
application (see [`rdagent-app-data_science-conf`](rdagent-app-data_science-conf.md)) actually produces.

> [!inferred] This is cross-checked directly, not inferred from naming alone: a full-text search of the
> pinned commit finds no import of `WebView`, `SimpleTraceWindow`, or `TraceWindow` anywhere outside this
> file, `rdagent/log/ui/` contains a separate, far larger module (`ds_trace.py`) with its own `dsapp.py`
> Streamlit page registration, and `web.py`'s last feature-level commit (`refactor for general data science`)
> predates `ds_trace.py`'s introduction by roughly nine months of subsequent, much more active history on the
> newer file. None of that is in this packet's Subgraph, so the *mechanism* of `ds_trace.py`/`dsapp.py` isn't
> covered here — but the conclusion that `web.py` is a superseded, Qlib-era viewer rather than the UI in
> active use is a reading of directly-observed facts, flagged here because it fundamentally changes how this
> page should be read.

Several subclasses exist purely to cope with Streamlit's execution model: because the whole script re-runs
top-to-bottom on every interaction rather than maintaining live widget state, `ProgressTabsWindow`'s
[`consume_msg`](../catalog/rdagent/log/ui/web.md#ProgressTabsWindow.consume_msg) and
[`ObjectsTabsWindow`](../catalog/rdagent/log/ui/web.md#ObjectsTabsWindow)'s both replay a per-tab message
cache the instant a new tab is created, so a sibling tab that already existed gets "caught up" to the same
point in the stream rather than starting blank. [`mock_msg`](../catalog/rdagent/log/ui/web.md#mock_msg) exists
for the opposite reason: it lets a `consume_msg` method written to expect a `Message` (for its
`.content`/`.tag`) also be driven directly from a bare domain object, so the same rendering code serves both
live log streaming and the one-shot "replay a whole `Trace` after the fact" mode used by `TraceObjWindow`'s
[`consume_msg`](../catalog/rdagent/log/ui/web.md#TraceObjWindow.consume_msg).

## Entry points
None of this module's classes are reachable from any script or CLI entry point in the current codebase (see
Design rationale). Within this packet's Subgraph, the closest things to an entry seam are:
- [`mock_msg`](../catalog/rdagent/log/ui/web.md#mock_msg) — synthesizes a `Message` on the fly so a window can
  be driven from a bare object; used by [`TraceObjWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#TraceObjWindow.consume_msg)
  to replay a [`Trace`](../catalog/rdagent/core/proposal.md#Trace)'s [`hist`](../catalog/rdagent/core/proposal.md#Trace.hist)
  outside of any live stream.
- [`StWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#StWindow.consume_msg) — the base-case renderer
  (one line via `container.code(...)`) that every other window either overrides or implicitly falls back to.

## Mechanism (step-by-step)
1. A message arrives at whichever `consume_msg` override sits at the current nesting level.
   [`SimpleTraceWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#SimpleTraceWindow.consume_msg), the
   topmost dispatcher in this Subgraph, first compares the *length* of `msg.tag` against the previously-seen
   tag to decide whether to print a new section header — using the dotted namespace's nesting **depth** as a
   proxy for "we entered a new stage," not its actual structure.

2. It special-cases `tag.endswith("llm_messages")` *before* any type check, routing to an `LLMWindow` only if
   `show_llm` is enabled, independent of `msg.content`'s type. Every other branch dispatches purely on
   `isinstance(msg.content, ...)`: [`Hypothesis`](../catalog/rdagent/core/proposal.md#Hypothesis),
   [`HypothesisFeedback`](../catalog/rdagent/core/proposal.md#HypothesisFeedback),
   [`QlibFactorExperiment`](../catalog/rdagent/scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment),
   [`QlibModelExperiment`](../catalog/rdagent/scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment),
   or a non-empty list whose first element's type ([`FactorTask`](../catalog/rdagent/components/coder/factor_coder/factor.md#FactorTask),
   [`ModelTask`](../catalog/rdagent/components/coder/model_coder/model.md#ModelTask),
   [`FactorFBWorkspace`](../catalog/rdagent/components/coder/factor_coder/factor.md#FactorFBWorkspace), or
   [`ModelFBWorkspace`](../catalog/rdagent/components/coder/model_coder/model.md#ModelFBWorkspace)) picks the
   tab layout.

3. [`ObjectsTabsWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#ObjectsTabsWindow.consume_msg) fans a
   list-valued message out into one Streamlit tab per element — reusing caller-supplied tab names when given,
   or mapping each object to a name otherwise — and, critically, synthesizes a *fresh* single-object
   [`Message`](../catalog/rdagent/log/base.md#Message) (copying `tag`, re-using
   [`content`](../catalog/rdagent/log/base.md#Message.content)) per tab, so the exact same `inner_class.consume_msg`
   used for a scalar message is reused recursively at every nesting level rather than needing a separate
   list-aware renderer per type.

4. [`TraceWindow.consume_msg`](../catalog/rdagent/log/ui/web.md#TraceWindow.consume_msg) — the outermost,
   full-page window — filters out `llm_messages` and plain string/dict content up front, updates a running
   hypothesis list and a plotly [`result`](../catalog/rdagent/core/experiment.md#Experiment.result) chart
   purely by matching `msg.tag.endswith(...)` suffixes (`"hypothesis generation"`, `"ef.feedback"`,
   `"ef.model runner result"`/`"ef.factor runner result"`), and *then* forwards the same message down into a
   `RoundTabsWindow`'s [`consume_msg`](../catalog/rdagent/log/ui/web.md#RoundTabsWindow.consume_msg) — a tab
   per `SingleRDLoopWindow` (whose own
   [`consume_msg`](../catalog/rdagent/log/ui/web.md#SingleRDLoopWindow.consume_msg) routes again by whether
   `"r"`/`"d"`/`"ef"` appears in the tag split on `.`). A single message can therefore be inspected by three
   independent tag/type filters on its way from the top of the tree to its final rendering leaf.

5. `TraceObjWindow`'s [`consume_msg`](../catalog/rdagent/log/ui/web.md#TraceObjWindow.consume_msg) is the one
   renderer in this Subgraph that does *not* stream from a live log at all: given a
   [`Trace`](../catalog/rdagent/core/proposal.md#Trace) directly, it iterates the recorded
   `(hypothesis, experiment, feedback)` tuples in [`hist`](../catalog/rdagent/core/proposal.md#Trace.hist) and
   replays each through `HypothesisWindow`'s
   [`consume_msg`](../catalog/rdagent/log/ui/web.md#HypothesisWindow.consume_msg), a Qlib experiment window,
   and `HypothesisFeedbackWindow`'s
   [`consume_msg`](../catalog/rdagent/log/ui/web.md#HypothesisFeedbackWindow.consume_msg), wrapping each in
   [`mock_msg`](../catalog/rdagent/log/ui/web.md#mock_msg) — an offline "replay the whole trace at once" mode,
   the opposite assumption from every other window's implicit "fed one message at a time, in order."

## Key data structures
- [`Message`](../catalog/rdagent/log/base.md#Message) (`tag`, `content` cited) — the atomic unit every
  window consumes. `tag` is treated as *both* a human-readable breadcrumb (split on `.` for headers) and a
  dispatch key (`endswith` checks) — its exact dotted-namespace convention is load-bearing even though
  nothing in this Subgraph enforces its shape.
- The `StWindow` hierarchy itself: a [`container`](../catalog/rdagent/log/ui/web.md#StWindow.container)
  reference (a Streamlit `DeltaGenerator`) is essentially the *only* state most subclasses carry — nesting is
  achieved by constructing a child window against a Streamlit sub-container (`.expander()`, `.tabs()`,
  `.container()`), not by any explicit tree object, so the "tree" only exists implicitly in one
  `consume_msg` call's call graph.

## Dynamics (design intent)
Strictly single-pass, synchronous, in log order — there is no concurrency. Every window assumes `consume_msg`
is invoked once per message in exactly the order the underlying log yields them, and the stateful windows
(`SimpleTraceWindow`, via its [`current_win`](../catalog/rdagent/log/ui/web.md#SimpleTraceWindow.current_win)
field, and `TraceWindow`) exist precisely because they need to recognize a *transition* between consecutive
messages (a new tag depth, a new hypothesis), not just react to one message in isolation.

## Edge cases
- `SimpleTraceWindow.consume_msg` mutates `msg.content` in place when filtering falsy list items
  (`msg.content = [m for m in msg.content if m]`) — if the same message object were ever handed to more than
  one consumer, the second would observe the filtered list, though nothing in this Subgraph currently does
  that.
- `TraceWindow.consume_msg`'s handling of an `"ef.feedback"`-tagged message indexes `self.hypotheses[-1]`
  unconditionally — an out-of-order or missing hypothesis-generation message ahead of it would raise
  `IndexError` rather than degrade gracefully.
- Any `Experiment` subtype other than `QlibFactorExperiment`/`QlibModelExperiment` — including `DSExperiment`,
  the type this wiki's own MLE-Bench-focused application actually produces — is invisible to this module's
  rich rendering; see Design rationale.

## Open questions
- Whether `ds_trace.py`/`dsapp.py` (outside this packet's Subgraph) reuse any of this module's `StWindow`
  base classes, or reimplement the message-dispatch pattern independently, isn't settled here.
- Whether anyone still runs this module directly (e.g. `streamlit run rdagent/log/ui/web.py`) as an ad hoc
  tool, as opposed to it being fully dead code, can't be confirmed from source alone.

## See also
- [`rdagent-app-data_science-conf`](rdagent-app-data_science-conf.md) — the application whose `DSExperiment`
  traces this module's rich rendering does not cover.
- [`rdagent-app-CI-run`](rdagent-app-CI-run.md) — a different application whose LLM conversations are
  transitively logged into the same `Message`/`Storage` infrastructure this viewer reads from.
