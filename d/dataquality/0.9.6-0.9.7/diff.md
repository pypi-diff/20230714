# Comparing `tmp/dataquality-0.9.6.tar.gz` & `tmp/dataquality-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.6.tar", last modified: Mon Jul 10 22:50:35 2023, max compression
+gzip compressed data, was "dataquality-0.9.7.tar", last modified: Fri Jul 14 21:09:18 2023, max compression
```

## Comparing `dataquality-0.9.6.tar` & `dataquality-0.9.7.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.926672 dataquality-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 22:49:08.000000 dataquality-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-10 22:50:35.926672 dataquality-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-10 22:49:08.000000 dataquality-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.874673 dataquality-0.9.6/dataquality/
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.878673 dataquality-0.9.6/dataquality/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/clients/objectstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.878673 dataquality-0.9.6/dataquality/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/core/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.882673 dataquality-0.9.6/dataquality/dq_auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_auto/text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.882673 dataquality-0.9.6/dataquality/dq_start/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dq_start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.886673 dataquality-0.9.6/dataquality/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/integrations/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.886673 dataquality-0.9.6/dataquality/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/base_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.890673 dataquality-0.9.6/dataquality/loggers/data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/data_logger/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.894673 dataquality-0.9.6/dataquality/loggers/logger_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/logger_config/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.898673 dataquality-0.9.6/dataquality/loggers/model_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.906673 dataquality-0.9.6/dataquality/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/schemas/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.914672 dataquality-0.9.6/dataquality/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/ampli.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/auto_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/dq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/hdf5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/hf_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/od.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.918672 dataquality-0.9.6/dataquality/utils/semantic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/vaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 22:49:08.000000 dataquality-0.9.6/dataquality/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.874673 dataquality-0.9.6/dataquality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 22:50:35.000000 dataquality-0.9.6/dataquality.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-10 22:49:08.000000 dataquality-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 22:50:35.926672 dataquality-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:49:08.000000 dataquality-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.918672 dataquality-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_dataquality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_telemetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:50:35.926672 dataquality-0.9.6/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/ner_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-10 22:49:08.000000 dataquality-0.9.6/tests/test_utils/tc_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 21:08:51.000000 dataquality-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-14 21:09:18.336846 dataquality-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-14 21:08:51.000000 dataquality-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/dq_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/dq_start/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/loggers/data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/loggers/logger_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/loggers/model_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/dataquality/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ampli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/dq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hf_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/od.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/vaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-14 21:08:51.000000 dataquality-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 21:09:18.336846 dataquality-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:08:51.000000 dataquality-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_dataquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_telemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/ner_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.9.6/LICENSE` & `dataquality-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/PKG-INFO` & `dataquality-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.6
+Version: 0.9.7
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.6/README.md` & `dataquality-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/__init__.py` & `dataquality-0.9.7/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
 
-__version__ = "0.9.6"
+__version__ = "0.9.7"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.6/dataquality/analytics.py` & `dataquality-0.9.7/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/clients/api.py` & `dataquality-0.9.7/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/clients/objectstore.py` & `dataquality-0.9.7/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/__init__.py` & `dataquality-0.9.7/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/_config.py` & `dataquality-0.9.7/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/auth.py` & `dataquality-0.9.7/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/finish.py` & `dataquality-0.9.7/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/init.py` & `dataquality-0.9.7/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/log.py` & `dataquality-0.9.7/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/core/report.py` & `dataquality-0.9.7/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/auto.py` & `dataquality-0.9.7/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.7/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/ner.py` & `dataquality-0.9.7/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.7/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/notebook.py` & `dataquality-0.9.7/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.7/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.7/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dq_start/__init__.py` & `dataquality-0.9.7/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/dqyolo.py` & `dataquality-0.9.7/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/fastai.py` & `dataquality-0.9.7/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/hf.py` & `dataquality-0.9.7/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/keras.py` & `dataquality-0.9.7/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/setfit.py` & `dataquality-0.9.7/dataquality/integrations/setfit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import io
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
+import os
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import pandas as pd
 import torch
 from datasets import Dataset, DatasetDict
 
 import dataquality as dq
 from dataquality.analytics import Analytics
