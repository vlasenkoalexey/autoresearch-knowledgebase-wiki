---
title: Executing LLM-written code (the sandbox caution)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Executing LLM-written code (the sandbox caution)

## Definition
The README opens with a prominent **Caution!**: this codebase *executes LLM-written code*. Because the
tree-search agent generates and then runs arbitrary Python it invented, the system inherits the risks of
that code — dangerous packages, uncontrolled web access, and unintended spawned processes. The README's
prescribed mitigation is to run the whole system inside a controlled sandbox such as a Docker container.

## In ai-scientist-v2 (grounded)
The execution surface the caution is about is the
[`Interpreter`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter) (owning module:
[`ai_scientist/treesearch/interpreter.py`](../catalog/ai_scientist/treesearch/interpreter.md)). Each node's
generated snippet is run through
[`Interpreter.run`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter.run), which executes in a
separate child process set up by
[`Interpreter.child_proc_setup`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter.child_proc_setup)
and torn down by
[`Interpreter.cleanup_session`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter.cleanup_session).
The outcome — including exception type/stack and captured terminal output — is returned as an
[`ExecutionResult`](../catalog/ai_scientist/treesearch/interpreter.md#ExecutionResult). Notably, the
guardrails the interpreter *does* enforce are a per-run wall-clock
[`Interpreter.timeout`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter.timeout) and an
injected
[`Interpreter.env_vars`](../catalog/ai_scientist/treesearch/interpreter.md#Interpreter.env_vars) set — a
child-process boundary and a timeout, **not** OS-level isolation. That is precisely why the README pushes
the isolation responsibility outward to the operator's container: the interpreter contains the code enough
to observe and time it, but it is not itself a security sandbox.

## Why it matters / when it applies
This caution applies to every experiment run — the moment `launch_scientist_bfts.py` starts a tree search,
LLM-authored code will run on the host. Anyone operating the system should assume the generated code is
untrusted and provide the isolation (Docker or equivalent) the README calls for, rather than relying on the
interpreter's in-process guards. It is the single most important operational precondition documented in the
README.

## Connections
- Code concepts:
  [ai_scientist-treesearch-interpreter](../concepts/ai_scientist-treesearch-interpreter.md) — the code
  execution subsystem in depth.
- Module catalogs:
  [ai_scientist/treesearch/interpreter](../catalog/ai_scientist/treesearch/interpreter.md).
- Related doc-concepts: [bfts-tree-search-configuration](bfts-tree-search-configuration.md) — the search
  that generates the code being executed.

## Source
Extracted from `README.md` (kept in place).
