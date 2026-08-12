---
title: 'Module: packages/coding-agent/test/acp-kernel-features.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/acp-kernel-features.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`acp-kernel-features.test.ts`/
symbols:
  bundledSkill: bundledSkill().
  why: why().
  AGENT_MESSAGE_SKILL: AGENT_MESSAGE_SKILL.
  toolEndEvent: toolEndEvent().
  why.result-typeLiteral0.stderr: why().(result)typeLiteral0:stderr.
  why.result-typeLiteral0.error: why().(result)typeLiteral0:error.
  why.result-typeLiteral0.error.typeLiteral1.traceback: why().(result)typeLiteral0:error.typeLiteral1:traceback.
  why.result-typeLiteral0.status: why().(result)typeLiteral0:status.
---
# Module: [`packages/coding-agent/test/acp-kernel-features.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts)

## Functions
- `bundledSkill(name: string, importName: string)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L27)
- `toolEndEvent(toolCallId: string, output: string, isError?: boolean)` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L35) — Wrap kernel output the way the ipython tool result reaches the event stream.
- `why(result: { status: string; stderr: string; error?: { traceback: string[]; } | undefined; })` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L23) — Surface the Python traceback: a bare status assertion hides the real cause.

## Module values
- `AGENT_MESSAGE_SKILL` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L32)
- `error` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L23)
- `status` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L23)
- `stderr` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L23)
- `traceback` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-kernel-features.test.ts#L23)

