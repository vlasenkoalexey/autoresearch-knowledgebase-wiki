---
title: "APIBackend() — a factory call disguised as a constructor"
type: concept
provenance: mixed
concept: rdagent-oai-llm_utils
updated: 2026-07-04
status: fresh
---
# APIBackend() — a factory call disguised as a constructor

## Overview
`rdagent/oai/llm_utils.py` is a tiny module that does one load-bearing thing: it makes
`APIBackend()` — the syntax literally every LLM-calling line in this ~40-call-site Research/Development
codebase uses — resolve to whichever *concrete* backend class is configured, at call time, via a single
settings string. `APIBackend` is not the abstract class of the same name from the sibling backend-base
module; it is a function alias, `APIBackend = get_api_backend`, so every call site that appears to be
instantiating an ABC directly is actually invoking a dynamic-import factory. That's the whole trick this
module exists to provide, plus one small utility built on top of it for embedding-based string similarity.

## Diagram
```mermaid
flowchart LR
    call["APIBackend(...)<br/>(≈40 call sites: hypothesis_gen,<br/>task_gen, evaluate, implement_one_task, ...)"]
    call --> alias["APIBackend = get_api_backend"]
    alias --> gab["get_api_backend(*args, **kwargs)"]
    gab --> ic["import_class(LLM_SETTINGS.backend)"]
    ic --> cls["resolved class<br/>(e.g. LiteLLMAPIBackend)"]
    cls --> inst["cls(*args, **kwargs)"]
    inst --> ret["a working APIBackend instance"]
    settings["LLM_SETTINGS.backend<br/>(dotted class path string)"] -.-> ic
```