@@ -32,14 +33,62 @@
 a.log_import("setfit")
 
 
 if TYPE_CHECKING:
     from setfit import SetFitModel, SetFitTrainer
 
 
+class Evaluate:
+    """Call function to evaluate SetFit model and log input and output to Galileo."""
+
+    def __init__(self, model: "SetFitModel", dq_store: Dict) -> None:
+        self.model = model
+        self.dq_store = dq_store
+
+    def __call__(
+        self,
+        dataset: Dataset,
+        split: Split,
+        meta: Optional[List] = None,
+        inference_name: Optional[str] = None,
+        column_mapping: Optional[Dict] = None,
+        batch_size: int = 64,
+        epoch: Optional[int] = None,
+    ) -> torch.Tensor:
+        """Evaluate SetFit model and log input and output to Galileo.
+        :param batch: batch of data as a dictionary
+        :param split: split of data (training, validation, test, inference)
+        :param meta: columns that should be logged as metadata
+        :param inference_name: inference name (if split is inference, must be provided)
+        :param column_mapping: mapping of column names (if different from default)
+        :return: output of SetFitModel.predict_proba function"""
+        a.log_function("setfit/evaluate")
+        column_mapping = column_mapping or dict(
+            id="id",
+            text="text",
+            label="label",
+        )
+        dataset = _apply_column_mapping(dataset, column_mapping)
+        if "id" not in dataset.features:
+            dataset = dataset.map(lambda x, idx: {"id": idx}, with_indices=True)
+        if epoch is not None:
+            dq.set_epoch(epoch)
+        cur_epoch = get_data_logger().logger_config.cur_epoch
+        return log_preds_setfit(
+            model=self.model,
+            dataset=dataset,
+            dq_store=self.dq_store,
+            batch_size=batch_size,
+            split=split,
+            inference_name=inference_name,
+            meta=meta,
+            epoch=cur_epoch,
+        )
+
+
 def unwatch(setfit_obj: Optional[Union["SetFitModel", "SetFitTrainer"]]) -> None:
     """Unpatch SetFit model by replacing predict_proba function with original
     function.
     :param setfit_obj: SetFitModel or SetFitTrainer
     """
     a.log_function("setfit/unwatch")
     setfitmanager = PatchManager()
@@ -55,15 +104,15 @@
     project_name: str = "",
     run_name: str = "",
     finish: bool = True,
     wait: bool = False,
     batch_size: Optional[int] = None,
     meta: Optional[List] = None,
     validate_before_training: bool = False,
