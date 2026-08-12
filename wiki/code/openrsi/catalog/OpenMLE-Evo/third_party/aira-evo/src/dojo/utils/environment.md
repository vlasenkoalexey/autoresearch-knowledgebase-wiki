---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.utils.environment`/
symbols:
  get_mlebench_data_dir: get_mlebench_data_dir().
  get_log_dir: get_log_dir().
  get_superimage_dir: get_superimage_dir().
  ENV_VAR_NOT_FOUND_ERR: ENV_VAR_NOT_FOUND_ERR.
  get_default_slurm_partition: get_default_slurm_partition().
  get_default_slurm_account: get_default_slurm_account().
  get_default_slurm_qos: get_default_slurm_qos().
  get_hardware: get_hardware().
  check_pytorch_gpu: check_pytorch_gpu().
  check_tensorflow_gpu: check_tensorflow_gpu().
  format_time: format_time().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py)

## Functions
- `check_pytorch_gpu()` — [`L32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L32) — Check if PyTorch can use a GPU.
- `check_tensorflow_gpu()` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L44) — Check if TensorFlow can use a GPU.
- `format_time(seconds)` — [`L56`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L56) — Convert time in seconds to a human-readable format.
- `get_default_slurm_account()` — [`L97`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L97) — Get the default Slurm account from the configuration.
- `get_default_slurm_partition()` — [`L89`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L89) — Get the default Slurm partition from the configuration.
- `get_default_slurm_qos()` — [`L105`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L105) — Get the default Slurm QoS from the configuration.
- `get_hardware()` — [`L20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L20) — Determine available hardware (GPU or CPU).
- `get_log_dir()` — [`L64`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L64) — Get the log directory, creating it if it doesn't exist.
- `get_mlebench_data_dir()` — [`L81`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L81) — Get the MLEBench data directory, creating it if it doesn't exist.
- `get_superimage_dir()` — [`L72`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L72) — Get the superimage directory, creating it if it doesn't exist.

## Module values
- `ENV_VAR_NOT_FOUND_ERR` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/environment.py#L14)

