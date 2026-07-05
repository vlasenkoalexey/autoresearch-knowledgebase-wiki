---
title: 'Module: rdagent/scenarios/finetune/download/hf.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/download/hf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.download.hf`/
symbols:
  download_model: download_model().
  download_dataset: download_dataset().
  _ensure_parent: _ensure_parent().
  _get_hf_token: _get_hf_token().
---
# Module: [`rdagent/scenarios/finetune/download/hf.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/download/hf.py)

## Functions
- `_ensure_parent(path: Path)` — [`L7`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/download/hf.py#L7)
- `_get_hf_token(token: Optional[str] = None)` — [`L11`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/download/hf.py#L11) — Get HuggingFace token from parameter or environment variables.
- `download_dataset(repo_id: str, out_dir: str, token: Optional[str] = None, revision: Optional[str] = None, force: bool = False)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/download/hf.py#L21) — Download HuggingFace dataset to a specified directory using snapshot_download.
- `download_model(repo_id: str, out_dir_root: Optional[str] = None, token: Optional[str] = None, revision: Optional[str] = None, force: bool = False)` — [`L66`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/download/hf.py#L66) — Download Hugging Face model to a subdirectory under the specified root: <out_dir_root>/<repo_id>

