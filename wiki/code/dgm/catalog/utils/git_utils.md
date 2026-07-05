---
title: 'Module: utils/git_utils.py'
type: catalog
provenance: extracted
module: utils/git_utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `utils.git_utils`/
symbols:
  diff_versus_commit: diff_versus_commit().
  apply_patch: apply_patch().
  reset_to_commit: reset_to_commit().
  remove_patch_by_files: remove_patch_by_files().
  filter_patch_by_files: filter_patch_by_files().
  get_git_commit_hash: get_git_commit_hash().
---
# Module: [`utils/git_utils.py`](../../../../../raw/code/dgm/utils/git_utils.py)

## Functions
- `apply_patch(git_dname, patch_str)` — [`L17`](../../../../../raw/code/dgm/utils/git_utils.py#L17) — Apply a patch to the repository at `git_dname`.
- `diff_versus_commit(git_dname, commit)` — [`L36`](../../../../../raw/code/dgm/utils/git_utils.py#L36) — Take a diff of `git_dname` current contents versus the `commit`, including untracked files, — documented in [coding_agent](../../concepts/coding_agent.md)
- `filter_patch_by_files(patch_str, target_files)` — [`L102`](../../../../../raw/code/dgm/utils/git_utils.py#L102) — Filters out the diff blocks related to any of the target_files in a patch string.
- `get_git_commit_hash(repo_path='.')` — [`L6`](../../../../../raw/code/dgm/utils/git_utils.py#L6)
- `remove_patch_by_files(patch_str, keyword='polyglot')` — [`L126`](../../../../../raw/code/dgm/utils/git_utils.py#L126) — Removes diff blocks related to files containing the keyword from a patch string.
- `reset_to_commit(git_dname, commit)` — [`L71`](../../../../../raw/code/dgm/utils/git_utils.py#L71) — Reset the repository at `git_dname` to the given `commit`.

