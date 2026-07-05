---
title: 'Module: test/notebook/testfiles/main_missing_sections.py'
type: catalog
provenance: extracted
module: test/notebook/testfiles/main_missing_sections.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.notebook.testfiles.main_missing_sections`/
symbols:
  main: main().
  inference_and_submission: inference_and_submission().
  DEVICE: DEVICE.
  DEBUG: DEBUG.
  CactusDataset.__getitem__: CactusDataset#__getitem__().
  MODEL_DIR: MODEL_DIR.
  SEED: SEED.
  CactusDataset: CactusDataset#
  get_transforms: get_transforms().
  get_dataloader: get_dataloader().
  parser: parser.
  get_efficientnet_b3: get_efficientnet_b3().
  args: args.
  SAMPLE_SUB_PATH: SAMPLE_SUB_PATH.
  eval_model: eval_model().
  confusion_info: confusion_info().
  CactusDataset.__len__: CactusDataset#__len__().
  CactusDataset.image_ids: CactusDataset#image_ids.
  CactusDataset.labels: CactusDataset#labels.
  CactusDataset.transforms: CactusDataset#transforms.
  TRAIN_DIR: TRAIN_DIR.
  TEST_DIR: TEST_DIR.
  TRAIN_CSV: TRAIN_CSV.
  print_eda: print_eda().
  CactusDataset.id2path: CactusDataset#id2path.
  compute_class_weight: compute_class_weight().
  train_one_epoch: train_one_epoch().
  CactusDataset.__init__: CactusDataset#__init__().
---
# Module: [`test/notebook/testfiles/main_missing_sections.py`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py)

## Classes
### `CactusDataset`
- def: [`test/notebook/testfiles/main_missing_sections.py:61`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L61)
- signature: `class CactusDataset(Dataset):`
- members:
  - `id2path` — [`L65`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L65)
  - `image_ids` — [`L63`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L63)
  - `labels` — [`L64`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L64)
  - `transforms` — [`L66`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L66)
- protocol/private: `__getitem__`[`L71`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L71), `__init__`[`L62`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L62), `__len__`[`L68`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L68)
- used by: (2 test-only callers)

## Functions
- `compute_class_weight(y)` — [`L155`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L155)
- `confusion_info(y_true, y_pred, threshold=0.5)` — [`L223`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L223)
- `eval_model(model, loss_fn, dataloader, device, class_weights)` — [`L197`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L197)
- `get_dataloader(dataset, batch_size, shuffle=False, num_workers=4, pin_memory=True)` — [`L137`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L137)
- `get_efficientnet_b3(dropout_rate=0.3)` — [`L146`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L146)
- `get_transforms(mode='train')` — [`L87`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L87)
- `inference_and_submission(train_df, train_id2path, test_img_ids, test_id2path, dropout_rate, class_weights, need_weights, BATCH_SIZE, N_WORKERS, cv_fold)` — [`L228`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L228)
- `main()` — [`L300`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L300)
- `print_eda(train_df)` — [`L39`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L39)
- `train_one_epoch(model, loss_fn, optimizer, scheduler, dataloader, device, class_weights)` — [`L171`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L171)

## Module values
- `DEBUG` — [`L23`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L23)
- `DEVICE` — [`L31`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L31)
- `MODEL_DIR` — [`L36`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L36)
- `SAMPLE_SUB_PATH` — [`L35`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L35)
- `SEED` — [`L25`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L25)
- `TEST_DIR` — [`L33`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L33)
- `TRAIN_CSV` — [`L34`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L34)
- `TRAIN_DIR` — [`L32`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L32)
- `args` — [`L22`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L22)
- `parser` — [`L20`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_sections.py#L20)

