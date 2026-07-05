---
title: 'Module: test/notebook/testfiles/main_missing_main_fn.py'
type: catalog
provenance: extracted
module: test/notebook/testfiles/main_missing_main_fn.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.notebook.testfiles.main_missing_main_fn`/
symbols:
  fold_model_path: fold_model_path.
  cm: cm.
  model_files: model_files.
  train_df: train_df.
  idx_neg: idx_neg.
  need_weights: need_weights.
  inference_and_submission: inference_and_submission().
  model: model.
  test_pred_list: test_pred_list.
  train_loss: train_loss.
  val_pred: val_pred.
  fold_class_weights: fold_class_weights.
  val_idx: val_idx.
  fold: fold.
  train_ds: train_ds.
  val_ds: val_ds.
  oof_cm: oof_cm.
  test_id2path: test_id2path.
  df_val: df_val.
  DEVICE: DEVICE.
  val_loader: val_loader.
  scores_df: scores_df.
  train_loader: train_loader.
  estimated_time: estimated_time.
  test_ds: test_ds.
  test_loader: test_loader.
  fold_test_pred: fold_test_pred.
  DEBUG: DEBUG.
  submission: submission.
  e: e.
  CactusDataset.__getitem__: CactusDataset#__getitem__().
  MODEL_DIR: MODEL_DIR.
  train_id2path: train_id2path.
  cv_fold: cv_fold.
  dropout_rate: dropout_rate.
  dist: dist.
  probs: probs.
  sampled_idxs: sampled_idxs.
  fold_idx: fold_idx.
  idx_pos: idx_pos.
  EPOCHS: EPOCHS.
  df_train: df_train.
  val_auc: val_auc.
  SEED: SEED.
  f: f.
  epoch: epoch.
  img_ids: img_ids.
  fold_labels: fold_labels.
  optimizer: optimizer.
  debug_time: debug_time.
  oof_auc: oof_auc.
  debug_epochs: debug_epochs.
  sample_sub: sample_sub.
  skf: skf.
  scheduler: scheduler.
  logits: logits.
  class_weights: class_weights.
  test_img_ids: test_img_ids.
  CactusDataset: CactusDataset#
  get_transforms: get_transforms().
  get_dataloader: get_dataloader().
  best_auc: best_auc.
  parser: parser.
  folds: folds.
  val_img_ids: val_img_ids.
  all_oof_true: all_oof_true.
  all_oof_pred: all_oof_pred.
  get_efficientnet_b3: get_efficientnet_b3().
  BATCH_SIZE: BATCH_SIZE.
  N_WORKERS: N_WORKERS.
  val_true: val_true.
  args: args.
  y_train: y_train.
  MIN_EPOCHS: MIN_EPOCHS.
  EARLY_STOP_PATIENCE: EARLY_STOP_PATIENCE.
  start_time: start_time.
  train_img_ids: train_img_ids.
  train_labels: train_labels.
  val_labels: val_labels.
  end_time: end_time.
  test_probs: test_probs.
  batch: batch.
  SAMPLE_SUB_PATH: SAMPLE_SUB_PATH.
  eval_model: eval_model().
  confusion_info: confusion_info().
  loss_fn: loss_fn.
  best_epoch: best_epoch.
  patience: patience.
  n_pos: n_pos.
  n_neg: n_neg.
  images: images.
  CactusDataset.__len__: CactusDataset#__len__().
  CactusDataset.image_ids: CactusDataset#image_ids.
  CactusDataset.labels: CactusDataset#labels.
  CactusDataset.transforms: CactusDataset#transforms.
  sample_frac: sample_frac.
  best_model_state: best_model_state.
  preds: preds.
  oof_true: oof_true.
  oof_pred: oof_pred.
  fold_scores: fold_scores.
  TRAIN_DIR: TRAIN_DIR.
  TEST_DIR: TEST_DIR.
  TRAIN_CSV: TRAIN_CSV.
  print_eda: print_eda().
  CactusDataset.id2path: CactusDataset#id2path.
  compute_class_weight: compute_class_weight().
  train_one_epoch: train_one_epoch().
  LR: LR.
  imbalance_ratio: imbalance_ratio.
  idx: idx.
  fold_val_ids: fold_val_ids.
  val_loss: val_loss.
  CactusDataset.__init__: CactusDataset#__init__().
---
# Module: [`test/notebook/testfiles/main_missing_main_fn.py`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py)

## Classes
### `CactusDataset`
- def: [`test/notebook/testfiles/main_missing_main_fn.py:61`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L61)
- signature: `class CactusDataset(Dataset):`
- members:
  - `id2path` — [`L65`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L65)
  - `image_ids` — [`L63`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L63)
  - `labels` — [`L64`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L64)
  - `transforms` — [`L66`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L66)
- protocol/private: `__getitem__`[`L71`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L71), `__init__`[`L62`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L62), `__len__`[`L68`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L68)
- used by: (4 test-only callers)

## Functions
- `compute_class_weight(y)` — [`L155`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L155)
- `confusion_info(y_true, y_pred, threshold=0.5)` — [`L223`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L223)
- `eval_model(model, loss_fn, dataloader, device, class_weights)` — [`L197`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L197)
- `get_dataloader(dataset, batch_size, shuffle=False, num_workers=4, pin_memory=True)` — [`L137`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L137)
- `get_efficientnet_b3(dropout_rate=0.3)` — [`L146`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L146)
- `get_transforms(mode='train')` — [`L87`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L87)
- `inference_and_submission(train_df, train_id2path, test_img_ids, test_id2path, dropout_rate, class_weights, need_weights, BATCH_SIZE, N_WORKERS, cv_fold)` — [`L228`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L228)
- `print_eda(train_df)` — [`L39`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L39)
- `train_one_epoch(model, loss_fn, optimizer, scheduler, dataloader, device, class_weights)` — [`L171`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L171)

## Module values
- `BATCH_SIZE` — [`L363`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L363)
- `DEBUG` — [`L23`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L23)
- `DEVICE` — [`L31`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L31)
- `EARLY_STOP_PATIENCE` — [`L367`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L367)
- `EPOCHS` — [`L365`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L365)
- `LR` — [`L368`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L368)
- `MIN_EPOCHS` — [`L366`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L366)
- `MODEL_DIR` — [`L36`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L36)
- `N_WORKERS` — [`L364`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L364)
- `SAMPLE_SUB_PATH` — [`L35`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L35)
- `SEED` — [`L25`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L25)
- `TEST_DIR` — [`L33`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L33)
- `TRAIN_CSV` — [`L34`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L34)
- `TRAIN_DIR` — [`L32`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L32)
- `all_oof_pred` — [`L460`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L460)
- `all_oof_true` — [`L459`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L459)
- `args` — [`L22`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L22)
- `batch` — [`L481`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L481)
- `best_auc` — [`L410`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L410)
- `best_epoch` — [`L411`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L411)
- `best_model_state` — [`L412`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L412)
- `class_weights` — [`L319`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L319)
- `cm` — [`L421`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L421)
- `cv_fold` — [`L327`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L327)
- `debug_epochs` — [`L359`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L359)
- `debug_time` — [`L451`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L451)
- `df_train` — [`L382`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L382)
- `df_val` — [`L383`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L383)
- `dist` — [`L335`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L335)
- `dropout_rate` — [`L339`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L339)
- `e` — [`L303`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L303)
- `end_time` — [`L449`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L449)
- `epoch` — [`L415`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L415)
- `estimated_time` — [`L452`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L452)
- `f` — [`L334`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L334)
- `fold` — [`L380`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L380)
- `fold_class_weights` — [`L407`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L407)
- `fold_idx` — [`L347`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L347)
- `fold_labels` — [`L348`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L348)
- `fold_model_path` — [`L438`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L438)
- `fold_scores` — [`L377`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L377)
- `fold_test_pred` — [`L487`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L487)
- `fold_val_ids` — [`L377`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L377)
- `folds` — [`L329`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L329)
- `idx` — [`L330`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L330)
- `idx_neg` — [`L350`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L350)
- `idx_pos` — [`L349`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L349)
- `images` — [`L482`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L482)
- `imbalance_ratio` — [`L319`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L319)
- `img_ids` — [`L482`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L482)
- `logits` — [`L484`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L484)
- `loss_fn` — [`L404`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L404)
- `model` — [`L402`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L402)
- `model_files` — [`L370`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L370)
- `n_neg` — [`L319`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L319)
- `n_pos` — [`L319`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L319)
- `need_weights` — [`L319`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L319)
- `oof_auc` — [`L461`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L461)
- `oof_cm` — [`L462`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L462)
- `oof_pred` — [`L377`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L377)
- `oof_true` — [`L377`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L377)
- `optimizer` — [`L405`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L405)
- `parser` — [`L20`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L20)
- `patience` — [`L413`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L413)
- `preds` — [`L479`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L479)
- `probs` — [`L485`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L485)
- `sample_frac` — [`L344`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L344)
- `sample_sub` — [`L310`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L310)
- `sampled_idxs` — [`L345`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L345)
- `scheduler` — [`L406`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L406)
- `scores_df` — [`L498`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L498)
- `skf` — [`L328`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L328)
- `start_time` — [`L378`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L378)
- `submission` — [`L493`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L493)
- `test_ds` — [`L466`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L466)
- `test_id2path` — [`L315`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L315)
- `test_img_ids` — [`L314`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L314)
- `test_loader` — [`L471`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L471)
- `test_pred_list` — [`L472`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L472)
- `test_probs` — [`L490`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L490)
- `train_df` — [`L302`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L302)
- `train_ds` — [`L390`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L390)
- `train_id2path` — [`L308`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L308)
- `train_img_ids` — [`L385`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L385)
- `train_labels` — [`L386`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L386)
- `train_loader` — [`L400`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L400)
- `train_loss` — [`L416`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L416)
- `val_auc` — [`L420`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L420)
- `val_ds` — [`L395`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L395)
- `val_idx` — [`L330`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L330)
- `val_img_ids` — [`L387`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L387)
- `val_labels` — [`L388`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L388)
- `val_loader` — [`L401`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L401)
- `val_loss` — [`L418`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L418)
- `val_pred` — [`L418`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L418)
- `val_true` — [`L418`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L418)
- `y_train` — [`L318`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main_missing_main_fn.py#L318)

