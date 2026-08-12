---
title: 'Module: OpenMLE-Gym/builder_core/utils/struct.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/builder_core/utils/struct.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.builder_core.utils.struct`/Structure#
symbols:
  Structure.comp_id_dir: comp_id_dir().
  Structure.public_dir: public_dir().
  Structure.raw_dir: raw_dir().
  Structure.private_dir: private_dir().
  Structure.__init__: __init__().
  Structure.data_dir: data_dir().
  Structure.utils_dir: utils_dir().
  Structure.TASK_DIR: TASK_DIR.
  Structure.data_comp_id_dir: data_comp_id_dir().
  Structure.DOWNLOAD_DIR: DOWNLOAD_DIR.
  Structure.COMP_DIR: COMP_DIR.
  Structure: ''
  Structure.DATA_DIR: DATA_DIR.
  Structure.BASE: BASE.
  Structure.TASK: TASK.
---
# Module: [`OpenMLE-Gym/builder_core/utils/struct.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py)

## Classes
### `Structure`
- def: [`OpenMLE-Gym/builder_core/utils/struct.py:3`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L3) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- signature: `class Structure:`
- members:
  - `comp_id_dir(self, comp_id: str)` — [`L25`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L25) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `data_comp_id_dir(self, comp_id: str)` — [`L28`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L28) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `data_dir(self, comp_id: str)` — [`L34`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L34) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `private_dir(self, comp_id: str)` — [`L46`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L46) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `public_dir(self, comp_id: str)` — [`L43`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L43) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `raw_dir(self, comp_id: str)` — [`L31`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L31) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `utils_dir(self, comp_id: str)` — [`L37`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L37) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `BASE` — [`L5`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L5)
  - `COMP_DIR` — [`L9`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L9)
  - `DATA_DIR` — [`L10`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L10)
  - `DOWNLOAD_DIR` — [`L8`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L8)
  - `TASK` — [`L6`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L6)
  - `TASK_DIR` — [`L7`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L7) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- protocol/private: `__init__`[`L4`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/struct.py#L4)
- used by: [`structure`](nodes.md#NodeExecutor.structure), [`prepare_single_competition`](nodes.md#NodeExecutor.prepare_single_competition), [`Copy`](nodes.md#NodeExecutor.Copy), [`Metric`](nodes.md#NodeExecutor.Metric), [`Perceive`](nodes.md#NodeExecutor.Perceive), [`Prepare`](nodes.md#NodeExecutor.Prepare), [`Describe`](nodes.md#NodeExecutor.Describe), [`Next`](nodes.md#NodeExecutor.Next), [`Download`](nodes.md#NodeExecutor.Download), [`Scrape`](nodes.md#NodeExecutor.Scrape), [`_cleanup_failed_competition`](nodes.md#NodeExecutor._cleanup_failed_competition), [`get_prepare_function`](nodes.md#NodeExecutor.get_prepare_function), [`prepare_validation`](nodes.md#NodeExecutor.prepare_validation)  (1 test-only)

