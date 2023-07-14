# Comparing `tmp/funasr-0.6.9.tar.gz` & `tmp/funasr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.6.9.tar", last modified: Thu Jul  6 11:10:16 2023, max compression
+gzip compressed data, was "funasr-0.7.0.tar", last modified: Fri Jul 14 11:07:13 2023, max compression
```

## Comparing `funasr-0.6.9.tar` & `funasr-0.7.0.tar`

### file list

```diff
@@ -1,442 +1,446 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.173673 funasr-0.6.9/
--rw-r--r--   0 zhifu      (502) staff       (20)    10194 2023-07-06 11:10:16.173286 funasr-0.6.9/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     9217 2023-07-06 06:23:18.000000 funasr-0.6.9/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.889404 funasr-0.6.9/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.920998 funasr-0.6.9/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    71449 2023-07-06 11:04:13.000000 funasr-0.6.9/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.9/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5565 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-06 11:07:57.000000 funasr-0.6.9/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12149 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.927161 funasr-0.6.9/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.9/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18668 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_model_from_file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_streaming_iterator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_sv_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.930484 funasr-0.6.9/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.950562 funasr-0.6.9/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.952530 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.959003 funasr-0.6.9/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3118 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.961658 funasr-0.6.9/funasr/datasets/small_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.6.9/funasr/datasets/small_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/datasets/small_datasets/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.962546 funasr-0.6.9/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.6.9/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.964319 funasr-0.6.9/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.965827 funasr-0.6.9/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.985536 funasr-0.6.9/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.9/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.990430 funasr-0.6.9/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.991414 funasr-0.6.9/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.994505 funasr-0.6.9/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.9/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.995491 funasr-0.6.9/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.999385 funasr-0.6.9/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.012843 funasr-0.6.9/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.023362 funasr-0.6.9/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.024914 funasr-0.6.9/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.6.9/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.029593 funasr-0.6.9/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.066277 funasr-0.6.9/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.071192 funasr-0.6.9/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/e2e_asr_bat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100258 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.078993 funasr-0.6.9/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.080872 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.083778 funasr-0.6.9/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.084527 funasr-0.6.9/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.085121 funasr-0.6.9/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.086463 funasr-0.6.9/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.087359 funasr-0.6.9/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.089351 funasr-0.6.9/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.091925 funasr-0.6.9/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.100690 funasr-0.6.9/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.103060 funasr-0.6.9/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.106498 funasr-0.6.9/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.9/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.107529 funasr-0.6.9/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/modules/eend_ola/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.109035 funasr-0.6.9/funasr/modules/eend_ola/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/report.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.111842 funasr-0.6.9/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.9/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.9/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.114953 funasr-0.6.9/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.117592 funasr-0.6.9/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.119957 funasr-0.6.9/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.6.9/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.121223 funasr-0.6.9/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.123046 funasr-0.6.9/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.123268 funasr-0.6.9/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.124356 funasr-0.6.9/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.9/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.125110 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.127489 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-06-30 02:11:21.000000 funasr-0.6.9/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.131021 funasr-0.6.9/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.132845 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.135491 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.139211 funasr-0.6.9/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.141602 funasr-0.6.9/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.146184 funasr-0.6.9/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    62178 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.148911 funasr-0.6.9/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.151523 funasr-0.6.9/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.153619 funasr-0.6.9/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.9/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.164166 funasr-0.6.9/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.6.9/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.6.9/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.9/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.6.9/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.6.9/funasr/utils/runtime_sdk_download_tool.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.9/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.6.9/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-06 11:09:47.000000 funasr-0.6.9/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.909489 funasr-0.6.9/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)    10194 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    14037 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      757 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-06 11:10:16.173784 funasr-0.6.9/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     3630 2023-06-30 02:11:21.000000 funasr-0.6.9/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.166932 funasr-0.6.9/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-05 02:29:20.000000 funasr-0.6.9/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.9/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.9/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.9/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.9/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-05 02:28:54.000000 funasr-0.6.9/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.9/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.900815 funasr-0.7.0/
+-rw-r--r--   0 zhifu      (502) staff       (20)    10026 2023-07-14 11:07:13.900558 funasr-0.7.0/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     9049 2023-07-14 07:04:33.000000 funasr-0.7.0/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.504896 funasr-0.7.0/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.537545 funasr-0.7.0/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    71935 2023-07-14 11:00:31.000000 funasr-0.7.0/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.7.0/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5565 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12181 2023-07-14 11:00:09.000000 funasr-0.7.0/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.543590 funasr-0.7.0/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.7.0/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18908 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.545767 funasr-0.7.0/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.546897 funasr-0.7.0/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.565961 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.572755 funasr-0.7.0/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3118 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.575120 funasr-0.7.0/funasr/datasets/small_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.7.0/funasr/datasets/small_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/datasets/small_datasets/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.575966 funasr-0.7.0/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.7.0/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.582351 funasr-0.7.0/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.584123 funasr-0.7.0/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.586876 funasr-0.7.0/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.7.0/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.589334 funasr-0.7.0/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.590155 funasr-0.7.0/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.592458 funasr-0.7.0/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.7.0/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.593201 funasr-0.7.0/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.597759 funasr-0.7.0/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.600592 funasr-0.7.0/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.668629 funasr-0.7.0/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.669178 funasr-0.7.0/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.7.0/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.702733 funasr-0.7.0/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.732041 funasr-0.7.0/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.738613 funasr-0.7.0/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/e2e_asr_bat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100274 2023-07-07 03:08:26.000000 funasr-0.7.0/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.773296 funasr-0.7.0/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20694 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/models/encoder/branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17014 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/models/encoder/e_branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.775695 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.782351 funasr-0.7.0/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.783439 funasr-0.7.0/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.784277 funasr-0.7.0/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.785459 funasr-0.7.0/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.786119 funasr-0.7.0/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.787910 funasr-0.7.0/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.789111 funasr-0.7.0/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.798122 funasr-0.7.0/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.800897 funasr-0.7.0/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3480 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/cgmlp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.803738 funasr-0.7.0/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.7.0/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.804611 funasr-0.7.0/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/modules/eend_ola/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.806217 funasr-0.7.0/funasr/modules/eend_ola/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/report.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/modules/embedding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5282 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/fastformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.808662 funasr-0.7.0/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.7.0/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4283 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.811110 funasr-0.7.0/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.812401 funasr-0.7.0/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.813814 funasr-0.7.0/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.7.0/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.814802 funasr-0.7.0/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.815201 funasr-0.7.0/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.815389 funasr-0.7.0/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.816368 funasr-0.7.0/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.7.0/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.817141 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.819711 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-06-30 02:11:21.000000 funasr-0.7.0/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.823282 funasr-0.7.0/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.825611 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.830272 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.833912 funasr-0.7.0/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.835661 funasr-0.7.0/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.840134 funasr-0.7.0/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    62140 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.850601 funasr-0.7.0/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.854034 funasr-0.7.0/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.855775 funasr-0.7.0/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.7.0/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.874817 funasr-0.7.0/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.7.0/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.7.0/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.7.0/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.7.0/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.7.0/funasr/utils/runtime_sdk_download_tool.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.7.0/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.7.0/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-14 11:02:23.000000 funasr-0.7.0/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.506233 funasr-0.7.0/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)    10026 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    14184 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      757 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-14 11:07:13.900886 funasr-0.7.0/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3630 2023-06-30 02:11:21.000000 funasr-0.7.0/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.900006 funasr-0.7.0/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-05 02:29:20.000000 funasr-0.7.0/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.7.0/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.7.0/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.7.0/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.7.0/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-05 02:28:54.000000 funasr-0.7.0/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.7.0/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.6.9/PKG-INFO` & `funasr-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.9
+Version: 0.7.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,21 +35,21 @@
 </p>
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Usage**](#usage)
-| [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
-| [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
+| [**Quick Start**](#quick-start)
+| [**Runtime**](./funasr/runtime/readme.md)
+| [**Model Zoo**](./docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
-| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
+
+<a name="whats-new"></a>
 ## What's new: 
 
 ### FunASR runtime-SDK
 
 - 2023.07.03: 
 We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 
@@ -57,19 +57,21 @@
 
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 ### Release notes
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
+<a name="highlights"></a>
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
+<a name="Installation"></a>
 ## Installation
 
 Install from pip
 ```shell
 pip3 install -U funasr
 # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple
@@ -91,15 +93,16 @@
 pip3 install -U modelscope
 # For the users in China, you could install with the command:
 # pip3 install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
 For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-## Usage
+<a name="quick-start"></a>
+## Quick Start
 
 You could use FunASR by:
 
 - egs
 - egs_modelscope
 - runtime
 
@@ -141,14 +144,16 @@
 
 For the client:
 ```shell
 python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
 #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
+
+<a name="contact"></a>
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
 
 |Dingding group |                     Wechat group                      |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.9 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.7.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -22,32 +22,28 @@
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
-[**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
-FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
-FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
-[**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+[**Quick Start**](#quick-start) | [**Runtime**](./funasr/runtime/readme.md) |
+[**Model Zoo**](./docs/model_zoo/modelscope_models.md) | [**Contact**]
+(#contact)  ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
 the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
 supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
 are pleased to announce that the M2MeT2.0 challenge has been accepted by the
 ASRU 2023 challenge special session. The registration is now open. The baseline
 system is conducted on FunASR and is provided as a receipe of AliMeeting
 corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-
-academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+academy/FunASR/releases)  ## Highlights - FunASR is a fundamental speech
 recognition toolkit that offers a variety of features, including speech
 recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
 Language Models, Speaker Verification, Speaker diarization and multi-talker
 ASR. - We have released a vast collection of academic and industrial pretrained
 models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
 speech-recognition), which can be accessed through our [Model Zoo](https://
 github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
@@ -55,49 +51,49 @@
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
 recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
 pretrained models from the [ModelScope](https://www.modelscope.cn/
 models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
 dataloader in FunASR enables faster training speeds for large-scale datasets.
 This feature enhances the efficiency of the speech recognition process for
-researchers and practitioners. ## Installation Install from pip ```shell pip3
+researchers and practitioners.  ## Installation Install from pip ```shell pip3
 install -U funasr # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
 install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
 && cd FunASR pip3 install -e ./ # For the users in China, you could install
 with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
 simple ``` If you want to use the pretrained models in ModelScope, you should
 install the modelscope: ```shell pip3 install -U modelscope # For the users in
 China, you could install with the command: # pip3 install -U modelscope -
 f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
 mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
 [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
-installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
-runtime ### egs If you want to train the model from scratch, you could use
-funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
-. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
-found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
-modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
-or finetune pretraining models from modelscope, you could use funasr by
-modelscope pipeline, as the following: ```python from modelscope.pipelines
+installation.html)  ## Quick Start You could use FunASR by: - egs -
+egs_modelscope - runtime ### egs If you want to train the model from scratch,
+you could use funasr directly by recipe, as the following: ```shell cd egs/
+aishell/paraformer . ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More
+examples could be found in [docs](https://alibaba-damo-academy.github.io/
+FunASR/en/modelscope_pipeline/quick_start.html) ### egs_modelscope If you want
+to infer or finetune pretraining models from modelscope, you could use funasr
+by modelscope pipeline, as the following: ```python from modelscope.pipelines
 import pipeline from modelscope.utils.constant import Tasks inference_pipeline
 = pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
 funasr_wss_server.py --port 10095 ``` For the client: ```shell python
 funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
 "5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ``` More examples could be found in [docs](https://alibaba-damo-
-academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2)  ## Contact If
 you have any questions about FunASR, please contact us by - email:
 [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
 Wechat group | |:---:|:-----------------------------------------------------:
 | |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
```

### Comparing `funasr-0.6.9/README.md` & `funasr-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 </p>
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Usage**](#usage)
-| [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
-| [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
+| [**Quick Start**](#quick-start)
+| [**Runtime**](./funasr/runtime/readme.md)
+| [**Model Zoo**](./docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
-| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
+
+<a name="whats-new"></a>
 ## What's new: 
 
 ### FunASR runtime-SDK
 
 - 2023.07.03: 
 We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 
@@ -32,19 +32,21 @@
 
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 ### Release notes
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
+<a name="highlights"></a>
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
+<a name="Installation"></a>
 ## Installation
 
 Install from pip
 ```shell
 pip3 install -U funasr
 # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple
@@ -66,15 +68,16 @@
 pip3 install -U modelscope
 # For the users in China, you could install with the command:
 # pip3 install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
 For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-## Usage
+<a name="quick-start"></a>
+## Quick Start
 
 You could use FunASR by:
 
 - egs
 - egs_modelscope
 - runtime
 
@@ -116,14 +119,16 @@
 
 For the client:
 ```shell
 python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
 #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
+
+<a name="contact"></a>
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
 
 |Dingding group |                     Wechat group                      |
```

#### html2text {}

```diff
@@ -9,32 +9,28 @@
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
-[**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
-FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
-FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
-[**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+[**Quick Start**](#quick-start) | [**Runtime**](./funasr/runtime/readme.md) |
+[**Model Zoo**](./docs/model_zoo/modelscope_models.md) | [**Contact**]
+(#contact)  ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
 the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
 supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
 are pleased to announce that the M2MeT2.0 challenge has been accepted by the
 ASRU 2023 challenge special session. The registration is now open. The baseline
 system is conducted on FunASR and is provided as a receipe of AliMeeting
 corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-
-academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+academy/FunASR/releases)  ## Highlights - FunASR is a fundamental speech
 recognition toolkit that offers a variety of features, including speech
 recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
 Language Models, Speaker Verification, Speaker diarization and multi-talker
 ASR. - We have released a vast collection of academic and industrial pretrained
 models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
 speech-recognition), which can be accessed through our [Model Zoo](https://
 github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
@@ -42,49 +38,49 @@
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
 recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
 pretrained models from the [ModelScope](https://www.modelscope.cn/
 models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
 dataloader in FunASR enables faster training speeds for large-scale datasets.
 This feature enhances the efficiency of the speech recognition process for
-researchers and practitioners. ## Installation Install from pip ```shell pip3
+researchers and practitioners.  ## Installation Install from pip ```shell pip3
 install -U funasr # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
 install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
 && cd FunASR pip3 install -e ./ # For the users in China, you could install
 with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
 simple ``` If you want to use the pretrained models in ModelScope, you should
 install the modelscope: ```shell pip3 install -U modelscope # For the users in
 China, you could install with the command: # pip3 install -U modelscope -
 f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
 mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
 [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
-installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
-runtime ### egs If you want to train the model from scratch, you could use
-funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
-. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
-found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
-modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
-or finetune pretraining models from modelscope, you could use funasr by
-modelscope pipeline, as the following: ```python from modelscope.pipelines
+installation.html)  ## Quick Start You could use FunASR by: - egs -
+egs_modelscope - runtime ### egs If you want to train the model from scratch,
+you could use funasr directly by recipe, as the following: ```shell cd egs/
+aishell/paraformer . ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More
+examples could be found in [docs](https://alibaba-damo-academy.github.io/
+FunASR/en/modelscope_pipeline/quick_start.html) ### egs_modelscope If you want
+to infer or finetune pretraining models from modelscope, you could use funasr
+by modelscope pipeline, as the following: ```python from modelscope.pipelines
 import pipeline from modelscope.utils.constant import Tasks inference_pipeline
 = pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
 funasr_wss_server.py --port 10095 ``` For the client: ```shell python
 funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
 "5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ``` More examples could be found in [docs](https://alibaba-damo-
-academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2)  ## Contact If
 you have any questions about FunASR, please contact us by - email:
 [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
 Wechat group | |:---:|:-----------------------------------------------------:
 | |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
```

### Comparing `funasr-0.6.9/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.7.0/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/asr_infer.py` & `funasr-0.7.0/funasr/bin/asr_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/asr_inference_launch.py` & `funasr-0.7.0/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,14 +435,15 @@
         rtf_avg = "decoding, feature length total: {}, forward_time total: {:.4f}, rtf avg: {:.4f}".format(length_total,
                                                                                                            forward_time_total,
                                                                                                            100 * forward_time_total / (
                                                                                                                    length_total * lfr_factor))
         logging.info(rtf_avg)
         if writer is not None:
             ibest_writer["rtf"]["rtf_avf"] = rtf_avg
+        torch.cuda.empty_cache()
         return asr_result_list
 
     return _forward
 
 
 def inference_paraformer_vad_punc(
         maxlenratio: float,
@@ -726,14 +727,15 @@
                 ibest_writer["vad"][key] = "{}".format(vadsegments)
                 ibest_writer["text"][key] = " ".join(word_lists)
                 ibest_writer["text_with_punc"][key] = text_postprocessed_punc
                 if time_stamp_postprocessed is not None:
                     ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
 
             logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
+        torch.cuda.empty_cache()
         return asr_result_list
 
     return _forward
 
 
 def inference_paraformer_online(
         maxlenratio: float,
@@ -1268,35 +1270,35 @@
         beam_size: int,
         ngpu: int,
         seed: int,
         lm_weight: float,
         nbest: int,
         num_workers: int,
         log_level: Union[int, str],
-        data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
+        # data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
         asr_train_config: Optional[str],
         asr_model_file: Optional[str],
-        cmvn_file: Optional[str],
-        beam_search_config: Optional[dict],
-        lm_train_config: Optional[str],
-        lm_file: Optional[str],
-        model_tag: Optional[str],
-        token_type: Optional[str],
-        bpemodel: Optional[str],
-        key_file: Optional[str],
-        allow_variable_data_keys: bool,
-        quantize_asr_model: Optional[bool],
-        quantize_modules: Optional[List[str]],
-        quantize_dtype: Optional[str],
-        streaming: Optional[bool],
-        simu_streaming: Optional[bool],
-        chunk_size: Optional[int],
-        left_context: Optional[int],
-        right_context: Optional[int],
-        display_partial_hypotheses: bool,
+        cmvn_file: Optional[str] = None,
+        beam_search_config: Optional[dict] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        model_tag: Optional[str] = None,
+        token_type: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        key_file: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        quantize_asr_model: Optional[bool] = False,
+        quantize_modules: Optional[List[str]] = None,
+        quantize_dtype: Optional[str] = "float16",
+        streaming: Optional[bool] = False,
+        simu_streaming: Optional[bool] = False,
+        chunk_size: Optional[int] = 16,
+        left_context: Optional[int] = 16,
+        right_context: Optional[int] = 0,
+        display_partial_hypotheses: bool = False,
         **kwargs,
 ) -> None:
     """Transducer model inference.
     Args:
         output_dir: Output directory path.
         batch_size: Batch decoding size.
         dtype: Data type.
@@ -1365,15 +1367,18 @@
         quantize_dtype=quantize_dtype,
         streaming=streaming,
         simu_streaming=simu_streaming,
         chunk_size=chunk_size,
         left_context=left_context,
         right_context=right_context,
     )
-    speech2text = Speech2TextTransducer(**speech2text_kwargs)
+    speech2text = Speech2TextTransducer.from_pretrained(
+        model_tag=model_tag,
+        **speech2text_kwargs,
+    )
 
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
@@ -1384,64 +1389,74 @@
             preprocess_args=speech2text.asr_train_args,
             data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
         )
+        asr_result_list = []
+
+        if output_dir is not None:
+            writer = DatadirWriter(output_dir)
+        else:
+            writer = None
 
         # 4 .Start for-loop
-        with DatadirWriter(output_dir) as writer:
-            for keys, batch in loader:
-                assert isinstance(batch, dict), type(batch)
-                assert all(isinstance(s, str) for s in keys), keys
-
-                _bs = len(next(iter(batch.values())))
-                assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-                batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-                assert len(batch.keys()) == 1
-
-                try:
-                    if speech2text.streaming:
-                        speech = batch["speech"]
-
-                        _steps = len(speech) // speech2text._ctx
-                        _end = 0
-                        for i in range(_steps):
-                            _end = (i + 1) * speech2text._ctx
-
-                            speech2text.streaming_decode(
-                                speech[i * speech2text._ctx: _end], is_final=False
-                            )
+        for keys, batch in loader:
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+            batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
+            assert len(batch.keys()) == 1
+
+            try:
+                if speech2text.streaming:
+                    speech = batch["speech"]
 
-                        final_hyps = speech2text.streaming_decode(
-                            speech[_end: len(speech)], is_final=True
+                    _steps = len(speech) // speech2text._ctx
+                    _end = 0
+                    for i in range(_steps):
+                        _end = (i + 1) * speech2text._ctx
+
+                        speech2text.streaming_decode(
+                            speech[i * speech2text._ctx: _end], is_final=False
                         )
-                    elif speech2text.simu_streaming:
-                        final_hyps = speech2text.simu_streaming_decode(**batch)
-                    else:
-                        final_hyps = speech2text(**batch)
-
-                    results = speech2text.hypotheses_to_results(final_hyps)
-                except TooShortUttError as e:
-                    logging.warning(f"Utterance {keys} {e}")
-                    hyp = Hypothesis(score=0.0, yseq=[], dec_state=None)
-                    results = [[" ", ["<space>"], [2], hyp]] * nbest
 
-                key = keys[0]
-                for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
+                    final_hyps = speech2text.streaming_decode(
+                        speech[_end: len(speech)], is_final=True
+                    )
+                elif speech2text.simu_streaming:
+                    final_hyps = speech2text.simu_streaming_decode(**batch)
+                else:
+                    final_hyps = speech2text(**batch)
+
+                results = speech2text.hypotheses_to_results(final_hyps)
+            except TooShortUttError as e:
+                logging.warning(f"Utterance {keys} {e}")
+                hyp = Hypothesis(score=0.0, yseq=[], dec_state=None)
+                results = [[" ", ["<space>"], [2], hyp]] * nbest
+
+            key = keys[0]
+            for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
+                item = {'key': key, 'value': text}
+                asr_result_list.append(item)
+                if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
 
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
 
                     if text is not None:
                         ibest_writer["text"][key] = text
 
+                logging.info("decoding, utt: {}, predictions: {}".format(key, text))
+        return asr_result_list
     return _forward
 
 
 def inference_sa_asr(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
```

### Comparing `funasr-0.6.9/funasr/bin/asr_train.py` & `funasr-0.7.0/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/build_trainer.py` & `funasr-0.7.0/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/data2vec_train.py` & `funasr-0.7.0/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/diar_infer.py` & `funasr-0.7.0/funasr/bin/diar_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/diar_inference_launch.py` & `funasr-0.7.0/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/diar_train.py` & `funasr-0.7.0/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/lm_inference_launch.py` & `funasr-0.7.0/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/lm_train.py` & `funasr-0.7.0/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/punc_infer.py` & `funasr-0.7.0/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/punc_inference_launch.py` & `funasr-0.7.0/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/punc_train.py` & `funasr-0.7.0/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/sa_asr_train.py` & `funasr-0.7.0/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/sv_infer.py` & `funasr-0.7.0/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/sv_inference_launch.py` & `funasr-0.7.0/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/tokenize_text.py` & `funasr-0.7.0/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/tp_infer.py` & `funasr-0.7.0/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/tp_inference_launch.py` & `funasr-0.7.0/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/train.py` & `funasr-0.7.0/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/vad_infer.py` & `funasr-0.7.0/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/bin/vad_inference_launch.py` & `funasr-0.7.0/funasr/bin/vad_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             for i, _ in enumerate(keys):
                 if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
                     results[i] = json.dumps(results[i])
                 item = {'key': keys[i], 'value': results[i]}
                 vad_results.append(item)
                 if writer is not None:
                     ibest_writer["text"][keys[i]] = "{}".format(results[i])
-
+        torch.cuda.empty_cache()
         return vad_results
 
     return _forward
 
 
 def inference_vad_online(
         batch_size: int,
```

### Comparing `funasr-0.6.9/funasr/build_utils/build_args.py` & `funasr-0.7.0/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_asr_model.py` & `funasr-0.7.0/funasr/build_utils/build_asr_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
 from funasr.models.encoder.resnet34_encoder import ResNet34Diar
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
+from funasr.models.encoder.branchformer_encoder import BranchformerEncoder
+from funasr.models.encoder.e_branchformer_encoder import EBranchformerEncoder
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.default import MultiChannelFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.windowing import SlidingWindow
@@ -109,14 +111,16 @@
     classes=dict(
         conformer=ConformerEncoder,
         transformer=TransformerEncoder,
         rnn=RNNEncoder,
         sanm=SANMEncoder,
         sanm_chunk_opt=SANMEncoderChunkOpt,
         data2vec_encoder=Data2VecEncoder,
+        branchformer=BranchformerEncoder,
+        e_branchformer=EBranchformerEncoder,
         mfcca_enc=MFCCAEncoder,
         chunk_conformer=ConformerChunkEncoder,
     ),
     default="rnn",
 )
 asr_encoder_choices = ClassChoices(
     "asr_encoder",
```

### Comparing `funasr-0.6.9/funasr/build_utils/build_dataloader.py` & `funasr-0.7.0/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_diar_model.py` & `funasr-0.7.0/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_distributed.py` & `funasr-0.7.0/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_lm_model.py` & `funasr-0.7.0/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_model.py` & `funasr-0.7.0/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_model_from_file.py` & `funasr-0.7.0/funasr/build_utils/build_model_from_file.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_optimizer.py` & `funasr-0.7.0/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_pretrain_model.py` & `funasr-0.7.0/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_punc_model.py` & `funasr-0.7.0/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_scheduler.py` & `funasr-0.7.0/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_streaming_iterator.py` & `funasr-0.7.0/funasr/build_utils/build_streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_sv_model.py` & `funasr-0.7.0/funasr/build_utils/build_sv_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_trainer.py` & `funasr-0.7.0/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/build_utils/build_vad_model.py` & `funasr-0.7.0/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/collate_fn.py` & `funasr-0.7.0/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/dataset.py` & `funasr-0.7.0/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/iterable_dataset.py` & `funasr-0.7.0/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.7.0/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.7.0/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.7.0/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/dataset.py` & `funasr-0.7.0/funasr/datasets/large_datasets/dataset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -225,23 +225,23 @@
                            data_types, 
                            frontend_conf=frontend_conf, 
                            shuffle=shuffle,
                            speed_perturb=speed_perturb,
                            mode=mode, 
                            )
 
-    filter_conf = conf.get('filter_conf', {})
-    filter_fn = partial(filter, **filter_conf)
-    dataset = FilterIterDataPipe(dataset, fn=filter_fn)
-
     if "text" in data_names:
         vocab = {'vocab': dict, 'seg_dict': seg_dict, 'punc_dict': punc_dict, 'bpe_tokenizer': bpe_tokenizer, 'hw_config': hw_config}
         tokenize_fn = partial(tokenize, **vocab)
         dataset = MapperIterDataPipe(dataset, fn=tokenize_fn)
 
+    filter_conf = conf.get('filter_conf', {})
+    filter_fn = partial(filter, **filter_conf)
+    dataset = FilterIterDataPipe(dataset, fn=filter_fn)
+
     if shuffle:
         buffer_conf = conf.get('shuffle_conf', {})
         buffer_size = buffer_conf['shuffle_size']
         sort_size = buffer_conf['sort_size']
     else:
         buffer_size = 0
         sort_size = 1
```

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.7.0/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/ms_dataset.py` & `funasr-0.7.0/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/preprocessor.py` & `funasr-0.7.0/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/small_datasets/collate_fn.py` & `funasr-0.7.0/funasr/datasets/small_datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/small_datasets/dataset.py` & `funasr-0.7.0/funasr/datasets/small_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/small_datasets/length_batch_sampler.py` & `funasr-0.7.0/funasr/datasets/small_datasets/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/small_datasets/preprocessor.py` & `funasr-0.7.0/funasr/datasets/small_datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/datasets/small_datasets/sequence_iter_factory.py` & `funasr-0.7.0/funasr/datasets/small_datasets/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/export_model.py` & `funasr-0.7.0/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/CT_Transformer.py` & `funasr-0.7.0/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/__init__.py` & `funasr-0.7.0/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.7.0/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.7.0/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.7.0/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/e2e_vad.py` & `funasr-0.7.0/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.7.0/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.7.0/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.7.0/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/modules/decoder_layer.py` & `funasr-0.7.0/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/modules/encoder_layer.py` & `funasr-0.7.0/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/modules/feedforward.py` & `funasr-0.7.0/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/modules/multihead_att.py` & `funasr-0.7.0/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/models/predictor/cif.py` & `funasr-0.7.0/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/test/test_onnx.py` & `funasr-0.7.0/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/test/test_onnx_punc.py` & `funasr-0.7.0/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.7.0/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/test/test_onnx_vad.py` & `funasr-0.7.0/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/export/utils/torch_function.py` & `funasr-0.7.0/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/fileio/datadir_writer.py` & `funasr-0.7.0/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/fileio/npy_scp.py` & `funasr-0.7.0/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/fileio/rand_gen_dataset.py` & `funasr-0.7.0/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/fileio/read_text.py` & `funasr-0.7.0/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/fileio/sound_scp.py` & `funasr-0.7.0/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/iterators/chunk_iter_factory.py` & `funasr-0.7.0/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/iterators/multiple_iter_factory.py` & `funasr-0.7.0/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/iterators/sequence_iter_factory.py` & `funasr-0.7.0/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/complex_utils.py` & `funasr-0.7.0/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/global_mvn.py` & `funasr-0.7.0/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/label_aggregation.py` & `funasr-0.7.0/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/log_mel.py` & `funasr-0.7.0/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/mask_along_axis.py` & `funasr-0.7.0/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/sinc_conv.py` & `funasr-0.7.0/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/stft.py` & `funasr-0.7.0/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/time_warp.py` & `funasr-0.7.0/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/layers/utterance_mvn.py` & `funasr-0.7.0/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/losses/label_smoothing_loss.py` & `funasr-0.7.0/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/main_funcs/average_nbest_models.py` & `funasr-0.7.0/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.7.0/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/main_funcs/collect_stats.py` & `funasr-0.7.0/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/main_funcs/pack_funcs.py` & `funasr-0.7.0/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/ctc.py` & `funasr-0.7.0/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/data2vec.py` & `funasr-0.7.0/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/contextual_decoder.py` & `funasr-0.7.0/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/rnn_decoder.py` & `funasr-0.7.0/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.7.0/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/sanm_decoder.py` & `funasr-0.7.0/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/sv_decoder.py` & `funasr-0.7.0/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/decoder/transformer_decoder.py` & `funasr-0.7.0/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr.py` & `funasr-0.7.0/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_bat.py` & `funasr-0.7.0/funasr/models/e2e_asr_bat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_common.py` & `funasr-0.7.0/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.7.0/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_mfcca.py` & `funasr-0.7.0/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_paraformer.py` & `funasr-0.7.0/funasr/models/e2e_asr_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2103,15 +2103,15 @@
             cer_att, wer_att = None, None
         else:
             ys_hat = decoder_out_1st.argmax(dim=-1)
             cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
 
         return loss_att, acc_att, cer_att, wer_att, loss_pre
 
-    def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, hw_list=None):
+    def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, hw_list=None, clas_scale=1.0):
         if hw_list is None:
             # default hotword list
             hw_list = [torch.Tensor([self.sos]).long().to(encoder_out.device)]  # empty hotword list
             hw_list_pad = pad_list(hw_list, 0)
             if self.use_decoder_embedding:
                 hw_embed = self.decoder.embed(hw_list_pad)
             else:
```

### Comparing `funasr-0.6.9/funasr/models/e2e_asr_transducer.py` & `funasr-0.7.0/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.7.0/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_diar_sond.py` & `funasr-0.7.0/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_sa_asr.py` & `funasr-0.7.0/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_sv.py` & `funasr-0.7.0/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_tp.py` & `funasr-0.7.0/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_uni_asr.py` & `funasr-0.7.0/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/e2e_vad.py` & `funasr-0.7.0/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/conformer_encoder.py` & `funasr-0.7.0/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.7.0/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.7.0/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.7.0/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.7.0/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.7.0/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.7.0/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/rnn_encoder.py` & `funasr-0.7.0/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/sanm_encoder.py` & `funasr-0.7.0/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/encoder/transformer_encoder.py` & `funasr-0.7.0/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/default.py` & `funasr-0.7.0/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.7.0/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/fused.py` & `funasr-0.7.0/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/s3prl.py` & `funasr-0.7.0/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/wav_frontend.py` & `funasr-0.7.0/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.7.0/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/frontend/windowing.py` & `funasr-0.7.0/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/joint_net/joint_network.py` & `funasr-0.7.0/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/pooling/statistic_pooling.py` & `funasr-0.7.0/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.7.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/predictor/cif.py` & `funasr-0.7.0/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/preencoder/linear.py` & `funasr-0.7.0/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/preencoder/sinc.py` & `funasr-0.7.0/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/seq_rnn_lm.py` & `funasr-0.7.0/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/specaug/specaug.py` & `funasr-0.7.0/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/target_delay_transformer.py` & `funasr-0.7.0/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/transformer_lm.py` & `funasr-0.7.0/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/models/vad_realtime_transformer.py` & `funasr-0.7.0/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/add_sos_eos.py` & `funasr-0.7.0/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/attention.py` & `funasr-0.7.0/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.7.0/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.7.0/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/beam_search/beam_search.py` & `funasr-0.7.0/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.7.0/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.7.0/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/data_utils.py` & `funasr-0.7.0/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/ema_module.py` & `funasr-0.7.0/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.7.0/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/quant_noise.py` & `funasr-0.7.0/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/utils.py` & `funasr-0.7.0/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.7.0/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/dynamic_conv.py` & `funasr-0.7.0/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/dynamic_conv2d.py` & `funasr-0.7.0/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/e2e_asr_common.py` & `funasr-0.7.0/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/eend_ola/encoder.py` & `funasr-0.7.0/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.7.0/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/eend_ola/utils/losses.py` & `funasr-0.7.0/funasr/modules/eend_ola/utils/losses.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/eend_ola/utils/power.py` & `funasr-0.7.0/funasr/modules/eend_ola/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/eend_ola/utils/report.py` & `funasr-0.7.0/funasr/modules/eend_ola/utils/report.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/embedding.py` & `funasr-0.7.0/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/beamformer.py` & `funasr-0.7.0/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.7.0/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.7.0/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/feature_transform.py` & `funasr-0.7.0/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/frontend.py` & `funasr-0.7.0/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/frontends/mask_estimator.py` & `funasr-0.7.0/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/layer_norm.py` & `funasr-0.7.0/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/lightconv.py` & `funasr-0.7.0/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/lightconv2d.py` & `funasr-0.7.0/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/mask.py` & `funasr-0.7.0/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/multi_layer_conv.py` & `funasr-0.7.0/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/nets_utils.py` & `funasr-0.7.0/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/positionwise_feed_forward.py` & `funasr-0.7.0/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/repeat.py` & `funasr-0.7.0/funasr/modules/repeat.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,46 @@
 from funasr.modules.layer_norm import LayerNorm
 import torch
 
 
 class MultiSequential(torch.nn.Sequential):
     """Multi-input multi-output torch.nn.Sequential."""
 
+    def __init__(self, *args, layer_drop_rate=0.0):
+        """Initialize MultiSequential with layer_drop.
+
+        Args:
+            layer_drop_rate (float): Probability of dropping out each fn (layer).
+
+        """
+        super(MultiSequential, self).__init__(*args)
+        self.layer_drop_rate = layer_drop_rate
+
     def forward(self, *args):
         """Repeat."""
-        for m in self:
-            args = m(*args)
+        _probs = torch.empty(len(self)).uniform_()
+        for idx, m in enumerate(self):
+            if not self.training or (_probs[idx] >= self.layer_drop_rate):
+                args = m(*args)
         return args
 
 
-def repeat(N, fn):
+def repeat(N, fn, layer_drop_rate=0.0):
     """Repeat module N times.
 
     Args:
         N (int): Number of repeat time.
         fn (Callable): Function to generate module.
+        layer_drop_rate (float): Probability of dropping out each fn (layer).
 
     Returns:
         MultiSequential: Repeated model instance.
 
     """
-    return MultiSequential(*[fn(n) for n in range(N)])
+    return MultiSequential(*[fn(n) for n in range(N)], layer_drop_rate=layer_drop_rate)
 
 
 class MultiBlocks(torch.nn.Module):
     """MultiBlocks definition.
     Args:
         block_list: Individual blocks of the encoder architecture.
         output_size: Architecture output size.
```

### Comparing `funasr-0.6.9/funasr/modules/rnn/argument.py` & `funasr-0.7.0/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/rnn/attentions.py` & `funasr-0.7.0/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/rnn/decoders.py` & `funasr-0.7.0/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/rnn/encoders.py` & `funasr-0.7.0/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/scorers/ctc.py` & `funasr-0.7.0/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.7.0/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/scorers/length_bonus.py` & `funasr-0.7.0/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/scorers/scorer_interface.py` & `funasr-0.7.0/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.7.0/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.7.0/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/streaming_utils/utils.py` & `funasr-0.7.0/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/subsampling.py` & `funasr-0.7.0/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/modules/subsampling_without_posenc.py` & `funasr-0.7.0/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/optimizers/fairseq_adam.py` & `funasr-0.7.0/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/optimizers/sgd.py` & `funasr-0.7.0/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/demo.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/libtorch/setup.py` & `funasr-0.7.0/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.7.0/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/build_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/folded_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/length_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.7.0/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/schedulers/abs_scheduler.py` & `funasr-0.7.0/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/schedulers/noam_lr.py` & `funasr-0.7.0/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.7.0/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/schedulers/warmup_lr.py` & `funasr-0.7.0/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/abs_task.py` & `funasr-0.7.0/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/asr.py` & `funasr-0.7.0/funasr/tasks/asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1534,15 +1534,14 @@
         """Required data depending on task mode.
         Args:
             cls: ASRBATTask object.
             args: Task arguments.
         Return:
             model: ASR BAT model.
         """
-        assert check_argument_types()
 
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
```

### Comparing `funasr-0.6.9/funasr/tasks/data2vec.py` & `funasr-0.7.0/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/diar.py` & `funasr-0.7.0/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/lm.py` & `funasr-0.7.0/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/punctuation.py` & `funasr-0.7.0/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/sa_asr.py` & `funasr-0.7.0/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/sv.py` & `funasr-0.7.0/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/tasks/vad.py` & `funasr-0.7.0/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/build_tokenizer.py` & `funasr-0.7.0/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/char_tokenizer.py` & `funasr-0.7.0/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/cleaner.py` & `funasr-0.7.0/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/korean_cleaner.py` & `funasr-0.7.0/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/phoneme_tokenizer.py` & `funasr-0.7.0/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.7.0/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/token_id_converter.py` & `funasr-0.7.0/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/text/word_tokenizer.py` & `funasr-0.7.0/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.7.0/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/device_funcs.py` & `funasr-0.7.0/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/forward_adaptor.py` & `funasr-0.7.0/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/initialize.py` & `funasr-0.7.0/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.7.0/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/model_summary.py` & `funasr-0.7.0/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/torch_utils/recursive_op.py` & `funasr-0.7.0/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/train/abs_model.py` & `funasr-0.7.0/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/train/class_choices.py` & `funasr-0.7.0/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/train/distributed_utils.py` & `funasr-0.7.0/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/train/reporter.py` & `funasr-0.7.0/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/train/trainer.py` & `funasr-0.7.0/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/asr_env_checking.py` & `funasr-0.7.0/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/asr_utils.py` & `funasr-0.7.0/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/cli_utils.py` & `funasr-0.7.0/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/compute_eer.py` & `funasr-0.7.0/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/compute_min_dcf.py` & `funasr-0.7.0/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/compute_wer.py` & `funasr-0.7.0/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/config_argparse.py` & `funasr-0.7.0/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/get_default_kwargs.py` & `funasr-0.7.0/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/griffin_lim.py` & `funasr-0.7.0/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/job_runner.py` & `funasr-0.7.0/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/misc.py` & `funasr-0.7.0/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/modelscope_param.py` & `funasr-0.7.0/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/modelscope_utils.py` & `funasr-0.7.0/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/nested_dict_action.py` & `funasr-0.7.0/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/postprocess_utils.py` & `funasr-0.7.0/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/prepare_data.py` & `funasr-0.7.0/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/runtime_sdk_download_tool.py` & `funasr-0.7.0/funasr/utils/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/sized_dict.py` & `funasr-0.7.0/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/timestamp_tools.py` & `funasr-0.7.0/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/types.py` & `funasr-0.7.0/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/vad_utils.py` & `funasr-0.7.0/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr/utils/wav_utils.py` & `funasr-0.7.0/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/funasr.egg-info/PKG-INFO` & `funasr-0.7.0/funasr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.9
+Version: 0.7.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,21 +35,21 @@
 </p>
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Usage**](#usage)
-| [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
-| [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
+| [**Quick Start**](#quick-start)
+| [**Runtime**](./funasr/runtime/readme.md)
+| [**Model Zoo**](./docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
-| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
+
+<a name="whats-new"></a>
 ## What's new: 
 
 ### FunASR runtime-SDK
 
 - 2023.07.03: 
 We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 
@@ -57,19 +57,21 @@
 
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 
 ### Release notes
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
+<a name="highlights"></a>
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
+<a name="Installation"></a>
 ## Installation
 
 Install from pip
 ```shell
 pip3 install -U funasr
 # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple
@@ -91,15 +93,16 @@
 pip3 install -U modelscope
 # For the users in China, you could install with the command:
 # pip3 install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
 For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-## Usage
+<a name="quick-start"></a>
+## Quick Start
 
 You could use FunASR by:
 
 - egs
 - egs_modelscope
 - runtime
 
@@ -141,14 +144,16 @@
 
 For the client:
 ```shell
 python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
 #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
+
+<a name="contact"></a>
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
 
 |Dingding group |                     Wechat group                      |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.9 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.7.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -22,32 +22,28 @@
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
-[**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
-FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
-FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
-[**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+[**Quick Start**](#quick-start) | [**Runtime**](./funasr/runtime/readme.md) |
+[**Model Zoo**](./docs/model_zoo/modelscope_models.md) | [**Contact**]
+(#contact)  ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
 the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
 supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
 are pleased to announce that the M2MeT2.0 challenge has been accepted by the
 ASRU 2023 challenge special session. The registration is now open. The baseline
 system is conducted on FunASR and is provided as a receipe of AliMeeting
 corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
 alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-
-academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+academy/FunASR/releases)  ## Highlights - FunASR is a fundamental speech
 recognition toolkit that offers a variety of features, including speech
 recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
 Language Models, Speaker Verification, Speaker diarization and multi-talker
 ASR. - We have released a vast collection of academic and industrial pretrained
 models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
 speech-recognition), which can be accessed through our [Model Zoo](https://
 github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
@@ -55,49 +51,49 @@
 www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
 vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
 recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
 pretrained models from the [ModelScope](https://www.modelscope.cn/
 models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
 dataloader in FunASR enables faster training speeds for large-scale datasets.
 This feature enhances the efficiency of the speech recognition process for
-researchers and practitioners. ## Installation Install from pip ```shell pip3
+researchers and practitioners.  ## Installation Install from pip ```shell pip3
 install -U funasr # For the users in China, you could install with the command:
 # pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
 install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
 && cd FunASR pip3 install -e ./ # For the users in China, you could install
 with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
 simple ``` If you want to use the pretrained models in ModelScope, you should
 install the modelscope: ```shell pip3 install -U modelscope # For the users in
 China, you could install with the command: # pip3 install -U modelscope -
 f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
 mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
 [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
-installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
-runtime ### egs If you want to train the model from scratch, you could use
-funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
-. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
-found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
-modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
-or finetune pretraining models from modelscope, you could use funasr by
-modelscope pipeline, as the following: ```python from modelscope.pipelines
+installation.html)  ## Quick Start You could use FunASR by: - egs -
+egs_modelscope - runtime ### egs If you want to train the model from scratch,
+you could use funasr directly by recipe, as the following: ```shell cd egs/
+aishell/paraformer . ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More
+examples could be found in [docs](https://alibaba-damo-academy.github.io/
+FunASR/en/modelscope_pipeline/quick_start.html) ### egs_modelscope If you want
+to infer or finetune pretraining models from modelscope, you could use funasr
+by modelscope pipeline, as the following: ```python from modelscope.pipelines
 import pipeline from modelscope.utils.constant import Tasks inference_pipeline
 = pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
 funasr_wss_server.py --port 10095 ``` For the client: ```shell python
 funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
 "5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ``` More examples could be found in [docs](https://alibaba-damo-
-academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2)  ## Contact If
 you have any questions about FunASR, please contact us by - email:
 [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
 Wechat group | |:---:|:-----------------------------------------------------:
 | |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
```

### Comparing `funasr-0.6.9/funasr.egg-info/SOURCES.txt` & `funasr-0.7.0/funasr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -160,16 +160,18 @@
 funasr/models/decoder/rnn_decoder.py
 funasr/models/decoder/rnnt_decoder.py
 funasr/models/decoder/sanm_decoder.py
 funasr/models/decoder/sv_decoder.py
 funasr/models/decoder/transformer_decoder.py
 funasr/models/encoder/__init__.py
 funasr/models/encoder/abs_encoder.py
+funasr/models/encoder/branchformer_encoder.py
 funasr/models/encoder/conformer_encoder.py
 funasr/models/encoder/data2vec_encoder.py
+funasr/models/encoder/e_branchformer_encoder.py
 funasr/models/encoder/ecapa_tdnn_encoder.py
 funasr/models/encoder/encoder_layer_mfcca.py
 funasr/models/encoder/fsmn_encoder.py
 funasr/models/encoder/mfcca_encoder.py
 funasr/models/encoder/resnet34_encoder.py
 funasr/models/encoder/rnn_encoder.py
 funasr/models/encoder/sanm_encoder.py
@@ -203,18 +205,20 @@
 funasr/models/preencoder/sinc.py
 funasr/models/specaug/__init__.py
 funasr/models/specaug/abs_specaug.py
 funasr/models/specaug/specaug.py
 funasr/modules/__init__.py
 funasr/modules/add_sos_eos.py
 funasr/modules/attention.py
+funasr/modules/cgmlp.py
 funasr/modules/dynamic_conv.py
 funasr/modules/dynamic_conv2d.py
 funasr/modules/e2e_asr_common.py
 funasr/modules/embedding.py
+funasr/modules/fastformer.py
 funasr/modules/layer_norm.py
 funasr/modules/lightconv.py
 funasr/modules/lightconv2d.py
 funasr/modules/mask.py
 funasr/modules/multi_layer_conv.py
 funasr/modules/nets_utils.py
 funasr/modules/positionwise_feed_forward.py
```

### Comparing `funasr-0.6.9/funasr.egg-info/requires.txt` & `funasr-0.7.0/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/setup.py` & `funasr-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_asr_inference_pipeline.py` & `funasr-0.7.0/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.7.0/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_lm_pipeline.py` & `funasr-0.7.0/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_punctuation_pipeline.py` & `funasr-0.7.0/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_sv_inference_pipeline.py` & `funasr-0.7.0/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_tp_pipeline.py` & `funasr-0.7.0/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.9/tests/test_vad_inference_pipeline.py` & `funasr-0.7.0/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

