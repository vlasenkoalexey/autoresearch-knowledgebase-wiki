---
title: Docker-sandboxed execution
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Docker-sandboxed execution

## Definition
Because the Development side of the loop runs *LLM-generated code*, R&D-Agent executes it inside Docker containers rather than on the host. The README makes Docker a hard prerequisite — "Users must ensure Docker is installed before attempting most scenarios," and the current user must be able to run Docker "without using sudo" (verified via `docker run hello-world`). Each scenario ships its own image (e.g. a Qlib image for the finance loops, an MLE-bench image for data science), and `rdagent health_check` explicitly probes whether the Docker installation works before a run.

## In rd-agent (grounded)
Sandboxed execution is the [`Env`](../catalog/rdagent/utils/env.md#Env) abstraction in module `rdagent/utils/env.py`, whose [`Env.run`](../catalog/rdagent/utils/env.md#Env.run) executes a command inside the environment. The Docker implementation is [`DockerEnv`](../catalog/rdagent/utils/env.md#DockerEnv), configured by [`DockerConf`](../catalog/rdagent/utils/env.md#DockerConf) (image, [`extra_volumes`](../catalog/rdagent/utils/env.md#DockerConf.extra_volumes), GPU kwargs); a [`LocalEnv`](../catalog/rdagent/utils/env.md#LocalEnv)/[`CondaConf`](../catalog/rdagent/utils/env.md#CondaConf) path exists as a non-Docker alternative. Scenario-specific images subclass the base: [`QTDockerEnv`](../catalog/rdagent/utils/env.md#QTDockerEnv) (Qlib quant), [`KGDockerEnv`](../catalog/rdagent/utils/env.md#KGDockerEnv) (Kaggle), and [`MLEBDockerEnv`](../catalog/rdagent/utils/env.md#MLEBDockerEnv) (MLE-bench). Code produced by the loop lands in an [`FBWorkspace`](../catalog/rdagent/core/experiment.md#FBWorkspace) and is run through [`FBWorkspace.execute`](../catalog/rdagent/core/experiment.md#FBWorkspace.execute) / [`FBWorkspace.run`](../catalog/rdagent/core/experiment.md#FBWorkspace.run), which dispatch into the chosen `Env`. The README's `docker`-related bits of [`health_check_cli`](../catalog/rdagent/app/cli.md#health_check_cli) surface exactly this dependency.

## Why it matters / when it applies
Sandboxing is what makes it safe to let an agent write and run arbitrary code across dozens of Kaggle-style tasks: dependencies are pinned per-scenario image, host state is protected, and runs are reproducible. The `extra_volumes` mechanism is how local datasets (e.g. `DS_LOCAL_DATA_PATH`, the downloaded competition data in the README's data-science example) are mounted into the container. Every scenario in the catalog ultimately executes through this layer, so a broken Docker setup blocks all of them — hence the mandatory `health_check`.

## Connections
- Code concepts: [utils/env](../concepts/rdagent-utils-env.md) — the Docker/conda sandbox in depth; [core/experiment](../concepts/rdagent-core-experiment.md) — the `FBWorkspace` whose code the sandbox runs.
- Module catalogs: [utils/env](../catalog/rdagent/utils/env.md), [core/experiment](../catalog/rdagent/core/experiment.md), [app/cli](../catalog/rdagent/app/cli.md).
- Related doc-concepts: [scenario-catalog](scenario-catalog.md), [research-development-framework](research-development-framework.md), [rdagent-cli](rdagent-cli.md).

## Source
Extracted from `README.md` (kept in place).
