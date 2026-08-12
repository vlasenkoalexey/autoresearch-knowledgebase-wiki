---
title: Prime Agent's trust model — not a sandbox
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Prime Agent's trust model — not a sandbox

## Definition
The README's `[!WARNING]` block is explicit: "Prime Agent executes model-generated Python and project
commands with your user permissions. Its worker and kernel processes improve lifecycle isolation and
recovery; they are **not** a security sandbox. Review changes and use trusted repositories, instructions,
skills, and extensions only. Run untrusted code or instructions in an external sandbox or restricted
environment."

## In prime-agent (grounded)
The worker/kernel process split this warning references is the same
[`KernelManager`](../concepts/packages-coding-agent-src-core-kernel-index.ts.md) `forkKernel`/process-boundary
mechanism documented on that concept page — real isolation for crash recovery and resource limits, but the
forked kernel still executes with the same OS user's permissions as the daemon, so it stops process crashes
from taking down a session, not a malicious skill or extension from reading the user's files.

## Why it matters / when it applies
This directly qualifies the [verification-independence](../../../concepts/verification-independence.md)
concept this wiki already tracks: prime-agent's `/refine` self-editing
([refinement.ts](../concepts/packages-coding-agent-src-core-refinement-refinement.ts.md)) and its
package-manager auto-discovery of skills/extensions
([package-manager.ts](../concepts/packages-coding-agent-src-core-package-manager.ts.md)) both operate
inside this same trust boundary — a self-modifying agent that pulls in externally-authored skills or
extensions is only as trustworthy as those sources, independent of how principled its own refinement
mechanism is. The authors are explicit that this is the user's responsibility to manage, not something the
harness enforces.

## Connections
- Code concepts: [`packages-coding-agent-src-core-kernel-index.ts`](../concepts/packages-coding-agent-src-core-kernel-index.ts.md),
  [`packages-coding-agent-src-core-package-manager.ts`](../concepts/packages-coding-agent-src-core-package-manager.ts.md),
  [`packages-coding-agent-src-core-refinement-refinement.ts`](../concepts/packages-coding-agent-src-core-refinement-refinement.ts.md)
- Wiki: [`concepts/verification-independence.md`](../../../concepts/verification-independence.md)

## Source
Extracted from `README.md` (kept in place).