## Design rationale (why it's built this way)
- **A dotted-path string plus a generic loader, not an enum or a dispatch table.** [`get_api_backend`](../catalog/rdagent/oai/llm_utils.md#get_api_backend)
  calls [`import_class`](../catalog/rdagent/core/utils.md#import_class) on [`LLM_SETTINGS`](../catalog/rdagent/oai/llm_conf.md#LLM_SETTINGS)`.backend`,
  a plain string (`"rdagent.oai.backend.LiteLLMAPIBackend"` by default). Adding a wholly new backend
  implementation is therefore a zero-code-change operation for every one of the ~40 call sites in the
  codebase — write a new class satisfying the four abstract primitives described on the
  [rdagent-oai-backend-base](rdagent-oai-backend-base.md) page, then change one config string. There is no
  registry to update here.
- **The alias makes the call site read like construction, and that's deliberate.** `APIBackend()` reads
  identically everywhere — [`hypothesis_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen),
  [`task_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen),
  [`generate_feedback`](../catalog/rdagent/scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback),
  and every [`implement_one_task`](../catalog/rdagent/scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task)
  variant across the coder components all open an LLM interaction with the same four characters — none of
  them need to know or care whether that resolves to the LiteLLM-routed backend or a legacy one.
  > [!inferred]
  > The source itself flags this indirection as slightly uncomfortable rather than fully settled: `get_api_backend`
  > carries a `# TODO: import it from base.py` comment, suggesting the author considered this factory
  > logically belonging next to the ABC it constructs (in `backend/base.py`) rather than in this separate
  > module — likely a historical artifact of how the base/deprec/litellm split evolved, though the source
  > doesn't say so directly.
- **Batched, normalized similarity rather than a bespoke endpoint.** [`calculate_embedding_distance_between_str_list`](../catalog/rdagent/oai/llm_utils.md#calculate_embedding_distance_between_str_list)
  concatenates the source and target string lists into a *single* [`APIBackend`](../catalog/rdagent/oai/llm_utils.md#APIBackend)`.create_embedding`
  call (one round trip, one cache pass, instead of two), then L2-normalizes both halves and takes a single
  matrix product to get a full pairwise cosine-similarity matrix — reusing the exact same caching/retry
  path every other embedding call in the codebase goes through, rather than adding a second one.

## Entry points
- [`APIBackend`](../catalog/rdagent/oai/llm_utils.md#APIBackend) — the entry point ~40+ call sites across
  the codebase use to get a working backend instance; syntactically indistinguishable from constructing
  the abstract class of the same name in `backend/base.py`, but actually a function call.
- [`get_api_backend`](../catalog/rdagent/oai/llm_utils.md#get_api_backend) — the real logic the alias
  points at; reached every single time any component needs to talk to an LLM or embedding model.
- [`calculate_embedding_distance_between_str_list`](../catalog/rdagent/oai/llm_utils.md#calculate_embedding_distance_between_str_list) —
  a narrower entry point for semantic-similarity comparisons, built directly on the same backend factory.

## Mechanism (step-by-step)
1. **The alias resolves at import time, the class resolves at call time.** `APIBackend = get_api_backend`
   is evaluated once, when the module loads; but [`get_api_backend`](../catalog/rdagent/oai/llm_utils.md#get_api_backend)
   itself re-reads [`LLM_SETTINGS`](../catalog/rdagent/oai/llm_conf.md#LLM_SETTINGS)`.backend` on *every*
   invocation, so a config change between calls (or between processes sharing the same settings file)
   changes which class gets constructed without any code reload.
2. **Dynamic import turns a string into a live class.** [`import_class`](../catalog/rdagent/core/utils.md#import_class)
   takes the dotted path and returns the actual Python class object; `get_api_backend` then instantiates it
   with whatever positional/keyword args the caller passed straight through — those flow into the
   `APIBackend.__init__` cache-flag parameters described on the sibling backend-base page.
3. **Every downstream FC-component sees an identical call surface.** Whether it's
   [`hypothesis_gen`](../catalog/rdagent/scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen)
   generating a research hypothesis or a coder's [`implement_one_task`](../catalog/rdagent/scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task)
   writing code, both open with the bare call `APIBackend()` — the factory indirection is invisible at
   every use site, which is the entire point.
4. **Similarity is one embedding call plus linear algebra, not an LLM round-trip per pair.** `calculate_embedding_distance_between_str_list`
   gets embeddings for the *whole* combined list from [`APIBackend`](../catalog/rdagent/oai/llm_utils.md#APIBackend)
   in one shot, splits the resulting vectors back into source/target halves by index, and normalizes before
   the dot product — an O(1)-call design regardless of how many source/target strings are compared.

## Key data structures
- **`LLM_SETTINGS.backend: str`** — the single field that decides which concrete class *every*
  `APIBackend()` call in the codebase actually resolves to; changing it changes the whole system's LLM
  provider without touching a call site.
- **`similarity_matrix: list[list[float]]`** — a dense `len(source) × len(target)` matrix returned as
  plain nested lists (not a numpy array, not a top-k result) — callers do their own thresholding or
  argmax on top of it.

## Dynamics (design intent)
There is no memoization or singleton behavior at this layer: `get_api_backend` constructs a brand-new
backend instance on every call, and every one of the ~40 `APIBackend()` call sites in the codebase gets a
fresh object that re-reads the caching/retry flags from [`LLM_SETTINGS`](../catalog/rdagent/oai/llm_conf.md#LLM_SETTINGS)
itself. This is cheap because the backend classes are close to stateless (the actual chat/embedding cache
lives in a shared on-disk store, not on the instance) — but a reader used to factory functions returning a
shared singleton should not assume that here.

## Edge cases
- `calculate_embedding_distance_between_str_list` returns `[[]]` if either input list is empty, a
  deliberately degenerate sentinel rather than raising — it guards a downstream divide-by-zero in the
  normalization step rather than pushing the empty-input check onto callers.
- Neither this module nor `import_class` validates `LLM_SETTINGS.backend` at settings-construction time; a
  bad dotted path surfaces as a raw import error on the *first* `APIBackend()` call in a run, not at
  startup.

## Open questions
- [`import_class`](../catalog/rdagent/core/utils.md#import_class)'s own error-handling behavior (what
  exception shape a bad path produces) is outside this packet's subgraph.
- Whether any caller actually depends on `get_api_backend` returning a *shared* instance across calls
  within one process (e.g. for embedding-cache reuse) isn't settled here — the default behavior is a fresh
  instance every time.

## See also
- [rdagent-oai-backend-base — the class every resolved backend is an instance of](rdagent-oai-backend-base.md)
- [rdagent-oai-llm_conf — the `backend` field and everything else this factory reads](rdagent-oai-llm_conf.md)