-) -> Callable:
+) -> Evaluate:
     """Watch a SetFit model or trainer and extract model outputs for dataquality.
     Returns a function that can be used to evaluate the model on a dataset.
     :param setfit: SetFit model or trainer
     :param labels: list of labels
     :param project_name: name of project
     :param run_name: name of run
     :param finish: whether to run dq.finish after evaluation
@@ -120,64 +169,23 @@
         assert labels and len(
             labels
         ), "Labels must be set (watch(trainer, labels=[...]))"
         dq.set_labels_for_run(labels)
         return evaluate(model)
 
 
-def evaluate(
-    model: "SetFitModel",
-) -> Callable:
+def evaluate(model: "SetFitModel") -> Evaluate:
     """Watch SetFit model by replacing predict_proba function with SetFitModelHook.
     :param model: SetFit model
     :return: SetFitModelHook object"""
 
-    dq_hook = SetFitModelHook(model)
-    dq_store = dq_hook.store
-
-    def dq_evaluate(
-        dataset: Dataset,
-        split: Split,
-        meta: Optional[List] = None,
-        inference_name: Optional[str] = None,
-        column_mapping: Optional[Dict] = None,
-        batch_size: int = 64,
-        epoch: Optional[int] = None,
-    ) -> torch.Tensor:
-        """Evaluate SetFit model and log input and output to Galileo.
-        :param batch: batch of data as a dictionary
-        :param split: split of data (training, validation, test, inference)
-        :param meta: columns that should be logged as metadata
-        :param inference_name: inference name (if split is inference, must be provided)
-        :param column_mapping: mapping of column names (if different from default)
-        :return: output of SetFitModel.predict_proba function"""
-        a.log_function("setfit/evaluate")
-        column_mapping = column_mapping or dict(
-            id="id",
-            text="text",
-            label="label",
-        )
-        dataset = _apply_column_mapping(dataset, column_mapping)
-        if "id" not in dataset.features:
-            dataset = dataset.map(lambda x, idx: {"id": idx}, with_indices=True)
-        if epoch is not None:
-            dq.set_epoch(epoch)
-        cur_epoch = get_data_logger().logger_config.cur_epoch
-        return log_preds_setfit(
-            model=model,
-            dataset=dataset,
-            dq_store=dq_store,
-            batch_size=batch_size,
-            split=split,
-            inference_name=inference_name,
-            meta=meta,
-            epoch=cur_epoch,
-        )
-
-    return dq_evaluate
+    hook = SetFitModelHook(model)
+    dq_store = hook.store
+    evaluate = Evaluate(model, dq_store)
+    return evaluate
 
 
 def auto(
     setfit_model: Union[
         "SetFitModel", str
     ] = "sentence-transformers/paraphrase-mpnet-base-v2",
     hf_data: Optional[Union[DatasetDict, str]] = None,
@@ -354,9 +362,10 @@
         dq_evaluate(
             ds,
             split=Split.inference,  # type: ignore
             inference_name=inf_name,  # type: ignore
             meta=meta_columns,
         )
 
-    dq.finish(wait=wait, create_data_embs=create_data_embs)
+    if not os.environ.get("DQ_SKIP_FINISH"):
+        dq.finish(wait=wait, create_data_embs=create_data_embs)
     return model
```

### Comparing `dataquality-0.9.6/dataquality/integrations/torch.py` & `dataquality-0.9.7/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-0.9.7/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.7/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/integrations/ultralytics.py` & `dataquality-0.9.7/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/internal.py` & `dataquality-0.9.7/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/base_logger.py` & `dataquality-0.9.7/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/seq2seq.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.7/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/seq2seq.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.7/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/seq2seq.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.7/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/metrics.py` & `dataquality-0.9.7/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/condition.py` & `dataquality-0.9.7/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/dataframe.py` & `dataquality-0.9.7/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/edit.py` & `dataquality-0.9.7/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/hf.py` & `dataquality-0.9.7/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/metrics.py` & `dataquality-0.9.7/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/ner.py` & `dataquality-0.9.7/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/report.py` & `dataquality-0.9.7/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/route.py` & `dataquality-0.9.7/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.7/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/seq2seq.py` & `dataquality-0.9.7/dataquality/schemas/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/split.py` & `dataquality-0.9.7/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/task_type.py` & `dataquality-0.9.7/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/schemas/torch.py` & `dataquality-0.9.7/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/ampli.py` & `dataquality-0.9.7/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/auto.py` & `dataquality-0.9.7/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/auto_trainer.py` & `dataquality-0.9.7/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/cuda.py` & `dataquality-0.9.7/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/cv.py` & `dataquality-0.9.7/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/dq_logger.py` & `dataquality-0.9.7/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/dqyolo.py` & `dataquality-0.9.7/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/emb.py` & `dataquality-0.9.7/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/file.py` & `dataquality-0.9.7/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/hdf5_store.py` & `dataquality-0.9.7/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/helpers.py` & `dataquality-0.9.7/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/hf_images.py` & `dataquality-0.9.7/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.7/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/keras.py` & `dataquality-0.9.7/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/ml.py` & `dataquality-0.9.7/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/name.py` & `dataquality-0.9.7/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/od.py` & `dataquality-0.9.7/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/patcher.py` & `dataquality-0.9.7/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/profiler.py` & `dataquality-0.9.7/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.7/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.7/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.7/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.7/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.7/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/seq2seq.py` & `dataquality-0.9.7/dataquality/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/setfit.py` & `dataquality-0.9.7/dataquality/utils/setfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,25 @@
     from setfit import SetFitModel, SetFitTrainer
 
 
 @dataclass
 class DataSampleLogArgs:
     split: Split
     inference_name: Optional[str] = None
-    meta: Optional[Dict] = None
+    meta: Dict = field(default_factory=dict)
     texts: List[str] = field(default_factory=list)
     ids: List[int] = field(default_factory=list)
     labels: List = field(default_factory=list)
 
     def clear(self) -> None:
         """Resets the arrays of the class."""
         self.texts.clear()
         self.ids.clear()
         self.labels.clear()
+        self.meta.clear()
 
 
 def _get_meta_cols(cols: Iterable) -> List[str]:
     """Returns the meta columns of a dataset."""
     default_cols = ["text", "label", "id"]
     meta_columns = [col for col in cols if col not in default_cols]
     return meta_columns
@@ -63,18 +64,15 @@
     :return: The predictions
     """
     text_col = "text"
     id_col = "id"
     label_col = "label"
     preds: List[Tensor] = []
     log_args: DataSampleLogArgs = DataSampleLogArgs(split=split)
