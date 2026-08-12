---
title: VisionOnlyAgent — a minimal-baseline sibling agent
type: concept
provenance: mixed
concept: agents-vision_only_agent
updated: 2026-08-12
status: fresh
---
# VisionOnlyAgent — a minimal-baseline sibling agent

## Overview

`VisionOnlyAgent.run_step` — *"Run a single agent step"* — is a separate, simpler agent class from
[`agents-PokeAgent`](agents-PokeAgent.md)'s `PokeAgent`, calling a VLM directly on screenshots
(`call_vlm_with_image`) without the objective/subagent/harness-evolution machinery — the kind of minimal
`H_min` baseline the paper's own evaluation compares `continualharness` against.

## See also
- [`agents-PokeAgent`](agents-PokeAgent.md) — the full scaffold this is a baseline sibling to.
