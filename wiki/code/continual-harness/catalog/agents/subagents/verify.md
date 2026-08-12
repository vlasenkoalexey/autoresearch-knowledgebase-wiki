---
title: 'Module: agents/subagents/verify.py'
type: catalog
provenance: extracted
module: agents/subagents/verify.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.verify`/
symbols:
  parse_verify_response: parse_verify_response().
  build_verify_prompt: build_verify_prompt().
  _extract_json_object: _extract_json_object().
  resolve_verification_target: resolve_verification_target().
  _strip_markdown_json_fence: _strip_markdown_json_fence().
---
# Module: [`agents/subagents/verify.py`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py)

## Functions
- `_extract_json_object(text: str)` — [`L131`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py#L131)
- `_strip_markdown_json_fence(text: str)` — [`L116`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py#L116) — Remove leading  fences so models can still return fenced JSON.
- `build_verify_prompt(*, context: Dict[str, Any], target: Dict[str, Any], last_n_steps: int, reasoning: str)` — [`L52`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py#L52) — Build the verify-subagent prompt.
- `parse_verify_response(raw_text: str, *, target: Dict[str, Any])` — [`L152`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py#L152) — Parse and normalize the verifier response.
- `resolve_verification_target(objective_state: Dict[str, Any], category: Optional[str] = None)` — [`L11`](../../../../../../raw/code/continual-harness/agents/subagents/verify.py#L11) — Resolve the authoritative objective that verify should judge.

