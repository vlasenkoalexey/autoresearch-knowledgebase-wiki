---
title: core.llm_client — the shared LLM plumbing both levels call through
type: concept
provenance: mixed
concept: core-llm_client
updated: 2026-07-05
status: fresh
---
# core.llm_client — the shared LLM plumbing both levels call through

## Overview
`core/llm_client.py` is the one piece of infrastructure every level of the bilevel loop shares: Level 1's
per-iteration proposal calls, Level 1.5's search-config analysis, and Level 2's four-round mechanism-research
dialogue all bottom out in the same
[`call`](../catalog/core/llm_client.md#LLMClient.call) /
[`call_llm`](../catalog/core/llm_client.md#call_llm) primitives and the same
[`parse_json_response`](../catalog/core/llm_client.md#parse_json_response) parser. That's not an accident —
the paper's central claim is that the *architecture* (bilevel structure), not a stronger meta-level model,
produces the gain, and one visible piece of evidence for that is that inner and outer calls share
undifferentiated plumbing: neither gets a special retry policy, a special parser, or bespoke error handling.
The one real design fork is *global* vs. *instance* configuration — [`call_llm`](../catalog/core/llm_client.md#call_llm)
is driven by module-level global config (the provider/model/key that `configure()` sets once at process
start, which `call_llm` then reads on every call), while [`LLMClient`](../catalog/core/llm_client.md#LLMClient)
carries that configuration per-instance — built precisely because a single process runs an inner-loop model
and an outer-loop model side by side.

## Diagram
```mermaid
flowchart TB
    PROVIDERS[("PROVIDERS registry")] --> LLMClient["LLMClient (instance-scoped)"]
    PROVIDERS --> call_llm["call_llm() (module-global config)"]
    LLMClient --> call["call()"]
    call_llm --> call
    call --> propose["_propose (train_opt runner, Level 1)"]
    call --> analyze["_analyze (Level 1.5)"]
    call --> extractLessons["_extract_lessons (Level 1)"]
    call --> session["_run_session / _generate_with_retries (Level 2, via core.base_mechanism_research)"]
    call --> researchArticle["research (article_opt Level 2)"]
    call --> researchTrain["research (train_opt Level 2)"]
    propose --> parse["parse_json_response()"]
    extractLessons --> parse
```

## Design rationale (why it's built this way)
[`LLMClient`](../catalog/core/llm_client.md#LLMClient)'s docstring states the reason for its existence
directly: "Use this instead of `configure()` + `call_llm()` when multiple providers must coexist in the same
process (e.g. inner loop uses MiniMax, outer loop uses DeepSeek). Does not touch module-level globals." That
sentence is a direct consequence of the paper's architecture — the bilevel design *requires* two LLM
configurations to be live simultaneously (an inner-loop provider proposing training-config edits, an
outer-loop provider running Level 1.5 analysis and Level 2's dialogue), so a single set of mutable
module-level globals configured once at process start can't serve both at once. Rather than special-case
that, the module keeps the simple global-config path for single-model callers (tests, scripts) and adds a
parallel instance-scoped path for anything that needs two models alive together.

[`parse_json_response`](../catalog/core/llm_client.md#parse_json_response) exists because every structured
exchange in this system — a Level 1 proposal's `changes` dict, a Level 1.5 `SearchConfig` update, a Level 2
spec's metadata — arrives as free-text LLM output that may or may not be clean JSON. Its docstring says it
"Handles: plain JSON, markdown code fences, inline JSON" and "Uses non-greedy matching to avoid consuming
multiple JSON objects" — i.e. it tries direct `json.loads` first, then a fenced-code-block regex, then a
manual balanced-brace scan, falling back to a `raw_content` sentinel rather than raising, so a single
malformed LLM response degrades a caller's proposal to a no-op instead of crashing the loop.

## Entry points
- [`call`](../catalog/core/llm_client.md#LLMClient.call) — the instance method every `LLMClient`-based caller
  goes through; this is where an inner-loop `_propose` and an outer-loop `research` session both actually
  hit the network.
- [`call_llm`](../catalog/core/llm_client.md#call_llm) — the module-level convenience entry point for
  single-provider callers (used by
  [`_extract_lessons`](../catalog/domains/article_opt/runner.md#InnerRunner._extract_lessons)); its own
  docstring: "Call the configured LLM provider with automatic retry."
- [`parse_json_response`](../catalog/core/llm_client.md#parse_json_response) — the landing point for every
  LLM response that's expected to carry structured data, reached immediately after a `call`/`call_llm`
  return.
- [`PROVIDERS`](../catalog/core/llm_client.md#PROVIDERS.PROVIDERS) — the registry both `LLMClient.__init__`
  and `call_llm` read to resolve base URL, default model, API-key env var, and whether a provider needs the
  native SDK path.

## Mechanism (step-by-step)
1. Every call — instance ([`call`](../catalog/core/llm_client.md#LLMClient.call)) or module-level
   ([`call_llm`](../catalog/core/llm_client.md#call_llm)) — wraps the underlying request in the same retry
   shape: a loop of `max_retries` attempts, catching any exception and sleeping
   `retry_delay * 2**attempt` between tries, then raising a `RuntimeError` wrapping the last error only after
   the budget is exhausted. Neither Level 1's proposal calls nor Level 2's four-round dialogue calls get a
   different retry policy — the same primitive backs both.
2. [`_propose`](../catalog/domains/train_opt/runner.md#TrainRunner._propose) (Level 1, training domain) is
   the clearest example of the pattern this module is built for: it calls `call`, immediately hands the raw
   text to [`parse_json_response`](../catalog/core/llm_client.md#parse_json_response), and treats a
   non-dict or `raw_content`-tagged result as a parse failure rather than propagating an exception.
3. [`_analyze`](../catalog/domains/train_opt/outer.md#TrainOuterLoop._analyze) (Level 1.5) uses the identical
   `call` + `parse_json_response` pair to turn the outer LLM's free text into a structured search-config
   update — its own docstring is "Ask outer LLM to analyze inner trace and propose search config changes,"
   confirming Level 1.5's output is itself just another JSON payload parsed through this same path.
4. [`_extract_lessons`](../catalog/domains/article_opt/runner.md#InnerRunner._extract_lessons) is the one
   caller in this subgraph that goes through the module-level
   [`call_llm`](../catalog/core/llm_client.md#call_llm) instead of an `LLMClient` instance, then also feeds
   the result through `parse_json_response` — its docstring: "Extract structured lessons from this run's
   outputs and evaluation."
5. Level 2's dialogue — [`research`](../catalog/domains/article_opt/mechanism_research.md#MechanismResearcher.research)
   and [`research`](../catalog/domains/train_opt/mechanism_research.md#TrainMechanismResearcher.research) for
   the two domains, driving [`_run_session`](../catalog/core/base_mechanism_research.md#BaseMechanismResearcher._run_session)
   and [`_generate_with_retries`](../catalog/core/base_mechanism_research.md#BaseMechanismResearcher._generate_with_retries) —
   issues every one of its four rounds (Explore, Critique, Specify, Generate) through the same `call`
   primitive on a `client: LLMClient` instance held by the researcher, with no code-generation-specific retry
   or backoff logic layered on top of what `call` already provides.

## Key data structures
- [`PROVIDERS`](../catalog/core/llm_client.md#PROVIDERS.PROVIDERS) — a dict keyed by provider name
  (`deepseek`, `openai`, `glm`, `minimax`, `anthropic` per the module docstring) holding `base_url`,
  `default_model`, `api_key_env`, and `native_sdk`; both configuration paths resolve through this one table.
- [`LLMClient`](../catalog/core/llm_client.md#LLMClient) — holds a resolved model/provider and a
  pre-constructed underlying SDK client, so that two `LLMClient` instances (e.g. one MiniMax, one DeepSeek)
  can be alive in the same process without interfering.

## Dynamics (design intent)
> [!inferred] Nothing in this packet's Subgraph shows the retry/backoff behavior actually executing (that
> would require mocking a failing provider call, which isn't among the cited tests) — the design intent
> above is read directly from `call`'s and `call_llm`'s control flow and docstrings, not observed.

## Edge cases
- [`parse_json_response`](../catalog/core/llm_client.md#parse_json_response) returns `{"raw_content": ""}`
  for an empty/falsy input string, and `{"raw_content": text}` when none of its three parse strategies
  succeed — callers such as `_propose` explicitly check for `"raw_content" in result` to detect this failure
  mode rather than assuming every returned value is the expected shape.
- Because [`LLMClient`](../catalog/core/llm_client.md#LLMClient) resolves and caches its underlying SDK
  client once at construction time, a `LLMClient` instance is bound to one provider/model/API-key for its
  whole lifetime — swapping models mid-run means constructing a new instance, not mutating the existing one
  (this is the opposite tradeoff from `call_llm`'s mutable globals).

## Open questions
- The provider-specific dispatch inside `call`/`call_llm` (native Anthropic SDK vs. OpenAI-compatible
  `chat.completions.create`, and the `<think>`-tag stripping some reasoning models require) is real behavior
  visible in `core/llm_client.py`, but the private helpers that implement it are not in this packet's own
  Subgraph (they surface instead in the `core-base_mechanism_research` packet) — see that page for the
  parts of this module cited there.

## See also
- [core-base_mechanism_research](core-base_mechanism_research.md) — the Level 2 researcher base class that
  is this module's heaviest caller (four `call`s per session, plus the code-fix retry loop).
- [core-inner_loop](core-inner_loop.md) — orchestrates the `run_once` calls whose `_propose`/
  `_extract_lessons` internals route through this module.
- [domains-train_opt-runner](domains-train_opt-runner.md) and
  [domains-article_opt-runner](domains-article_opt-runner.md) — hold the concrete `_propose`/
  `_extract_lessons` callers cited above.
- [domains-train_opt-outer](domains-train_opt-outer.md) — holds `_analyze`, Level 1.5's consumer of this
  module.
- [../../../sources/bilevel-autoresearch.md](../../../sources/bilevel-autoresearch.md) — see "Both the inner
  and outer loop use the *same* LLM" for why this module deliberately doesn't differentiate its callers.
