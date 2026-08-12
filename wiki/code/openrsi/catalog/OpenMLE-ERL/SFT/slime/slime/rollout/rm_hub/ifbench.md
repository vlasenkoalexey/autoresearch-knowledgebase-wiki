---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.rm_hub.ifbench`/
symbols:
  _build_input_example: _build_input_example().
  compute_ifbench_reward: compute_ifbench_reward().
  _ensure_ifbench_dependencies: _ensure_ifbench_dependencies().
  _load_evaluation_lib: _load_evaluation_lib().
  evaluation_lib: evaluation_lib.
  InputExample: InputExample.
  logger: logger.
  _WORKSPACE_PARENT: _WORKSPACE_PARENT.
  _LOCAL_IFBENCH_REQUIREMENTS: _LOCAL_IFBENCH_REQUIREMENTS.
  _ensure_ifbench_repo: _ensure_ifbench_repo().
  _coerce_kwargs_list: _coerce_kwargs_list().
  KwargsDict: KwargsDict.
  _WORKSPACE_ROOT: _WORKSPACE_ROOT.
  JsonDict: JsonDict.
  _normalize_instruction_ids: _normalize_instruction_ids().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py)

## Functions
- `_build_input_example(metadata: JsonDict)` — [`L131`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L131)
- `_coerce_kwargs_list(raw_kwargs: Any, num_instructions: int)` — [`L100`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L100) — Convert stored kwargs into the list structure expected by IFBench.
- `_ensure_ifbench_dependencies(repo_path: Path)` — [`L47`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L47) — Install IFBench requirements the first time the module is imported.
- `_ensure_ifbench_repo()` — [`L19`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L19) — Clone IFBench repo if needed and ensure it is available on sys.path.
- `_load_evaluation_lib()` — [`L69`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L69)
- `_normalize_instruction_ids(raw_ids: Sequence[Any])` — [`L86`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L86) — Ensure instruction identifiers are clean strings.
- `compute_ifbench_reward(response: str, label: Any, metadata: JsonDict | None = None)` — [`L154`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L154) — Score a model response using the official IFBench rules.

## Module values
- `InputExample` — [`L79`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L79)
- `JsonDict` — [`L82`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L82)
- `KwargsDict` — [`L83`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L83)
- `_LOCAL_IFBENCH_REQUIREMENTS` — [`L16`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L16)
- `_WORKSPACE_PARENT` — [`L15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L15)
- `_WORKSPACE_ROOT` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L14)
- `evaluation_lib` — [`L78`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L78)
- `logger` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/rm_hub/ifbench.py#L12)