-    inference_dict: Dict[str, str] = {}
-    if inference_name is not None:
-        log_args.inference_name = inference_name
-        inference_dict["inference_name"] = inference_name
+    log_args.inference_name = inference_name
 
     logger_config = dq.get_data_logger().logger_config
     labels = logger_config.labels
     epoch = epoch or 0
 
     # Check if the data should be logged by checking if the split is in the
     # input_data_logged
@@ -88,45 +86,49 @@
         assert id_col in batch, f"column '{id_col}' text must be in batch"
 
         if inference_name is None and not skip_logging:
             assert label_col in batch, f"column '{label_col}' must be in batch"
             log_args.labels += [labels[label] for label in batch[label_col]]
 
         pred = model.predict_proba(batch[text_col])
+        meta_column_batch = log_args.meta
         if return_preds:
             preds.append(pred)
         # 🔭🌕 Galileo logging
         if not skip_logging:
             log_args.texts += batch[text_col]
             log_args.ids += batch[id_col]
             if meta is not None:
-                meta_colum_batch = {}
                 for meta_col in meta:
                     if meta_col in batch:
-                        meta_colum_batch[meta_col] = batch[meta_col]
+                        if meta_col not in meta_column_batch:
+                            meta_column_batch[meta_col] = batch[meta_col]
+                        else:
+                            meta_column_batch[meta_col] += batch[meta_col]
+
                     else:
                         print(f"Meta column: {meta_col} was not found in batch")
-                if meta_colum_batch:
-                    log_args.meta = meta_colum_batch
+
             if len(log_args.texts) >= BATCH_LOG_SIZE:
                 dq.log_data_samples(**asdict(log_args))
                 log_args.clear()
         # 🔭🌕 Galileo logging
         dq.log_model_outputs(
             ids=batch[id_col],
             probs=dq_store["output"],
             embs=dq_store["input_args"][0],
             split=split,
             epoch=epoch,
-            **inference_dict,  # type: ignore
+            inference_name=inference_name,
         )
 
     # Log any leftovers
-    if log_args and not skip_logging:
+    if len(log_args.ids) and not skip_logging:
         dq.log_data_samples(**asdict(log_args))
+    log_args.clear()
     if not return_preds:
         return torch.tensor([])
     return torch.concat(preds)
 
 
 def _prepare_config() -> None:
     """
```

### Comparing `dataquality-0.9.6/dataquality/utils/thread_pool.py` & `dataquality-0.9.7/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/torch.py` & `dataquality-0.9.7/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/transformers.py` & `dataquality-0.9.7/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/ultralytics.py` & `dataquality-0.9.7/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/upload.py` & `dataquality-0.9.7/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/vaex.py` & `dataquality-0.9.7/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality/utils/version.py` & `dataquality-0.9.7/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality.egg-info/PKG-INFO` & `dataquality-0.9.7/dataquality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.6
+Version: 0.9.7
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.6/dataquality.egg-info/SOURCES.txt` & `dataquality-0.9.7/dataquality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/dataquality.egg-info/requires.txt` & `dataquality-0.9.7/dataquality.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/pyproject.toml` & `dataquality-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_dataquality.py` & `dataquality-0.9.7/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_telemetrics.py` & `dataquality-0.9.7/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/data_utils.py` & `dataquality-0.9.7/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.7/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.7/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.7/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/lightning_model.py` & `dataquality-0.9.7/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/mock_data.py` & `dataquality-0.9.7/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/mock_request.py` & `dataquality-0.9.7/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/ner_constants.py` & `dataquality-0.9.7/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.7/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.6/tests/test_utils/tc_constants.py` & `dataquality-0.9.7/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

